# Comparing `tmp/whoisit-2.7.6.tar.gz` & `tmp/whoisit-2.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whoisit-2.7.6.tar", last modified: Tue Apr 30 09:48:48 2024, max compression
+gzip compressed data, was "whoisit-2.7.7.tar", last modified: Sun May  5 04:01:17 2024, max compression
```

## Comparing `whoisit-2.7.6.tar` & `whoisit-2.7.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-30 09:48:48.507689 whoisit-2.7.6/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1528 2021-06-06 06:10:53.000000 whoisit-2.7.6/LICENSE
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2021-06-10 06:05:53.000000 whoisit-2.7.6/MANIFEST.in
--rw-r--r--   0 meeb      (1000) meeb      (1000)    21999 2024-04-30 09:48:48.507689 whoisit-2.7.6/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21080 2024-04-30 09:42:11.000000 whoisit-2.7.6/README.md
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:28:45.000000 whoisit-2.7.6/requirements.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2024-04-30 09:48:48.507689 whoisit-2.7.6/setup.cfg
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1359 2024-04-30 09:48:20.000000 whoisit-2.7.6/setup.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-30 09:48:48.507689 whoisit-2.7.6/tests/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-06-06 06:14:06.000000 whoisit-2.7.6/tests/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    11786 2022-12-06 10:28:45.000000 whoisit-2.7.6/tests/test_bootstrap.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    21934 2022-12-06 10:28:45.000000 whoisit-2.7.6/tests/test_parser.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     5150 2021-11-18 03:52:35.000000 whoisit-2.7.6/tests/test_query.py
--rw-r--r--   0 meeb      (1000) meeb      (1000)     2070 2023-06-03 08:56:21.000000 whoisit-2.7.6/tests/test_ssl.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-30 09:48:48.507689 whoisit-2.7.6/whoisit/
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     3100 2024-04-30 09:39:47.000000 whoisit-2.7.6/whoisit/__init__.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    17741 2023-06-03 08:55:54.000000 whoisit-2.7.6/whoisit/bootstrap.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      937 2022-12-06 10:28:45.000000 whoisit-2.7.6/whoisit/errors.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      522 2021-06-08 06:47:34.000000 whoisit-2.7.6/whoisit/logger.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     1952 2024-04-30 09:46:15.000000 whoisit-2.7.6/whoisit/overrides.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)    16292 2024-04-30 09:34:29.000000 whoisit-2.7.6/whoisit/parser.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     8965 2023-06-03 07:58:57.000000 whoisit-2.7.6/whoisit/query.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)     4147 2024-04-30 08:46:33.000000 whoisit-2.7.6/whoisit/utils.py
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       18 2024-04-30 09:48:26.000000 whoisit-2.7.6/whoisit/version.py
-drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-04-30 09:48:48.507689 whoisit-2.7.6/whoisit.egg-info/
--rw-r--r--   0 meeb      (1000) meeb      (1000)    21999 2024-04-30 09:48:48.000000 whoisit-2.7.6/whoisit.egg-info/PKG-INFO
--rw-rw-r--   0 meeb      (1000) meeb      (1000)      489 2024-04-30 09:48:48.000000 whoisit-2.7.6/whoisit.egg-info/SOURCES.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2024-04-30 09:48:48.000000 whoisit-2.7.6/whoisit.egg-info/dependency_links.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2024-04-30 09:48:48.000000 whoisit-2.7.6/whoisit.egg-info/requires.txt
--rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2024-04-30 09:48:48.000000 whoisit-2.7.6/whoisit.egg-info/top_level.txt
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-05 04:01:17.404141 whoisit-2.7.7/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1528 2021-06-06 06:10:53.000000 whoisit-2.7.7/LICENSE
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2021-06-10 06:05:53.000000 whoisit-2.7.7/MANIFEST.in
+-rw-r--r--   0 meeb      (1000) meeb      (1000)    23141 2024-05-05 04:01:17.404141 whoisit-2.7.7/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    22222 2024-04-30 10:00:33.000000 whoisit-2.7.7/README.md
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2022-12-06 10:28:45.000000 whoisit-2.7.7/requirements.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       79 2024-05-05 04:01:17.404141 whoisit-2.7.7/setup.cfg
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     1359 2024-05-05 03:59:05.000000 whoisit-2.7.7/setup.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-05 04:01:17.404141 whoisit-2.7.7/tests/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        0 2021-06-06 06:14:06.000000 whoisit-2.7.7/tests/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    11791 2024-05-05 03:58:20.000000 whoisit-2.7.7/tests/test_bootstrap.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    21934 2022-12-06 10:28:45.000000 whoisit-2.7.7/tests/test_parser.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     5150 2021-11-18 03:52:35.000000 whoisit-2.7.7/tests/test_query.py
+-rw-r--r--   0 meeb      (1000) meeb      (1000)     2070 2023-06-03 08:56:21.000000 whoisit-2.7.7/tests/test_ssl.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-05 04:01:17.404141 whoisit-2.7.7/whoisit/
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     3100 2024-04-30 09:39:47.000000 whoisit-2.7.7/whoisit/__init__.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    17808 2024-05-05 03:57:25.000000 whoisit-2.7.7/whoisit/bootstrap.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      937 2022-12-06 10:28:45.000000 whoisit-2.7.7/whoisit/errors.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      522 2021-06-08 06:47:34.000000 whoisit-2.7.7/whoisit/logger.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     2062 2024-05-05 03:57:25.000000 whoisit-2.7.7/whoisit/overrides.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)    16292 2024-04-30 09:34:29.000000 whoisit-2.7.7/whoisit/parser.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     8965 2023-06-03 07:58:57.000000 whoisit-2.7.7/whoisit/query.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)     4147 2024-04-30 08:46:33.000000 whoisit-2.7.7/whoisit/utils.py
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       18 2024-05-05 03:59:13.000000 whoisit-2.7.7/whoisit/version.py
+drwxrwxr-x   0 meeb      (1000) meeb      (1000)        0 2024-05-05 04:01:17.404141 whoisit-2.7.7/whoisit.egg-info/
+-rw-r--r--   0 meeb      (1000) meeb      (1000)    23141 2024-05-05 04:01:17.000000 whoisit-2.7.7/whoisit.egg-info/PKG-INFO
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)      489 2024-05-05 04:01:17.000000 whoisit-2.7.7/whoisit.egg-info/SOURCES.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)        1 2024-05-05 04:01:17.000000 whoisit-2.7.7/whoisit.egg-info/dependency_links.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       43 2024-05-05 04:01:17.000000 whoisit-2.7.7/whoisit.egg-info/requires.txt
+-rw-rw-r--   0 meeb      (1000) meeb      (1000)       14 2024-05-05 04:01:17.000000 whoisit-2.7.7/whoisit.egg-info/top_level.txt
```

### Comparing `whoisit-2.7.6/LICENSE` & `whoisit-2.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.6/PKG-INFO` & `whoisit-2.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisit
-Version: 2.7.6
+Version: 2.7.7
 Summary: A Python client to RDAP WHOIS-like services for internet resources.
 Home-page: https://github.com/meeb/whoisit
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: BSD
 Keywords: whoisit,whois,rdap,ip,network,cidr,prefix,domain,asn,autnum,tld,entity,handle,arin,afrinic,apnic,ripe,lacnic
 Classifier: Development Status :: 5 - Production/Stable
