# Comparing `tmp/glue_utils-0.2.2b0.tar.gz` & `tmp/glue_utils-0.2.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.2.2b0.tar", max compression
+gzip compressed data, was "glue_utils-0.2.2b1.tar", max compression
```

## Comparing `glue_utils-0.2.2b0.tar` & `glue_utils-0.2.2b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.2b0/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.2b0/README.md
--rw-r--r--   0        0        0     3298 2024-05-04 14:01:12.346140 glue_utils-0.2.2b0/pyproject.toml
--rw-r--r--   0        0        0       98 2024-05-04 14:01:24.443348 glue_utils-0.2.2b0/src/glue_utils/__init__.py
--rw-r--r--   0        0        0       68 2024-05-03 09:05:30.885798 glue_utils-0.2.2b0/src/glue_utils/glueetl/__init__.py
--rw-r--r--   0        0        0     3126 2024-05-04 13:59:47.431646 glue_utils-0.2.2b0/src/glue_utils/glueetl/job.py
--rw-r--r--   0        0        0      830 2024-05-04 13:59:47.431943 glue_utils-0.2.2b0/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.2.2b0/src/glue_utils/py.typed
--rw-r--r--   0        0        0     2252 1970-01-01 00:00:00.000000 glue_utils-0.2.2b0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.2b1/LICENSE
+-rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.2b1/README.md
+-rw-r--r--   0        0        0     3280 2024-05-05 03:01:24.046072 glue_utils-0.2.2b1/pyproject.toml
+-rw-r--r--   0        0        0       98 2024-05-05 03:01:28.151666 glue_utils-0.2.2b1/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-03 09:05:30.885798 glue_utils-0.2.2b1/src/glue_utils/glueetl/__init__.py
+-rw-r--r--   0        0        0     2089 2024-05-05 02:57:51.451892 glue_utils-0.2.2b1/src/glue_utils/glueetl/job.py
+-rw-r--r--   0        0        0     1225 2024-05-05 02:26:30.596508 glue_utils-0.2.2b1/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.2.2b1/src/glue_utils/py.typed
+-rw-r--r--   0        0        0     2252 1970-01-01 00:00:00.000000 glue_utils-0.2.2b1/PKG-INFO
```

### Comparing `glue_utils-0.2.2b0/LICENSE` & `glue_utils-0.2.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.2b0/README.md` & `glue_utils-0.2.2b1/README.md`

 * *Files identical despite different names*

### Comparing `glue_utils-0.2.2b0/pyproject.toml` & `glue_utils-0.2.2b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.2.2b0"
+version = "0.2.2b1"
 # Uncomment this when dependabot has finally been updated to it is 
 # supported by dependabot.
 # package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
@@ -32,15 +32,14 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest-randomly = "^3.15.0"
 pytest-cov = "^5.0.0"
 mypy = "^1.10.0"
-pytest = "^8.2.0"
 ruff = "^0.4.3"
 
 [tool.poetry.group.local.dependencies]
 # The "local" dependency group refers to dependencies that already 
 # exist in AWS Glue's runtime. We don't need to install these in the
 # container. We only need them for local (non-container) development to 
 # aid the IDE in providing code completion and type checking.
```

### Comparing `glue_utils-0.2.2b0/src/glue_utils/glueetl/job.py` & `glue_utils-0.2.2b1/src/glue_utils/glueetl/job.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """Module providing the GlueETLJob class for handling Glue ETL jobs."""
 
 from __future__ import annotations
 
-import sys
 from contextlib import contextmanager
-from dataclasses import fields
-from typing import TYPE_CHECKING, Generic, cast, overload
+from typing import TYPE_CHECKING, Generic, cast
 
 from awsglue.context import GlueContext
 from awsglue.job import Job
-from awsglue.utils import getResolvedOptions
-from pyspark import SparkConf, SparkContext
+from pyspark import SparkContext
 from typing_extensions import TypeVar
 
 from glue_utils import BaseOptions
 
 if TYPE_CHECKING:
     from collections.abc import Generator
 
@@ -22,82 +19,45 @@
 
 T = TypeVar("T", bound=BaseOptions, default=BaseOptions)
 
 
 class GlueETLJob(Generic[T]):
     """Class that handles the boilerplate setup for Glue ETL jobs."""
 
-    name: str
     options: T
     sc: SparkContext
     spark: SparkSession
     glue_context: GlueContext
 
-    @overload
-    def __init__(
-        self: GlueETLJob[BaseOptions],
-    ) -> None: ...
-
-    @overload
-    def __init__(
-        self: GlueETLJob[T],
-        *,
-        options_cls: type[T],
-    ) -> None: ...
-
     def __init__(
         self,
-        *,
         options_cls: type[T | BaseOptions] = BaseOptions,
     ) -> None:
         """Initialize the GlueETLJob.
 
         Parameters
         ----------
         options_cls, optional
             Has to be a subclass of BaseOptions, by default BaseOptions
 
         """
         if not issubclass(options_cls, BaseOptions):
             msg = "options_cls must be a subclass of BaseOptions."
             raise TypeError(msg)
 
-        params = []
-        if "--JOB_NAME" in sys.argv:
-            params.append("JOB_NAME")
-        params.extend(field.name for field in fields(options_cls))
-
-        job_options = getResolvedOptions(sys.argv, params)
-
-        self.options = cast(T, options_cls.from_resolved_options(job_options))
+        self.options = cast(T, options_cls.from_resolved_options())
 
-        self.name = job_options.get("JOB_NAME", "glueetl-job")
+        job_name = self.options.job_arguments.get("JOB_NAME", "glueetl-job")
 
-        self.sc = self.create_spark_context()
-        self.glue_context = self.create_glue_context()
+        self.sc = SparkContext.getOrCreate()
+        self.glue_context = GlueContext(self.sc)
         self.spark = self.glue_context.spark_session
 
         self._job = Job(self.glue_context)
-        self._job.init(self.name, job_options)
-
-    def create_spark_context(self) -> SparkContext:
-        """Create a SparkContext.
-
-        Override this method to customize the SparkContext creation.
-        """
-        spark_conf = SparkConf().setAppName(self.name)
-
-        return SparkContext.getOrCreate(spark_conf)
-
-    def create_glue_context(self) -> GlueContext:
-        """Create a GlueContext.
-
-        Override this method to customize the GlueContext creation.
-        """
-        return GlueContext(self.sc)
+        self._job.init(job_name, self.options.job_arguments)
 
     @contextmanager
     def managed_glue_context(
         self,
         *,
         commit: bool = True,
     ) -> Generator[GlueContext, None, None]:
```

### Comparing `glue_utils-0.2.2b0/PKG-INFO` & `glue_utils-0.2.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.2.2b0
+Version: 0.2.2b1
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
 Requires-Python: >=3.9,<4.0
```

