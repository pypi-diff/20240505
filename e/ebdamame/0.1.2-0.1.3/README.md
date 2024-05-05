# Comparing `tmp/ebdamame-0.1.2.tar.gz` & `tmp/ebdamame-0.1.3.tar.gz`

## Comparing `ebdamame-0.1.2.tar` & `ebdamame-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 ebdamame-0.1.2/README.md
--rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 ebdamame-0.1.2/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ebdamame-0.1.2/requirements.in
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 ebdamame-0.1.2/requirements.txt
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 ebdamame-0.1.2/setup.cfg
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ebdamame-0.1.2/setup.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ebdamame-0.1.2/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/dependabot.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/packaging.yml
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ebdamame-0.1.2/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ebdamame-0.1.2/src/_ebddocx2table_version.py
--rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 ebdamame-0.1.2/src/ebdamame/__init__.py
--rw-r--r--   0        0        0    17292 2020-02-02 00:00:00.000000 ebdamame-0.1.2/src/ebdamame/docxtableconverter.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ebdamame-0.1.2/src/ebdamame/py.typed
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 ebdamame-0.1.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ebdamame-0.1.2/LICENSE
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ebdamame-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 ebdamame-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 ebdamame-0.1.3/README.md
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ebdamame-0.1.3/main.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ebdamame-0.1.3/requirements.in
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 ebdamame-0.1.3/requirements.txt
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 ebdamame-0.1.3/setup.cfg
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ebdamame-0.1.3/setup.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ebdamame-0.1.3/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.github/workflows/packaging.yml
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ebdamame-0.1.3/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0    11095 2020-02-02 00:00:00.000000 ebdamame-0.1.3/src/ebdamame/__init__.py
+-rw-r--r--   0        0        0    17377 2020-02-02 00:00:00.000000 ebdamame-0.1.3/src/ebdamame/docxtableconverter.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ebdamame-0.1.3/src/ebdamame/py.typed
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ebdamame-0.1.3/src/ebdamame/version.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 ebdamame-0.1.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ebdamame-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 ebdamame-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 ebdamame-0.1.3/PKG-INFO
```

### Comparing `ebdamame-0.1.2/.pre-commit-config.yaml` & `ebdamame-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/README.md` & `ebdamame-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/setup.cfg` & `ebdamame-0.1.3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # The content of this file is only necessary for python packages
 [metadata]
-name = ebddocx2table
+name = ebdamame
 author = Hochfrequenz Unternehmensberatung GmbH
 author_email = info@hochfrequenz.de
 description = library to scrape .docx files with Entscheidungsbaumdiagramm tables into a truely machine readable structure 
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
-url = https://github.com/Hochfrequenz/ebddocx2table
+url = https://github.com/Hochfrequenz/ebdamame
 project_urls =
-    Documentation = https://github.com/Hochfrequenz/ebddocx2table
-    Code = https://github.com/Hochfrequenz/ebddocx2table
-    Bug tracker = https://github.com/Hochfrequenz/ebddocx2table/issues
+    Documentation = https://github.com/Hochfrequenz/ebdamame
+    Code = https://github.com/Hochfrequenz/ebdamame
+    Bug tracker = https://github.com/Hochfrequenz/ebdamame/issues
 classifiers =
     Development Status :: 4 - Beta
     Intended Audience :: Developers
     Programming Language :: Python
     Programming Language :: Python :: 3.11
     Programming Language :: Python :: 3.12
     Operating System :: OS Independent
@@ -27,15 +27,15 @@
 package_dir =
     = src
 packages = find:
 zip_safe = False
 include_package_data = True
 python_requires = >=3.11
 install_requires =
-    ebdtable2graph>=0.1.20
+    rebdhuhn>=0.2.3
     python-docx
     more_itertools
     attrs
     click
     # write here line by line the dependencies for your package
 
 [options.packages.find]
