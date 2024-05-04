# Comparing `tmp/liveflask-1.0.6.tar.gz` & `tmp/liveflask-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveflask-1.0.6.tar", last modified: Wed May  1 22:12:58 2024, max compression
+gzip compressed data, was "liveflask-1.0.7.tar", last modified: Sat May  4 23:27:59 2024, max compression
```

## Comparing `liveflask-1.0.6.tar` & `liveflask-1.0.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 22:12:58.772213 liveflask-1.0.6/
--rw-rw-rw-   0        0        0     1368 2024-05-01 22:12:58.770212 liveflask-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-01 22:12:58.713213 liveflask-1.0.6/liveflask/
--rw-rw-rw-   0        0        0     6131 2024-05-01 20:53:47.000000 liveflask-1.0.6/liveflask/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 22:12:58.722213 liveflask-1.0.6/liveflask/attributes/
--rw-rw-rw-   0        0        0     2023 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 22:12:58.724214 liveflask-1.0.6/liveflask/attributes/__pycache__/
--rw-rw-rw-   0        0        0     3650 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-05-01 22:12:58.726214 liveflask-1.0.6/liveflask/static/
-drwxrwxrwx   0        0        0        0 2024-05-01 22:12:58.740214 liveflask-1.0.6/liveflask/static/liveflask/
--rw-rw-rw-   0        0        0     1566 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/static/liveflask/action.js
--rw-rw-rw-   0        0        0        0 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/static/liveflask/constants.js
--rw-rw-rw-   0        0        0      245 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/static/liveflask/events.js
--rw-rw-rw-   0        0        0      872 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/static/liveflask/liveflask.js
--rw-rw-rw-   0        0        0     2191 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/static/liveflask/model.js
--rw-rw-rw-   0        0        0     1660 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/static/liveflask/polling.js
--rw-rw-rw-   0        0        0     8474 2024-05-01 22:11:00.000000 liveflask-1.0.6/liveflask/static/liveflask/utils.js
--rw-rw-rw-   0        0        0    73154 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/static/lodash.min.js
-drwxrwxrwx   0        0        0        0 2024-05-01 22:12:58.742213 liveflask-1.0.6/liveflask/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/templates/liveflask-head.html
--rw-rw-rw-   0        0        0      348 2024-05-01 22:10:42.000000 liveflask-1.0.6/liveflask/templates/liveflask-scripts.html
-drwxrwxrwx   0        0        0        0 2024-05-01 22:12:58.756213 liveflask-1.0.6/liveflask/traits/
--rw-rw-rw-   0        0        0      205 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/Bootable.py
--rw-rw-rw-   0        0        0        0 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 22:12:58.768214 liveflask-1.0.6/liveflask/traits/__pycache__/
--rw-rw-rw-   0        0        0      867 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
--rw-rw-rw-   0        0        0      198 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3292 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
--rw-rw-rw-   0        0        0     4272 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/__pycache__/has_props.cpython-311.pyc
--rw-rw-rw-   0        0        0     2835 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
--rw-rw-rw-   0        0        0     4776 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
--rw-rw-rw-   0        0        0     2042 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/has_actions.py
--rw-rw-rw-   0        0        0     2488 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/has_props.py
--rw-rw-rw-   0        0        0     2486 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/has_renders.py
--rw-rw-rw-   0        0        0     4106 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/traits/has_snapshots.py
--rw-rw-rw-   0        0        0     2032 2024-05-01 20:37:18.000000 liveflask-1.0.6/liveflask/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-01 22:12:58.720214 liveflask-1.0.6/liveflask.egg-info/
--rw-rw-rw-   0        0        0     1368 2024-05-01 22:12:58.000000 liveflask-1.0.6/liveflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1204 2024-05-01 22:12:58.000000 liveflask-1.0.6/liveflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 22:12:58.000000 liveflask-1.0.6/liveflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-01 22:12:58.000000 liveflask-1.0.6/liveflask.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-01 22:12:58.000000 liveflask-1.0.6/liveflask.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 22:12:58.772213 liveflask-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1222 2024-05-01 22:12:54.000000 liveflask-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.459731 liveflask-1.0.7/
+-rw-rw-rw-   0        0        0     1368 2024-05-04 23:27:59.458729 liveflask-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.411729 liveflask-1.0.7/liveflask/
+-rw-rw-rw-   0        0        0     6302 2024-05-04 23:25:43.000000 liveflask-1.0.7/liveflask/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.419730 liveflask-1.0.7/liveflask/attributes/
+-rw-rw-rw-   0        0        0     2023 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.420729 liveflask-1.0.7/liveflask/attributes/__pycache__/
+-rw-rw-rw-   0        0        0     3650 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/attributes/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.422729 liveflask-1.0.7/liveflask/static/
+drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.433731 liveflask-1.0.7/liveflask/static/liveflask/
+-rw-rw-rw-   0        0        0     1566 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/action.js
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/constants.js
+-rw-rw-rw-   0        0        0      245 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/events.js
+-rw-rw-rw-   0        0        0      872 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/liveflask.js
+-rw-rw-rw-   0        0        0     2191 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/model.js
+-rw-rw-rw-   0        0        0     1660 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/liveflask/polling.js
+-rw-rw-rw-   0        0        0     8475 2024-05-04 23:27:21.000000 liveflask-1.0.7/liveflask/static/liveflask/utils.js
+-rw-rw-rw-   0        0        0    73154 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/static/lodash.min.js
+drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.436729 liveflask-1.0.7/liveflask/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/templates/liveflask-head.html
+-rw-rw-rw-   0        0        0      348 2024-05-04 23:19:29.000000 liveflask-1.0.7/liveflask/templates/liveflask-scripts.html
+drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.446729 liveflask-1.0.7/liveflask/traits/
+-rw-rw-rw-   0        0        0      205 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/Bootable.py
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.456728 liveflask-1.0.7/liveflask/traits/__pycache__/
+-rw-rw-rw-   0        0        0      867 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/Bootable.cpython-311.pyc
+-rw-rw-rw-   0        0        0      198 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3292 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/has_actions.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4272 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/has_props.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2835 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/has_renders.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4776 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2042 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/has_actions.py
+-rw-rw-rw-   0        0        0     2488 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/has_props.py
+-rw-rw-rw-   0        0        0     2486 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/has_renders.py
+-rw-rw-rw-   0        0        0     4106 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/traits/has_snapshots.py
+-rw-rw-rw-   0        0        0     2032 2024-05-01 21:07:09.000000 liveflask-1.0.7/liveflask/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-04 23:27:59.417729 liveflask-1.0.7/liveflask.egg-info/
+-rw-rw-rw-   0        0        0     1368 2024-05-04 23:27:59.000000 liveflask-1.0.7/liveflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1204 2024-05-04 23:27:59.000000 liveflask-1.0.7/liveflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 23:27:59.000000 liveflask-1.0.7/liveflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-04 23:27:59.000000 liveflask-1.0.7/liveflask.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-04 23:27:59.000000 liveflask-1.0.7/liveflask.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 23:27:59.459731 liveflask-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1222 2024-05-04 23:27:46.000000 liveflask-1.0.7/setup.py
```

### Comparing `liveflask-1.0.6/PKG-INFO` & `liveflask-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.6
+Version: 1.0.7
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.6/liveflask/__init__.py` & `liveflask-1.0.7/liveflask/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import ast
 import functools
 import os
 import secrets
 import gzip
-from flask import Blueprint, render_template, Response
+from flask import Blueprint, render_template, Response, Flask
 from flask import request
 from markupsafe import Markup
-
+from flask_wtf import CSRFProtect
 from .traits.has_actions import HasActions
 from .traits.has_props import HasProps
 from .traits.has_renders import HasRenders
 from .traits.has_snapshots import HasSnapshots
 
 
 def parse_argument(arg):
@@ -83,19 +83,24 @@
     return DecoratedClass
 
 
 class LiveFlask(HasRenders, HasProps, HasSnapshots, HasActions):
     pass
 
 
