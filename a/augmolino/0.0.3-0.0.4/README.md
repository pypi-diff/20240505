# Comparing `tmp/augmolino-0.0.3.tar.gz` & `tmp/augmolino-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\augmolino-0.0.3.tar", last modified: Wed Jan 25 13:47:19 2023, max compression
+gzip compressed data, was "dist\augmolino-0.0.4.tar", last modified: Sun May  5 18:19:48 2024, max compression
```

## Comparing `augmolino-0.0.3.tar` & `augmolino-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 13:47:19.768123 augmolino-0.0.3/
--rw-rw-rw-   0        0        0    35823 2023-01-19 16:09:40.000000 augmolino-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      415 2023-01-25 13:47:19.770122 augmolino-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2023-01-22 14:36:45.000000 augmolino-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-25 13:47:19.717125 augmolino-0.0.3/augmolino/
--rw-rw-rw-   0        0        0        0 2023-01-19 16:09:40.000000 augmolino-0.0.3/augmolino/__init__.py
--rw-rw-rw-   0        0        0     9842 2023-01-25 13:45:45.000000 augmolino-0.0.3/augmolino/augmentation.py
--rw-rw-rw-   0        0        0     4753 2023-01-22 14:18:19.000000 augmolino-0.0.3/augmolino/augmenter.py
--rw-rw-rw-   0        0        0      747 2023-01-22 14:30:06.000000 augmolino-0.0.3/augmolino/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-25 13:47:19.765122 augmolino-0.0.3/augmolino.egg-info/
--rw-rw-rw-   0        0        0      415 2023-01-25 13:47:19.000000 augmolino-0.0.3/augmolino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-01-25 13:47:19.000000 augmolino-0.0.3/augmolino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 13:47:19.000000 augmolino-0.0.3/augmolino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-19 18:48:50.000000 augmolino-0.0.3/augmolino.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2023-01-25 13:47:19.000000 augmolino-0.0.3/augmolino.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-25 13:47:19.000000 augmolino-0.0.3/augmolino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-01-25 13:47:19.773123 augmolino-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-01-25 13:46:29.000000 augmolino-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:19:48.975685 augmolino-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2024-05-05 18:07:59.000000 augmolino-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      509 2024-05-05 18:19:48.973682 augmolino-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1081 2024-05-05 18:07:59.000000 augmolino-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 18:19:48.905678 augmolino-0.0.4/augmolino/
+-rw-rw-rw-   0        0        0        0 2024-05-05 18:07:59.000000 augmolino-0.0.4/augmolino/__init__.py
+-rw-rw-rw-   0        0        0     9860 2024-05-05 18:15:38.000000 augmolino-0.0.4/augmolino/augmentation.py
+-rw-rw-rw-   0        0        0     4753 2024-05-05 18:07:59.000000 augmolino-0.0.4/augmolino/augmenter.py
+-rw-rw-rw-   0        0        0      747 2024-05-05 18:07:59.000000 augmolino-0.0.4/augmolino/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:19:48.971683 augmolino-0.0.4/augmolino.egg-info/
+-rw-rw-rw-   0        0        0      509 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       30 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-05 18:19:48.000000 augmolino-0.0.4/augmolino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-05 18:19:48.978683 augmolino-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      669 2024-05-05 18:16:36.000000 augmolino-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:19:48.967685 augmolino-0.0.4/tests/
+-rw-rw-rw-   0        0        0     4111 2024-05-05 18:07:59.000000 augmolino-0.0.4/tests/test_augmentation.py
+-rw-rw-rw-   0        0        0     2643 2024-05-05 18:07:59.000000 augmolino-0.0.4/tests/test_augmenter.py
+-rw-rw-rw-   0        0        0      163 2024-05-05 18:12:59.000000 augmolino-0.0.4/tests/test_utils.py
```

### Comparing `augmolino-0.0.3/LICENSE` & `augmolino-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `augmolino-0.0.3/README.md` & `augmolino-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `augmolino-0.0.3/augmolino/augmentation.py` & `augmolino-0.0.4/augmolino/augmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         `kwargs`:
             Arguments for executing of `function`.    
         """
         self._load(f_source)
         self.f_dest = self._parsePath(f_dest)
 
         # append kwargs in case some are appended after init
-        self.kwargs |= kwargs
+        self.kwargs = {**self.kwargs, **kwargs}
 
         x_new = self._executeFunction()
 
         if self.f_dest != None:
             sf.write(self.f_dest, x_new, self.sample_rate)
             return None
```

### Comparing `augmolino-0.0.3/augmolino/augmenter.py` & `augmolino-0.0.4/augmolino/augmenter.py`

 * *Files identical despite different names*

### Comparing `augmolino-0.0.3/augmolino/utils.py` & `augmolino-0.0.4/augmolino/utils.py`

 * *Files identical despite different names*

### Comparing `augmolino-0.0.3/setup.py` & `augmolino-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(name='augmolino',
       packages=['augmolino'],
-      version='0.0.3',
+      version='0.0.4',
       description='augmentation for audio based datasets for machine learning',
       url='https://github.com/jake-is-ESD-protected/augmolino',
       download_url="https://github.com/jake-is-ESD-protected/augmolino/archive/refs/tags/0.0.2.tar.gz",
       author='Jakob Tschavoll',
       author_email='jt@tschavoll.at',
       license='GPL 3.0',
       classifiers=[],
```

