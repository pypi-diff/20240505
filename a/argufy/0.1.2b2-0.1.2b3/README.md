# Comparing `tmp/argufy-0.1.2b2.tar.gz` & `tmp/argufy-0.1.2b3.tar.gz`

## Comparing `argufy-0.1.2b2.tar` & `argufy-0.1.2b3.tar`

### file list

```diff
@@ -1,60 +1,58 @@
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 argufy-0.1.2b2/.docstr.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 argufy-0.1.2b2/.flake8
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 argufy-0.1.2b2/mkdocs.yml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 argufy-0.1.2b2/docs/commands.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b2/docs/docstrings.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 argufy-0.1.2b2/docs/getting-started.md
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 argufy-0.1.2b2/docs/index.md
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 argufy-0.1.2b2/docs/roadmap.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b2/docs/subcommands.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b2/docs/type-hints.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 argufy-0.1.2b2/docs/development/argument.md
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 argufy-0.1.2b2/docs/development/parser.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/bool.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/complete.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/group.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/kwargs.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/simple.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/commands/__init__.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/commands/__main__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/commands/cmd1.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/commands/cmd2.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/dataclass/__init__.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/dataclass/__main__.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/dataclass/cmd.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/dataclass/config.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/multiparse/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/multiparse/__main__.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/multiparse/cmd1.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/multiparse/cmd2.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/multiparse/config.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/parents/parents.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/subcommands/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/subcommands/__main__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/subcommands/cmd1.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/subcommands/cmd2.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 argufy-0.1.2b2/examples/subcommands/config.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 argufy-0.1.2b2/src/argufy/__init__.py
--rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 argufy-0.1.2b2/src/argufy/argument.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 argufy-0.1.2b2/src/argufy/exceptions.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 argufy-0.1.2b2/src/argufy/formatter.py
--rw-r--r--   0        0        0    18843 2020-02-02 00:00:00.000000 argufy-0.1.2b2/src/argufy/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b2/src/argufy/py.typed
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tasks/__init__.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tasks/build.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tasks/doc.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tasks/qa.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tests/test_argument_type_hints.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tests/test_version.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tests/commands/command_parser.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tests/commands/test_command_parser.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tests/docstrings/test_google.py
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tests/docstrings/test_numpy.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tests/docstrings/test_restructured.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tests/subcommands/subcommands_parser.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 argufy-0.1.2b2/tests/subcommands/test_subcommands_parser.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 argufy-0.1.2b2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 argufy-0.1.2b2/LICENSE
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 argufy-0.1.2b2/README.md
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 argufy-0.1.2b2/pyproject.toml
--rw-r--r--   0        0        0    17040 2020-02-02 00:00:00.000000 argufy-0.1.2b2/PKG-INFO
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 argufy-0.1.2b3/.docstr.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 argufy-0.1.2b3/.flake8
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 argufy-0.1.2b3/mkdocs.yml
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 argufy-0.1.2b3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 argufy-0.1.2b3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/commands.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/docstrings.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/getting-started.md
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/index.md
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/roadmap.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/subcommands.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/type-hints.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/development/argument.md
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 argufy-0.1.2b3/docs/development/parser.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/bool.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/complete.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/group.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/kwargs.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/simple.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/commands/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/commands/__main__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/commands/cmd1.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/commands/cmd2.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/dataclass/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/dataclass/__main__.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/dataclass/cmd.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/dataclass/config.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/multiparse/__init__.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/multiparse/__main__.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/multiparse/cmd1.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/multiparse/cmd2.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/multiparse/config.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/parents/parents.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/subcommands/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/subcommands/__main__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/subcommands/cmd1.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/subcommands/cmd2.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 argufy-0.1.2b3/examples/subcommands/config.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/__init__.py
+-rw-r--r--   0        0        0     8850 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/argument.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/exceptions.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/formatter.py
+-rw-r--r--   0        0        0    19275 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 argufy-0.1.2b3/src/argufy/py.typed
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/test_argument_type_hints.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/test_version.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/commands/command_parser.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/commands/test_command_parser.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/docstrings/test_google.py
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/docstrings/test_numpy.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/docstrings/test_restructured.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/subcommands/subcommands_parser.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 argufy-0.1.2b3/tests/subcommands/test_subcommands_parser.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 argufy-0.1.2b3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 argufy-0.1.2b3/LICENSE
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 argufy-0.1.2b3/README.md
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 argufy-0.1.2b3/pyproject.toml
+-rw-r--r--   0        0        0    17162 2020-02-02 00:00:00.000000 argufy-0.1.2b3/PKG-INFO
```

