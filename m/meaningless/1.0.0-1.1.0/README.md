# Comparing `tmp/meaningless-1.0.0.tar.gz` & `tmp/meaningless-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meaningless-1.0.0.tar", last modified: Fri Mar 17 06:55:43 2023, max compression
+gzip compressed data, was "meaningless-1.1.0.tar", last modified: Wed Apr 24 19:16:59 2024, max compression
```

## Comparing `meaningless-1.0.0.tar` & `meaningless-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 06:55:40.000000 meaningless-1.0.0/
--rw-rw-rw-   0        0        0     2630 2023-02-22 09:52:10.000000 meaningless-1.0.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1089 2022-03-10 06:43:02.000000 meaningless-1.0.0/LICENSE.md
--rw-rw-rw-   0        0        0    23633 2023-03-17 06:55:44.000000 meaningless-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    18755 2023-02-22 09:50:22.000000 meaningless-1.0.0/README.md
--rw-rw-rw-   0        0        0      137 2023-02-27 08:51:42.000000 meaningless-1.0.0/REQUIREMENTS.txt
-drwxrwxrwx   0        0        0        0 2023-03-17 06:55:40.000000 meaningless-1.0.0/meaningless/
--rw-rw-rw-   0        0        0     1468 2023-01-25 20:22:26.000000 meaningless-1.0.0/meaningless/__init__.py
--rw-rw-rw-   0        0        0    24096 2023-02-24 04:34:44.000000 meaningless-1.0.0/meaningless/bible_base_downloader.py
--rw-rw-rw-   0        0        0    28274 2023-01-25 21:50:54.000000 meaningless-1.0.0/meaningless/bible_base_extractor.py
--rw-rw-rw-   0        0        0      753 2022-03-10 06:43:06.000000 meaningless-1.0.0/meaningless/bible_csv_downloader.py
--rw-rw-rw-   0        0        0      768 2022-03-10 06:43:06.000000 meaningless-1.0.0/meaningless/bible_csv_extractor.py
--rw-rw-rw-   0        0        0      758 2021-10-01 08:02:46.000000 meaningless-1.0.0/meaningless/bible_json_downloader.py
--rw-rw-rw-   0        0        0      773 2021-10-01 08:02:46.000000 meaningless-1.0.0/meaningless/bible_json_extractor.py
--rw-rw-rw-   0        0        0    20936 2023-03-03 08:48:40.000000 meaningless-1.0.0/meaningless/bible_web_extractor.py
--rw-rw-rw-   0        0        0      752 2023-01-25 20:27:56.000000 meaningless-1.0.0/meaningless/bible_xml_downloader.py
--rw-rw-rw-   0        0        0      769 2023-01-25 20:27:56.000000 meaningless-1.0.0/meaningless/bible_xml_extractor.py
--rw-rw-rw-   0        0        0      757 2021-10-01 08:02:46.000000 meaningless-1.0.0/meaningless/bible_yaml_downloader.py
--rw-rw-rw-   0        0        0      774 2021-10-01 08:02:46.000000 meaningless-1.0.0/meaningless/bible_yaml_extractor.py
-drwxrwxrwx   0        0        0        0 2023-03-17 06:55:42.000000 meaningless-1.0.0/meaningless/utilities/
--rw-rw-rw-   0        0        0      347 2023-01-25 20:22:42.000000 meaningless-1.0.0/meaningless/utilities/__init__.py
--rw-rw-rw-   0        0        0    20038 2023-03-10 10:38:24.000000 meaningless-1.0.0/meaningless/utilities/common.py
--rw-rw-rw-   0        0        0     4581 2023-01-25 20:03:40.000000 meaningless-1.0.0/meaningless/utilities/csv_file_interface.py
--rw-rw-rw-   0        0        0     3442 2023-01-25 21:50:56.000000 meaningless-1.0.0/meaningless/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1579 2022-09-09 08:42:42.000000 meaningless-1.0.0/meaningless/utilities/json_file_interface.py
--rw-rw-rw-   0        0        0     9004 2023-01-25 21:50:52.000000 meaningless-1.0.0/meaningless/utilities/xml_file_interface.py
--rw-rw-rw-   0        0        0     1675 2021-01-06 07:52:14.000000 meaningless-1.0.0/meaningless/utilities/yaml_file_interface.py
-drwxrwxrwx   0        0        0        0 2023-03-17 06:55:42.000000 meaningless-1.0.0/meaningless.egg-info/
--rw-rw-rw-   0        0        0    23633 2023-03-17 06:55:40.000000 meaningless-1.0.0/meaningless.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      939 2023-03-17 06:55:40.000000 meaningless-1.0.0/meaningless.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 06:55:40.000000 meaningless-1.0.0/meaningless.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-03-17 06:55:40.000000 meaningless-1.0.0/meaningless.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-17 06:55:40.000000 meaningless-1.0.0/meaningless.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1446 2023-03-05 07:40:24.000000 meaningless-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-17 06:55:44.000000 meaningless-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 19:16:54.000000 meaningless-1.1.0/
+-rw-rw-rw-   0        0        0     2938 2024-04-24 10:51:56.000000 meaningless-1.1.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1089 2022-03-10 07:43:02.000000 meaningless-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0    24117 2024-04-24 19:17:00.000000 meaningless-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    18755 2023-03-17 08:01:20.000000 meaningless-1.1.0/README.md
+-rw-rw-rw-   0        0        0      137 2023-03-17 08:01:20.000000 meaningless-1.1.0/REQUIREMENTS.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 19:16:54.000000 meaningless-1.1.0/meaningless/
+-rw-rw-rw-   0        0        0     1468 2023-03-17 08:01:26.000000 meaningless-1.1.0/meaningless/__init__.py
+-rw-rw-rw-   0        0        0    24096 2023-03-17 08:01:26.000000 meaningless-1.1.0/meaningless/bible_base_downloader.py
+-rw-rw-rw-   0        0        0    28274 2023-03-17 08:01:26.000000 meaningless-1.1.0/meaningless/bible_base_extractor.py
+-rw-rw-rw-   0        0        0      753 2022-03-10 07:43:06.000000 meaningless-1.1.0/meaningless/bible_csv_downloader.py
+-rw-rw-rw-   0        0        0      768 2022-03-10 07:43:06.000000 meaningless-1.1.0/meaningless/bible_csv_extractor.py
+-rw-rw-rw-   0        0        0      758 2021-10-01 09:02:46.000000 meaningless-1.1.0/meaningless/bible_json_downloader.py
+-rw-rw-rw-   0        0        0      773 2021-10-01 09:02:46.000000 meaningless-1.1.0/meaningless/bible_json_extractor.py
+-rw-rw-rw-   0        0        0    21014 2024-01-28 03:38:14.000000 meaningless-1.1.0/meaningless/bible_web_extractor.py
+-rw-rw-rw-   0        0        0      752 2023-03-17 08:01:28.000000 meaningless-1.1.0/meaningless/bible_xml_downloader.py
+-rw-rw-rw-   0        0        0      769 2023-03-17 08:01:28.000000 meaningless-1.1.0/meaningless/bible_xml_extractor.py
+-rw-rw-rw-   0        0        0      757 2021-10-01 09:02:46.000000 meaningless-1.1.0/meaningless/bible_yaml_downloader.py
+-rw-rw-rw-   0        0        0      774 2021-10-01 09:02:46.000000 meaningless-1.1.0/meaningless/bible_yaml_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-24 19:16:54.000000 meaningless-1.1.0/meaningless/utilities/
+-rw-rw-rw-   0        0        0      347 2023-03-17 08:01:28.000000 meaningless-1.1.0/meaningless/utilities/__init__.py
+-rw-rw-rw-   0        0        0    20038 2024-03-17 09:21:14.000000 meaningless-1.1.0/meaningless/utilities/common.py
+-rw-rw-rw-   0        0        0     4581 2023-01-25 21:03:40.000000 meaningless-1.1.0/meaningless/utilities/csv_file_interface.py
+-rw-rw-rw-   0        0        0     3442 2023-03-17 08:01:28.000000 meaningless-1.1.0/meaningless/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1579 2022-09-09 09:42:42.000000 meaningless-1.1.0/meaningless/utilities/json_file_interface.py
+-rw-rw-rw-   0        0        0     9004 2023-03-17 08:01:28.000000 meaningless-1.1.0/meaningless/utilities/xml_file_interface.py
+-rw-rw-rw-   0        0        0     1675 2021-01-06 08:52:14.000000 meaningless-1.1.0/meaningless/utilities/yaml_file_interface.py
+drwxrwxrwx   0        0        0        0 2024-04-24 19:16:54.000000 meaningless-1.1.0/meaningless.egg-info/
+-rw-rw-rw-   0        0        0    24117 2024-04-24 19:16:52.000000 meaningless-1.1.0/meaningless.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      939 2024-04-24 19:16:52.000000 meaningless-1.1.0/meaningless.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 19:16:52.000000 meaningless-1.1.0/meaningless.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-24 19:16:52.000000 meaningless-1.1.0/meaningless.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 19:16:52.000000 meaningless-1.1.0/meaningless.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1505 2024-01-27 09:15:38.000000 meaningless-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 19:17:00.000000 meaningless-1.1.0/setup.cfg
```

### Comparing `meaningless-1.0.0/CHANGELOG.md` & `meaningless-1.1.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Change Log
 