```

### Comparing `ebdamame-0.1.2/tox.ini` & `ebdamame-0.1.3/tox.ini`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/.github/dependabot.yml` & `ebdamame-0.1.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/.github/workflows/coverage.yml` & `ebdamame-0.1.3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/.github/workflows/dependabot_automerge.yml` & `ebdamame-0.1.3/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/.github/workflows/formatting.yml` & `ebdamame-0.1.3/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/.github/workflows/packaging.yml` & `ebdamame-0.1.3/.github/workflows/packaging.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/.github/workflows/python-publish.yml` & `ebdamame-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/.github/workflows/pythonlint.yml` & `ebdamame-0.1.3/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/.github/workflows/unittests.yml` & `ebdamame-0.1.3/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/dev_requirements/requirements-packaging.txt` & `ebdamame-0.1.3/dev_requirements/requirements-packaging.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,75 @@
+# SHA1:93e4fbf2b6cce1574fe3d5315360512fa9927699
 #
-# This file is autogenerated by pip-compile with Python 3.12
-# by the following command:
+# This file is autogenerated by pip-compile-multi
+# To update, run:
 #
-#    pip-compile dev_requirements/requirements-packaging.in
+#    pip-compile-multi
 #
+backports-tarfile==1.1.1
+    # via jaraco-context
 build==1.2.1
-    # via -r dev_requirements/requirements-packaging.in
+    # via -r dev_requirements\requirements-packaging.in
 certifi==2024.2.2
     # via requests
-cffi==1.16.0
-    # via cryptography
 charset-normalizer==3.3.2
     # via requests
-cryptography==42.0.5
-    # via secretstorage
-docutils==0.20.1
+colorama==0.4.6
+    # via build
+docutils==0.21.2
     # via readme-renderer
 idna==3.7
     # via requests
-importlib-metadata==7.0.2
+importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
-jaraco-classes==3.3.1
+jaraco-classes==3.4.0
     # via keyring
-jeepney==0.8.0
-    # via
-    #   keyring
-    #   secretstorage
-keyring==24.3.1
+jaraco-context==5.3.0
+    # via keyring
+jaraco-functools==4.0.1
+    # via keyring
+keyring==25.2.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
-    # via jaraco-classes
-nh3==0.2.15
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
+nh3==0.2.17
     # via readme-renderer
 packaging==24.0
     # via build
 pkginfo==1.10.0
     # via twine
-pycparser==2.21
-    # via cffi
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   readme-renderer
     #   rich
-pyproject-hooks==1.0.0
+pyproject-hooks==1.1.0
     # via build
+pywin32-ctypes==0.2.2
+    # via keyring
 readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.7.1
     # via twine
-secretstorage==3.3.3
-    # via keyring
 twine==5.0.0
-    # via -r dev_requirements/requirements-packaging.in
+    # via -r dev_requirements\requirements-packaging.in
 urllib3==2.2.1
     # via
     #   requests
     #   twine
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `ebdamame-0.1.2/src/ebdamame/__init__.py` & `ebdamame-0.1.3/src/ebdamame/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,41 +6,42 @@
 import logging
 import re
 from io import BytesIO
 from pathlib import Path
 from typing import Dict, Generator, Iterable, List, Optional, Tuple, Union
 
 import attrs
-from docx import Document  # type:ignore[import]
-from docx.oxml import CT_P, CT_Tbl  # type:ignore[import]
-from docx.table import Table, _Cell  # type:ignore[import]
-from docx.text.paragraph import Paragraph  # type:ignore[import]
+import docx
+from docx.document import Document as DocumentType
+from docx.oxml import CT_P, CT_Tbl
+from docx.table import Table, _Cell
+from docx.text.paragraph import Paragraph
 
 _logger = logging.getLogger(__name__)
 
 
-def get_document(docx_file_path: Path) -> Document:
+def get_document(docx_file_path: Path) -> DocumentType:
     """
     opens and returns the document specified in the docx_file_path using python-docx
     """
     with open(docx_file_path, "rb") as docx_file:
         source_stream = BytesIO(docx_file.read())
         # Originally I tried the recipe from
         # https://python-docx.readthedocs.io/en/latest/user/documents.html#opening-a-file-like-document
         # but then switched from StringIO to BytesIO (without explicit 'utf-8') because of:
         # UnicodeDecodeError: 'charmap' codec can't decode byte 0x81 in position 605: character maps to <undefined>
     try:
-        document = Document(source_stream)
+        document = docx.Document(source_stream)
         _logger.info("Successfully read the file '%s'", docx_file_path)
         return document
     finally:
         source_stream.close()
 
 
-def _get_tables_and_paragaphs(document: Document) -> Generator[Union[Table, Paragraph], None, None]:
+def _get_tables_and_paragraphs(document: DocumentType) -> Generator[Union[Table, Paragraph], None, None]:
     """
     Yields tables and paragraphs from the given document in the order in which they occur in the document.
     This is helpful because document.tables and document.paragraphs are de-coupled and give you no information which
     paragraph follows which table.
     """
     parent_elements = document.element.body
     for item in parent_elements.iterchildren():
