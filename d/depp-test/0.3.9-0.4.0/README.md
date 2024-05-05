# Comparing `tmp/depp_test-0.3.9.tar.gz` & `tmp/depp_test-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depp_test-0.3.9.tar", last modified: Tue Jan  9 21:06:08 2024, max compression
+gzip compressed data, was "depp_test-0.4.0.tar", last modified: Sun May  5 09:20:01 2024, max compression
```

## Comparing `depp_test-0.3.9.tar` & `depp_test-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-01-09 21:06:08.100739 depp_test-0.3.9/
--rw-r--r--   0 yueyu      (501) staff       (20)     1067 2022-03-31 05:54:54.000000 depp_test-0.3.9/LICENSE
--rw-r--r--   0 yueyu      (501) staff       (20)      449 2024-01-09 21:06:08.100490 depp_test-0.3.9/PKG-INFO
--rw-r--r--   0 yueyu      (501) staff       (20)     9392 2022-08-16 00:49:49.000000 depp_test-0.3.9/README.md
--rw-r--r--   0 yueyu      (501) staff       (20)     1941 2023-04-27 23:37:10.000000 depp_test-0.3.9/agg_dist.py
--rw-r--r--   0 yueyu      (501) staff       (20)      577 2023-04-27 23:37:10.000000 depp_test-0.3.9/comb_json.py
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-01-09 21:06:08.098698 depp_test-0.3.9/depp/
--rw-r--r--   0 yueyu      (501) staff       (20)     5765 2024-01-04 18:06:29.000000 depp_test-0.3.9/depp/Agg_model.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4909 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/Agg_model_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5935 2022-03-31 06:34:25.000000 depp_test-0.3.9/depp/Model_new.py
--rw-r--r--   0 yueyu      (501) staff       (20)     8681 2024-01-04 18:00:11.000000 depp_test-0.3.9/depp/Model_pl.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5542 2022-03-31 06:34:25.000000 depp_test-0.3.9/depp/Model_pl.split.py
--rw-r--r--   0 yueyu      (501) staff       (20)    11301 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/Model_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)        0 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/__init__.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1605 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/assign_cluster_by_placement.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5019 2023-11-29 20:58:50.000000 depp_test-0.3.9/depp/combine_similar_seq.py
--rw-r--r--   0 yueyu      (501) staff       (20)      526 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/count_gapped_ratio.py
--rw-r--r--   0 yueyu      (501) staff       (20)    12673 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/data.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2431 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/data.split.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4009 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/data_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1730 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/default_config.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2433 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/depp_distance.py
--rw-r--r--   0 yueyu      (501) staff       (20)     2063 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/depp_distance_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1645 2022-03-31 06:34:25.000000 depp_test-0.3.9/depp/distance_correction.py
--rw-r--r--   0 yueyu      (501) staff       (20)      766 2023-04-27 23:36:52.000000 depp_test-0.3.9/depp/filter_by_entropy_gap.sh
--rw-r--r--   0 yueyu      (501) staff       (20)      782 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/get_names_by_entropy_gap.py
--rw-r--r--   0 yueyu      (501) staff       (20)      873 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/get_tree_dist.py
--rw-r--r--   0 yueyu      (501) staff       (20)      576 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/grep_jplace.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1008 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/grep_seq.py
--rw-r--r--   0 yueyu      (501) staff       (20)      909 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/grep_seq_group.py
--rw-r--r--   0 yueyu      (501) staff       (20)      743 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/select_placement.py
--rw-------   0 yueyu      (501) staff       (20)      895 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/select_species_by_distance.py
--rw-r--r--   0 yueyu      (501) staff       (20)      366 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/set_bl_one.py
--rw-r--r--   0 yueyu      (501) staff       (20)     7731 2023-04-27 23:36:57.000000 depp_test-0.3.9/depp/submodule.py
--rw-r--r--   0 yueyu      (501) staff       (20)     1578 2023-11-03 19:56:54.000000 depp_test-0.3.9/depp/test_scripts.py
--rw-r--r--   0 yueyu      (501) staff       (20)    37938 2024-01-04 18:03:17.000000 depp_test-0.3.9/depp/utils.py
--rw-r--r--   0 yueyu      (501) staff       (20)     4245 2023-11-29 00:27:08.000000 depp_test-0.3.9/depp-place-rRNA-one-type.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     6648 2024-01-09 21:05:22.000000 depp_test-0.3.9/depp-place-rRNA.sh
-drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-01-09 21:06:08.099827 depp_test-0.3.9/depp_test.egg-info/
--rw-r--r--   0 yueyu      (501) staff       (20)      449 2024-01-09 21:06:07.000000 depp_test-0.3.9/depp_test.egg-info/PKG-INFO
--rw-r--r--   0 yueyu      (501) staff       (20)     1060 2024-01-09 21:06:08.000000 depp_test-0.3.9/depp_test.egg-info/SOURCES.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        1 2024-01-09 21:06:07.000000 depp_test-0.3.9/depp_test.egg-info/dependency_links.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        1 2022-03-31 15:15:32.000000 depp_test-0.3.9/depp_test.egg-info/not-zip-safe
--rw-r--r--   0 yueyu      (501) staff       (20)      155 2024-01-09 21:06:07.000000 depp_test-0.3.9/depp_test.egg-info/requires.txt
--rw-r--r--   0 yueyu      (501) staff       (20)        5 2024-01-09 21:06:07.000000 depp_test-0.3.9/depp_test.egg-info/top_level.txt
--rw-r--r--   0 yueyu      (501) staff       (20)     1149 2023-04-27 23:37:10.000000 depp_test-0.3.9/merge_json.py
--rwxr-xr-x   0 yueyu      (501) staff       (20)      912 2023-04-27 23:37:14.000000 depp_test-0.3.9/run_upp.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     2339 2023-04-27 23:37:10.000000 depp_test-0.3.9/seq_sep.py
--rw-r--r--   0 yueyu      (501) staff       (20)       38 2024-01-09 21:06:08.100801 depp_test-0.3.9/setup.cfg
--rw-r--r--   0 yueyu      (501) staff       (20)     2009 2024-01-09 21:05:48.000000 depp_test-0.3.9/setup.py
--rw-r--r--   0 yueyu      (501) staff       (20)     6976 2023-11-06 06:04:49.000000 depp_test-0.3.9/train_cluster_depp.sh
--rw-r--r--   0 yueyu      (501) staff       (20)     4773 2023-04-27 23:37:10.000000 depp_test-0.3.9/train_depp.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5033 2023-04-27 23:37:10.000000 depp_test-0.3.9/train_depp_recon.py
--rw-r--r--   0 yueyu      (501) staff       (20)     5173 2023-04-27 23:37:14.000000 depp_test-0.3.9/wol_placement.sh
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-05-05 09:20:01.554207 depp_test-0.4.0/
+-rw-r--r--   0 yueyu      (501) staff       (20)     1067 2022-03-31 05:54:54.000000 depp_test-0.4.0/LICENSE
+-rw-r--r--   0 yueyu      (501) staff       (20)      449 2024-05-05 09:20:01.554052 depp_test-0.4.0/PKG-INFO
+-rw-r--r--   0 yueyu      (501) staff       (20)     9392 2022-08-16 00:49:49.000000 depp_test-0.4.0/README.md
+-rw-r--r--   0 yueyu      (501) staff       (20)     1941 2023-04-27 23:37:10.000000 depp_test-0.4.0/agg_dist.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      577 2023-04-27 23:37:10.000000 depp_test-0.4.0/comb_json.py
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-05-05 09:20:01.552864 depp_test-0.4.0/depp/
+-rw-r--r--   0 yueyu      (501) staff       (20)     5765 2024-03-16 00:19:45.000000 depp_test-0.4.0/depp/Agg_model.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4909 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/Agg_model_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5935 2022-03-31 06:34:25.000000 depp_test-0.4.0/depp/Model_new.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     9942 2024-04-12 18:12:31.000000 depp_test-0.4.0/depp/Model_pl.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5542 2022-03-31 06:34:25.000000 depp_test-0.4.0/depp/Model_pl.split.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    11301 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/Model_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)        0 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/__init__.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1605 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/assign_cluster_by_placement.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5019 2023-11-29 20:58:50.000000 depp_test-0.4.0/depp/combine_similar_seq.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      526 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/count_gapped_ratio.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    13238 2024-02-14 03:55:22.000000 depp_test-0.4.0/depp/data.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2431 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/data.split.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4009 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/data_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1755 2024-04-30 08:19:07.000000 depp_test-0.4.0/depp/default_config.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2433 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/depp_distance.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     2063 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/depp_distance_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1645 2022-03-31 06:34:25.000000 depp_test-0.4.0/depp/distance_correction.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      766 2023-04-27 23:36:52.000000 depp_test-0.4.0/depp/filter_by_entropy_gap.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)      782 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/get_names_by_entropy_gap.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1555 2024-04-11 20:45:25.000000 depp_test-0.4.0/depp/get_read_data_by_masking.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      873 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/get_tree_dist.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      576 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/grep_jplace.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1008 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/grep_seq.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      909 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/grep_seq_group.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      743 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/select_placement.py
+-rw-------   0 yueyu      (501) staff       (20)      895 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/select_species_by_distance.py
+-rw-r--r--   0 yueyu      (501) staff       (20)      366 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/set_bl_one.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     7731 2023-04-27 23:36:57.000000 depp_test-0.4.0/depp/submodule.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     1578 2023-11-03 19:56:54.000000 depp_test-0.4.0/depp/test_scripts.py
+-rw-r--r--   0 yueyu      (501) staff       (20)    37936 2024-03-16 00:18:48.000000 depp_test-0.4.0/depp/utils.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     4236 2024-04-11 21:06:50.000000 depp_test-0.4.0/depp-place-rRNA-one-type.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     7527 2024-04-30 09:54:06.000000 depp_test-0.4.0/depp-place-rRNA.sh
+drwxr-xr-x   0 yueyu      (501) staff       (20)        0 2024-05-05 09:20:01.553819 depp_test-0.4.0/depp_test.egg-info/
+-rw-r--r--   0 yueyu      (501) staff       (20)      449 2024-05-05 09:20:01.000000 depp_test-0.4.0/depp_test.egg-info/PKG-INFO
+-rw-r--r--   0 yueyu      (501) staff       (20)     1093 2024-05-05 09:20:01.000000 depp_test-0.4.0/depp_test.egg-info/SOURCES.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        1 2024-05-05 09:20:01.000000 depp_test-0.4.0/depp_test.egg-info/dependency_links.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        1 2022-03-31 15:15:32.000000 depp_test-0.4.0/depp_test.egg-info/not-zip-safe
+-rw-r--r--   0 yueyu      (501) staff       (20)      155 2024-05-05 09:20:01.000000 depp_test-0.4.0/depp_test.egg-info/requires.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)        5 2024-05-05 09:20:01.000000 depp_test-0.4.0/depp_test.egg-info/top_level.txt
+-rw-r--r--   0 yueyu      (501) staff       (20)     1149 2023-04-27 23:37:10.000000 depp_test-0.4.0/merge_json.py
+-rwxr-xr-x   0 yueyu      (501) staff       (20)      912 2023-04-27 23:37:14.000000 depp_test-0.4.0/run_upp.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     2339 2023-04-27 23:37:10.000000 depp_test-0.4.0/seq_sep.py
+-rw-r--r--   0 yueyu      (501) staff       (20)       38 2024-05-05 09:20:01.554279 depp_test-0.4.0/setup.cfg
+-rw-r--r--   0 yueyu      (501) staff       (20)     2009 2024-05-05 09:19:42.000000 depp_test-0.4.0/setup.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     6976 2023-11-06 06:04:49.000000 depp_test-0.4.0/train_cluster_depp.sh
+-rw-r--r--   0 yueyu      (501) staff       (20)     4773 2023-04-27 23:37:10.000000 depp_test-0.4.0/train_depp.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5033 2023-04-27 23:37:10.000000 depp_test-0.4.0/train_depp_recon.py
+-rw-r--r--   0 yueyu      (501) staff       (20)     5173 2023-04-27 23:37:14.000000 depp_test-0.4.0/wol_placement.sh
```

### Comparing `depp_test-0.3.9/LICENSE` & `depp_test-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/README.md` & `depp_test-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/agg_dist.py` & `depp_test-0.4.0/agg_dist.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/comb_json.py` & `depp_test-0.4.0/comb_json.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/Agg_model.py` & `depp_test-0.4.0/depp/Agg_model.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/Agg_model_recon.py` & `depp_test-0.4.0/depp/Agg_model_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/Model_new.py` & `depp_test-0.4.0/depp/Model_new.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/Model_pl.py` & `depp_test-0.4.0/depp/Model_pl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import time
 
 import torch
 import os
 import math
 import torch.nn as nn
 from depp import submodule
 from depp import data
