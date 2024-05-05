# Comparing `tmp/ieugwaspy-1.0.0.tar.gz` & `tmp/ieugwaspy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ieugwaspy-1.0.0.tar", last modified: Fri May  3 12:26:54 2024, max compression
+gzip compressed data, was "ieugwaspy-1.0.2.tar", last modified: Sun May  5 09:28:19 2024, max compression
```

## Comparing `ieugwaspy-1.0.0.tar` & `ieugwaspy-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1453 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/ieugwaspy/
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      728 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/backwards.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1268 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5628 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/query.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/ieugwaspy/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/ieugwaspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-03 12:26:54.000000 ieugwaspy-1.0.0/ieugwaspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-03 12:26:54.000000 ieugwaspy-1.0.0/ieugwaspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 12:26:54.000000 ieugwaspy-1.0.0/ieugwaspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 12:26:54.000000 ieugwaspy-1.0.0/ieugwaspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 12:26:54.000000 ieugwaspy-1.0.0/ieugwaspy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      695 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 12:26:54.567554 ieugwaspy-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-03 12:26:43.000000 ieugwaspy-1.0.0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:28:19.520997 ieugwaspy-1.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1090 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-05 09:28:19.520997 ieugwaspy-1.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1455 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:28:19.516997 ieugwaspy-1.0.2/ieugwaspy/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      838 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      660 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/backwards.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1299 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6860 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1047 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/ieugwaspy/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:28:19.520997 ieugwaspy-1.0.2/ieugwaspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-05 09:28:19.000000 ieugwaspy-1.0.2/ieugwaspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-05 09:28:19.000000 ieugwaspy-1.0.2/ieugwaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 09:28:19.000000 ieugwaspy-1.0.2/ieugwaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 09:28:19.000000 ieugwaspy-1.0.2/ieugwaspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 09:28:19.000000 ieugwaspy-1.0.2/ieugwaspy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 09:28:19.520997 ieugwaspy-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      695 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:28:19.520997 ieugwaspy-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-05 09:28:12.000000 ieugwaspy-1.0.2/tests/test_api.py
```

### Comparing `ieugwaspy-1.0.0/LICENSE` & `ieugwaspy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ieugwaspy-1.0.0/PKG-INFO` & `ieugwaspy-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieugwaspy
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python interface to IEU GWAS database API
 Home-page: https://mrcieu.github.io/ieugwaspy/
 Author: Tom Gaunt
 Author-email: tom@biocompute.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,8 +33,9 @@
 - Obtain the summary results of specific variants across specific studies. LD-proxy lookups are performed automatically if a specific variant is absent from a study
 - Perform PheWAS (look up all associations for a variant)
 - Convert between chromosome:position and rsids and getting annotations
 
 
 #### Developer notes
 To run tests, use `pytest -v -s --select-api="dev"`
+
 To generate docs, use `pdoc --html ieugwaspy; rm -rf docs/; mkdir docs; mv html/ieugwaspy/* docs/; rm -r html/`
```

### Comparing `ieugwaspy-1.0.0/README.md` & `ieugwaspy-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 - Obtain the summary results of specific variants across specific studies. LD-proxy lookups are performed automatically if a specific variant is absent from a study
 - Perform PheWAS (look up all associations for a variant)
 - Convert between chromosome:position and rsids and getting annotations
 
 
 #### Developer notes
 To run tests, use `pytest -v -s --select-api="dev"`
-To generate docs, use `pdoc --html ieugwaspy; rm -rf docs/; mkdir docs; mv html/ieugwaspy/* docs/; rm -r html/`
+
+To generate docs, use `pdoc --html ieugwaspy; rm -rf docs/; mkdir docs; mv html/ieugwaspy/* docs/; rm -r html/`
```

### Comparing `ieugwaspy-1.0.0/ieugwaspy/api.py` & `ieugwaspy-1.0.2/ieugwaspy/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """API management
 """
 import ieugwaspy.config as config
 import webbrowser
 
+from .query import status
+
 
 def select_api(key="public"):
     """Select API base URL (no return value)
 
     Args:
         key: the short name for the required API base url
 
+    Returns:
+        data: JSON object as returned by API
+
     """
     if key in config.urls.keys():
         config.env["base_url"] = config.urls[key]
         print("API server is now: " + config.env["base_url"])
+        return status()
     else:
         print("Please select one from the following: \n" + "\n".join([k + " - " + v for k, v in config.urls.items()]))
 
 
 def get_jwt():
     """Obtain a token (JWT) and save it locally
     """
```

### Comparing `ieugwaspy-1.0.0/ieugwaspy/backwards.py` & `ieugwaspy-1.0.2/ieugwaspy/backwards.py`

 * *Files identical despite different names*

### Comparing `ieugwaspy-1.0.0/ieugwaspy/config.py` & `ieugwaspy-1.0.2/ieugwaspy/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 urls = {
     "public": "https://api.opengwas.io/api/",
     "private": "http://ieu-db-interface.epi.bris.ac.uk:8082/api/",
     "dev": "http://localhost:8019/api/"
 }
 url_obtain_jwt = "https://api.opengwas.io/profile/"
 
