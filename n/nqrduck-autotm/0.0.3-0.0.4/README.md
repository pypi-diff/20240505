# Comparing `tmp/nqrduck_autotm-0.0.3.tar.gz` & `tmp/nqrduck_autotm-0.0.4.tar.gz`

## Comparing `nqrduck_autotm-0.0.3.tar` & `nqrduck_autotm-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   637712 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/docs/img/autotm-labeled.png
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/src/nqrduck_autotm/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/src/nqrduck_autotm/autotm.py
--rw-r--r--   0        0        0    49927 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/src/nqrduck_autotm/controller.py
--rw-r--r--   0        0        0    19934 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/src/nqrduck_autotm/model.py
--rw-r--r--   0        0        0    36465 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/src/nqrduck_autotm/view.py
--rw-r--r--   0        0        0    20632 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/src/nqrduck_autotm/widget.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/src/nqrduck_autotm/resources/AutoTM.ini
--rw-r--r--   0        0        0    17613 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/src/nqrduck_autotm/resources/autotm_widget.ui
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/LICENSE
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/README.md
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   637712 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/docs/img/autotm-labeled.png
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/src/nqrduck_autotm/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/src/nqrduck_autotm/autotm.py
+-rw-r--r--   0        0        0    49927 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/src/nqrduck_autotm/controller.py
+-rw-r--r--   0        0        0    19934 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/src/nqrduck_autotm/model.py
+-rw-r--r--   0        0        0    36463 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/src/nqrduck_autotm/view.py
+-rw-r--r--   0        0        0    20632 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/src/nqrduck_autotm/widget.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/src/nqrduck_autotm/resources/AutoTM.ini
+-rw-r--r--   0        0        0    17613 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/src/nqrduck_autotm/resources/autotm_widget.ui
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/README.md
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 nqrduck_autotm-0.0.4/PKG-INFO
```

### Comparing `nqrduck_autotm-0.0.3/.github/workflows/python-publish.yml` & `nqrduck_autotm-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_autotm-0.0.3/docs/img/autotm-labeled.png` & `nqrduck_autotm-0.0.4/docs/img/autotm-labeled.png`

 * *Files identical despite different names*

### Comparing `nqrduck_autotm-0.0.3/src/nqrduck_autotm/controller.py` & `nqrduck_autotm-0.0.4/src/nqrduck_autotm/controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck_autotm-0.0.3/src/nqrduck_autotm/model.py` & `nqrduck_autotm-0.0.4/src/nqrduck_autotm/model.py`

 * *Files identical despite different names*

### Comparing `nqrduck_autotm-0.0.3/src/nqrduck_autotm/view.py` & `nqrduck_autotm-0.0.4/src/nqrduck_autotm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,24 +398,24 @@
         self.lut_window = self.LutWindow(self.module)
         self.lut_window.show()
 
     @pyqtSlot()
     def on_export_button_clicked(self) -> None:
         """Slot for when the export button is clicked."""
         logger.debug("Export button clicked")
-        file_manager = self.QFileManager(S11Data.FILE_EXTENSION, parent=self.widget)
+        file_manager = self.FileManager(S11Data.FILE_EXTENSION, parent=self.widget)
         file_name = file_manager.saveFileDialog()
         if file_name:
             self.module.controller.save_measurement(file_name)
 
     @pyqtSlot()
     def on_import_button_clicked(self) -> None:
         """Slot for when the import button is clicked."""
         logger.debug("Import button clicked")
-        file_manager = self.QFileManager(S11Data.FILE_EXTENSION, parent=self.widget)
+        file_manager = self.FileManager(S11Data.FILE_EXTENSION, parent=self.widget)
         file_name = file_manager.loadFileDialog()
         if file_name:
             self.module.controller.load_measurement(file_name)
 
     class StepperSavedPositionsWindow(QDialog):
         def __init__(self, module, parent=None):
             super().__init__(parent)
```

### Comparing `nqrduck_autotm-0.0.3/src/nqrduck_autotm/widget.py` & `nqrduck_autotm-0.0.4/src/nqrduck_autotm/widget.py`

 * *Files identical despite different names*

### Comparing `nqrduck_autotm-0.0.3/src/nqrduck_autotm/resources/autotm_widget.ui` & `nqrduck_autotm-0.0.4/src/nqrduck_autotm/resources/autotm_widget.ui`

 * *Files identical despite different names*

### Comparing `nqrduck_autotm-0.0.3/LICENSE` & `nqrduck_autotm-0.0.4/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Julia Pfitzer
+Copyright (c) 2023 jupfi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `nqrduck_autotm-0.0.3/README.md` & `nqrduck_autotm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_autotm-0.0.3/pyproject.toml` & `nqrduck_autotm-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nqrduck-autotm"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A module for the NQRduck program (a simple python script™) for automatic Tuning and Matching (TM) system used for magnetic resonance spectroscopy."
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `nqrduck_autotm-0.0.3/PKG-INFO` & `nqrduck_autotm-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: nqrduck-autotm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A module for the NQRduck program (a simple python script™) for automatic Tuning and Matching (TM) system used for magnetic resonance spectroscopy.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-autotm/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-autotm
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
         
-        Copyright (c) 2023 Julia Pfitzer
+        Copyright (c) 2023 jupfi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -27,15 +27,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: matplotlib
 Requires-Dist: nqrduck
 Requires-Dist: pyqt6
 Requires-Dist: pyserial
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
```

