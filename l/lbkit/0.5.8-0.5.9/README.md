# Comparing `tmp/lbkit-0.5.8.tar.gz` & `tmp/lbkit-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbkit-0.5.8.tar", last modified: Fri May  3 18:33:06 2024, max compression
+gzip compressed data, was "lbkit-0.5.9.tar", last modified: Sun May  5 17:17:52 2024, max compression
```

## Comparing `lbkit-0.5.8.tar` & `lbkit-0.5.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.637037 lbkit-0.5.8/
--rw-rw-r--   0 root         (0) root         (0)      122 2024-05-03 18:32:59.000000 lbkit-0.5.8/AUTHORS
--rw-rw-r--   0 root         (0) root         (0)    11357 2024-05-03 18:32:59.000000 lbkit-0.5.8/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      149 2024-05-03 18:32:59.000000 lbkit-0.5.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      667 2024-05-03 18:33:06.637037 lbkit-0.5.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      388 2024-05-03 18:32:59.000000 lbkit-0.5.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.633037 lbkit-0.5.8/lbkit/
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-03 18:33:00.000000 lbkit-0.5.8/lbkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.633037 lbkit-0.5.8/lbkit/ci_robot/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/ci_robot/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12840 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/ci_robot/gitee.py
--rw-rw-r--   0 root         (0) root         (0)     8483 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.633037 lbkit-0.5.8/lbkit/codegen/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4241 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/codegen.py
--rw-rw-r--   0 root         (0) root         (0)    22507 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/ctype_defination.py
--rw-rw-r--   0 root         (0) root         (0)    33054 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/idf_interface.py
--rw-rw-r--   0 root         (0) root         (0)      287 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.633037 lbkit-0.5.8/lbkit/codegen/template/
--rw-rw-r--   0 root         (0) root         (0)     6172 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/client.c.mako
--rw-rw-r--   0 root         (0) root         (0)     3048 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/client.h.mako
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/interface.c.mako
--rw-rw-r--   0 root         (0) root         (0)     2297 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/interface.introspect.xml.mako
--rw-rw-r--   0 root         (0) root         (0)    40581 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/public.c.mako
--rw-rw-r--   0 root         (0) root         (0)     9230 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/public.h.mako
--rw-rw-r--   0 root         (0) root         (0)    13342 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/server.c.mako
--rw-rw-r--   0 root         (0) root         (0)     1629 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/codegen/template/server.h.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.633037 lbkit-0.5.8/lbkit/component/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2155 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/arg_parser.py
--rw-rw-r--   0 root         (0) root         (0)    13224 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/build.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.637037 lbkit-0.5.8/lbkit/component/template/
--rw-rw-r--   0 root         (0) root         (0)     9157 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/template/conanbase.mako
--rw-rw-r--   0 root         (0) root         (0)     1289 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/template/deploy.mako
--rw-rw-r--   0 root         (0) root         (0)     5554 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/component/test.py
--rw-rw-r--   0 root         (0) root         (0)     2119 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/errors.py
--rw-rw-r--   0 root         (0) root         (0)      829 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.637037 lbkit-0.5.8/lbkit/integration/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2762 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/build_manifest.py
--rw-rw-r--   0 root         (0) root         (0)     3751 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/build_prepare.py
--rw-rw-r--   0 root         (0) root         (0)     8475 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/build_rootfs.py
--rw-rw-r--   0 root         (0) root         (0)     2890 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/config.py
--rw-rw-r--   0 root         (0) root         (0)     4637 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.637037 lbkit-0.5.8/lbkit/integration/template/
--rw-rw-r--   0 root         (0) root         (0)     1276 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/integration/template/conanfile.py.mako
--rw-rw-r--   0 root         (0) root         (0)      114 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/lbkit.py
--rw-rw-r--   0 root         (0) root         (0)     1355 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/log.py
--rw-rw-r--   0 root         (0) root         (0)     3551 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/misc.py
--rw-rw-r--   0 root         (0) root         (0)     4458 2024-05-03 18:32:59.000000 lbkit-0.5.8/lbkit/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 18:33:06.637037 lbkit-0.5.8/lbkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      667 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1268 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-03 18:33:06.000000 lbkit-0.5.8/lbkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 18:33:06.637037 lbkit-0.5.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1295 2024-05-03 18:32:59.000000 lbkit-0.5.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 17:17:52.758766 lbkit-0.5.9/
+-rw-rw-r--   0 root         (0) root         (0)      122 2024-05-05 17:17:46.000000 lbkit-0.5.9/AUTHORS
+-rw-rw-r--   0 root         (0) root         (0)    11357 2024-05-05 17:17:46.000000 lbkit-0.5.9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      149 2024-05-05 17:17:46.000000 lbkit-0.5.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      667 2024-05-05 17:17:52.758766 lbkit-0.5.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      388 2024-05-05 17:17:46.000000 lbkit-0.5.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 17:17:52.754766 lbkit-0.5.9/lbkit/
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-05 17:17:47.000000 lbkit-0.5.9/lbkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 17:17:52.754766 lbkit-0.5.9/lbkit/ci_robot/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/ci_robot/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12840 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/ci_robot/gitee.py
+-rw-rw-r--   0 root         (0) root         (0)     8483 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 17:17:52.754766 lbkit-0.5.9/lbkit/codegen/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4241 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/codegen.py
+-rw-rw-r--   0 root         (0) root         (0)    22507 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/ctype_defination.py
+-rw-rw-r--   0 root         (0) root         (0)    33306 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/idf_interface.py
+-rw-rw-r--   0 root         (0) root         (0)      287 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 17:17:52.754766 lbkit-0.5.9/lbkit/codegen/template/
+-rw-rw-r--   0 root         (0) root         (0)     6172 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/template/client.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     3048 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/template/client.h.mako
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/template/interface.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     2297 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/template/interface.introspect.xml.mako
+-rw-rw-r--   0 root         (0) root         (0)    40931 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/template/public.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     9230 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/template/public.h.mako
+-rw-rw-r--   0 root         (0) root         (0)    13584 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/template/server.c.mako
+-rw-rw-r--   0 root         (0) root         (0)     1629 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/codegen/template/server.h.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 17:17:52.754766 lbkit-0.5.9/lbkit/component/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/component/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2155 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/component/arg_parser.py
+-rw-rw-r--   0 root         (0) root         (0)    13224 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/component/build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 17:17:52.754766 lbkit-0.5.9/lbkit/component/template/
+-rw-rw-r--   0 root         (0) root         (0)     9157 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/component/template/conanbase.mako
+-rw-rw-r--   0 root         (0) root         (0)     1289 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/component/template/deploy.mako
+-rw-rw-r--   0 root         (0) root         (0)     5554 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/component/test.py
+-rw-rw-r--   0 root         (0) root         (0)     2119 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/errors.py
+-rw-rw-r--   0 root         (0) root         (0)      829 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 17:17:52.758766 lbkit-0.5.9/lbkit/integration/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/integration/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2762 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/integration/build_manifest.py
+-rw-rw-r--   0 root         (0) root         (0)     3751 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/integration/build_prepare.py
+-rw-rw-r--   0 root         (0) root         (0)     8475 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/integration/build_rootfs.py
+-rw-rw-r--   0 root         (0) root         (0)     2890 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/integration/config.py
+-rw-rw-r--   0 root         (0) root         (0)     4637 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/integration/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 17:17:52.758766 lbkit-0.5.9/lbkit/integration/template/
+-rw-rw-r--   0 root         (0) root         (0)     1276 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/integration/template/conanfile.py.mako
+-rw-rw-r--   0 root         (0) root         (0)      114 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/lbkit.py
+-rw-rw-r--   0 root         (0) root         (0)     1355 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/log.py
+-rw-rw-r--   0 root         (0) root         (0)     3551 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/misc.py
+-rw-rw-r--   0 root         (0) root         (0)     4458 2024-05-05 17:17:46.000000 lbkit-0.5.9/lbkit/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 17:17:52.758766 lbkit-0.5.9/lbkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      667 2024-05-05 17:17:52.000000 lbkit-0.5.9/lbkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-05-05 17:17:52.000000 lbkit-0.5.9/lbkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 17:17:52.000000 lbkit-0.5.9/lbkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-05 17:17:52.000000 lbkit-0.5.9/lbkit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-05-05 17:17:52.000000 lbkit-0.5.9/lbkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-05 17:17:52.000000 lbkit-0.5.9/lbkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 17:17:52.758766 lbkit-0.5.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1295 2024-05-05 17:17:46.000000 lbkit-0.5.9/setup.py
```

### Comparing `lbkit-0.5.8/LICENSE` & `lbkit-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/PKG-INFO` & `lbkit-0.5.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbkit
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tools provided by litebmc.com
 Home-page: https://www.litebmc.com
 Author: xuhj@litebmc.com
 Author-email: xuhj@litebmc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbkit-0.5.8/lbkit/ci_robot/gitee.py` & `lbkit-0.5.9/lbkit/ci_robot/gitee.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/cli.py` & `lbkit-0.5.9/lbkit/cli.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/codegen/codegen.py` & `lbkit-0.5.9/lbkit/codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/codegen/ctype_defination.py` & `lbkit-0.5.9/lbkit/codegen/ctype_defination.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/codegen/idf_interface.py` & `lbkit-0.5.9/lbkit/codegen/idf_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     "deprecated": IdfAnnotation("org.freedesktop.DBus.Deprecated", "true"),
     "emits_changes": IdfAnnotation("org.freedesktop.DBus.Property.EmitsChangedSignal", "true"),
     "emits_invalidates": IdfAnnotation("org.freedesktop.DBus.Property.EmitsChangedSignal", "invalidates"),
     "emits_const": IdfAnnotation("org.freedesktop.DBus.Property.EmitsChangedSignal", "const"),
     "emits_false": IdfAnnotation("org.freedesktop.DBus.Property.EmitsChangedSignal", "false"),
     "private": IdfAnnotation("com.litebmc.Dbus.Property.Private", "const"),
     "refobj": IdfAnnotation("com.litebmc.Dbus.Property.RefObject", "true"),
