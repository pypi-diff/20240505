# Comparing `tmp/sae_lens-1.3.0.tar.gz` & `tmp/sae_lens-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-1.3.0.tar", max compression
+gzip compressed data, was "sae_lens-1.4.0.tar", max compression
```

## Comparing `sae_lens-1.3.0.tar` & `sae_lens-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-05-03 10:11:03.016341 sae_lens-1.3.0/LICENSE
--rw-r--r--   0        0        0     2553 2024-05-03 10:11:03.016341 sae_lens-1.3.0/README.md
--rw-r--r--   0        0        0     1889 2024-05-03 10:11:04.744338 sae_lens-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      943 2024-05-03 10:11:04.744338 sae_lens-1.3.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    17062 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20134 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     1164 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0        0 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     2674 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     6643 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0        0 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    16793 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2849 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0    10112 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     6169 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     1528 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1020 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     3675 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8266 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2319 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    17403 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    19601 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1628 2024-05-03 10:11:03.028341 sae_lens-1.3.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     4147 1970-01-01 00:00:00.000000 sae_lens-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-05 00:47:08.104824 sae_lens-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2553 2024-05-05 00:47:08.104824 sae_lens-1.4.0/README.md
+-rw-r--r--   0        0        0     1889 2024-05-05 00:47:09.224817 sae_lens-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-05-05 00:47:09.224817 sae_lens-1.4.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 00:47:08.112824 sae_lens-1.4.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-05-05 00:47:08.112824 sae_lens-1.4.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-05-05 00:47:08.112824 sae_lens-1.4.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    17062 2024-05-05 00:47:08.112824 sae_lens-1.4.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20134 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     1164 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0        0 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     2674 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     6643 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0        0 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    18342 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     2849 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0    12089 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6169 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     3008 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1020 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     3675 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8284 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2319 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    17503 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    28498 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0     1628 2024-05-05 00:47:08.116824 sae_lens-1.4.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     4147 1970-01-01 00:00:00.000000 sae_lens-1.4.0/PKG-INFO
```

### Comparing `sae_lens-1.3.0/LICENSE` & `sae_lens-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/README.md` & `sae_lens-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/pyproject.toml` & `sae_lens-1.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "1.3.0"
+version = "1.4.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `sae_lens-1.3.0/sae_lens/__init__.py` & `sae_lens-1.4.0/sae_lens/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.0"
+__version__ = "1.4.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import cache_activations_runner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-1.3.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-1.4.0/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-1.4.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-1.4.0/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-1.4.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/analysis/tsea.py` & `sae_lens-1.4.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/pretrained_saes.yaml` & `sae_lens-1.4.0/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/toolkit/pretrained_sae_loaders.py` & `sae_lens-1.4.0/sae_lens/toolkit/pretrained_sae_loaders.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-1.4.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-1.4.0/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/training/activations_store.py` & `sae_lens-1.4.0/sae_lens/training/activations_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import os
 from typing import Any, Iterator, Literal, TypeVar, cast
 
 import torch
+import tqdm
 from datasets import (
     Dataset,
     DatasetDict,
     IterableDataset,
     IterableDatasetDict,
     load_dataset,
 )
+from safetensors.torch import load_file, save_file
 from torch.utils.data import DataLoader
 from transformer_lens.hook_points import HookedRootModule
 
 from sae_lens.training.config import (
     CacheActivationsRunnerConfig,
     LanguageModelSAERunnerConfig,
 )
@@ -107,14 +109,15 @@
         self.store_batch_size = store_batch_size
         self.train_batch_size = train_batch_size
         self.prepend_bos = prepend_bos
         self.device = device
         self.dtype = dtype
         self.cached_activations_path = cached_activations_path
 
+        self.n_dataset_processed = 0
         self.iterable_dataset = iter(self.dataset)
 
         # Check if dataset is tokenized
         dataset_sample = next(self.iterable_dataset)
 
         # check if it's tokenized
         if "tokens" in dataset_sample.keys():
@@ -398,14 +401,52 @@
             # Try to get the next batch
             return next(self.dataloader)
         except StopIteration:
             # If the DataLoader is exhausted, create a new one
             self._dataloader = self.get_data_loader()
             return next(self.dataloader)
 
