# Comparing `tmp/aiogram3_form-1.0.2.tar.gz` & `tmp/aiogram3_form-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_form-1.0.2.tar", max compression
+gzip compressed data, was "aiogram3_form-2.0.0.tar", max compression
```

## Comparing `aiogram3_form-1.0.2.tar` & `aiogram3_form-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2024-03-07 12:57:37.589635 aiogram3_form-1.0.2/LICENSE
--rw-r--r--   0        0        0     1151 2024-03-12 23:29:36.006733 aiogram3_form-1.0.2/README.md
--rw-r--r--   0        0        0      290 2024-03-12 22:37:25.522433 aiogram3_form-1.0.2/aiogram3_form/__init__.py
--rw-r--r--   0        0        0     1349 2024-03-12 22:53:11.612350 aiogram3_form-1.0.2/aiogram3_form/field.py
--rw-r--r--   0        0        0      997 2024-03-12 22:40:18.790479 aiogram3_form-1.0.2/aiogram3_form/filters.py
--rw-r--r--   0        0        0     8813 2024-03-12 22:59:30.303083 aiogram3_form-1.0.2/aiogram3_form/form.py
--rw-r--r--   0        0        0      282 2024-03-12 22:33:29.612411 aiogram3_form-1.0.2/aiogram3_form/state.py
--rw-r--r--   0        0        0      505 2024-03-12 23:27:06.233876 aiogram3_form-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 aiogram3_form-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-07 12:57:37.589635 aiogram3_form-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1151 2024-03-12 23:29:50.534053 aiogram3_form-2.0.0/README.md
+-rw-r--r--   0        0        0      520 2024-05-05 02:11:14.608700 aiogram3_form-2.0.0/aiogram3_form/__init__.py
+-rw-r--r--   0        0        0     1308 2024-05-05 02:10:43.371085 aiogram3_form-2.0.0/aiogram3_form/field.py
+-rw-r--r--   0        0        0     2832 2024-05-05 02:09:33.376424 aiogram3_form-2.0.0/aiogram3_form/filters.py
+-rw-r--r--   0        0        0     7071 2024-05-05 02:12:28.234533 aiogram3_form-2.0.0/aiogram3_form/form.py
+-rw-r--r--   0        0        0      392 2024-05-04 07:33:11.731995 aiogram3_form-2.0.0/aiogram3_form/utils.py
+-rw-r--r--   0        0        0      505 2024-05-05 02:12:38.085043 aiogram3_form-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 aiogram3_form-2.0.0/PKG-INFO
```

### Comparing `aiogram3_form-1.0.2/LICENSE` & `aiogram3_form-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_form-1.0.2/README.md` & `aiogram3_form-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `aiogram3_form-1.0.2/aiogram3_form/form.py` & `aiogram3_form-2.0.0/aiogram3_form/form.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,142 +1,118 @@
-import functools
 import inspect
 from abc import ABC, ABCMeta
-from typing import Any, Callable, NamedTuple, Optional, Set, Tuple, Type, Union
+from typing import Any, Callable, Coroutine, Generator, NamedTuple, Set, TypedDict
 
 from aiogram import Bot, types
 from aiogram.dispatcher.router import Router
+from aiogram.filters.state import StateFilter
 from aiogram.fsm.context import FSMContext
 from aiogram.utils.magic_filter import MagicFilter
 
-from . import filters
+from . import filters, utils
 from .field import FormFieldData, FormFieldInfo
-from .state import FormState
 
 SubmitCallback = Callable[..., Any]
-Markup = Union[types.ReplyKeyboardMarkup, types.InlineKeyboardMarkup]
+Markup = types.ReplyKeyboardMarkup | types.InlineKeyboardMarkup
 
 
-def _get_form_filter_for_type(field_type: Type):
-    field_filter = filters.DEFAULT_FORM_FILTERS.get(field_type)
-
-    if field_filter is None:
-        raise TypeError(
-            f"There is no default filter for type {field_type}. You should consider writing your own filter"  # noqa: E501
-        )
-
-    return field_filter
-
-
-def _form_fields_data_generator(cls: "FormMeta"):
+def _form_fields_data_generator(cls: "FormMeta") -> Generator[FormFieldData, Any, None]:
     annotations = inspect.get_annotations(cls)
 
     for field_name, field_type in annotations.items():
         field_info = getattr(cls, field_name, None)
 
         if not isinstance(field_info, FormFieldInfo):
             continue
 
         if field_info.filter is None:
-            field_filter = _get_form_filter_for_type(field_type)
+            field_filter = filters.get_form_filter_for_type(field_type)
         else:
             field_filter = field_info.filter
 
         if isinstance(field_filter, MagicFilter):
-            filter_type = filters._FormFilterType.magic
+            transformer = filters.MagicInputTransformer(field_filter)
         elif inspect.iscoroutinefunction(field_filter):
-            filter_type = filters._FormFilterType.coro
+            transformer = filters.AsyncInputTransformer(field_filter)
         elif inspect.isfunction(field_filter):
-            filter_type = filters._FormFilterType.func
+            transformer = filters.SyncInputTransformer(field_filter)
         else:
             raise TypeError(
                 f"Invalid filter of type {field_filter.__class__.__name__} for field {field_name}"  # noqa: E501
             )
 
         yield FormFieldData(
-            name=field_name,
-            type=field_type,
-            info=field_info,
-            filter=filters._FormFilter(field_filter, filter_type),
+            name=field_name, type=field_type, info=field_info, transformer=transformer
         )
 
 
-def _prepare_function(func: Callable, *args, **kwargs):
-    arg_spec = inspect.getfullargspec(func)
-
-    prepared_kwargs = {
-        k: v
-        for k, v in kwargs.items()
-        if k in arg_spec.args or k in arg_spec.kwonlyargs
-    }
-
-    partial_func = functools.partial(func, *args, **prepared_kwargs)
-    return partial_func
+class FormStateData(TypedDict):
+    __form_name: str
+    __current_field_index: int
+    __form_values: dict[str, Any]
 
 
 class FormMeta(ABCMeta):
     __form_cls_names: Set[str] = set()
 
     def __new__(cls, cls_name: str, parents: tuple, cls_dict: dict):
         if cls_name in cls.__form_cls_names:
             raise NameError("Form with the same name does exist")
 
         cls.__form_cls_names.add(cls_name)
 
         subcls = super().__new__(cls, cls_name, parents, cls_dict)
         setattr(subcls, "fields", tuple(_form_fields_data_generator(subcls)))
-
         return subcls
 
 
-class FormSubmitCallback(NamedTuple):
+class FormSubmitData(NamedTuple):
     callback: SubmitCallback
     clear_state: bool
 
 
 class Form(ABC, metaclass=FormMeta):
-    fields: Tuple[FormFieldData, ...]
-
-    __submit_callback: Optional[FormSubmitCallback] = None
+    fields: tuple[FormFieldData, ...]
+    __submit_data: FormSubmitData
 
     def __init__(self, bot: Bot, chat_id: int):
         self.bot = bot
         self.chat_id = chat_id
 
     @classmethod
     def submit(cls, *, router: Router, clear_state: bool = True):
         def _decorator(submit_callback: SubmitCallback):
-            if cls.__submit_callback is not None:
+            if cls.__submit_data is not None:
                 raise ValueError(f"{cls.__name__} submit callback already set")
 
-            cls.__submit_callback = FormSubmitCallback(submit_callback, clear_state)
+            cls.__submit_data = FormSubmitData(submit_callback, clear_state)
 
             router.message.register(
                 cls.__resolve_callback,
-                FormState.waiting_field_value,
+                StateFilter(cls.__name__),
                 cls.__current_field_filter,
             )
 
             return submit_callback
 
         return _decorator
 
     @classmethod
-    def __create_object(cls, handler_data: dict[str, Any], state_data: FormState.Data):
+    def __create_object(cls, handler_data: dict[str, Any], state_data: FormStateData):
         form_object = cls(handler_data["bot"], handler_data["event_chat"].id)
         form_object.__dict__.update(state_data["__form_values"])
         return form_object
 
     @classmethod
     async def start(cls, bot: Bot, state_ctx: FSMContext, **data: Any) -> types.Message:
         first_field = cls.fields[0]
 
-        await state_ctx.set_state(FormState.waiting_field_value)
+        await state_ctx.set_state(cls.__name__)
 
-        state_data: FormState.Data = {
+        state_data: FormStateData = {
             "__form_name": cls.__name__,
             "__form_values": {},
             "__current_field_index": 0,
         }
 
         await state_ctx.update_data(state_data)  # type: ignore
 
@@ -149,124 +125,91 @@
             state_ctx.key.chat_id,
             first_field.info.enter_message_text,  # type: ignore
             reply_markup=first_field.info.reply_markup,
         )
 
     @classmethod
     async def __resolve_callback(
-        cls, message: types.Message, state: FSMContext, value: Any, **data
+        cls, message: types.Message, state: FSMContext, _form_value: Any, **data: Any
     ):
-        state_data: FormState.Data = await state.get_data()  # type: ignore
+        state_data: FormStateData = await state.get_data()  # type: ignore
 
         current_field = cls.fields[state_data["__current_field_index"]]
-        state_data["__form_values"][current_field.name] = value
-
-        next_field_index = state_data["__current_field_index"] + 1
+        state_data["__form_values"][current_field.name] = _form_value
 
         try:
+            next_field_index = state_data["__current_field_index"] + 1
             next_field = cls.fields[next_field_index]
             state_data["__current_field_index"] = next_field_index
-            await state.set_data(state_data)  # type: ignore
+
+            await state.set_data(
+                state_data,  # type: ignore
+            )
 
             if next_field.info.enter_callback:
                 return await next_field.info.enter_callback(
                     state.key.chat_id, state.key.user_id, data | state_data
                 )
 
             return await message.answer(
                 next_field.info.enter_message_text,  # type: ignore
                 reply_markup=next_field.info.reply_markup,
             )
         except IndexError:
             pass  # submit reached
 
-        if cls.__submit_callback is None:
-            raise TypeError("Submit callback should be set")
+        if cls.__submit_data.clear_state:
+            await state.set_state(None)
 
         form_object = cls.__create_object(data, state_data)
         data["state"] = state
 
-        prepared_submit_callback = _prepare_function(
-            cls.__submit_callback.callback, form_object, **data
+        prepared_submit_callback = utils.prepare_function(
+            cls.__submit_data.callback, form_object, **data
         )
 
-        try:
-            await prepared_submit_callback()
-        finally:
-            if cls.__submit_callback.clear_state:
-                await state.clear()
+        await prepared_submit_callback()
 
     @classmethod
     async def __current_field_filter(
-        cls, message: types.Message, state: FSMContext, **data
-    ):
-        state_data: FormState.Data = await state.get_data()  # type: ignore
+        cls, message: types.Message, **data: Any
+    ) -> dict[str, Any] | bool:
+        state: FSMContext = data["state"]
+        state_data: FormStateData = await state.get_data()  # type: ignore
 
         if state_data["__form_name"] != cls.__name__:
             return False
 
         current_field = cls.fields[state_data["__current_field_index"]]
+        filter_result, success = (
+            await current_field.transformer.transform_input_message(message, data)
+        )
 
-        async def send_error_message():
-            if current_field.info.error_message_text:
-                return await message.answer(
-                    current_field.info.error_message_text,
-                    reply_markup=current_field.info.reply_markup,
-                )
-
-        if current_field.filter.filter_type == filters._FormFilterType.magic:
-            filter_result = current_field.filter.filter.resolve(
-                message,
-            )
-
-            if filter_result is not None and filter_result is not False:
-                return dict(value=filter_result)
-
-            await send_error_message()
-            return False
-
-        if current_field.filter.filter_type == filters._FormFilterType.coro:
-            prepared_field_filter = _prepare_function(
-                current_field.filter.filter, message, **data
-            )
-
-            filter_result = await prepared_field_filter()
-
-            if filter_result is not False:
-                return dict(value=filter_result)
-
-            await send_error_message()
-            return False
+        if success:
+            return dict(_form_value=filter_result)
 
-        if current_field.filter.filter_type == filters._FormFilterType.func:
-            prepared_field_filter = _prepare_function(
-                current_field.filter.filter, message, **data
+        if current_field.info.error_message_text:
+            await message.answer(
+                current_field.info.error_message_text,
+                reply_markup=current_field.info.reply_markup,
             )
 
-            filter_result = prepared_field_filter()
-
-            if filter_result is not False:
-                return dict(value=filter_result)
+        return False
 
-            await send_error_message()
-            return False
-
-        raise TypeError(f"Invalid filter specified for field {current_field.name}")
-
-    async def answer(
+    def answer(
         self,
         text: str,
-        reply_markup: Union[
-            types.InlineKeyboardMarkup,
-            types.ReplyKeyboardMarkup,
-            types.ReplyKeyboardRemove,
-            types.ForceReply,
-            None,
-        ] = None,
-        reply_to_message_id: Optional[int] = None,
-    ):
-        return await self.bot.send_message(
+        reply_markup: (
+            types.InlineKeyboardMarkup
+            | types.ReplyKeyboardMarkup
+            | types.ReplyKeyboardRemove
+            | types.ForceReply
+            | None
+        ) = None,
+        reply_to_message_id: int | None = None,
+    ) -> Coroutine[Any, Any, types.Message]:
+        return self.bot.send_message(
             self.chat_id,
             text=text,
             reply_markup=reply_markup,
             reply_to_message_id=reply_to_message_id,
         )
```

### Comparing `aiogram3_form-1.0.2/PKG-INFO` & `aiogram3_form-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-form
-Version: 1.0.2
+Version: 2.0.0
 Summary: A library to create forms in aiogram3
 License: MIT
 Author: TrixiS
 Author-email: oficialmorozov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