@@ -92,15 +92,15 @@
 
 In each case `results` will be a dictionary containing the most useful information for
 each request type. If the data you want is not in the response you can request the raw,
 unparsed and large RDAP JSON data by adding the `raw=True` argument to the request, for
 example:
 
 ```python
-results = whoisit.domain('example.com', raw=True, follow_related=True)
+results = whoisit.domain('example.com', raw=True)
 # 'results' is now the full, raw response from the RDAP service
 ```
 
 If for some reason you accidentally end up querying the wrong RDAP endpoint your query
 should end up still working, for example if you query ARIN for information on the IP
 address `1.1.1.1` it will redirect you to APNIC (where `1.1.1.1` is allocated)
 automatically.
@@ -124,18 +124,14 @@
 # which RDAP service to query as the entity has no RIR prefix or postfix
 results = whoisit.entity('AS5089-MNT')
 
 # This will work OK because the entity is registered at RIPE
 results = whoisit.entity('AS5089-MNT', rir='ripe')
 ```
 
-By default for domain lookups `whoisit` will attempt to make sub-requests to any listed
-related or registered child RDAP endpoints. You can disable this by setting
-`follow_related=False`.
-
 
 ### Weaken SSL ciphers
 
 Some RDAP servers do not have particularly secure SSL implementations. As RDAP returns
 read-only and public information it may be acceptable for you to want to downgrade the
 security of your `whoisit` requests to successfully return data.
 
@@ -154,14 +150,46 @@
 
 Note that with `allow_insecure_ssl=True` the upstream RDAP server certificate is
 still validated, it just permits weaker SSL ciphers during the handshake. You should
 only use `allow_insecure_ssl=True` if your request fails with an SSL cipher or
 handshake error first.
 
 
+### Domain lookup subrequests
+
+Many RDAP endpoints for domains supply a related RDAP server run by a registry which
+may contain more information about the domain. `whoisit` by default will attempt to
+make a subrequest to the related RDAP endpoint if available to obtain more detailed
+results. Occasionally, the related RDAP endpoints may fail or return data in an
+invalid format. You can disable related RDAP endpoint subrequests by passing the
+`follow_related=False` argument to `whoisit.domain(...)`. For example (as of 2024-04-30):
+
+```python
+results = whoisit.domain('example.com', follow_related=False)
+```
+
+If you encounter a parsing error when using related RDAP endpoint data you can also
+skip the parsing by using `raw=True` but continue to use related RDAP data. `whoisit`
+will attempt to handle the RDAP data returned but there will be occasions when RDAP
+results change beyond what `whoisit` can parse. When using raw data you will need to
+parse the data yourself.
+
+You can also write a fallback:
+
+```python
+try:
+    results = whoisit.domain('example.com')
+    # Assume an error parsing the related RDAP data occurs here
+except Exception as e:
+    print(f'Failed to look up domain, trying fallback: {e}')
+    results = whoisit.domain('example.com', follow_related=False)
+    # Likely to succeed if the related RDAP data was the issue
+```
+
+
 ## Bootstrapping
 
 `whoisit` needs to know which RDAP service to query for a resource. This information is
 provided by the IANA as bootstrapping information. Bootstrapping data simply says things
 like "this CIDR is allocated to ARIN, this CIDR is allocated to RIPE" and so on for all
 resources. The bootstrap data means you should be directly querying the correct RDAP
 server for your request at all times. You should cache the bootstrap information locally
```