-def LiveFlaskExt(app):
+def LiveFlaskExt(app: Flask):
     app.add_template_global(
         LiveFlask().inital_render, 'live'
     )
 
+    if "csrf" not in list(app.extensions.keys()):
+        # register CSRF protection
+        csrf = CSRFProtect(app)
+
+
     package_dir = os.path.dirname(os.path.abspath(__file__))
     enduser_project_dir = os.getcwd()
     # check if the project directory has a templates folder
     if not os.path.exists(f"{enduser_project_dir}/templates"):
         os.makedirs(f"{enduser_project_dir}/templates")
 
     # check if the templates folder has a liveflask folder
```

### Comparing `liveflask-1.0.6/liveflask/attributes/__init__.py` & `liveflask-1.0.7/liveflask/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask/attributes/__pycache__/__init__.cpython-311.pyc` & `liveflask-1.0.7/liveflask/attributes/__pycache__/__init__.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
+moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
 files sz: 2023
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.6/liveflask/static/liveflask/action.js` & `liveflask-1.0.7/liveflask/static/liveflask/action.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask/static/liveflask/liveflask.js` & `liveflask-1.0.7/liveflask/static/liveflask/liveflask.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask/static/liveflask/model.js` & `liveflask-1.0.7/liveflask/static/liveflask/model.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask/static/liveflask/polling.js` & `liveflask-1.0.7/liveflask/static/liveflask/polling.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask/static/liveflask/utils.js` & `liveflask-1.0.7/liveflask/static/liveflask/utils.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with CRLF line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -238,293 +238,293 @@
 00000ed0: 6566 6c61 736b 2f22 2c20 7b0d 0a20 2020  eflask/", {..   
 00000ee0: 2020 2020 206d 6574 686f 643a 2022 504f       method: "PO
 00000ef0: 5354 222c 0d0a 2020 2020 2020 2020 6865  ST",..        he
 00000f00: 6164 6572 733a 207b 2243 6f6e 7465 6e74  aders: {"Content
 00000f10: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
 00000f20: 7469 6f6e 2f6a 736f 6e22 2c20 2258 2d43  tion/json", "X-C
 00000f30: 5352 462d 546f 6b65 6e22 3a20 6373 7266  SRF-Token": csrf
-00000f40: 546f 6b65 6e7d 2c0d 0a20 2020 2020 2020  Token},..       
-00000f50: 2062 6f64 793a 204a 534f 4e2e 7374 7269   body: JSON.stri
-00000f60: 6e67 6966 7928 7b0d 0a20 2020 2020 2020  ngify({..       
-00000f70: 2020 2020 2073 6e61 7073 686f 743a 2073       snapshot: s
-00000f80: 6e61 7073 686f 742c 0d0a 2020 2020 2020  napshot,..      
-00000f90: 2020 2020 2020 2e2e 2e61 6464 5f74 6f5f        ...add_to_
-00000fa0: 7061 796c 6f61 640d 0a20 2020 2020 2020  payload..       
-00000fb0: 207d 290d 0a20 2020 207d 292e 7468 656e   })..    }).then
-00000fc0: 2869 203d 3e20 692e 6a73 6f6e 2829 292e  (i => i.json()).
-00000fd0: 7468 656e 2872 6573 706f 6e73 6520 3d3e  then(response =>
-00000fe0: 207b 0d0a 2020 2020 2020 2020 6c65 7420   {..        let 
-00000ff0: 7b68 746d 6c2c 2073 6e61 7073 686f 747d  {html, snapshot}
-00001000: 203d 2072 6573 706f 6e73 650d 0a20 2020   = response..   
-00001010: 2020 2020 2065 6c2e 5f5f 6c69 7665 666c       el.__livefl
-00001020: 6173 6b20 3d20 736e 6170 7368 6f74 0d0a  ask = snapshot..
-00001030: 2020 2020 2020 2020 656c 2e5f 5f6c 6976          el.__liv
-00001040: 6566 6c61 736b 5b27 6368 696c 6472 656e  eflask['children
-00001050: 275d 203d 2063 6869 6c64 7265 6e0d 0a0d  '] = children...
-00001060: 0a20 2020 2020 2020 2069 6620 2874 6172  .        if (tar
-00001070: 6765 742e 6861 7341 7474 7269 6275 7465  get.hasAttribute
-00001080: 2822 6461 7461 2d70 6f6c 6c22 2920 3d3d  ("data-poll") ==
-00001090: 3d20 7472 7565 2920 7b0d 0a20 2020 2020  = true) {..     
-000010a0: 2020 2020 2020 206d 6f72 7068 646f 6d28         morphdom(
-000010b0: 7461 7267 6574 2c20 6372 6561 7465 456c  target, createEl
-000010c0: 656d 656e 7446 726f 6d48 544d 4c28 6874  ementFromHTML(ht
-000010d0: 6d6c 292e 7175 6572 7953 656c 6563 746f  ml).querySelecto
-000010e0: 7228 605b 6461 7461 2d70 6f6c 6c3d 247b  r(`[data-poll=${
-000010f0: 7461 7267 6574 2e67 6574 4174 7472 6962  target.getAttrib
-00001100: 7574 6528 2764 6174 612d 706f 6c6c 2729  ute('data-poll')
-00001110: 7d5d 6029 2e6f 7574 6572 4854 4d4c 290d  }]`).outerHTML).
-00001120: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001130: 7572 6e3b 0d0a 2020 2020 2020 2020 7d0d  urn;..        }.
-00001140: 0a0d 0a20 2020 2020 2020 2075 7064 6174  ...        updat
-00001150: 655f 646f 6d28 656c 2c20 6874 6d6c 290d  e_dom(el, html).
-00001160: 0a0d 0a20 2020 2020 2020 206c 6574 2065  ...        let e
-00001170: 6d69 7473 203d 2065 6c2e 5f5f 6c69 7665  mits = el.__live
-00001180: 666c 6173 6b3f 2e64 6174 613f 2e65 6d69  flask?.data?.emi
-00001190: 7473 3b0d 0a0d 0a20 2020 2020 2020 2069  ts;....        i
-000011a0: 6620 2865 6d69 7473 2021 3d3d 2075 6e64  f (emits !== und
-000011b0: 6566 696e 6564 2920 7b0d 0a20 2020 2020  efined) {..     
-000011c0: 2020 2020 2020 202f 2a20 6c6f 6f70 2074         /* loop t
-000011d0: 6872 6f75 6768 2074 6865 2065 6d69 7473  hrough the emits
-000011e0: 2061 6e64 2066 6972 6520 7468 6520 6576   and fire the ev
-000011f0: 656e 7473 202a 2f0d 0a20 2020 2020 2020  ents */..       
-00001200: 2020 2020 204f 626a 6563 742e 6b65 7973       Object.keys
-00001210: 2865 6d69 7473 292e 666f 7245 6163 6828  (emits).forEach(
-00001220: 6576 656e 7420 3d3e 207b 0d0a 2020 2020  event => {..    
-00001230: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
-00001240: 6375 7272 656e 745f 6576 656e 7420 3d20  current_event = 
-00001250: 656d 6974 735b 6576 656e 745d 0d0a 2020  emits[event]..  
-00001260: 2020 2020 2020 2020 2020 2020 2020 2f2f                //
-00001270: 204c 6f76 6520 7468 6973 206f 6e65 2063   Love this one c
-00001280: 6f6e 736f 6c65 2e6c 6f67 2822 4375 7272  onsole.log("Curr
-00001290: 656e 7420 4576 656e 743a 2022 2c20 6375  ent Event: ", cu
-000012a0: 7272 656e 745f 6576 656e 7429 0d0a 2020  rrent_event)..  
-000012b0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-000012c0: 7420 6576 656e 745f 6e61 6d65 203d 2063  t event_name = c
-000012d0: 7572 7265 6e74 5f65 7665 6e74 5b27 6576  urrent_event['ev
-000012e0: 656e 7427 5d0d 0a20 2020 2020 2020 2020  ent']..         
-000012f0: 2020 2020 2020 206c 6574 2065 7665 6e74         let event
-00001300: 5f70 6172 616d 7320 3d20 6375 7272 656e  _params = curren
-00001310: 745f 6576 656e 745b 2770 6172 616d 7327  t_event['params'
-00001320: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00001330: 2020 206c 6574 206b 7761 7267 7320 3d20     let kwargs = 
-00001340: 6375 7272 656e 745f 6576 656e 745b 276b  current_event['k
-00001350: 7761 7267 7327 5d0d 0a20 2020 2020 2020  wargs']..       
-00001360: 2020 2020 2020 2020 206c 6574 2074 6f20           let to 
-00001370: 3d20 6375 7272 656e 745f 6576 656e 745b  = current_event[
-00001380: 2774 6f27 5d0d 0a20 2020 2020 2020 2020  'to']..         
-00001390: 2020 2020 2020 206c 6574 2066 696e 616c         let final
-000013a0: 5f70 6172 616d 7320 3d20 6576 656e 745f  _params = event_
-000013b0: 6e61 6d65 0d0a 2020 2020 2020 2020 2020  name..          
-000013c0: 2020 2020 2020 2f2f 204c 6f76 6520 7468        // Love th
-000013d0: 6973 206f 6e65 2063 6f6e 736f 6c65 2e6c  is one console.l
-000013e0: 6f67 2822 456d 6974 7465 6420 4576 656e  og("Emitted Even
-000013f0: 743a 2022 2c20 6576 656e 745f 6e61 6d65  t: ", event_name
-00001400: 2c20 2220 7769 7468 2070 6172 616d 733a  , " with params:
-00001410: 2022 2c20 6576 656e 745f 7061 7261 6d73   ", event_params
-00001420: 2c20 2220 746f 3a20 222c 2074 6f29 0d0a  , " to: ", to)..
-00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001440: 646f 6375 6d65 6e74 2e64 6973 7061 7463  document.dispatc
-00001450: 6845 7665 6e74 286e 6577 2043 7573 746f  hEvent(new Custo
-00001460: 6d45 7665 6e74 2865 7665 6e74 5f6e 616d  mEvent(event_nam
-00001470: 652c 207b 0d0a 2020 2020 2020 2020 2020  e, {..          
-00001480: 2020 2020 2020 2020 2020 6465 7461 696c            detail
-00001490: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
-000014a0: 2020 2020 2020 2020 2020 2020 2065 7665               eve
-000014b0: 6e74 3a20 6576 656e 745f 6e61 6d65 2c0d  nt: event_name,.
-000014c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000014d0: 2020 2020 2020 2020 2070 6172 616d 733a           params:
-000014e0: 2065 7665 6e74 5f70 6172 616d 732c 0d0a   event_params,..
-000014f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001500: 2020 2020 2020 2020 6b77 6172 6773 3a20          kwargs: 
-00001510: 6b77 6172 6773 2c0d 0a20 2020 2020 2020  kwargs,..       
-00001520: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
-00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 7d29 293b 0d0a 2020 2020 2020 2020 2020  }));..          
-00001550: 2020 2020 2020 6966 2028 746f 203d 3d3d        if (to ===
-00001560: 2022 7365 6c66 2229 207b 0d0a 2020 2020   "self") {..    
+00000f40: 546f 6b65 6e7d 202c 0d0a 2020 2020 2020  Token} ,..      
+00000f50: 2020 626f 6479 3a20 4a53 4f4e 2e73 7472    body: JSON.str
+00000f60: 696e 6769 6679 287b 0d0a 2020 2020 2020  ingify({..      
+00000f70: 2020 2020 2020 736e 6170 7368 6f74 3a20        snapshot: 
+00000f80: 736e 6170 7368 6f74 2c0d 0a20 2020 2020  snapshot,..     
+00000f90: 2020 2020 2020 202e 2e2e 6164 645f 746f         ...add_to
+00000fa0: 5f70 6179 6c6f 6164 0d0a 2020 2020 2020  _payload..      
+00000fb0: 2020 7d29 0d0a 2020 2020 7d29 2e74 6865    })..    }).the
+00000fc0: 6e28 6920 3d3e 2069 2e6a 736f 6e28 2929  n(i => i.json())
+00000fd0: 2e74 6865 6e28 7265 7370 6f6e 7365 203d  .then(response =
+00000fe0: 3e20 7b0d 0a20 2020 2020 2020 206c 6574  > {..        let
+00000ff0: 207b 6874 6d6c 2c20 736e 6170 7368 6f74   {html, snapshot
+00001000: 7d20 3d20 7265 7370 6f6e 7365 0d0a 2020  } = response..  
+00001010: 2020 2020 2020 656c 2e5f 5f6c 6976 6566        el.__livef
+00001020: 6c61 736b 203d 2073 6e61 7073 686f 740d  lask = snapshot.
+00001030: 0a20 2020 2020 2020 2065 6c2e 5f5f 6c69  .        el.__li
+00001040: 7665 666c 6173 6b5b 2763 6869 6c64 7265  veflask['childre
+00001050: 6e27 5d20 3d20 6368 696c 6472 656e 0d0a  n'] = children..
+00001060: 0d0a 2020 2020 2020 2020 6966 2028 7461  ..        if (ta
+00001070: 7267 6574 2e68 6173 4174 7472 6962 7574  rget.hasAttribut
+00001080: 6528 2264 6174 612d 706f 6c6c 2229 203d  e("data-poll") =
+00001090: 3d3d 2074 7275 6529 207b 0d0a 2020 2020  == true) {..    
+000010a0: 2020 2020 2020 2020 6d6f 7270 6864 6f6d          morphdom
+000010b0: 2874 6172 6765 742c 2063 7265 6174 6545  (target, createE
+000010c0: 6c65 6d65 6e74 4672 6f6d 4854 4d4c 2868  lementFromHTML(h
+000010d0: 746d 6c29 2e71 7565 7279 5365 6c65 6374  tml).querySelect
+000010e0: 6f72 2860 5b64 6174 612d 706f 6c6c 3d24  or(`[data-poll=$
+000010f0: 7b74 6172 6765 742e 6765 7441 7474 7269  {target.getAttri
+00001100: 6275 7465 2827 6461 7461 2d70 6f6c 6c27  bute('data-poll'
+00001110: 297d 5d60 292e 6f75 7465 7248 544d 4c29  )}]`).outerHTML)
+00001120: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00001130: 7475 726e 3b0d 0a20 2020 2020 2020 207d  turn;..        }
+00001140: 0d0a 0d0a 2020 2020 2020 2020 7570 6461  ....        upda
+00001150: 7465 5f64 6f6d 2865 6c2c 2068 746d 6c29  te_dom(el, html)
+00001160: 0d0a 0d0a 2020 2020 2020 2020 6c65 7420  ....        let 
+00001170: 656d 6974 7320 3d20 656c 2e5f 5f6c 6976  emits = el.__liv
+00001180: 6566 6c61 736b 3f2e 6461 7461 3f2e 656d  eflask?.data?.em
+00001190: 6974 733b 0d0a 0d0a 2020 2020 2020 2020  its;....        
+000011a0: 6966 2028 656d 6974 7320 213d 3d20 756e  if (emits !== un
+000011b0: 6465 6669 6e65 6429 207b 0d0a 2020 2020  defined) {..    
+000011c0: 2020 2020 2020 2020 2f2a 206c 6f6f 7020          /* loop 
+000011d0: 7468 726f 7567 6820 7468 6520 656d 6974  through the emit
+000011e0: 7320 616e 6420 6669 7265 2074 6865 2065  s and fire the e
+000011f0: 7665 6e74 7320 2a2f 0d0a 2020 2020 2020  vents */..      
+00001200: 2020 2020 2020 4f62 6a65 6374 2e6b 6579        Object.key
+00001210: 7328 656d 6974 7329 2e66 6f72 4561 6368  s(emits).forEach
+00001220: 2865 7665 6e74 203d 3e20 7b0d 0a20 2020  (event => {..   
+00001230: 2020 2020 2020 2020 2020 2020 206c 6574               let
+00001240: 2063 7572 7265 6e74 5f65 7665 6e74 203d   current_event =
+00001250: 2065 6d69 7473 5b65 7665 6e74 5d0d 0a20   emits[event].. 
+00001260: 2020 2020 2020 2020 2020 2020 2020 202f                 /
+00001270: 2f20 4c6f 7665 2074 6869 7320 6f6e 6520  / Love this one 
+00001280: 636f 6e73 6f6c 652e 6c6f 6728 2243 7572  console.log("Cur
+00001290: 7265 6e74 2045 7665 6e74 3a20 222c 2063  rent Event: ", c
+000012a0: 7572 7265 6e74 5f65 7665 6e74 290d 0a20  urrent_event).. 
+000012b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000012c0: 6574 2065 7665 6e74 5f6e 616d 6520 3d20  et event_name = 
+000012d0: 6375 7272 656e 745f 6576 656e 745b 2765  current_event['e
+000012e0: 7665 6e74 275d 0d0a 2020 2020 2020 2020  vent']..        
+000012f0: 2020 2020 2020 2020 6c65 7420 6576 656e          let even
+00001300: 745f 7061 7261 6d73 203d 2063 7572 7265  t_params = curre
+00001310: 6e74 5f65 7665 6e74 5b27 7061 7261 6d73  nt_event['params
+00001320: 275d 0d0a 2020 2020 2020 2020 2020 2020  ']..            
+00001330: 2020 2020 6c65 7420 6b77 6172 6773 203d      let kwargs =
+00001340: 2063 7572 7265 6e74 5f65 7665 6e74 5b27   current_event['
+00001350: 6b77 6172 6773 275d 0d0a 2020 2020 2020  kwargs']..      
+00001360: 2020 2020 2020 2020 2020 6c65 7420 746f            let to
+00001370: 203d 2063 7572 7265 6e74 5f65 7665 6e74   = current_event
+00001380: 5b27 746f 275d 0d0a 2020 2020 2020 2020  ['to']..        
+00001390: 2020 2020 2020 2020 6c65 7420 6669 6e61          let fina
+000013a0: 6c5f 7061 7261 6d73 203d 2065 7665 6e74  l_params = event
+000013b0: 5f6e 616d 650d 0a20 2020 2020 2020 2020  _name..         
+000013c0: 2020 2020 2020 202f 2f20 4c6f 7665 2074         // Love t
+000013d0: 6869 7320 6f6e 6520 636f 6e73 6f6c 652e  his one console.
+000013e0: 6c6f 6728 2245 6d69 7474 6564 2045 7665  log("Emitted Eve
+000013f0: 6e74 3a20 222c 2065 7665 6e74 5f6e 616d  nt: ", event_nam
+00001400: 652c 2022 2077 6974 6820 7061 7261 6d73  e, " with params
+00001410: 3a20 222c 2065 7665 6e74 5f70 6172 616d  : ", event_param
+00001420: 732c 2022 2074 6f3a 2022 2c20 746f 290d  s, " to: ", to).
+00001430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001440: 2064 6f63 756d 656e 742e 6469 7370 6174   document.dispat
+00001450: 6368 4576 656e 7428 6e65 7720 4375 7374  chEvent(new Cust
+00001460: 6f6d 4576 656e 7428 6576 656e 745f 6e61  omEvent(event_na
+00001470: 6d65 2c20 7b0d 0a20 2020 2020 2020 2020  me, {..         
+00001480: 2020 2020 2020 2020 2020 2064 6574 6169             detai
+00001490: 6c3a 207b 0d0a 2020 2020 2020 2020 2020  l: {..          
+000014a0: 2020 2020 2020 2020 2020 2020 2020 6576                ev
+000014b0: 656e 743a 2065 7665 6e74 5f6e 616d 652c  ent: event_name,
+000014c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000014d0: 2020 2020 2020 2020 2020 7061 7261 6d73            params
+000014e0: 3a20 6576 656e 745f 7061 7261 6d73 2c0d  : event_params,.
+000014f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001500: 2020 2020 2020 2020 206b 7761 7267 733a           kwargs:
+00001510: 206b 7761 7267 732c 0d0a 2020 2020 2020   kwargs,..      
+00001520: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
+00001530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001540: 207d 2929 3b0d 0a20 2020 2020 2020 2020   }));..         
+00001550: 2020 2020 2020 2069 6620 2874 6f20 3d3d         if (to ==
+00001560: 3d20 2273 656c 6622 2920 7b0d 0a20 2020  = "self") {..   
 00001570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001580: 7365 6e64 5f72 6571 7565 7374 2865 6c2c  send_request(el,
-00001590: 207b 6d65 7468 6f64 3a20 2265 6d69 7422   {method: "emit"
-000015a0: 2c20 6172 6773 3a20 6669 6e61 6c5f 7061  , args: final_pa
-000015b0: 7261 6d73 2c20 6b77 6172 6773 3a20 6b77  rams, kwargs: kw
-000015c0: 6172 6773 7d2c 2074 6172 6765 7429 2e74  args}, target).t
-000015d0: 6865 6e28 2829 203d 3e20 7b0d 0a20 2020  hen(() => {..   
+00001580: 2073 656e 645f 7265 7175 6573 7428 656c   send_request(el
+00001590: 2c20 7b6d 6574 686f 643a 2022 656d 6974  , {method: "emit
+000015a0: 222c 2061 7267 733a 2066 696e 616c 5f70  ", args: final_p
+000015b0: 6172 616d 732c 206b 7761 7267 733a 206b  arams, kwargs: k
+000015c0: 7761 7267 737d 2c20 7461 7267 6574 292e  wargs}, target).
+000015d0: 7468 656e 2828 2920 3d3e 207b 0d0a 2020  then(() => {..  
 000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015f0: 2020 2020 202f 2f20 5570 6461 7465 2044       // Update D
-00001600: 4f4d 2073 796e 6368 726f 6e6f 7573 6c79  OM synchronously
-00001610: 2061 6674 6572 2065 6d69 7474 696e 6720   after emitting 
-00001620: 6576 656e 7473 0d0a 2020 2020 2020 2020  events..        
+000015f0: 2020 2020 2020 2f2f 2055 7064 6174 6520        // Update 
+00001600: 444f 4d20 7379 6e63 6872 6f6e 6f75 736c  DOM synchronousl
+00001610: 7920 6166 7465 7220 656d 6974 7469 6e67  y after emitting
+00001620: 2065 7665 6e74 730d 0a20 2020 2020 2020   events..       
 00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001640: 7570 6461 7465 5f64 6f6d 2865 6c2c 2065  update_dom(el, e
-00001650: 6c2e 696e 6e65 7248 544d 4c29 3b0d 0a20  l.innerHTML);.. 
+00001640: 2075 7064 6174 655f 646f 6d28 656c 2c20   update_dom(el, 
+00001650: 656c 2e69 6e6e 6572 4854 4d4c 293b 0d0a  el.innerHTML);..
 00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 207d 293b 0d0a 2020 2020 2020 2020     });..        
-00001680: 2020 2020 2020 2020 7d20 656c 7365 2069          } else i
-00001690: 6620 2874 6f20 3d3d 3d20 2261 6c6c 2229  f (to === "all")
-000016a0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000016b0: 2020 2020 2020 2020 6c65 7420 636f 6d70          let comp
-000016c0: 6f6e 656e 7473 203d 2064 6f63 756d 656e  onents = documen
-000016d0: 742e 7175 6572 7953 656c 6563 746f 7241  t.querySelectorA
-000016e0: 6c6c 2860 5b64 6174 612d 636f 6d70 6f6e  ll(`[data-compon
-000016f0: 656e 745d 6029 0d0a 2020 2020 2020 2020  ent]`)..        
-00001700: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
-00001710: 6f6e 656e 7473 2e66 6f72 4561 6368 2863  onents.forEach(c
-00001720: 6f6d 706f 6e65 6e74 203d 3e20 7b0d 0a20  omponent => {.. 
+00001670: 2020 2020 7d29 3b0d 0a20 2020 2020 2020      });..       
+00001680: 2020 2020 2020 2020 207d 2065 6c73 6520           } else 
+00001690: 6966 2028 746f 203d 3d3d 2022 616c 6c22  if (to === "all"
+000016a0: 2920 7b0d 0a20 2020 2020 2020 2020 2020  ) {..           
+000016b0: 2020 2020 2020 2020 206c 6574 2063 6f6d           let com
+000016c0: 706f 6e65 6e74 7320 3d20 646f 6375 6d65  ponents = docume
+000016d0: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
+000016e0: 416c 6c28 605b 6461 7461 2d63 6f6d 706f  All(`[data-compo
+000016f0: 6e65 6e74 5d60 290d 0a20 2020 2020 2020  nent]`)..       
+00001700: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+00001710: 706f 6e65 6e74 732e 666f 7245 6163 6828  ponents.forEach(
+00001720: 636f 6d70 6f6e 656e 7420 3d3e 207b 0d0a  component => {..
 00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2020 2020 2020 202f 2f20 4c6f 7665 2074         // Love t
-00001750: 6869 7320 6f6e 6520 636f 6e73 6f6c 652e  his one console.
-00001760: 6c6f 6728 2245 6d69 7474 696e 6720 746f  log("Emitting to
-00001770: 2061 6c6c 2063 6f6d 706f 6e65 6e74 202d   all component -
-00001780: 2022 2c20 636f 6d70 6f6e 656e 742c 2022   ", component, "
-00001790: 2077 6974 6820 7061 7261 6d73 3a20 222c   with params: ",
-000017a0: 2066 696e 616c 5f70 6172 616d 7329 0d0a   final_params)..
-000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017c0: 2020 2020 2020 2020 7365 6e64 5f72 6571          send_req
-000017d0: 7565 7374 2863 6f6d 706f 6e65 6e74 2c20  uest(component, 
-000017e0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-000017f0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00001800: 6574 686f 643a 2022 656d 6974 222c 0d0a  ethod: "emit",..
-00001810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001820: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00001830: 3a20 6669 6e61 6c5f 7061 7261 6d73 2c0d  : final_params,.
-00001840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001850: 2020 2020 2020 2020 2020 2020 206b 7761               kwa
-00001860: 7267 733a 206b 7761 7267 730d 0a20 2020  rgs: kwargs..   
+00001740: 2020 2020 2020 2020 2f2f 204c 6f76 6520          // Love 
+00001750: 7468 6973 206f 6e65 2063 6f6e 736f 6c65  this one console
+00001760: 2e6c 6f67 2822 456d 6974 7469 6e67 2074  .log("Emitting t
+00001770: 6f20 616c 6c20 636f 6d70 6f6e 656e 7420  o all component 
+00001780: 2d20 222c 2063 6f6d 706f 6e65 6e74 2c20  - ", component, 
+00001790: 2220 7769 7468 2070 6172 616d 733a 2022  " with params: "
+000017a0: 2c20 6669 6e61 6c5f 7061 7261 6d73 290d  , final_params).
+000017b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000017c0: 2020 2020 2020 2020 2073 656e 645f 7265           send_re
+000017d0: 7175 6573 7428 636f 6d70 6f6e 656e 742c  quest(component,
+000017e0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001800: 6d65 7468 6f64 3a20 2265 6d69 7422 2c0d  method: "emit",.
+00001810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001820: 2020 2020 2020 2020 2020 2020 2061 7267               arg
+00001830: 733a 2066 696e 616c 5f70 6172 616d 732c  s: final_params,
+00001840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001850: 2020 2020 2020 2020 2020 2020 2020 6b77                kw
+00001860: 6172 6773 3a20 6b77 6172 6773 0d0a 2020  args: kwargs..  
 00001870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001880: 2020 2020 207d 2c20 7461 7267 6574 293b       }, target);
-00001890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000018a0: 2020 2020 2020 7d29 0d0a 2020 2020 2020        })..      
-000018b0: 2020 2020 2020 2020 2020 7d20 656c 7365            } else
-000018c0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000018d0: 2020 2020 2020 2020 6c65 7420 636f 6d70          let comp
-000018e0: 6f6e 656e 7473 203d 2064 6f63 756d 656e  onents = documen
-000018f0: 742e 7175 6572 7953 656c 6563 746f 7241  t.querySelectorA
-00001900: 6c6c 2860 5b64 6174 612d 636f 6d70 6f6e  ll(`[data-compon
-00001910: 656e 743d 247b 746f 7d5d 6029 0d0a 2020  ent=${to}]`)..  
+00001880: 2020 2020 2020 7d2c 2074 6172 6765 7429        }, target)
+00001890: 3b0d 0a20 2020 2020 2020 2020 2020 2020  ;..             
+000018a0: 2020 2020 2020 207d 290d 0a20 2020 2020         })..     
+000018b0: 2020 2020 2020 2020 2020 207d 2065 6c73             } els
+000018c0: 6520 7b0d 0a20 2020 2020 2020 2020 2020  e {..           
+000018d0: 2020 2020 2020 2020 206c 6574 2063 6f6d           let com
+000018e0: 706f 6e65 6e74 7320 3d20 646f 6375 6d65  ponents = docume
+000018f0: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
+00001900: 416c 6c28 605b 6461 7461 2d63 6f6d 706f  All(`[data-compo
+00001910: 6e65 6e74 3d24 7b74 6f7d 5d60 290d 0a20  nent=${to}]`).. 
 00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001930: 2020 636f 6d70 6f6e 656e 7473 2e66 6f72    components.for
-00001940: 4561 6368 2863 6f6d 706f 6e65 6e74 203d  Each(component =
-00001950: 3e20 7b0d 0a20 2020 2020 2020 2020 2020  > {..           
-00001960: 2020 2020 2020 2020 2020 2020 2073 656e               sen
-00001970: 645f 7265 7175 6573 7428 636f 6d70 6f6e  d_request(compon
-00001980: 656e 742c 207b 0d0a 2020 2020 2020 2020  ent, {..        
+00001930: 2020 2063 6f6d 706f 6e65 6e74 732e 666f     components.fo
+00001940: 7245 6163 6828 636f 6d70 6f6e 656e 7420  rEach(component 
+00001950: 3d3e 207b 0d0a 2020 2020 2020 2020 2020  => {..          
+00001960: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00001970: 6e64 5f72 6571 7565 7374 2863 6f6d 706f  nd_request(compo
+00001980: 6e65 6e74 2c20 7b0d 0a20 2020 2020 2020  nent, {..       
 00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019a0: 2020 2020 6d65 7468 6f64 3a20 2265 6d69      method: "emi
-000019b0: 7422 2c0d 0a20 2020 2020 2020 2020 2020  t",..           
+000019a0: 2020 2020 206d 6574 686f 643a 2022 656d       method: "em
+000019b0: 6974 222c 0d0a 2020 2020 2020 2020 2020  it",..          
 000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 2061 7267 733a 2066 696e 616c 5f70 6172   args: final_par
-000019e0: 616d 732c 0d0a 2020 2020 2020 2020 2020  ams,..          
+000019d0: 2020 6172 6773 3a20 6669 6e61 6c5f 7061    args: final_pa
+000019e0: 7261 6d73 2c0d 0a20 2020 2020 2020 2020  rams,..         
 000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a00: 2020 6b77 6172 6773 3a20 6b77 6172 6773    kwargs: kwargs
-00001a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001a20: 2020 2020 2020 2020 2020 7d2c 2074 6172            }, tar
-00001a30: 6765 7429 2e74 6865 6e28 2829 203d 3e20  get).then(() => 
-00001a40: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00001a50: 2020 2020 2020 2020 2020 2020 2020 202f                 /
-00001a60: 2f20 5570 6461 7465 2044 4f4d 2073 796e  / Update DOM syn
-00001a70: 6368 726f 6e6f 7573 6c79 2061 6674 6572  chronously after
-00001a80: 2065 6d69 7474 696e 6720 6576 656e 7473   emitting events
-00001a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 7570                up
-00001ab0: 6461 7465 5f64 6f6d 2863 6f6d 706f 6e65  date_dom(compone
-00001ac0: 6e74 2c20 636f 6d70 6f6e 656e 742e 696e  nt, component.in
-00001ad0: 6e65 7248 544d 4c29 3b0d 0a20 2020 2020  nerHTML);..     
+00001a00: 2020 206b 7761 7267 733a 206b 7761 7267     kwargs: kwarg
+00001a10: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00001a20: 2020 2020 2020 2020 2020 207d 2c20 7461             }, ta
+00001a30: 7267 6574 292e 7468 656e 2828 2920 3d3e  rget).then(() =>
+00001a40: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2f2f 2055 7064 6174 6520 444f 4d20 7379  // Update DOM sy
+00001a70: 6e63 6872 6f6e 6f75 736c 7920 6166 7465  nchronously afte
+00001a80: 7220 656d 6974 7469 6e67 2065 7665 6e74  r emitting event
+00001a90: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00001aa0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00001ab0: 7064 6174 655f 646f 6d28 636f 6d70 6f6e  pdate_dom(compon
+00001ac0: 656e 742c 2063 6f6d 706f 6e65 6e74 2e69  ent, component.i
+00001ad0: 6e6e 6572 4854 4d4c 293b 0d0a 2020 2020  nnerHTML);..    
 00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001af0: 2020 207d 293b 0d0a 2020 2020 2020 2020     });..        
-00001b00: 2020 2020 2020 2020 2020 2020 7d29 0d0a              })..
-00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 7d0d 0a0d 0a20 2020 2020 2020 2020 2020  }....           
-00001b30: 207d 290d 0a20 2020 2020 2020 207d 0d0a   })..        }..
-00001b40: 0d0a 2020 2020 2020 2020 2f2f 206c 6f6f  ..        // loo
-00001b50: 7020 7468 726f 7567 6820 656c 2e5f 5f6c  p through el.__l
-00001b60: 6976 6566 6c61 736b 2e64 6174 612e 7572  iveflask.data.ur
-00001b70: 6c20 616e 6420 7570 6461 7465 2074 6865  l and update the
-00001b80: 2070 6167 6520 7572 6c20 7769 7468 2074   page url with t
-00001b90: 6865 206e 6577 2075 726c 0d0a 2020 2020  he new url..    
-00001ba0: 2020 2020 6c65 7420 7572 6c5f 6f62 6a65      let url_obje
-00001bb0: 6374 203d 2065 6c2e 5f5f 6c69 7665 666c  ct = el.__livefl
-00001bc0: 6173 6b3f 2e64 6174 613f 2e75 726c 3b0d  ask?.data?.url;.
-00001bd0: 0a20 2020 2020 2020 202f 2f20 7572 6c5f  .        // url_
-00001be0: 6f62 6a65 6374 2069 7320 6120 6b65 792d  object is a key-
-00001bf0: 7661 6c75 6520 7061 6972 206f 626a 6563  value pair objec
-00001c00: 7420 7769 7468 206b 6579 2061 7320 7468  t with key as th
-00001c10: 6520 7175 6572 7920 7061 7261 6d65 7465  e query paramete
-00001c20: 7220 616e 6420 7661 6c75 6520 6173 2074  r and value as t
-00001c30: 6865 2076 616c 7565 0d0a 2020 2020 2020  he value..      
-00001c40: 2020 6966 2028 7572 6c5f 6f62 6a65 6374    if (url_object
-00001c50: 2021 3d3d 2075 6e64 6566 696e 6564 2920   !== undefined) 
-00001c60: 7b0d 0a20 2020 2020 2020 2020 2020 206c  {..            l
-00001c70: 6574 2075 726c 203d 206e 6577 2055 524c  et url = new URL
-00001c80: 2877 696e 646f 772e 6c6f 6361 7469 6f6e  (window.location
-00001c90: 2e68 7265 6629 3b0d 0a20 2020 2020 2020  .href);..       
-00001ca0: 2020 2020 204f 626a 6563 742e 6b65 7973       Object.keys
-00001cb0: 2875 726c 5f6f 626a 6563 7429 2e66 6f72  (url_object).for
-00001cc0: 4561 6368 286b 6579 203d 3e20 7b0d 0a20  Each(key => {.. 
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00001ce0: 726c 2e73 6561 7263 6850 6172 616d 732e  rl.searchParams.
-00001cf0: 7365 7428 6b65 792c 2075 726c 5f6f 626a  set(key, url_obj
-00001d00: 6563 745b 6b65 795d 293b 0d0a 2020 2020  ect[key]);..    
-00001d10: 2020 2020 2020 2020 7d29 3b0d 0a20 2020          });..   
-00001d20: 2020 2020 2020 2020 2077 696e 646f 772e           window.
-00001d30: 6869 7374 6f72 792e 7075 7368 5374 6174  history.pushStat
-00001d40: 6528 7b7d 2c20 2727 2c20 7572 6c29 3b0d  e({}, '', url);.
-00001d50: 0a20 2020 2020 2020 207d 0d0a 0d0a 2020  .        }....  
-00001d60: 2020 7d29 2e74 6865 6e28 656c 203d 3e20    }).then(el => 
-00001d70: 7b0d 0a0d 0a0d 0a20 2020 207d 290d 0a7d  {......    })..}
-00001d80: 0d0a 0d0a 0d0a 6675 6e63 7469 6f6e 2075  ......function u
-00001d90: 7064 6174 655f 646f 6d28 656c 2c20 6874  pdate_dom(el, ht
-00001da0: 6d6c 2920 7b0d 0a20 2020 206c 6574 2063  ml) {..    let c
-00001db0: 6c61 7373 5f6e 616d 6520 3d20 656c 2e5f  lass_name = el._
-00001dc0: 5f6c 6976 6566 6c61 736b 5b27 636c 6173  _liveflask['clas
-00001dd0: 7327 5d0d 0a20 2020 2068 746d 6c20 3d20  s']..    html = 
-00001de0: 603c 6469 7620 6461 7461 2d63 6f6d 706f  `<div data-compo
-00001df0: 6e65 6e74 3d22 247b 636c 6173 735f 6e61  nent="${class_na
-00001e00: 6d65 7d22 2069 643d 2224 7b65 6c2e 6964  me}" id="${el.id
-00001e10: 7d22 3e24 7b68 746d 6c7d 3c2f 6469 763e  }">${html}</div>
-00001e20: 600d 0a20 2020 206d 6f72 7068 646f 6d28  `..    morphdom(
-00001e30: 656c 2c20 6874 6d6c 2c20 7b0d 0a20 2020  el, html, {..   
-00001e40: 2020 2020 206f 6e42 6566 6f72 6545 6c55       onBeforeElU
-00001e50: 7064 6174 6564 3a20 6675 6e63 7469 6f6e  pdated: function
-00001e60: 2028 6672 6f6d 456c 2c20 746f 456c 2920   (fromEl, toEl) 
-00001e70: 7b0d 0a20 2020 2020 2020 2020 2020 202f  {..            /
-00001e80: 2f20 7370 6563 202d 2068 7474 7073 3a2f  / spec - https:/
-00001e90: 2f64 6f6d 2e73 7065 632e 7768 6174 7767  /dom.spec.whatwg
-00001ea0: 2e6f 7267 2f23 636f 6e63 6570 742d 6e6f  .org/#concept-no
-00001eb0: 6465 2d65 7175 616c 730d 0a20 2020 2020  de-equals..     
-00001ec0: 2020 2020 2020 2069 6620 2866 726f 6d45         if (fromE
-00001ed0: 6c2e 6973 4571 7561 6c4e 6f64 6528 746f  l.isEqualNode(to
-00001ee0: 456c 2929 207b 0d0a 2020 2020 2020 2020  El)) {..        
-00001ef0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00001f00: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
-00001f10: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
-00001f20: 2072 6574 7572 6e20 7472 7565 0d0a 2020   return true..  
-00001f30: 2020 2020 2020 7d2c 0d0a 0d0a 2020 2020        },....    
-00001f40: 2020 2020 6f6e 456c 5570 6461 7465 643a      onElUpdated:
-00001f50: 2066 756e 6374 696f 6e20 2865 6c65 6d65   function (eleme
-00001f60: 6e74 2920 7b0d 0a20 2020 2020 2020 2020  nt) {..         
-00001f70: 2020 2069 6620 2865 6c2e 5f5f 6c69 7665     if (el.__live
-00001f80: 666c 6173 6b5b 2763 6869 6c64 7265 6e27  flask['children'
-00001f90: 5d2e 6c65 6e67 7468 2021 3d3d 2030 2920  ].length !== 0) 
-00001fa0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00001fb0: 2020 2075 7064 6174 655f 6368 696c 6472     update_childr
-00001fc0: 656e 2865 6c2e 5f5f 6c69 7665 666c 6173  en(el.__liveflas
-00001fd0: 6b5b 2763 6869 6c64 7265 6e27 5d29 0d0a  k['children'])..
-00001fe0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00001ff0: 2020 2020 2020 207d 2c0d 0a0d 0a20 2020         },....   
-00002000: 207d 293b 0d0a 0d0a 2020 2020 696e 6974   });....    init
-00002010: 5f61 6374 696f 6e28 656c 290d 0a7d 0d0a  _action(el)..}..
-00002020: 0d0a 0d0a 6675 6e63 7469 6f6e 2075 7064  ....function upd
-00002030: 6174 655f 6368 696c 6472 656e 2863 6869  ate_children(chi
-00002040: 6c64 7265 6e20 3d20 5b5d 2920 7b0d 0a20  ldren = []) {.. 
-00002050: 2020 206c 6574 206d 6174 6368 6564 5f63     let matched_c
-00002060: 6f6d 706f 6e65 6e74 3b0d 0a20 2020 2063  omponent;..    c
-00002070: 6869 6c64 7265 6e2e 666f 7245 6163 6828  hildren.forEach(
-00002080: 6920 3d3e 207b 0d0a 2020 2020 2020 2020  i => {..        
-00002090: 6d61 7463 6865 645f 636f 6d70 6f6e 656e  matched_componen
-000020a0: 7420 3d20 646f 6375 6d65 6e74 2e67 6574  t = document.get
-000020b0: 456c 656d 656e 7442 7949 6428 6024 7b69  ElementById(`${i
-000020c0: 2e5f 5f6c 6976 6566 6c61 736b 5b27 6b65  .__liveflask['ke
-000020d0: 7927 5d7d 6029 3b0d 0a20 2020 2020 2020  y']}`);..       
-000020e0: 206d 6f72 7068 646f 6d28 6d61 7463 6865   morphdom(matche
-000020f0: 645f 636f 6d70 6f6e 656e 742c 2069 2e6f  d_component, i.o
-00002100: 7574 6572 4854 4d4c 290d 0a20 2020 207d  uterHTML)..    }
-00002110: 290d 0a7d 0d0a 0d0a 0d0a                 )..}......
+00001af0: 2020 2020 7d29 3b0d 0a20 2020 2020 2020      });..       
+00001b00: 2020 2020 2020 2020 2020 2020 207d 290d               }).
+00001b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b20: 207d 0d0a 0d0a 2020 2020 2020 2020 2020   }....          
+00001b30: 2020 7d29 0d0a 2020 2020 2020 2020 7d0d    })..        }.
+00001b40: 0a0d 0a20 2020 2020 2020 202f 2f20 6c6f  ...        // lo
+00001b50: 6f70 2074 6872 6f75 6768 2065 6c2e 5f5f  op through el.__
+00001b60: 6c69 7665 666c 6173 6b2e 6461 7461 2e75  liveflask.data.u
+00001b70: 726c 2061 6e64 2075 7064 6174 6520 7468  rl and update th
+00001b80: 6520 7061 6765 2075 726c 2077 6974 6820  e page url with 
+00001b90: 7468 6520 6e65 7720 7572 6c0d 0a20 2020  the new url..   
+00001ba0: 2020 2020 206c 6574 2075 726c 5f6f 626a       let url_obj
+00001bb0: 6563 7420 3d20 656c 2e5f 5f6c 6976 6566  ect = el.__livef
+00001bc0: 6c61 736b 3f2e 6461 7461 3f2e 7572 6c3b  lask?.data?.url;
+00001bd0: 0d0a 2020 2020 2020 2020 2f2f 2075 726c  ..        // url
+00001be0: 5f6f 626a 6563 7420 6973 2061 206b 6579  _object is a key
+00001bf0: 2d76 616c 7565 2070 6169 7220 6f62 6a65  -value pair obje
+00001c00: 6374 2077 6974 6820 6b65 7920 6173 2074  ct with key as t
+00001c10: 6865 2071 7565 7279 2070 6172 616d 6574  he query paramet
+00001c20: 6572 2061 6e64 2076 616c 7565 2061 7320  er and value as 
+00001c30: 7468 6520 7661 6c75 650d 0a20 2020 2020  the value..     
+00001c40: 2020 2069 6620 2875 726c 5f6f 626a 6563     if (url_objec
+00001c50: 7420 213d 3d20 756e 6465 6669 6e65 6429  t !== undefined)
+00001c60: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00001c70: 6c65 7420 7572 6c20 3d20 6e65 7720 5552  let url = new UR
+00001c80: 4c28 7769 6e64 6f77 2e6c 6f63 6174 696f  L(window.locatio
+00001c90: 6e2e 6872 6566 293b 0d0a 2020 2020 2020  n.href);..      
+00001ca0: 2020 2020 2020 4f62 6a65 6374 2e6b 6579        Object.key
+00001cb0: 7328 7572 6c5f 6f62 6a65 6374 292e 666f  s(url_object).fo
+00001cc0: 7245 6163 6828 6b65 7920 3d3e 207b 0d0a  rEach(key => {..
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ce0: 7572 6c2e 7365 6172 6368 5061 7261 6d73  url.searchParams
+00001cf0: 2e73 6574 286b 6579 2c20 7572 6c5f 6f62  .set(key, url_ob
+00001d00: 6a65 6374 5b6b 6579 5d29 3b0d 0a20 2020  ject[key]);..   
+00001d10: 2020 2020 2020 2020 207d 293b 0d0a 2020           });..  
+00001d20: 2020 2020 2020 2020 2020 7769 6e64 6f77            window
+00001d30: 2e68 6973 746f 7279 2e70 7573 6853 7461  .history.pushSta
+00001d40: 7465 287b 7d2c 2027 272c 2075 726c 293b  te({}, '', url);
+00001d50: 0d0a 2020 2020 2020 2020 7d0d 0a0d 0a20  ..        }.... 
+00001d60: 2020 207d 292e 7468 656e 2865 6c20 3d3e     }).then(el =>
+00001d70: 207b 0d0a 0d0a 0d0a 2020 2020 7d29 0d0a   {......    })..
+00001d80: 7d0d 0a0d 0a0d 0a66 756e 6374 696f 6e20  }......function 
+00001d90: 7570 6461 7465 5f64 6f6d 2865 6c2c 2068  update_dom(el, h
+00001da0: 746d 6c29 207b 0d0a 2020 2020 6c65 7420  tml) {..    let 
+00001db0: 636c 6173 735f 6e61 6d65 203d 2065 6c2e  class_name = el.
+00001dc0: 5f5f 6c69 7665 666c 6173 6b5b 2763 6c61  __liveflask['cla
+00001dd0: 7373 275d 0d0a 2020 2020 6874 6d6c 203d  ss']..    html =
+00001de0: 2060 3c64 6976 2064 6174 612d 636f 6d70   `<div data-comp
+00001df0: 6f6e 656e 743d 2224 7b63 6c61 7373 5f6e  onent="${class_n
+00001e00: 616d 657d 2220 6964 3d22 247b 656c 2e69  ame}" id="${el.i
+00001e10: 647d 223e 247b 6874 6d6c 7d3c 2f64 6976  d}">${html}</div
+00001e20: 3e60 0d0a 2020 2020 6d6f 7270 6864 6f6d  >`..    morphdom
+00001e30: 2865 6c2c 2068 746d 6c2c 207b 0d0a 2020  (el, html, {..  
+00001e40: 2020 2020 2020 6f6e 4265 666f 7265 456c        onBeforeEl
+00001e50: 5570 6461 7465 643a 2066 756e 6374 696f  Updated: functio
+00001e60: 6e20 2866 726f 6d45 6c2c 2074 6f45 6c29  n (fromEl, toEl)
+00001e70: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00001e80: 2f2f 2073 7065 6320 2d20 6874 7470 733a  // spec - https:
+00001e90: 2f2f 646f 6d2e 7370 6563 2e77 6861 7477  //dom.spec.whatw
+00001ea0: 672e 6f72 672f 2363 6f6e 6365 7074 2d6e  g.org/#concept-n
+00001eb0: 6f64 652d 6571 7561 6c73 0d0a 2020 2020  ode-equals..    
+00001ec0: 2020 2020 2020 2020 6966 2028 6672 6f6d          if (from
+00001ed0: 456c 2e69 7345 7175 616c 4e6f 6465 2874  El.isEqualNode(t
+00001ee0: 6f45 6c29 2920 7b0d 0a20 2020 2020 2020  oEl)) {..       
+00001ef0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001f00: 6661 6c73 650d 0a20 2020 2020 2020 2020  false..         
+00001f10: 2020 207d 0d0a 2020 2020 2020 2020 2020     }..          
+00001f20: 2020 7265 7475 726e 2074 7275 650d 0a20    return true.. 
+00001f30: 2020 2020 2020 207d 2c0d 0a0d 0a20 2020         },....   
+00001f40: 2020 2020 206f 6e45 6c55 7064 6174 6564       onElUpdated
+00001f50: 3a20 6675 6e63 7469 6f6e 2028 656c 656d  : function (elem
+00001f60: 656e 7429 207b 0d0a 2020 2020 2020 2020  ent) {..        
+00001f70: 2020 2020 6966 2028 656c 2e5f 5f6c 6976      if (el.__liv
+00001f80: 6566 6c61 736b 5b27 6368 696c 6472 656e  eflask['children
+00001f90: 275d 2e6c 656e 6774 6820 213d 3d20 3029  '].length !== 0)
+00001fa0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00001fb0: 2020 2020 7570 6461 7465 5f63 6869 6c64      update_child
+00001fc0: 7265 6e28 656c 2e5f 5f6c 6976 6566 6c61  ren(el.__livefla
+00001fd0: 736b 5b27 6368 696c 6472 656e 275d 290d  sk['children']).
+00001fe0: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
+00001ff0: 2020 2020 2020 2020 7d2c 0d0a 0d0a 2020          },....  
+00002000: 2020 7d29 3b0d 0a0d 0a20 2020 2069 6e69    });....    ini
+00002010: 745f 6163 7469 6f6e 2865 6c29 0d0a 7d0d  t_action(el)..}.
+00002020: 0a0d 0a0d 0a66 756e 6374 696f 6e20 7570  .....function up
+00002030: 6461 7465 5f63 6869 6c64 7265 6e28 6368  date_children(ch
+00002040: 696c 6472 656e 203d 205b 5d29 207b 0d0a  ildren = []) {..
+00002050: 2020 2020 6c65 7420 6d61 7463 6865 645f      let matched_
+00002060: 636f 6d70 6f6e 656e 743b 0d0a 2020 2020  component;..    
+00002070: 6368 696c 6472 656e 2e66 6f72 4561 6368  children.forEach
+00002080: 2869 203d 3e20 7b0d 0a20 2020 2020 2020  (i => {..       
+00002090: 206d 6174 6368 6564 5f63 6f6d 706f 6e65   matched_compone
+000020a0: 6e74 203d 2064 6f63 756d 656e 742e 6765  nt = document.ge
+000020b0: 7445 6c65 6d65 6e74 4279 4964 2860 247b  tElementById(`${
+000020c0: 692e 5f5f 6c69 7665 666c 6173 6b5b 276b  i.__liveflask['k
+000020d0: 6579 275d 7d60 293b 0d0a 2020 2020 2020  ey']}`);..      
+000020e0: 2020 6d6f 7270 6864 6f6d 286d 6174 6368    morphdom(match
+000020f0: 6564 5f63 6f6d 706f 6e65 6e74 2c20 692e  ed_component, i.
+00002100: 6f75 7465 7248 544d 4c29 0d0a 2020 2020  outerHTML)..    
+00002110: 7d29 0d0a 7d0d 0a0d 0a0d 0a              })..}......
```

### Comparing `liveflask-1.0.6/liveflask/static/lodash.min.js` & `liveflask-1.0.7/liveflask/static/lodash.min.js`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask/traits/__pycache__/Bootable.cpython-311.pyc` & `liveflask-1.0.7/liveflask/traits/__pycache__/Bootable.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
+moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
 files sz: 205
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.6/liveflask/traits/__pycache__/has_actions.cpython-311.pyc` & `liveflask-1.0.7/liveflask/traits/__pycache__/has_actions.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
+moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
 files sz: 2042
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.6/liveflask/traits/__pycache__/has_props.cpython-311.pyc` & `liveflask-1.0.7/liveflask/traits/__pycache__/has_props.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
+moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
 files sz: 2488
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.6/liveflask/traits/__pycache__/has_renders.cpython-311.pyc` & `liveflask-1.0.7/liveflask/traits/__pycache__/has_renders.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
+moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
 files sz: 2486
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.6/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc` & `liveflask-1.0.7/liveflask/traits/__pycache__/has_snapshots.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xfea73266 (Wed May  1 20:37:18 2024 UTC)
+moddate:  0xfdae3266 (Wed May  1 21:07:09 2024 UTC)
 files sz: 4106
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `liveflask-1.0.6/liveflask/traits/has_actions.py` & `liveflask-1.0.7/liveflask/traits/has_actions.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask/traits/has_props.py` & `liveflask-1.0.7/liveflask/traits/has_props.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask/traits/has_renders.py` & `liveflask-1.0.7/liveflask/traits/has_renders.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask/traits/has_snapshots.py` & `liveflask-1.0.7/liveflask/traits/has_snapshots.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask/utils.py` & `liveflask-1.0.7/liveflask/utils.py`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/liveflask.egg-info/PKG-INFO` & `liveflask-1.0.7/liveflask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveflask
-Version: 1.0.6
+Version: 1.0.7
 Summary: Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.
 Home-page: https://github.com/JarriqTheTechie/liveflask
 Author: Jarriq Rolle
 Author-email: jrolle@baysidetechgroup.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `liveflask-1.0.6/liveflask.egg-info/SOURCES.txt` & `liveflask-1.0.7/liveflask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveflask-1.0.6/setup.py` & `liveflask-1.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme_pypi.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="liveflask",
-    version="1.0.6",
+    version="1.0.7",
     author="Jarriq Rolle",
     author_email="jrolle@baysidetechgroup.com",
     description="Seamlessly integrate modern reactive components into Flask templates, eliminating the need for mastering new templating languages or wrestling with complex JavaScript frameworks. With our solution, developers can enhance their Flask applications with dynamic functionality while maintaining a familiar development environment, streamlining the process and ensuring a smoother user experience.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JarriqTheTechie/liveflask",
     packages=['liveflask'],
```

