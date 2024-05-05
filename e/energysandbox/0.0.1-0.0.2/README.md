# Comparing `tmp/energysandbox-0.0.1.tar.gz` & `tmp/energysandbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energysandbox-0.0.1.tar", last modified: Wed May  1 02:06:25 2024, max compression
+gzip compressed data, was "energysandbox-0.0.2.tar", last modified: Sun May  5 19:49:50 2024, max compression
```

## Comparing `energysandbox-0.0.1.tar` & `energysandbox-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 02:06:25.721583 energysandbox-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-05-01 01:27:20.000000 energysandbox-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      414 2024-05-01 02:06:25.720582 energysandbox-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       35 2024-05-01 01:25:49.000000 energysandbox-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 02:06:25.715582 energysandbox-0.0.1/energysandbox/
-drwxrwxrwx   0        0        0        0 2024-05-01 02:06:25.720582 energysandbox-0.0.1/energysandbox/energysandbox.egg-info/
--rw-rw-rw-   0        0        0      414 2024-05-01 02:06:25.000000 energysandbox-0.0.1/energysandbox/energysandbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-05-01 02:06:25.000000 energysandbox-0.0.1/energysandbox/energysandbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 02:06:25.000000 energysandbox-0.0.1/energysandbox/energysandbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-01 02:06:25.000000 energysandbox-0.0.1/energysandbox/energysandbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 02:06:25.000000 energysandbox-0.0.1/energysandbox/energysandbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 02:06:25.721583 energysandbox-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      857 2024-05-01 02:05:51.000000 energysandbox-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:49:50.266959 energysandbox-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-05-01 01:27:20.000000 energysandbox-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      414 2024-05-05 19:49:50.266959 energysandbox-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       35 2024-05-01 01:25:49.000000 energysandbox-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 19:49:50.256761 energysandbox-0.0.2/energysandbox/
+drwxrwxrwx   0        0        0        0 2024-05-05 19:49:50.265960 energysandbox-0.0.2/energysandbox/energysandbox.egg-info/
+-rw-rw-rw-   0        0        0      414 2024-05-05 19:49:50.000000 energysandbox-0.0.2/energysandbox/energysandbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-05 19:49:50.000000 energysandbox-0.0.2/energysandbox/energysandbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 19:49:50.000000 energysandbox-0.0.2/energysandbox/energysandbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-05 19:49:50.000000 energysandbox-0.0.2/energysandbox/energysandbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 19:49:50.000000 energysandbox-0.0.2/energysandbox/energysandbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 19:49:50.266959 energysandbox-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      857 2024-05-05 19:47:36.000000 energysandbox-0.0.2/setup.py
```

### Comparing `energysandbox-0.0.1/LICENSE.txt` & `energysandbox-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `energysandbox-0.0.1/setup.py` & `energysandbox-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='energysandbox', # name of package which will be package dir below project
-    version='0.0.1',
+    version='0.0.2',
     # url='https://github.com/yourname/yourproject',
     author='Sandstone Group',
     author_email='mtanner@sandstone-group.com',
     description='Energy Sandbox toolset for ETL in the oil and gas business',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(where="energysandbox"),
```

