# Comparing `tmp/connectome_interpreter-1.7.0.tar.gz` & `tmp/connectome_interpreter-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.7.0.tar", last modified: Wed May  1 16:04:01 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.7.1.tar", last modified: Sun May  5 10:36:24 2024, max compression
```

## Comparing `connectome_interpreter-1.7.0.tar` & `connectome_interpreter-1.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 16:04:01.642562 connectome_interpreter-1.7.0/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.7.0/LICENSE
--rw-rw-rw-   0        0        0     1066 2024-05-01 16:04:01.641560 connectome_interpreter-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 16:04:01.595155 connectome_interpreter-1.7.0/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.7.0/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    35488 2024-05-01 12:12:06.000000 connectome_interpreter-1.7.0/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    22184 2024-05-01 14:15:27.000000 connectome_interpreter-1.7.0/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16135 2024-04-28 19:46:57.000000 connectome_interpreter-1.7.0/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    32941 2024-05-01 15:50:45.000000 connectome_interpreter-1.7.0/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-01 16:04:01.623706 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0     1066 2024-05-01 16:04:01.000000 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-05-01 16:04:01.000000 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 16:04:01.000000 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-05-01 16:04:01.000000 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-01 16:04:01.000000 connectome_interpreter-1.7.0/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 16:04:01.642562 connectome_interpreter-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     2068 2024-05-01 15:57:55.000000 connectome_interpreter-1.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-01 16:04:01.639411 connectome_interpreter-1.7.0/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.7.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.7.0/tests/test_compress_paths.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.7.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:36:24.700765 connectome_interpreter-1.7.1/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0     1066 2024-05-05 10:36:24.700765 connectome_interpreter-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 10:36:24.658359 connectome_interpreter-1.7.1/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.7.1/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    35488 2024-05-05 09:46:39.000000 connectome_interpreter-1.7.1/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    22184 2024-05-01 14:15:27.000000 connectome_interpreter-1.7.1/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16135 2024-04-28 19:46:57.000000 connectome_interpreter-1.7.1/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    32941 2024-05-01 16:25:53.000000 connectome_interpreter-1.7.1/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:36:24.694729 connectome_interpreter-1.7.1/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0     1066 2024-05-05 10:36:24.000000 connectome_interpreter-1.7.1/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-05-05 10:36:24.000000 connectome_interpreter-1.7.1/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 10:36:24.000000 connectome_interpreter-1.7.1/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-05-05 10:36:24.000000 connectome_interpreter-1.7.1/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-05 10:36:24.000000 connectome_interpreter-1.7.1/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 10:36:24.701765 connectome_interpreter-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     2068 2024-05-05 10:31:22.000000 connectome_interpreter-1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 10:36:24.698814 connectome_interpreter-1.7.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.7.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.7.1/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.7.1/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.7.0/LICENSE` & `connectome_interpreter-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.0/PKG-INFO` & `connectome_interpreter-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.7.0
+Version: 1.7.1
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
```

### Comparing `connectome_interpreter-1.7.0/README.md` & `connectome_interpreter-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.0/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.7.1/connectome_interpreter/activation_maximisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         threshold (float, optional): The threshold for activation of neurons. Defaults to 0.01.
     """
 
     def __init__(self, all_weights, sensory_indices, num_layers=2, threshold=0.01, tanh_steepness=5):
         super(MultilayeredNetwork, self).__init__()
 
         # num_neurons x num_neurons = 18k * 18k, ~1.2GB
-        self.all_weights = torch.nn.parameter.Parameter(all_weights)
+        self.all_weights = all_weights  # this does not require grad
         self.sensory_indices = torch.tensor(
             sensory_indices)  # shape: vector of sensory indices. These are the ones we manipulate
         self.num_layers = num_layers
         self.threshold = threshold
         self.tanh_steepness = tanh_steepness
         self.activations = []
```

### Comparing `connectome_interpreter-1.7.0/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.7.1/connectome_interpreter/compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.0/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.7.1/connectome_interpreter/path_finding.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.0/connectome_interpreter/utils.py` & `connectome_interpreter-1.7.1/connectome_interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.0/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.7.1/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.7.0
+Version: 1.7.1
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
```

### Comparing `connectome_interpreter-1.7.0/connectome_interpreter.egg-info/SOURCES.txt` & `connectome_interpreter-1.7.1/connectome_interpreter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.0/setup.py` & `connectome_interpreter-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.7.0',
+    version='1.7.1',
     packages=find_packages(),
     install_requires=install_requires_list,
     extras_require={
         'get_ngl_link': ['nglscenes'],
         'wandb': ['wandb'],
     },
     # Optional metadata
```

### Comparing `connectome_interpreter-1.7.0/tests/test_compress_paths.py` & `connectome_interpreter-1.7.1/tests/test_compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.0/tests/test_utils.py` & `connectome_interpreter-1.7.1/tests/test_utils.py`

 * *Files identical despite different names*

