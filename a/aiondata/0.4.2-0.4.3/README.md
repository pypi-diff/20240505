# Comparing `tmp/aiondata-0.4.2.tar.gz` & `tmp/aiondata-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiondata-0.4.2.tar", max compression
+gzip compressed data, was "aiondata-0.4.3.tar", max compression
```

## Comparing `aiondata-0.4.2.tar` & `aiondata-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11372 2024-04-10 08:39:27.092199 aiondata-0.4.2/LICENSE
--rw-r--r--   0        0        0     4606 2024-04-10 08:39:27.092199 aiondata-0.4.2/README.md
--rw-r--r--   0        0        0      419 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/bindingdb.py
--rw-r--r--   0        0        0     2118 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/datasets.py
--rw-r--r--   0        0        0     4714 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/moleculenet.py
--rw-r--r--   0        0        0     8692 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/protein_structure.py
--rw-r--r--   0        0        0     5413 2024-04-10 08:39:27.092199 aiondata-0.4.2/aiondata/weizmann_ccca.py
--rw-r--r--   0        0        0     1505 2024-04-10 08:39:27.096199 aiondata-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11372 2024-05-05 08:08:35.202989 aiondata-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4606 2024-05-05 08:08:35.202989 aiondata-0.4.3/README.md
+-rw-r--r--   0        0        0      419 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/__init__.py
+-rw-r--r--   0        0        0     5289 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/bindingdb.py
+-rw-r--r--   0        0        0     2118 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/datasets.py
+-rw-r--r--   0        0        0     4714 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/moleculenet.py
+-rw-r--r--   0        0        0     8692 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/protein_structure.py
+-rw-r--r--   0        0        0     5413 2024-05-05 08:08:35.202989 aiondata-0.4.3/aiondata/weizmann_ccca.py
+-rw-r--r--   0        0        0     1505 2024-05-05 08:08:35.206989 aiondata-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 aiondata-0.4.3/PKG-INFO
```

### Comparing `aiondata-0.4.2/LICENSE` & `aiondata-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.2/README.md` & `aiondata-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.2/aiondata/bindingdb.py` & `aiondata-0.4.3/aiondata/bindingdb.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,20 +23,20 @@
         "IC50 (nM)",
         "Kd (nM)",
         "EC50 (nM)",
         "kon (M-1-s-1)",
         "koff (s-1)",
     }
 
-    def __init__(self, fd: Optional[io.BytesIO] = None):
+    def __init__(self, fd: Optional[io.BufferedReader] = None):
         """
         Initializes a BindingDB instance.
 
         Args:
-            fd (Optional[io.BytesIO]): The file-like object containing the dataset content.
+            fd (Optional[io.BufferedReader]): The file-like object containing the dataset content.
                 If `fd` is not provided, the dataset content will be fetched from the default source.
         """
         if fd is None:
             cached_sdf = self.get_cache_path().parent / "BindingDB.sdf.zip"
             if cached_sdf.exists():
                 self.fd = self.from_compressed_file(cached_sdf)
             else:
@@ -70,27 +70,27 @@
                     return float_value
             except ValueError:
                 return value
 
     @staticmethod
     def from_url(url: str) -> "BindingDB":
         """
-        Creates a BindingDB instance from a URL containing a compressed SDF file (typically upstream).
+        Creates a BindingDB instance from a URL containing a compressed SDF file, using streaming.
 
         Args:
             url (str): The URL of the dataset.
 
         Returns:
             A BindingDB instance.
         """
         with urllib.request.urlopen(url) as response:
             with zipfile.ZipFile(io.BytesIO(response.read())) as z:
                 sdf_name = z.namelist()[0]
                 with z.open(sdf_name) as sdf_file:
-                    sdf_content = io.BytesIO(sdf_file.read())
+                    sdf_content = io.BufferedReader(sdf_file)
         return BindingDB(sdf_content)
 
     @staticmethod
     def from_compressed_file(file_path: str) -> "BindingDB":
         """
         Creates a BindingDB instance from a compressed SDF file.
 
@@ -99,66 +99,65 @@
 
         Returns:
             A BindingDB instance.
         """
         with zipfile.ZipFile(file_path) as z:
             sdf_name = z.namelist()[0]
             with z.open(sdf_name) as sdf_file:
