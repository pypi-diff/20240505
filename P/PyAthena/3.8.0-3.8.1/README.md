# Comparing `tmp/pyathena-3.8.0.tar.gz` & `tmp/pyathena-3.8.1.tar.gz`

## Comparing `pyathena-3.8.0.tar` & `pyathena-3.8.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/__init__.py
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/async_cursor.py
--rw-r--r--   0        0        0    23825 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/common.py
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/connection.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/converter.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/cursor.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/error.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/formatter.py
--rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/py.typed
--rw-r--r--   0        0        0    23041 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/result_set.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/arrow/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/fastparquet/__init__.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/fastparquet/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/filesystem/__init__.py
--rw-r--r--   0        0        0    33151 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/filesystem/s3.py
--rw-r--r--   0        0        0    14350 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/filesystem/s3_object.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    13467 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0    10297 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/pandas/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/spark/__init__.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/spark/async_cursor.py
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/spark/common.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/spark/cursor.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/arrow.py
--rw-r--r--   0        0        0    42007 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/base.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/pandas.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/rest.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/types.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyathena/sqlalchemy/util.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pyathena-3.8.0/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pyathena-3.8.0/LICENSE
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pyathena-3.8.0/README.rst
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pyathena-3.8.0/pyproject.toml
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 pyathena-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/__init__.py
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    23825 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/common.py
+-rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/connection.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/converter.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/cursor.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/error.py
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/formatter.py
+-rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/py.typed
+-rw-r--r--   0        0        0    23041 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/result_set.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/arrow/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    34952 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0    14350 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13467 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0    10297 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/pandas/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/spark/__init__.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/spark/async_cursor.py
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/spark/common.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/spark/cursor.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    42007 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pyathena-3.8.1/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pyathena-3.8.1/LICENSE
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pyathena-3.8.1/README.rst
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pyathena-3.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 pyathena-3.8.1/PKG-INFO
```

### Comparing `pyathena-3.8.0/pyathena/__init__.py` & `pyathena-3.8.1/pyathena/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection, ConnectionCursor
     from pyathena.cursor import Cursor
 
-__version__ = "3.8.0"
+__version__ = "3.8.1"
 user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 2
 paramstyle: str = "pyformat"
```

### Comparing `pyathena-3.8.0/pyathena/async_cursor.py` & `pyathena-3.8.1/pyathena/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/common.py` & `pyathena-3.8.1/pyathena/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/connection.py` & `pyathena-3.8.1/pyathena/connection.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/converter.py` & `pyathena-3.8.1/pyathena/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/cursor.py` & `pyathena-3.8.1/pyathena/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/error.py` & `pyathena-3.8.1/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/formatter.py` & `pyathena-3.8.1/pyathena/formatter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/model.py` & `pyathena-3.8.1/pyathena/model.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/result_set.py` & `pyathena-3.8.1/pyathena/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/util.py` & `pyathena-3.8.1/pyathena/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/arrow/async_cursor.py` & `pyathena-3.8.1/pyathena/arrow/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/arrow/converter.py` & `pyathena-3.8.1/pyathena/arrow/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/arrow/cursor.py` & `pyathena-3.8.1/pyathena/arrow/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/arrow/result_set.py` & `pyathena-3.8.1/pyathena/arrow/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/arrow/util.py` & `pyathena-3.8.1/pyathena/arrow/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/fastparquet/util.py` & `pyathena-3.8.1/pyathena/fastparquet/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/filesystem/s3.py` & `pyathena-3.8.1/pyathena/filesystem/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,19 @@
     from pyathena.connection import Connection
 
 _logger = logging.getLogger(__name__)  # type: ignore
 
 
 class S3FileSystem(AbstractFileSystem):
     # https://docs.aws.amazon.com/AmazonS3/latest/userguide/qfacts.html
