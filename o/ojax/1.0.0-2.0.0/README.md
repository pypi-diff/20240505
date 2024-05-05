# Comparing `tmp/ojax-1.0.0.tar.gz` & `tmp/ojax-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ojax-1.0.0.tar", last modified: Sat May  4 15:28:18 2024, max compression
+gzip compressed data, was "ojax-2.0.0.tar", last modified: Sun May  5 16:16:35 2024, max compression
```

## Comparing `ojax-1.0.0.tar` & `ojax-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 sheny    (30818) tumuser  (20909)        0 2024-05-04 15:28:18.820884 ojax-1.0.0/
--rw-r--r--   0 sheny    (30818) tumuser  (20909)    11357 2024-04-26 12:42:34.000000 ojax-1.0.0/LICENSE
--rw-r--r--   0 sheny    (30818) tumuser  (20909)     4274 2024-05-04 15:28:18.816883 ojax-1.0.0/PKG-INFO
-drwxr-xr-x   0 sheny    (30818) tumuser  (20909)        0 2024-05-04 15:28:18.804883 ojax-1.0.0/ojax/
--rw-r--r--   0 sheny    (30818) tumuser  (20909)      233 2024-05-04 15:28:08.000000 ojax-1.0.0/ojax/__init__.py
--rw-r--r--   0 sheny    (30818) tumuser  (20909)     9770 2024-05-02 19:04:07.000000 ojax-1.0.0/ojax/otree.py
--rw-r--r--   0 sheny    (30818) tumuser  (20909)     3818 2024-05-02 19:07:32.000000 ojax-1.0.0/ojax/pureclass.py
--rw-r--r--   0 sheny    (30818) tumuser  (20909)        0 2023-07-28 17:48:19.000000 ojax-1.0.0/ojax/py.typed
-drwxr-xr-x   0 sheny    (30818) tumuser  (20909)        0 2024-05-04 15:28:18.816883 ojax-1.0.0/ojax.egg-info/
--rw-r--r--   0 sheny    (30818) tumuser  (20909)     4274 2024-05-04 15:28:18.000000 ojax-1.0.0/ojax.egg-info/PKG-INFO
--rw-r--r--   0 sheny    (30818) tumuser  (20909)      265 2024-05-04 15:28:18.000000 ojax-1.0.0/ojax.egg-info/SOURCES.txt
--rw-r--r--   0 sheny    (30818) tumuser  (20909)        1 2024-05-04 15:28:18.000000 ojax-1.0.0/ojax.egg-info/dependency_links.txt
--rw-r--r--   0 sheny    (30818) tumuser  (20909)       12 2024-05-04 15:28:18.000000 ojax-1.0.0/ojax.egg-info/requires.txt
--rw-r--r--   0 sheny    (30818) tumuser  (20909)        5 2024-05-04 15:28:18.000000 ojax-1.0.0/ojax.egg-info/top_level.txt
--rw-r--r--   0 sheny    (30818) tumuser  (20909)      507 2024-05-04 15:03:05.000000 ojax-1.0.0/pyproject.toml
--rw-r--r--   0 sheny    (30818) tumuser  (20909)     3976 2024-05-04 00:01:39.000000 ojax-1.0.0/readme.rst
--rw-r--r--   0 sheny    (30818) tumuser  (20909)       38 2024-05-04 15:28:18.820884 ojax-1.0.0/setup.cfg
--rw-------   0 sheny    (30818) tumuser  (20909)       96 2024-05-03 12:55:17.000000 ojax-1.0.0/setup.py
-drwxr-xr-x   0 sheny    (30818) tumuser  (20909)        0 2024-05-04 15:28:18.812883 ojax-1.0.0/test/
--rw-r--r--   0 sheny    (30818) tumuser  (20909)     2601 2024-05-02 17:44:03.000000 ojax-1.0.0/test/test_example.py
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-05 16:16:35.453082 ojax-2.0.0/
+-rw-rw-r--   0 ys        (1000) ys        (1000)    11357 2024-05-04 19:05:49.000000 ojax-2.0.0/LICENSE
+-rw-r--r--   0 ys        (1000) ys        (1000)     4266 2024-05-05 16:16:35.453082 ojax-2.0.0/PKG-INFO
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-05 16:16:35.453082 ojax-2.0.0/ojax/
+-rw-rw-r--   0 ys        (1000) ys        (1000)      245 2024-05-05 16:13:02.000000 ojax-2.0.0/ojax/__init__.py
+-rw-rw-r--   0 ys        (1000) ys        (1000)    11042 2024-05-05 16:13:02.000000 ojax-2.0.0/ojax/otree.py
+-rw-rw-r--   0 ys        (1000) ys        (1000)     3818 2024-05-04 19:05:49.000000 ojax-2.0.0/ojax/pureclass.py
+-rw-rw-r--   0 ys        (1000) ys        (1000)        0 2024-05-04 19:05:49.000000 ojax-2.0.0/ojax/py.typed
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-05 16:16:35.453082 ojax-2.0.0/ojax.egg-info/
+-rw-r--r--   0 ys        (1000) ys        (1000)     4266 2024-05-05 16:16:35.000000 ojax-2.0.0/ojax.egg-info/PKG-INFO
+-rw-rw-r--   0 ys        (1000) ys        (1000)      285 2024-05-05 16:16:35.000000 ojax-2.0.0/ojax.egg-info/SOURCES.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)        1 2024-05-05 16:16:35.000000 ojax-2.0.0/ojax.egg-info/dependency_links.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)        4 2024-05-05 16:16:35.000000 ojax-2.0.0/ojax.egg-info/requires.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)        5 2024-05-05 16:16:35.000000 ojax-2.0.0/ojax.egg-info/top_level.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)      498 2024-05-04 19:05:49.000000 ojax-2.0.0/pyproject.toml
+-rw-rw-r--   0 ys        (1000) ys        (1000)     3976 2024-05-05 14:48:35.000000 ojax-2.0.0/readme.rst
+-rw-rw-r--   0 ys        (1000) ys        (1000)       38 2024-05-05 16:16:35.453082 ojax-2.0.0/setup.cfg
+-rw-rw-r--   0 ys        (1000) ys        (1000)       96 2024-05-04 19:05:49.000000 ojax-2.0.0/setup.py
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-05 16:16:35.453082 ojax-2.0.0/tests/
+-rw-rw-r--   0 ys        (1000) ys        (1000)     2611 2024-05-05 16:13:02.000000 ojax-2.0.0/tests/test_example.py
+-rw-rw-r--   0 ys        (1000) ys        (1000)     5746 2024-05-05 16:13:02.000000 ojax-2.0.0/tests/test_ojax.py
```

### Comparing `ojax-1.0.0/LICENSE` & `ojax-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ojax-1.0.0/PKG-INFO` & `ojax-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ojax
-Version: 1.0.0
+Version: 2.0.0
 Summary: An extension for modular JAX code.
 Author: Yuesong Shen
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/ysngshn/ojax
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: jax>=0.4.26
+Requires-Dist: jax
 
 
 
 
 
 OJAX
 ====
