# Comparing `tmp/keras-vision-0.4.1.tar.gz` & `tmp/keras-vision-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-vision-0.4.1.tar", last modified: Sun May  5 18:31:55 2024, max compression
+gzip compressed data, was "keras-vision-0.4.2.tar", last modified: Sun May  5 18:57:07 2024, max compression
```

## Comparing `keras-vision-0.4.1.tar` & `keras-vision-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 18:31:55.745030 keras-vision-0.4.1/
--rw-rw-rw-   0        0        0     1389 2024-05-05 18:31:55.743518 keras-vision-0.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-05 18:31:55.727505 keras-vision-0.4.1/keras_vision/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:31:55.742520 keras-vision-0.4.1/keras_vision/MobileViT_v1/
--rw-rw-rw-   0        0        0      501 2024-05-03 18:35:52.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/__init__.py
--rw-rw-rw-   0        0        0     4516 2024-05-03 18:38:00.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/base_layers.py
--rw-rw-rw-   0        0        0     2428 2024-05-03 18:38:07.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/configs.py
--rw-rw-rw-   0        0        0     8176 2024-05-05 18:29:05.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/mobile_vit_v1.py
--rw-rw-rw-   0        0        0    13452 2024-05-05 15:29:51.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
--rw-rw-rw-   0        0        0     2529 2024-05-03 18:37:13.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
--rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/utils.py
--rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras-vision-0.4.1/keras_vision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:31:55.734528 keras-vision-0.4.1/keras_vision.egg-info/
--rw-rw-rw-   0        0        0     1389 2024-05-05 18:31:55.000000 keras-vision-0.4.1/keras_vision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-05-05 18:31:55.000000 keras-vision-0.4.1/keras_vision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 18:31:55.000000 keras-vision-0.4.1/keras_vision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-05 18:31:55.000000 keras-vision-0.4.1/keras_vision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-05 18:31:55.000000 keras-vision-0.4.1/keras_vision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 18:31:55.746038 keras-vision-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-05-05 18:30:00.000000 keras-vision-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:57:07.488933 keras-vision-0.4.2/
+-rw-rw-rw-   0        0        0     1396 2024-05-05 18:57:07.487938 keras-vision-0.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-05 18:57:07.469388 keras-vision-0.4.2/keras_vision/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:57:07.486930 keras-vision-0.4.2/keras_vision/MobileViT_v1/
+-rw-rw-rw-   0        0        0      501 2024-05-03 18:35:52.000000 keras-vision-0.4.2/keras_vision/MobileViT_v1/__init__.py
+-rw-rw-rw-   0        0        0     4516 2024-05-03 18:38:00.000000 keras-vision-0.4.2/keras_vision/MobileViT_v1/base_layers.py
+-rw-rw-rw-   0        0        0     2428 2024-05-03 18:38:07.000000 keras-vision-0.4.2/keras_vision/MobileViT_v1/configs.py
+-rw-rw-rw-   0        0        0     8176 2024-05-05 18:29:05.000000 keras-vision-0.4.2/keras_vision/MobileViT_v1/mobile_vit_v1.py
+-rw-rw-rw-   0        0        0    13452 2024-05-05 15:29:51.000000 keras-vision-0.4.2/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
+-rw-rw-rw-   0        0        0     2529 2024-05-03 18:37:13.000000 keras-vision-0.4.2/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
+-rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras-vision-0.4.2/keras_vision/MobileViT_v1/utils.py
+-rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras-vision-0.4.2/keras_vision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:57:07.476398 keras-vision-0.4.2/keras_vision.egg-info/
+-rw-rw-rw-   0        0        0     1396 2024-05-05 18:57:07.000000 keras-vision-0.4.2/keras_vision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-05 18:57:07.000000 keras-vision-0.4.2/keras_vision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:57:07.000000 keras-vision-0.4.2/keras_vision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-05 18:57:07.000000 keras-vision-0.4.2/keras_vision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-05 18:57:07.000000 keras-vision-0.4.2/keras_vision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:57:07.489940 keras-vision-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1832 2024-05-05 18:56:37.000000 keras-vision-0.4.2/setup.py
```

### Comparing `keras-vision-0.4.1/PKG-INFO` & `keras-vision-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-vision
-Version: 0.4.1
+Version: 0.4.2
 Summary: Building Vision models in Keras3 for framework agnostic training and inference.
 Home-page: https://github.com/veb-101/keras-vision
 Author: Vaibhav Singh
 Author-email: vaibhav.singh.3001@gmail.com
 License: Apache 2.0
 Keywords: keras3 tensorflow Jax PyTorch Vision
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: keras
+Requires-Dist: keras>=3.3.3
 
 Porting all models from everywhere to Keras for leveraging multi-backend support.
 
 Cause why not?🤷🏻‍♂️
 
 ### Updates
```

### Comparing `keras-vision-0.4.1/keras_vision/MobileViT_v1/base_layers.py` & `keras-vision-0.4.2/keras_vision/MobileViT_v1/base_layers.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.1/keras_vision/MobileViT_v1/configs.py` & `keras-vision-0.4.2/keras_vision/MobileViT_v1/configs.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.1/keras_vision/MobileViT_v1/mobile_vit_v1.py` & `keras-vision-0.4.2/keras_vision/MobileViT_v1/mobile_vit_v1.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.1/keras_vision/MobileViT_v1/mobile_vit_v1_block.py` & `keras-vision-0.4.2/keras_vision/MobileViT_v1/mobile_vit_v1_block.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.1/keras_vision/MobileViT_v1/multihead_self_attention_2D.py` & `keras-vision-0.4.2/keras_vision/MobileViT_v1/multihead_self_attention_2D.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.1/keras_vision/MobileViT_v1/utils.py` & `keras-vision-0.4.2/keras_vision/MobileViT_v1/utils.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.1/keras_vision.egg-info/PKG-INFO` & `keras-vision-0.4.2/keras_vision.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-vision
-Version: 0.4.1
+Version: 0.4.2
 Summary: Building Vision models in Keras3 for framework agnostic training and inference.
 Home-page: https://github.com/veb-101/keras-vision
 Author: Vaibhav Singh
 Author-email: vaibhav.singh.3001@gmail.com
 License: Apache 2.0
 Keywords: keras3 tensorflow Jax PyTorch Vision
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: keras
+Requires-Dist: keras>=3.3.3
 
 Porting all models from everywhere to Keras for leveraging multi-backend support.
 
 Cause why not?🤷🏻‍♂️
 
 ### Updates
```

### Comparing `keras-vision-0.4.1/keras_vision.egg-info/SOURCES.txt` & `keras-vision-0.4.2/keras_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4.1/setup.py` & `keras-vision-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 DESCRIPTION = "Building Vision models in Keras3 for framework agnostic training and inference."
 
 # Setting up
 setup(
     name="keras-vision",
     version=__version__,
     author="Vaibhav Singh",
@@ -40,12 +40,12 @@
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     # Note that this is a string of words separated by whitespace, not a list.
     keywords="keras3 tensorflow Jax PyTorch Vision",
     install_requires=[
-        "keras",
+        "keras>=3.3.3",
     ],
     python_requires=">=3.10",
     license="Apache 2.0",
 )
```