### Comparing `whoisit-2.7.6/README.md` & `whoisit-2.7.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 In each case `results` will be a dictionary containing the most useful information for
 each request type. If the data you want is not in the response you can request the raw,
 unparsed and large RDAP JSON data by adding the `raw=True` argument to the request, for
 example:
 
 ```python
-results = whoisit.domain('example.com', raw=True, follow_related=True)
+results = whoisit.domain('example.com', raw=True)
 # 'results' is now the full, raw response from the RDAP service
 ```
 
 If for some reason you accidentally end up querying the wrong RDAP endpoint your query
 should end up still working, for example if you query ARIN for information on the IP
 address `1.1.1.1` it will redirect you to APNIC (where `1.1.1.1` is allocated)
 automatically.
@@ -101,18 +101,14 @@
 # which RDAP service to query as the entity has no RIR prefix or postfix
 results = whoisit.entity('AS5089-MNT')
 
 # This will work OK because the entity is registered at RIPE
 results = whoisit.entity('AS5089-MNT', rir='ripe')
 ```
 
-By default for domain lookups `whoisit` will attempt to make sub-requests to any listed
-related or registered child RDAP endpoints. You can disable this by setting
-`follow_related=False`.
-
 
 ### Weaken SSL ciphers
 
 Some RDAP servers do not have particularly secure SSL implementations. As RDAP returns
 read-only and public information it may be acceptable for you to want to downgrade the
 security of your `whoisit` requests to successfully return data.
 
@@ -131,14 +127,46 @@
 
 Note that with `allow_insecure_ssl=True` the upstream RDAP server certificate is
 still validated, it just permits weaker SSL ciphers during the handshake. You should
 only use `allow_insecure_ssl=True` if your request fails with an SSL cipher or
 handshake error first.
 
 
+### Domain lookup subrequests
+
+Many RDAP endpoints for domains supply a related RDAP server run by a registry which
+may contain more information about the domain. `whoisit` by default will attempt to
+make a subrequest to the related RDAP endpoint if available to obtain more detailed
+results. Occasionally, the related RDAP endpoints may fail or return data in an
+invalid format. You can disable related RDAP endpoint subrequests by passing the
+`follow_related=False` argument to `whoisit.domain(...)`. For example (as of 2024-04-30):
+
+```python
+results = whoisit.domain('example.com', follow_related=False)
+```
+
+If you encounter a parsing error when using related RDAP endpoint data you can also
+skip the parsing by using `raw=True` but continue to use related RDAP data. `whoisit`
+will attempt to handle the RDAP data returned but there will be occasions when RDAP
+results change beyond what `whoisit` can parse. When using raw data you will need to
+parse the data yourself.
+
+You can also write a fallback:
+
+```python
+try:
+    results = whoisit.domain('example.com')
+    # Assume an error parsing the related RDAP data occurs here
+except Exception as e:
+    print(f'Failed to look up domain, trying fallback: {e}')
+    results = whoisit.domain('example.com', follow_related=False)
+    # Likely to succeed if the related RDAP data was the issue
+```
+
+
 ## Bootstrapping
 
 `whoisit` needs to know which RDAP service to query for a resource. This information is
 provided by the IANA as bootstrapping information. Bootstrapping data simply says things
 like "this CIDR is allocated to ARIN, this CIDR is allocated to RIPE" and so on for all
 resources. The bootstrap data means you should be directly querying the correct RDAP
 server for your request at all times. You should cache the bootstrap information locally
```