+    @classmethod
+    def load(
+        cls,
+        file_path: str,
+        model: HookedRootModule,
+        cfg: LanguageModelSAERunnerConfig | CacheActivationsRunnerConfig,
+        dataset: HfDataset | None = None,
+    ):
+        activation_store = cls.from_config(model=model, cfg=cfg, dataset=dataset)
+
+        state_dict = load_file(file_path)
+        if "storage_buffer" in state_dict.keys():
+            activation_store._storage_buffer = state_dict["storage_buffer"].to(
+                cfg.device
+            )
+        n_dataset_processed = state_dict["n_dataset_processed"].item()
+        # fastforward data
+        pbar = tqdm.tqdm(
+            total=n_dataset_processed - activation_store.n_dataset_processed,
+            desc="Fast forwarding data",
+        )
+        while activation_store.n_dataset_processed < n_dataset_processed:
+            next(activation_store.iterable_dataset)
+            pbar.update(1)
+            activation_store.n_dataset_processed += 1
+        return activation_store
+
+    def state_dict(self) -> dict[str, torch.Tensor]:
+        result = {
+            "n_dataset_processed": torch.tensor(self.n_dataset_processed),
+        }
+        if self._storage_buffer is not None:  # first time might be None
+            result["storage_buffer"] = self._storage_buffer
+        return result
+
+    def save(self, file_path: str):
+        save_file(self.state_dict(), file_path)
+
     def _get_next_dataset_tokens(self) -> torch.Tensor:
         device = self.device
         if not self.is_dataset_tokenized:
             s = next(self.iterable_dataset)[self.tokens_column]
             tokens = self.model.to_tokens(
                 s,
                 truncate=True,
@@ -423,14 +464,15 @@
                 requires_grad=False,
             )
             if (
                 not self.prepend_bos
                 and tokens[0] == self.model.tokenizer.bos_token_id  # type: ignore
             ):
                 tokens = tokens[1:]
+        self.n_dataset_processed += 1
         return tokens
 
 
 T = TypeVar("T")
 
 
 def listify(x: T | list[T]) -> list[T]:
```

### Comparing `sae_lens-1.3.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-1.4.0/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/training/config.py` & `sae_lens-1.4.0/sae_lens/training/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from dataclasses import dataclass, field
 from typing import Any, Optional, cast
 
 import torch
 import wandb
 
 from sae_lens import __version__
@@ -96,20 +97,24 @@
     feature_sampling_window: int = 2000
     dead_feature_window: int = 1000  # unless this window is larger feature sampling,
 
     dead_feature_threshold: float = 1e-8
 
     # WANDB
     log_to_wandb: bool = True
+    log_activations_store_to_wandb: bool = False
+    log_optimizer_state_to_wandb: bool = False
     wandb_project: str = "mats_sae_training_language_model"
+    wandb_id: Optional[str] = None
     run_name: Optional[str] = None
     wandb_entity: Optional[str] = None
     wandb_log_frequency: int = 10
 
     # Misc
+    resume: bool = False
     n_checkpoints: int = 0
     checkpoint_path: str = "checkpoints"
     verbose: bool = True
     model_kwargs: dict[str, Any] = field(default_factory=dict)
     sae_lens_version: str = field(default_factory=lambda: __version__)
     sae_lens_training_version: str = field(default_factory=lambda: __version__)
 
@@ -156,18 +161,19 @@
         self.device: str | torch.device = torch.device(self.device)
 
         if self.lr_end is None:
             if isinstance(self.lr, list):
                 self.lr_end = [lr / 10 for lr in self.lr]
             else:
                 self.lr_end = self.lr / 10
-
-        unique_id = cast(
-            Any, wandb
-        ).util.generate_id()  # not sure why this type is erroring
+        unique_id = self.wandb_id
+        if unique_id is None:
+            unique_id = cast(
+                Any, wandb
+            ).util.generate_id()  # not sure why this type is erroring
         self.checkpoint_path = f"{self.checkpoint_path}/{unique_id}"
 
         if self.verbose:
             print(
                 f"Run name: {self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.training_tokens:3.3e}"
             )
             # Print out some useful info:
@@ -206,14 +212,58 @@
             print(
                 f"Number tokens in sparsity calculation window: {self.feature_sampling_window * self.train_batch_size:.2e}"
             )
 
         if not isinstance(self.use_ghost_grads, list) and self.use_ghost_grads:
             print("Using Ghost Grads.")
 