@@ -112,14 +113,39 @@
         else:
             self.training_classifier = False
         self.current_model = current_model
         self.counting = 0
 
         self.save_hyperparameters(self.hparams)
 
+
+    def get_distance_ratio(self):
+        loader = DataLoader(self.train_data,
+                            batch_size=self.hparams.batch_size,
+                            num_workers=self.hparams.num_worker,
+                            shuffle=True,
+                            drop_last=True)
+        with torch.no_grad():
+            init_distance = []
+            for batch_idx, batch in enumerate(loader):
+                seq = batch['seqs'].float().to(self.device)
+                model_idx = batch['cluster_idx'].long()
+                encoding = self(seq, model_idx[0])
+                distance = utils.distance(encoding, encoding.detach(),
+                                          self.hparams.distance_mode)
+
+                not_self = torch.ones_like(distance)
+                not_self[torch.arange(0, len(distance)), torch.arange(0, len(distance))] = 0
+                init_distance.append(distance[not_self == 1])
+            init_distance = torch.cat(init_distance)
+            mean_init_distance = init_distance.mean()
+        mean_tree_distance = np.sqrt(self.train_data.distance_matrix.values).mean().mean()
+        self.encoder.distance_ratio[:] = (mean_tree_distance / mean_init_distance).item()
+
+
     def forward(self, x, model_idx=None) -> torch.Tensor:
         if self.training_classifier:
             return self.classifier(x)
         return self.encoder(x)
 
     def training_step(self, batch, batch_idx):
 