### Comparing `whoisit-2.7.6/setup.py` & `whoisit-2.7.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 
-version = '2.7.6'
+version = '2.7.7'
 
 
 with open('README.md', 'rt') as f:
     long_description = f.read()
 
 
 with open('requirements.txt', 'rt') as f:
```

### Comparing `whoisit-2.7.6/tests/test_bootstrap.py` & `whoisit-2.7.7/tests/test_bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     maxDiff = None
 
     def setUp(self):
         whoisit.clear_bootstrapping()
         with open(BASE_DIR / 'data_bootstrap.json', 'rt') as f:
             self.bootstrap_data = f.read()
-    
+
     def tearDown(self):
         whoisit.clear_bootstrapping()
 
     def test_bootstrap_saving(self):
         whoisit.clear_bootstrapping()
         whoisit.load_bootstrap_data(self.bootstrap_data)
         test_dict = json.loads(self.bootstrap_data)
@@ -199,15 +199,15 @@
             whoisit._bootstrap.get_rir_endpoint('test')
 
         # Check the RIRs are all supported
         for name, endpoint in whoisit._bootstrap.RIR_RDAP_ENDPOINTS.items():
             self.assertEqual(whoisit._bootstrap.get_rir_endpoint(name), endpoint)
 
         # Check the RIR names are valid
