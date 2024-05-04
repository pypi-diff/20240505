# Comparing `tmp/yappt-0.3.1.tar.gz` & `tmp/yappt-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yappt-0.3.1.tar", last modified: Tue Feb 13 00:10:22 2024, max compression
+gzip compressed data, was "yappt-0.3.2.tar", last modified: Sat May  4 22:32:47 2024, max compression
```

## Comparing `yappt-0.3.1.tar` & `yappt-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-13 00:10:22.396899 yappt-0.3.1/
--rw-r--r--   0 padhia    (1000) users      (100)     1063 2024-02-12 20:11:11.000000 yappt-0.3.1/LICENSE
--rw-r--r--   0 padhia    (1000) users      (100)     1929 2024-02-13 00:10:22.396899 yappt-0.3.1/PKG-INFO
--rw-r--r--   0 padhia    (1000) users      (100)     1638 2024-02-13 00:07:46.000000 yappt-0.3.1/README.md
--rw-r--r--   0 padhia    (1000) users      (100)      663 2024-02-12 19:12:18.000000 yappt-0.3.1/pyproject.toml
--rw-r--r--   0 padhia    (1000) users      (100)       38 2024-02-13 00:10:22.397899 yappt-0.3.1/setup.cfg
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-13 00:10:22.393899 yappt-0.3.1/tests/
--rw-r--r--   0 padhia    (1000) users      (100)      672 2024-02-13 00:01:54.000000 yappt-0.3.1/tests/test_iterator.py
--rw-r--r--   0 padhia    (1000) users      (100)     3456 2024-02-13 00:00:35.000000 yappt-0.3.1/tests/test_tabulate.py
--rw-r--r--   0 padhia    (1000) users      (100)      603 2024-02-12 19:22:52.000000 yappt-0.3.1/tests/test_treeiter.py
--rw-r--r--   0 padhia    (1000) users      (100)     1718 2024-02-12 19:12:47.000000 yappt-0.3.1/tests/test_types.py
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-13 00:10:22.394899 yappt-0.3.1/yappt/
--rw-r--r--   0 padhia    (1000) users      (100)      344 2024-02-13 00:07:08.000000 yappt-0.3.1/yappt/__init__.py
--rw-r--r--   0 padhia    (1000) users      (100)     2327 2024-02-13 00:05:54.000000 yappt-0.3.1/yappt/grid.py
--rw-r--r--   0 padhia    (1000) users      (100)        0 2022-11-22 02:07:45.000000 yappt-0.3.1/yappt/py.typed
--rw-r--r--   0 padhia    (1000) users      (100)     5653 2024-02-13 00:05:46.000000 yappt-0.3.1/yappt/tabulate.py
--rw-r--r--   0 padhia    (1000) users      (100)     1397 2024-02-13 00:06:08.000000 yappt-0.3.1/yappt/treeiter.py
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-13 00:10:22.396899 yappt-0.3.1/yappt/types/
--rw-r--r--   0 padhia    (1000) users      (100)      299 2024-02-08 22:51:31.000000 yappt-0.3.1/yappt/types/__init__.py
--rw-r--r--   0 padhia    (1000) users      (100)     3921 2024-02-09 20:22:43.000000 yappt-0.3.1/yappt/types/column.py
--rw-r--r--   0 padhia    (1000) users      (100)     1348 2024-02-09 17:49:35.000000 yappt-0.3.1/yappt/types/duration.py
--rw-r--r--   0 padhia    (1000) users      (100)     3401 2024-02-09 19:42:40.000000 yappt-0.3.1/yappt/types/grid.py
--rw-r--r--   0 padhia    (1000) users      (100)     2153 2024-02-09 19:41:33.000000 yappt-0.3.1/yappt/types/prettyint.py
--rw-r--r--   0 padhia    (1000) users      (100)     2886 2024-02-13 00:06:19.000000 yappt-0.3.1/yappt/util.py
-drwxr-xr-x   0 padhia    (1000) users      (100)        0 2024-02-13 00:10:22.396899 yappt-0.3.1/yappt.egg-info/
--rw-r--r--   0 padhia    (1000) users      (100)     1929 2024-02-13 00:10:22.000000 yappt-0.3.1/yappt.egg-info/PKG-INFO
--rw-r--r--   0 padhia    (1000) users      (100)      449 2024-02-13 00:10:22.000000 yappt-0.3.1/yappt.egg-info/SOURCES.txt
--rw-r--r--   0 padhia    (1000) users      (100)        1 2024-02-13 00:10:22.000000 yappt-0.3.1/yappt.egg-info/dependency_links.txt
--rw-r--r--   0 padhia    (1000) users      (100)        6 2024-02-13 00:10:22.000000 yappt-0.3.1/yappt.egg-info/top_level.txt
+drwxr-xr-x   0 padhia     (501) staff       (20)        0 2024-05-04 22:32:47.236973 yappt-0.3.2/
+-rw-r--r--   0 padhia     (501) staff       (20)     1063 2024-05-04 22:26:18.000000 yappt-0.3.2/LICENSE
+-rw-r--r--   0 padhia     (501) staff       (20)     2050 2024-05-04 22:32:47.236684 yappt-0.3.2/PKG-INFO
+-rw-r--r--   0 padhia     (501) staff       (20)     1640 2024-05-04 22:28:12.000000 yappt-0.3.2/README.md
+-rw-r--r--   0 padhia     (501) staff       (20)      783 2024-05-04 22:28:12.000000 yappt-0.3.2/pyproject.toml
+-rw-r--r--   0 padhia     (501) staff       (20)       38 2024-05-04 22:32:47.237023 yappt-0.3.2/setup.cfg
+drwxr-xr-x   0 padhia     (501) staff       (20)        0 2024-05-04 22:32:47.232271 yappt-0.3.2/tests/
+-rw-r--r--   0 padhia     (501) staff       (20)      673 2024-05-04 22:28:12.000000 yappt-0.3.2/tests/test_iterator.py
+-rw-r--r--   0 padhia     (501) staff       (20)     3457 2024-05-04 22:28:12.000000 yappt-0.3.2/tests/test_tabulate.py
+-rw-r--r--   0 padhia     (501) staff       (20)      604 2024-05-04 22:28:12.000000 yappt-0.3.2/tests/test_treeiter.py
+-rw-r--r--   0 padhia     (501) staff       (20)     1719 2024-05-04 22:28:12.000000 yappt-0.3.2/tests/test_types.py
+drwxr-xr-x   0 padhia     (501) staff       (20)        0 2024-05-04 22:32:47.233613 yappt-0.3.2/yappt/
+-rw-r--r--   0 padhia     (501) staff       (20)      345 2024-05-04 22:28:12.000000 yappt-0.3.2/yappt/__init__.py
+-rw-r--r--   0 padhia     (501) staff       (20)     2328 2024-05-04 22:28:12.000000 yappt-0.3.2/yappt/grid.py
+-rw-r--r--   0 padhia     (501) staff       (20)        0 2024-05-04 22:26:18.000000 yappt-0.3.2/yappt/py.typed
+-rw-r--r--   0 padhia     (501) staff       (20)     5814 2024-05-04 22:28:12.000000 yappt-0.3.2/yappt/tabulate.py
+-rw-r--r--   0 padhia     (501) staff       (20)     1397 2024-05-04 22:26:18.000000 yappt-0.3.2/yappt/treeiter.py
+drwxr-xr-x   0 padhia     (501) staff       (20)        0 2024-05-04 22:32:47.236008 yappt-0.3.2/yappt/types/
+-rw-r--r--   0 padhia     (501) staff       (20)      299 2024-05-04 22:26:18.000000 yappt-0.3.2/yappt/types/__init__.py
+-rw-r--r--   0 padhia     (501) staff       (20)     3952 2024-05-04 22:28:12.000000 yappt-0.3.2/yappt/types/column.py
+-rw-r--r--   0 padhia     (501) staff       (20)     1349 2024-05-04 22:28:12.000000 yappt-0.3.2/yappt/types/duration.py
+-rw-r--r--   0 padhia     (501) staff       (20)     3402 2024-05-04 22:28:12.000000 yappt-0.3.2/yappt/types/grid.py
+-rw-r--r--   0 padhia     (501) staff       (20)     2154 2024-05-04 22:28:12.000000 yappt-0.3.2/yappt/types/prettyint.py
+-rw-r--r--   0 padhia     (501) staff       (20)     3120 2024-05-04 22:28:12.000000 yappt-0.3.2/yappt/util.py
+drwxr-xr-x   0 padhia     (501) staff       (20)        0 2024-05-04 22:32:47.236316 yappt-0.3.2/yappt.egg-info/
+-rw-r--r--   0 padhia     (501) staff       (20)     2050 2024-05-04 22:32:47.000000 yappt-0.3.2/yappt.egg-info/PKG-INFO
+-rw-r--r--   0 padhia     (501) staff       (20)      477 2024-05-04 22:32:47.000000 yappt-0.3.2/yappt.egg-info/SOURCES.txt
+-rw-r--r--   0 padhia     (501) staff       (20)        1 2024-05-04 22:32:47.000000 yappt-0.3.2/yappt.egg-info/dependency_links.txt
+-rw-r--r--   0 padhia     (501) staff       (20)       16 2024-05-04 22:32:47.000000 yappt-0.3.2/yappt.egg-info/requires.txt
+-rw-r--r--   0 padhia     (501) staff       (20)        6 2024-05-04 22:32:47.000000 yappt-0.3.2/yappt.egg-info/top_level.txt
```

### Comparing `yappt-0.3.1/LICENSE` & `yappt-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yappt-0.3.1/PKG-INFO` & `yappt-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: yappt
-Version: 0.3.1
-Summary: Yet another pretty print for tables and trees
+Version: 0.3.2
+Summary: Yet another pretty printer for tables and trees
 Author-email: Paresh Adhia <padhia+github@gmail.com>