### Comparing `argufy-0.1.2b2/mkdocs.yml` & `argufy-0.1.2b3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/docs/commands.md` & `argufy-0.1.2b3/docs/commands.md`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/docs/getting-started.md` & `argufy-0.1.2b3/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/docs/index.md` & `argufy-0.1.2b3/docs/index.md`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/docs/roadmap.md` & `argufy-0.1.2b3/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/bool.py` & `argufy-0.1.2b3/examples/bool.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/complete.py` & `argufy-0.1.2b3/examples/complete.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/group.py` & `argufy-0.1.2b3/examples/group.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/kwargs.py` & `argufy-0.1.2b3/examples/kwargs.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/simple.py` & `argufy-0.1.2b3/examples/simple.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/commands/cmd1.py` & `argufy-0.1.2b3/examples/commands/cmd1.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/commands/cmd2.py` & `argufy-0.1.2b3/examples/commands/cmd2.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/dataclass/__main__.py` & `argufy-0.1.2b3/examples/dataclass/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 # copyright: (c) 2020 by Jesse Johnson.
 # license: Apache 2.0, see LICENSE for more details.
 """Provide CLI for example."""
 
 import sys
+
 from argufy import Parser
 
 from . import cmd
 
 
 def main() -> None:
     """Demonstrate main with CLI."""
```

### Comparing `argufy-0.1.2b2/examples/dataclass/cmd.py` & `argufy-0.1.2b3/examples/dataclass/cmd.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/multiparse/__main__.py` & `argufy-0.1.2b3/examples/multiparse/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 # copyright: (c) 2020 by Jesse Johnson.
 # license: Apache 2.0, see LICENSE for more details.
 """Provide CLI for example."""
 
 import sys
+
 from argufy import Parser
 
 from . import cmd1, cmd2
 
 
 def main() -> None:
     """Demonstrate main with CLI."""
```

### Comparing `argufy-0.1.2b2/examples/multiparse/cmd1.py` & `argufy-0.1.2b3/examples/multiparse/cmd1.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/multiparse/cmd2.py` & `argufy-0.1.2b3/examples/multiparse/cmd2.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/parents/parents.py` & `argufy-0.1.2b3/examples/parents/parents.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/subcommands/__main__.py` & `argufy-0.1.2b3/examples/subcommands/__main__.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/subcommands/cmd1.py` & `argufy-0.1.2b3/examples/subcommands/cmd1.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/examples/subcommands/cmd2.py` & `argufy-0.1.2b3/examples/subcommands/cmd2.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/src/argufy/__init__.py` & `argufy-0.1.2b3/src/argufy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 from argufy.formatter import ArgufyHelpFormatter  # noqa
 from argufy.parser import Parser  # noqa
 
 __author__ = 'Jesse P. Johnson'
 __author_email__ = 'jpj6652@gmail.com'
 __title__ = 'argufy'
 __description__ = 'Inspection based parser built on argparse.'