@@ -112,15 +113,15 @@
     """
     if _ebd_key_pattern.match(ebd_key) is None:
         raise ValueError(f"The ebd_key '{ebd_key}' does not match {_ebd_key_pattern.pattern}")
     document = get_document(docx_file_path)
 
     is_inside_subsection_of_requested_table: bool = False
     tables: List[Table] = []
-    tables_and_paragraphs = _get_tables_and_paragaphs(document)
+    tables_and_paragraphs = _get_tables_and_paragraphs(document)
     for table_or_paragraph in tables_and_paragraphs:
         if isinstance(table_or_paragraph, Paragraph):
             paragraph: Paragraph = table_or_paragraph
             # Assumptions:
             # 1. before each EbdTable there is a paragraph whose text starts with the respective EBD key
             # 2. there are no duplicates
             is_inside_subsection_of_requested_table = (
@@ -209,15 +210,16 @@
     section_counter = itertools.count(start=1)
     section = 1
     section_title: Optional[str] = None
     subsection_counter = itertools.count(start=1)
     subsection = 1
     subsection_title: Optional[str] = None
     for paragraph in paragraphs:
-        match paragraph.style.style_id:
+        # since pyton-docx 1.1.2 there are type hints; seems like the style is not guaranteed to be not None
+        match paragraph.style.style_id:  #  type:ignore[union-attr]
             case "berschrift1":
                 chapter = next(chapter_counter)
                 chapter_title = paragraph.text.strip()
                 section_counter = itertools.count(start=1)
                 section_title = None
                 subsection_counter = itertools.count(start=1)
                 subsection_title = None
```

### Comparing `ebdamame-0.1.2/src/ebdamame/docxtableconverter.py` & `ebdamame-0.1.3/src/ebdamame/docxtableconverter.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,25 @@
 import logging
 import re
 from enum import Enum
 from itertools import cycle, groupby
 from typing import Generator, List, Literal, Optional, Tuple
 
 import attrs
-from docx.table import Table, _Cell, _Row  # type:ignore[import]
-from ebdtable2graph.models import EbdTable, EbdTableRow, EbdTableSubRow
-from ebdtable2graph.models.ebd_table import _STEP_NUMBER_REGEX, EbdCheckResult, EbdTableMetaData, MultiStepInstruction
+from docx.table import Table, _Cell, _Row
 from more_itertools import first, first_true, last
+from rebdhuhn.models.ebd_table import (
+    _STEP_NUMBER_REGEX,
+    EbdCheckResult,
+    EbdTable,
+    EbdTableMetaData,
+    EbdTableRow,
+    EbdTableSubRow,
+    MultiStepInstruction,
+)
 
 _logger = logging.getLogger(__name__)
 
 
 def _is_pruefende_rolle_cell_text(text: str) -> bool:
     """ "
     Returns true iff the given text mentions the market role that is responsible for applying this entscheidungsbaum
@@ -42,14 +49,17 @@
 def _get_index_of_first_column_with_step_number(cells: List[_Cell]) -> int:
     """
     returns the index of the first cell in cells, that contains a step number
     """
     first_step_number_cell = first_true(
         cells, pred=lambda cell: _step_number_pattern.match(cell.text.strip()) is not None
     )
+    if first_step_number_cell is None:
+        raise ValueError("No cell containing a valid step number found.")
+
     step_number_column_index = cells.index(first_step_number_cell)
     _logger.debug("The step number is in column %i", step_number_column_index)
     return step_number_column_index
 
 
 def _get_use_cases(cells: List[_Cell]) -> List[str]:
     """
```

### Comparing `ebdamame-0.1.2/.gitignore` & `ebdamame-0.1.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -128,9 +128,7 @@
 # Pyre type checker
 .pyre/
 
 .idea/
 
 # vscode settings
 .vscode/
-
-src/_ebdamame_version.py
```

### Comparing `ebdamame-0.1.2/LICENSE` & `ebdamame-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ebdamame-0.1.2/pyproject.toml` & `ebdamame-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "ebdtable2graph>=0.1.19",
+    "rebdhuhn>=0.2.3",
     "python-docx",
     "more_itertools",
     "attrs",
     "click"
     # add all the dependencies from requirements.in here, too
 ]
 dynamic = ["readme", "version"]
@@ -48,18 +48,15 @@
 content-type = "text/markdown"
 fragments = [{ path = "README.md" }]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
-version-file = "src/_ebddocx2table_version.py"
-template = '''
-version = "{version}"
-'''
+version-file = "src/ebdamame/version.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = ["/unittests"]
 
 [tool.hatch.build.targets.wheel]
 only-include = ["src"]
 sources = ["src"]
```

### Comparing `ebdamame-0.1.2/PKG-INFO` & `ebdamame-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ebdamame
-Version: 0.1.2
+Version: 0.1.3
 Summary: A scraper to library to scrape .docx files with 'Entscheidungsbaumdiagramm' tables into a truely machine readable structure
 Project-URL: Changelog, https://github.com/Hochfrequenz/ebdamame/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/ebdamame
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info@hochfrequenz.de>
 License: GPL
 License-File: LICENSE
 Keywords: EBD,Energiewirtschaft,Marktkommunikation
@@ -16,17 +16,17 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Requires-Dist: attrs
 Requires-Dist: click
-Requires-Dist: ebdtable2graph>=0.1.19
 Requires-Dist: more-itertools
 Requires-Dist: python-docx
+Requires-Dist: rebdhuhn>=0.2.3
 Description-Content-Type: text/markdown
 
 # ebdamame
 
 ![Unittests status badge](https://github.com/Hochfrequenz/ebdamame/workflows/Unittests/badge.svg)
 ![Coverage status badge](https://github.com/Hochfrequenz/ebdamame/workflows/Coverage/badge.svg)
 ![Linting status badge](https://github.com/Hochfrequenz/ebdamame/workflows/Linting/badge.svg)
```

