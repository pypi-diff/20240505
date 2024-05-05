# Comparing `tmp/vastpy-0.2.0.tar.gz` & `tmp/vastpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastpy-0.2.0.tar", max compression
+gzip compressed data, was "vastpy-0.2.1.tar", max compression
```

## Comparing `vastpy-0.2.0.tar` & `vastpy-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1628 2023-03-21 11:44:48.273010 vastpy-0.2.0/README.md
--rw-r--r--   0        0        0      277 2023-03-21 11:45:51.345485 vastpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3007 2023-03-21 11:43:24.350566 vastpy-0.2.0/vastpy/__init__.py
--rw-r--r--   0        0        0     2195 1970-01-01 00:00:00.000000 vastpy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-01 09:07:29.471312 vastpy-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1625 2024-02-06 09:46:54.350267 vastpy-0.2.1/README.md
+-rw-r--r--   0        0        0      277 2024-05-05 11:56:36.646872 vastpy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3005 2024-05-05 11:57:01.935406 vastpy-0.2.1/vastpy/__init__.py
+-rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 vastpy-0.2.1/PKG-INFO
```

### Comparing `vastpy-0.2.0/README.md` & `vastpy-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ```
 
 Creating objects:
 
 ```python
 policy, = client.viewpolicies.get(name='default')
 
-view = client.views.post(path='/prod/pgsql', policy_id=default['id'], create_dir=True)
+view = client.views.post(path='/prod/pgsql', policy_id=policy['id'], create_dir=True)
 ```
 
 Modifying/deleting objects:
 
 ```python
 view, = client.views.get(path='/prod/pgsql')
 
@@ -64,15 +64,15 @@
 Reading metrics:
 
 ```python
 
 client.monitors.ad_hoc_query.get(object_type='cluster',
                                  time_frame='5m',
 				 prop_list=['ProtoMetrics,proto_name=ProtoCommon,iops',
-				            'ProtoMetrics,proto_name=ProtoCommon,iops'])
+				            'ProtoMetrics,proto_name=ProtoCommon,bw'])
 
 ```
 
 Version Compatibility
 ---------------------
 
 This package is compatible with any VAST version as it's schema-less.
```

### Comparing `vastpy-0.2.0/vastpy/__init__.py` & `vastpy-0.2.1/vastpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,8 +67,8 @@
     def put(self, **params):
         return self.request('PUT', data=params)
     def patch(self, **params):
         return self.request('PATCH', data=params)
     def options(self, **params):
         return self.request('OPTIONS', fields=params)
     def delete(self, **params):
-        return self.request('DELETE', fields=params)
+        return self.request('DELETE', data=params)
```

### Comparing `vastpy-0.2.0/PKG-INFO` & `vastpy-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: vastpy
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Alon Horev
 Author-email: alon@vastdata.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: urllib3 (>=1.2,<2.0)
 Description-Content-Type: text/markdown
 
 
 VASTPY
 ======
 
@@ -61,15 +62,15 @@
 ```
 
 Creating objects:
 
 ```python
 policy, = client.viewpolicies.get(name='default')
 
-view = client.views.post(path='/prod/pgsql', policy_id=default['id'], create_dir=True)
+view = client.views.post(path='/prod/pgsql', policy_id=policy['id'], create_dir=True)
 ```
 
 Modifying/deleting objects:
 
 ```python
 view, = client.views.get(path='/prod/pgsql')
 
@@ -81,15 +82,15 @@
 Reading metrics:
 
 ```python
 
 client.monitors.ad_hoc_query.get(object_type='cluster',
                                  time_frame='5m',
 				 prop_list=['ProtoMetrics,proto_name=ProtoCommon,iops',
-				            'ProtoMetrics,proto_name=ProtoCommon,iops'])
+				            'ProtoMetrics,proto_name=ProtoCommon,bw'])
 
 ```
 
 Version Compatibility
 ---------------------
 
 This package is compatible with any VAST version as it's schema-less.
```

