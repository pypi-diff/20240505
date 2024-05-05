# Comparing `tmp/miniagents-0.0.7.tar.gz` & `tmp/miniagents-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniagents-0.0.7.tar", max compression
+gzip compressed data, was "miniagents-0.0.8.tar", max compression
```

## Comparing `miniagents-0.0.7.tar` & `miniagents-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.7/LICENSE
--rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.7/miniagents/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.7/miniagents/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.7/miniagents/ext/llms/__init__.py
--rw-r--r--   0        0        0     4364 2024-04-18 21:45:37.115573 miniagents-0.0.7/miniagents/ext/llms/anthropic.py
--rw-r--r--   0        0        0    20146 2024-04-21 22:07:14.263095 miniagents-0.0.7/miniagents/miniagents.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.7/miniagents/promisegraph/__init__.py
--rw-r--r--   0        0        0      563 2024-04-02 17:38:48.000619 miniagents-0.0.7/miniagents/promisegraph/errors.py
--rw-r--r--   0        0        0     3795 2024-04-23 16:28:22.928918 miniagents-0.0.7/miniagents/promisegraph/node.py
--rw-r--r--   0        0        0    18881 2024-04-21 22:07:14.265115 miniagents-0.0.7/miniagents/promisegraph/promise.py
--rw-r--r--   0        0        0      453 2024-04-18 21:45:37.118627 miniagents-0.0.7/miniagents/promisegraph/sentinels.py
--rw-r--r--   0        0        0     1888 2024-04-16 00:22:57.814833 miniagents-0.0.7/miniagents/promisegraph/sequence.py
--rw-r--r--   0        0        0     2219 2024-04-16 00:22:57.815527 miniagents-0.0.7/miniagents/promisegraph/typing.py
--rw-r--r--   0        0        0     2356 2024-04-21 22:07:14.265779 miniagents-0.0.7/miniagents/utils.py
--rw-r--r--   0        0        0      694 2024-04-21 22:16:19.745259 miniagents-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.8/LICENSE
+-rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.8/miniagents/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.8/miniagents/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.8/miniagents/ext/llms/__init__.py
+-rw-r--r--   0        0        0     4307 2024-04-29 06:06:00.887264 miniagents-0.0.8/miniagents/ext/llms/anthropic.py
+-rw-r--r--   0        0        0     8301 2024-05-05 14:27:35.144467 miniagents-0.0.8/miniagents/messages.py
+-rw-r--r--   0        0        0    16169 2024-05-05 14:47:49.141620 miniagents-0.0.8/miniagents/miniagents.py
+-rw-r--r--   0        0        0        0 2024-04-27 10:16:52.343384 miniagents-0.0.8/miniagents/promising/__init__.py
+-rw-r--r--   0        0        0      548 2024-04-28 10:26:42.580105 miniagents-0.0.8/miniagents/promising/errors.py
+-rw-r--r--   0        0        0     6122 2024-05-05 14:27:35.146244 miniagents-0.0.8/miniagents/promising/node.py
+-rw-r--r--   0        0        0    20940 2024-05-05 14:27:35.146955 miniagents-0.0.8/miniagents/promising/promising.py
+-rw-r--r--   0        0        0      453 2024-04-27 10:16:52.345574 miniagents-0.0.8/miniagents/promising/sentinels.py
+-rw-r--r--   0        0        0     1881 2024-04-28 10:27:04.793246 miniagents-0.0.8/miniagents/promising/sequence.py
+-rw-r--r--   0        0        0     2474 2024-04-28 10:26:42.582714 miniagents-0.0.8/miniagents/promising/typing.py
+-rw-r--r--   0        0        0     2302 2024-04-29 06:06:00.889297 miniagents-0.0.8/miniagents/utils.py
+-rw-r--r--   0        0        0      694 2024-04-23 16:40:25.878553 miniagents-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.8/PKG-INFO
```

### Comparing `miniagents-0.0.7/LICENSE` & `miniagents-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.7/miniagents/ext/llms/anthropic.py` & `miniagents-0.0.8/miniagents/ext/llms/anthropic.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 """
 
 import typing
 from functools import partial
 from typing import AsyncIterator, Any, Optional
 
 from miniagents.miniagents import (
-    MessagePromise,
     Message,
     miniagent,
     MiniAgent,
     MiniAgents,
     InteractionContext,
 )
-from miniagents.promisegraph.node import Node
+from miniagents.promising.node import Node
 
 if typing.TYPE_CHECKING:
     import anthropic as anthropic_original
 
 
 class AnthropicMessage(Message):
     """
