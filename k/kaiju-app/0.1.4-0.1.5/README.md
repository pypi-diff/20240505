# Comparing `tmp/kaiju_app-0.1.4-py3-none-any.whl.zip` & `tmp/kaiju_app-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,14 @@
-Zip file size: 18876 bytes, number of entries: 13
--rw-r--r--  2.0 unx      314 b- defN 24-May-02 15:12 kaiju_app/__init__.py
--rw-r--r--  2.0 unx    16909 b- defN 24-May-02 15:12 kaiju_app/app.py
--rw-r--r--  2.0 unx     1473 b- defN 24-May-02 15:12 kaiju_app/bases.py
--rw-r--r--  2.0 unx     4545 b- defN 24-May-02 15:12 kaiju_app/configurator.py
--rw-r--r--  2.0 unx      314 b- defN 24-May-02 15:12 kaiju_app/interfaces.py
--rw-r--r--  2.0 unx    10494 b- defN 24-May-02 15:12 kaiju_app/loader.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 15:12 kaiju_app/py.typed
--rw-r--r--  2.0 unx    14232 b- defN 24-May-02 15:12 kaiju_app/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 24-May-02 15:12 kaiju_app-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     5156 b- defN 24-May-02 15:12 kaiju_app-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 15:12 kaiju_app-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-02 15:12 kaiju_app-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1008 b- defN 24-May-02 15:12 kaiju_app-0.1.4.dist-info/RECORD
-13 files, 55616 bytes uncompressed, 17212 bytes compressed:  69.1%
+Zip file size: 18659 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      314 b- defN 24-May-05 17:16 kaiju_app/__init__.py
+-rw-r--r--  2.0 unx    16909 b- defN 24-May-05 17:16 kaiju_app/app.py
+-rw-r--r--  2.0 unx     1909 b- defN 24-May-05 17:16 kaiju_app/bases.py
+-rw-r--r--  2.0 unx     4546 b- defN 24-May-05 17:16 kaiju_app/configurator.py
+-rw-r--r--  2.0 unx    10494 b- defN 24-May-05 17:16 kaiju_app/loader.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-05 17:16 kaiju_app/py.typed
+-rw-r--r--  2.0 unx    14232 b- defN 24-May-05 17:16 kaiju_app/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-05 17:16 kaiju_app-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5207 b- defN 24-May-05 17:16 kaiju_app-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-05 17:16 kaiju_app-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-05 17:16 kaiju_app-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      929 b- defN 24-May-05 17:16 kaiju_app-0.1.5.dist-info/RECORD
+12 files, 55711 bytes uncompressed, 17117 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -6,35 +6,32 @@
 
 Filename: kaiju_app/bases.py
 Comment: 
 
 Filename: kaiju_app/configurator.py
 Comment: 
 
-Filename: kaiju_app/interfaces.py
-Comment: 
-
 Filename: kaiju_app/loader.py
 Comment: 
 
 Filename: kaiju_app/py.typed
 Comment: 
 
 Filename: kaiju_app/utils.py
 Comment: 
 
-Filename: kaiju_app-0.1.4.dist-info/LICENSE
+Filename: kaiju_app-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_app-0.1.4.dist-info/METADATA
+Filename: kaiju_app-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_app-0.1.4.dist-info/WHEEL
+Filename: kaiju_app-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_app-0.1.4.dist-info/top_level.txt
+Filename: kaiju_app-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_app-0.1.4.dist-info/RECORD
+Filename: kaiju_app-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_app/__init__.py

```diff
@@ -1,11 +1,11 @@
 """Application and service base classes for server asyncio applications."""
 
 from kaiju_app.app import *
 from kaiju_app.bases import *
 from kaiju_app.configurator import *
 from kaiju_app.loader import *
 
-__python_version__ = "3.12"
+__python_version__ = "3.11"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

## kaiju_app/app.py

```diff
@@ -5,19 +5,19 @@
 from contextlib import suppress
 from contextvars import ContextVar
 from dataclasses import MISSING, Field, dataclass, field
 from enum import Enum
 from types import MappingProxyType
 from typing import Any, Awaitable, Callable, Self, TypedDict, TypeVar, final
 
-from kaiju_scheduler import Scheduler, ScheduledTask, Server
+from kaiju_scheduler import ScheduledTask, Scheduler, Server
 from uvlog import Logger
 
 from kaiju_app.bases import Error
