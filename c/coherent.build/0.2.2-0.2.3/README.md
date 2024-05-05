# Comparing `tmp/coherent_build-0.2.2.tar.gz` & `tmp/coherent_build-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_build-0.2.2.tar", last modified: Sun May  5 14:13:14 2024, max compression
+gzip compressed data, was "coherent_build-0.2.3.tar", last modified: Sun May  5 14:49:13 2024, max compression
```

## Comparing `coherent_build-0.2.2.tar` & `coherent_build-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 14:05:04.255927 coherent_build-0.2.2/
--rw-r--r--   0 jaraco     (501) staff       (20)     6148 2024-05-02 15:28:09.027061 coherent_build-0.2.2/.DS_Store
-drwx------   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883440 coherent_build-0.2.2/.pytest_cache/
--rw-r--r--   0 jaraco     (501) staff       (20)       37 2024-05-04 14:50:05.883209 coherent_build-0.2.2/.pytest_cache/.gitignore
--rw-r--r--   0 jaraco     (501) staff       (20)      191 2024-05-04 14:50:05.883265 coherent_build-0.2.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 jaraco     (501) staff       (20)      302 2024-05-04 14:50:05.883131 coherent_build-0.2.2/.pytest_cache/README.md
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883467 coherent_build-0.2.2/.pytest_cache/v/
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883703 coherent_build-0.2.2/.pytest_cache/v/cache/
--rw-r--r--   0 jaraco     (501) staff       (20)        2 2024-05-05 13:52:14.326103 coherent_build-0.2.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0 jaraco     (501) staff       (20)       38 2024-05-05 13:52:14.325637 coherent_build-0.2.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 jaraco     (501) staff       (20)        2 2024-05-05 13:52:14.326323 coherent_build-0.2.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 jaraco     (501) staff       (20)      129 2024-05-04 14:42:38.291197 coherent_build-0.2.2/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)     6974 2024-05-05 14:11:05.879658 coherent_build-0.2.2/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.2.2/__main__.py
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 14:05:28.419491 coherent_build-0.2.2/coherent/
-lrwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 14:05:28.419477 coherent_build-0.2.2/coherent/build -> ..
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       58 2024-05-05 14:13:14.523175 coherent_build-0.2.2/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 14:46:31.084525 coherent_build-0.2.3/
+-rw-r--r--   0 jaraco     (501) staff       (20)     6148 2024-05-02 15:28:09.027061 coherent_build-0.2.3/.DS_Store
+drwx------   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883440 coherent_build-0.2.3/.pytest_cache/
+-rw-r--r--   0 jaraco     (501) staff       (20)       37 2024-05-04 14:50:05.883209 coherent_build-0.2.3/.pytest_cache/.gitignore
+-rw-r--r--   0 jaraco     (501) staff       (20)      191 2024-05-04 14:50:05.883265 coherent_build-0.2.3/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jaraco     (501) staff       (20)      302 2024-05-04 14:50:05.883131 coherent_build-0.2.3/.pytest_cache/README.md
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883467 coherent_build-0.2.3/.pytest_cache/v/
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-04 14:50:05.883703 coherent_build-0.2.3/.pytest_cache/v/cache/
+-rw-r--r--   0 jaraco     (501) staff       (20)        2 2024-05-05 13:52:14.326103 coherent_build-0.2.3/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0 jaraco     (501) staff       (20)       38 2024-05-05 13:52:14.325637 coherent_build-0.2.3/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jaraco     (501) staff       (20)        2 2024-05-05 13:52:14.326323 coherent_build-0.2.3/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.2.3/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)     7066 2024-05-05 14:43:41.351044 coherent_build-0.2.3/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)      495 2024-05-02 02:13:39.559121 coherent_build-0.2.3/__main__.py
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 14:46:32.466307 coherent_build-0.2.3/coherent/
+lrwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-05 14:46:32.466295 coherent_build-0.2.3/coherent/build -> ..
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      436 2024-05-05 14:49:13.631196 coherent_build-0.2.3/PKG-INFO
```

### Comparing `coherent_build-0.2.2/.DS_Store` & `coherent_build-0.2.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `coherent_build-0.2.2/__init__.py` & `coherent_build-0.2.3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 def normalize(name):
     # todo: do proper normalization
     return name.replace(".", "_")
 
 
 def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
-    metadata = Metadata.from_sdist()
+    metadata = Metadata.from_sdist() or Metadata.discover()
     root = metadata["Name"].replace(".", "/")
     filename = pathlib.Path(wheel_directory) / f"{metadata.id}-py3-none-any.whl"
     with WheelFile(filename, "w") as zf:
         for info in wheel_walk(Wheel(root)):
             zf.write(info.path, arcname=info.name)
         for md_name, contents in make_wheel_metadata(metadata):
             zf.writestr(md_name, contents)
@@ -219,15 +219,16 @@
         yield "Summary", summary_from_github()
         for dep in read_deps():
             yield "Requires-Dist", dep
         yield from description_from_readme()
 
     @classmethod
     def from_sdist(cls):
-        return cls(importlib.metadata.PathDistribution(pathlib.Path()).metadata)
+        sdist_metadata = importlib.metadata.PathDistribution(pathlib.Path()).metadata
+        return (sdist_metadata or None) and cls(sdist_metadata)
 
     def render(self):
         self._description_in_payload()
         return str(self)
 
 
 def guess_content_type(path: pathlib.Path):
```

