# Comparing `tmp/glue_utils-0.2.2b1.tar.gz` & `tmp/glue_utils-0.2.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.2.2b1.tar", max compression
+gzip compressed data, was "glue_utils-0.2.2b2.tar", max compression
```

## Comparing `glue_utils-0.2.2b1.tar` & `glue_utils-0.2.2b2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.2b1/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.2b1/README.md
--rw-r--r--   0        0        0     3280 2024-05-05 03:01:24.046072 glue_utils-0.2.2b1/pyproject.toml
--rw-r--r--   0        0        0       98 2024-05-05 03:01:28.151666 glue_utils-0.2.2b1/src/glue_utils/__init__.py
--rw-r--r--   0        0        0       68 2024-05-03 09:05:30.885798 glue_utils-0.2.2b1/src/glue_utils/glueetl/__init__.py
--rw-r--r--   0        0        0     2089 2024-05-05 02:57:51.451892 glue_utils-0.2.2b1/src/glue_utils/glueetl/job.py
--rw-r--r--   0        0        0     1225 2024-05-05 02:26:30.596508 glue_utils-0.2.2b1/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.2.2b1/src/glue_utils/py.typed
--rw-r--r--   0        0        0     2252 1970-01-01 00:00:00.000000 glue_utils-0.2.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.2b2/LICENSE
+-rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.2b2/README.md
+-rw-r--r--   0        0        0     3280 2024-05-05 05:44:08.804148 glue_utils-0.2.2b2/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-05-05 05:44:14.583905 glue_utils-0.2.2b2/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-03 09:05:30.885798 glue_utils-0.2.2b2/src/glue_utils/glueetl/__init__.py
+-rw-r--r--   0        0        0     2579 2024-05-05 05:21:19.481253 glue_utils-0.2.2b2/src/glue_utils/glueetl/job.py
+-rw-r--r--   0        0        0     1050 2024-05-05 05:38:44.945899 glue_utils-0.2.2b2/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.2.2b2/src/glue_utils/py.typed
+-rw-r--r--   0        0        0     2252 1970-01-01 00:00:00.000000 glue_utils-0.2.2b2/PKG-INFO
```

### Comparing `glue_utils-0.2.2b1/LICENSE` & `glue_utils-0.2.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.2b1/README.md` & `glue_utils-0.2.2b2/README.md`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.2b1/pyproject.toml` & `glue_utils-0.2.2b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.2.2b1"
+version = "0.2.2b2"
 # Uncomment this when dependabot has finally been updated to it is 
 # supported by dependabot.
 # package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `glue_utils-0.2.2b1/src/glue_utils/glueetl/job.py` & `glue_utils-0.2.2b2/src/glue_utils/glueetl/job.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Module providing the GlueETLJob class for handling Glue ETL jobs."""
 
 from __future__ import annotations
 
+import sys
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Generic, cast
+from dataclasses import fields
+from typing import TYPE_CHECKING, Generic, cast, overload
 
 from awsglue.context import GlueContext
 from awsglue.job import Job
+from awsglue.utils import getResolvedOptions
 from pyspark import SparkContext
 from typing_extensions import TypeVar
 
 from glue_utils import BaseOptions
 
 if TYPE_CHECKING:
     from collections.abc import Generator
@@ -24,14 +27,26 @@
     """Class that handles the boilerplate setup for Glue ETL jobs."""
 
     options: T
     sc: SparkContext
     spark: SparkSession
     glue_context: GlueContext
 
+    @overload
+    def __init__(
+        self: GlueETLJob[BaseOptions],
+    ) -> None: ...
+
+    @overload
+    def __init__(
+        self: GlueETLJob[T],
+        *,
+        options_cls: type[T],
+    ) -> None: ...
+
     def __init__(
         self,
         options_cls: type[T | BaseOptions] = BaseOptions,
     ) -> None:
         """Initialize the GlueETLJob.
 
         Parameters
@@ -40,24 +55,31 @@
             Has to be a subclass of BaseOptions, by default BaseOptions
 
         """
         if not issubclass(options_cls, BaseOptions):
             msg = "options_cls must be a subclass of BaseOptions."
             raise TypeError(msg)
 
-        self.options = cast(T, options_cls.from_resolved_options())
+        field_names = {field.name for field in fields(options_cls)}
+
+        params = []
+        if "--JOB_NAME" in sys.argv:
+            params.append("JOB_NAME")
+        params.extend(field_names)
+
+        _options = getResolvedOptions(sys.argv, params)
 
-        job_name = self.options.job_arguments.get("JOB_NAME", "glueetl-job")
+        self.options = cast(T, options_cls.from_options(_options))
 
         self.sc = SparkContext.getOrCreate()
         self.glue_context = GlueContext(self.sc)
         self.spark = self.glue_context.spark_session
 
         self._job = Job(self.glue_context)
-        self._job.init(job_name, self.options.job_arguments)
+        self._job.init(_options.get("JOB_NAME", ""), _options)
 
     @contextmanager
     def managed_glue_context(
         self,
         *,
         commit: bool = True,
     ) -> Generator[GlueContext, None, None]:
```

### Comparing `glue_utils-0.2.2b1/src/glue_utils/options.py` & `glue_utils-0.2.2b2/src/glue_utils/options.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 """Module for conveniently parsing options resolved from command-line arguments."""
 
 from __future__ import annotations
 
 import sys
-from dataclasses import InitVar, dataclass, fields
+from dataclasses import dataclass, fields
 from typing import Any
 
 from awsglue.utils import getResolvedOptions
 from typing_extensions import Self
 
 
 @dataclass
 class BaseOptions:
     """Dataclass for storing resolved options."""
 
-    job_arguments: InitVar[dict[str, Any]]
-
     @classmethod
-    def from_resolved_options(cls) -> Self:
-        """Create an instance of the class from Glue's resolved options."""
-        params = []
-        if "--JOB_NAME" in sys.argv:
-            params.append("JOB_NAME")
+    def from_sys_argv(cls) -> Self:
+        """Create an instance of the class from Glue's resolved arguments."""
+        resolved_options = getResolvedOptions(
+            sys.argv, [field.name for field in fields(cls)]
+        )
 
-        field_names = {field.name for field in fields(cls)}
+        return cls.from_options(resolved_options)
 
-        params.extend(field_names)
+    @classmethod
+    def from_options(cls, options: dict[str, Any] | None = None) -> Self:
+        """Create an instance of the class from the provided options."""
+        if not options:
+            return cls()
 
-        resolved_options = getResolvedOptions(sys.argv, params)
+        field_names = {field.name for field in fields(cls)}
 
         return cls(
-            job_arguments=resolved_options,
-            **{
-                key: value
-                for key, value in resolved_options.items()
-                if key in field_names
-            },
+            **{key: value for key, value in options.items() if key in field_names},
         )
-
-    def __post_init__(self, job_arguments: dict[str, Any] | None) -> None:
-        """Ensure that the job_arguments attribute is set."""
-        self.job_arguments = job_arguments or {}
```

### Comparing `glue_utils-0.2.2b1/PKG-INFO` & `glue_utils-0.2.2b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.2.2b1
+Version: 0.2.2b2
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
 Requires-Python: >=3.9,<4.0
```