+    def get_checkpoints_by_step(self) -> tuple[dict[int, str], bool]:
+        """
+        Returns (dict, is_done)
+        where dict is [steps] = path
+        for each checkpoint, and
+        is_done is True if there is a "final_{steps}" checkpoint
+        """
+        is_done = False
+        checkpoints = [
+            f
+            for f in os.listdir(self.checkpoint_path)
+            if os.path.isdir(os.path.join(self.checkpoint_path, f))
+        ]
+        mapped_to_steps = {}
+        for c in checkpoints:
+            try:
+                steps = int(c)
+            except ValueError:
+                if c.startswith("final"):
+                    steps = int(c.split("_")[1])
+                    is_done = True
+                else:
+                    continue  # ignore this directory
+            full_path = os.path.join(self.checkpoint_path, c)
+            mapped_to_steps[steps] = full_path
+        return mapped_to_steps, is_done
+
+    def get_resume_checkpoint_path(self) -> str:
+        """
+        Gets the checkpoint path with the most steps
+        raises StopIteration if the model is done (there is a final_{steps} directoryh
+        raises FileNotFoundError if there are no checkpoints found
+        """
+        mapped_to_steps, is_done = self.get_checkpoints_by_step()
+        if is_done:
+            raise StopIteration("Finished training model")
+        if len(mapped_to_steps) == 0:
+            raise FileNotFoundError("no checkpoints available to resume from")
+        else:
+            max_step = max(list(mapped_to_steps.keys()))
+            checkpoint_dir = mapped_to_steps[max_step]
+            print(f"resuming from step {max_step} at path {checkpoint_dir}")
+            return mapped_to_steps[max_step]
+
 
 @dataclass
 class CacheActivationsRunnerConfig:
     """
     Configuration for caching activations of an LLM.
     """
```

### Comparing `sae_lens-1.3.0/sae_lens/training/evals.py` & `sae_lens-1.4.0/sae_lens/training/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/training/geometric_median.py` & `sae_lens-1.4.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/training/load_model.py` & `sae_lens-1.4.0/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/training/optim.py` & `sae_lens-1.4.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/training/sae_group.py` & `sae_lens-1.4.0/sae_lens/training/sae_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             cfg_copy.hook_point = cfg_copy.hook_point.format(
                 layer=cfg_copy.hook_point_layer
             )
 
             sae = SparseAutoencoder(cfg_copy)
 
             sae_name = (
-                f"{sae.cfg.model_name}_{sae.cfg.hook_point}_{sae.cfg.d_sae}_"
+                f"{sae.cfg.model_name.replace('/', '_')}_{sae.cfg.hook_point}_{sae.cfg.d_sae}_"
                 + "_".join([f"{k}_{v}" for k, v in zip(keys, combination)])
             )
 
             # Create and store both the SparseAutoencoder instance and its parameters
             self.autoencoders[sae_name] = sae
 
     def __getitem__(self, key: str) -> SparseAutoencoder:
```

### Comparing `sae_lens-1.3.0/sae_lens/training/session_loader.py` & `sae_lens-1.4.0/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-1.4.0/sae_lens/training/sparse_autoencoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     load_pretrained_sae_lens_sae_components,
 )
 from sae_lens.toolkit.pretrained_saes_directory import get_pretrained_saes_directory
 from sae_lens.training.activation_functions import get_activation_fn
 from sae_lens.training.config import LanguageModelSAERunnerConfig
 from sae_lens.training.utils import BackwardsCompatiblePickleClass
 
+SPARSITY_PATH = "sparsity.safetensors"
+SAE_WEIGHTS_PATH = "sae_weights.safetensors"
+SAE_CFG_PATH = "cfg.json"
+
 
 class ForwardOutput(NamedTuple):
     sae_out: torch.Tensor
     feature_acts: torch.Tensor
     loss: torch.Tensor
     mse_loss: torch.Tensor
     l1_loss: torch.Tensor
@@ -194,15 +198,15 @@
                 sae_out=sae_out,
                 per_item_mse_loss=per_item_mse_loss,
                 hidden_pre=hidden_pre,
                 dead_neuron_mask=dead_neuron_mask,
             )
 
         mse_loss = per_item_mse_loss.mean()