-    # The minimum size of a part in a multipart upload is 5MB.
-    MULTIPART_UPLOAD_MINIMUM_SIZE: int = 5 * 2**20  # 5MB
+    # The minimum size of a part in a multipart upload is 5MiB.
+    MULTIPART_UPLOAD_MINIMUM_PART_SIZE: int = 5 * 2**20  # 5MiB
+    # https://docs.aws.amazon.com/AmazonS3/latest/userguide/qfacts.html
+    # The maximum size of a part in a multipart upload is 5GiB.
+    MULTIPART_UPLOAD_MAXIMUM_PART_SIZE: int = 5 * 2**30  # 5GiB
     DEFAULT_BLOCK_SIZE: int = 5 * 2**20  # 5MB
     PATTERN_PATH: Pattern[str] = re.compile(
         r"(^s3://|^s3a://|^)(?P<bucket>[a-zA-Z0-9.\-_]+)(/(?P<key>[^?]+)|/)?"
         r"($|\?version(Id|ID|id|_id)=(?P<version_id>.+)$)"
     )
 
     protocol = ["s3", "s3a"]
@@ -558,21 +561,21 @@
             **kwargs,
         )
 
     def _get_object(
         self,
         bucket: str,
         key: str,
-        ranges: Optional[Tuple[int, int]],
+        ranges: Optional[Tuple[int, int]] = None,
         version_id: Optional[str] = None,
         **kwargs,
     ) -> Tuple[int, bytes]:
         request = {"Bucket": bucket, "Key": key}
         if ranges:
-            range_ = f"bytes={ranges[0]}-{ranges[1] - 1}"
+            range_ = S3File._format_ranges(ranges)
             request.update({"Range": range_})
         else:
             ranges = (0, 0)
             range_ = "bytes=0-"
         if version_id:
             request.update({"VersionId": version_id})
 
@@ -614,24 +617,27 @@
     def _upload_part_copy(
         self,
         bucket: str,
         key: str,
         copy_source: str,
         upload_id: str,
         part_number: int,
+        copy_source_ranges: Optional[Tuple[int, int]] = None,
         **kwargs,
     ) -> S3MultipartUploadPart:
         request = {
             "Bucket": bucket,
             "Key": key,
             "CopySource": copy_source,
             "UploadId": upload_id,
             "PartNumber": part_number,
         }
-
+        if copy_source_ranges:
+            range_ = S3File._format_ranges(copy_source_ranges)
+            request.update({"CopySourceRange": range_})
         _logger.debug(
             f"Upload part copy from {copy_source} to s3://{bucket}/{key} as part {part_number}."
         )
         response = self._call(
             self._client.upload_part_copy,
             **request,
             **kwargs,
@@ -733,30 +739,32 @@
                     f"the version_id: {path_version_id} specified in the path do not match."
                 )
             self.version_id: Optional[str] = version_id
         elif path_version_id:
             self.version_id = path_version_id
         else:
             self.version_id = version_id
-        if "r" not in mode and block_size < self.fs.MULTIPART_UPLOAD_MINIMUM_SIZE:
+        if "r" not in mode and block_size < self.fs.MULTIPART_UPLOAD_MINIMUM_PART_SIZE:
             # When writing occurs, the block size should not be smaller
             # than the minimum size of a part in a multipart upload.
-            raise ValueError(f"Block size must be >= {self.fs.MULTIPART_UPLOAD_MINIMUM_SIZE}MB.")
+            raise ValueError(
+                f"Block size must be >= {self.fs.MULTIPART_UPLOAD_MINIMUM_PART_SIZE}MB."
+            )
 
         self.append_block = False
         if "r" in mode:
             info = self.fs.info(self.path, version_id=self.version_id)
             if etag := info.get("etag"):
                 self.s3_additional_kwargs.update({"IfMatch": etag})
             self._details = info
         elif "a" in mode and self.fs.exists(path):
             self.append_block = True
             info = self.fs.info(self.path, version_id=self.version_id)
             loc = info.get("size", 0)
-            if loc < self.fs.MULTIPART_UPLOAD_MINIMUM_SIZE:
+            if loc < self.fs.MULTIPART_UPLOAD_MINIMUM_PART_SIZE:
                 self.write(self.fs.cat(self.path))
             self.loc = loc
             self.s3_additional_kwargs.update(info.to_api_repr())
             self._details = info
         else:
             self._details = {}
 
@@ -774,24 +782,50 @@
 
         self.multipart_upload = self.fs._create_multipart_upload(
             bucket=self.bucket,
             key=self.key,
             **self.s3_additional_kwargs,
         )
         if self.append_block:
