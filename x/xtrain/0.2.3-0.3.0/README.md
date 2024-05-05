# Comparing `tmp/xtrain-0.2.3.tar.gz` & `tmp/xtrain-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtrain-0.2.3.tar", max compression
+gzip compressed data, was "xtrain-0.3.0.tar", max compression
```

## Comparing `xtrain-0.2.3.tar` & `xtrain-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2024-05-03 20:13:02.317288 xtrain-0.2.3/LICENSE
--rw-r--r--   0        0        0     1231 2024-05-03 20:13:02.317288 xtrain-0.2.3/README.md
--rw-r--r--   0        0        0      833 2024-05-03 20:13:18.473312 xtrain-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      203 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/__init__.py
--rw-r--r--   0        0        0    11115 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/base_trainer.py
--rw-r--r--   0        0        0     3986 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/closure.py
--rw-r--r--   0        0        0     1631 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/loss.py
--rw-r--r--   0        0        0     4564 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/strategy.py
--rw-r--r--   0        0        0     5517 2024-05-03 20:13:02.321288 xtrain-0.2.3/xtrain/utils.py
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xtrain-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-05 14:14:46.587230 xtrain-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1231 2024-05-05 14:14:46.587230 xtrain-0.3.0/README.md
+-rw-r--r--   0        0        0      833 2024-05-05 14:15:03.595030 xtrain-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-05-05 14:14:46.591229 xtrain-0.3.0/xtrain/__init__.py
+-rw-r--r--   0        0        0    12105 2024-05-05 14:14:46.591229 xtrain-0.3.0/xtrain/base_trainer.py
+-rw-r--r--   0        0        0     3986 2024-05-05 14:14:46.591229 xtrain-0.3.0/xtrain/closure.py
+-rw-r--r--   0        0        0     1631 2024-05-05 14:14:46.591229 xtrain-0.3.0/xtrain/loss.py
+-rw-r--r--   0        0        0     4901 2024-05-05 14:14:46.591229 xtrain-0.3.0/xtrain/strategy.py
+-rw-r--r--   0        0        0     6210 2024-05-05 14:14:46.591229 xtrain-0.3.0/xtrain/utils.py
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xtrain-0.3.0/PKG-INFO
```

### Comparing `xtrain-0.2.3/LICENSE` & `xtrain-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.3/README.md` & `xtrain-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.3/pyproject.toml` & `xtrain-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtrain"
-version = "0.2.3"
+version = "0.3.0"
 description = "A Flax trainer"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 flax = "^0.8"
```

### Comparing `xtrain-0.2.3/xtrain/base_trainer.py` & `xtrain-0.3.0/xtrain/base_trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .loss import LossLog, LossFunc
 from .strategy import JIT
 from .utils import (
     Peekable,
     _get_name,
     unpack_prediction_and_state,
     unpack_x_y_sample_weight,
+    wrap_data_stream
 )
 
 @runtime_checkable
 class Metric(Protocol):
     def update(self, batch: Any, prediction: Any) -> Any:
         ...
 
@@ -72,14 +73,15 @@
 
     ctx: Trainer = struct.field(pytree_node=False)
     data: Iterator = struct.field(pytree_node=False)
     train_state: TrainState
     rngs: dict[str, RNG]
     loss_logs: tuple[LossLog]
     variables: dict = struct.field(default_factory=dict)
+    frozen: dict = struct.field(default_factory=dict, pytree_node=False)
 
     @property
     def parameters(self):
         return self.train_state.params
 
     @property
     def step(self):
@@ -158,14 +160,41 @@
 
         path.parent.mkdir(parents=True, exist_ok=True)
 
         with open(path, "wb") as f:
             pickle.dump((module, params), f)
 
 
+    def freeze(self, spec:str, *, unfreeze=False, ignore_key_error=False):
+        spec = spec.strip().strip("/").split("/")
+
+        if not ignore_key_error:
+            try:
+                sub = self.parameters
+                for k in spec:
+                    sub = sub[k]
+            except:
+                raise ValueError("The key {k} in the supplied spec doesn't exist.")
+
+        def _map_fn(path, x):
+            if len(path) < len(spec):
+                return x
+            for k, p in enumerate(path[:len(spec)]):
+                if p.key != spec[k]:
+                    return x
+
+            return not unfreeze
+
+        self.frozen = jax.tree_util.tree_map_with_path(
+            _map_fn, self.frozen
+        )
+    
+    def unfreeze(self, spec:str):
+        return self.freeze(spec, unfreeze=True)
+
 @dataclasses.dataclass
 class Trainer:
     """A general purpose FLAX model trainer. Help avoiding most of the biolerplate code when trainning with FLAX.
 
     Attributes:
         model: A Flax module
         losses: A collection of loss function ( loss_fn(batch:Any, prediction:Any)->float ).
@@ -229,19 +258,20 @@
             **kwargs: Additional keyward args passed to the model. E.g. "training=True"
 
         Returns:
             TrainIterator. Stepping through the iterator will train the model.
 
         """
         config = dataclasses.replace(self, strategy=strategy or self.strategy)
-        config.dataset = dataset
+
+        config.dataset = wrap_data_stream(dataset)
 
         assert config.strategy is not None
 
-        dataset_iter = Peekable(iter(dataset))
+        dataset_iter = Peekable(iter(config.dataset))
 
         seed = (
             self.seed
             if isinstance(self.seed, jnp.ndarray)
             else jax.random.PRNGKey(self.seed)
         )
 