```

### Comparing `ojax-1.0.0/ojax/otree.py` & `ojax-2.0.0/ojax/otree.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import (
     TypeVar,
     Optional,
+    Union,
     Sequence,
 )
 import enum
 import dataclasses
 import jax
 from . import pureclass
 
@@ -27,14 +28,50 @@
     Returns:
         The ``ojax.FieldType`` if available, and ``None`` otherwise.
     """
 
     return f.metadata.get("ojax-field-type")
 
 
+def fields(
+        otree: Union["OTree", "type(OTree)"],
+        field_type: Optional[FieldType] = None,
+        infer: bool = True,
+) -> tuple[dataclasses.Field, ...]:
+    """Convenience function extending dataclasses.fields() that can filter
+    fields by OTree field type.
+
+    Args:
+        otree: the OTree instance to examine.
+        field_type: if not None, specifies the field type to filter the list of
+            fields from OTree.
+        infer: determines if the field type should be inferred in case it is
+            not available. Has no effect when ``field_type = None``.
+
+    Returns:
+        A tuple of fields from the given OTree.
+    """
+
+    if field_type is not None and field_type not in FieldType:
+        raise ValueError(f"{field_type} is not a FieldType.")
+    t_fields = dataclasses.fields(otree)
+    if field_type is None:
+        return t_fields
+    else:
+        if infer:
+            return tuple(
+                f for f in t_fields
+                if otree.__infer_otree_field_type__(f) is field_type
+            )
+        else:
+            return tuple(
+                f for f in t_fields if get_field_type(f) is field_type
+            )
+
+
 def aux(
     *,
     default=dataclasses.MISSING,
     default_factory=dataclasses.MISSING,
     init=True,
     repr=True,
     hash=None,
@@ -181,27 +218,29 @@
             **kwargs: Keyword arguments specifying new values to be updated for
                 the corresponding child fields.
 
         Returns:
             New OTree instance with updated children.
         """
 
-        aux_names = set(
-            f.name
-            for f in dataclasses.fields(self)
-            if self.infer_field_type(f) is FieldType.AUX
-        )
-        aux_args = aux_names.intersection(kwargs.keys())
+        aux_args = set(
+            f.name for f in fields(self, FieldType.AUX, True)
+        ).intersection(kwargs.keys())
         if len(aux_args) != 0:
             raise ValueError(
                 f'update of keys {aux_args} not allowed, use "ojax.new()" '
-                f"instead to create instance of {self.__class__.__name__} with"
-                f" different PyTree structure."
+                f"instead to create new instances of {self.__class__.__name__}"
+                f" with updated auxiliary fields."
             )
+        child_names = set(
+            f.name for f in fields(self, FieldType.CHILD, True)
+        )
         for k, v in kwargs.items():