-__version__ = '0.1.2b2'
+__version__ = '0.1.2b3'
 __license__ = 'Apache-2.0'
 __copyright__ = 'Copyright 2020 Jesse Johnson.'
 __all__: List[str] = ['Argument', 'ArgufyHelpFormatter', 'Parser']
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `argufy-0.1.2b2/src/argufy/argument.py` & `argufy-0.1.2b3/src/argufy/argument.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 # license: Apache 2.0, see LICENSE for more details.
 """Arguments for inspection based CLI parser."""
 
 # import logging
 import re
 import typing
 from ast import literal_eval
-from inspect import Parameter, _empty as empty
+from inspect import Parameter
+from inspect import _empty as empty
+from pydoc import locate
 from typing import Any, List, Optional, Union
 
 from docstring_parser.common import DocstringParam
 
 
-class Argument:
+class Argument:  # pylint: disable=too-many-instance-attributes
     """Represent argparse arguments."""
 
     __short_flags: List[str] = ['-h']
 
     def __init__(
         self,
-        docstring: DocstringParam,
+        docstring: Optional[DocstringParam] = None,
         parameters: Optional[Parameter] = None,
     ) -> None:
         """Initialize argparse argument."""
         # self.attributes: Dict[Any, Any] = {}
 
         # set parameter default
         if parameters:
@@ -67,15 +69,15 @@
                 self.type = typing.get_origin(parameters.annotation)
         else:
             self.type = parameters.annotation
 
     def __parse_docstring(self, docstring: DocstringParam) -> None:
         """Get parameter types from docstring."""
         # Parse docstring for parameter types and defaults
-        if ',' in docstring.type_name:
+        if docstring.type_name and ',' in docstring.type_name:
             for arg in docstring.type_name.split(',', 1):
                 if not hasattr(self, 'type'):
                     # NOTE: Limit input that eval will parse
                     if arg.__class__.__module__ == 'builtins':
                         self.type = literal_eval(arg) if arg != 'str' else str
                 if arg.lower() == 'optional' and not hasattr(self, 'default'):
                     # XXX: should optional not exist instead of 'None'
@@ -84,15 +86,15 @@
                 if re.search(r'^\s*\{.*\}\s*$', arg):
                     self.choices = literal_eval(arg.strip())
         if not hasattr(self, 'type'):
             # NOTE: Limit input that eval will parse
             if docstring.type_name in (
                 ('float', 'int', 'str', 'list', 'dict', 'tuple')
             ):
-                self.type = eval(docstring.type_name)  # nosec
+                self.type = locate(docstring.type_name)
 
     @property
     def name(self) -> List[str]:
         """Get argparse command/argument name."""
         return self.__name
 
     @name.setter
```

### Comparing `argufy-0.1.2b2/src/argufy/formatter.py` & `argufy-0.1.2b3/src/argufy/formatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 """Simple argparse."""
 
 # from pprint import pprint
 import argparse
 from argparse import Action, HelpFormatter
-from typing import Iterable, Optional
+from typing import TYPE_CHECKING, Iterable, Optional
 
 import colorama
 from colorama import Fore, Style
 
+if TYPE_CHECKING:
+    from argparse import (
+        # _ArgumentGroup as ArgumentGroup,
+        _MutuallyExclusiveGroup as MutuallyExclusiveGroup,
+    )
+
 colorama.init()
 
 
 class ArgufyHelpFormatter(HelpFormatter):
     """Provide formatting for Argufy."""
 
     # argparse.HelpFormatter(prog, max_help_position=80, width=130)
 
     def add_usage(
         self,
         usage: Optional[str],
         actions: Iterable[Action],
-        groups: Iterable[argparse._ArgumentGroup],
+        # groups: Iterable['ArgumentGroup'],
+        groups: Iterable['MutuallyExclusiveGroup'],
         prefix: Optional[str] = 'usage: ',
     ) -> None:
         """Format usage message."""
         if prefix is not None:
             prefix = self.font(prefix)
-        super(ArgufyHelpFormatter, self).add_usage(
-            usage, actions, groups, prefix
-        )
+        super().add_usage(usage, actions, groups, prefix)
 
     @staticmethod
     def font(text: str, width: str = 'BRIGHT') -> str:
         """Set the string thickness."""
         return getattr(Style, width) + text + Style.RESET_ALL
 
     @staticmethod
