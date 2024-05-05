# Comparing `tmp/offlinesec_client-1.1.0.tar.gz` & `tmp/offlinesec_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offlinesec_client-1.1.0.tar", last modified: Fri May  3 11:33:42 2024, max compression
+gzip compressed data, was "offlinesec_client-1.1.1.tar", last modified: Sat May  4 07:12:16 2024, max compression
```

## Comparing `offlinesec_client-1.1.0.tar` & `offlinesec_client-1.1.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 11:33:42.139343 offlinesec_client-1.1.0/
--rw-rw-rw-   0        0        0     6793 2024-05-03 11:33:42.138278 offlinesec_client-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6499 2024-05-03 06:54:42.000000 offlinesec_client-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 11:33:42.130898 offlinesec_client-1.1.0/offlinesec_client/
--rw-rw-rw-   0        0        0       23 2024-05-03 05:48:17.000000 offlinesec_client-1.1.0/offlinesec_client/__init__.py
--rw-rw-rw-   0        0        0      110 2023-07-14 20:07:51.000000 offlinesec_client-1.1.0/offlinesec_client/__main__.py
--rw-rw-rw-   0        0        0     4252 2024-05-03 05:48:17.000000 offlinesec_client-1.1.0/offlinesec_client/abap_system.py
--rw-rw-rw-   0        0        0     4080 2023-10-03 17:05:46.000000 offlinesec_client-1.1.0/offlinesec_client/agr_1251.py
--rw-rw-rw-   0        0        0     1255 2024-05-03 05:48:17.000000 offlinesec_client-1.1.0/offlinesec_client/bo_system.py
--rw-rw-rw-   0        0        0     2893 2023-09-14 14:17:57.000000 offlinesec_client-1.1.0/offlinesec_client/config.py
--rw-rw-rw-   0        0        0      577 2023-09-17 12:59:15.000000 offlinesec_client-1.1.0/offlinesec_client/const.py
--rw-rw-rw-   0        0        0     1594 2023-10-10 16:14:36.000000 offlinesec_client-1.1.0/offlinesec_client/cwbntcust.py
--rw-rw-rw-   0        0        0     4342 2023-12-03 15:32:46.000000 offlinesec_client-1.1.0/offlinesec_client/func.py
--rw-rw-rw-   0        0        0     3435 2023-08-21 06:40:25.000000 offlinesec_client-1.1.0/offlinesec_client/get_reports.py
--rw-rw-rw-   0        0        0     2235 2024-05-03 05:48:17.000000 offlinesec_client-1.1.0/offlinesec_client/java_system.py
--rw-rw-rw-   0        0        0     1847 2024-04-07 08:20:55.000000 offlinesec_client-1.1.0/offlinesec_client/multi_systems.py
--rw-rw-rw-   0        0        0     4118 2023-10-21 13:22:58.000000 offlinesec_client-1.1.0/offlinesec_client/req_bo_notes.py
--rw-rw-rw-   0        0        0     4642 2023-11-17 19:46:10.000000 offlinesec_client-1.1.0/offlinesec_client/req_java_notes.py
--rw-rw-rw-   0        0        0     4601 2023-10-14 08:09:41.000000 offlinesec_client-1.1.0/offlinesec_client/req_notes_report.py
--rw-rw-rw-   0        0        0     4652 2023-07-15 08:41:30.000000 offlinesec_client-1.1.0/offlinesec_client/req_param_report.py
--rw-rw-rw-   0        0        0     1926 2024-04-28 06:12:18.000000 offlinesec_client-1.1.0/offlinesec_client/req_patch_day.py
--rw-rw-rw-   0        0        0     4060 2023-10-03 20:26:25.000000 offlinesec_client-1.1.0/offlinesec_client/req_roles_report.py
--rw-rw-rw-   0        0        0     1885 2024-04-28 06:33:53.000000 offlinesec_client-1.1.0/offlinesec_client/req_sec_notes.py
--rw-rw-rw-   0        0        0     2499 2023-08-21 12:55:22.000000 offlinesec_client-1.1.0/offlinesec_client/resolve_report.py
--rw-rw-rw-   0        0        0     5092 2024-03-10 09:46:08.000000 offlinesec_client-1.1.0/offlinesec_client/rsparam.py
--rw-rw-rw-   0        0        0     5028 2023-09-19 06:24:24.000000 offlinesec_client-1.1.0/offlinesec_client/sap_gui.py
--rw-rw-rw-   0        0        0     2931 2023-11-19 10:07:16.000000 offlinesec_client-1.1.0/offlinesec_client/sap_system.py
-drwxrwxrwx   0        0        0        0 2024-05-03 11:33:42.137245 offlinesec_client-1.1.0/offlinesec_client.egg-info/
--rw-rw-rw-   0        0        0     6793 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      578 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 11:33:42.139343 offlinesec_client-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1620 2024-05-03 05:48:17.000000 offlinesec_client-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:12:16.080564 offlinesec_client-1.1.1/
+-rw-rw-rw-   0        0        0     6793 2024-05-04 07:12:16.079533 offlinesec_client-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6499 2024-05-03 06:54:42.000000 offlinesec_client-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 07:12:16.072218 offlinesec_client-1.1.1/offlinesec_client/
+-rw-rw-rw-   0        0        0       23 2024-05-04 07:11:02.000000 offlinesec_client-1.1.1/offlinesec_client/__init__.py
+-rw-rw-rw-   0        0        0      110 2023-07-14 20:07:51.000000 offlinesec_client-1.1.1/offlinesec_client/__main__.py
+-rw-rw-rw-   0        0        0     4252 2024-05-03 05:48:17.000000 offlinesec_client-1.1.1/offlinesec_client/abap_system.py
+-rw-rw-rw-   0        0        0     4080 2023-10-03 17:05:46.000000 offlinesec_client-1.1.1/offlinesec_client/agr_1251.py
+-rw-rw-rw-   0        0        0     1852 2024-05-04 07:05:36.000000 offlinesec_client-1.1.1/offlinesec_client/api_sec_notes.py
+-rw-rw-rw-   0        0        0     1255 2024-05-03 05:48:17.000000 offlinesec_client-1.1.1/offlinesec_client/bo_system.py
+-rw-rw-rw-   0        0        0     2893 2023-09-14 14:17:57.000000 offlinesec_client-1.1.1/offlinesec_client/config.py
+-rw-rw-rw-   0        0        0      577 2023-09-17 12:59:15.000000 offlinesec_client-1.1.1/offlinesec_client/const.py
+-rw-rw-rw-   0        0        0     1594 2023-10-10 16:14:36.000000 offlinesec_client-1.1.1/offlinesec_client/cwbntcust.py
+-rw-rw-rw-   0        0        0     4342 2023-12-03 15:32:46.000000 offlinesec_client-1.1.1/offlinesec_client/func.py
+-rw-rw-rw-   0        0        0     3435 2023-08-21 06:40:25.000000 offlinesec_client-1.1.1/offlinesec_client/get_reports.py
+-rw-rw-rw-   0        0        0     2235 2024-05-03 05:48:17.000000 offlinesec_client-1.1.1/offlinesec_client/java_system.py
+-rw-rw-rw-   0        0        0     1847 2024-04-07 08:20:55.000000 offlinesec_client-1.1.1/offlinesec_client/multi_systems.py
+-rw-rw-rw-   0        0        0     4118 2023-10-21 13:22:58.000000 offlinesec_client-1.1.1/offlinesec_client/req_bo_notes.py
+-rw-rw-rw-   0        0        0     4642 2023-11-17 19:46:10.000000 offlinesec_client-1.1.1/offlinesec_client/req_java_notes.py
+-rw-rw-rw-   0        0        0     4601 2023-10-14 08:09:41.000000 offlinesec_client-1.1.1/offlinesec_client/req_notes_report.py
+-rw-rw-rw-   0        0        0     4652 2023-07-15 08:41:30.000000 offlinesec_client-1.1.1/offlinesec_client/req_param_report.py
+-rw-rw-rw-   0        0        0     2095 2024-05-04 06:59:30.000000 offlinesec_client-1.1.1/offlinesec_client/req_patch_day.py
+-rw-rw-rw-   0        0        0     4060 2023-10-03 20:26:25.000000 offlinesec_client-1.1.1/offlinesec_client/req_roles_report.py
+-rw-rw-rw-   0        0        0     2054 2024-05-04 06:59:30.000000 offlinesec_client-1.1.1/offlinesec_client/req_sec_notes.py
+-rw-rw-rw-   0        0        0     2502 2024-05-04 07:05:36.000000 offlinesec_client-1.1.1/offlinesec_client/resolve_report.py
+-rw-rw-rw-   0        0        0     5092 2024-03-10 09:46:08.000000 offlinesec_client-1.1.1/offlinesec_client/rsparam.py
+-rw-rw-rw-   0        0        0     5028 2023-09-19 06:24:24.000000 offlinesec_client-1.1.1/offlinesec_client/sap_gui.py
+-rw-rw-rw-   0        0        0     2931 2023-11-19 10:07:16.000000 offlinesec_client-1.1.1/offlinesec_client/sap_system.py
+drwxrwxrwx   0        0        0        0 2024-05-04 07:12:16.078505 offlinesec_client-1.1.1/offlinesec_client.egg-info/
+-rw-rw-rw-   0        0        0     6793 2024-05-04 07:12:15.000000 offlinesec_client-1.1.1/offlinesec_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2024-05-04 07:12:15.000000 offlinesec_client-1.1.1/offlinesec_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 07:12:15.000000 offlinesec_client-1.1.1/offlinesec_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      578 2024-05-04 07:12:15.000000 offlinesec_client-1.1.1/offlinesec_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2024-05-04 07:12:15.000000 offlinesec_client-1.1.1/offlinesec_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-04 07:12:15.000000 offlinesec_client-1.1.1/offlinesec_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 07:12:16.080564 offlinesec_client-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1620 2024-05-03 05:48:17.000000 offlinesec_client-1.1.1/setup.py
```

### Comparing `offlinesec_client-1.1.0/PKG-INFO` & `offlinesec_client-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinesec_client
-Version: 1.1.0
+Version: 1.1.1
 Summary: Offline Security Client
 Home-page: https://offlinesec.com
 Author: Offline Security
 Author-email: info@offlinesec.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `offlinesec_client-1.1.0/README.md` & `offlinesec_client-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/abap_system.py` & `offlinesec_client-1.1.1/offlinesec_client/abap_system.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/agr_1251.py` & `offlinesec_client-1.1.1/offlinesec_client/agr_1251.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/bo_system.py` & `offlinesec_client-1.1.1/offlinesec_client/bo_system.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/config.py` & `offlinesec_client-1.1.1/offlinesec_client/config.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/const.py` & `offlinesec_client-1.1.1/offlinesec_client/const.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/cwbntcust.py` & `offlinesec_client-1.1.1/offlinesec_client/cwbntcust.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/func.py` & `offlinesec_client-1.1.1/offlinesec_client/func.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/get_reports.py` & `offlinesec_client-1.1.1/offlinesec_client/get_reports.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/java_system.py` & `offlinesec_client-1.1.1/offlinesec_client/java_system.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/multi_systems.py` & `offlinesec_client-1.1.1/offlinesec_client/multi_systems.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/req_bo_notes.py` & `offlinesec_client-1.1.1/offlinesec_client/req_bo_notes.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/req_java_notes.py` & `offlinesec_client-1.1.1/offlinesec_client/req_java_notes.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/req_notes_report.py` & `offlinesec_client-1.1.1/offlinesec_client/req_notes_report.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/req_param_report.py` & `offlinesec_client-1.1.1/offlinesec_client/req_param_report.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/req_patch_day.py` & `offlinesec_client-1.1.1/offlinesec_client/req_patch_day.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,28 +21,31 @@
     return res
 
 
 def init_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("-f", "--file", action="store", type=check_file_arg,
                         help="File Name (SAP systems (ABAP, JAVA, BO, ...) and their software components in YAML format)", required=True)
-    parser.add_argument('--wait', action='store_true', help="Wait 5 minutes and download the report")
+    parser.add_argument('-w', '--wait', action='store_true', help="Wait 5 minutes and download the report")
+    parser.add_argument('-i', '--id', action='store', help="The scan Id (any unique identifier)")
     parser.parse_args()
     return vars(parser.parse_args())
 
 
 def print_errors(errors):
     for error in errors:
         print(error)
 
 
 def process_it(args):
     systems = process_yaml_file(args)
     additional_keys = dict()
     additional_keys["patch_day"] = True
+    if args["id"]:
+        additional_keys["id"] = args["id"]
     offlinesec_client.func.send_to_server(systems, UPLOAD_URL, additional_keys)
 
     wait = args["wait"]
     if wait:
         for remaining in range(310, 0, -1):
             sys.stdout.write("\r")
             sys.stdout.write("{:2d} seconds remaining.".format(remaining))
```