-                sdf_content = io.BytesIO(sdf_file.read())
+                sdf_content = io.BufferedReader(sdf_file)
         return BindingDB(sdf_content)
 
     @staticmethod
     def from_uncompressed_file(file_path: str) -> "BindingDB":
         """
         Creates a BindingDB instance from an uncompressed SDF file.
 
         Args:
             file_path (str): The path to the uncompressed file.
 
         Returns:
             A BindingDB instance.
         """
-        with open(file_path, "rb") as f:
-            file_content = io.BytesIO(f.read())
-        return BindingDB(file_content)
+        return BindingDB(open(file_path, "rb"))
 
     def to_generator(self, progress_bar: bool = True) -> Generator[dict, None, None]:
         """
         Converts the dataset to a generator.
 
         Args:
             progress_bar (bool): Whether to display a progress bar.
 
         Yields:
             dict: A dictionary representing a record in the dataset.
         """
         RDLogger.DisableLog("rdApp.*")  # Suppress RDKit warnings and errors
 
-        sd = Chem.ForwardSDMolSupplier(self.fd, sanitize=False, removeHs=False)
-
         if progress_bar:
             pb = tqdm
         else:
 
             def pb(x, **kwargs):
                 return x
 
-        for mol in pb(sd, desc="Parsing BindingDB", unit=" molecule"):
-            if mol is not None:
-                record = {
-                    prop: self._convert_to_numeric(prop, mol.GetProp(prop))
-                    for prop in mol.GetPropNames()
-                    if mol.HasProp(prop)
-                }
-
-                # Normalize PubChem SID and CID fields that are sometimes present in the SDF
-                if "PubChem SID" in record:
-                    record["PubChem SID of Ligand"] = record.pop("PubChem SID")
-                if "PubChem CID" in record:
-                    record["PubChem CID of Ligand"] = record.pop("PubChem CID")
+        with Chem.ForwardSDMolSupplier(self.fd, sanitize=True, removeHs=False) as sd:
+            for mol in pb(sd, desc="Parsing BindingDB", unit=" molecules"):
+                if mol is not None:
+                    record = {
+                        prop: self._convert_to_numeric(prop, mol.GetProp(prop))
+                        for prop in mol.GetPropNames()
+                        if mol.HasProp(prop)
+                    }
+
+                    # Normalize PubChem SID and CID fields that are sometimes present in the SDF
+                    if "PubChem SID" in record:
+                        record["PubChem SID of Ligand"] = record.pop("PubChem SID")
+                    if "PubChem CID" in record:
+                        record["PubChem CID of Ligand"] = record.pop("PubChem CID")
 
-                record["SMILES"] = Chem.MolToSmiles(mol)
-                yield record
+                    record["SMILES"] = Chem.MolToSmiles(mol)
+                    yield record
+                else:
+                    break
 
         # Re-enable logging
         RDLogger.EnableLog("rdApp.error")
         RDLogger.EnableLog("rdApp.warning")
```

### Comparing `aiondata-0.4.2/aiondata/datasets.py` & `aiondata-0.4.3/aiondata/datasets.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.2/aiondata/moleculenet.py` & `aiondata-0.4.3/aiondata/moleculenet.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.2/aiondata/protein_structure.py` & `aiondata-0.4.3/aiondata/protein_structure.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.2/aiondata/weizmann_ccca.py` & `aiondata-0.4.3/aiondata/weizmann_ccca.py`

 * *Files identical despite different names*

### Comparing `aiondata-0.4.2/pyproject.toml` & `aiondata-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiondata"
-version = "0.4.2"
+version = "0.4.3"
 description = "A common data access layer for AI-driven drug discovery."
 authors = ["JJ Ben-Joseph <jj@tensorspace.ai>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://www.github.com/aion-labs/aiondata"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `aiondata-0.4.2/PKG-INFO` & `aiondata-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiondata
-Version: 0.4.2
+Version: 0.4.3
 Summary: A common data access layer for AI-driven drug discovery.
 Home-page: https://www.github.com/aion-labs/aiondata
 License: Apache
 Author: JJ Ben-Joseph
 Author-email: jj@tensorspace.ai
 Requires-Python: >=3.10
 Classifier: Development Status :: 3 - Alpha
```

