# Comparing `tmp/lego_handlers-1.1.0.tar.gz` & `tmp/lego_handlers-1.1.1.tar.gz`

## Comparing `lego_handlers-1.1.0.tar` & `lego_handlers-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/requirements.lock
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/.github/workflows/CD.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/scripts/new-release.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/src/lego_handlers/__init__.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/src/lego_handlers/components.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/src/lego_handlers/py.typed
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/tests/test_something.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/.gitignore
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/README.md
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/requirements.lock
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/.github/workflows/CD.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/scripts/new-release.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/src/lego_handlers/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/src/lego_handlers/components.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/src/lego_handlers/py.typed
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/tests/test_something.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/.gitignore
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/README.md
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/PKG-INFO
```

### Comparing `lego_handlers-1.1.0/requirements-dev.lock` & `lego_handlers-1.1.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.0/.github/workflows/CD.yml` & `lego_handlers-1.1.1/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.0/.github/workflows/CI.yml` & `lego_handlers-1.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.0/scripts/new-release.py` & `lego_handlers-1.1.1/scripts/new-release.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.0/src/lego_handlers/__init__.py` & `lego_handlers-1.1.1/src/lego_handlers/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Lego handlers."""
 
 import asyncio
 from collections.abc import Callable
 from typing import TypeVar
 
 from result import Err, Ok, Result
+from typing_extensions import assert_never
 
 from lego_handlers.components import (
     DomainError,
     DomainEvent,
     ResponseData,
 )
 
@@ -17,21 +18,22 @@
 
 async def process_result(
     result: Result[tuple[ResponseData, list[DomainEvent]], DomainError],
     handler: Callable[[Result[ResponseData, DomainError]], T],
     *,
     publish_events: bool,
 ) -> T:
-    match result:
-        case Ok((response, events)):
-            if publish_events:
-                await _publish_events(events=events)
-            return handler(Ok(response))
-        case Err():
-            return handler(result)
+    if isinstance(result, Ok):
+        response_data, events = result.unwrap()
+        if publish_events:
+            await _publish_events(events=events)
+        return handler(Ok(response_data))
+    if isinstance(result, Err):
+        return handler(result)
+    assert_never(result)
 
 
 async def _publish_events(events: list[DomainEvent]) -> None:
     """Publish events."""
     await asyncio.gather(
         *(event.publish() for event in events), return_exceptions=False
     )
```

### Comparing `lego_handlers-1.1.0/tests/test_something.py` & `lego_handlers-1.1.1/tests/test_something.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.0/pyproject.toml` & `lego_handlers-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lego-handlers"
-version = "1.1.0"
+version = "1.1.1"
 description = "Add your description here"
 authors = [{ name = "Tomperez98", email = "tomasperezalvarez@gmail.com" }]
 dependencies = [
     "result>=0.16.1",
 ]
 readme = "README.md"
 requires-python = ">= 3.10"
```