@@ -133,15 +159,15 @@
             loss = nn.functional.cross_entropy(c, model_idx)
             self.val_loss += loss
             return {'loss': loss}
         else:
             encoding = self(seq, model_idx[0])
             gt_distance = self.train_data.true_distance(nodes, nodes).to(device)
 
-            distance = utils.distance(encoding, encoding.detach(), self.hparams.distance_mode)
+            distance = utils.distance(encoding, encoding.detach(), self.hparams.distance_mode) * self.hparams.distance_ratio
 
             not_self = torch.ones_like(distance)
             not_self[torch.arange(0, len(distance)), torch.arange(0, len(distance))] = 0
 
             dis_loss = utils.mse_loss(distance[not_self == 1], gt_distance[not_self == 1], self.hparams.weighted_method)
             loss = self.dis_loss_w * dis_loss * self.hparams.dis_loss_ratio
 
@@ -194,14 +220,15 @@
     def val_dataloader(self):
         # TODO: do a real train/val split
         # self.train_data = data.data(self.hparams, calculate_distance_matrix=True)
         # self.train_data_list = data.make_datalist(self.hparams)
         if not self.training_classifier:
             print(f'training {self.current_model} model...')
             self.train_data = data.get_data(self.current_model, self.hparams)
+
         else:
             # self.train_data = self.train_data_list[-1]
             print(f'training classifier...')
             self.train_data = data.get_data(-1, self.hparams)
         loader = DataLoader(self.train_data,
                             batch_size=self.hparams.batch_size,
                             shuffle=False,
```

### Comparing `depp_test-0.3.9/depp/Model_pl.split.py` & `depp_test-0.4.0/depp/Model_pl.split.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/Model_recon.py` & `depp_test-0.4.0/depp/Model_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/assign_cluster_by_placement.py` & `depp_test-0.4.0/depp/assign_cluster_by_placement.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/combine_similar_seq.py` & `depp_test-0.4.0/depp/combine_similar_seq.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/count_gapped_ratio.py` & `depp_test-0.4.0/depp/count_gapped_ratio.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/data.py` & `depp_test-0.4.0/depp/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-
+import collections
 import os
 import torch
 import treeswift
 import numpy as np
 import pandas as pd
 from depp import utils
 from torch.utils.data import Dataset
@@ -33,14 +33,15 @@
 
 class data(Dataset):
     def __init__(self, args, backbone_tree_file, backbone_seq_file, idx, calculate_distance_matrix=False):
         self.args = args
         print('Loding data...')
         self_seq = SeqIO.to_dict(SeqIO.parse(backbone_seq_file, "fasta"))
         tree = treeswift.read_tree(backbone_tree_file, 'newick')
+        self.tree = tree
 
 #        self.nodes = list(self_seq.keys())
 
         print('finish data loading!')
 
         args.sequence_length = len(list(self_seq.values())[0])
         L = args.sequence_length
@@ -48,16 +49,26 @@
         if calculate_distance_matrix:
             print('Calculating distance matrix...')
             self.distance_matrix = tree.distance_matrix(leaf_labels=True)
             for key in self.distance_matrix:
                 self.distance_matrix[key][key] = 0
             self.distance_matrix = pd.DataFrame.from_dict(self.distance_matrix)
             print('Finish distance matrix calculation!')
-        self.nodes, self.seq = utils.process_seq(self_seq, args, True)
-        self.seq = dict(zip(self.nodes, self.seq))
+        self.nodes, self.seq = utils.process_seq(self_seq, args, False)
+        nodes2, seq2 = utils.process_seq(self_seq, args, True)
+        seq_tmp = collections.defaultdict(list)
+        for i, n in enumerate(self.nodes):
+            seq_tmp[n.split('_')[0].split('splithere')[0]].append(self.seq[i])
+        for i, n in enumerate(nodes2):
+            if n not in seq_tmp:
+                print('Error!')
+            # seq_tmp[n].append(seq2[i])
+            seq_tmp[n] = [seq2[i]]
+        # self.seq = dict(zip(self.nodes, self.seq))
+        self.seq, self.nodes = seq_tmp, list(seq_tmp.keys())
         self.model_idx = idx
 
     def true_distance(self, nodes1, nodes2):
         # gt_distance_list = itemgetter(*nodes1)(self.distance_matrix)
         # gt_distance = [torch.tensor(itemgetter(*nodes2)(item)).view(1, len(nodes2)) for item in gt_distance_list]
         # gt_distance = torch.cat(gt_distance, dim=0)
         gt_distance = self.distance_matrix.loc[nodes1][nodes2]
@@ -87,15 +98,15 @@
             sample['seqs'] = seq
             sample['seqs'][(mask != 1).repeat(4, 1)] = self.args.gap_encode
             sample['cluster_idx'] = self.model_idx
             return sample
         else:
             sample = {}
             node_name = self.nodes[idx]
-            seq = self.seq[node_name]
+            seq = self.seq[node_name][np.random.randint(len(self.seq[node_name]))]
             sample['seqs'] = seq
             sample['nodes'] = node_name
             sample['cluster_idx'] = self.model_idx
             return sample
 
     def __len__(self):
         return len(self.nodes)
```

### Comparing `depp_test-0.3.9/depp/data.split.py` & `depp_test-0.4.0/depp/data.split.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/data_recon.py` & `depp_test-0.4.0/depp/data_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/default_config.py` & `depp_test-0.4.0/depp/default_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 'end_model_idx': None,
 'cluster_num': 1,
 'seqdir': None,
 'use_cluster': None,
 'classifier_seqdir': None,
 'use_multi_class': None,
 'prob_thr': 5,
-'cluster_corr': None
+'cluster_corr': None,
+'train_mode': 'partial'
 }
 
 #def get_cfg_defaults():
 #    """Get a yacs CfgNode object with default values for my_project."""
 #    # Return a clone so that the defaults will not be altered
 #    # This is for the "local variable" use pattern
 #    return _C.clone()
