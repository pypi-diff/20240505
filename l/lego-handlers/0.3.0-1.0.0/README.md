# Comparing `tmp/lego_handlers-0.3.0.tar.gz` & `tmp/lego_handlers-1.0.0.tar.gz`

## Comparing `lego_handlers-0.3.0.tar` & `lego_handlers-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/requirements-dev.lock
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/requirements.lock
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/.github/workflows/CD.yml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/scripts/new-release.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/src/lego_handlers/__init__.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/src/lego_handlers/components.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/src/lego_handlers/py.typed
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/tests/test_something.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/.gitignore
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/README.md
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/requirements-dev.lock
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/requirements.lock
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/.github/workflows/CD.yml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/.vscode/settings.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/scripts/new-release.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/src/lego_handlers/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/src/lego_handlers/components.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/src/lego_handlers/py.typed
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/tests/test_something.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/.gitignore
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/README.md
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lego_handlers-1.0.0/PKG-INFO
```

### Comparing `lego_handlers-0.3.0/requirements-dev.lock` & `lego_handlers-1.0.0/requirements-dev.lock`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
-coverage==7.5.0
+coverage==7.5.1
     # via pytest-cov
 exceptiongroup==1.2.1
     # via pytest
 iniconfig==2.0.0
     # via pytest
 mypy==1.10.0
 mypy-extensions==1.0.0
     # via mypy
 packaging==24.0
     # via pytest
 pluggy==1.5.0
     # via pytest
-pytest==8.1.1
+pytest==8.2.0
     # via pytest-asyncio
     # via pytest-cov
 pytest-asyncio==0.23.6
 pytest-cov==5.0.0
 result==0.16.1
     # via lego-handlers
 toml==0.10.2
```

### Comparing `lego_handlers-0.3.0/.github/workflows/CD.yml` & `lego_handlers-1.0.0/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-0.3.0/.github/workflows/CI.yml` & `lego_handlers-1.0.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lego_handlers-0.3.0/scripts/new-release.py` & `lego_handlers-1.0.0/scripts/new-release.py`

 * *Files identical despite different names*

### Comparing `lego_handlers-0.3.0/tests/test_something.py` & `lego_handlers-1.0.0/tests/test_something.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from dataclasses import dataclass
-from typing import TypeAlias
 from uuid import UUID, uuid4
 
 import lego_handlers
 from lego_handlers.components import (
-    CommandComponent,
     DomainError,
     DomainEvent,
-    ResponseComponent,
+    ResponseData,
 )
 from result import Err, Ok, Result
 
 
 @dataclass(frozen=True)
-class ResponseCreateAccount(ResponseComponent):
+class ResponseCreateAccount(ResponseData):
     account_id: UUID
     initial_balance: int
 
 
 @dataclass(frozen=True)
 class AccountCreated(DomainEvent):
     async def publish(self) -> None: ...
@@ -31,44 +29,57 @@
 
 
 class ZeroInitialBalanceError(DomainError):
     def __init__(self) -> None:
         super().__init__("Not possible to create account with zero initial balance.")
 
 
-CreateAccountErrors: TypeAlias = NegativeInitialBalanceError | ZeroInitialBalanceError
+def create_account(
+    initial_balance: int,
+) -> Result[
+    tuple[ResponseCreateAccount, list[DomainEvent]],
+    ZeroInitialBalanceError | NegativeInitialBalanceError,
+]:
+    events: list[DomainEvent] = []
+    if initial_balance < 0:
+        return Err(NegativeInitialBalanceError())
+
+    if initial_balance == 0:
+        return Err(ZeroInitialBalanceError())
+
+    events.append(AccountCreated())
+
+    return Ok(
+        (
+            ResponseCreateAccount(account_id=uuid4(), initial_balance=initial_balance),
+            events,
+        )
+    )
 
 
-@dataclass(frozen=True)
-class CreateAccount(CommandComponent[CreateAccountErrors, ResponseCreateAccount]):
-    initial_balance: int
-
-    def run(
-        self, events: list[DomainEvent]
-    ) -> Result[ResponseCreateAccount, CreateAccountErrors]:
-        if self.initial_balance < 0:
-            return Err(NegativeInitialBalanceError())
-
-        if self.initial_balance == 0:
-            return Err(ZeroInitialBalanceError())
-
-        events.append(AccountCreated())
-
-        return Ok(
-            ResponseCreateAccount(
-                account_id=uuid4(), initial_balance=self.initial_balance
-            )
-        )
+def _result_hanlder(result: Result[ResponseData, DomainError]) -> str:
+    match result:
+        case Ok():
+            return "Data"
+        case Err():
+            return str(result)
 
 
 async def test_run_command() -> None:
     intial_balance = 10
-    create_account_events: list[DomainEvent] = []
-    command_result = CreateAccount(
+    command_result = create_account(
         initial_balance=intial_balance,
-    ).run(
-        events=create_account_events,
     )
     assert isinstance(command_result, Ok)
-    assert command_result.unwrap().initial_balance == intial_balance
-    assert len(create_account_events) == 1
-    await lego_handlers.publish_events(events=create_account_events)
+    response_data, events = command_result.unwrap()
+    assert response_data.initial_balance == intial_balance
+    assert len(events) == 1
+    await lego_handlers.process_result(
+        result=command_result,
+        handler=_result_hanlder,
+        publish_events=False,
+    )
+
+
+def test_error() -> None:
+    command_result = create_account(initial_balance=-10)
+    assert isinstance(command_result, Err)
```

### Comparing `lego_handlers-0.3.0/pyproject.toml` & `lego_handlers-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lego-handlers"
-version = "0.3.0"
+version = "1.0.0"
 description = "Add your description here"
 authors = [{ name = "Tomperez98", email = "tomasperezalvarez@gmail.com" }]
 dependencies = [
     "result>=0.16.1",
 ]
 readme = "README.md"
 requires-python = ">= 3.10"
```

