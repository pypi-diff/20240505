# Comparing `tmp/beanhub_extract-0.0.1.tar.gz` & `tmp/beanhub_extract-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_extract-0.0.1.tar", max compression
+gzip compressed data, was "beanhub_extract-0.0.2.tar", max compression
```

## Comparing `beanhub_extract-0.0.1.tar` & `beanhub_extract-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-04 19:12:34.862865 beanhub_extract-0.0.1/LICENSE
--rw-r--r--   0        0        0      165 2024-05-04 19:12:34.862865 beanhub_extract-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-04 19:15:18.172840 beanhub_extract-0.0.1/beanhub_extract/__init__.py
--rw-r--r--   0        0        0     1546 2024-05-04 23:20:03.664905 beanhub_extract-0.0.1/beanhub_extract/data_types.py
--rw-r--r--   0        0        0        0 2024-05-04 21:40:07.754964 beanhub_extract-0.0.1/beanhub_extract/extractors/__init__.py
--rw-r--r--   0        0        0     1774 2024-05-05 00:05:16.096929 beanhub_extract-0.0.1/beanhub_extract/extractors/mercury.py
--rw-r--r--   0        0        0     1011 2024-05-05 00:02:00.491322 beanhub_extract-0.0.1/beanhub_extract/utils.py
--rw-r--r--   0        0        0      617 2024-05-04 23:25:49.359077 beanhub_extract-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 beanhub_extract-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/LICENSE
+-rw-r--r--   0        0        0      165 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/beanhub_extract/__init__.py
+-rw-r--r--   0        0        0     1502 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/beanhub_extract/data_types.py
+-rw-r--r--   0        0        0        0 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/beanhub_extract/extractors/__init__.py
+-rw-r--r--   0        0        0     1774 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/beanhub_extract/extractors/mercury.py
+-rw-r--r--   0        0        0      977 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/beanhub_extract/utils.py
+-rw-r--r--   0        0        0      595 2024-05-05 00:26:26.608346 beanhub_extract-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 beanhub_extract-0.0.2/PKG-INFO
```

### Comparing `beanhub_extract-0.0.1/LICENSE` & `beanhub_extract-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.1/beanhub_extract/data_types.py` & `beanhub_extract-0.0.2/beanhub_extract/data_types.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import dataclasses
-import datetime
-import decimal
-
-
-@dataclasses.dataclass(frozen=True)
-class Transaction:
-    extractor: str
-    # the filename of import source
-    file: str | None = None
-    # the entry line number of the source file
-    lineno: int | None = None
-    # date of the transaction
-    date: datetime.date | None = None
-    # date when the transaction posted
-    post_date: datetime.date | None = None
-    # timestamp of the transaction
-    timestamp: datetime.datetime | None = None
-    # timezone of the transaction, needs to be one of timezone value supported by pytz
-    timezone: str | None = None
-    # description of the transaction
-    desc: str | None = None
-    # description of the transaction provided by the bank
-    bank_desc: str | None = None
-    # transaction amount
-    amount: decimal.Decimal | None = None
-    # ISO 4217 currency symbol
-    currency: str | None = None
-    # category of the transaction, like Entertainment, Shopping, etc..
-    category: str | None = None
-    # status of the transaction
-    status: str | None = None
-    # type of the transaction, such as Sale, Return, Debit, etc
-    type: str | None = None
-    # Source account of the transaction
-    source_account: str | None = None
-    # destination account of the transaction
-    dest_account: str | None = None
-    # note or memo for the transaction
-    note: str | None = None
-    # Reference value
-    reference: str | None = None
-    # Payee of the transaction
-    payee: str | None = None
+import dataclasses
+import datetime
+import decimal
+
+
+@dataclasses.dataclass(frozen=True)
+class Transaction:
+    extractor: str
+    # the filename of import source
+    file: str | None = None
+    # the entry line number of the source file
+    lineno: int | None = None
+    # date of the transaction
+    date: datetime.date | None = None
+    # date when the transaction posted
+    post_date: datetime.date | None = None
+    # timestamp of the transaction
+    timestamp: datetime.datetime | None = None
+    # timezone of the transaction, needs to be one of timezone value supported by pytz
+    timezone: str | None = None
+    # description of the transaction
+    desc: str | None = None
+    # description of the transaction provided by the bank
+    bank_desc: str | None = None
+    # transaction amount
+    amount: decimal.Decimal | None = None
+    # ISO 4217 currency symbol
+    currency: str | None = None
+    # category of the transaction, like Entertainment, Shopping, etc..
+    category: str | None = None
+    # status of the transaction
+    status: str | None = None
+    # type of the transaction, such as Sale, Return, Debit, etc
+    type: str | None = None
+    # Source account of the transaction
+    source_account: str | None = None
+    # destination account of the transaction
+    dest_account: str | None = None
+    # note or memo for the transaction
+    note: str | None = None
+    # Reference value
+    reference: str | None = None
+    # Payee of the transaction
+    payee: str | None = None
```

### Comparing `beanhub_extract-0.0.1/beanhub_extract/extractors/mercury.py` & `beanhub_extract-0.0.2/beanhub_extract/extractors/mercury.py`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.1/beanhub_extract/utils.py` & `beanhub_extract-0.0.2/beanhub_extract/utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import dataclasses
-import pathlib
-
-from .data_types import Transaction
-
-
-def strip_base_path(
-    base: pathlib.Path | pathlib.PurePath,
-    filepath: str | pathlib.Path | pathlib.PurePath,
-    pure_posix: bool = False,
-) -> str:
-    """Strip file base path (parent folder) from given file path"""
-    if not isinstance(filepath, pathlib.Path):
-        if pure_posix:
-            filepath = pathlib.PurePosixPath(filepath)
-        else:
-            filepath = pathlib.Path(filepath)
-    return str(filepath.relative_to(base))
-
-
-def strip_txn_base_path(
-    base: pathlib.Path | pathlib.PurePath,
-    transaction: Transaction,
-    pure_posix: bool = False,
-) -> Transaction:
-    """Strip file base path (parent folder) from given transaction"""
-    if transaction.file is None:
-        return transaction
-    return Transaction(
-        **(
-            dataclasses.asdict(transaction)
-            | dict(file=strip_base_path(base, transaction.file, pure_posix))
-        )
-    )
+import dataclasses
+import pathlib
+
+from .data_types import Transaction
+
+
+def strip_base_path(
+    base: pathlib.Path | pathlib.PurePath,
+    filepath: str | pathlib.Path | pathlib.PurePath,
+    pure_posix: bool = False,
+) -> str:
+    """Strip file base path (parent folder) from given file path"""
+    if not isinstance(filepath, pathlib.Path):
+        if pure_posix:
+            filepath = pathlib.PurePosixPath(filepath)
+        else:
+            filepath = pathlib.Path(filepath)
+    return str(filepath.relative_to(base))
+
+
+def strip_txn_base_path(
+    base: pathlib.Path | pathlib.PurePath,
+    transaction: Transaction,
+    pure_posix: bool = False,
+) -> Transaction:
+    """Strip file base path (parent folder) from given transaction"""
+    if transaction.file is None:
+        return transaction
+    return Transaction(
+        **(
+            dataclasses.asdict(transaction)
+            | dict(file=strip_base_path(base, transaction.file, pure_posix))
+        )
+    )
```