```

### Comparing `depp_test-0.3.9/depp/depp_distance.py` & `depp_test-0.4.0/depp/depp_distance.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/depp_distance_recon.py` & `depp_test-0.4.0/depp/depp_distance_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/distance_correction.py` & `depp_test-0.4.0/depp/distance_correction.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/filter_by_entropy_gap.sh` & `depp_test-0.4.0/depp/filter_by_entropy_gap.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/get_names_by_entropy_gap.py` & `depp_test-0.4.0/depp/get_names_by_entropy_gap.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/get_tree_dist.py` & `depp_test-0.4.0/depp/get_tree_dist.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/grep_jplace.py` & `depp_test-0.4.0/depp/grep_jplace.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/grep_seq.py` & `depp_test-0.4.0/depp/grep_seq.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/grep_seq_group.py` & `depp_test-0.4.0/depp/grep_seq_group.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/select_placement.py` & `depp_test-0.4.0/depp/select_placement.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/select_species_by_distance.py` & `depp_test-0.4.0/depp/select_species_by_distance.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/submodule.py` & `depp_test-0.4.0/depp/submodule.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/test_scripts.py` & `depp_test-0.4.0/depp/test_scripts.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/depp/utils.py` & `depp_test-0.4.0/depp/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -838,9 +838,7 @@
 #     # data_origin.to_csv(os.path.join(dis_file_root, f'depp.csv'), sep='\t')
 #     # if not os.path.isdir(f'{args.outdir}/depp_tmp'):
 #     #     os.makedirs(f'{args.outdir}/depp_tmp')
 #     # with open(f'{args.outdir}/depp_tmp/seq_name.txt', 'w') as f:
 #     #     f.write("\n".join(query_seq_names) + '\n')
 #     print('original distanace matrix saved!')
 #     print("take {:.2f} seconds".format(t5-t1))