-from kaiju_app.utils import State, timeout, Namespace
+from kaiju_app.utils import Namespace, State, timeout
 
 __all__ = [
     "APP_CONTEXT",
     "Application",
     "service",
     "Service",
     "ServiceState",
```

## kaiju_app/bases.py

```diff
@@ -1,13 +1,35 @@
 """Base and basic types."""
 
-from abc import ABC
-from typing import ClassVar, Mapping, TypedDict, Any
+from abc import ABC, abstractmethod
+from typing import Any, ClassVar, Mapping, Protocol, TypedDict
 
-__all__ = ["Error", "ErrorData"]
+__all__ = ["Error", "ErrorData", "JSONType", "Encoder", "Contextable"]
+
+
+class Contextable(Protocol):
+
+    async def start(self) -> None: ...
+
+    async def stop(self) -> None: ...
+
+
+class JSONType(Protocol):
+
+    @abstractmethod
+    def json_repr(self) -> dict[str, Any]: ...
+
+
+class Encoder(Protocol):
+
+    @abstractmethod
+    def encode(self, obj: Any, /) -> bytes: ...
+
+    @abstractmethod
+    def decode(self, data: bytes, /) -> Any: ...
 
 
 class _ErrorDataData(TypedDict):
     type: str
     type_base: str
     extra: Mapping[str, Any]
```

## kaiju_app/configurator.py

```diff
@@ -56,15 +56,15 @@
         3. Load OS environment variables
         4. Load CLI environment variables from '--env' flags
         5. Evaluate template using resulting env dict
         6. Normalize and return the project config dict
 
         See :py:func:`~kaiju_app.utils.merge_dicts` function on the rules of how dictionaries are merged.
 
-        See the `template-dict documentation <http://template-dict.readthedocs.io>`_ on template syntax.
+        See the `template-dict documentation <https://template-dict.readthedocs.io>`_ on template syntax.
 
         """
         template = Template(merge_dicts(*templates))
         envs = [*envs]
         if load_os_env:
             envs.append(self.get_os_env(template))
         if load_cli_env:
```

## kaiju_app/utils.py

```diff
@@ -2,15 +2,15 @@
 
 import asyncio
 from abc import ABC
 from ast import literal_eval
 from bisect import bisect
 from collections.abc import Hashable, Sized
 from contextlib import suppress
-from typing import Any, Collection, Generic, Iterable, Mapping, TypeVar, NewType
+from typing import Any, Collection, Generic, Iterable, Mapping, NewType, TypeVar
 
 from kaiju_scheduler import RetryError, retry, timeout
 from template_dict import Template
 
 __all__ = [
     "timeout",
     "eval_string",
```

## Comparing `kaiju_app-0.1.4.dist-info/LICENSE` & `kaiju_app-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_app-0.1.4.dist-info/METADATA` & `kaiju_app-0.1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: kaiju-app
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python modular application and services
 Home-page: https://github.com/violet-black/kaiju-app
 Author: violetblackdev@gmail.com
 License: MIT
 Keywords: application,microservice,asyncio,infrastructure
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.12
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: template-dict
 Requires-Dist: uvlog
 Requires-Dist: kaiju-scheduler
 Provides-Extra: dev
 Requires-Dist: pip-tools ; extra == 'dev'
```

## Comparing `kaiju_app-0.1.4.dist-info/RECORD` & `kaiju_app-0.1.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-kaiju_app/__init__.py,sha256=rhZoLvFPQf3_TyVqS_MTrKyJiHcn5hfioF7BDeoWjOM,314
-kaiju_app/app.py,sha256=cu86bZifQgi8OjaeTgLYKzBI5DH41youQPKDhLjt7sk,16909
-kaiju_app/bases.py,sha256=5I-Icjqe-2MaNV9GseDE0hOHlJPW4tCZkSTLcR0e26k,1473
-kaiju_app/configurator.py,sha256=4S56zroYvZrk2CP2_aAnt_2b63mdOG2JXLTX1tRe3wI,4545
-kaiju_app/interfaces.py,sha256=Rkz0pDMk_0AUC8MwOSTrq7cbhhCiXQISdpb5CJKIPGw,314
+kaiju_app/__init__.py,sha256=_WOgxIp_mnJTW1BsQEJ7eaGWZriA49Rj-8tc65RxoME,314
+kaiju_app/app.py,sha256=Gcnbgrpm2dE5uPjdQeF04OYdxRx-Uy2unERgybXBilw,16909
+kaiju_app/bases.py,sha256=zDJFeBtZIUFaC6cEBJXLe7lsukK8vlr9HupDfOWsdyk,1909
+kaiju_app/configurator.py,sha256=J8UlUCghdGi7gvKGHa74htTPfrrngZwUpaHzcNT3t84,4546
 kaiju_app/loader.py,sha256=n7e7piO86Ym4rp_-wpeu7dfz5lOevF_vPeHnQP82-EQ,10494
 kaiju_app/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kaiju_app/utils.py,sha256=kkU_ENfQj2OfPgde193iYK3tOJkfeX-aGmt-sm5Q0TA,14232
-kaiju_app-0.1.4.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
-kaiju_app-0.1.4.dist-info/METADATA,sha256=cJ4ci2voiHq34NG_SDWtpPmjg1b62H6yC6CgBtIaIPw,5156
-kaiju_app-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-kaiju_app-0.1.4.dist-info/top_level.txt,sha256=oaPejx2Wf_jdrr583PfUJWkCx3c4XqOCJGPVrNTQVbg,10
-kaiju_app-0.1.4.dist-info/RECORD,,
+kaiju_app/utils.py,sha256=zkaEx_wQIQ_YO8FtxDDQQz43z4Wmds3OJcEcOtHzdQo,14232
+kaiju_app-0.1.5.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
+kaiju_app-0.1.5.dist-info/METADATA,sha256=6LZNuczPH0bKUhWbIxF-b5OvHvrIVRo3ckC4BnsH-J0,5207
+kaiju_app-0.1.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+kaiju_app-0.1.5.dist-info/top_level.txt,sha256=oaPejx2Wf_jdrr583PfUJWkCx3c4XqOCJGPVrNTQVbg,10
+kaiju_app-0.1.5.dist-info/RECORD,,
```

