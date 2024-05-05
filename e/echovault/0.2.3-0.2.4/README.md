# Comparing `tmp/echovault-0.2.3.tar.gz` & `tmp/echovault-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echovault-0.2.3.tar", max compression
+gzip compressed data, was "echovault-0.2.4.tar", max compression
```

## Comparing `echovault-0.2.3.tar` & `echovault-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.3/README.md
--rw-r--r--   0        0        0       34 2024-04-25 18:14:25.800920 echovault-0.2.3/echovault/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.3/echovault/__init__.py~
--rw-r--r--   0        0        0     1028 2024-04-25 04:59:27.197132 echovault-0.2.3/echovault/_container.py
--rw-r--r--   0        0        0     1030 2024-04-24 19:49:03.244111 echovault-0.2.3/echovault/_container.py~
--rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.3/echovault/db.py~
--rw-r--r--   0        0        0     1782 2024-04-24 19:17:52.808075 echovault-0.2.3/echovault/dict.py
--rw-r--r--   0        0        0     2283 2024-04-23 18:43:20.644733 echovault-0.2.3/echovault/dict.py~
--rw-r--r--   0        0        0     1217 2024-04-25 05:01:58.009942 echovault-0.2.3/echovault/list.py
--rw-r--r--   0        0        0     1176 2024-04-24 19:49:34.034385 echovault-0.2.3/echovault/list.py~
--rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.3/echovault/table.py~
--rw-r--r--   0        0        0     3606 2024-04-25 19:47:51.389876 echovault-0.2.3/echovault/vault.py
--rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.3/echovault/vault.py~
--rw-r--r--   0        0        0      380 2024-04-25 19:48:05.366688 echovault-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-19 19:04:53.372948 echovault-0.2.4/README.md
+-rw-r--r--   0        0        0       34 2024-04-25 18:14:25.800920 echovault-0.2.4/echovault/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 05:54:15.655547 echovault-0.2.4/echovault/__init__.py~
+-rw-r--r--   0        0        0     1028 2024-04-28 19:08:59.099761 echovault-0.2.4/echovault/_container.py
+-rw-r--r--   0        0        0     1030 2024-04-24 19:49:03.244111 echovault-0.2.4/echovault/_container.py~
+-rw-r--r--   0        0        0        0 2024-04-11 19:04:01.114880 echovault-0.2.4/echovault/db.py~
+-rw-r--r--   0        0        0     2733 2024-04-30 18:15:33.064347 echovault-0.2.4/echovault/dict.py
+-rw-r--r--   0        0        0     2283 2024-04-23 18:43:20.644733 echovault-0.2.4/echovault/dict.py~
+-rw-r--r--   0        0        0     2305 2024-04-30 19:41:38.740513 echovault-0.2.4/echovault/list.py
+-rw-r--r--   0        0        0     1176 2024-04-24 19:49:34.034385 echovault-0.2.4/echovault/list.py~
+-rw-r--r--   0        0        0     2903 2024-04-14 19:48:17.176500 echovault-0.2.4/echovault/table.py~
+-rw-r--r--   0        0        0     6912 2024-05-05 18:15:23.514138 echovault-0.2.4/echovault/vault.py
+-rw-r--r--   0        0        0     8070 2024-05-05 18:08:25.266920 echovault-0.2.4/echovault/vault.py.bck
+-rw-r--r--   0        0        0     1289 2024-04-14 19:18:41.190124 echovault-0.2.4/echovault/vault.py~
+-rw-r--r--   0        0        0      380 2024-05-05 18:21:21.324123 echovault-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1492 1970-01-01 00:00:00.000000 echovault-0.2.4/PKG-INFO
```

### Comparing `echovault-0.2.3/README.md` & `echovault-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `echovault-0.2.3/echovault/_container.py` & `echovault-0.2.4/echovault/_container.py`

 * *Files identical despite different names*

### Comparing `echovault-0.2.3/echovault/_container.py~` & `echovault-0.2.4/echovault/_container.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.3/echovault/dict.py` & `echovault-0.2.4/echovault/list.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,79 @@
 from dulwich.objects import Tree, Blob
-from pickle import dumps, loads
-from base64 import b64decode, b64encode
-from stat import S_IFREG
-from echovault._container import Container 
-
-class Dict(Container):
-    @staticmethod
-    def encode(value):
-        return b64encode(dumps(value))
-
-    @staticmethod
-    def decode(value):
-        return loads(b64decode(value))
-    
-    def __init__(self, object_store, container, identifier, items=(), *, tree=None):
+from stat import S_IFREG, S_IFDIR
+from uuid import uuid4
+from echovault._container import Container
+from echovault.dict import Dict
+
+class List(Container):
+    def __init__(self, object_store, container, identifier, values=(), *, tree=None):
         super().__init__(object_store, container, identifier, tree)
