# Comparing `tmp/wpp_whatsapp-0.2.2.2.tar.gz` & `tmp/wpp_whatsapp-0.2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpp_whatsapp-0.2.2.2.tar", last modified: Sat Apr 27 03:18:31 2024, max compression
+gzip compressed data, was "wpp_whatsapp-0.2.2.3.tar", last modified: Sun May  5 18:41:01 2024, max compression
```

## Comparing `wpp_whatsapp-0.2.2.2.tar` & `wpp_whatsapp-0.2.2.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.274876 wpp_whatsapp-0.2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-27 03:18:31.274876 wpp_whatsapp-0.2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.266876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.266876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/Whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.266876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/download_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/jsFunction.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/scrap-img.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/wa_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/BusinessLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/CatalogLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ControlsLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/GroupLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/HostLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/LabelsLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ListenerLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ProfileLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13361 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/RetrieverLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/SenderLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/StatusLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/UILayer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/model/status_find.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/init_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/js_lib/
--rw-r--r--   0 runner    (1001) docker     (127)    89768 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/js_lib/wapi.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp/utils/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-27 03:18:31.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-27 03:18:31.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 03:18:31.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-27 03:18:31.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-27 03:18:31.000000 wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 03:18:31.274876 wpp_whatsapp-0.2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 03:18:31.270876 wpp_whatsapp-0.2.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/test/test_hiden.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-27 03:18:27.000000 wpp_whatsapp-0.2.2.2/test/test_setinterval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.175731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.175731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/Whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.175731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/download_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/jsFunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/scrap-img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/wa_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/BusinessLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/CatalogLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ControlsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/GroupLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/HostLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/LabelsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12529 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ListenerLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ProfileLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13361 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/RetrieverLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19632 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/SenderLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/StatusLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/UILayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/model/status_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/init_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10304 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/js_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    89768 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/js_lib/wapi.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp/utils/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-05 18:41:01.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-05 18:41:01.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:41:01.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 18:41:01.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 18:41:01.000000 wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:41:01.179731 wpp_whatsapp-0.2.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/test/test_hiden.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-05 18:40:57.000000 wpp_whatsapp-0.2.2.3/test/test_setinterval.py
```

### Comparing `wpp_whatsapp-0.2.2.2/LICENSE` & `wpp_whatsapp-0.2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/PKG-INFO` & `wpp_whatsapp-0.2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPP_Whatsapp
-Version: 0.2.2.2
+Version: 0.2.2.3
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wpp_whatsapp-0.2.2.2/README.md` & `wpp_whatsapp-0.2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/Whatsapp.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/Whatsapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.options = {}
         self.options.update(defaultOptions)
         for key, value in kwargs.items():
             if key in self.options:
                 self.options[key] = value
 
         # self.autoCloseInterval = None
-        self.version = version or self.options.get('whatsappVersion')
+        self.version = version # or self.options.get('whatsappVersion')
         self.wa_js_version = wa_js_version
         self.autoCloseCalled = False
         self.isInitialized = False
         self.isInjected = False
         self.isStarted = False
         self.isLogged = False
         self.isInChat = False
```

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/const.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/const.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/decorators.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/download_file.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/download_file.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/jsFunction.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/jsFunction.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/helpers/wa_version.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/helpers/wa_version.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/CatalogLayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/CatalogLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ControlsLayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ControlsLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/GroupLayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/GroupLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/HostLayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/HostLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/LabelsLayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/LabelsLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ListenerLayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ListenerLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from event_emitter import EventEmitter
+from playwright.async_api import Error
+
 from WPP_Whatsapp.api.layers.ProfileLayer import ProfileLayer
 
 OnMessage = 'onMessage'
 OnAnyMessage = 'onAnyMessage'
 onAck = 'onAck'
 onNotificationMessage = 'onNotificationMessage'
 onParticipantsChanged = 'onParticipantsChanged'
@@ -62,19 +64,24 @@
             'onIncomingCall',
             'onRevokedMessage',
             'onReactionMessage',
             'onPollResponse'
         ]
 
         for func in functions:
-            has = await self.ThreadsafeBrowser.page_evaluate("(func) => typeof window[func] === 'function'", func, page=self.page)
+            has = await self.ThreadsafeBrowser.page_evaluate("(func) => typeof window[func] === 'function'", func,
+                                                             page=self.page)
             if not has:
                 self.logger.debug(f'{self.session}: Exposing {func} function')
                 handel_func = HandelFunc(func, self.session, self.logger, self.__listenerEmitter).handel_func
-                await self.ThreadsafeBrowser.expose_function(func, handel_func, page=self.page)
+                try:
+                    await self.ThreadsafeBrowser.expose_function(func, handel_func, page=self.page)
+                except Error as e:
+                    if "has been already registered" not in e.message:
+                        raise e
 
         await self.ThreadsafeBrowser.page_evaluate("""() => {
         try {
           if (!window['onMessage'].exposed) {
             WPP.on('chat.new_message', (msg) => {
               if (msg.isSentByMe || msg.isStatusV3) {
                 return;
```

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/ProfileLayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/ProfileLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/RetrieverLayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/RetrieverLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/SenderLayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/SenderLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/StatusLayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/StatusLayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/layers/UILayer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/layers/UILayer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/api/model/status_find.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/api/model/status_find.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/browser.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/browser.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/init_multi.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/init_multi.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/controllers/initializer.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/controllers/initializer.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/js_lib/wapi.js` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/js_lib/wapi.js`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp/utils/ffmpeg.py` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/PKG-INFO` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPP_Whatsapp
-Version: 0.2.2.2
+Version: 0.2.2.3
 Summary: WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination
 Home-page: https://github.com/3mora2/WPP_Whatsapp
 Author: Ammar Alkotb
 Author-email: ammar.alkotb@gmail.com
 License: MIT License
 Project-URL: Bug Report, https://github.com/3mora2/WPP_Whatsapp/issues/new
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wpp_whatsapp-0.2.2.2/WPP_Whatsapp.egg-info/SOURCES.txt` & `wpp_whatsapp-0.2.2.3/WPP_Whatsapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/setup.py` & `wpp_whatsapp-0.2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 long_description = open("README.md", encoding="utf-8").read()
 description = ("WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support "
                "the creation of any interaction, such as customer service, media sending, intelligence recognition "
                "based on phrases artificial and many other things, use your imagination")
 
-version = "0.2.2.2"
+version = "0.2.2.3"
 
 setup(
     name="WPP_Whatsapp",
     version=version,
     license="MIT License",
     author="Ammar Alkotb",
     author_email="ammar.alkotb@gmail.com",
```

### Comparing `wpp_whatsapp-0.2.2.2/test/test_hiden.py` & `wpp_whatsapp-0.2.2.3/test/test_hiden.py`

 * *Files identical despite different names*

### Comparing `wpp_whatsapp-0.2.2.2/test/test_setinterval.py` & `wpp_whatsapp-0.2.2.3/test/test_setinterval.py`

 * *Files identical despite different names*