@@ -96,18 +95,17 @@
                     f"but {len(anthropic_final_message.content)} were returned instead"
                 )
             yield anthropic_final_message.content[0].text  # yield the whole text as one "piece"
 
         metadata_so_far["anthropic"] = anthropic_final_message.model_dump(exclude={"content"})
 
     ctx.reply(
-        MessagePromise(
+        AnthropicMessage.promise(
             schedule_immediately=True,  # TODO Oleksandr: should this be customizable ?
             message_token_producer=message_token_producer,
-            message_class=AnthropicMessage,
         )
     )
 
 
 def _message_to_anthropic_dict(message: Message) -> dict[str, Any]:
     # TODO Oleksandr: introduce a lambda function to derive roles from messages ?
     try:
```

### Comparing `miniagents-0.0.7/miniagents/miniagents.py` & `miniagents-0.0.8/miniagents/miniagents.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,264 +1,137 @@
-# pylint: disable=too-many-arguments
 """
-Split this module into multiple modules.
+"Core" classes of the MiniAgents framework.
 """
-from typing import Protocol, AsyncIterator, Any, Union, Iterable, AsyncIterable, Optional, Callable
 
-from miniagents.promisegraph.node import Node
-from miniagents.promisegraph.promise import StreamedPromise, AppendProducer, Promise, PromiseContext
-from miniagents.promisegraph.sentinels import Sentinel, DEFAULT
-from miniagents.promisegraph.sequence import FlatSequence
-from miniagents.promisegraph.typing import StreamedPieceProducer, PromiseBound
+from typing import Protocol, AsyncIterator, Any, Union, Optional, Callable, Iterable
 
+from pydantic import BaseModel
 
-class NodeCollectedEventHandler(Protocol):
+from miniagents.messages import MessageType, MessagePromise, MessageSequencePromise, Message
+from miniagents.promising.node import Node
+from miniagents.promising.promising import AppendProducer, Promise, PromisingContext
+from miniagents.promising.sentinels import Sentinel, DEFAULT
+from miniagents.promising.sequence import FlatSequence
+from miniagents.promising.typing import StreamedPieceProducer, NodeCollectedEventHandler
+
+
+class SerializeMessageEventHandler(Protocol):
     """
     TODO Oleksandr: docstring
     """
 
-    async def __call__(self, promise: PromiseBound, node: Node) -> None: ...
+    async def __call__(self, promise: MessagePromise, message: Message) -> None: ...
 
 
-class MiniAgents(PromiseContext):
+class MiniAgents(PromisingContext):
     """
     TODO Oleksandr: docstring
     """
 
     def __init__(
         self,
         stream_llm_tokens_by_default: bool = True,
         on_node_collected: Union[NodeCollectedEventHandler, Iterable[NodeCollectedEventHandler]] = (),
+        on_serialize_message: Union[SerializeMessageEventHandler, Iterable[SerializeMessageEventHandler]] = (),
         **kwargs,
     ) -> None:
-        super().__init__(**kwargs)
-        self.on_node_collected_handlers: list[NodeCollectedEventHandler] = (
-            [on_node_collected] if callable(on_node_collected) else list(on_node_collected)
+        on_node_collected = (
+            [self._schedule_serialize_message_event, on_node_collected]
+            if callable(on_node_collected)
+            else [self._schedule_serialize_message_event, *on_node_collected]
         )
-        self.on_promise_collected(self._schedule_on_node_collected)
-
+        super().__init__(on_node_collected=on_node_collected, **kwargs)
         self.stream_llm_tokens_by_default = stream_llm_tokens_by_default
+        self.on_serialize_message_handlers: list[SerializeMessageEventHandler] = (
+            [on_serialize_message] if callable(on_serialize_message) else list(on_serialize_message)
+        )
 
     @classmethod
     def get_current(cls) -> "MiniAgents":
         """
         TODO Oleksandr: docstring
         """
         # noinspection PyTypeChecker
         return super().get_current()
 
-    def on_node_collected(self, handler: NodeCollectedEventHandler) -> NodeCollectedEventHandler:
+    def on_serialize_message(self, handler: SerializeMessageEventHandler) -> SerializeMessageEventHandler:
         """
-        Add a handler to be called after a promise of type Node is collected.
+        Add a handler that will be called every time a Message needs to be serialized.
         """
-        self.on_node_collected_handlers.append(handler)
+        self.on_serialize_message_handlers.append(handler)
         return handler
 
-    async def _schedule_on_node_collected(self, _, result: Any) -> None:
+    # noinspection PyProtectedMember
+    async def _schedule_serialize_message_event(self, _, node: Node) -> None:
         """
         TODO Oleksandr: docstring
         """
-        if not isinstance(result, Node):
+        # pylint: disable=protected-access
+        if not isinstance(node, Message):
             return
-        for handler in self.on_node_collected_handlers:
-            self.schedule_task(handler(_, result))
-
-
-class Message(Node):
-    """
-    A message that can be sent between agents.
-    """
-
-    text: Optional[str] = None
-    text_template: Optional[str] = None
-
-    def _as_string(self) -> str:
-        if self.text is not None:
-            return self.text
-        if self.text_template is not None:
-            return self.text_template.format(**self.model_dump())
-        return super()._as_string()
-
-
-class AgentInteractionNode(Node):
-    """
-    TODO Oleksandr
-    """
-
-    agent_alias: str
-
-
-class AgentCallNode(Node):
-    """
-    TODO Oleksandr
-    """
-
-    message_hash_keys: tuple[str, ...]
-
 
-class AgentReplyNode(Node):
-    """
-    TODO Oleksandr
-    """
+        for sub_message in node.sub_messages():
+            if sub_message._serialize_message_event_triggered:
+                continue
+
+            for handler in self.on_serialize_message_handlers:
+                self.schedule_task(handler(_, sub_message))
+            sub_message._serialize_message_event_triggered = True
 
-    agent_call_hash_key: str
-    reply_hash_keys: tuple[str, ...]
-
-
-class MessageTokenProducer(Protocol):
-    """
-    A protocol for message piece producer functions.
-    """
+        if node._serialize_message_event_triggered:
+            return
 
-    def __call__(self, metadata_so_far: dict[str, Any]) -> AsyncIterator[str]: ...
+        for handler in self.on_serialize_message_handlers:
+            self.schedule_task(handler(_, node))
+        node._serialize_message_event_triggered = True
 
 
-class MessagePromise(StreamedPromise[str, Message]):
+def miniagent(
+    func: Optional["AgentFunction"] = None,
+    /,  # TODO Oleksandr: do I really need to enforce positional-only upon `func` ?
+    alias: Optional[str] = None,
+    description: Optional[str] = None,
+    uppercase_func_name: bool = True,
+    normalize_spaces_in_docstring: bool = True,
+    interaction_metadata: Optional[dict[str, Any]] = None,
+) -> Union["MiniAgent", Callable[["AgentFunction"], "MiniAgent"]]:
     """
-    A promise of a message that can be streamed token by token.
+    A decorator that converts an agent function into an agent.
     """
-
-    def __init__(
-        self,
-        schedule_immediately: Union[bool, Sentinel] = DEFAULT,
-        message_token_producer: MessageTokenProducer = None,
-        prefill_message: Optional[Message] = None,
-        metadata_so_far: Optional[dict[str, Any]] = None,
-        message_class: type[Message] = Message,
-    ) -> None:
-        # TODO Oleksandr: raise an error if both ready_message and message_token_producer/metadata_so_far are not None
-        #  (or both are None)
-        if prefill_message:
-            super().__init__(
-                schedule_immediately=schedule_immediately,
-                prefill_pieces=[str(prefill_message)],
-                prefill_whole=prefill_message,
-            )
-        else:
-            super().__init__(
-                schedule_immediately=schedule_immediately,
-                producer=self._producer,
-                packager=self._packager,
+    if func is None:
+        # the decorator `@miniagent(...)` was used with arguments
+        def _decorator(f: "AgentFunction") -> "MiniAgent":
+            return MiniAgent(
+                f,
+                alias=alias,
+                description=description,
+                uppercase_func_name=uppercase_func_name,
+                normalize_spaces_in_docstring=normalize_spaces_in_docstring,
+                interaction_metadata=interaction_metadata,
             )
-            self._message_token_producer = message_token_producer
-            self._metadata_so_far = metadata_so_far or {}
-            self._message_class = message_class
-
-    def _producer(self, _) -> AsyncIterator[str]:
-        return self._message_token_producer(self._metadata_so_far)
-
-    async def _packager(self, _) -> Message:
-        return self._message_class(
-            text="".join([token async for token in self]),
-            **self._metadata_so_far,
-        )
-
-    def __aiter__(self) -> AsyncIterator[str]:
-        # PyCharm fails to see that MessagePromise inherits AsyncIterable protocol from StreamedPromise,
-        # hence the need to explicitly declare the __aiter__ method here
-        return super().__aiter__()
 
+        return _decorator
 
-# TODO Oleksandr: add documentation somewhere that explains what MessageType and SingleMessageType represent
-SingleMessageType = Union[str, dict[str, Any], Message, MessagePromise, BaseException]
-MessageType = Union[SingleMessageType, Iterable["MessageType"], AsyncIterable["MessageType"]]
+    # the decorator `@miniagent` was used either without arguments or as a direct function call
+    return MiniAgent(
+        func,
+        alias=alias,
+        description=description,
+        uppercase_func_name=uppercase_func_name,
+        normalize_spaces_in_docstring=normalize_spaces_in_docstring,
+        interaction_metadata=interaction_metadata,
+    )
 
 
-class MessageSequencePromise(StreamedPromise[MessagePromise, tuple[MessagePromise, ...]]):
+class AgentFunction(Protocol):
     """
-    A promise of a sequence of messages that can be streamed message by message.
+    A protocol for agent functions.
     """
 
-    async def acollect_messages(self) -> tuple[Message, ...]:
-        """
-        Collect all messages from the sequence and return them as a tuple of Message objects.
-        """
-        # pylint: disable=consider-using-generator
-        return tuple([await message_promise.acollect() async for message_promise in self])
-
-    def __aiter__(self) -> AsyncIterator[MessagePromise]:
-        # PyCharm fails to see that MessageSequencePromise inherits AsyncIterable protocol from StreamedPromise,
-        # hence the need to explicitly declare the __aiter__ method here
-        return super().__aiter__()
-
-
-class MessageSequence(FlatSequence[MessageType, MessagePromise]):
-    """
-    TODO Oleksandr: produce a docstring for this class after you actually use it in real agents
-    """
-
-    append_producer: Optional[AppendProducer[MessageType]]
-    sequence_promise: MessageSequencePromise
-
-    def __init__(
-        self,
-        producer_capture_errors: Union[bool, Sentinel] = DEFAULT,
-        schedule_immediately: Union[bool, Sentinel] = DEFAULT,
-        incoming_producer: Optional[StreamedPieceProducer[MessageType]] = None,
-    ) -> None:
-        if incoming_producer:
-            # an external producer is provided, so we don't create the default AppendProducer
-            self.append_producer = None
-        else:
-            self.append_producer = AppendProducer(capture_errors=producer_capture_errors)
-            incoming_producer = self.append_producer
-
-        super().__init__(
-            incoming_producer=incoming_producer,
-            flattener=self._flattener,
-            schedule_immediately=schedule_immediately,
-            sequence_promise_class=MessageSequencePromise,
-        )
-
-    @classmethod
-    def turn_into_sequence_promise(cls, messages: MessageType) -> MessageSequencePromise:
-        """
-        Convert an arbitrarily nested collection of messages of various types (strings, dicts, Message objects,
-        MessagePromise objects etc. - see `MessageType` definition for details) into a flat and uniform
-        MessageSequencePromise object.
-        """
-        message_sequence = cls(
-            producer_capture_errors=True,
-            schedule_immediately=False,
-        )
-        with message_sequence.append_producer:
-            message_sequence.append_producer.append(messages)
-        return message_sequence.sequence_promise
-
-    @classmethod
-    async def acollect_messages(cls, messages: MessageType) -> tuple[Message, ...]:
-        """
-        Convert an arbitrarily nested collection of messages of various types (strings, dicts, Message objects,
-        MessagePromise objects etc. - see `MessageType` definition for details) into a flat and uniform tuple of
-        Message objects.
-        """
-        return await cls.turn_into_sequence_promise(messages).acollect_messages()
-
-    @staticmethod
-    async def _flattener(_, zero_or_more_items: MessageType) -> AsyncIterator[MessagePromise]:
-        if isinstance(zero_or_more_items, MessagePromise):
-            yield zero_or_more_items
-        elif isinstance(zero_or_more_items, Message):
-            yield MessagePromise(prefill_message=zero_or_more_items)
-        elif isinstance(zero_or_more_items, str):
-            yield MessagePromise(prefill_message=Message(text=zero_or_more_items))
-        elif isinstance(zero_or_more_items, dict):
-            yield MessagePromise(prefill_message=Message(**zero_or_more_items))
-        elif isinstance(zero_or_more_items, BaseException):
-            raise zero_or_more_items
-        elif hasattr(zero_or_more_items, "__iter__"):
-            for item in zero_or_more_items:
-                async for message_promise in MessageSequence._flattener(_, item):
-                    yield message_promise
-        elif hasattr(zero_or_more_items, "__aiter__"):
-            async for item in zero_or_more_items:
-                async for message_promise in MessageSequence._flattener(_, item):
-                    yield message_promise
-        else:
-            raise TypeError(f"unexpected message type: {type(zero_or_more_items)}")
+    async def __call__(self, ctx: "InteractionContext", **kwargs) -> None: ...
 
 
 class InteractionContext:
     """
     TODO Oleksandr: docstring
     """
 
@@ -276,20 +149,55 @@
         # TODO Oleksandr: add a warning that iterators, async iterators and generators, if passed as `messages` will
         #  not be iterated over immediately, which means that if two agent calls are passed as a generator, those
         #  agent calls will not be scheduled for parallel execution, unless the generator is wrapped into a list (to
         #  guarantee that it will be iterated over immediately)
         self._reply_producer.append(messages)
 
 
-class AgentFunction(Protocol):
+class AgentCall:
     """
-    A protocol for agent functions.
+    TODO Oleksandr: docstring
+    TODO Oleksandr: turn this into a context manager ?
     """
 
-    async def __call__(self, ctx: InteractionContext, **kwargs) -> None: ...
+    def __init__(
+        self,
+        message_producer: AppendProducer[MessageType],
+        reply_sequence_promise: MessageSequencePromise,
+    ) -> None:
+        self._message_producer = message_producer
+        self._reply_sequence_promise = reply_sequence_promise
+
+        self._message_producer.open()
+
+    def send_message(self, message: MessageType) -> "AgentCall":
+        """
+        Send an input message to the agent.
+        """
+        self._message_producer.append(message)
+        return self
+
+    def reply_sequence(self) -> MessageSequencePromise:
+        """
+        Finish the agent call and return the agent's response(s).
+
+        NOTE: After this method is called it is not possible to send any more requests to this AgentCall object.
+        """
+        self.finish()
+        return self._reply_sequence_promise
+
+    def finish(self) -> "AgentCall":
+        """
+        Finish the agent call.
+
+        NOTE: After this method is called it is not possible to send any more requests to this AgentCall object.
+        """
+        # TODO Oleksandr: also make sure to close the producer when the parent agent call is finished
+        self._message_producer.close()
+        return self
 
 
 class MiniAgent:
     """
     A wrapper for an agent function that allows calling the agent.
     """
 
@@ -298,19 +206,20 @@
         func: AgentFunction,
         alias: Optional[str] = None,
         description: Optional[str] = None,
         # TODO Oleksandr: use DEFAULT for the following two arguments (and put them into MiniAgents class)
         uppercase_func_name: bool = True,
         normalize_spaces_in_docstring: bool = True,
         interaction_metadata: Optional[dict[str, Any]] = None,
+        # TODO Oleksandr: turn MiniAgent into a Node object so arbitrary agent level metadata can be stored in it ?
     ) -> None:
         self._func = func
         # TODO Oleksandr: do deep copy ? freeze with Node ? yoo need to start putting these things down into the
         #  "Philosophy" section of README
-        self._interaction_metadata = interaction_metadata or {}
+        self.interaction_metadata = interaction_metadata or {}
 
         self.alias = alias
         if self.alias is None:
             self.alias = func.__name__
             if uppercase_func_name:
                 self.alias = self.alias.upper()
 
@@ -329,39 +238,28 @@
     def inquire(
         self,
         messages: Optional[MessageType] = None,
         schedule_immediately: Union[bool, Sentinel] = DEFAULT,
         **function_kwargs,
     ) -> MessageSequencePromise:
         """
-        TODO Oleksandr: update this docstring
-        "Ask" the agent and immediately receive an AsyncMessageSequence object that can be used to obtain the agent's
-        response(s). If blank_history is False and history_tracker/branch_from is not specified and pre-existing
-        messages are passed as requests (for ex. messages that came from other agents), then this agent call will be
-        automatically branched off of the conversation branch those pre-existing messages belong to (the history will
-        be inherited from those messages, in other words).
+        TODO Oleksandr: docstring
         """
         agent_call = self.initiate_inquiry(schedule_immediately=schedule_immediately, **function_kwargs)
         if messages is not None:
             agent_call.send_message(messages)
         return agent_call.reply_sequence()
 
     def initiate_inquiry(
         self,
         schedule_immediately: Union[bool, Sentinel] = DEFAULT,
         **function_kwargs,
     ) -> "AgentCall":
         """
-        TODO Oleksandr: update this docstring
-        Initiate the process of "asking" the agent. Returns an AgentCall object that can be used to send requests to
-        the agent by calling `send_request()` zero or more times and receive its responses by calling
-        `response_sequence()` at the end. If blank_history is False and history_tracker/branch_from is not specified
-        and pre-existing messages are passed as requests (for ex. messages that came from other agents), then this
-        agent call will be automatically branched off of the conversation branch those pre-existing messages belong to
-        (the history will be inherited from those messages, in other words).
+        TODO Oleksandr: docstring
         """
         input_sequence = MessageSequence(
             schedule_immediately=False,
         )
         reply_sequence = AgentReplyMessageSequence(
             mini_agent=self,
             function_kwargs=function_kwargs,
@@ -372,15 +270,117 @@
         agent_call = AgentCall(
             message_producer=input_sequence.append_producer,
             reply_sequence_promise=reply_sequence.sequence_promise,
         )
         return agent_call
 
 
-# noinspection PyProtectedMember
+class AgentInteractionNode(Message):
+    """
+    TODO Oleksandr
+    """
+
+    agent_alias: str
+
+
+class AgentCallNode(AgentInteractionNode):
+    """
+    TODO Oleksandr
+    """
+
+    messages: tuple[Message, ...]
+
+
+class AgentReplyNode(AgentInteractionNode):
+    """
+    TODO Oleksandr
+    """
+
+    agent_call: AgentCallNode
+    replies: tuple[Message, ...]
+
+
+class MessageSequence(FlatSequence[MessageType, MessagePromise]):
+    """
+    TODO Oleksandr: produce a docstring for this class after you actually use it in real agents
+    """
+
+    append_producer: Optional[AppendProducer[MessageType]]
+    sequence_promise: MessageSequencePromise
+
+    def __init__(
+        self,
+        producer_capture_errors: Union[bool, Sentinel] = DEFAULT,
+        schedule_immediately: Union[bool, Sentinel] = DEFAULT,
+        incoming_producer: Optional[StreamedPieceProducer[MessageType]] = None,
+    ) -> None:
+        if incoming_producer:
+            # an external producer is provided, so we don't create the default AppendProducer
+            self.append_producer = None
+        else:
+            self.append_producer = AppendProducer(capture_errors=producer_capture_errors)
+            incoming_producer = self.append_producer
+
+        super().__init__(
+            incoming_producer=incoming_producer,
+            flattener=self._flattener,
+            schedule_immediately=schedule_immediately,
+            sequence_promise_class=MessageSequencePromise,
+        )
+
+    @classmethod
+    def turn_into_sequence_promise(cls, messages: MessageType) -> MessageSequencePromise:
+        """
+        Convert an arbitrarily nested collection of messages of various types (strings, dicts, Message objects,
+        MessagePromise objects etc. - see `MessageType` definition for details) into a flat and uniform
+        MessageSequencePromise object.
+        """
+        message_sequence = cls(
+            producer_capture_errors=True,
+            schedule_immediately=False,
+        )
+        with message_sequence.append_producer:
+            message_sequence.append_producer.append(messages)
+        return message_sequence.sequence_promise
+
+    @classmethod
+    async def acollect_messages(cls, messages: MessageType) -> tuple[Message, ...]:
+        """
+        Convert an arbitrarily nested collection of messages of various types (strings, dicts, Message objects,
+        MessagePromise objects etc. - see `MessageType` definition for details) into a flat and uniform tuple of
+        Message objects.
+        """
+        return await cls.turn_into_sequence_promise(messages).acollect_messages()
+
+    @classmethod
+    async def _flattener(cls, _, zero_or_more_items: MessageType) -> AsyncIterator[MessagePromise]:
+        if isinstance(zero_or_more_items, MessagePromise):
+            yield zero_or_more_items
+        elif isinstance(zero_or_more_items, Message):
+            yield zero_or_more_items.as_promise
+        elif isinstance(zero_or_more_items, BaseModel):
+            yield Message(**zero_or_more_items.model_dump()).as_promise
+        elif isinstance(zero_or_more_items, dict):
+            yield Message(**zero_or_more_items).as_promise
+        elif isinstance(zero_or_more_items, str):
+            yield Message(text=zero_or_more_items).as_promise
+        elif isinstance(zero_or_more_items, BaseException):
+            raise zero_or_more_items
+        elif hasattr(zero_or_more_items, "__iter__"):
+            for item in zero_or_more_items:
+                async for message_promise in cls._flattener(_, item):
+                    yield message_promise
+        elif hasattr(zero_or_more_items, "__aiter__"):
+            async for item in zero_or_more_items:
+                async for message_promise in cls._flattener(_, item):
+                    yield message_promise
+        else:
+            raise TypeError(f"Unexpected message type: {type(zero_or_more_items)}")
+
+
 class AgentReplyMessageSequence(MessageSequence):
     """
     TODO Oleksandr: docstring
     """
 
     def __init__(
         self,
@@ -395,133 +395,46 @@
         )
         self._mini_agent = mini_agent
         self._input_sequence_promise = input_sequence_promise
         # TODO Oleksandr: freeze function_kwargs as a Node object ? or just do deep copy ?
         self._function_kwargs = function_kwargs
 
     async def _producer(self, _) -> AsyncIterator[MessagePromise]:
-        # pylint: disable=protected-access
         async def run_the_agent(_) -> AgentCallNode:
             ctx = InteractionContext(
                 this_agent=self._mini_agent,
                 messages=self._input_sequence_promise,
                 reply_producer=self.append_producer,
             )
             with self.append_producer:
                 # errors are not raised above this `with` block, thanks to `producer_capture_errors=True`
+                # pylint: disable=protected-access
+                # noinspection PyProtectedMember
                 await self._mini_agent._func(ctx, **self._function_kwargs)
 
-            message_hash_keys = [
-                message.hash_key for message in await self._input_sequence_promise.acollect_messages()
-            ]
             return AgentCallNode(
-                message_hash_keys=message_hash_keys,
+                messages=await self._input_sequence_promise.acollect_messages(),
                 agent_alias=self._mini_agent.alias,
-                **self._mini_agent._interaction_metadata,
-                **self._function_kwargs,  # this will override any keys from `self._interaction_metadata`
+                **self._mini_agent.interaction_metadata,
+                **self._function_kwargs,  # this will override any keys from `self.interaction_metadata`
             )
 
         agent_call_promise = Promise[AgentCallNode](
             schedule_immediately=True,
             fulfiller=run_the_agent,
         )
 
         async for reply_promise in super()._producer(_):
             yield reply_promise  # at this point all MessageType items are "flattened" into MessagePromise items
 
         async def create_agent_reply_node(_) -> AgentReplyNode:
-            reply_hash_keys = [message.hash_key for message in await self.sequence_promise.acollect_messages()]
             return AgentReplyNode(
-                reply_hash_keys=reply_hash_keys,
+                replies=await self.sequence_promise.acollect_messages(),
                 agent_alias=self._mini_agent.alias,
-                agent_call_hash_key=(await agent_call_promise.acollect()).hash_key,
-                **self._mini_agent._interaction_metadata,
+                agent_call=await agent_call_promise.acollect(),
+                **self._mini_agent.interaction_metadata,
             )
 
         Promise[AgentReplyNode](
             schedule_immediately=True,  # use a separate async task to avoid deadlock upon AgentReplyNode "collection"
             fulfiller=create_agent_reply_node,
         )
-
-
-def miniagent(
-    func: Optional[AgentFunction] = None,
-    /,  # TODO Oleksandr: do I really need to enforce positional-only upon `func` ?
-    alias: Optional[str] = None,
-    description: Optional[str] = None,
-    uppercase_func_name: bool = True,
-    normalize_spaces_in_docstring: bool = True,
-    interaction_metadata: Optional[dict[str, Any]] = None,
-) -> Union["MiniAgent", Callable[[AgentFunction], MiniAgent]]:
-    """
-    A decorator that converts an agent function into an agent.
-    """
-    if func is None:
-        # the decorator `@miniagent(...)` was used with arguments
-        def _decorator(f: "AgentFunction") -> "MiniAgent":
-            return MiniAgent(
-                f,
-                alias=alias,
-                description=description,
-                uppercase_func_name=uppercase_func_name,
-                normalize_spaces_in_docstring=normalize_spaces_in_docstring,
-                interaction_metadata=interaction_metadata,
-            )
-
-        return _decorator
-
-    # the decorator `@miniagent` was used either without arguments or as a direct function call
-    return MiniAgent(
-        func,
-        alias=alias,
-        description=description,
-        uppercase_func_name=uppercase_func_name,
-        normalize_spaces_in_docstring=normalize_spaces_in_docstring,
-        interaction_metadata=interaction_metadata,
-    )
-
-
-class AgentCall:
-    """
-    TODO Oleksandr: update this docstring
-    TODO Oleksandr: turn this into a context manager ?
-    A call to an agent. This object is returned by Agent.start_asking()/start_telling() methods. It is used to send
-    requests to the agent and receive its responses.
-    """
-
-    def __init__(
-        self,
-        message_producer: AppendProducer[MessageType],
-        reply_sequence_promise: MessageSequencePromise,
-    ) -> None:
-        self._message_producer = message_producer
-        self._reply_sequence_promise = reply_sequence_promise
-
-        self._message_producer.open()
-
-    def send_message(self, message: MessageType) -> "AgentCall":
-        """
-        TODO Oleksandr: update this docstring ?
-        Send a request to the agent.
-        """
-        self._message_producer.append(message)
-        return self
-
-    def reply_sequence(self) -> MessageSequencePromise:
-        """
-        TODO Oleksandr: update this docstring ?
-        Finish the agent call and return the agent's response(s).
-
-        NOTE: After this method is called it is not possible to send any more requests to this AgentCall object.
-        """
-        self.finish()
-        return self._reply_sequence_promise
-
-    def finish(self) -> "AgentCall":
-        """
-        Finish the agent call.
-
-        NOTE: After this method is called it is not possible to send any more requests to this AgentCall object.
-        """
-        # TODO Oleksandr: also make sure to close the producer when the parent agent call is finished
-        self._message_producer.close()
-        return self
```

### Comparing `miniagents-0.0.7/miniagents/promisegraph/errors.py` & `miniagents-0.0.8/miniagents/promising/errors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-This module contains the custom errors used in the `PromiseGraph` part of the library.
+This module contains the custom errors used in the `Promising` part of the library.
 """
 
 
-class PromiseGraphError(Exception):
+class PromisingError(Exception):
     """
-    Base class for errors in the `PromiseGraph` part of the library.
+    Base class for errors in the `Promising` part of the library.
     """
 
 
-class AppendNotOpenError(PromiseGraphError):
+class AppendNotOpenError(PromisingError):
     """
     Raised when an `AppendProducer` is not open for appending yet and an attempt is made to append to it.
     """
 
 
-class AppendClosedError(PromiseGraphError):
+class AppendClosedError(PromisingError):
     """
     Raised when an `AppendProducer` has already been closed for appending and an attempt is made to append to it.
     """
```

### Comparing `miniagents-0.0.7/miniagents/promisegraph/promise.py` & `miniagents-0.0.8/miniagents/promising/promising.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,76 @@
 """
 The main class in this module is `StreamedPromise`. See its docstring for more information.
 """
 
 import asyncio
 import contextvars
+import logging
 from asyncio import Task
 from contextvars import ContextVar
 from types import TracebackType
 from typing import Generic, AsyncIterator, Union, Optional, Iterable, Awaitable, Any
 
-from miniagents.promisegraph.errors import AppendClosedError, AppendNotOpenError
-from miniagents.promisegraph.sentinels import Sentinel, NO_VALUE, FAILED, END_OF_QUEUE, DEFAULT
-from miniagents.promisegraph.typing import (
+from miniagents.promising.errors import AppendClosedError, AppendNotOpenError
+from miniagents.promising.node import Node
+from miniagents.promising.sentinels import Sentinel, NO_VALUE, FAILED, END_OF_QUEUE, DEFAULT
+from miniagents.promising.typing import (
     T,
     PIECE,
     WHOLE,
     StreamedPieceProducer,
     StreamedWholePackager,
     PromiseCollectedEventHandler,
     PromiseFulfiller,
+    NodeCollectedEventHandler,
 )
 
+logger = logging.getLogger(__name__)
 
-class PromiseContext:
+
+class PromisingContext:
     """
     This is the main class for managing the context of promises. It is a context manager that is used to configure
     default settings for promises and to handle the lifecycle of promises (attach `on_promise_collected` handlers).
     TODO Oleksandr: explain this class in more detail
+    TODO Oleksandr: especially the fact that on_node_collected is called for each Node instance only once (Node
+     instances keep track of whether on_node_collected has been called for them or not, and if it has, it is not
+     called)
     """
 
-    _current: ContextVar[Optional["PromiseContext"]] = ContextVar("PromiseContext._current", default=None)
+    _current: ContextVar[Optional["PromisingContext"]] = ContextVar("PromisingContext._current", default=None)
 
     def __init__(
         self,
         schedule_immediately_by_default: bool = True,
         producer_capture_errors_by_default: bool = False,
         longer_node_hash_keys: bool = False,  # TODO Oleksandr: does it belong in this class ?
         on_promise_collected: Union[PromiseCollectedEventHandler, Iterable[PromiseCollectedEventHandler]] = (),
+        on_node_collected: Union[NodeCollectedEventHandler, Iterable[NodeCollectedEventHandler]] = (),
     ) -> None:
         self.parent = self._current.get()
+
         self.on_promise_collected_handlers: list[PromiseCollectedEventHandler] = (
-            [on_promise_collected] if callable(on_promise_collected) else list(on_promise_collected)
+            [self._schedule_node_collected_event, on_promise_collected]
+            if callable(on_promise_collected)
+            else [self._schedule_node_collected_event, *on_promise_collected]
+        )
+        self.on_node_collected_handlers: list[NodeCollectedEventHandler] = (
+            [on_node_collected] if callable(on_node_collected) else list(on_node_collected)
         )
         self.child_tasks: set[Task] = set()
 
         self.schedule_immediately_by_default = schedule_immediately_by_default
         self.producer_capture_errors_by_default = producer_capture_errors_by_default
         self.longer_node_hash_keys = longer_node_hash_keys
 
         self._previous_ctx_token: Optional[contextvars.Token] = None
 
     @classmethod
-    def get_current(cls) -> "PromiseContext":
+    def get_current(cls) -> "PromisingContext":
         """
         Get the current context. If no context is currently active, raise an error.
         """
         current = cls._current.get()
         if not current:
             raise RuntimeError(
                 f"No {cls.__name__} is currently active. Did you forget to do `async with {cls.__name__}():`?"
@@ -70,59 +85,93 @@
     def on_promise_collected(self, handler: PromiseCollectedEventHandler) -> PromiseCollectedEventHandler:
         """
         Add a handler to be called after a promise is collected.
         """
         self.on_promise_collected_handlers.append(handler)
         return handler
 
-    def schedule_task(self, awaitable: Awaitable) -> Task:
+    def on_node_collected(self, handler: NodeCollectedEventHandler) -> NodeCollectedEventHandler:
+        """
+        Add a handler to be called after a promise of type Node is collected.
+        """
+        self.on_node_collected_handlers.append(handler)
+        return handler
+
+    async def _schedule_node_collected_event(self, _, result: Any) -> None:
+        """
+        TODO Oleksandr: docstring
+        """
+        if not isinstance(result, Node):
+            return
+        # pylint: disable=protected-access
+        # noinspection PyProtectedMember
+        if result._node_collected_event_triggered:
+            return
+
+        for handler in self.on_node_collected_handlers:
+            self.schedule_task(handler(_, result))
+        result._node_collected_event_triggered = True
+
+    def schedule_task(self, awaitable: Awaitable, suppress_errors: bool = False) -> Task:
         """
         Schedule a task in the current context. "Scheduling" a task this way instead of just creating it with
         `asyncio.create_task()` allows the context to keep track of the child tasks and to wait for them to finish
         before finalizing the context.
         """
 
         async def awaitable_wrapper() -> Any:
+            # noinspection PyBroadException
             try:
                 return await awaitable
-                # TODO Oleksandr: memorize exceptions so they can be raised when PromiseContext is finalized ?
-                #  HUGE NO! that would be a memory leak
+            except BaseException:  # pylint: disable=broad-except
+                if suppress_errors:
+                    logger.debug("AN ERROR OCCURRED IN A SCHEDULED TASK BUT WAS SUPPRESSED", exc_info=True)
+                else:
+                    raise
             finally:
                 self.child_tasks.remove(task)
 
         task = asyncio.create_task(awaitable_wrapper())
         self.child_tasks.add(task)
         return task
 
-    def activate(self) -> "PromiseContext":
+    def activate(self) -> "PromisingContext":
         """
         Activate the context. This is a context manager method that is used to activate the context for the duration
         of the `async with` block. Can be called as a regular method as well in cases where it is not possible to use
-        the `async with` block (e.g., if a PromiseContext needs to be activated for the duration of an async webserver
+        the `async with` block (e.g., if a PromisingContext needs to be activated for the duration of an async webserver
         being up).
         """
         if self._previous_ctx_token:
-            raise RuntimeError("PromiseContext is not reentrant")
+            raise RuntimeError("PromisingContext is not reentrant")
         self._previous_ctx_token = self._current.set(self)  # <- this is the context switch
         return self
 
-    async def afinalize(self) -> None:
+    async def aflush_tasks(self) -> None:
         """
-        Finalize the context (wait for all the child tasks to finish and reset the context). This method is called
-        automatically at the end of the `async with` block.
+        Wait for all the child tasks to finish. This is useful when you want to wait for all the child tasks to finish
+        before proceeding with the rest of the code.
         """
+        # TODO Oleksandr: introduce `raise_if_errors` flag ?
         while self.child_tasks:
             await asyncio.gather(
                 *self.child_tasks,
                 return_exceptions=True,  # this prevents waiting until the first exception and then giving up
             )  # TODO Oleksandr: log exceptions that `gather` may return ?
+
+    async def afinalize(self) -> None:
+        """
+        Finalize the context (wait for all the child tasks to finish and reset the context). This method is called
+        automatically at the end of the `async with` block.
+        """
+        await self.aflush_tasks()
         self._current.reset(self._previous_ctx_token)
         self._previous_ctx_token = None
 
-    async def __aenter__(self) -> "PromiseContext":
+    async def __aenter__(self) -> "PromisingContext":
         return self.activate()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         await self.afinalize()
 
 
 class Promise(Generic[T]):
@@ -133,32 +182,32 @@
     def __init__(
         self,
         schedule_immediately: Union[bool, Sentinel] = DEFAULT,
         fulfiller: Optional[PromiseFulfiller[T]] = None,
         prefill_result: Union[Optional[T], Sentinel] = NO_VALUE,
     ) -> None:
         # TODO Oleksandr: raise an error if both prefilled_whole and packager are set (or both are not set)
-        promise_context = PromiseContext.get_current()
+        promising_context = PromisingContext.get_current()
 
         if schedule_immediately is DEFAULT:
-            schedule_immediately = promise_context.schedule_immediately_by_default
+            schedule_immediately = promising_context.schedule_immediately_by_default
 
         self.__fulfiller = fulfiller
 
         if prefill_result is NO_VALUE:
             # NO_VALUE is used because `None` is also a legitimate value
             self._result: Union[T, Sentinel, BaseException] = NO_VALUE
         else:
             self._result = prefill_result
             self._schedule_collected_event_handlers()
 
         self._fulfiller_lock = asyncio.Lock()
 
         if schedule_immediately and prefill_result is NO_VALUE:
-            promise_context.schedule_task(self.acollect())
+            promising_context.schedule_task(self.acollect())
 
     async def acollect(self) -> T:
         """
         TODO Oleksandr: update this docstring
         "Accumulates" all the pieces of the stream and returns the "whole" value. Will return the exact
         same object (the exact same instance) if called multiple times on the same instance of `StreamedPromise`.
         """
@@ -175,19 +224,19 @@
                     self._schedule_collected_event_handlers()
 
         if isinstance(self._result, BaseException):
             raise self._result
         return self._result
 
     def _schedule_collected_event_handlers(self):
-        promise_ctx = PromiseContext.get_current()
-        while promise_ctx:
-            for handler in promise_ctx.on_promise_collected_handlers:
-                promise_ctx.schedule_task(handler(self, self._result))
-            promise_ctx = promise_ctx.parent
+        promising_context = PromisingContext.get_current()
+        while promising_context:
+            for handler in promising_context.on_promise_collected_handlers:
+                promising_context.schedule_task(handler(self, self._result))
+            promising_context = promising_context.parent
 
 
 class StreamedPromise(Generic[PIECE, WHOLE], Promise[WHOLE]):
     """
     A StreamedPromise represents a promise of a whole value that can be streamed piece by piece.
 
     The StreamedPromise allows for "replaying" the stream of pieces without involving the producer
@@ -197,27 +246,27 @@
 
     :param producer: A callable that returns an async iterator yielding the pieces of the whole value.
     :param packager: A callable that takes an async iterable of pieces and returns the whole value
                      ("packages" the pieces).
     TODO Oleksandr: explain the `schedule_immediately` parameter
     """
 
-    def __init__(  # pylint: disable=too-many-arguments
+    def __init__(
         self,
         schedule_immediately: Union[bool, Sentinel] = DEFAULT,
         producer: Optional[StreamedPieceProducer[PIECE]] = None,
         packager: Optional[StreamedWholePackager[WHOLE]] = None,
         prefill_pieces: Union[Optional[Iterable[PIECE]], Sentinel] = NO_VALUE,
         prefill_whole: Union[Optional[WHOLE], Sentinel] = NO_VALUE,
     ) -> None:
         # TODO Oleksandr: raise an error if both prefill_pieces and producer are set (or both are not set)
-        promise_context = PromiseContext.get_current()
+        promising_context = PromisingContext.get_current()
 
         if schedule_immediately is DEFAULT:
-            schedule_immediately = promise_context.schedule_immediately_by_default
+            schedule_immediately = promising_context.schedule_immediately_by_default
 
         super().__init__(
             schedule_immediately=schedule_immediately,
             fulfiller=packager,
             prefill_result=prefill_whole,
         )
         self.__producer = producer
@@ -229,15 +278,15 @@
 
         self._all_pieces_consumed = prefill_pieces is not NO_VALUE
         self._producer_lock = asyncio.Lock()
 
         if schedule_immediately and prefill_pieces is NO_VALUE:
             # start producing pieces at the earliest task switch (put them in a queue for further consumption)
             self._queue = asyncio.Queue()
-            promise_context.schedule_task(self._aproduce_the_stream())
+            promising_context.schedule_task(self._aproduce_the_stream())
         else:
             # each piece will be produced on demand (when the first consumer iterates over it and not earlier)
             self._queue = None
 
         self._producer_iterator: Union[Optional[AsyncIterator[PIECE]], Sentinel] = None
 
     def __aiter__(self) -> AsyncIterator[PIECE]:
@@ -345,15 +394,15 @@
     """
 
     def __init__(self, capture_errors: Union[bool, Sentinel] = DEFAULT) -> None:
         self._queue = asyncio.Queue()
         self._append_open = False
         self._append_closed = False
         if capture_errors is DEFAULT:
-            self._capture_errors = PromiseContext.get_current().producer_capture_errors_by_default
+            self._capture_errors = PromisingContext.get_current().producer_capture_errors_by_default
         else:
             self._capture_errors = capture_errors
 
     def __enter__(self) -> "AppendProducer":
         return self.open()
 
     def __exit__(
```

### Comparing `miniagents-0.0.7/miniagents/promisegraph/sequence.py` & `miniagents-0.0.8/miniagents/promising/sequence.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 The main class in this module is `FlatSequence`. See its docstring for more information.
 """
 
 from typing import Generic, AsyncIterator, Union
 
-from miniagents.promisegraph.promise import StreamedPromise
-from miniagents.promisegraph.sentinels import Sentinel, DEFAULT
-from miniagents.promisegraph.typing import SequenceFlattener, IN, OUT, StreamedPieceProducer
+from miniagents.promising.promising import StreamedPromise
+from miniagents.promising.sentinels import Sentinel, DEFAULT
+from miniagents.promising.typing import SequenceFlattener, IN, OUT, StreamedPieceProducer
 
 
 class FlatSequence(Generic[IN, OUT]):
     """
     TODO Oleksandr: produce a docstring for this class after you use it in the MiniAgents framework
     """
```

### Comparing `miniagents-0.0.7/miniagents/promisegraph/typing.py` & `miniagents-0.0.8/miniagents/promising/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """
-Types for the PromiseGraph part of the library.
+Types for the Promising part of the library.
 """
 
+import typing
 from typing import TypeVar, AsyncIterator, Protocol, Union, Any
 
+if typing.TYPE_CHECKING:
+    from miniagents.promising.node import Node
+
 T = TypeVar("T")
 PIECE = TypeVar("PIECE")
 WHOLE = TypeVar("WHOLE")
 IN = TypeVar("IN")
 OUT = TypeVar("OUT")
 PromiseBound = TypeVar("PromiseBound", bound="Promise")
 StreamedPromiseBound = TypeVar("StreamedPromiseBound", bound="StreamedPromise")
@@ -47,14 +51,22 @@
     scheduled to be called after StreamedPromise.acollect() finishes collecting the promise. "Scheduled" means
     that the function is passed to the event loop for execution without blocking the current coroutine.
     """
 
     async def __call__(self, promise: PromiseBound, result: Any) -> None: ...
 
 
+class NodeCollectedEventHandler(Protocol):
+    """
+    TODO Oleksandr: docstring
+    """
+
+    async def __call__(self, promise: PromiseBound, node: "Node") -> None: ...
+
+
 class SequenceFlattener(Protocol[IN, OUT]):
     """
     A protocol for sequence flatteners. A sequence flattener is a function that takes a single object of type `IN`
     and asynchronously converts it into zero or more objects of type `OUT`. In other words, it "flattens" a single
     `IN` into zero or more instances of `OUT`.
     """
```

### Comparing `miniagents-0.0.7/miniagents/utils.py` & `miniagents-0.0.8/miniagents/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Utility functions of the MiniAgents framework.
 """
 
 from typing import AsyncIterator, Any, Optional
 
-from miniagents.miniagents import MessageType, MessageSequence, MessagePromise
+from miniagents.miniagents import MessageType, MessageSequence, MessagePromise, Message
 
 
 def join_messages(
     messages: MessageType,
     delimiter: Optional[str] = "\n\n",
     strip_leading_newlines: bool = False,
     collect_original_message_hash_keys: bool = True,
-    message_metadata: Optional[dict[str, Any]] = None,
+    **message_metadata,
 ) -> MessagePromise:
     """
     Join multiple messages into a single message using a delimiter.
 
     :param messages: A list of messages to join.
     :param strip_leading_newlines: If True, leading newlines will be stripped from each message. Language models,
     when prompted in a certain way, may produce leading newlines in the response. This parameter allows you to
@@ -45,11 +45,10 @@
                     yield token
 
             if collect_original_message_hash_keys:
                 metadata_so_far["original_message_hash_keys"].append((await message_promise.acollect()).hash_key)
 
             first_message = False
 
-        if message_metadata:
-            metadata_so_far.update(message_metadata)
+        metadata_so_far.update(message_metadata)
 
-    return MessagePromise(message_token_producer=token_producer)
+    return Message.promise(message_token_producer=token_producer)
```

### Comparing `miniagents-0.0.7/pyproject.toml` & `miniagents-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 119
 
 [tool.coverage.run]
 branch = true
 
 [tool.poetry]
 name = "miniagents"
-version = "0.0.7"
+version = "0.0.8"
 description = """\
 TODO Oleksandr\
 """
 authors = ["Oleksandr Tereshchenko <toporok@gmail.com>"]
 homepage = "https://github.com/teremterem/MiniAgents"
 readme = "README.md"
 license = "MIT"
```

### Comparing `miniagents-0.0.7/PKG-INFO` & `miniagents-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniagents
-Version: 0.0.7
+Version: 0.0.8
 Summary: TODO Oleksandr
 Home-page: https://github.com/teremterem/MiniAgents
 License: MIT
 Author: Oleksandr Tereshchenko
 Author-email: toporok@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