-        self.update(items)
+        self.extend(values)
 
     def __getitem__(self, key):
-        _, id_ = self.tree[self.encode(key)]
-        return loads(self.object_store[id_].data)
-
-    def __setitem__(self, key, value):
-        self.update(((key, value),))
+        _, id_ = self.tree[key]
+        return Dict(self.object_store,
+                    self,
+                    key,
+                    tree=self.object_store[id_])
 
-    def update(self, items):
-        if hasattr(items, 'items'):
-            items = items.items()
         
-        for key, value in items:
-            blob = Blob()
-            blob.data = dumps(value)
-        
-            if not blob.id in self.object_store:
-                self.object_store.add_object(blob)
+    def __iter__(self):
+        for key in self.tree:
+            if key == b'_':
+                continue
             
-            self.tree[self.encode(key)] = S_IFREG | 0o755, blob.id
-
-        self._update()
+            yield self[key]
 
+    def __repr__(self):
+        return repr(list(iter(self)))
+            
+    def append(self, value):
+        self.extend((value,))
+            
+    def extend(self, iterable):
+        for item in iterable:
+            identifier = str(uuid4()).encode('utf-8')
+            self.tree[identifier] = S_IFDIR, None
+            entry = Dict(self.object_store,
+                         self,
+                         identifier,
+                         item)
 
-    def __delitem__(self, key):
-        del self.tree[self.encode(key)]
-        
         self._update()
             
-    def __iter__(self):
-        return (self.decode(raw_key)
-                for raw_key
-                in iter(self.tree)
-                if raw_key != b'_')
-
-    def keys(self):
-        yield from iter(self)
-
-    def items(self):
-        for key in self.keys():
-            yield (key, self[key])
-
-    def values(self):
-        for _, id_ in self.tree.values:
-            return loads(self.object_store[id_].data)
+    def remove(self, entry):
+        del self.tree[entry.identifier]
         
-    def __repr__(self):
-        return repr(dict(self.items()))
+        self._update()
+
+    def diff(self, other):
+        if self.tree.id == other.tree.id:
+            return
+
+        sks = set(self.tree) - {b'_'}
+        oks = set(other.tree) - {b'_'}
+
+        removed = oks - sks
+        if removed:
+            yield ('-', removed)
+
+        added = sks - oks
+        if added:
+            yield ('+',
+                   tuple(dict(self[key].items())
+                         for key in added))
+            
+        for key in sks.intersection(oks):
+            for difference in self[key].diff(other[key]):
+                yield ('!=', key, *difference)
+
+    def patch(self, differences):
+        for difference in differences:
+            match difference:
+                case ('-', removed):
+                    for key in removed:
+                        self.remove(self[key])
+                case ('+', added):
+                    self.extend(added)
+                case ('!=', key, *difference):
+                    self[key].patch((difference,))
```

### Comparing `echovault-0.2.3/echovault/dict.py~` & `echovault-0.2.4/echovault/dict.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.3/echovault/list.py` & `echovault-0.2.4/echovault/list.py~`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dulwich.objects import Tree, Blob
 from stat import S_IFREG, S_IFDIR
 from uuid import uuid4
 from echovault._container import Container
-from echovault.dict import Dict
-
+            
 class List(Container):
     def __init__(self, object_store, container, identifier, values=(), *, tree=None):
         super().__init__(object_store, container, identifier, tree)
         self.extend(values)
 
     def __iter__(self):
         for key in self.tree:
@@ -21,20 +20,19 @@
                        tree=self.object_store[id_])
             
     def append(self, value):
         self.extend((value,))
             
     def extend(self, iterable):
         for item in iterable:
-            identifier = str(uuid4()).encode('utf-8')
-            self.tree[identifier] = S_IFDIR, None
             entry = Dict(self.object_store,
                          self,
-                         identifier,
+                         str(uuid4()).encode('utf-8'),
                          item)
+            self.tree[entry.identifier] = S_IFDIR, entry.tree.id
 
         self._update()
             
     def remove(self, entry):
         del self.tree[entry.identifier]
         
         self._update()
```

### Comparing `echovault-0.2.3/echovault/table.py~` & `echovault-0.2.4/echovault/table.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.3/echovault/vault.py~` & `echovault-0.2.4/echovault/vault.py~`

 * *Files identical despite different names*

### Comparing `echovault-0.2.3/PKG-INFO` & `echovault-0.2.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echovault
-Version: 0.2.3
+Version: 0.2.4
 Summary: echovault is git data storage
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