+    "required": IdfAnnotation("com.litebmc.Dbus.Property.Required", "true"),
 }
 
 ACCESS_MAP = {
     "readonly": "read",
     "writeonly": "write",
     "readwrite": "readwrite"
 }
@@ -711,15 +712,18 @@
             sig += prop.signature
         return "(" + sig + ")"
 
     @property
     def odf_schema(self):
         schema = {}
         with_schema_prop_cnt = 0
+        required = []
         for prop in self.properties:
+            if "required" in prop.flags:
+                required.append(prop.name)
             odf = prop.odf_schema(True)
             if odf is not None:
                 schema[prop.name] = odf
                 with_schema_prop_cnt += 1
             else:
                 log.warning(f"the schema of prop {prop.name} is None")
             # 顶层属性可以有一个flags标记属性
@@ -730,14 +734,16 @@
         odf = {
             "$schema": "http://json-schema.org/draft-07/schema#",
             "title": self.name + " schema#",
             "description": f"schema of the interface " + self.name,
             "type": "object",
             "additionalProperties": False
         }
+        if len(required) > 0:
+            odf["required"] = required
         if with_schema_prop_cnt > 0:
             odf["properties"] = schema
             odf["$defs"] = {
                 "ref_value": {
                     "type": "string",
                     "description": "Property reference syntax. The format must be `\\$\\{([<]*|:)<interface>:<object_path>.<property name>\\}`",
                     "pattern": "^\\$\\{([<]*|:)(([a-zA-Z_][A-Za-z0-9_]*)(\\.[a-zA-Z_][A-Za-z0-9_]*)+:)[/]?[A-Z0-9a-z_]+(/[A-Z0-9a-z_]+)*\\.[A-Za-z][a-zA-Z0-9_-]*\\}$"
```

### Comparing `lbkit-0.5.8/lbkit/codegen/template/client.c.mako` & `lbkit-0.5.9/lbkit/codegen/template/client.c.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/codegen/template/client.h.mako` & `lbkit-0.5.9/lbkit/codegen/template/client.h.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/codegen/template/interface.introspect.xml.mako` & `lbkit-0.5.9/lbkit/codegen/template/interface.introspect.xml.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/codegen/template/public.c.mako` & `lbkit-0.5.9/lbkit/codegen/template/public.c.mako`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,15 @@
         % for func in prop.odf_validate(False):
         if (!${func.replace("node,", "val,")})
             valid = FALSE;
         % endfor
         g_string_truncate(prop, len);
     }
     % endfor
+    g_hash_table_destroy(prop_table);
     return valid;
 }
 
 gboolean _validate_odf_as_struct_${name}_v(yaml_document_t *doc, yaml_node_t *node,
     GString *prop, GSList **error_list)
 {
     g_assert(doc && node && prop && error_list);
@@ -1157,16 +1158,22 @@
 static gboolean _validate_odf_prop_${prop.name}(yaml_document_t *doc, GHashTable *prop_table,
     GString *prop, GSList **error_list)
 {
     gboolean valid = TRUE;
     gsize len = prop->len;
     yaml_node_t *node = g_hash_table_lookup(prop_table, "${prop.name}");
     do {
-        if (!node)
+        if (!node) {
+    ## 检查属性是否存在
+    % if "required" in prop.flags:
+            *error_list = g_slist_append(*error_list, g_error_new(ODF_ERROR, ODF_ERROR_PROP_MISSING, "Property %s is missing", prop->str));
+            valid = FALSE;
+    % endif
             break;
+        }
         g_string_append(prop, ".${prop.name}");
     % if "refobj" not in prop.flags:
         if (validate_odf_as_ref_prop(doc, node, prop))
             break;
     % endif
     % if len(prop.odf_validate(True)) > 1:
         % for func in prop.odf_validate(True):
@@ -1193,21 +1200,22 @@
     }
 
     if (node->type != YAML_MAPPING_NODE) {
         *error_list = g_slist_append(*error_list, g_error_new(ODF_ERROR, ODF_ERROR_PROP_VALIDATE_TYPE_ERROR,
             "the node type of object %s is not a mapping, get %s", object_name, gcl_yaml_node_type_str(node->type)));
         return FALSE;
     }
-    GString *prop = g_string_sized_new(128);
+    cleanup_gstring GString *prop = g_string_sized_new(128);
     g_string_printf(prop, "%s", object_name);
     gboolean valid = TRUE;
     GHashTable *prop_table = load_yaml_mapping_to_hash_table(doc, node);
     % for prop in stru.values.parameters:
     valid = _validate_odf_prop_${prop.name}(doc, prop_table, prop, error_list) && valid;
     % endfor
+    g_hash_table_destroy(prop_table);
     return valid;
 }
 
 % if len(intf.plugin.actions) > 0:
 static void __attribute__((constructor(101))) ${class_name}_public_register(void)
 {
     % for action in intf.plugin.actions:
```

### Comparing `lbkit-0.5.8/lbkit/codegen/template/public.h.mako` & `lbkit-0.5.9/lbkit/codegen/template/public.h.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/codegen/template/server.c.mako` & `lbkit-0.5.9/lbkit/codegen/template/server.c.mako`

 * *Files 2% similar despite different names*

```diff
@@ -268,17 +268,19 @@
 {
     const gchar *flags = NULL;
     yaml_node_t *val = g_hash_table_lookup(prop_table, "_${prop.name}_flags");
     if (val && val->type == YAML_SCALAR_NODE) {
         flags = val->data.scalar.value;
     }
     val = g_hash_table_lookup(prop_table, "${prop.name}");
+    ## validate接口在加载odf前完成属性是否必选校验，此处如果是必选属性一定存在
     if (!val) {
         if (flags) {
-            ref_loaded(obj, &${properties}.${prop.name}, NULL, NULL, user_data, flags);
+            ## 属性不存在时传入的value为空，需要开发者在回调函数中完成异常（有flags无属性值）处理
+            ref_loaded(obj, &${properties}.${prop.name}, doc, NULL, user_data, flags);
         }
         return;
     }
     % if "refobj" in prop.flags:
     ref_loaded(obj, &${properties}.${prop.name}, doc, val, user_data, flags);
     % else:
     if (val->type == YAML_SCALAR_NODE && val->data.scalar.value[0] == '$' &&
```

### Comparing `lbkit-0.5.8/lbkit/codegen/template/server.h.mako` & `lbkit-0.5.9/lbkit/codegen/template/server.h.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/component/arg_parser.py` & `lbkit-0.5.9/lbkit/component/arg_parser.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/component/build.py` & `lbkit-0.5.9/lbkit/component/build.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/component/template/conanbase.mako` & `lbkit-0.5.9/lbkit/component/template/conanbase.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/component/template/deploy.mako` & `lbkit-0.5.9/lbkit/component/template/deploy.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/component/test.py` & `lbkit-0.5.9/lbkit/component/test.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/errors.py` & `lbkit-0.5.9/lbkit/errors.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/helper.py` & `lbkit-0.5.9/lbkit/helper.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/integration/build_manifest.py` & `lbkit-0.5.9/lbkit/integration/build_manifest.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/integration/build_prepare.py` & `lbkit-0.5.9/lbkit/integration/build_prepare.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/integration/build_rootfs.py` & `lbkit-0.5.9/lbkit/integration/build_rootfs.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/integration/config.py` & `lbkit-0.5.9/lbkit/integration/config.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/integration/task.py` & `lbkit-0.5.9/lbkit/integration/task.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/integration/template/conanfile.py.mako` & `lbkit-0.5.9/lbkit/integration/template/conanfile.py.mako`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/log.py` & `lbkit-0.5.9/lbkit/log.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/misc.py` & `lbkit-0.5.9/lbkit/misc.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit/tools.py` & `lbkit-0.5.9/lbkit/tools.py`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/lbkit.egg-info/PKG-INFO` & `lbkit-0.5.9/lbkit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbkit
-Version: 0.5.8
+Version: 0.5.9
 Summary: Tools provided by litebmc.com
 Home-page: https://www.litebmc.com
 Author: xuhj@litebmc.com
 Author-email: xuhj@litebmc.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lbkit-0.5.8/lbkit.egg-info/SOURCES.txt` & `lbkit-0.5.9/lbkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbkit-0.5.8/setup.py` & `lbkit-0.5.9/setup.py`

 * *Files identical despite different names*

