# Comparing `tmp/lego_handlers-1.1.1.tar.gz` & `tmp/lego_handlers-1.1.2.tar.gz`

## Comparing `lego_handlers-1.1.1.tar` & `lego_handlers-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/requirements-dev.lock
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/requirements.lock
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/.github/workflows/CD.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/scripts/new-release.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/src/lego_handlers/__init__.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/src/lego_handlers/components.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/src/lego_handlers/py.typed
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/tests/test_something.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/.gitignore
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/README.md
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/requirements.lock
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/.github/workflows/CD.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/scripts/new-release.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/src/lego_handlers/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/src/lego_handlers/components.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/src/lego_handlers/py.typed
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/tests/test_something.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/.gitignore
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/README.md
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-1.1.2/PKG-INFO
```

### Comparing `lego_handlers-1.1.1/requirements-dev.lock` & `lego_handlers-1.1.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.1/.github/workflows/CD.yml` & `lego_handlers-1.1.2/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.1/.github/workflows/CI.yml` & `lego_handlers-1.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.1/scripts/new-release.py` & `lego_handlers-1.1.2/scripts/new-release.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-1.1.1/src/lego_handlers/__init__.py` & `lego_handlers-1.1.2/src/lego_handlers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 from lego_handlers.components import (
     DomainError,
     DomainEvent,
     ResponseData,
 )
 
 T = TypeVar("T")
+E = TypeVar("E", bound=DomainError)
+R = TypeVar("R", bound=ResponseData)
 
 
 async def process_result(
-    result: Result[tuple[ResponseData, list[DomainEvent]], DomainError],
-    handler: Callable[[Result[ResponseData, DomainError]], T],
+    result: Result[tuple[R, list[DomainEvent]], E],
+    handler: Callable[[Result[R, E]], T],
     *,
     publish_events: bool,
 ) -> T:
     if isinstance(result, Ok):
         response_data, events = result.unwrap()
         if publish_events:
             await _publish_events(events=events)
```

### Comparing `lego_handlers-1.1.1/tests/test_something.py` & `lego_handlers-1.1.2/tests/test_something.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from typing import TypeAlias
 from uuid import UUID, uuid4
 
 import lego_handlers
 from lego_handlers.components import (
     DomainError,
     DomainEvent,
     ResponseData,
@@ -29,19 +30,22 @@
 
 
 class ZeroInitialBalanceError(DomainError):
     def __init__(self) -> None:
         super().__init__("Not possible to create account with zero initial balance.")
 
 
+_DomainErrors: TypeAlias = ZeroInitialBalanceError | NegativeInitialBalanceError
+
+
 def create_account(
     initial_balance: int,
 ) -> Result[
     tuple[ResponseCreateAccount, list[DomainEvent]],
-    ZeroInitialBalanceError | NegativeInitialBalanceError,
+    _DomainErrors,
 ]:
     events: list[DomainEvent] = []
     if initial_balance < 0:
         return Err(NegativeInitialBalanceError())
 
     if initial_balance == 0:
         return Err(ZeroInitialBalanceError())
@@ -52,15 +56,17 @@
         (
             ResponseCreateAccount(account_id=uuid4(), initial_balance=initial_balance),
             events,
         )
     )
 
 
-def _result_hanlder(result: Result[ResponseData, DomainError]) -> str:
+def _result_hanlder(
+    result: Result[ResponseCreateAccount, _DomainErrors],
+) -> str:
     match result:
         case Ok():
             return "Data"
         case Err():
             return str(result)
```

### Comparing `lego_handlers-1.1.1/pyproject.toml` & `lego_handlers-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lego-handlers"
-version = "1.1.1"
+version = "1.1.2"
 description = "Add your description here"
 authors = [{ name = "Tomperez98", email = "tomasperezalvarez@gmail.com" }]
 dependencies = [
     "result>=0.16.1",
 ]
 readme = "README.md"
 requires-python = ">= 3.10"
```

