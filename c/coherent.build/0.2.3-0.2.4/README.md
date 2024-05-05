# Comparing `tmp/coherent_build-0.2.3.tar.gz` & `tmp/coherent_build-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_build-0.2.3.tar", last modified: Sun May  5 14:49:13 2024, max compression
+gzip compressed data, was "coherent_build-0.2.4.tar", last modified: Sun May  5 15:12:55 2024, max compression
```

## Comparing `coherent_build-0.2.3.tar` & `coherent_build-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,6 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 14:46:31.084525 coherent_build-0.2.3/
--rw-r--r--   0 jaraco     (501) staff       (20)     6148 2024-05-02 15:28:09.027061 coherent_build-0.2.3/.DS_Store
-drwx------   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883440 coherent_build-0.2.3/.pytest_cache/
--rw-r--r--   0 jaraco     (501) staff       (20)       37 2024-05-04 14:50:05.883209 coherent_build-0.2.3/.pytest_cache/.gitignore
--rw-r--r--   0 jaraco     (501) staff       (20)      191 2024-05-04 14:50:05.883265 coherent_build-0.2.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 jaraco     (501) staff       (20)      302 2024-05-04 14:50:05.883131 coherent_build-0.2.3/.pytest_cache/README.md
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883467 coherent_build-0.2.3/.pytest_cache/v/
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883703 coherent_build-0.2.3/.pytest_cache/v/cache/
--rw-r--r--   0 jaraco     (501) staff       (20)        2 2024-05-05 13:52:14.326103 coherent_build-0.2.3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 jaraco     (501) staff       (20)       38 2024-05-05 13:52:14.325637 coherent_build-0.2.3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 jaraco     (501) staff       (20)        2 2024-05-05 13:52:14.326323 coherent_build-0.2.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.2.3/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)     7066 2024-05-05 14:43:41.351044 coherent_build-0.2.3/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.2.3/__main__.py
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 14:46:32.466307 coherent_build-0.2.3/coherent/
-lrwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 14:46:32.466295 coherent_build-0.2.3/coherent/build -> ..
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      436 2024-05-05 14:49:13.631196 coherent_build-0.2.3/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 15:12:55.048730 coherent_build-0.2.4/
+-rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.2.4/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)     7526 2024-05-05 15:07:59.786119 coherent_build-0.2.4/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.2.4/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      436 2024-05-05 15:12:55.695288 coherent_build-0.2.4/PKG-INFO
```

### Comparing `coherent_build-0.2.3/__init__.py` & `coherent_build-0.2.4/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,15 +65,32 @@
         if re.match(ignore_pattern, info.name.removeprefix("./")):
             return
         info.name = self.name + "/" + info.name.removeprefix("./")
         return info
 
 
 class SDist(Filter):
-    ignored = [r"\.git", "dist", r".*\b__pycache__$"]
+    """
+    >>> sf = SDist(name="foo")
+
+    Ignores the .git directory
+    >>> sf(types.SimpleNamespace(name='./.git'))
+
+    Ignores __pycache__ directories
+    >>> sf(types.SimpleNamespace(name='./bar/__pycache__'))
+
+    Ignore paths starting with a dot
+    >>> sf(types.SimpleNamespace(name='./bar/.DS_Store'))
+
+    Should not ignore nested dist dirs
+    >>> sf(types.SimpleNamespace(name='./bar/dist'))
+    namespace(name='foo/bar/dist')
+    """
+
+    ignored = ["dist", r"(.*[/])?__pycache__$", r"(.*[/])?[.]"]
 
 
 class Wheel(Filter):
     ignored = ["docs", "tests", "README.*", "PKG-INFO", "(meta)"]
 
 
 class ZipInfo(types.SimpleNamespace):
```

