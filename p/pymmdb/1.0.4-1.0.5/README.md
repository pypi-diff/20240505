# Comparing `tmp/pymmdb-1.0.4-py3-none-any.whl.zip` & `tmp/pymmdb-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7483 bytes, number of entries: 7
+Zip file size: 7487 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-03 17:24 pymmdb/__init__.py
--rw-rw-rw-  2.0 fat     6054 b- defN 24-May-04 18:31 pymmdb/mmdb.py
--rw-rw-rw-  2.0 fat    11358 b- defN 24-May-04 21:08 pymmdb-1.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      522 b- defN 24-May-04 21:08 pymmdb-1.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-04 21:08 pymmdb-1.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-May-04 21:08 pymmdb-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      524 b- defN 24-May-04 21:08 pymmdb-1.0.4.dist-info/RECORD
-7 files, 18579 bytes uncompressed, 6557 bytes compressed:  64.7%
+-rw-rw-rw-  2.0 fat     6019 b- defN 24-May-05 12:15 pymmdb/mmdb.py
+-rw-rw-rw-  2.0 fat    11358 b- defN 24-May-05 12:16 pymmdb-1.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      522 b- defN 24-May-05 12:16 pymmdb-1.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 12:16 pymmdb-1.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-05 12:16 pymmdb-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      524 b- defN 24-May-05 12:16 pymmdb-1.0.5.dist-info/RECORD
+7 files, 18544 bytes uncompressed, 6561 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pymmdb/__init__.py
 Comment: 
 
 Filename: pymmdb/mmdb.py
 Comment: 
 
-Filename: pymmdb-1.0.4.dist-info/LICENSE
+Filename: pymmdb-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: pymmdb-1.0.4.dist-info/METADATA
+Filename: pymmdb-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: pymmdb-1.0.4.dist-info/WHEEL
+Filename: pymmdb-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: pymmdb-1.0.4.dist-info/top_level.txt
+Filename: pymmdb-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pymmdb-1.0.4.dist-info/RECORD
+Filename: pymmdb-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymmdb/mmdb.py

```diff
@@ -12,35 +12,35 @@
         self.server_address = "https://mmdb.piaqia.com/"
         self.package_path = os.path.split(os.path.realpath(__file__))[0]
         self.storage_path = os.path.join(self.package_path, "cache") if storage_path is None else storage_path
         self.mmdb_info = self.get_mmdb_info(self.server_address)
         os.makedirs(self.storage_path, exist_ok=True)
         
     def list_species(self):
-        return self.mmdb_info['Species'].unique()
+        print("Species: ", ', '.join(self.mmdb_info['Species'].unique()))
     
     def list_tissue(self):
-        return self.mmdb_info['Tissue'].unique()
+        print("Tissue: ", ', '.join(self.mmdb_info['Tissue'].unique()))
     
     def list_disease(self):
-        return self.mmdb_info['Disease'].unique()
+        print("Disease: ", ', '.join(self.mmdb_info['Disease'].unique()))
     
     def list_technology_type(self):
-        return self.mmdb_info['Technology_type'].unique()
+        print("Technology Type: ", ', '.join(self.mmdb_info['Technology_type'].unique()))
     
     def list_technology(self):
-        return self.mmdb_info['Technology'].unique()
+        print("Technology: ", ', '.join(self.mmdb_info['Technology'].unique()))
     
     def list_mmdb_info(self):
         print("MMDB Information: ")
-        print("Species: ", ', '.join(self.list_species()))
-        print("Tissue: ", ', '.join(self.list_tissue()))
-        print("Disease: ", ', '.join(self.list_disease()))
-        print("Technology: ", ', '.join(self.list_technology()))
-        print("Technology_type: ", ', '.join(self.list_technology_type()))
+        self.list_species()
+        self.list_tissue()
+        self.list_disease()
+        self.list_technology()
+        self.list_technology_type()
             
     def list_dataset(self, species=None, tissue=None, disease=None, technology_type=None):
         query = self.mmdb_info
         if species is not None: query = query[query['Species'] == species]
         if tissue is not None: query = query[query['Tissue'] == tissue]
         if disease is not None: query = query[query['Disease'] == disease]
         if technology_type is not None: query = query[query['Technology_type'] == technology_type]
```

## Comparing `pymmdb-1.0.4.dist-info/LICENSE` & `pymmdb-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymmdb-1.0.4.dist-info/METADATA` & `pymmdb-1.0.5.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymmdb
-Version: 1.0.4
+Version: 1.0.5
 Summary: scMMDB interface for python
 Home-page: https://mmdb.piaqia.com/
 Author: Jiawei Li
 Author-email: ljwstruggle@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pymmdb-1.0.4.dist-info/RECORD` & `pymmdb-1.0.5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 pymmdb/__init__.py,sha256=OeXfsopCWdqrMn2gElziZIj000Dc0RM0IZ1AlGcw5xM,22
-pymmdb/mmdb.py,sha256=oyrPb94qfAAgbMRCSZ_ka8rrvm_SXnIaUMpRPYHyZAk,6054
-pymmdb-1.0.4.dist-info/LICENSE,sha256=4CMNxQX_1_fpLFGl7T8cTzWclv5-YP0HsK6vK0HlMAM,11358
-pymmdb-1.0.4.dist-info/METADATA,sha256=IyD9dRiOyUHPl9MDcEiQ65Vaag6bFJadtiKDTIOsXUc,522
-pymmdb-1.0.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-pymmdb-1.0.4.dist-info/top_level.txt,sha256=H83lm-_ZXcxvsT4YLr_8Eg0mf6gcEmAUrPNrLzm5B6k,7
-pymmdb-1.0.4.dist-info/RECORD,,
+pymmdb/mmdb.py,sha256=Ng9eRTQnHgmH-n5GIpF_-BCouBjQ1qnvbuFoqWXT3mw,6019
+pymmdb-1.0.5.dist-info/LICENSE,sha256=4CMNxQX_1_fpLFGl7T8cTzWclv5-YP0HsK6vK0HlMAM,11358
+pymmdb-1.0.5.dist-info/METADATA,sha256=oBkjS8qK5JHwgSTwGDWMX9kCS0jkkBtejDTod8rn69U,522
+pymmdb-1.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pymmdb-1.0.5.dist-info/top_level.txt,sha256=H83lm-_ZXcxvsT4YLr_8Eg0mf6gcEmAUrPNrLzm5B6k,7
+pymmdb-1.0.5.dist-info/RECORD,,
```

