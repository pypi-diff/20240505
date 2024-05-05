# Comparing `tmp/lego_handlers-1.0.0.tar.gz` & `tmp/lego_handlers-1.1.0.tar.gz`

## Comparing `lego_handlers-1.0.0.tar` & `lego_handlers-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/requirements-dev.lock
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/requirements.lock
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/.github/workflows/CD.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/scripts/new-release.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/src/lego_handlers/__init__.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/src/lego_handlers/components.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/src/lego_handlers/py.typed
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/tests/test_something.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/.gitignore
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/README.md
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/requirements-dev.lock
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/requirements.lock
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/.github/workflows/CD.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/scripts/new-release.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/src/lego_handlers/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/src/lego_handlers/components.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/src/lego_handlers/py.typed
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/tests/test_something.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/.gitignore
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/README.md
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/PKG-INFO
```

### Comparing `lego_handlers-1.0.0/requirements-dev.lock` & `lego_handlers-1.1.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.0.0/.github/workflows/CD.yml` & `lego_handlers-1.1.0/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.0.0/.github/workflows/CI.yml` & `lego_handlers-1.1.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.0.0/scripts/new-release.py` & `lego_handlers-1.1.0/scripts/new-release.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.0.0/src/lego_handlers/__init__.py` & `lego_handlers-1.1.0/src/lego_handlers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 
 from lego_handlers.components import (
     DomainError,
     DomainEvent,
     ResponseData,
 )
 
-R = TypeVar("R", bound=ResponseData)
 T = TypeVar("T")
 
 
 async def process_result(
-    result: Result[tuple[R, list[DomainEvent]], DomainError],
-    handler: Callable[[Result[R, DomainError]], T],
+    result: Result[tuple[ResponseData, list[DomainEvent]], DomainError],
+    handler: Callable[[Result[ResponseData, DomainError]], T],
     *,
     publish_events: bool,
 ) -> T:
     match result:
         case Ok((response, events)):
             if publish_events:
                 await _publish_events(events=events)
```

### Comparing `lego_handlers-1.0.0/tests/test_something.py` & `lego_handlers-1.1.0/tests/test_something.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.0.0/pyproject.toml` & `lego_handlers-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lego-handlers"
-version = "1.0.0"
+version = "1.1.0"
 description = "Add your description here"
 authors = [{ name = "Tomperez98", email = "tomasperezalvarez@gmail.com" }]
 dependencies = [
     "result>=0.16.1",
 ]
 readme = "README.md"
 requires-python = ">= 3.10"
```