@@ -53,31 +58,26 @@
     #         ArgufyHelpFormatter, self
     #     )._format_action_invocation(action)
 
     def _expand_help(self, action: Action) -> str:
         """Format help message."""
         if action.help:
             return self.shade(
-                super(ArgufyHelpFormatter, self)
-                ._expand_help(action)
-                .rstrip('.')
-                .lower(),
+                super()._expand_help(action).rstrip('.').lower(),
                 'YELLOW',
             )
-        else:
-            return ''
+        return ''
 
     def _format_action(self, action: Action) -> str:
         """Format arguments."""
         if isinstance(action, argparse._SubParsersAction._ChoicesPseudoAction):
             subcommand = self.shade(
                 self.font(self._format_action_invocation(action))
             )
             help_text = self._expand_help(action)
             # TODO: calculate correct spacing
             return f"    {subcommand.ljust(37)}{help_text}\n"
-        else:
-            # action.option_strings = [
-            #     self.font(self.shade(option))
-            #     for option in action.option_strings
-            # ]
-            return super(ArgufyHelpFormatter, self)._format_action(action)
+        # action.option_strings = [
+        #     self.font(self.shade(option))
+        #     for option in action.option_strings
+        # ]
+        return super()._format_action(action)
```

### Comparing `argufy-0.1.2b2/src/argufy/parser.py` & `argufy-0.1.2b3/src/argufy/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,57 +2,57 @@
 # license: Apache 2.0, see LICENSE for more details.
 """Argufy is an inspection based CLI parser."""
 
 import inspect
 import logging
 import sys
 import typing
-from argparse import ArgumentParser, _SubParsersAction as SubParsersAction
+from argparse import ArgumentParser
+from argparse import _SubParsersAction as SubParsersAction
 
 # from dataclasses import is_dataclass
-from inspect import (
-    Parameter,
-    _ParameterKind as ParameterKind,
-    _empty as empty,
-)
+from inspect import Parameter
+from inspect import _empty as empty
+from inspect import _ParameterKind as ParameterKind
 from types import ModuleType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
 )
 
-from docstring_parser import parse as docstring_parse
+from docstring_parser import parse as docparse
 
 from argufy.argument import Argument
 from argufy.formatter import ArgufyHelpFormatter
 
 if TYPE_CHECKING:
     from argparse import Namespace
-    from docstring_parser import DocstringParam
     from inspect import Signature
 
+    from docstring_parser import Docstring, DocstringParam
+
 log = logging.getLogger(__name__)
 
 # Define function as parameters for MyPy
 F = TypeVar('F', bound=Callable[..., Any])
 
 
 class Parser(ArgumentParser):
     """Provide CLI parser for function."""
 
     exclude_prefixes = ('@', '_')
 
-    def __init__(self, *args: str, **kwargs: Any) -> None:
+    def __init__(self, **kwargs: Any) -> None:
         """Initialize parser.
 
         Parameters
         ----------
         prog: str
             The name of the program
         usage: str
@@ -81,31 +81,27 @@
             Allows long options to be abbreviated if the abbreviation is
             unambiguous
 
         """
         # TODO: handle environment variables
 
         module = self.__get_parent_module()
-        if module:
-            docstring = docstring_parse(module.__doc__)
+        if module and module.__doc__:
+            docstring = docparse(module.__doc__)
             if not kwargs.get('description'):
                 kwargs['description'] = docstring.short_description
-
             if 'prog' not in kwargs:
                 kwargs['prog'] = module.__name__.split('.')[0]
-
         if 'version' in kwargs:
             self.prog_version = kwargs.pop('version')
-
         # if 'prefix' in kwargs:
         #     self.prefix = kwargs.pop('prefix')
         # else:
         #     self.prefix = kwargs['prog'].upper()
-        # log.debug(self.prefix)
-
+        # log.debug(str(self.prefix))
         if 'log_level' in kwargs:
             log.setLevel(getattr(logging, kwargs.pop('log_level').upper()))
         if 'log_handler' in kwargs:
             log_handler = kwargs.pop('log_handler')
             log.addHandler(logging.StreamHandler(log_handler))
 
         self.use_module_args = kwargs.pop('use_module_args', False)