-
-
```

### Comparing `depp_test-0.3.9/depp-place-rRNA-one-type.sh` & `depp_test-0.4.0/depp-place-rRNA-one-type.sh`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 # check whether output directory exist
 if [ ! -d "$out_dir" ]; then
   echo "$out_dir not exist"
   exit 1
 fi
 
-echo "start ${data_type} data placement"
+echo "start query placement..."
 
 cp ${query_file} ${tmpdir}/
 
 # split large file into multiple small ones
 N=$(grep ">" ${query_file} | wc -l)
 mkdir ${tmpdir}/split_seq
 awk -v size=2000 -v pre=${tmpdir}/split_seq/seq -v pad="${#N}" '
```

### Comparing `depp_test-0.3.9/depp-place-rRNA.sh` & `depp_test-0.4.0/depp-place-rRNA.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,51 @@
 #!/bin/bash
 #
 #set -x
 #set -e
 #set -o
 
-while getopts q:a:o:t:x:d:s:l: flag
-do
+tmp_dir=$TMPDIR
+
+while getopts ":q:a:o:t:x:d:l:p:h" flag; do
     case "${flag}" in
-	q) query_file=${OPTARG};;
-	a) accessory_dir=${OPTARG};;
-  o) out_dir=${OPTARG};;
-  t) data_type=${OPTARG};;
-  x) cores=${OPTARG};;
-  d) debug=${OPTARG};;
-  l) align=${OPTARG};;
-#  s) script_dir=${OPTARG};;
+        q) query_file=${OPTARG} ;;
+        a) accessory_dir=${OPTARG} ;;
+        o) out_dir=${OPTARG} ;;
+        t) data_type=${OPTARG} ;;
+        x) cores=${OPTARG} ;;
+        d) debug=${OPTARG} ;;
+        l) align=${OPTARG} ;;
+        p) tmp_dir=${OPTARG} ;;
+        h)
+          echo "Usage: $(basename "$0") [options]"
+          echo "Options:"
+          echo "  -q  Specify query sequences file in FASTA format"
+          echo "  -a  Specify accessory directory"
+          echo "  -o  Specify output directory"
+          echo "  -t  Specify data type, (default: mixed)"
+          echo "  -x  Specify number of cores, (default: 1)"
+          echo "  -p  Specify TMPDIR, (default: system's TMPDIR)"
+          echo "  -h  Display this help message"
+          exit 0 ;;
+        \?)
+            echo "Invalid option: -$OPTARG" >&2
+            exit 1 ;;
+        :)
+            echo "Option -$OPTARG requires an argument." >&2
+            exit 1 ;;
     esac
 done
 