+allowance_reset_timestamp = 0
+
 
 def _save_env():
     """Save env variables to .ieugwaspy.json
 
     """
     with open(".ieugwaspy.json", "w") as f:
         json.dump(env, f)
```

### Comparing `ieugwaspy-1.0.0/ieugwaspy/query.py` & `ieugwaspy-1.0.2/ieugwaspy/query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,41 @@
 """API query functions
 """
+import datetime
+import time
 import requests
-
 from retry import retry
 from urllib.parse import urljoin
 
 import ieugwaspy.config as config
 import ieugwaspy.variants as variants
 import ieugwaspy.backwards as backwards
 
 
+def _check_allowance_reset_timestamp():
+    """Check existence of config.allowance_reset_timestamp, reset it when the time has passed or if not, halt the request
+    """
+    if config.allowance_reset_timestamp == 0:
+        return
+    if int(time.time()) > config.allowance_reset_timestamp:
+        config.allowance_reset_timestamp = 0
+    else:
+        raise Exception("You have run out of allowance. Please retry after {}".format(datetime.datetime.strftime(datetime.datetime.fromtimestamp(config.allowance_reset_timestamp).astimezone(), '%Y-%m-%d %H:%M %Z')))
+
+
+def _save_allowance_reset_timestamp(headers):
+    """Calculate and save the retry timestamp when there is no remaining allowance
+
+    Args:
+        headers: response headers
+    """
+    if headers.get('X-Allowance-Remaining', None) == "0":
+        config.allowance_reset_timestamp = int(time.time()) + int(headers.get('Retry-After', 0))
+
+
 @retry(tries=5, delay=2, backoff=2)
 def _api_query(path, method="GET", data=[]):
     """This is a general-purpose function called by other functions to query the API and return the resulting data in JSON format.  
 
     Args:
         path: the path component of the URL
         method: the HTTP method
@@ -35,14 +57,20 @@
         response = requests.get(url, headers=headers)
     elif method == "POST":
         response = requests.post(url, headers=headers, data=data)
     else:
         raise Exception("Invalid API method")
 
     try:
+        _check_allowance_reset_timestamp()
+    except Exception as e:
+        return str(e)
+
+    try:
+        _save_allowance_reset_timestamp(response.headers)
         return response.json()
     except Exception as e:
         raise Exception("Unable to parse the response. " + str(e))
 
 
 def status():
     """Check API status
@@ -50,14 +78,24 @@
     Returns:
         result: JSON object as returned by API
 
     """
     return _api_query("status")
 
 
+def user():
+    """Get user information
+
+    Returns:
+        result: JSON object as returned by API
+
+    """
+    return _api_query("user")
+
+
 def gwasinfo(id=[]):
     """This function will return GWAS study meta-data describing the specific studies selected by id
 
     Args:
         id (list): OpenGWAS IDs of specific studies, e.g. ["ieu-a-1239", "ieu-a-2"]
 
     Returns:
```

### Comparing `ieugwaspy-1.0.0/ieugwaspy/variants.py` & `ieugwaspy-1.0.2/ieugwaspy/variants.py`

 * *Files identical despite different names*

### Comparing `ieugwaspy-1.0.0/ieugwaspy.egg-info/PKG-INFO` & `ieugwaspy-1.0.2/ieugwaspy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ieugwaspy
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python interface to IEU GWAS database API
 Home-page: https://mrcieu.github.io/ieugwaspy/
 Author: Tom Gaunt
 Author-email: tom@biocompute.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -33,8 +33,9 @@
 - Obtain the summary results of specific variants across specific studies. LD-proxy lookups are performed automatically if a specific variant is absent from a study
 - Perform PheWAS (look up all associations for a variant)
 - Convert between chromosome:position and rsids and getting annotations
 
 
 #### Developer notes
 To run tests, use `pytest -v -s --select-api="dev"`
+
 To generate docs, use `pdoc --html ieugwaspy; rm -rf docs/; mkdir docs; mv html/ieugwaspy/* docs/; rm -r html/`
```

### Comparing `ieugwaspy-1.0.0/setup.py` & `ieugwaspy-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="ieugwaspy",
-    version="1.0.0",
+    version="1.0.2",
     author="Tom Gaunt",
     author_email="tom@biocompute.org.uk",
     description="Python interface to IEU GWAS database API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://mrcieu.github.io/ieugwaspy/",
     packages=setuptools.find_packages(),
```

### Comparing `ieugwaspy-1.0.0/tests/test_api.py` & `ieugwaspy-1.0.2/tests/test_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 
 
 def test_apistatus(ieugwaspy_instance):
     data = ieugwaspy_instance.status()
     assert data["API version"]
 
 
+def test_user(ieugwaspy_instance):
+    data = ieugwaspy_instance.user()
+    assert "uid" in data["user"]
+
+
 def test_variants_to_rsid(ieugwaspy_instance):
     data = ieugwaspy_instance.variants_to_rsid(["rs1234", "10:44865737"])
     assert set(data) == {"rs1234", "rs7777"}
 
 
 def test_gwasinfo_single(ieugwaspy_instance):
     data = ieugwaspy_instance.gwasinfo(["ieu-a-1239"])
```