@@ -155,53 +151,46 @@
         }
 
     @staticmethod
     def _get_excludes(exclude_prefixes: Tuple[str, ...] = tuple()) -> tuple:
         """Combine class excludes with instance."""
         if exclude_prefixes != ():
             return tuple(exclude_prefixes) + Parser.exclude_prefixes
-        else:
-            return Parser.exclude_prefixes
+        return Parser.exclude_prefixes
 
     @staticmethod
     def __get_description(
-        name: str,
-        docstring: 'DocstringParam',
-    ) -> Optional[str]:
+        name: str, docstring: 'Docstring'
+    ) -> Optional['DocstringParam']:
         """Get argument description from docstring."""
         return next((d for d in docstring.params if d.arg_name == name), None)
 
     @staticmethod
     def __get_keyword_args(
-        signature: 'Signature',
-        docstring: 'DocstringParam',
+        signature: 'Signature', docstring: 'Docstring'
     ) -> List[str]:
         """Get keyward arguments from docstring."""
-        parameters = [x for x in signature.parameters]
         return [
             x.arg_name
             for x in docstring.params
-            if x.arg_name not in parameters
+            if x.arg_name not in list(signature.parameters)
         ]
 
     @staticmethod
-    def __generate_parameter(
-        name: str,
-        module: ModuleType,
-    ) -> Parameter:
+    def __generate_parameter(name: str, module: ModuleType) -> Parameter:
         """Generate inpect parameter."""
         parameter = Parameter(
             name,
             ParameterKind.POSITIONAL_OR_KEYWORD,
             default=getattr(module, name),
             annotation=empty,
         )
         return parameter
 
-    def add_commands(
+    def add_commands(  # pylint: disable=too-many-locals,too-many-branches
         self,
         module: ModuleType,
         parser: Optional[ArgumentParser] = None,
         exclude_prefixes: tuple = tuple(),
         command_type: Optional[str] = None,
     ) -> 'Parser':
         """Add commands.
@@ -225,15 +214,15 @@
         """
         # use self or an existing parser
         if not parser:
             parser = self
         parser.formatter_class = ArgufyHelpFormatter
 
         module_name = module.__name__.split('.')[-1]
-        docstring = docstring_parse(module.__doc__)
+        docstring = docparse(module.__doc__) if module.__doc__ else None
         excludes = Parser._get_excludes(exclude_prefixes)
 
         # use exsiting subparser or create a new one
         if not any(isinstance(x, SubParsersAction) for x in parser._actions):
             # TODO: use metavar for hidden commands
             parser.add_subparsers(dest=module_name, parser_class=Parser)
 
@@ -246,15 +235,15 @@
         # set command name scheme
         if command_type is None:
             command_type = self.command_type
 
         # create subcommand for command
         if command_type == 'subcommand':
             if command:
-                msg = docstring.short_description
+                msg = docstring.short_description if docstring else None
                 subcommand = command.add_parser(
                     module_name.replace('_', '-'),
                     description=msg,
                     formatter_class=self.formatter_class,
                     help=msg,
                 )
                 subcommand.set_defaults(mod=module)
@@ -264,25 +253,26 @@
                 module=module,
                 parser=subcommand,
                 exclude_prefixes=Parser._get_excludes(exclude_prefixes),
                 command_type='command',
             )
 
         # TODO: separate into method
+        # pylint: disable-next=too-many-nested-blocks
         for name, value in inspect.getmembers(module):
             # TODO: Possible singledispatch candidate
             if not name.startswith(excludes):
                 # skip classes for now
                 if inspect.isclass(value):
                     # TODO: check if dataclass instance
                     # TODO: check if class instance
                     continue  # pragma: no cover
 
                 # create commands from functions
-                elif inspect.isfunction(value):
+                if inspect.isfunction(value):
                     # TODO: Turn parameter-less function into switch
 
                     # merge builder function maing_args into parser
                     if (
                         self.main_args_builder
                         and name == self.main_args_builder['function']
                     ):
@@ -301,26 +291,28 @@
                         if command:
                             # control command name format
                             if self.command_scheme == 'chain':
                                 cmd_name = f"{module_name}.{name}"
                             else:
                                 cmd_name = name
 