+## 1.1.0
+- Fixed an issue where `get_passage_range` in the Web Extractor would incorrectly cap the upper limit of passages to 100
+- Drop library support for Python 3.8
+- Python version support now extends to the 4 earliest versions (subject to its EOL date) which are at least receiving security fixes
+
 ## 1.0.0
 - Removed legacy_xml_file_interface module and the `use_legacy_mode` flag in the XML Downloader and Extractor
 - Added experimental Apocrypha Web Extractor for the NRSVUE translation
 - Added translation support for: NMB
 
 ## 0.7.0
 - Refined xml_file_interface to use a more standard XML document structure with easier integration with XSLT
```

### Comparing `meaningless-1.0.0/LICENSE.md` & `meaningless-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/PKG-INFO` & `meaningless-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meaningless
-Version: 1.0.0
+Version: 1.1.0
 Summary: Retrieves, processes and downloads Bible passages from Bible Gateway
 Author-email: Daniel Tran <dantran.au@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Daniel Tran
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,28 +24,32 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/daniel-tran/meaningless
 Project-URL: Documentation, https://daniel-tran.github.io/meaningless
 Keywords: bible,yaml,json,xml,csv,biblegateway
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Religion
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Religion
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: beautifulsoup4>=4.11.2
+Requires-Dist: ruamel.yaml>=0.17.21
+Requires-Dist: xmltodict>=0.13.0
 
 [![Test Status](https://github.com/daniel-tran/meaningless/actions/workflows/run_tests.yaml/badge.svg)](https://github.com/daniel-tran/meaningless/actions/workflows/run_tests.yaml)
 
 Meaningless is a Python library used to retrieve, process and download Bible passages from Bible Gateway.
 
 Features include:
 - Passage retrieval from the [Bible Gateway](https://www.biblegateway.com) site or from a local YAML/JSON/XML/CSV file.
@@ -540,14 +544,19 @@
 
 # Disclaimer
 
 This library is not endorsed by nor affiliated with Bible Gateway or any of its partners.
 
 # Change Log
 
+## 1.1.0
+- Fixed an issue where `get_passage_range` in the Web Extractor would incorrectly cap the upper limit of passages to 100
+- Drop library support for Python 3.8
+- Python version support now extends to the 4 earliest versions (subject to its EOL date) which are at least receiving security fixes
+
 ## 1.0.0
 - Removed legacy_xml_file_interface module and the `use_legacy_mode` flag in the XML Downloader and Extractor
 - Added experimental Apocrypha Web Extractor for the NRSVUE translation
 - Added translation support for: NMB
 
 ## 0.7.0
 - Refined xml_file_interface to use a more standard XML document structure with easier integration with XSLT
```

### Comparing `meaningless-1.0.0/README.md` & `meaningless-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/__init__.py` & `meaningless-1.1.0/meaningless/__init__.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/bible_base_downloader.py` & `meaningless-1.1.0/meaningless/bible_base_downloader.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/bible_base_extractor.py` & `meaningless-1.1.0/meaningless/bible_base_extractor.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/bible_csv_downloader.py` & `meaningless-1.1.0/meaningless/bible_csv_downloader.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/bible_csv_extractor.py` & `meaningless-1.1.0/meaningless/bible_csv_extractor.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/bible_json_downloader.py` & `meaningless-1.1.0/meaningless/bible_json_downloader.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/bible_json_extractor.py` & `meaningless-1.1.0/meaningless/bible_json_extractor.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/bible_web_extractor.py` & `meaningless-1.1.0/meaningless/bible_web_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,18 +139,18 @@
         :return: All passages between the specified passages (inclusive). Empty string/list if the passage is invalid.
         :rtype: str or list
         """
         # Capping the chapter and passage information, as this gets included in site search string and can cause
         # the web request to stagger if this manages to be long enough.
         capped_chapter_from = common.get_capped_integer(chapter_from,
                                                         max_value=common.get_chapter_count(book, self.translation))
-        capped_passage_from = common.get_capped_integer(passage_from)
+        capped_passage_from = common.get_capped_integer(passage_from, max_value=common.get_end_of_chapter())
         capped_chapter_to = common.get_capped_integer(chapter_to,
                                                       max_value=common.get_chapter_count(book, self.translation))
-        capped_passage_to = common.get_capped_integer(passage_to)
+        capped_passage_to = common.get_capped_integer(passage_to, max_value=common.get_end_of_chapter())
         # Defer to a direct search invocation when sourcing passages from the same chapter
         if capped_chapter_from == capped_chapter_to:
             return self.search(f'{book} {capped_chapter_from}:{capped_passage_from} - {capped_passage_to}')
 
         # Get the partial section of the first chapter being requested, omitting some initial passages
         initial_chapter = self.get_passages(book, capped_chapter_from, capped_passage_from, common.get_end_of_chapter())
         # Get the partial section of the last chapter being requested, omitting some trailing passages
```

### Comparing `meaningless-1.0.0/meaningless/bible_xml_downloader.py` & `meaningless-1.1.0/meaningless/bible_xml_downloader.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/bible_xml_extractor.py` & `meaningless-1.1.0/meaningless/bible_xml_extractor.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/bible_yaml_downloader.py` & `meaningless-1.1.0/meaningless/bible_yaml_downloader.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/bible_yaml_extractor.py` & `meaningless-1.1.0/meaningless/bible_yaml_extractor.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/utilities/common.py` & `meaningless-1.1.0/meaningless/utilities/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from urllib.request import urlopen
 from urllib.error import URLError
 from time import sleep
 import re
 
 # This is a collection of helper methods used across the various modules.
 
-MEANINGLESS_VERSION = '1.0.0'
+MEANINGLESS_VERSION = '1.1.0'
 '''
 The current version of the Meaningless library.
 '''
 
 
 def is_unsupported_translation(translation):
     """
```

### Comparing `meaningless-1.0.0/meaningless/utilities/csv_file_interface.py` & `meaningless-1.1.0/meaningless/utilities/csv_file_interface.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/utilities/exceptions.py` & `meaningless-1.1.0/meaningless/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/utilities/json_file_interface.py` & `meaningless-1.1.0/meaningless/utilities/json_file_interface.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/utilities/xml_file_interface.py` & `meaningless-1.1.0/meaningless/utilities/xml_file_interface.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless/utilities/yaml_file_interface.py` & `meaningless-1.1.0/meaningless/utilities/yaml_file_interface.py`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/meaningless.egg-info/PKG-INFO` & `meaningless-1.1.0/meaningless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meaningless
-Version: 1.0.0
+Version: 1.1.0
 Summary: Retrieves, processes and downloads Bible passages from Bible Gateway
 Author-email: Daniel Tran <dantran.au@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Daniel Tran
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,28 +24,32 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/daniel-tran/meaningless
 Project-URL: Documentation, https://daniel-tran.github.io/meaningless
 Keywords: bible,yaml,json,xml,csv,biblegateway
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Religion
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Religion
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: beautifulsoup4>=4.11.2
+Requires-Dist: ruamel.yaml>=0.17.21
+Requires-Dist: xmltodict>=0.13.0
 
 [![Test Status](https://github.com/daniel-tran/meaningless/actions/workflows/run_tests.yaml/badge.svg)](https://github.com/daniel-tran/meaningless/actions/workflows/run_tests.yaml)
 
 Meaningless is a Python library used to retrieve, process and download Bible passages from Bible Gateway.
 
 Features include:
 - Passage retrieval from the [Bible Gateway](https://www.biblegateway.com) site or from a local YAML/JSON/XML/CSV file.
@@ -540,14 +544,19 @@
 
 # Disclaimer
 
 This library is not endorsed by nor affiliated with Bible Gateway or any of its partners.
 
 # Change Log
 
+## 1.1.0
+- Fixed an issue where `get_passage_range` in the Web Extractor would incorrectly cap the upper limit of passages to 100
+- Drop library support for Python 3.8
+- Python version support now extends to the 4 earliest versions (subject to its EOL date) which are at least receiving security fixes
+
 ## 1.0.0
 - Removed legacy_xml_file_interface module and the `use_legacy_mode` flag in the XML Downloader and Extractor
 - Added experimental Apocrypha Web Extractor for the NRSVUE translation
 - Added translation support for: NMB
 
 ## 0.7.0
 - Refined xml_file_interface to use a more standard XML document structure with easier integration with XSLT
```

### Comparing `meaningless-1.0.0/meaningless.egg-info/SOURCES.txt` & `meaningless-1.1.0/meaningless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meaningless-1.0.0/pyproject.toml` & `meaningless-1.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 authors = [
   {name = 'Daniel Tran', email = 'dantran.au@gmail.com'}
 ]
 description = 'Retrieves, processes and downloads Bible passages from Bible Gateway'
 license.file = 'LICENSE.md'
 keywords = ['bible', 'yaml', 'json', 'xml', 'csv', 'biblegateway']
 classifiers = [
-  'Development Status :: 4 - Beta',
+  'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Religion',
   'Intended Audience :: Developers',
   'License :: OSI Approved :: MIT License',
   'Natural Language :: English',
   'Operating System :: Microsoft :: Windows',
   'Operating System :: POSIX :: Linux',
-  'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
+  'Programming Language :: Python :: 3.11',
+  'Programming Language :: Python :: 3.12',
   'Topic :: Religion'
 ]
-requires-python = '>=3.8'
+requires-python = '>=3.9'
 
 [project.urls]
 'Homepage' = 'https://github.com/daniel-tran/meaningless'
 'Documentation' = 'https://daniel-tran.github.io/meaningless'
 
 [tool.setuptools]
 # This disables module auto discovery, since some top-level folders are not supposed to be packaged
```