+Project-URL: Homepage, https://github.com/padhia/yappt
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
 
 # yappt
 
-Yet another pretty print for tables and trees.
+Yet another pretty printer for tables and trees.
 
 **Note:** Versions `0.3.0` and later aren't compatible with earlier versions
 
 A collection of classes and functions to format textual data for printing. The main functions (`tabulate` and `treeiter`) do not require reading entire dataset into memory, allowing printing large amount of data in streaming fashion.
 
 Class       | Capabilities
 ------------|------------------------------------------------------------------------------------------------------
```

### Comparing `yappt-0.3.1/README.md` & `yappt-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # yappt
 
-Yet another pretty print for tables and trees.
+Yet another pretty printer for tables and trees.
 
 **Note:** Versions `0.3.0` and later aren't compatible with earlier versions
 
 A collection of classes and functions to format textual data for printing. The main functions (`tabulate` and `treeiter`) do not require reading entire dataset into memory, allowing printing large amount of data in streaming fashion.
 
 Class       | Capabilities
 ------------|------------------------------------------------------------------------------------------------------
```

### Comparing `yappt-0.3.1/pyproject.toml` & `yappt-0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yappt"
-description = "Yet another pretty print for tables and trees"
+description = "Yet another pretty printer for tables and trees"
 authors = [{ name = "Paresh Adhia", email = "padhia+github@gmail.com" }]
 readme = "README.md"
 requires-python = ">= 3.9"
 classifiers = ["Programming Language :: Python :: 3"]
 dynamic = ["version"]
 
