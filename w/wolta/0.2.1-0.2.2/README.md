# Comparing `tmp/wolta-0.2.1.tar.gz` & `tmp/wolta-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolta-0.2.1.tar", last modified: Sun Apr 28 15:10:51 2024, max compression
+gzip compressed data, was "wolta-0.2.2.tar", last modified: Sun May  5 15:48:51 2024, max compression
```

## Comparing `wolta-0.2.1.tar` & `wolta-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 15:10:51.888051 wolta-0.2.1/
--rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0    20060 2024-04-28 15:10:51.887035 wolta-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    18630 2024-04-27 23:19:00.000000 wolta-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 15:10:51.888051 wolta-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1221 2024-04-28 15:10:47.000000 wolta-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:10:51.847909 wolta-0.2.1/wolta/
--rw-rw-rw-   0        0        0      115 2024-04-27 21:13:06.000000 wolta-0.2.1/wolta/__init__.py
--rw-rw-rw-   0        0        0    12216 2024-04-27 19:19:42.000000 wolta-0.2.1/wolta/data_tools.py
--rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.2.1/wolta/feature_tools.py
--rw-rw-rw-   0        0        0    33410 2024-04-28 15:10:47.000000 wolta-0.2.1/wolta/model_tools.py
--rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.2.1/wolta/progressive_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:10:51.885862 wolta-0.2.1/wolta.egg-info/
--rw-rw-rw-   0        0        0    20060 2024-04-28 15:10:51.000000 wolta-0.2.1/wolta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-28 15:10:51.000000 wolta-0.2.1/wolta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 15:10:51.000000 wolta-0.2.1/wolta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-28 15:10:51.000000 wolta-0.2.1/wolta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       61 2024-04-28 15:10:51.000000 wolta-0.2.1/wolta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 15:48:51.363189 wolta-0.2.2/
+-rw-rw-rw-   0        0        0      589 2024-03-30 14:38:25.000000 wolta-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    20873 2024-05-05 15:48:51.362152 wolta-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    19416 2024-05-05 15:48:10.000000 wolta-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:48:51.363189 wolta-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2024-05-05 15:19:08.000000 wolta-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:48:51.317525 wolta-0.2.2/wolta/
+-rw-rw-rw-   0        0        0      115 2024-04-27 21:13:06.000000 wolta-0.2.2/wolta/__init__.py
+-rw-rw-rw-   0        0        0    14525 2024-05-05 14:20:24.000000 wolta-0.2.2/wolta/data_tools.py
+-rw-rw-rw-   0        0        0     3029 2024-03-31 16:03:51.000000 wolta-0.2.2/wolta/feature_tools.py
+-rw-rw-rw-   0        0        0    33410 2024-04-28 15:10:47.000000 wolta-0.2.2/wolta/model_tools.py
+-rw-rw-rw-   0        0        0     2075 2024-03-31 11:34:06.000000 wolta-0.2.2/wolta/progressive_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:48:51.361114 wolta-0.2.2/wolta.egg-info/
+-rw-rw-rw-   0        0        0    20873 2024-05-05 15:48:51.000000 wolta-0.2.2/wolta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-05-05 15:48:51.000000 wolta-0.2.2/wolta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:48:51.000000 wolta-0.2.2/wolta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-05 15:48:51.000000 wolta-0.2.2/wolta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       61 2024-05-05 15:48:51.000000 wolta-0.2.2/wolta.egg-info/top_level.txt
```

### Comparing `wolta-0.2.1/LICENSE.txt` & `wolta-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wolta-0.2.1/PKG-INFO` & `wolta-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.2.1
+Version: 0.2.2
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -185,14 +185,41 @@
 
 **Parameters**:
 * y
 * strategy, {'normal', 'normal-extra'}, default by, 'normal'
 
 ***
 
+### state_sum
+
+It gives information about features.
+
+**Returns**: dictionary which keys are feature names. (if get_dict param is True)
+
+**Parameters**:
+* df, pandas dataframe
+* requested, array of string
+
+| value | meaning                     |
+| --- |-----------------------------|
+| min | minimum value for a feature |
+| max | maximum value for a feature |
+| width | difference between max and min |
+| std | standard |
+| mean | mean |
+| med | median |
+| var | variance |
+
+* only, list of string, it gets results for these features only, by default None. If it is none, function gets results for all features
+* exclude, list of string, it gets results for except these features, by default None.
+* get_dict, by default False
+* verbose, by default True
+
+***
+
 ### create_chunks
 
 **Parameters**:
 
 * path, _string_
 * sample_amount, _int_, sample amount for each chunk
 * target_dir, _string_, directory path to save chunks, by default, None
```

### Comparing `wolta-0.2.1/README.md` & `wolta-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,41 @@
 
 **Parameters**:
 * y
 * strategy, {'normal', 'normal-extra'}, default by, 'normal'
 
 ***
 