### Comparing `offlinesec_client-1.1.0/offlinesec_client/req_roles_report.py` & `offlinesec_client-1.1.1/offlinesec_client/req_roles_report.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/req_sec_notes.py` & `offlinesec_client-1.1.1/offlinesec_client/req_sec_notes.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,27 +21,30 @@
     return res
 
 
 def init_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("-f", "--file", action="store", type=check_file_arg,
                         help="File Name (SAP systems (ABAP, JAVA, BO, ...) and their software components in YAML format)", required=True)
-    parser.add_argument('--wait', action='store_true', help="Wait 5 minutes and download the report")
+    parser.add_argument('-w', '--wait', action='store_true', help="Wait 5 minutes and download the report")
+    parser.add_argument('-i', '--id', action='store', help="The scan Id (any unique identifier)")
     parser.parse_args()
     return vars(parser.parse_args())
 
 
 def print_errors(errors):
     for error in errors:
         print(error)
 
 
 def process_it(args):
     systems = process_yaml_file(args)
     additional_keys = dict()
+    if args["id"]:
+        additional_keys["id"] = args["id"]
     offlinesec_client.func.send_to_server(systems, UPLOAD_URL, additional_keys)
 
     wait = args["wait"]
     if wait:
         for remaining in range(310, 0, -1):
             sys.stdout.write("\r")
             sys.stdout.write("{:2d} seconds remaining.".format(remaining))