+[project.optional-dependencies]
+tests = ["pytest"]
+
+[project.urls]
+Homepage = "https://github.com/padhia/yappt"
+
 [tool.setuptools]
 packages = ["yappt", "yappt.types"]
 
 [tool.setuptools.dynamic]
 version = { attr = "yappt.__version__" }
 
 [tool.setuptools.package-data]
 "*" = ["py.typed"]
 
 [tool.ruff]
 line-length = 130
 target-version = "py39"
-extend-select = ["I"]
+lint.extend-select = ["I"]
 
 [tool.pytest.ini_options]
 pythonpath = ["."]
```

### Comparing `yappt-0.3.1/tests/test_iterator.py` & `yappt-0.3.2/tests/test_iterator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "test tabulate with an iterator as an input"
+
 from textwrap import dedent
 from typing import Optional
 
 from yappt import tabulate_iter
 
 
 def test_dataclass() -> None:
```

### Comparing `yappt-0.3.1/tests/test_tabulate.py` & `yappt-0.3.2/tests/test_tabulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "test tabulate"
+
 from dataclasses import dataclass, field
 from datetime import date
 from textwrap import dedent
 from typing import Optional
 
 from yappt import tabulate_iter
```

### Comparing `yappt-0.3.1/tests/test_treeiter.py` & `yappt-0.3.2/tests/test_treeiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "test treeiter"
+
 from textwrap import dedent
 from typing import Iterable
 
 from yappt import treeiter
 
 
 def test_treeiter() -> None:
```

### Comparing `yappt-0.3.1/tests/test_types.py` & `yappt-0.3.2/tests/test_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "test types"
+
 import pytest
 
 from yappt import Duration, PrettyInt, format_bool
 
 
 def test_duration() -> None:
     assert format(Duration(seconds=300)) == "5m"
```

### Comparing `yappt-0.3.1/yappt/grid.py` & `yappt-0.3.2/yappt/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "print rows as a grid"
+
 import logging
 import os
 from itertools import chain, islice
 from typing import Iterable, Optional, Sequence
 
 from .types import BasicGridStyle, BoxedGridStyle, GridConnectors, GridStyle