-            self.multipart_upload_parts.append(
-                self._executor.submit(
-                    self.fs._upload_part_copy,
-                    bucket=self.bucket,
-                    key=self.key,
-                    copy_source=self.path,
-                    upload_id=cast(str, cast(S3MultipartUpload, self.multipart_upload).upload_id),
-                    part_number=1,
+            if self.tell() > S3FileSystem.MULTIPART_UPLOAD_MAXIMUM_PART_SIZE:
+                info = self.fs.info(self.path, version_id=self.version_id)
+                ranges = self._get_ranges(
+                    0,
+                    # Set copy source file byte size
+                    info.get("size", 0),
+                    self.max_workers,
+                    S3FileSystem.MULTIPART_UPLOAD_MAXIMUM_PART_SIZE,
+                )
+                for i, range in enumerate(ranges):
+                    self.multipart_upload_parts.append(
+                        self._executor.submit(
+                            self.fs._upload_part_copy,
+                            bucket=self.bucket,
+                            key=self.key,
+                            copy_source=self.path,
+                            upload_id=cast(
+                                str, cast(S3MultipartUpload, self.multipart_upload).upload_id
+                            ),
+                            part_number=i + 1,
+                            copy_source_ranges=range,
+                        )
+                    )
+            else:
+                self.multipart_upload_parts.append(
+                    self._executor.submit(
+                        self.fs._upload_part_copy,
+                        bucket=self.bucket,
+                        key=self.key,
+                        copy_source=self.path,
+                        upload_id=cast(
+                            str, cast(S3MultipartUpload, self.multipart_upload).upload_id
+                        ),
+                        part_number=1,
+                    )
                 )
-            )
 
     def _upload_chunk(self, final: bool = False) -> bool:
         if self.tell() < self.blocksize:
             # Files smaller than block size in size cannot be multipart uploaded.
             if self.autocommit and final:
                 self.commit()
             return True
@@ -903,14 +937,18 @@
                 ranges[0],
                 self.version_id,
                 **self.s3_additional_kwargs,
             )[1]
         return object_
 
     @staticmethod
+    def _format_ranges(ranges: Tuple[int, int]):
+        return f"bytes={ranges[0]}-{ranges[1] - 1}"
+
+    @staticmethod
     def _get_ranges(
         start: int, end: int, max_workers: int, worker_block_size: int
     ) -> List[Tuple[int, int]]:
         ranges = []
         range_size = end - start
         if max_workers > 1 and range_size > worker_block_size:
             range_start = start
```

### Comparing `pyathena-3.8.0/pyathena/filesystem/s3_object.py` & `pyathena-3.8.1/pyathena/filesystem/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/pandas/async_cursor.py` & `pyathena-3.8.1/pyathena/pandas/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/pandas/converter.py` & `pyathena-3.8.1/pyathena/pandas/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/pandas/cursor.py` & `pyathena-3.8.1/pyathena/pandas/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/pandas/result_set.py` & `pyathena-3.8.1/pyathena/pandas/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/pandas/util.py` & `pyathena-3.8.1/pyathena/pandas/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/spark/async_cursor.py` & `pyathena-3.8.1/pyathena/spark/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/spark/common.py` & `pyathena-3.8.1/pyathena/spark/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/spark/cursor.py` & `pyathena-3.8.1/pyathena/spark/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/sqlalchemy/arrow.py` & `pyathena-3.8.1/pyathena/sqlalchemy/arrow.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/sqlalchemy/base.py` & `pyathena-3.8.1/pyathena/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/sqlalchemy/pandas.py` & `pyathena-3.8.1/pyathena/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/sqlalchemy/requirements.py` & `pyathena-3.8.1/pyathena/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyathena/sqlalchemy/types.py` & `pyathena-3.8.1/pyathena/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/LICENSE` & `pyathena-3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/README.rst` & `pyathena-3.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/pyproject.toml` & `pyathena-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.0/PKG-INFO` & `pyathena-3.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: PyAthena
-Version: 3.8.0
+Version: 3.8.1
 Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
 Project-URL: homepage, https://github.com/laughingman7743/PyAthena/
 Project-URL: repository, https://github.com/laughingman7743/PyAthena/
 Author-email: laughingman7743 <laughingman7743@gmail.com>
 License: Copyright 2017 laughingman7743
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