```

### Comparing `offlinesec_client-1.1.0/offlinesec_client/resolve_report.py` & `offlinesec_client-1.1.1/offlinesec_client/resolve_report.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 
     if title.startswith("Critical Authorizations"):
         roles = read_dict_file()
         resolve_roles_page1(ws, roles)
         ws = wb.worksheets[1]
         resolve_roles_page2(ws, roles)
 
-        img = openpyxl.drawing.image.Image('logo.jpg')
-        img.anchor = 'A1'
-        ws.add_image(img)
+        #img = openpyxl.drawing.image.Image('logo.jpg')
+        #img.anchor = 'A1'
+        #ws.add_image(img)
 
         wb.save(file)
         print(" * Roles in file %s have been converted" % (os.path.basename(file),))
 
 
 
 def resolve_roles_page1(ws, roles):
```

### Comparing `offlinesec_client-1.1.0/offlinesec_client/rsparam.py` & `offlinesec_client-1.1.1/offlinesec_client/rsparam.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/sap_gui.py` & `offlinesec_client-1.1.1/offlinesec_client/sap_gui.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client/sap_system.py` & `offlinesec_client-1.1.1/offlinesec_client/sap_system.py`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/offlinesec_client.egg-info/PKG-INFO` & `offlinesec_client-1.1.1/offlinesec_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offlinesec-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: Offline Security Client
 Home-page: https://offlinesec.com
 Author: Offline Security
 Author-email: info@offlinesec.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `offlinesec_client-1.1.0/offlinesec_client.egg-info/SOURCES.txt` & `offlinesec_client-1.1.1/offlinesec_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 offlinesec_client/__init__.py
 offlinesec_client/__main__.py
 offlinesec_client/abap_system.py
 offlinesec_client/agr_1251.py
+offlinesec_client/api_sec_notes.py
 offlinesec_client/bo_system.py
 offlinesec_client/config.py
 offlinesec_client/const.py
 offlinesec_client/cwbntcust.py
 offlinesec_client/func.py
 offlinesec_client/get_reports.py
 offlinesec_client/java_system.py
```

### Comparing `offlinesec_client-1.1.0/offlinesec_client.egg-info/entry_points.txt` & `offlinesec_client-1.1.1/offlinesec_client.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `offlinesec_client-1.1.0/setup.py` & `offlinesec_client-1.1.1/setup.py`

 * *Files identical despite different names*

