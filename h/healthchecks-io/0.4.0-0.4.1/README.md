# Comparing `tmp/healthchecks_io-0.4.0.tar.gz` & `tmp/healthchecks_io-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healthchecks_io-0.4.0.tar", max compression
+gzip compressed data, was "healthchecks_io-0.4.1.tar", max compression
```

## Comparing `healthchecks_io-0.4.0.tar` & `healthchecks_io-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1063 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/LICENSE
--rw-r--r--   0        0        0     1089 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/LICENSE.rst
--rw-r--r--   0        0        0     3170 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/README.rst
--rw-r--r--   0        0        0     2351 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1377 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/__init__.py
--rw-r--r--   0        0        0      227 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/client/__init__.py
--rw-r--r--   0        0        0    10633 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/client/_abstract.py
--rw-r--r--   0        0        0    20245 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/client/async_client.py
--rw-r--r--   0        0        0     6762 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/client/check_trap.py
--rw-r--r--   0        0        0      885 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/client/exceptions.py
--rw-r--r--   0        0        0    19689 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/client/sync_client.py
--rw-r--r--   0        0        0        0 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/py.typed
--rw-r--r--   0        0        0      393 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/schemas/__init__.py
--rw-r--r--   0        0        0      601 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/schemas/badges.py
--rw-r--r--   0        0        0     9572 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/schemas/checks.py
--rw-r--r--   0        0        0      469 2023-02-21 05:20:01.808061 healthchecks_io-0.4.0/src/healthchecks_io/schemas/integrations.py
--rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 healthchecks_io-0.4.0/setup.py
--rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 healthchecks_io-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1089 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/LICENSE.rst
+-rw-r--r--   0        0        0     3170 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/README.rst
+-rw-r--r--   0        0        0     2471 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1378 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/__init__.py
+-rw-r--r--   0        0        0    10427 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/_abstract.py
+-rw-r--r--   0        0        0    20246 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/async_client.py
+-rw-r--r--   0        0        0     6673 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/check_trap.py
+-rw-r--r--   0        0        0      885 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/exceptions.py
+-rw-r--r--   0        0        0    19690 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/client/sync_client.py
+-rw-r--r--   0        0        0        0 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/py.typed
+-rw-r--r--   0        0        0      394 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/schemas/__init__.py
+-rw-r--r--   0        0        0      602 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/schemas/badges.py
+-rw-r--r--   0        0        0     9557 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/schemas/checks.py
+-rw-r--r--   0        0        0      470 2024-05-05 19:26:14.618737 healthchecks_io-0.4.1/src/healthchecks_io/schemas/integrations.py
+-rw-r--r--   0        0        0     4461 1970-01-01 00:00:00.000000 healthchecks_io-0.4.1/PKG-INFO
```

### Comparing `healthchecks_io-0.4.0/LICENSE` & `healthchecks_io-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.0/LICENSE.rst` & `healthchecks_io-0.4.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.0/README.rst` & `healthchecks_io-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.0/pyproject.toml` & `healthchecks_io-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "healthchecks_io"
-version = "0.4.0"
+version = "0.4.1"
 description = "A python client package for Healthchecks.io API"
 authors = ["Andrew Herrington <andrew.the.techie@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/andrewthetechie/py-healthchecks.io"
 repository = "https://github.com/andrewthetechie/py-healthchecks.io"
 documentation = "https://py-healthchecks.io.readthedocs.io"
@@ -21,67 +21,70 @@
 	"Framework :: AsyncIO"
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/andrewthetechie/py-healthchecks.io/releases"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 pydantic = "^1.9.1"
-httpx = ">=0.23.0,<0.24.0"
+httpx = ">=0.23.0,<0.25.0"
 croniter = "^1.1.0"
-pytz = ">=2021.3,<2023.0"
+pytz = ">=2021.3,<2024.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 coverage = {extras = ["toml"], version = "^7.1"}
 safety = "^2.3.5"
 mypy = "^1.0"
 xdoctest = {extras = ["colors"], version = "^1.1.1"}
-sphinx = "^4.3.2"
+sphinx = ">=4.3.2,<6.0.0"
 sphinx-autobuild = ">=2021.3.14"
 pre-commit = "^2.21.0"
 reorder-python-imports = "^3.9.0"
 pre-commit-hooks = "^4.4.0"
 pyupgrade = "^3.3.1"
 furo = ">=2021.11.12"
 pytest-cov = "^4.0.0"
-types-croniter = "^1.3.2"
-types-pytz = "^2022.7.1"
-pytest-asyncio = "^0.20.3"
-respx = "^0.20.1"
+types-croniter = ">=1.3.2,<3.0.0"
+types-pytz = ">=2022.7.1,<2024.0.0"
+pytest-asyncio = ">=0.20.3,<0.24.0"
+respx = ">=0.20.1,<0.22.0"
 pytest-mock = "^3.10.0"
 pytest-lazy-fixture = "^0.6.3"
 pytest-xdist = "^3.2.0"
-ruff = "^0.0.249"
+ruff = ">=0.0.249,<0.4.4"
 bandit = "^1.7.4"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
 source = ["healthchecks_io"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 100
 
+[tool.bandit]
+exclude_dirs = ["tests", "noxfile.py", ".github/scripts", "test_errbot", "dist"]
+
 [tool.mypy]
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "-n 4 --ignore examples --cov=healthchecks_io --cov-report xml:.coverage.xml --cov-report=term-missing --cov-fail-under 91"
 
 [tool.ruff]
 line-length = 120
-target-version = "py37"
+target-version = "py38"
```

### Comparing `healthchecks_io-0.4.0/src/healthchecks_io/__init__.py` & `healthchecks_io-0.4.1/src/healthchecks_io/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Py Healthchecks.Io."""
+
 # set by poetry-dynamic-versioning
-__version__ = "0.4.0"  # noqa: E402
+__version__ = "0.4.1"  # noqa: E402
 
 from .client import AsyncClient  # noqa: F401, E402
 from .client import Client  # noqa: F401, E402
 from .client import CheckTrap  # noqa: F401, E402
 from .client.exceptions import BadAPIRequestError  # noqa: F401, E402
 from .client.exceptions import CheckNotFoundError  # noqa: F401, E402
 from .client.exceptions import HCAPIAuthError  # noqa: F401, E402
```

### Comparing `healthchecks_io-0.4.0/src/healthchecks_io/client/_abstract.py` & `healthchecks_io-0.4.1/src/healthchecks_io/client/_abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,15 @@
         self._finalizer = finalize(self, self._finalizer_method)
 
     @abstractmethod
     def _finalizer_method(self) -> None:  # pragma: no cover
         """Finalizer method is called by weakref.finalize when the object is dereferenced to do cleanup of clients."""
         pass
 
-    def _get_api_request_url(
-        self, path: str, params: Optional[Dict[str, Any]] = None
-    ) -> str:
+    def _get_api_request_url(self, path: str, params: Optional[Dict[str, Any]] = None) -> str:
         """Get a full request url for the healthchecks api.
 
         Args:
             path (str): Path to request from
             params (Optional[Dict[str, str]], optional): URL Parameters. Defaults to None.
 
         Returns:
@@ -161,17 +159,15 @@
         if response.status_code == 429:
             raise HCAPIRateLimitError(f"Rate limited on {response.request.url}")
 
         if response.status_code == 404:
             raise CheckNotFoundError(f"CHeck not found at {response.request.url}")
 
         if response.status_code == 400:
-            raise BadAPIRequestError(
-                f"Bad request when requesting {response.request.url}. {response.text}"
-            )
+            raise BadAPIRequestError(f"Bad request when requesting {response.request.url}. {response.text}")
 
         return response
 
     @staticmethod
     def check_ping_response(response: Response) -> Response:
         """Checks a healthchecks.io ping response.
 
@@ -204,29 +200,23 @@
         if response.status_code == 404 or "not found" in response.text:
             raise CheckNotFoundError(f"CHeck not found at {response.request.url}")
 
         if "rate limited" in response.text or response.status_code == 429:
             raise HCAPIRateLimitError(f"Rate limited on {response.request.url}")
 
         if response.status_code == 400:
-            raise BadAPIRequestError(
-                f"Bad request when requesting {response.request.url}. {response.text}"
-            )
+            raise BadAPIRequestError(f"Bad request when requesting {response.request.url}. {response.text}")
 
         if response.status_code == 409:
-            raise NonUniqueSlugError(
-                f"Bad request, slug conflict {response.request.url}. {response.text}"
-            )
+            raise NonUniqueSlugError(f"Bad request, slug conflict {response.request.url}. {response.text}")
 
         return response
 
     @staticmethod
-    def _add_url_params(
-        url: str, params: Dict[str, Union[str, int, bool]], replace: bool = True
-    ) -> str:
+    def _add_url_params(url: str, params: Dict[str, Union[str, int, bool]], replace: bool = True) -> str:
         """Add GET params to provided URL being aware of existing.
 
         :param url: string of target URL
         :param params: dict containing requested params to be added
         :param replace: bool True If true, replace params if they exist with new values, otherwise append
         :return: string with updated URL
 
@@ -251,20 +241,15 @@
             # Merging URL arguments dict with new params
             parsed_get_args.update(parsed_params)
             extra_parameters = ""
         else:
             # get all the duplicated keys from params and urlencode them, we'll concat this to the params string later
             duplicated_params = [x for x in params if x in parsed_get_args]
             # get all the args that aren't duplicated and add them to parsed_get_args
-            parsed_get_args.update(
-                {
-                    key: parsed_params[key]
-                    for key in [x for x in params if x not in parsed_get_args]
-                }
-            )
+            parsed_get_args.update({key: parsed_params[key] for key in [x for x in params if x not in parsed_get_args]})
             # if we have any duplicated parameters, urlencode them, we append them later
             extra_parameters = (
                 f"&{urlencode({key: params[key] for key in duplicated_params}, doseq=True)}"
                 if len(duplicated_params) > 0
                 else ""
             )
```

### Comparing `healthchecks_io-0.4.0/src/healthchecks_io/client/async_client.py` & `healthchecks_io-0.4.1/src/healthchecks_io/client/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """An async healthchecks.io client."""
+
 import asyncio
 from types import TracebackType
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
```

### Comparing `healthchecks_io-0.4.0/src/healthchecks_io/client/check_trap.py` & `healthchecks_io-0.4.1/src/healthchecks_io/client/check_trap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CheckTrap is a context manager to wrap around python code to communicate results to a Healthchecks check."""
+
 from types import TracebackType
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import Union
 
 from .async_client import AsyncClient
@@ -64,17 +65,15 @@
             HCAPIRateLimitError: Raised when status code is 429 or response text has "rate limited" in it
             NonUniqueSlugError: Raused when status code is 409.
 
         Returns:
             CheckTrap: self
         """
         if isinstance(self.client, AsyncClient):
-            raise WrongClientError(
-                "You passed an AsyncClient, use this as an async context manager"
-            )
+            raise WrongClientError("You passed an AsyncClient, use this as an async context manager")
         result = self.client.start_ping(uuid=self.uuid, slug=self.slug)
         if not result[0]:
             raise PingFailedError(result[1])
         return self
 
     def __exit__(
         self,
@@ -92,17 +91,15 @@
             exc (Optional[BaseException]): [description]
             traceback (Optional[TracebackType]): [description]
 
         Returns:
             Optional[bool]: self.suppress_exceptions, if true will not raise any exceptions
         """
         if exc_type is None:
-            self.client.success_ping(
-                self.uuid, self.slug, data="\n".join(self.log_lines)
-            )
+            self.client.success_ping(self.uuid, self.slug, data="\n".join(self.log_lines))
         else:
             self.add_log(str(exc))
             self.add_log(str(traceback))
             self.client.fail_ping(self.uuid, self.slug, data="\n".join(self.log_lines))
         return self.suppress_exceptions
 
     async def __aenter__(self) -> "CheckTrap":
@@ -121,17 +118,15 @@
             HCAPIRateLimitError: Raised when status code is 429 or response text has "rate limited" in it
             NonUniqueSlugError: Raused when status code is 409.
 
         Returns:
             CheckTrap: self
         """
         if isinstance(self.client, Client):
-            raise WrongClientError(
-                "You passed a sync Client, use this as a regular context manager"
-            )
+            raise WrongClientError("You passed a sync Client, use this as a regular context manager")
         result = await self.client.start_ping(self.uuid, self.slug)
         if not result[0]:
             raise PingFailedError(result[1])
         return self
 
     async def __aexit__(
         self,
```

### Comparing `healthchecks_io-0.4.0/src/healthchecks_io/client/exceptions.py` & `healthchecks_io-0.4.1/src/healthchecks_io/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `healthchecks_io-0.4.0/src/healthchecks_io/client/sync_client.py` & `healthchecks_io-0.4.1/src/healthchecks_io/client/sync_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """An async healthchecks.io client."""
+
 from types import TracebackType
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
```

### Comparing `healthchecks_io-0.4.0/src/healthchecks_io/schemas/badges.py` & `healthchecks_io-0.4.1/src/healthchecks_io/schemas/badges.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Schemas for badges.
 
 https://healthchecks.io/docs/api/
 """
+
 from typing import Dict
 
 from pydantic import BaseModel
 
 
 class Badges(BaseModel):
     """Object with the Badges urls."""
```

### Comparing `healthchecks_io-0.4.0/src/healthchecks_io/schemas/checks.py` & `healthchecks_io-0.4.1/src/healthchecks_io/schemas/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Schemas for checks.
 
 https://healthchecks.io/docs/api/
 """
+
 from datetime import datetime
 from pathlib import PurePath
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
@@ -84,16 +85,15 @@
         description="A cron expression defining this check's schedule. "
         "If you specify both timeout and schedule parameters, "
         "Healthchecks.io will create a Cron check and ignore the "
         "timeout value.",
     )
     tz: Optional[str] = Field(
         "UTC",
-        description="Server's timezone. This setting only has an effect "
-        "in combination with the schedule parameter.",
+        description="Server's timezone. This setting only has an effect " "in combination with the schedule parameter.",
     )
     manual_resume: Optional[bool] = Field(
         False,
         description="Controls whether a paused check automatically resumes "
         "when pinged (the default) or not. If set to false, a paused "
         "check will leave the paused state when it receives a ping. "
         "If set to true, a paused check will ignore pings and stay "
@@ -180,16 +180,15 @@
         description="A cron expression defining this check's schedule. "
         "If you specify both timeout and schedule parameters, "
         "Healthchecks.io will create a Cron check and ignore the "
         "timeout value.",
     )
     tz: Optional[str] = Field(
         None,
-        description="Server's timezone. This setting only has an effect "
-        "in combination with the schedule parameter.",
+        description="Server's timezone. This setting only has an effect " "in combination with the schedule parameter.",
     )
     manual_resume: Optional[bool] = Field(
         None,
         description="Controls whether a paused check automatically resumes "
         "when pinged (the default) or not. If set to false, a paused "
         "check will leave the paused state when it receives a ping. "
         "If set to true, a paused check will ignore pings and stay "
```

### Comparing `healthchecks_io-0.4.0/setup.py` & `healthchecks_io-0.4.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,138 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: healthchecks_io
+Version: 0.4.1
+Summary: A python client package for Healthchecks.io API
+Home-page: https://github.com/andrewthetechie/py-healthchecks.io
+License: MIT
+Author: Andrew Herrington
+Author-email: andrew.the.techie@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.7
+Requires-Dist: croniter (>=1.1.0,<2.0.0)
+Requires-Dist: httpx (>=0.23.0,<0.25.0)
+Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Requires-Dist: pytz (>=2021.3,<2024.0)
+Project-URL: Changelog, https://github.com/andrewthetechie/py-healthchecks.io/releases
+Project-URL: Documentation, https://py-healthchecks.io.readthedocs.io
+Project-URL: Repository, https://github.com/andrewthetechie/py-healthchecks.io
+Description-Content-Type: text/x-rst
+
+Py Healthchecks.Io
+==================
+
+|PyPI| |Status| |Python Version| |License|
+
+|Read the Docs| |Tests| |Codecov|
+
+|pre-commit| |Black|
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/healthchecks-io.svg
+   :target: https://pypi.org/project/healthchecks-io/
+   :alt: PyPI
+.. |Status| image:: https://img.shields.io/pypi/status/healthchecks-io.svg
+   :target: https://pypi.org/project/healthchecks-io/
+   :alt: Status
+.. |Python Version| image:: https://img.shields.io/pypi/pyversions/healthchecks-io
+   :target: https://pypi.org/project/healthchecks-io
+   :alt: Python Version
+.. |License| image:: https://img.shields.io/pypi/l/healthchecks-io
+   :target: https://opensource.org/licenses/MIT
+   :alt: License
+.. |Read the Docs| image:: https://img.shields.io/readthedocs/py-healthchecksio/latest.svg?label=Read%20the%20Docs
+   :target: https://py-healthchecksio.readthedocs.io/en/latest/
+   :alt: Read the documentation at https://py-healthchecksio.readthedocs.io/en/latest/
+.. |Tests| image:: https://github.com/andrewthetechie/py-healthchecks.io/workflows/Tests/badge.svg
+   :target: https://github.com/andrewthetechie/py-healthchecks.io/actions?workflow=Tests
+   :alt: Tests
+.. |Codecov| image:: https://codecov.io/gh/andrewthetechie/py-healthchecks.io/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/andrewthetechie/py-healthchecks.io
+   :alt: Codecov
+.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: Black
+
+A python client for healthchecks.io. Supports the management api and ping api.
+
+Features
+--------
+
+* Sync and Async clients based on HTTPX
+* Supports the management api and the ping api
+* Supports Healthchecks.io SAAS and self-hosted instances
+
+
+Requirements
+------------
+
+* httpx
+* pytz
+* pydantic
+
+
+Installation
+------------
+
+You can install *Py Healthchecks.Io* via pip_ from PyPI_:
+
+.. code:: console
+
+   $ pip install healthchecks-io
+
+
+Usage
+-----
+
+Please see the `Usage <Usage_>`_ for details.
+
+
+Contributing
+------------
+
+Contributions are very welcome.
+To learn more, see the `Contributor Guide`_.
+
+
+License
+-------
+
+Distributed under the terms of the `MIT license`_,
+*Py Healthchecks.Io* is free and open source software.
+
+
+Issues
+------
+
+If you encounter any problems,
+please `file an issue`_ along with a detailed description.
+
+
+Credits
+-------
+
+This project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.
+
+.. _@cjolowicz: https://github.com/cjolowicz
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _MIT license: https://opensource.org/licenses/MIT
+.. _PyPI: https://pypi.org/
+.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+.. _file an issue: https://github.com/andrewthetechie/py-healthchecks.io/issues
+.. _pip: https://pip.pypa.io/
+.. github-only
+.. _Contributor Guide: CONTRIBUTING.rst
+.. _Usage: https://py-healthchecksio.readthedocs.io/en/latest/usage.html
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['healthchecks_io', 'healthchecks_io.client', 'healthchecks_io.schemas']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['croniter>=1.1.0,<2.0.0',
- 'httpx>=0.23.0,<0.24.0',
- 'pydantic>=1.9.1,<2.0.0',
- 'pytz>=2021.3,<2023.0']
-
-setup_kwargs = {
-    'name': 'healthchecks-io',
-    'version': '0.4.0',
-    'description': 'A python client package for Healthchecks.io API',
-    'long_description': "Py Healthchecks.Io\n==================\n\n|PyPI| |Status| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/healthchecks-io.svg\n   :target: https://pypi.org/project/healthchecks-io/\n   :alt: PyPI\n.. |Status| image:: https://img.shields.io/pypi/status/healthchecks-io.svg\n   :target: https://pypi.org/project/healthchecks-io/\n   :alt: Status\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/healthchecks-io\n   :target: https://pypi.org/project/healthchecks-io\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/healthchecks-io\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/py-healthchecksio/latest.svg?label=Read%20the%20Docs\n   :target: https://py-healthchecksio.readthedocs.io/en/latest/\n   :alt: Read the documentation at https://py-healthchecksio.readthedocs.io/en/latest/\n.. |Tests| image:: https://github.com/andrewthetechie/py-healthchecks.io/workflows/Tests/badge.svg\n   :target: https://github.com/andrewthetechie/py-healthchecks.io/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/andrewthetechie/py-healthchecks.io/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/andrewthetechie/py-healthchecks.io\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\nA python client for healthchecks.io. Supports the management api and ping api.\n\nFeatures\n--------\n\n* Sync and Async clients based on HTTPX\n* Supports the management api and the ping api\n* Supports Healthchecks.io SAAS and self-hosted instances\n\n\nRequirements\n------------\n\n* httpx\n* pytz\n* pydantic\n\n\nInstallation\n------------\n\nYou can install *Py Healthchecks.Io* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install healthchecks-io\n\n\nUsage\n-----\n\nPlease see the `Usage <Usage_>`_ for details.\n\n\nContributing\n------------\n\nContributions are very welcome.\nTo learn more, see the `Contributor Guide`_.\n\n\nLicense\n-------\n\nDistributed under the terms of the `MIT license`_,\n*Py Healthchecks.Io* is free and open source software.\n\n\nIssues\n------\n\nIf you encounter any problems,\nplease `file an issue`_ along with a detailed description.\n\n\nCredits\n-------\n\nThis project was generated from `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_ template.\n\n.. _@cjolowicz: https://github.com/cjolowicz\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _MIT license: https://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _file an issue: https://github.com/andrewthetechie/py-healthchecks.io/issues\n.. _pip: https://pip.pypa.io/\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Usage: https://py-healthchecksio.readthedocs.io/en/latest/usage.html\n",
-    'author': 'Andrew Herrington',
-    'author_email': 'andrew.the.techie@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/andrewthetechie/py-healthchecks.io',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