-        sparsity = feature_acts.norm(p=self.lp_norm, dim=1).mean(dim=(0,))
+        sparsity = feature_acts.norm(p=self.lp_norm, dim=-1).mean()
         l1_loss = self.l1_coefficient * sparsity
         loss = mse_loss + l1_loss + ghost_grad_loss
 
         return ForwardOutput(
             sae_out=sae_out,
             feature_acts=feature_acts,
             loss=loss,
@@ -277,30 +281,30 @@
 
     def save_model(self, path: str, sparsity: Optional[torch.Tensor] = None):
 
         if not os.path.exists(path):
             os.mkdir(path)
 
         # generate the weights
-        save_file(self.state_dict(), f"{path}/sae_weights.safetensors")
+        save_file(self.state_dict(), f"{path}/{SAE_WEIGHTS_PATH}")
 
         # save the config
         config = {
             **self.cfg.__dict__,
             # some args may not be serializable by default
             "dtype": str(self.cfg.dtype),
             "device": str(self.cfg.device),
         }
 
-        with open(f"{path}/cfg.json", "w") as f:
+        with open(f"{path}/{SAE_CFG_PATH}", "w") as f:
             json.dump(config, f)
 
         if sparsity is not None:
             sparsity_in_dict = {"sparsity": sparsity}
-            save_file(sparsity_in_dict, f"{path}/sparsity.safetensors")  # type: ignore
+            save_file(sparsity_in_dict, f"{path}/{SPARSITY_PATH}")  # type: ignore
 
     @classmethod
     def load_from_pretrained_legacy(cls, path: str):
         """
         Load function for the model. Loads the model's state_dict and the config used to train it.
         This method can be called directly on the class, without needing an instance.
         """
```

### Comparing `sae_lens-1.3.0/sae_lens/training/toy_model_runner.py` & `sae_lens-1.4.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/training/toy_models.py` & `sae_lens-1.4.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-1.4.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 import os
-from dataclasses import dataclass
-from typing import Any, cast
+import pickle
+import random
+import signal
+from dataclasses import dataclass, field, fields
+from typing import Any, Optional, cast
 
+import numpy as np
 import torch
 import wandb
 from safetensors.torch import save_file
 from torch.optim import Adam, Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 from tqdm import tqdm
 from transformer_lens.hook_points import HookedRootModule
 
 from sae_lens import __version__
-from sae_lens.training.activations_store import ActivationsStore
+from sae_lens.training.activations_store import ActivationsStore, HfDataset
+from sae_lens.training.config import LanguageModelSAERunnerConfig
 from sae_lens.training.evals import run_evals
 from sae_lens.training.geometric_median import compute_geometric_median
 from sae_lens.training.optim import get_scheduler
 from sae_lens.training.sae_group import SparseAutoencoderDictionary
-from sae_lens.training.sparse_autoencoder import SparseAutoencoder
+from sae_lens.training.sparse_autoencoder import (
+    SAE_CFG_PATH,
+    SAE_WEIGHTS_PATH,
+    SPARSITY_PATH,
+    SparseAutoencoder,
+)
 
 # used to map between parameters which are updated during finetuning and the config str.
 FINETUNING_PARAMETERS = {
     "scale": ["scaling_factor"],
     "decoder": ["scaling_factor", "W_dec", "b_dec"],
     "unrotated_decoder": ["scaling_factor", "b_dec"],
 }
@@ -64,14 +74,102 @@
             if name in FINETUNING_PARAMETERS[sae.cfg.finetuning_method]:
                 param.requires_grad = True
             else:
                 param.requires_grad = False
 
         self.finetuning = True
 
+    def state_dict(self) -> dict[str, torch.Tensor]:
+        state_dict = {}
+        for attr in fields(self):
+            value = getattr(self, attr.name)
+            # serializable fields
+            if hasattr(value, "state_dict"):
+                state_dict[attr.name] = value.state_dict()
+            else:
+                state_dict[attr.name] = value
+        return state_dict
+
+    @classmethod
+    def load(cls, path: str, sae: SparseAutoencoder, total_training_steps: int):
+        with open(path, "rb") as f:
+            state_dict = pickle.load(f)
+        attached_ctx = _build_train_context(
+            sae=sae, total_training_steps=total_training_steps
+        )
+        for attr in fields(attached_ctx):
+            value = getattr(attached_ctx, attr.name)
+            # optimizer and scheduler, this attaches them properly
+            if hasattr(value, "state_dict"):
+                value.load_state_dict(state_dict[attr.name])
+                state_dict[attr.name] = value
+        ctx = cls(**state_dict)  # pyright: ignore [reportArgumentType]
+        # if fine tuning, we need to set sae requires grad properly
+        if ctx.finetuning:
+            ctx.begin_finetuning(sae=sae)
+        return ctx
+
+    def save(self, path: str):
+        with open(path, "wb") as f:
+            pickle.dump(self.state_dict(), f)
+
+
+@dataclass
+class SAETrainingRunState:
+    """
+    Training run state for all SAES
+    includes n_training_steps
+    n_training_tokens
+    started_fine_tuning
+    and rng states
+    """
+
+    n_training_steps: int = 0
+    n_training_tokens: int = 0
+    started_fine_tuning: bool = False
+    checkpoint_paths: list[str] = field(default_factory=list)
+    torch_state: Optional[torch.Tensor] = None
+    torch_cuda_state: Optional[list[torch.Tensor]] = None
+    numpy_state: Optional[
+        dict[str, Any]
+        | tuple[str, np.ndarray[Any, np.dtype[np.uint32]], int, int, float]
+    ] = None
+    random_state: Optional[Any] = None
+
+    def __post_init__(self):
+        if self.torch_state is None:
+            self.torch_state = torch.get_rng_state()
+        if self.torch_cuda_state is None:
+            self.torch_cuda_state = torch.cuda.get_rng_state_all()
+        if self.numpy_state is None:
+            self.numpy_state = np.random.get_state()
+        if self.random_state is None:
+            self.random_state = random.getstate()
+
+    def set_random_state(self):
+        assert self.torch_state is not None
+        torch.random.set_rng_state(self.torch_state)
+        assert self.torch_cuda_state is not None
+        torch.cuda.set_rng_state_all(self.torch_cuda_state)
+        assert self.numpy_state is not None
+        np.random.set_state(self.numpy_state)
+        assert self.random_state is not None
+        random.setstate(self.random_state)
+
+    @classmethod
+    def load(cls, path: str):
+        with open(path, "rb") as f:
+            attr_dict = pickle.load(f)
+        return cls(**attr_dict)
+
+    def save(self, path: str):
+        attr_dict = {**self.__dict__}
+        with open(path, "wb") as f:
+            pickle.dump(attr_dict, f)
+
 
 @dataclass
 class TrainSAEGroupOutput:
     sae_group: SparseAutoencoderDictionary
     checkpoint_paths: list[str]
     log_feature_sparsities: dict[str, torch.Tensor]
 
@@ -87,157 +185,203 @@
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
 ) -> SparseAutoencoderDictionary:
     """
     @deprecated Use `train_sae_group_on_language_model` instead. This method is kept for backward compatibility.
     """
     return train_sae_group_on_language_model(
-        model,
-        sae_group,
-        activation_store,
-        batch_size,
-        n_checkpoints,
-        feature_sampling_window,
-        use_wandb,
-        wandb_log_frequency,
+        model=model,
+        sae_group=sae_group,
+        activation_store=activation_store,
+        batch_size=batch_size,
+        n_checkpoints=n_checkpoints,
+        feature_sampling_window=feature_sampling_window,
+        use_wandb=use_wandb,
+        wandb_log_frequency=wandb_log_frequency,
     ).sae_group
 
 
