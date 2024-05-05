# Comparing `tmp/beanhub_extract-0.0.3.tar.gz` & `tmp/beanhub_extract-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_extract-0.0.3.tar", max compression
+gzip compressed data, was "beanhub_extract-0.0.4.tar", max compression
```

## Comparing `beanhub_extract-0.0.3.tar` & `beanhub_extract-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/LICENSE
--rw-r--r--   0        0        0      165 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/beanhub_extract/__init__.py
--rw-r--r--   0        0        0     1502 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/beanhub_extract/data_types.py
--rw-r--r--   0        0        0      115 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/beanhub_extract/extractors/__init__.py
--rw-r--r--   0        0        0     1774 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/beanhub_extract/extractors/mercury.py
--rw-r--r--   0        0        0      977 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/beanhub_extract/utils.py
--rw-r--r--   0        0        0      578 2024-05-05 06:34:17.640603 beanhub_extract-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 beanhub_extract-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-05 19:10:11.535802 beanhub_extract-0.0.4/LICENSE
+-rw-r--r--   0        0        0      165 2024-05-05 19:10:11.535802 beanhub_extract-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 19:10:11.535802 beanhub_extract-0.0.4/beanhub_extract/__init__.py
+-rw-r--r--   0        0        0     1655 2024-05-05 19:10:11.535802 beanhub_extract-0.0.4/beanhub_extract/data_types.py
+-rw-r--r--   0        0        0      115 2024-05-05 19:10:11.535802 beanhub_extract-0.0.4/beanhub_extract/extractors/__init__.py
+-rw-r--r--   0        0        0     2008 2024-05-05 19:10:11.535802 beanhub_extract-0.0.4/beanhub_extract/extractors/mercury.py
+-rw-r--r--   0        0        0      977 2024-05-05 19:10:11.535802 beanhub_extract-0.0.4/beanhub_extract/utils.py
+-rw-r--r--   0        0        0      578 2024-05-05 19:10:11.535802 beanhub_extract-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 beanhub_extract-0.0.4/PKG-INFO
```

### Comparing `beanhub_extract-0.0.3/LICENSE` & `beanhub_extract-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.3/beanhub_extract/data_types.py` & `beanhub_extract-0.0.4/beanhub_extract/data_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 @dataclasses.dataclass(frozen=True)
 class Transaction:
     extractor: str
     # the filename of import source
     file: str | None = None
     # the entry line number of the source file
     lineno: int | None = None
+    # the entry line number of the source file in reverse order. comes handy for CSV files in desc datetime order
+    reversed_lineno: int | None = None
     # date of the transaction
     date: datetime.date | None = None
     # date when the transaction posted
     post_date: datetime.date | None = None
     # timestamp of the transaction
     timestamp: datetime.datetime | None = None
     # timezone of the transaction, needs to be one of timezone value supported by pytz
```

### Comparing `beanhub_extract-0.0.3/beanhub_extract/extractors/mercury.py` & `beanhub_extract-0.0.4/beanhub_extract/extractors/mercury.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,29 +23,33 @@
     date = parse_date(parts[0])
     time = parse_time(parts[1])
     return datetime.datetime.combine(date, time)
 
 
 class MercuryExtractor:
     EXTRACTOR_NAME = "mercury"
+    DEFAULT_IMPORT_ID = "{{ file }}:{{ reversed_lineno }}"
 
     def __init__(self, input_file: typing.TextIO):
         self.input_file = input_file
 
     def __call__(self) -> typing.Generator[Transaction, None, None]:
         filename = None
         if hasattr(self.input_file, "name"):
             filename = self.input_file.name
         reader = csv.DictReader(self.input_file)
+        # this consumes quite some memory, but it should be fine assume most csv dump files are small
+        rows = list(reader)
         timezone = pytz.UTC
-        for i, row in enumerate(reader):
+        for i, row in enumerate(rows):
             yield Transaction(
                 extractor=self.EXTRACTOR_NAME,
                 file=filename,
                 lineno=i + 1,
+                reversed_lineno=len(rows) - i,
                 date=parse_date(row["Date (UTC)"]),
                 desc=row["Description"],
                 amount=decimal.Decimal(row["Amount"]),
                 status=row["Status"],
                 source_account=row["Source Account"],
                 bank_desc=row["Bank Description"],
                 reference=row["Reference"],
```

### Comparing `beanhub_extract-0.0.3/beanhub_extract/utils.py` & `beanhub_extract-0.0.4/beanhub_extract/utils.py`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.3/pyproject.toml` & `beanhub_extract-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-extract"
-version = "0.0.3"
+version = "0.0.4"
 description = "The simple library for extracting all kind of bank account transaction export files, mostly for beanhub-import to inject and generate transactions"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `beanhub_extract-0.0.3/PKG-INFO` & `beanhub_extract-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-extract
-Version: 0.0.3
+Version: 0.0.4
 Summary: The simple library for extracting all kind of bank account transaction export files, mostly for beanhub-import to inject and generate transactions
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