+TMPDIR=$tmp_dir
+echo "Use $TMPDIR as TEMPDIR"
+
 align="${align:-noalign}"
+data_type="${data_type:-mixed}"
+cores="${cores:-1}"
 # check if data type input is valid
 valid_data="16s_full_length 16s_v4_100 16s_v4_150 16s_v3_v4 mixed"
 #contains() {
 #  [[ $1 =~ (^|[[:space:]])$2($|[[:space:]]) ]] && exit(0) || exit(1)
 #}
 function notcontains(){
   local list="$1"
@@ -61,15 +84,15 @@
     export TMPDIR=/scratch/$USER/job_$SLURM_JOB_ID
   else
 #    echo "temporary file stores to $out_dir"
     TMPDIR=$(mktemp -d)
     mkdir -p ${TMPDIR}
     export TMPDIR=${TMPDIR}
   fi
-  tmpdir=`mktemp -d -t 'depp-tmp-XXXXXXXXXX'`
+  tmpdir=`mktemp -d -t 'depp-tmp-XXXXXXXX'`
   # check if the directory is created
   if [[ ! "$tmpdir" || ! -d "$tmpdir" ]]; then
     echo "Could not create temp dir"
     exit 1
   fi
   if [ $align == "noalign" ];
   then
@@ -78,15 +101,15 @@
 
     # align sequences
     echo "aligning the sequences..."
 
     # split query sequences into multiple files (/tmp directory)
     for i in ${tmpdir}/query_seq/*.fa;
     do
-      upptmpdir=`mktemp -d -t 'upp'`
+      upptmpdir=`mktemp -d -t 'upp-XXXXXXXX'`
       # check if the directory is created
       if [[ ! "$tmpdir" || ! -d "$tmpdir" ]]; then
         echo "Could not create temp dir"
         exit 1
       fi
       j="${i##*/}"
       dt="${j%.*}"