+def get_total_training_tokens(sae_group: SparseAutoencoderDictionary) -> int:
+    return sae_group.cfg.training_tokens + sae_group.cfg.finetuning_tokens
+
+
 def train_sae_group_on_language_model(
     model: HookedRootModule,
     sae_group: SparseAutoencoderDictionary,
     activation_store: ActivationsStore,
+    train_contexts: Optional[dict[str, SAETrainContext]] = None,
+    training_run_state: Optional[SAETrainingRunState] = None,
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
 ) -> TrainSAEGroupOutput:
+    total_training_tokens = get_total_training_tokens(sae_group=sae_group)
     _update_sae_lens_training_version(sae_group)
-    total_training_tokens = (
-        sae_group.cfg.training_tokens + sae_group.cfg.finetuning_tokens
-    )
     total_training_steps = total_training_tokens // batch_size
-    n_training_steps = 0
-    n_training_tokens = 0
-    started_fine_tuning = False
 
     checkpoint_thresholds = []
     if n_checkpoints > 0:
         checkpoint_thresholds = list(
             range(0, total_training_tokens, total_training_tokens // n_checkpoints)
         )[1:]
 
     all_layers = sae_group.cfg.hook_point_layer
     if not isinstance(all_layers, list):
         all_layers = [all_layers]
 
-    train_contexts = {
-        name: _build_train_context(sae, total_training_steps)
-        for name, sae in sae_group.autoencoders.items()
-    }
-
-    _init_sae_group_b_decs(sae_group, activation_store, all_layers)
-
     pbar = tqdm(total=total_training_tokens, desc="Training SAE")
-    checkpoint_paths: list[str] = []
-    while n_training_tokens < total_training_tokens:
-        # Do a training step.
-        layer_acts = activation_store.next_batch()
-        n_training_tokens += batch_size
-
-        mse_losses: list[torch.Tensor] = []
-        l1_losses: list[torch.Tensor] = []
-
-        for name, sparse_autoencoder in sae_group.autoencoders.items():
-            ctx = train_contexts[name]
-            wandb_suffix = _wandb_log_suffix(sae_group.cfg, sparse_autoencoder.cfg)
-            step_output = _train_step(
-                sparse_autoencoder=sparse_autoencoder,
-                layer_acts=layer_acts,
-                ctx=ctx,
-                feature_sampling_window=feature_sampling_window,
-                use_wandb=use_wandb,
-                n_training_steps=n_training_steps,
-                all_layers=all_layers,
-                batch_size=batch_size,
-                wandb_suffix=wandb_suffix,
+
+    # not resuming
+    if training_run_state is None and train_contexts is None:
+        train_contexts = {
+            name: _build_train_context(sae, total_training_steps)
+            for name, sae in sae_group.autoencoders.items()
+        }
+        training_run_state = SAETrainingRunState()
+        _init_sae_group_b_decs(sae_group, activation_store, all_layers)
+    # resuming
+    else:
+        if train_contexts is None:
+            raise ValueError(
+                "train_contexts is None, when resuming, pass in training_run_state and train_contexts"
             )
-            mse_losses.append(step_output.mse_loss)
-            l1_losses.append(step_output.l1_loss)
-            if use_wandb:
-                with torch.no_grad():
-                    if (n_training_steps + 1) % wandb_log_frequency == 0:
-                        wandb.log(
-                            _build_train_step_log_dict(
-                                sparse_autoencoder,
-                                step_output,
-                                ctx,
-                                wandb_suffix,
-                                n_training_tokens,
-                            ),
-                            step=n_training_steps,
-                        )
-
-                    # record loss frequently, but not all the time.
-                    if (n_training_steps + 1) % (wandb_log_frequency * 10) == 0:
-                        sparse_autoencoder.eval()
-                        run_evals(
-                            sparse_autoencoder,
-                            activation_store,
-                            model,
-                            n_training_steps,
-                            suffix=wandb_suffix,
-                        )
-                        sparse_autoencoder.train()
-
-        # checkpoint if at checkpoint frequency
-        if checkpoint_thresholds and n_training_tokens > checkpoint_thresholds[0]:
-            checkpoint_path = _save_checkpoint(
-                sae_group,
-                train_contexts=train_contexts,
-                checkpoint_name=n_training_tokens,
+        if training_run_state is None:
+            raise ValueError(
+                "training_run_state is None, when resuming, pass in training_run_state and train_contexts"
             )
-            checkpoint_paths.append(checkpoint_path)
-            checkpoint_thresholds.pop(0)
+        pbar.update(training_run_state.n_training_tokens)
+        training_run_state.set_random_state()
 
-        ###############
+    class InterruptedException(Exception):
+        pass
 
-        n_training_steps += 1
-        pbar.set_description(
-            f"{n_training_steps}| MSE Loss {torch.stack(mse_losses).mean().item():.3f} | L1 {torch.stack(l1_losses).mean().item():.3f}"
-        )
-        pbar.update(batch_size)
+    def interrupt_callback(sig_num: Any, stack_frame: Any):
+        raise InterruptedException()
+
+    try:
+        # signal handlers (if preempted)
+        signal.signal(signal.SIGINT, interrupt_callback)
+        signal.signal(signal.SIGTERM, interrupt_callback)
+
+        while training_run_state.n_training_tokens < total_training_tokens:
+            # Do a training step.
+            layer_acts = activation_store.next_batch()
+            training_run_state.n_training_tokens += batch_size
+
+            mse_losses: list[torch.Tensor] = []
+            l1_losses: list[torch.Tensor] = []
 
-        ### If n_training_tokens > sae_group.cfg.training_tokens, then we should switch to fine-tuning (if we haven't already)
-        if (not started_fine_tuning) and (
-            n_training_tokens > sae_group.cfg.training_tokens
-        ):
-            started_fine_tuning = True
             for name, sparse_autoencoder in sae_group.autoencoders.items():
                 ctx = train_contexts[name]
-                # this should turn grads on for the scaling factor and other parameters.
-                ctx.begin_finetuning(sae_group.autoencoders[name])
+                wandb_suffix = _wandb_log_suffix(sae_group.cfg, sparse_autoencoder.cfg)
+                step_output = _train_step(
+                    sparse_autoencoder=sparse_autoencoder,
+                    layer_acts=layer_acts,
+                    ctx=ctx,
+                    feature_sampling_window=feature_sampling_window,
+                    use_wandb=use_wandb,
+                    n_training_steps=training_run_state.n_training_steps,
+                    all_layers=all_layers,
+                    batch_size=batch_size,
+                    wandb_suffix=wandb_suffix,
+                )
+                mse_losses.append(step_output.mse_loss)
+                l1_losses.append(step_output.l1_loss)
+                if use_wandb:
+                    with torch.no_grad():
+                        if (
+                            training_run_state.n_training_steps + 1
+                        ) % wandb_log_frequency == 0:
+                            wandb.log(
+                                _build_train_step_log_dict(
+                                    sparse_autoencoder,
+                                    step_output,
+                                    ctx,
+                                    wandb_suffix,
+                                    training_run_state.n_training_tokens,
+                                ),
+                                step=training_run_state.n_training_steps,
+                            )
+
+                        # record loss frequently, but not all the time.
+                        if (training_run_state.n_training_steps + 1) % (
+                            wandb_log_frequency * 10
+                        ) == 0:
+                            sparse_autoencoder.eval()
+                            run_evals(
+                                sparse_autoencoder,
+                                activation_store,
+                                model,
+                                training_run_state.n_training_steps,
+                                suffix=wandb_suffix,
+                            )
+                            sparse_autoencoder.train()
+
+            # checkpoint if at checkpoint frequency
+            if (
+                checkpoint_thresholds
+                and training_run_state.n_training_tokens > checkpoint_thresholds[0]
+            ):
+                _save_checkpoint(
+                    sae_group,
+                    activation_store=activation_store,
+                    train_contexts=train_contexts,
+                    training_run_state=training_run_state,
+                    checkpoint_name=training_run_state.n_training_tokens,
+                )
+                checkpoint_thresholds.pop(0)
+
+            ###############
+
+            training_run_state.n_training_steps += 1
+            pbar.set_description(
+                f"{training_run_state.n_training_steps}| MSE Loss {torch.stack(mse_losses).mean().item():.3f} | L1 {torch.stack(l1_losses).mean().item():.3f}"
+            )
+            pbar.update(batch_size)
 
+            ### If n_training_tokens > sae_group.cfg.training_tokens, then we should switch to fine-tuning (if we haven't already)
+            if (not training_run_state.started_fine_tuning) and (
+                training_run_state.n_training_tokens > sae_group.cfg.training_tokens
+            ):
+                training_run_state.started_fine_tuning = True
+                for name, sparse_autoencoder in sae_group.autoencoders.items():
+                    ctx = train_contexts[name]
+                    # this should turn grads on for the scaling factor and other parameters.
+                    ctx.begin_finetuning(sae_group.autoencoders[name])
+    except (KeyboardInterrupt, InterruptedException):
+        print("interrupted, saving progress")
+        checkpoint_name = training_run_state.n_training_tokens
+        _save_checkpoint(
+            sae_group,
+            activation_store=activation_store,
+            train_contexts=train_contexts,
+            training_run_state=training_run_state,
+            checkpoint_name=checkpoint_name,
+        )
+        print("done saving")
+        raise
     # save final sae group to checkpoints folder
-    final_checkpoint = _save_checkpoint(
+    _save_checkpoint(
         sae_group,
+        activation_store=activation_store,
         train_contexts=train_contexts,
-        checkpoint_name="final",
+        training_run_state=training_run_state,
+        checkpoint_name=f"final_{training_run_state.n_training_tokens}",
         wandb_aliases=["final_model"],
     )
-    checkpoint_paths.append(final_checkpoint)
 
     log_feature_sparsities = {
         name: ctx.log_feature_sparsity for name, ctx in train_contexts.items()
     }
 
     return TrainSAEGroupOutput(
         sae_group=sae_group,
-        checkpoint_paths=checkpoint_paths,
+        checkpoint_paths=training_run_state.checkpoint_paths,
         log_feature_sparsities=log_feature_sparsities,
     )
 
 
 def _wandb_log_suffix(cfg: Any, hyperparams: Any):
     # Create a mapping from cfg list keys to their corresponding hyperparams attributes
     key_mapping = {
@@ -500,43 +644,121 @@
         f"sparsity/mean_passes_since_fired{wandb_suffix}": ctx.n_forward_passes_since_fired.mean().item(),
         f"sparsity/dead_features{wandb_suffix}": ghost_grad_neuron_mask.sum().item(),
         f"details/current_learning_rate{wandb_suffix}": current_learning_rate,
         "details/n_training_tokens": n_training_tokens,
     }
 
 
+ACTIVATION_STORE_PATH = "activation_store.safetensors"
+TRAINING_RUN_STATE_PATH = "training_run_state.pkl"
+SAE_CONTEXT_PATH = "ctx.safetensors"
+
+
+def load_checkpoint(
+    checkpoint_path: str,
+    cfg: LanguageModelSAERunnerConfig,
+    model: HookedRootModule,
+    batch_size: int,
+    dataset: HfDataset | None = None,
+) -> tuple[
+    SAETrainingRunState,
+    ActivationsStore,
+    SparseAutoencoderDictionary,
+    dict[str, SAETrainContext],
+]:
+    training_run_state_path = f"{checkpoint_path}/{TRAINING_RUN_STATE_PATH}"
+    training_run_state = SAETrainingRunState.load(training_run_state_path)
+
+    activation_store_path = f"{checkpoint_path}/{ACTIVATION_STORE_PATH}"
+    activation_store = ActivationsStore.load(
+        activation_store_path, model=model, cfg=cfg, dataset=dataset
+    )
+
+    sae_group = SparseAutoencoderDictionary.load_from_pretrained(
+        checkpoint_path, device=str(cfg.device)
+    )
+
+    total_training_steps = get_total_training_tokens(sae_group=sae_group) // batch_size
+
+    train_contexts = {}
+    for name, sae in sae_group.autoencoders.items():
+        path = f"{checkpoint_path}/{name}"
+        ctx_path = f"{path}/{SAE_CONTEXT_PATH}"
+        train_contexts[name] = SAETrainContext.load(
+            ctx_path, sae=sae, total_training_steps=total_training_steps
+        )
+
+    # overwrite sae gruop cfg with our new cfg in case we want to change things
+    sae_group.cfg = cfg
+    # TODO: individual saes don't get new cfgs, maybe they should idk its messy bc of _init_autoencoders stuff
+    return training_run_state, activation_store, sae_group, train_contexts
+
+
 def _save_checkpoint(
     sae_group: SparseAutoencoderDictionary,
+    activation_store: ActivationsStore,
     train_contexts: dict[str, SAETrainContext],
+    training_run_state: SAETrainingRunState,
     checkpoint_name: int | str,
     wandb_aliases: list[str] | None = None,
 ) -> str:
 
     checkpoint_path = f"{sae_group.cfg.checkpoint_path}/{checkpoint_name}"
+    training_run_state.checkpoint_paths.append(checkpoint_path)
     os.makedirs(checkpoint_path, exist_ok=True)
+
+    training_run_state_path = f"{checkpoint_path}/{TRAINING_RUN_STATE_PATH}"
+    training_run_state.save(training_run_state_path)
+    if sae_group.cfg.log_to_wandb:
+        training_run_state_artifact = wandb.Artifact(
+            f"{sae_group.get_name()}_training_run_state",
+            type="training_run_state",
+            metadata=dict(sae_group.cfg.__dict__),
+        )
+        training_run_state_artifact.add_file(training_run_state_path)
+        # TODO: should these have aliases=wandb_aliases?
+        wandb.log_artifact(training_run_state_artifact)
+
+    activation_store_path = f"{checkpoint_path}/{ACTIVATION_STORE_PATH}"
+    activation_store.save(activation_store_path)
+    if sae_group.cfg.log_to_wandb and sae_group.cfg.log_activations_store_to_wandb:
+        activation_store_artifact = wandb.Artifact(
+            f"{sae_group.get_name()}_activations_store",
+            type="activation_store",
+            metadata=dict(sae_group.cfg.__dict__),
+        )
+        activation_store_artifact.add_file(activation_store_path)
+        wandb.log_artifact(activation_store_artifact)
+
     for name, sae in sae_group.autoencoders.items():
 
         ctx = train_contexts[name]
         path = f"{checkpoint_path}/{name}"
+        os.makedirs(path, exist_ok=True)
+        ctx_path = f"{path}/{SAE_CONTEXT_PATH}"
+        ctx.save(ctx_path)
+
         if sae.normalize_sae_decoder:
             sae.set_decoder_norm_to_unit_norm()
         sae.save_model(path)
         log_feature_sparsities = {"sparsity": ctx.log_feature_sparsity}
 
-        log_feature_sparsity_path = f"{path}/sparsity.safetensors"
+        log_feature_sparsity_path = f"{path}/{SPARSITY_PATH}"
         save_file(log_feature_sparsities, log_feature_sparsity_path)
 
         if sae_group.cfg.log_to_wandb and os.path.exists(log_feature_sparsity_path):
             model_artifact = wandb.Artifact(
                 f"{sae_group.get_name()}",
                 type="model",
                 metadata=dict(sae_group.cfg.__dict__),
             )
-            model_artifact.add_file(f"{path}/sae_weights.safetensors")
-            model_artifact.add_file(f"{path}/cfg.json")
+            model_artifact.add_file(f"{path}/{SAE_WEIGHTS_PATH}")
+            model_artifact.add_file(f"{path}/{SAE_CFG_PATH}")
+            if sae_group.cfg.log_optimizer_state_to_wandb:
+                model_artifact.add_file(ctx_path)
             wandb.log_artifact(model_artifact, aliases=wandb_aliases)
 
             sparsity_artifact = wandb.Artifact(
                 f"{sae_group.get_name()}_log_feature_sparsity",
                 type="log_feature_sparsity",
                 metadata=dict(sae_group.cfg.__dict__),
             )
```

### Comparing `sae_lens-1.3.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-1.4.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/sae_lens/training/utils.py` & `sae_lens-1.4.0/sae_lens/training/utils.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.3.0/PKG-INFO` & `sae_lens-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 1.3.0
+Version: 1.4.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