```

### Comparing `yappt-0.3.1/yappt/tabulate.py` & `yappt-0.3.2/yappt/tabulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 "tabulate (print in a grid) an iterable of either dataclass objects, or Sequences"
+
+import sys
 from dataclasses import fields, is_dataclass
 from itertools import chain, islice, zip_longest
-from typing import Any, Callable, Iterable, Optional, Sequence, TypeVar
+from typing import Any, Callable, Iterable, Optional, Sequence, TextIO, TypeVar
 
 from .grid import GridStyle, iter_with_grid
 from .types import Column, HAlign
+from .util import DEFAULT_FMTSPEC
 
 T = TypeVar("T")
 
 
 def tabulate(
     rows: Iterable[Sequence[Any] | Any],
     headers: Optional[Sequence[str]] = None,
     types: Optional[Sequence[type]] = None,
     *,
     peek: int = 200,
-    default_fmtspc: dict[type, str] = {},
+    default_fmtspc: dict[type, str] = DEFAULT_FMTSPEC,
     grid_style: Optional[GridStyle] = None,
     default_grid_style: Optional[GridStyle] = None,
+    file: TextIO = sys.stdout,
 ) -> None:
     """
     pretty print rows of data in tabular form
 
     Args:
         rows: iterable of dataclass instances or Sequences. All rows must be of same type
         headers: column titles, defaults to column number. valid only when row is a Sequence
@@ -39,24 +43,24 @@
         headers,
         types,
         peek=peek,
         default_fmtspc=default_fmtspc,
         grid_style=grid_style,
         default_grid_style=default_grid_style,
     ):
-        print(line)
+        print(line, file=file)
 
 
 def tabulate_iter(
     rows: Iterable[Sequence[Any] | Any],
     headers: Optional[Sequence[str]] = None,
     types: Optional[Sequence[type]] = None,
     *,
     peek: int = 200,
-    default_fmtspc: dict[type, str] = {},
+    default_fmtspc: dict[type, str] = DEFAULT_FMTSPEC,
     grid_style: Optional[GridStyle] = None,
     default_grid_style: Optional[GridStyle] = None,
 ) -> Iterable[str]:
     """
     accepts an Iterable of either dataclass instances or Sequences, and returns an Iterable of strings of data in a grid
 
     Args:
@@ -75,46 +79,46 @@
     try:
         first = next(it)
     except StopIteration:
         return
 
     it = chain([first], it)
     if is_dataclass(first):
-        cols, formatted_rows = iter_dc_fmt(it, first.__class__, default_fmtspc)  # type: ignore
+        cols, formatted_rows = formatted_obj_iter(it, first.__class__, default_fmtspc)  # type: ignore
     elif isinstance(first, Sequence):
-        cols, formatted_rows = iter_seq_fmt(it, types or [type(c) for c in first], headers, default_fmtspc)
+        cols, formatted_rows = formatted_seq_iter(it, types or [type(c) for c in first], headers, default_fmtspc)
     else:
         raise TypeError(f"Input to tabulate() must be an Iterable of either dataclass or a Sequnce, not {type(first)}")
 
     it = chain([[m.title for m in cols]], formatted_rows)
     if peek > 0:
         it = aligned_seq_iter(it, [m.alignment for m in cols], peek + 1)  # +1 to adjust for the header row
     it = iter_with_grid(iter(it), num_headers=1, grid_style=grid_style, default_grid_style=default_grid_style)
 
     yield from it
 
 