@@ -100,15 +123,15 @@
       cnt=0
       for i in ${upptmpdir}/seq*;
       do
         mkdir ${upptmpdir}/tmp
         mkdir ${upptmpdir}/tmp_result
         grep ">" ${i} | sed "s/^>//g" | sort > ${upptmpdir}/tmp_result/query_ids.txt
         upp_c=${cores}
-        witch.py -y -q ${i} -b ${accessory_dir}/${dt}_ao.fasta -e ${accessory_dir}/${dt}.nwk -o output_alignment.fasta -d ${upptmpdir}/tmp_result/ -t $upp_c
+        witch.py -y -k 4 -A 1000 -q ${i} -b ${accessory_dir}/${dt}_ao.fasta -e ${accessory_dir}/${dt}.nwk -o output_alignment.fasta -d ${upptmpdir}/tmp_result/ -t $upp_c
 #        grep -w -A 1 -f ${upptmpdir}/xtmp_result/query_ids.txt ${upptmpdir}/tmp_result/output_alignment_masked.fasta --no-group-separator > ${upptmpdir}/aligned/${cnt}.fa
         seqkit grep -w 0 -f ${upptmpdir}/tmp_result/query_ids.txt ${upptmpdir}/tmp_result/output_alignment.fasta.masked -o ${upptmpdir}/aligned/${cnt}.fa
         cnt=$((cnt+1))
         rm -rf ${upptmpdir}/tmp
         rm -rf ${upptmpdir}/tmp_result
       done
       cat ${upptmpdir}/aligned/*.fa > ${tmpdir}/${dt}_aligned.fa
@@ -159,15 +182,15 @@
     # check whether ssds for tmp files exist
 #    echo "use /scratch/$USER/job_$SLURM_JOB_ID as temporary directory"
     export TMPDIR=/scratch/$USER/job_$SLURM_JOB_ID
   else
 #    echo "temporary file stores to $out_dir"
     export TMPDIR=${out_dir}
   fi
-  tmpdir=`mktemp -d -t 'depp-tmp-XXXXXXXXXX'`
+  tmpdir=`mktemp -d -t 'depp-tmp-XXXXXXXX'`
   # check if the directory is created
   if [[ ! "$tmpdir" || ! -d "$tmpdir" ]]; then
     echo "Could not create temp dir"
     exit 1
   fi
   depp-place-rRNA-one-type.sh -q ${query_file} -a ${accessory_dir} -o ${tmpdir} -t $data_type -x ${cores}
   comb_json.py --indir ${tmpdir} --outfile ${tmpdir}/placement.jplace
```

### Comparing `depp_test-0.3.9/depp_test.egg-info/SOURCES.txt` & `depp_test-0.4.0/depp_test.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 depp/data_recon.py
 depp/default_config.py
 depp/depp_distance.py
 depp/depp_distance_recon.py
 depp/distance_correction.py
 depp/filter_by_entropy_gap.sh
 depp/get_names_by_entropy_gap.py
+depp/get_read_data_by_masking.py
 depp/get_tree_dist.py
 depp/grep_jplace.py
 depp/grep_seq.py
 depp/grep_seq_group.py
 depp/select_placement.py
 depp/select_species_by_distance.py
 depp/set_bl_one.py
```

### Comparing `depp_test-0.3.9/merge_json.py` & `depp_test-0.4.0/merge_json.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/run_upp.sh` & `depp_test-0.4.0/run_upp.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/seq_sep.py` & `depp_test-0.4.0/seq_sep.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/setup.py` & `depp_test-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name='depp_test',    # This is the name of your PyPI-package.
-        version='0.3.9',    # Update the version number for new releases
+        version='0.4.0',    # Update the version number for new releases
         scripts=['train_depp.py',
                  'depp/depp_distance.py',
                  'agg_dist.py',
                  'wol_placement.sh',
                  'run_upp.sh',
                  'merge_json.py',
                  'train_depp_recon.py',
```

### Comparing `depp_test-0.3.9/train_cluster_depp.sh` & `depp_test-0.4.0/train_cluster_depp.sh`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/train_depp.py` & `depp_test-0.4.0/train_depp.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/train_depp_recon.py` & `depp_test-0.4.0/train_depp_recon.py`

 * *Files identical despite different names*

### Comparing `depp_test-0.3.9/wol_placement.sh` & `depp_test-0.4.0/wol_placement.sh`

 * *Files identical despite different names*