+            if k not in child_names:
+                continue
             old_v = object.__getattribute__(self, k)
             if jax.tree.structure(v) != jax.tree.structure(old_v):
                 raise ValueError(
                     f"PyTree structure mismatch at key {k}: "
                     f"expected\n{jax.tree.structure(old_v)}\n"
                     f"received\n{jax.tree.structure(v)}"
                 )
@@ -211,16 +250,16 @@
         self,
     ) -> tuple[tuple, tuple[tuple[tuple[str, int], ...], tuple]]:
         """Define the flatten behavior of OTree as a PyTree."""
 
         tree_leaves = []
         num_arrays = []
         aux_values = []
-        for f in dataclasses.fields(self):
-            name, ftype = f.name, self.infer_field_type(f)
+        for f in fields(self):
+            name, ftype = f.name, self.__infer_otree_field_type__(f)
             if ftype is FieldType.AUX:
                 aux_values.append(getattr(self, name))
                 num_arrays.append((name, 0))
             elif ftype is FieldType.CHILD:
                 entry = getattr(self, name)
                 entry_leaves, entry_aux = jax.tree.flatten(entry)
                 tree_leaves.extend(entry_leaves)
@@ -241,16 +280,16 @@
         """Define the unflatten behavior of OTree as a PyTree."""
         
         num_arrays, aux_values = aux_data
         num_arrays = dict(num_arrays)
         aux_values_iter = iter(aux_values)
         tree_children = {}
         offset = 0
-        for f in dataclasses.fields(cls):
-            name, ftype = f.name, cls.infer_field_type(f)
+        for f in fields(cls):
+            name, ftype = f.name, cls.__infer_otree_field_type__(f)
             if ftype is FieldType.AUX:
                 tree_children[name] = next(aux_values_iter)
             elif ftype is FieldType.CHILD:
                 count = num_arrays[name]
                 child_leaves = children[offset : offset + count]
                 tree_child = jax.tree.unflatten(
                     next(aux_values_iter), child_leaves
@@ -263,15 +302,15 @@
                 raise NotImplementedError
         # alternative to cls.__init__ since it might be custom
         otree = cls.__new__(cls)
         otree.assign_(**tree_children)
         return otree
 
     @classmethod
-    def infer_field_type(cls, f: dataclasses.Field) -> FieldType:
+    def __infer_otree_field_type__(cls, f: dataclasses.Field) -> FieldType:
         """Infer the OJAX field type from a :class:`dataclasses.Field` object.
 
         When :class:`ojax.FieldType` is unspecified (when
         :py:meth:`get_field_type` returns ``None``), the annotated ``f.type``
         is used for inference: for subclasses of :class:`jax.Array` and
         :class:`ojax.OTree` are assumed to be child fields and the rest are
         assumed to be auxiliary fields. You can override this method through
```

### Comparing `ojax-1.0.0/ojax/pureclass.py` & `ojax-2.0.0/ojax/pureclass.py`

 * *Files identical despite different names*

### Comparing `ojax-1.0.0/ojax.egg-info/PKG-INFO` & `ojax-2.0.0/ojax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ojax
-Version: 1.0.0
+Version: 2.0.0
 Summary: An extension for modular JAX code.
 Author: Yuesong Shen
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/ysngshn/ojax
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: jax>=0.4.26
+Requires-Dist: jax
 
 
 
 
 
 OJAX
 ====
```

### Comparing `ojax-1.0.0/readme.rst` & `ojax-2.0.0/readme.rst`

 * *Files identical despite different names*

### Comparing `ojax-1.0.0/test/test_example.py` & `ojax-2.0.0/tests/test_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from dataclasses import field, fields
+from dataclasses import field
 import jax
 import jax.numpy as jnp
 from jax.random import PRNGKey, split as jrsplit, normal as jrnormal
-from ojax import aux, child, OTree, get_field_type
+from ojax import aux, child, OTree, get_field_type, fields
 
 
 # defines a fully connected layer for neural networks
 class Dense(OTree):
     input_features: int  # inferred to be auxiliary data
     output_features: int = aux()  # or explicit declaration
     weight: jnp.ndarray = field(default=..., init=False)  # inferred as child
@@ -39,15 +39,15 @@
     # define layer
     init_weight = jrnormal(key_weight, shape=(output_features, data_features))
     init_bias = jrnormal(key_bias, shape=(output_features,))
     layer = Dense(data_features, output_features)
     # No inplace update, need to get the returned updated layer instance!
     layer = layer.update_parameters(weight=init_weight, bias=init_bias)
     for f in fields(layer):
-        print(f.name, get_field_type(f), OTree.infer_field_type(f))
+        print(f.name, get_field_type(f), OTree.__infer_otree_field_type__(f))
         # input_features None aux
         # output_features aux aux
         # weight None child
         # bias child child
     # use layer as a pytree
     layer_w, layer_b = jax.tree.flatten(layer)[0]
     assert (layer_w == init_weight).all() and (layer_b == init_bias).all()
```