-                            msg = docstring_parse(
-                                value.__doc__
-                            ).short_description
+                            msg = (
+                                docparse(value.__doc__).short_description
+                                if value.__doc__
+                                else None
+                            )
                             cmd = command.add_parser(
                                 cmd_name.replace('_', '-'),
                                 description=msg,
                                 formatter_class=self.formatter_class,
                                 help=msg,
                             )
                             cmd.set_defaults(mod=module, fn=value)
                         # add arguments from function
-                        # log.debug(f"command {name} {value} {cmd}")
+                        # log.debug("command %s %s %s", name, value, cmd)
                         self.add_arguments(value, cmd)
 
                 # create arguments from module varibles
                 elif (
                     self.use_module_args
                     and not isinstance(value, ModuleType)
                     and not hasattr(typing, name)
@@ -329,15 +321,17 @@
                         and name != self.main_args_builder['instance']
                     )
                 ):
                     # TODO: Reconcile inspect parameters with dict
                     # TODO: use argparse.SUPPRESS for hidden arguments
                     arguments = self.__clean_args(
                         Argument(
-                            self.__get_description(name, docstring),
+                            self.__get_description(name, docstring)
+                            if docstring
+                            else None,
                             self.__generate_parameter(name, module),
                         )
                     )
                     name = arguments.pop('name')
                     parser.add_argument(*name, **arguments)
         return self
 
@@ -359,38 +353,39 @@
             Return object itself to allow chaining functions.
 
         """
         if not parser:
             parser = self
 
         # prep object for inspection
-        docstring = docstring_parse(obj.__doc__)
+        docstring = docparse(obj.__doc__)
         signature = inspect.signature(obj)
 
         # populate subcommand with keyword arguments
         for arg in signature.parameters:
             param = signature.parameters[arg]
             description = self.__get_description(arg, docstring)
-            # log.debug(f"param: {param}, {param.kind}")
+            log.debug("param: %s, %s", param, param.kind)
 
             if not param.kind == Parameter.VAR_KEYWORD:
-                log.debug(f"param annotation: {param.annotation}")
+                log.debug("param annotation: %s", param.annotation)
                 argument = self.__clean_args(Argument(description, param))
                 name = argument.pop('name')
                 # print(name, argument)
                 parser.add_argument(*name, **argument)
 
         # populate options
-        # log.debug(f"params {params}")
-        for arg in self.__get_keyword_args(signature, docstring):
-            description = self.__get_description(arg, docstring)
-            arguments = self.__clean_args(Argument(description))
-            parser.add_argument(f"--{arg.replace('_', '-')}", **arguments)
+        # log.debug("params %s", params)
+        if docstring:
+            for arg in self.__get_keyword_args(signature, docstring):
+                description = self.__get_description(arg, docstring)
+                arguments = self.__clean_args(Argument(docstring=description))
+                parser.add_argument(f"--{arg.replace('_', '-')}", **arguments)
 
-        # log.debug(f"arguments {arguments}")
+        # log.debug("arguments %s", arguments)
         # TODO for any docstring not collected parse here (args, kwargs)
         # log.debug('docstring params', docstring.params)
         return self
 
     def __set_main_arguments(self, ns: 'Namespace') -> 'Namespace':
         """Separate and set main arguments from builder function.
 
@@ -441,24 +436,28 @@
         if 'mod' in ns:
             mod = vars(ns).pop('mod')
         else:
             mod = None
 
         # separate namespace from other variables
         signature = inspect.signature(fn)
-        docstring = docstring_parse(fn.__doc__)
+        docstring = docparse(fn.__doc__) if fn.__doc__ else None
 
         # inspect non-signature keyword args
-        keywords = self.__get_keyword_args(signature, docstring)
+        keywords = (
+            self.__get_keyword_args(signature, docstring)
+            if docstring
+            else list(signature.parameters)
+        )
         args = [
             {k: vars(ns).pop(k)}
             for k in list(vars(ns).keys()).copy()
             if not signature.parameters.get(k) and k not in keywords
         ]