+### state_sum
+
+It gives information about features.
+
+**Returns**: dictionary which keys are feature names. (if get_dict param is True)
+
+**Parameters**:
+* df, pandas dataframe
+* requested, array of string
+
+| value | meaning                     |
+| --- |-----------------------------|
+| min | minimum value for a feature |
+| max | maximum value for a feature |
+| width | difference between max and min |
+| std | standard |
+| mean | mean |
+| med | median |
+| var | variance |
+
+* only, list of string, it gets results for these features only, by default None. If it is none, function gets results for all features
+* exclude, list of string, it gets results for except these features, by default None.
+* get_dict, by default False
+* verbose, by default True
+
+***
+
 ### create_chunks
 
 **Parameters**:
 
 * path, _string_
 * sample_amount, _int_, sample amount for each chunk
 * target_dir, _string_, directory path to save chunks, by default, None
```

### Comparing `wolta-0.2.1/setup.py` & `wolta-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'Data Science Library'
 LONG_DESCRIPTION = 'A package for data science'
 
 setup(
     name="wolta",
     version=VERSION,
     author="iamalreadynoob",
```

### Comparing `wolta-0.2.1/wolta/data_tools.py` & `wolta-0.2.2/wolta/data_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -478,8 +478,93 @@
 
     elif type == 'np':
         for i in range(matrix.shape[1]):
             for j in range(matrix.shape[0]):
                 if matrix[j, i] == replace:
                     matrix.iloc[j, i] = None
 
-        return matrix
+        return matrix
+
+
+def stat_sum(df, requested, only=None, exclude=None, get_dict=False, verbose=True):
+    process_columns = []
+
+    if only is None:
+        process_columns = list(df.columns)
+    else:
+        process_columns = list(only)
+
+    if exclude is not None:
+        for col in exclude:
+            if col in process_columns:
+                process_columns.remove(col)
+
+    if requested[0] == 'all':
+        requested = ['min', 'max', 'width', 'mean', 'std', 'med', 'var']
+
+    gen_results = {}
+
+    for col in process_columns:
+        results = {}
+
+        if verbose:
+            print(col)
+
+        for req in requested:
+            if req == 'min':
+                res = np.amin(df[col].values)
+                results[req] = res
+
+                if verbose:
+                    print('min: {}'.format(str(res)))
+
+            elif req == 'max':
+                res = np.amax(df[col].values)
+                results[req] = res
+
+                if verbose:
+                    print('max: {}'.format(str(res)))
+
+            elif req == 'width':
+                res_max = np.amax(df[col].values)
+                res_min = np.amin(df[col].values)
+                res = res_max - res_min
+                results[req] = res
+
+                if verbose:
+                    print('width: {}'.format(str(res)))
+
+            elif req == 'mean':
+                res = np.mean(df[col].values)
+                results[req] = res
+
+                if verbose:
+                    print('mean: {}'.format(str(res)))
+
+            elif req == 'std':
+                res = np.std(df[col].values)
+                results[req] = res
+
+                if verbose:
+                    print('std: {}'.format(str(res)))
+
+            elif req == 'med':
+                res = np.median(df[col].values)
+                results[req] = res
+
+                if verbose:
+                    print('median: {}'.format(str(res)))
+
+            elif req == 'var':
+                res = np.var(df[col].values)
+                results[req] = res
+
+                if verbose:
+                    print('variance: {}'.format(str(res)))
+
+        gen_results[col] = results
+
+        if verbose:
+            print('***')
+
+    if get_dict:
+        return gen_results
```

### Comparing `wolta-0.2.1/wolta/feature_tools.py` & `wolta-0.2.2/wolta/feature_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.2.1/wolta/model_tools.py` & `wolta-0.2.2/wolta/model_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.2.1/wolta/progressive_tools.py` & `wolta-0.2.2/wolta/progressive_tools.py`

 * *Files identical despite different names*

### Comparing `wolta-0.2.1/wolta.egg-info/PKG-INFO` & `wolta-0.2.2/wolta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolta
-Version: 0.2.1
+Version: 0.2.2
 Summary: Data Science Library
 Author: iamalreadynoob
 Author-email: <sadikefe69@gmail.com>
 Keywords: python,machine,learning,machine learning,data science,data
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -185,14 +185,41 @@
 
 **Parameters**:
 * y
 * strategy, {'normal', 'normal-extra'}, default by, 'normal'
 
 ***
 
+### state_sum
+
+It gives information about features.
+
+**Returns**: dictionary which keys are feature names. (if get_dict param is True)
+
+**Parameters**:
+* df, pandas dataframe
+* requested, array of string
+
+| value | meaning                     |
+| --- |-----------------------------|
+| min | minimum value for a feature |
+| max | maximum value for a feature |
+| width | difference between max and min |
+| std | standard |
+| mean | mean |
+| med | median |
+| var | variance |
+
+* only, list of string, it gets results for these features only, by default None. If it is none, function gets results for all features
+* exclude, list of string, it gets results for except these features, by default None.
+* get_dict, by default False
+* verbose, by default True
+
+***
+
 ### create_chunks
 
 **Parameters**:
 
 * path, _string_
 * sample_amount, _int_, sample amount for each chunk
 * target_dir, _string_, directory path to save chunks, by default, None
```