-def iter_seq_fmt(
+def formatted_seq_iter(
     rows: Iterable[Sequence[Any]],
     types: Sequence[type[Any]],
     headers: Optional[Sequence[str]] = None,
-    default_fmtspec: dict[type, str] = {},
+    default_fmtspec: dict[type, str] = DEFAULT_FMTSPEC,
 ) -> tuple[list[Column[Any]], Iterable[Sequence[str]]]:
     if headers is None:
         headers = [f"_{e}" for e, _ in enumerate(types, start=1)]
     cols = [Column.from_type(h, t, default_fmtspec=default_fmtspec) for h, t in zip(headers, types)]
     xs = [(c.format, e) for e, c in enumerate(cols)]
 
     def as_seq(o: Sequence[str]) -> list[str]:
         return [f(o[e]) for f, e in xs]
 
     return (cols, (as_seq(o) for o in rows))
 
 
-def iter_dc_fmt(
+def formatted_obj_iter(
     rows: Iterable[T], DC_Type: type[T], default_fmtspec: dict[type, str] = {}
 ) -> tuple[list[Column[Any]], Iterable[Sequence[str]]]:
     cols = Column.from_dataclass(DC_Type, default_fmtspec)
     attrs = [f.name for f in fields(DC_Type)]  # type: ignore
     xs = [(c.format, n) for c, n in zip(cols, attrs)]
 
     def as_seq(o: T) -> list[str]:
```

### Comparing `yappt-0.3.1/yappt/treeiter.py` & `yappt-0.3.2/yappt/treeiter.py`

 * *Files identical despite different names*

### Comparing `yappt-0.3.1/yappt/types/column.py` & `yappt-0.3.2/yappt/types/column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 "class to store metadata for formatting a column"
+
 import datetime as dt
 from dataclasses import Field, dataclass, fields
 from decimal import Decimal
 from enum import Enum
 from typing import Callable, Generic, Optional, TypeVar, get_type_hints
 
-from ..util import bare_type, format_bool
+from ..util import DEFAULT_FMTSPEC, bare_type, format_bool
 from .duration import Duration
 from .prettyint import PrettyInt
 
 T = TypeVar("T")
 
 
 class HAlign(str, Enum):
@@ -75,15 +76,15 @@
 
     @staticmethod
     def from_type(
         title: str,
         type_hint: type[T],
         format_spec: Optional[str] = None,
         align: Optional[str] = None,
-        default_fmtspec: dict[type, str] = {},
+        default_fmtspec: dict[type, str] = DEFAULT_FMTSPEC,
     ) -> "Column[T]":
         """
         Instantiate a Column instance for a Python type
 
         Args:
             title: column title
             type_hint: a Python type to determine formatting style; if the type is Optional[T], T is used instead
```

### Comparing `yappt-0.3.1/yappt/types/duration.py` & `yappt-0.3.2/yappt/types/duration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "datetime.timedelta subclass that produces formatted human-readable output"
+
 import datetime as dt
 import re
 
 
 class Duration(dt.timedelta):
     """Python datetime.timedelta subclass that can be formatted.
```

### Comparing `yappt-0.3.1/yappt/types/grid.py` & `yappt-0.3.2/yappt/types/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "classes that represent grid drawing styles"
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Iterable, Sequence
 
 
 @dataclass(frozen=True)
 class GridConnectors:
```

### Comparing `yappt-0.3.1/yappt/types/prettyint.py` & `yappt-0.3.2/yappt/types/prettyint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "int subclass that formats in pretty human-readable format"
+
 import re
 
 
 class PrettyInt(int):
     "An int subclass that formats values for human readability (similar to --human-readable option of the ls command)"
 
     @staticmethod
```

### Comparing `yappt-0.3.1/yappt/util.py` & `yappt-0.3.2/yappt/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 "utility types and functions"
+
+import datetime as dt
 import re
+from decimal import Decimal
 from types import UnionType
 from typing import Iterable, TypeVar, Union, get_origin
 
 T = TypeVar("T")
 
+DEFAULT_FMTSPEC: dict[type, str] = {
+    int: ",d",
+    float: ",.2f",
+    Decimal: ",.2f",
+    dt.date: "%Y-%m-%d",
+    dt.time: "%H:%M:%S",
+    dt.datetime: "%Y-%m-%d %H:%M:%S",
+}
+
 
 def iter_more(xs: Iterable[T]) -> Iterable[tuple[bool, T]]:
     """retrun a new iterable based on the given iterable, that peeks past the current value for existence and returns
     tuple (more, item), where more is True if current is not the last item
 
     Args:
         xs: An Iterable of type T
```

### Comparing `yappt-0.3.1/yappt.egg-info/PKG-INFO` & `yappt-0.3.2/yappt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: yappt
-Version: 0.3.1
-Summary: Yet another pretty print for tables and trees
+Version: 0.3.2
+Summary: Yet another pretty printer for tables and trees
 Author-email: Paresh Adhia <padhia+github@gmail.com>
+Project-URL: Homepage, https://github.com/padhia/yappt
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
 
 # yappt
 
-Yet another pretty print for tables and trees.
+Yet another pretty printer for tables and trees.
 
 **Note:** Versions `0.3.0` and later aren't compatible with earlier versions
 
 A collection of classes and functions to format textual data for printing. The main functions (`tabulate` and `treeiter`) do not require reading entire dataset into memory, allowing printing large amount of data in streaming fashion.
 
 Class       | Capabilities
 ------------|------------------------------------------------------------------------------------------------------
```