@@ -256,34 +286,30 @@
             seed, key = jax.random.split(seed)
             keys = jax.random.split(seed, len(rng_cols) + 1)
             init_rngs = dict(zip(rng_cols + ["params"], keys))
 
             init_vars = self._initialize(init_rngs, dataset_iter)
 
         if frozen is None:
-            tx = self.optimizer
-        else:
             frozen = jax.tree_util.tree_map(lambda _: False, init_vars["params"])
-            optimizers = {True: optax.set_to_zero(), False: self.optimizer}
-            tx = optax.multi_transform(
-                optimizers,
-                frozen,
-            )
+        else:
+            if jax.tree_util.tree_structure(frozen) != jax.tree_util.tree_structure(init_vars["params"]):
+                raise ValueError(f"Invalid frozen dict. Its tree stucture is different from that of the model parameters")
 
         params = init_vars.pop("params")
         train_state = TrainState.create(
             apply_fn=_cached_partial(
                 self.model.apply,
                 mutable=self.mutable,
                 capture_intermediates=self.capture_intermediates,
                 method=method,
                 **kwargs,
             ),
             params=params,
-            tx=tx,
+            tx=self.optimizer,
         )
 
         losses = self.losses
         try:
             iter(losses)
         except:
             losses = (losses,)
@@ -292,14 +318,15 @@
         return TrainIterator(
             ctx=config,
             data=dataset_iter,
             train_state=train_state,
             rngs=rngs,
             loss_logs=loss_logs,
             variables=init_vars,
+            frozen=frozen,
         )
 
     def test(
         self,
         dataset: Iterable,
         metrics: METRICS,
         variables: dict,
```

### Comparing `xtrain-0.2.3/xtrain/closure.py` & `xtrain-0.3.0/xtrain/closure.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.3/xtrain/loss.py` & `xtrain-0.3.0/xtrain/loss.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.3/xtrain/strategy.py` & `xtrain-0.3.0/xtrain/strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,19 @@
         # print('JIT train_step')
         grads, (loss_logs, preds) = jax.grad(cls.loss_fn, has_aux=True)(
             train_obj.train_state.params,
             train_obj,
             batch,
         )
 
+        grads = jax.tree_util.tree_map(
+            lambda x, freeze: jax.numpy.zeros_like(x) if freeze else x,
+            grads, train_obj.frozen,
+        )
+
         state = train_obj.train_state.apply_gradients(grads=grads)
 
         return state, loss_logs, preds
 
 
 class Core(Eager):
     predict = jax.jit(Eager.predict, static_argnames="apply_fn")
@@ -113,14 +118,20 @@
         grads, (loss_logs, preds) = jax.grad(cls.loss_fn, has_aux=True)(
             train_obj.train_state.params,
             train_obj,
             batch,
         )
 
         grads = jax.lax.pmean(grads, axis_name="mapped")
+        
+        grads = jax.tree_util.tree_map(
+            lambda x, freeze: jax.numpy.zeros_like(x) if freeze else x,
+            grads, train_obj.frozen,
+        )
+        
         state = train_obj.train_state.apply_gradients(grads=grads)
 
         # aggregate logs
         loss_logs = jax.tree_map(partial(jax.lax.pmean, axis_name="mapped"), loss_logs)
 
         #         # sync batch statistics
         #         model.map(partial(jax.lax.pmean, axis_name="mapped"), tx.BatchStat, inplace=True)
```

### Comparing `xtrain-0.2.3/xtrain/utils.py` & `xtrain-0.3.0/xtrain/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -166,14 +166,18 @@
                     yield batch
 
             return parse_dataloader_gen()
 
         def __iter__(self):
             return self.get_dataset()
 
+        @classmethod
+        def is_adaptor_for(cls, data):
+            return isinstance(data, DataLoader)
+
 except ImportError:
     TorchDataLoaderAdapter = None
 
 
 try:
     from tensorflow.data import Dataset
 
@@ -187,26 +191,48 @@
         """
 
         def __init__(self, ds: Dataset):
             self._dataset = ds
 
         def __iter__(self):
             return self._dataset.as_numpy_iterator()
+    
+        @classmethod
+        def is_adaptor_for(cls, data):
+            return isinstance(data, Dataset)
 
 except ImportError:
     TFDatasetAdapter = None
 
 
 class GeneratorAdapter:
     def __init__(self, g):
         self._generator = g
 
     def __iter__(self):
         return self._generator()
 
+    @classmethod
+    def is_adaptor_for(cls, data):
+        # treat any callable as potentially a generator func
+        return callable(data)
+
+def wrap_data_stream(ds):
+    all_adaptors = [TFDatasetAdapter, TorchDataLoaderAdapter, GeneratorAdapter]
+
+    for adp in all_adaptors:
+        if adp is not None and adp.is_adaptor_for(ds):
+            return adp(ds)
+
+    try:
+        iter(ds)
+    except:
+        raise ValueError(f"Unrecognized datasource {ds}")
+
+    return ds
 
 class Peekable:
     def __init__(self, iterator):
         self.iterator = iterator
         self.peeked = deque()
 
     def __iter__(self):
```

### Comparing `xtrain-0.2.3/PKG-INFO` & `xtrain-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtrain
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Flax trainer
 Author: Ji Yu
 Author-email: jyu@uchc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

