# Comparing `tmp/sts_lib-0.30.3.tar.gz` & `tmp/sts_lib-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.30.3.tar", last modified: Sat May  4 08:50:47 2024, max compression
+gzip compressed data, was "sts_lib-0.31.0.tar", last modified: Sun May  5 14:58:07 2024, max compression
```

## Comparing `sts_lib-0.30.3.tar` & `sts_lib-0.31.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.553971 sts_lib-0.30.3/
--rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.30.3/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.30.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6916 2024-05-04 08:50:47.553971 sts_lib-0.30.3/PKG-INFO
--rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.30.3/README.md
--rw-rw-rw-   0        0        0     1728 2024-05-04 08:50:47.553971 sts_lib-0.30.3/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.30.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.422407 sts_lib-0.30.3/sts/
--rw-rw-rw-   0        0        0    52916 2024-05-04 08:48:31.000000 sts_lib-0.30.3/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.30.3/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.422407 sts_lib-0.30.3/sts/data/
-drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.438030 sts_lib-0.30.3/sts/data/config/
--rw-rw-rw-   0        0        0      915 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      608 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      346 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      410 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      419 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      267 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      417 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      607 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      247 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      261 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      267 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      245 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      606 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      670 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      344 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.475845 sts_lib-0.30.3/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-05-02 13:01:51.000000 sts_lib-0.30.3/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    22659 2024-05-04 08:41:18.000000 sts_lib-0.30.3/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.507097 sts_lib-0.30.3/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-05-02 20:11:02.000000 sts_lib-0.30.3/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-05-02 12:17:13.000000 sts_lib-0.30.3/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 08:50:47.538335 sts_lib-0.30.3/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     6916 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-04 08:50:47.000000 sts_lib-0.30.3/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 14:58:07.545160 sts_lib-0.31.0/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.31.0/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.31.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6916 2024-05-05 14:58:07.545160 sts_lib-0.31.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5463 2024-04-29 19:01:51.000000 sts_lib-0.31.0/README.md
+-rw-rw-rw-   0        0        0     1728 2024-05-05 14:58:07.545160 sts_lib-0.31.0/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.31.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:58:07.505189 sts_lib-0.31.0/sts/
+-rw-rw-rw-   0        0        0    52782 2024-05-05 14:57:28.000000 sts_lib-0.31.0/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.31.0/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:58:07.505189 sts_lib-0.31.0/sts/data/
+drwxrwxrwx   0        0        0        0 2024-05-05 14:58:07.521160 sts_lib-0.31.0/sts/data/config/
+-rw-rw-rw-   0        0        0      915 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      608 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      346 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      410 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      419 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      267 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      417 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      607 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      247 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      261 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      267 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      245 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      606 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      670 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      344 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-05-05 14:58:07.537160 sts_lib-0.31.0/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-05-05 14:57:49.000000 sts_lib-0.31.0/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-05-05 08:43:39.000000 sts_lib-0.31.0/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    22659 2024-05-05 14:12:58.000000 sts_lib-0.31.0/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-05-05 14:58:07.537160 sts_lib-0.31.0/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-05-05 14:57:54.000000 sts_lib-0.31.0/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-05-05 14:56:48.000000 sts_lib-0.31.0/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 14:58:07.545160 sts_lib-0.31.0/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     6916 2024-05-05 14:58:07.000000 sts_lib-0.31.0/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-05-05 14:58:07.000000 sts_lib-0.31.0/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 14:58:07.000000 sts_lib-0.31.0/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-05 14:58:07.000000 sts_lib-0.31.0/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-05-05 14:58:07.000000 sts_lib-0.31.0/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-05 14:58:07.000000 sts_lib-0.31.0/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.30.3/LICENSE` & `sts_lib-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/PKG-INFO` & `sts_lib-0.31.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.30.3
+Version: 0.31.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.30.3/README.md` & `sts_lib-0.31.0/README.md`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/setup.cfg` & `sts_lib-0.31.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/__init__.py` & `sts_lib-0.31.0/sts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.30.3'
+__version__ = '0.31.0'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 StsConvExclude = namedtuple('StsConvExclude', ['text'])
 
 
 class StreamList(list):
@@ -462,98 +462,104 @@
 
         This will invoke stsdict.apply_enum and it's recommended that stsdict
         be a Table or Trie for better performance.
 
         Returns:
             a new object with the same class.
         """
-        dict1 = self._join_postfix(stsdict)
-        dict2 = stsdict._join_prefix(self)
-        return dict1.update(dict2)
+        newdict = self.__class__()
 
-    def _join_prefix(self, stsdict):
-        """Prefix self with stsdict.
+        """postfix
 
-        Convert keys of self using the reversed stsdict, enumerating all
-        possible matches.
+        Convert values of self using stsdict, enumerating all longest
+        conversions.
 
-        Yield a new key-value pair for the first value of an stsdict entry,
-        e.g.:
+        Example:
+            self:
+                因为 => 因爲
+            stsdict:
+                爲 => 為
+            result:
+                因为 => 因為
+        """
+        for key, values in self.items():
+            for value in values:
+                newdict.add(key, stsdict.apply_enum(value))
+
+        """merge
+
+        Merge entries in stsdict.
+        """
+        newdict.update(stsdict)
 
-            table:
-                註冊表 => 登錄檔
+        """prefix
+
+        Convert each key of stsdict using reversed self, enumerating all
+        possible conversions.
+
+        Add a new key-value pair for the first value of an entry,
+
+        Example:
+            self:
+                纳 => 納
+            self reversed:
+                納 => 纳
             stsdict:
-                注 => 註 注
-            reversed stsdict:
-                註 => 注
-            table._join_prefix(stsdict):
-                注冊表 => 登錄檔
-                註冊表 => 登錄檔
+                納米 => 奈米
+            result:
+                纳米 => 奈米
 
-        Yield a new minor key-value pair for each minor value of an stsdict
-        entry, e.g.:
+        Add a new minor key-value pair (which is never the first candidate) for
+        each minor value of an entry.
 
-            table:
-                註冊表 => 登錄檔
+        Example:
+            self:
+                妳 => 你 奶
+            self reversed:
+                奶 => 妳
             stsdict:
-                注 => 注 註
-            reversed stsdict:
-                註 => 注
-            table._join_prefix(stsdict):
-                註冊表 => 登錄檔
-                注冊表 => 注冊表 登錄檔
+                奶娘 => 奶媽
+            result:
+                妳娘 => 妳娘 奶媽
 
-        Returns:
-            a new object with the same class.
+        Example:
+            self:
+                妳 => 你 奶
+            self reversed:
+                奶 => 妳
+            stsdict:
+                奶娘 => 奶媽
+                妳娘 => 你娘
+            result:
+                妳娘 => 你娘 奶媽
         """
-        dict_ = self.__class__()
-        converter = self.__class__()
-        converter_minor = self.__class__()
-        for key, values in stsdict.items():
+        conv = self.__class__()
+        conv_minor = self.__class__()
+        for key, values in self.items():
             for i, value in enumerate(values):
                 if i == 0:
-                    converter.add(value, [key])
+                    conv.add(value, [key])
                 else:
-                    converter_minor.add(value, [key])
-        for key, values in self.items():
-            for newkey in converter.apply_enum(key, include_short=True, include_self=True):
-                dict_.add(newkey, values)
-            for newkey in converter_minor.apply_enum(key, include_short=True, include_self=True):
+                    conv_minor.add(value, [key])
+
+        for key, values in stsdict.items():
+            for newkey in conv.apply_enum(key, include_short=True, include_self=True):
+                newdict.add(newkey, values)
+
+        for key, values in stsdict.items():
+            for newkey in conv_minor.apply_enum(key, include_short=True, include_self=True):
                 if newkey == key:
                     continue
                 try:
-                    assert dict_[newkey]
+                    assert newdict[newkey]
                 except (KeyError, AssertionError):
-                    dict_.add(newkey, newkey)
-                dict_.add(newkey, values)
-        return dict_
+                    newdict.add(newkey, newkey)
+                newdict.add(newkey, values)
 
-    def _join_postfix(self, stsdict):
-        """Postfix self with stsdict.
-
-        Convert values of self using stsdict, enumerating all maximal matches.
-        Plus all conversions of stsdict.
-
-        Example:
-            table:
-                因为 => 因爲
-            stsdict:
-                爲 => 為
-            table._join_postfix(stsdict):
-                因为 => 因為
-                爲 => 為
-
-        Returns:
-            a new object with the same class.
-        """
-        dict_ = self.__class__()
-        for key, values in self.items():
-            for value in values:
-                dict_.add(key, stsdict.apply_enum(value))
-        return dict_.update(stsdict)
+        return newdict
 
     def _split(self, parts):
         """Split parts into a list of Unicode composites.
 
         With automatic type handling.
         """
         if isinstance(parts, str):
@@ -569,15 +575,19 @@
         Args:
             parts: a string or iterable parts to be matched.
 
         Returns:
             an StsDictMatch or None if no match.
         """
         parts = self._split(parts)
-        i = max(len(Unicode.split(key)) for key in self._dict)
+        try:
+            i = max(len(Unicode.split(key)) for key in self._dict)
+        except ValueError:
+            # self._dict is empty
+            i = 0
         i = min(i, min(len(parts), maxpos) - pos)
         while i >= 1:
             end = pos + i
             current_parts = parts[pos:end]
             current = ''.join(current_parts)
             try:
                 match = self._dict[current]
```

### Comparing `sts_lib-0.30.3/sts/cli.py` & `sts_lib-0.31.0/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/config/_default.json` & `sts_lib-0.31.0/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/config/hk2s.json` & `sts_lib-0.31.0/sts/data/config/hk2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/config/s2twp.json` & `sts_lib-0.31.0/sts/data/config/s2twp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/config/tw2s.json` & `sts_lib-0.31.0/sts/data/config/tw2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/config/tw2sp.json` & `sts_lib-0.31.0/sts/data/config/tw2sp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.31.0/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.31.0/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.31.0/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.31.0/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.31.0/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.31.0/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.31.0/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.31.0/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.31.0/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.31.0/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.31.0/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.31.0/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/htmlpage.tpl.html` & `sts_lib-0.31.0/sts/data/htmlpage.tpl.html`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/scheme/st_multi.txt` & `sts_lib-0.31.0/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts/data/scheme/variant.txt` & `sts_lib-0.31.0/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.30.3/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.31.0/sts_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.30.3
+Version: 0.31.0
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.30.3/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.31.0/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