-        expected = ('afrinic', 'arin', 'apnic', 'jpnic', 'idnic', 'krnic',
+        expected = ('afnic', 'afrinic', 'arin', 'apnic', 'jpnic', 'idnic', 'krnic',
                     'lacnic', 'registro.br', 'ripe', 'twnic')
         self.assertEqual(whoisit._bootstrap.get_rir_endpoint_names(), expected)
 
         # Clean up
         whoisit.clear_bootstrapping()
 
     def test_iana_overrides(self):
```

### Comparing `whoisit-2.7.6/tests/test_parser.py` & `whoisit-2.7.7/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.6/tests/test_query.py` & `whoisit-2.7.7/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.6/tests/test_ssl.py` & `whoisit-2.7.7/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.6/whoisit/__init__.py` & `whoisit-2.7.7/whoisit/__init__.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.6/whoisit/bootstrap.py` & `whoisit-2.7.7/whoisit/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,27 +29,29 @@
     DEFAULT_RDAP_FALLBACKS = (
         'https://rdap.arin.net/registry/',
         'https://rdap.db.ripe.net/',
         'https://rdap.apnic.net/'
     )
     # Map of RIR RDAP endpoints
     RIR_RDAP_ENDPOINTS = {
+        'afnic': 'https://rdap.nic.fr/',
         'afrinic': 'https://rdap.afrinic.net/rdap/',
         'arin': 'https://rdap.arin.net/registry/',
         'apnic': 'https://rdap.apnic.net/',
         'jpnic': 'https://jpnic.rdap.apnic.net/',
         'idnic': 'https://idnic.rdap.apnic.net/',
         'krnic': 'https://krnic.rdap.apnic.net/',
         'lacnic': 'https://rdap.lacnic.net/rdap/',
         'registro.br': 'https://rdap.registro.br/',
         'ripe': 'https://rdap.db.ripe.net/',
         'twnic': 'https://twnic.rdap.apnic.net/',
     }
     # Map of entity prefix and postfixes to RIRs, used to guess entity RIR
     RIR_ENTITY_PREFIXES = {
+        'AFNIC': 'afnic',
         'AFRINIC': 'afrinic',
         'ARIN': 'arin',
         'AP': 'apnic',
         'JPNIC': 'jpnic',
         'KR': 'krnic',
         'ID': 'idnic',
         'LACNIC': 'lacnic',
```

### Comparing `whoisit-2.7.6/whoisit/errors.py` & `whoisit-2.7.7/whoisit/errors.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.6/whoisit/logger.py` & `whoisit-2.7.7/whoisit/logger.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.6/whoisit/overrides.py` & `whoisit-2.7.7/whoisit/overrides.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,10 +37,13 @@
         'lc': ['https://rdap.identitydigital.services/rdap/'],
         'me': ['https://rdap.identitydigital.services/rdap/'],
         'mn': ['https://rdap.identitydigital.services/rdap/'],
         'pr': ['https://rdap.identitydigital.services/rdap/'],
         'sc': ['https://rdap.identitydigital.services/rdap/'],
         'sh': ['https://rdap.identitydigital.services/rdap/'],
         'vc': ['https://rdap.identitydigital.services/rdap/'],
+
+        # 2024-05-03 - .co has an RDAP endpoint it's just not listed
+        'co': ['https://rdap.nic.co/'],
     }
 
 }
```

### Comparing `whoisit-2.7.6/whoisit/parser.py` & `whoisit-2.7.7/whoisit/parser.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.6/whoisit/query.py` & `whoisit-2.7.7/whoisit/query.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.6/whoisit/utils.py` & `whoisit-2.7.7/whoisit/utils.py`

 * *Files identical despite different names*

### Comparing `whoisit-2.7.6/whoisit.egg-info/PKG-INFO` & `whoisit-2.7.7/whoisit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisit
-Version: 2.7.6
+Version: 2.7.7
 Summary: A Python client to RDAP WHOIS-like services for internet resources.
 Home-page: https://github.com/meeb/whoisit
 Author: https://github.com/meeb
 Author-email: meeb@meeb.org
 License: BSD
 Keywords: whoisit,whois,rdap,ip,network,cidr,prefix,domain,asn,autnum,tld,entity,handle,arin,afrinic,apnic,ripe,lacnic
 Classifier: Development Status :: 5 - Production/Stable