-        log.debug(f"arguments {args}, {keywords}")
+        log.debug("arguments %s, %s", args, keywords)
 
         # set module variables
         if mod and self.use_module_args:
             for arg in args:
                 for k, v in arg.items():
                     mod.__dict__[k] = v
         return ns
@@ -519,15 +518,15 @@
         -------
         Optional[Callable[[F], F]]:
             Call function with arguments.
 
         """
         # parse variables
         arguments, namespace = self.retrieve(args, ns)
-        log.debug(f"dispatch: {arguments}, {namespace}")
+        log.debug("dispatch: %s, %s", arguments, namespace)
 
         main_ns_result = self.__set_main_arguments(namespace)
 
         # call function with variables
         if 'fn' in namespace:
             ns_vars = vars(namespace)
             fn = ns_vars.pop('fn')
```

### Comparing `argufy-0.1.2b2/tests/test_argument_type_hints.py` & `argufy-0.1.2b3/tests/test_argument_type_hints.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/tests/commands/command_parser.py` & `argufy-0.1.2b3/tests/commands/command_parser.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/tests/commands/test_command_parser.py` & `argufy-0.1.2b3/tests/commands/test_command_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 Attributes
 ----------
 check_attribute: bool
     Check document attributes
 
 '''
 
+import sys
 from ast import literal_eval
 
 import pytest
-import sys
 
-from argufy import __version__, Parser
+from argufy import Parser, __version__
 
 sys.path.append('.')
 import command_parser  # noqa: E402
+
 # module = sys.modules[__name__]
 
 
 def test_help():
     '''Do help function for CLI.'''
     parser = Parser(version=__version__)
     parser.add_commands(command_parser, exclude_prefixes=['test_'])
```

### Comparing `argufy-0.1.2b2/tests/docstrings/test_google.py` & `argufy-0.1.2b3/tests/docstrings/test_google.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/tests/docstrings/test_numpy.py` & `argufy-0.1.2b3/tests/docstrings/test_numpy.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/tests/docstrings/test_restructured.py` & `argufy-0.1.2b3/tests/docstrings/test_restructured.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/tests/subcommands/subcommands_parser.py` & `argufy-0.1.2b3/tests/subcommands/subcommands_parser.py`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/.gitignore` & `argufy-0.1.2b3/.gitignore`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/LICENSE` & `argufy-0.1.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/README.md` & `argufy-0.1.2b3/README.md`

 * *Files identical despite different names*

### Comparing `argufy-0.1.2b2/pyproject.toml` & `argufy-0.1.2b3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling>=1.11.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "argufy"
-version = "0.1.2b2"
+version = "0.1.2b3"
 description = "Inspection based parser based on argparse."
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["parser"]
 requires-python = ">=3.6.2"
 authors = [{name = "Jesse P. Johnson", email = "jpj6652@gmail.com"}]
 maintainers = [{name = "Jesse P. Johnson", email = "jpj6652@gmail.com"}]
@@ -20,49 +20,51 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries"
 ]
 dependencies = [
     "docstring-parser>=0.7.2",
-    "colorama>=0.4.4",
+    "colorama>=0.4.4"
 ]
 
 [project.optional-dependencies]
-dev = [
-    # build
-    "invoke>=1.4.1",
+build = [
+    "build",
     "proman-versioning>=0.5.0-alpha.2",
-    "twine",
+    "twine"
+]
+dev = [
     # test
     "pytest>=6.2.5",
     "pytest-cov>=2.10.0",
     "tox>=3.25.0",
     # sca
-    "mypy>=0.942",
-    "bandit>=1.6.2",
-    "pylint>=2.9.5",
+    "mypy>=1",
+    "pylint>=3",
     # style
     "black==22.3.0",
     "isort>=5.10.1",
     "flake8>=3.8.3",
     # sast
     "bandit>=1.6.2",
-    "safety>=1.9.0",
+    "safety>=1.9.0"
 ]
 docs = [
     "docstr-coverage>=1.2.0",
     "mkdocs>=1.2.2",
-    "mkdocstrings>=0.16.2",
     "mkdocs-material>=7.2.0",
-    "pydocstyle[toml]>=6.1.1",
+    "mkdocstrings[python]>=0.16.2",
+    "pydocstyle[toml]>=6.1.1"
 ]
 
 [project.urls]
 homepage = "https://github.com/kuwv/python-argufy"
 repository = "https://github.com/kuwv/python-argufy"
 documentation = "https://kuwv.github.io/python-argufy/"
 
@@ -93,21 +95,40 @@
 line-length = 79
 skip-string-normalization = true
 include = '\.pyi?$'
 exclude = '''
 (
   /(
     | \.git
+    | \.github
     | \.mypy_cache
     | \.pytest_cache
-    | _build
     | build
     | dist
+    | docs
+    | site
   )
 )
 '''
 
+[tool.pylint]
+fail-under = 9.0
+
+[tool.pylint."FORMAT"]
+max-line-length = 79
+
+[tool.pylint."MESSAGES CONTROL"]
+disable = [
+    "C0103",
+    "R0903",
+    "W0212",
+    "W0715"
+]
+
+[tool.pylint."MISCELLANEOUS"]
+notes = []
+
 [tool.mypy]
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_untyped_defs = true
 ignore_missing_imports = true
```

### Comparing `argufy-0.1.2b2/PKG-INFO` & `argufy-0.1.2b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: argufy
-Version: 0.1.2b2
+Version: 0.1.2b3
 Summary: Inspection based parser based on argparse.
 Project-URL: homepage, https://github.com/kuwv/python-argufy
 Project-URL: repository, https://github.com/kuwv/python-argufy
 Project-URL: documentation, https://kuwv.github.io/python-argufy/
 Author-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 Maintainer-email: "Jesse P. Johnson" <jpj6652@gmail.com>
 License:                                  Apache License
@@ -217,37 +217,40 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6.2
 Requires-Dist: colorama>=0.4.4
 Requires-Dist: docstring-parser>=0.7.2
+Provides-Extra: build
+Requires-Dist: build; extra == 'build'
+Requires-Dist: proman-versioning>=0.5.0-alpha.2; extra == 'build'
+Requires-Dist: twine; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: bandit>=1.6.2; extra == 'dev'
 Requires-Dist: black==22.3.0; extra == 'dev'
 Requires-Dist: flake8>=3.8.3; extra == 'dev'
-Requires-Dist: invoke>=1.4.1; extra == 'dev'
 Requires-Dist: isort>=5.10.1; extra == 'dev'
-Requires-Dist: mypy>=0.942; extra == 'dev'
-Requires-Dist: proman-versioning>=0.5.0-alpha.2; extra == 'dev'
-Requires-Dist: pylint>=2.9.5; extra == 'dev'
+Requires-Dist: mypy>=1; extra == 'dev'
+Requires-Dist: pylint>=3; extra == 'dev'
 Requires-Dist: pytest-cov>=2.10.0; extra == 'dev'
 Requires-Dist: pytest>=6.2.5; extra == 'dev'
 Requires-Dist: safety>=1.9.0; extra == 'dev'
 Requires-Dist: tox>=3.25.0; extra == 'dev'
-Requires-Dist: twine; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: docstr-coverage>=1.2.0; extra == 'docs'
 Requires-Dist: mkdocs-material>=7.2.0; extra == 'docs'
 Requires-Dist: mkdocs>=1.2.2; extra == 'docs'
-Requires-Dist: mkdocstrings>=0.16.2; extra == 'docs'
+Requires-Dist: mkdocstrings[python]>=0.16.2; extra == 'docs'
 Requires-Dist: pydocstyle[toml]>=6.1.1; extra == 'docs'
 Description-Content-Type: text/markdown
 
 # python-argufy
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Build Status](https://travis-ci.org/kuwv/python-argufy.svg?branch=master)](https://travis-ci.org/kuwv/python-argufy)
```