@@ -92,15 +92,15 @@
 
 In each case `results` will be a dictionary containing the most useful information for
 each request type. If the data you want is not in the response you can request the raw,
 unparsed and large RDAP JSON data by adding the `raw=True` argument to the request, for
 example:
 
 ```python
-results = whoisit.domain('example.com', raw=True, follow_related=True)
+results = whoisit.domain('example.com', raw=True)
 # 'results' is now the full, raw response from the RDAP service
 ```
 
 If for some reason you accidentally end up querying the wrong RDAP endpoint your query
 should end up still working, for example if you query ARIN for information on the IP
 address `1.1.1.1` it will redirect you to APNIC (where `1.1.1.1` is allocated)
 automatically.
@@ -124,18 +124,14 @@
 # which RDAP service to query as the entity has no RIR prefix or postfix
 results = whoisit.entity('AS5089-MNT')
 
 # This will work OK because the entity is registered at RIPE
 results = whoisit.entity('AS5089-MNT', rir='ripe')
 ```
 
-By default for domain lookups `whoisit` will attempt to make sub-requests to any listed
-related or registered child RDAP endpoints. You can disable this by setting
-`follow_related=False`.
-
 
 ### Weaken SSL ciphers
 
 Some RDAP servers do not have particularly secure SSL implementations. As RDAP returns
 read-only and public information it may be acceptable for you to want to downgrade the
 security of your `whoisit` requests to successfully return data.
 
@@ -154,14 +150,46 @@
 
 Note that with `allow_insecure_ssl=True` the upstream RDAP server certificate is
 still validated, it just permits weaker SSL ciphers during the handshake. You should
 only use `allow_insecure_ssl=True` if your request fails with an SSL cipher or
 handshake error first.
 
 
+### Domain lookup subrequests
+
+Many RDAP endpoints for domains supply a related RDAP server run by a registry which
+may contain more information about the domain. `whoisit` by default will attempt to
+make a subrequest to the related RDAP endpoint if available to obtain more detailed
+results. Occasionally, the related RDAP endpoints may fail or return data in an
+invalid format. You can disable related RDAP endpoint subrequests by passing the
+`follow_related=False` argument to `whoisit.domain(...)`. For example (as of 2024-04-30):
+
+```python
+results = whoisit.domain('example.com', follow_related=False)
+```
+
+If you encounter a parsing error when using related RDAP endpoint data you can also
+skip the parsing by using `raw=True` but continue to use related RDAP data. `whoisit`
+will attempt to handle the RDAP data returned but there will be occasions when RDAP
+results change beyond what `whoisit` can parse. When using raw data you will need to
+parse the data yourself.
+
+You can also write a fallback:
+
+```python
+try:
+    results = whoisit.domain('example.com')
+    # Assume an error parsing the related RDAP data occurs here
+except Exception as e:
+    print(f'Failed to look up domain, trying fallback: {e}')
+    results = whoisit.domain('example.com', follow_related=False)
+    # Likely to succeed if the related RDAP data was the issue
+```
+
+
 ## Bootstrapping
 
 `whoisit` needs to know which RDAP service to query for a resource. This information is
 provided by the IANA as bootstrapping information. Bootstrapping data simply says things
 like "this CIDR is allocated to ARIN, this CIDR is allocated to RIPE" and so on for all
 resources. The bootstrap data means you should be directly querying the correct RDAP
 server for your request at all times. You should cache the bootstrap information locally
```

