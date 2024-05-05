# Comparing `tmp/archivefile-0.2.0.tar.gz` & `tmp/archivefile-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archivefile-0.2.0.tar", max compression
+gzip compressed data, was "archivefile-0.3.0.tar", max compression
```

## Comparing `archivefile-0.2.0.tar` & `archivefile-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3603 2024-04-27 20:01:20.311675 archivefile-0.2.0/README.md
--rw-r--r--   0        0        0     2146 2024-04-27 20:01:20.315675 archivefile-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      690 2024-04-27 20:01:20.315675 archivefile-0.2.0/src/archivefile/__init__.py
--rw-r--r--   0        0        0      244 2024-04-27 20:01:20.315675 archivefile-0.2.0/src/archivefile/_compat.py
--rw-r--r--   0        0        0    32102 2024-04-27 20:01:20.315675 archivefile-0.2.0/src/archivefile/_core.py
--rw-r--r--   0        0        0      950 2024-04-27 20:01:20.315675 archivefile-0.2.0/src/archivefile/_enums.py
--rw-r--r--   0        0        0      199 2024-04-27 20:01:20.315675 archivefile-0.2.0/src/archivefile/_exceptions.py
--rw-r--r--   0        0        0      878 2024-04-27 20:01:20.315675 archivefile-0.2.0/src/archivefile/_models.py
--rw-r--r--   0        0        0      333 2024-04-27 20:01:20.315675 archivefile-0.2.0/src/archivefile/_types.py
--rw-r--r--   0        0        0     2406 2024-04-27 20:01:20.315675 archivefile-0.2.0/src/archivefile/_utils.py
--rw-r--r--   0        0        0      526 2024-04-27 20:01:20.315675 archivefile-0.2.0/src/archivefile/_version.py
--rw-r--r--   0        0        0        0 2024-04-27 20:01:20.315675 archivefile-0.2.0/src/archivefile/py.typed
--rw-r--r--   0        0        0     5233 1970-01-01 00:00:00.000000 archivefile-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4912 2024-05-05 07:25:35.226997 archivefile-0.3.0/README.md
+-rw-r--r--   0        0        0     2309 2024-05-05 07:25:35.226997 archivefile-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      598 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_compat.py
+-rw-r--r--   0        0        0    36784 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_core.py
+-rw-r--r--   0        0        0      980 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_enums.py
+-rw-r--r--   0        0        0      201 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_exceptions.py
+-rw-r--r--   0        0        0     1404 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_models.py
+-rw-r--r--   0        0        0     1171 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_types.py
+-rw-r--r--   0        0        0     2775 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_utils.py
+-rw-r--r--   0        0        0      526 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_version.py
+-rw-r--r--   0        0        0        0 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/py.typed
+-rw-r--r--   0        0        0     6718 1970-01-01 00:00:00.000000 archivefile-0.3.0/PKG-INFO
```

### Comparing `archivefile-0.2.0/pyproject.toml` & `archivefile-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "archivefile"
-version = "0.2.0"
+version = "0.3.0"
 description = "Unified interface for tar, zip, sevenzip, and rar files"
 authors = ["Raventric <78981416+Ravencentric@users.noreply.github.com>"]
 readme = "README.md"
 license = "Unlicense"
-packages = [{include = "archivefile", from = "src"}]
-keywords = ["archive", "zipfile", "tarfile", "sevenzip", "rarfile", "python"]
+packages = [{ include = "archivefile", from = "src" }]
+keywords = ["archive", "archivefile", "zipfile", "tarfile", "sevenzip", "rarfile"]
 homepage = "https://ravencentric.github.io/archivefile"
 repository = "https://github.com/Ravencentric/archivefile"
 documentation = "https://ravencentric.github.io/archivefile"
 classifiers = [
     "License :: OSI Approved :: The Unlicense (Unlicense)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
@@ -21,36 +21,42 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 rarfile = ">=4.2"
 py7zr = ">=0.21.0"
 typing-extensions = ">=4.11.0"
-pydantic = ">=2.7.0"
+pydantic = ">=2.7.1"
 pycryptodomex = ">=3.20.0"
 pyppmd = ">=1.1.0"
 zipfile-deflate64 = "^0.2.0"
 pybcj = ">=1.0.2"
 multivolumefile = ">=0.2.3"
-bigtree = ">=0.17.2"
+rich = { version = ">=13.7.1", optional = true }
+bigtree = { version = ">=0.17.2", optional = true }
 brotli = { version = ">=1.1.0", markers = "platform_python_implementation == 'CPython'" }
-brotlicffi =  { version = ">=1.1.0.0", markers = "platform_python_implementation == 'PyPy'" }
+brotlicffi = { version = ">=1.1.0.0", markers = "platform_python_implementation == 'PyPy'" }
 importlib-metadata = { version = ">=7.1.0", python = "<3.10" }
-eval-type-backport = {version = ">=0.1.3", python = "<3.10"}
+eval-type-backport = { version = ">=0.2.0", python = "<3.10" }
+
+[tool.poetry.extras]
+bigtree = ["bigtree"]
+rich = ["rich"]
+all = ["bigtree", "rich"]
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^1.9.0"
-ruff = "^0.3.7"
-pytest = "^8.1.1"
-coverage = "^7.5.0"
+mypy = "^1.10.0"
+ruff = "^0.4.3"
+pytest = "^8.2.0"
+coverage = "^7.5.1"
 pre-commit = "^3.7.0"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs-material = "^9.5.18"
-mkdocstrings = {extras = ["python"], version = "^0.24.0"}
+mkdocs-material = "^9.5.21"
+mkdocstrings = { extras = ["python"], version = "^0.24.0" }
 mkdocs-autorefs = "^1.0.1"
 
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.lint]
 extend-select = ["I"]
@@ -61,16 +67,12 @@
 pretty = true
 
 [[tool.mypy.overrides]]
 module = ["rarfile"]
 ignore_missing_imports = true
 
 [tool.coverage.run]
-omit = [
-    "src/archivefile/_version.py",
-    "src/archivefile/_compat.py",
-    "tests/*"
-]
+omit = ["src/archivefile/_version.py", "src/archivefile/_compat.py", "tests/*"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `archivefile-0.2.0/src/archivefile/__init__.py` & `archivefile-0.3.0/src/archivefile/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from __future__ import annotations
 
 from archivefile._core import ArchiveFile
-from archivefile._enums import ZipCompression
+from archivefile._enums import CompressionType
 from archivefile._exceptions import ArchiveFileError, UnsupportedArchiveOperation
 from archivefile._models import ArchiveMember
-from archivefile._types import OpenArchiveMode, StrPath
 from archivefile._utils import is_archive
 from archivefile._version import Version, _get_version
 
 __version__ = _get_version()
 __version_tuple__ = Version(*map(int, __version__.split(".")))
 
 __all__ = [
     "ArchiveFile",
     "ArchiveFileError",
     "ArchiveMember",
     "UnsupportedArchiveOperation",
     "is_archive",
-    "StrPath",
-    "OpenArchiveMode",
-    "ZipCompression",
+    "CompressionType",
 ]
```

### Comparing `archivefile-0.2.0/src/archivefile/_core.py` & `archivefile-0.3.0/src/archivefile/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,56 +6,66 @@
 from pathlib import Path
 from tarfile import TarFile, is_tarfile
 from tempfile import TemporaryDirectory
 from types import TracebackType
 from typing import Any
 from zipfile import ZipFile, is_zipfile
 
-from bigtree.tree.construct import list_to_tree
 from py7zr import SevenZipFile, is_7zfile
 from pydantic import validate_call
 from rarfile import RarFile, RarInfo, is_rarfile
 from typing_extensions import Literal, Self
 
-from archivefile._enums import CommonExtensions, ZipCompression
+from archivefile._enums import CommonExtensions, CompressionType
 from archivefile._exceptions import UnsupportedArchiveOperation
 from archivefile._models import ArchiveMember
-from archivefile._types import OpenArchiveMode, StrPath
-from archivefile._utils import check_extension, filter_kwargs
+from archivefile._types import CompressionLevel, ErrorHandler, OpenArchiveMode, SortBy, StrPath, TableStyle, TreeStyle
+from archivefile._utils import check_extension, filter_kwargs, realpath
 
 
 class ArchiveFile:
-    """The ArchiveFile Class provides a unified interface to zip, tar, rar, and 7zip archives."""
-
     @validate_call
     def __init__(
         self,
         file: StrPath,
         mode: OpenArchiveMode = "r",
         *,
         password: str | None = None,
         **kwargs: Any,
     ) -> None:
         """
         Open an archive file.
 
         Parameters
         ----------
-        file: StrPath
-            Path to the archive file. This must be an existing file.
-        mode: OpenArchiveMode, optional
-            Specifies the mode for opening the archive file. Default is "r".
-        password: str, optional
-            Password for encrypted archive files. Default is None.
-        kwargs: Any
-            Keyword arugments to pass to the underlying ZipFile/TarFile/RarFile/SevenZipFile handler.
+        file : StrPath
+            Path to the archive file.
+        mode : OpenArchiveMode, optional
+            Specifies the mode for opening the archive file.
+        password : str, optional
+            Password for encrypted archive files.
+        kwargs : Any
+            Keyword arugments to pass to the underlying handler.
             Kwargs that are not relevent to the current handler will automatically
             be removed so you don't have to worry about accidentally passing ZipFile's kwargs to TarFile.
+
+        Returns
+        -------
+        None
+
+        References
+        ----------
+        ArchiveFile currently supports the following handlers:
+
+        - [`ZipFile`][zipfile.ZipFile]
+        - [`TarFile`][tarfile.TarFile.open]
+        - [`RarFile`][rarfile.RarFile]
+        - [`SevenZipFile`][py7zr.SevenZipFile]
         """
-        self._file = file.expanduser().resolve() if isinstance(file, Path) else Path(file).expanduser().resolve()
+        self._file = realpath(file)
         self._mode = mode
         self._password = password
         self._kwargs = kwargs
         self._initialize_handler()
 
     def _initialize_handler(self) -> None:
         archive = self._file
@@ -64,15 +74,15 @@
         tarfile_mode = self._mode
         mode = self._mode[0]  # reduce stuff like `r:gz` or `w:gz` down to `r` and `w` for non tarfiles
         write = not mode.startswith("r")
 
         if not archive.exists():
             if write:
                 if check_extension(extensions, CommonExtensions.TAR):
-                    self._handler = tarfile.open(archive, mode=tarfile_mode, **filter_kwargs(TarFile, kwargs=kwargs))  # type: ignore
+                    self._handler = tarfile.open(archive, mode=tarfile_mode, **filter_kwargs(TarFile, kwargs=kwargs))
                     # https://docs.python.org/3/library/tarfile.html#supporting-older-python-versions
                     self._handler.extraction_filter = getattr(tarfile, "data_filter", (lambda member, path: member))
 
                 elif check_extension(extensions, CommonExtensions.ZIP):
                     self._handler = ZipFile(archive, mode=mode, **filter_kwargs(ZipFile, kwargs=kwargs))  # type: ignore
 
                 elif check_extension(extensions, CommonExtensions.SEVENZIP):
@@ -87,15 +97,15 @@
                     raise UnsupportedArchiveOperation('Cannot write a rar file. Rar files only support mode="r"!')
                 else:
                     raise UnsupportedArchiveOperation(f"Unsupported archive format: {archive.suffix}")
             else:
                 raise FileNotFoundError(archive)
 
         elif is_tarfile(archive):
-            self._handler = tarfile.open(archive, mode=tarfile_mode, **filter_kwargs(TarFile, kwargs=kwargs))  # type: ignore
+            self._handler = tarfile.open(archive, mode=tarfile_mode, **filter_kwargs(TarFile, kwargs=kwargs))
 
         elif is_zipfile(archive):
             self._handler = ZipFile(archive, mode=mode, **filter_kwargs(ZipFile, kwargs=kwargs))  # type: ignore
 
         elif is_7zfile(archive):
             if mode == "x":
                 raise FileExistsError(archive)
@@ -118,41 +128,41 @@
     def __exit__(
         self, type: type[BaseException] | None, value: BaseException | None, traceback: TracebackType | None
     ) -> None:
         self._handler.close()
 
     @property
     def file(self) -> Path:
-        """Path to the archive file"""
+        """Path to the archive file."""
         return self._file
 
     @property
     def mode(self) -> OpenArchiveMode:
-        """Mode in which the archive file was opened"""
+        """Mode in which the archive file was opened."""
         return self._mode
 
     @property
     def password(self) -> str | None:
-        """Archive password"""
+        """Archive password."""
         return self._password
 
     @property
     def handler(self) -> str:
-        """Name of the handler used"""
+        """Name of the handler used."""
         return self._handler.__class__.__name__
 
     @validate_call
-    def get_member(self, member: StrPath) -> ArchiveMember:  # type: ignore
+    def get_member(self, member: StrPath) -> ArchiveMember:
         """
-        Get the ArchiveMember object for the member by it's name.
+        Retrieve an ArchiveMember object by it's name.
 
         Parameters
         ----------
-        member: StrPath
-            Name or path of the member as present in the archive.
+        member : StrPath
+            Name of the member.
 
         Returns
         -------
         ArchiveMember
             Represents a member of the archive.
 
         Examples
@@ -180,55 +190,55 @@
                 is_file=tarinfo.isfile(),
             )
 
         elif isinstance(self._handler, ZipFile):
             zipinfo = self._handler.getinfo(member)
             return ArchiveMember(
                 name=zipinfo.filename,
-                size=zipinfo.file_size,  # type: ignore
-                compressed_size=zipinfo.compress_size,  # type: ignore
+                size=zipinfo.file_size,
+                compressed_size=zipinfo.compress_size,
                 datetime=datetime(*zipinfo.date_time),
                 checksum=zipinfo.CRC,
                 is_dir=zipinfo.is_dir(),
                 is_file=not zipinfo.is_dir(),
             )
 
         elif isinstance(self._handler, SevenZipFile):
             member_list = self._handler.list()
             # Unlike the rest, SevenZip member directories do not end with `/`, so we need to strip it out
             sevenzipinfo = [fileinfo for fileinfo in member_list if fileinfo.filename == member.removesuffix("/")][0]
             return ArchiveMember(
                 name=sevenzipinfo.filename,
-                size=sevenzipinfo.uncompressed,  # type: ignore
+                size=sevenzipinfo.uncompressed,
                 # Sometimes sevenzip can return 0 for compressed size when there's no compression
                 # in that case we simply return the uncompressed size instead.
-                compressed_size=sevenzipinfo.compressed or sevenzipinfo.uncompressed,  # type: ignore
-                datetime=sevenzipinfo.creationtime,  # type: ignore
+                compressed_size=sevenzipinfo.compressed or sevenzipinfo.uncompressed,
+                datetime=sevenzipinfo.creationtime,
                 checksum=sevenzipinfo.crc32,
                 is_dir=sevenzipinfo.is_directory,
                 is_file=not sevenzipinfo.is_directory,
             )
 
         else:
             rarinfo: RarInfo = self._handler.getinfo(member)
             is_dir = True if rarinfo.filename.endswith("/") else False
             return ArchiveMember(
                 name=rarinfo.filename,
-                size=rarinfo.file_size,  # type: ignore
-                compressed_size=rarinfo.compress_size,  # type: ignore
+                size=rarinfo.file_size,
+                compressed_size=rarinfo.compress_size,
                 datetime=datetime(*rarinfo.date_time),
                 checksum=rarinfo.CRC,
                 is_dir=is_dir,
                 is_file=not is_dir,
             )
 
     @validate_call
     def get_members(self) -> tuple[ArchiveMember, ...]:
         """
-        Retrieve all members from the archive as a tuple of ArchiveMember objects.
+        Retrieve all members of the archive as a tuple of ArchiveMember objects.
 
         Returns
         -------
         tuple[ArchiveMember, ...]
             Members of the archive as a tuple of ArchiveMember objects.
 
         Examples
@@ -259,15 +269,15 @@
         else:
             names = self._handler.namelist()
             return tuple([self.get_member(name) for name in names])
 
     @validate_call
     def get_names(self) -> tuple[str, ...]:
         """
-        Retrieve names of all members in the archive as a tuple of strings.
+        Retrieve all members of the archive as a tuple of strings.
 
         Returns
         -------
         tuple[str, ...]
             Members of the archive as a tuple of strings.
 
         Examples
@@ -291,73 +301,167 @@
 
         elif isinstance(self._handler, SevenZipFile):
             return tuple(self._handler.getnames())
 
         else:
             return tuple(self._handler.namelist())
 
-    def tree(
+    def print_tree(
         self,
+        *,
         max_depth: int = 0,
-        style: Literal["ansi", "ascii", "const", "const_bold", "rounded", "double"] = "const",
+        style: TreeStyle = "const",
     ) -> None:
         """
         Print the contents of the archive as a tree.
 
         Parameters
         ----------
         max_depth : int, optional
             Maximum depth to print.
-        style : Literal["ansi", "ascii", "const", "const_bold", "rounded", "double"], optional
-            The style of the tree
+        style : TreeStyle, optional
+            The style of the tree.
 
         Returns
         -------
         None
 
+        Notes
+        -----
+        The [`bigtree`](https://pypi.org/p/bigtree/) dependency is required to use this method.
+
+        You can install it via either of these commands:
+
+        - `pip install archivefile[bigtree]`
+        - `pip install archivefile[all]`
+
         Examples
         --------
         ```py
         from archivefile import ArchiveFile
 
-        with ArchiveFile("source.tar") as archive:
-            archive.tree()
-            # hello-world
-            # ├── .github
-            # │   └── workflows
-            # │       ├── docs.yml
-            # │       ├── release.yml
-            # │       └── test.yml
-            # ├── .gitignore
-            # ├── docs
-            # │   └── index.md
-            # ├── pyproject.toml
-            # ├── README.md
-            # ├── src
-            # │   └── hello-world
-            # │       └── __init__.py
-            # ├── tests
-            # │   ├── test_hello_world.py
-            # │   └── __init__.py
-            # └── LICENSE
+        with ArchiveFile("source.tar.gz") as archive:
+            archive.print_tree()
+            # source.tar.gz
+            # └── hello-world
+            #     ├── pyproject.toml
+            #     ├── README.md
+            #     ├── src
+            #     │   └── hello_world
+            #     │       └── __init__.py
+            #     └── tests
+            #         └── __init__.py
         ```
         """
-        tree = list_to_tree(self.get_names())  # type: ignore
+        try:
+            from bigtree.tree.construct import list_to_tree
+        except ModuleNotFoundError:  # pragma: no cover
+            raise ModuleNotFoundError("The 'print_tree()' method requires the 'bigtree' dependency.")
+
+        paths = [f"{self.file.name}/{member}" for member in self.get_names()]
+        tree = list_to_tree(paths)
         tree.show(max_depth=max_depth, style=style)
 
     @validate_call
-    def extract(self, member: StrPath | ArchiveMember, destination: StrPath = Path.cwd()) -> Path:
+    def print_table(
+        self,
+        *,
+        title: str | None = None,
+        style: TableStyle = "markdown",
+        sort_by: SortBy = "name",
+        descending: bool = False,
+        **kwargs: Any,
+    ) -> None:
+        """
+        Print the contents of the archive as a table.
+
+        Parameters
+        ----------
+        title : str, optional
+            Title of the table. Defaults to archive file name.
+        style : TableStyle, optional
+            The style of the table.
+        sort_by : SortBy, optional
+            Key used to sort the table.
+        descending : bool, optional
+            If True, sorting will be in descending order.
+        kwargs : Any
+            Additional keyword arguments to be passed to the [`Table`][rich.table.Table] constructor.
+
+        Returns
+        -------
+        None
+
+        Notes
+        -----
+        The [`rich`](https://pypi.org/p/rich/) dependency is required to use this method.
+
+        You can install it via either of these commands:
+
+        - `pip install archivefile[rich]`
+        - `pip install archivefile[all]`
+
+        Examples
+        --------
+        ```py
+        from archivefile import ArchiveFile
+
+        with ArchiveFile("source.zip") as archive:
+            archive.print_table()
+            #                                                     source.zip
+            #
+            # | Name                                    | Date modified             | Type   | Size | Compressed Size |
+            # |-----------------------------------------|---------------------------|--------|------|-----------------|
+            # | hello-world/                            | 2024-05-02T09:41:24+00:00 | Folder | 0B   | 0B              |
+            # | hello-world/README.md                   | 2024-05-02T09:41:24+00:00 | File   | 0B   | 0B              |
+            # | hello-world/pyproject.toml              | 2024-05-02T09:41:24+00:00 | File   | 363B | 241B            |
+            # | hello-world/src/                        | 2024-05-02T09:41:24+00:00 | Folder | 0B   | 0B              |
+            # | hello-world/src/hello_world/            | 2024-05-02T09:41:24+00:00 | Folder | 0B   | 0B              |
+            # | hello-world/src/hello_world/__init__.py | 2024-05-02T09:41:24+00:00 | File   | 0B   | 0B              |
+            # | hello-world/tests/                      | 2024-05-02T09:41:24+00:00 | Folder | 0B   | 0B              |
+            # | hello-world/tests/__init__.py           | 2024-05-02T09:41:24+00:00 | File   | 0B   | 0B              |
+        ```
+        """
+        try:
+            from rich import box as RichBox
+            from rich import print as richprint
+            from rich.table import Table as RichTable
+        except ModuleNotFoundError:  # pragma: no cover
+            raise ModuleNotFoundError("The 'print_table()' method requires the 'rich' dependency.")
+
+        if title is None:
+            title = self.file.name
+
+        members = self.get_members()
+        table = RichTable(title=title, box=getattr(RichBox, style.upper()), **kwargs)
+        table.add_column("Name", no_wrap=True)
+        table.add_column("Date modified", no_wrap=True)
+        table.add_column("Type", no_wrap=True)
+        table.add_column("Size", no_wrap=True)
+        table.add_column("Compressed Size", no_wrap=True)
+        for member in sorted(members, key=lambda member: getattr(member, sort_by), reverse=descending):
+            table.add_row(
+                member.name,
+                member.datetime.isoformat(),
+                "File" if member.is_file else "Folder",
+                member.size.human_readable(),
+                member.compressed_size.human_readable(),
+            )
+        richprint(table)
+
+    @validate_call
+    def extract(self, member: StrPath | ArchiveMember, *, destination: StrPath = Path.cwd()) -> Path:
         """
-        Extract a member from the archive.
+        Extract a member of the archive.
 
         Parameters
         ----------
-        member: StrPath, ArchiveMember
-            Full name of the member to extract or an ArchiveMember object.
-        destination: StrPath
+        member : StrPath, ArchiveMember
+            Name of the member or an ArchiveMember object.
+        destination : StrPath
             The path to the directory where the member will be extracted.
             If not specified, the current working directory is used as the default destination.
 
         Returns
         -------
         Path
             The path to the extracted file.
@@ -365,25 +469,24 @@
         Examples
         --------
         ```py
         from archivefile import ArchiveFile
 
         with ArchiveFile("source.zip") as archive:
             file = archive.extract("hello-world/pyproject.toml")
-            file.read_text()
+            print(file.read_text())
             # [tool.poetry]
             # name = "hello-world"
             # version = "0.1.0"
             # description = ""
             # readme = "README.md"
             # packages = [{include = "hello_world", from = "src"}]
         ```
         """
-        destination = destination if isinstance(destination, Path) else Path(destination)
-        destination = destination.expanduser().resolve()
+        destination = realpath(destination)
         destination.mkdir(parents=True, exist_ok=True)
 
         if isinstance(member, ArchiveMember):
             member = member.name
 
         if isinstance(member, Path):
             # Do not expand/resolve member if the input is a path
@@ -406,27 +509,27 @@
 
         else:
             self._handler.extract(member=member, path=destination, pwd=self._password)
             return destination / member
 
     @validate_call
     def extractall(
-        self, destination: StrPath = Path.cwd(), members: Iterable[StrPath | ArchiveMember] | None = None
+        self, *, destination: StrPath = Path.cwd(), members: Iterable[StrPath | ArchiveMember] | None = None
     ) -> Path:
         """
-        Extract all members of the archive to destination directory.
+        Extract all the members of the archive to the destination directory.
 
         Parameters
         ----------
-        destination: StrPath
-            The path to the directory where the members will be extracted to.
+        destination : StrPath
+            The path to the directory where the members will be extracted.
             If not specified, the current working directory is used as the default destination.
-        members: Iterable[StrPath | ArchiveMember], optional
+        members : Iterable[StrPath | ArchiveMember], optional
             Iterable of member names or ArchiveMember objects to extract.
-            Default is None which will extract all members.
+            Default is `None` which will extract all members.
 
         Returns
         -------
         Path
             The path to the destination directory.
 
         Examples
@@ -445,74 +548,78 @@
             # /source/hello-world/src
             # /source/hello-world/tests
             # /source/hello-world/src/hello_world
             # /source/hello-world/src/hello_world/__init__.py
             # /source/hello-world/tests/__init__.py
         ```
         """
-        destination = destination if isinstance(destination, Path) else Path(destination)
-        destination = destination.expanduser().resolve()
+        destination = realpath(destination)
         destination.mkdir(parents=True, exist_ok=True)
 
-        members = (
-            [
-                member.relative_to(member.anchor).as_posix()
-                if isinstance(member, Path)
-                else member.name
-                if isinstance(member, ArchiveMember)
-                else member
-                for member in members
-            ]
-            if members
-            else None
-        )
+        names: list[str] = []
+        if members:
+            for member in members:
+                if isinstance(member, ArchiveMember):
+                    names.append(member.name)
+                elif isinstance(member, Path):
+                    names.append(member.relative_to(member.anchor).as_posix())
+                else:
+                    names.append(member)
 
         if isinstance(self._handler, TarFile):
-            self._handler.extractall(path=destination, members=members)  # type: ignore
+            if names:
+                tar_members = [self._handler.getmember(name) for name in names]
+                self._handler.extractall(path=destination, members=tar_members)
+            else:
+                self._handler.extractall(path=destination)
             return destination
 
         elif isinstance(self._handler, ZipFile):
-            self._handler.extractall(
-                path=destination, members=members, pwd=self._password.encode() if self._password else None
-            )
+            password = self._password.encode() if self._password else None
+
+            if names:
+                self._handler.extractall(path=destination, members=names, pwd=password)
+            else:
+                self._handler.extractall(path=destination, pwd=password)
             return destination
 
         elif isinstance(self._handler, SevenZipFile):
             # SevenZipFile doesn't have a members=[...] parameter like the rest
-            if members:
-                self._handler.extract(path=destination, targets=members)
+            if names:
+                self._handler.extract(path=destination, targets=names)
             else:
                 self._handler.extractall(path=destination)
             return destination
 
         else:
-            self._handler.extractall(path=destination, members=members, pwd=self._password)
+            if names:
+                self._handler.extractall(path=destination, members=names, pwd=self._password)
+            else:
+                self._handler.extractall(path=destination, members=names, pwd=self._password)
             return destination
 
     @validate_call
     def read_text(
         self,
         member: StrPath | ArchiveMember,
+        *,
         encoding: str | None = "utf-8",
-        errors: Literal[
-            "strict", "ignore", "replace", "backslashreplace", "surrogateescape", "xmlcharrefreplace", "namereplace"
-        ]
-        | None = None,
+        errors: ErrorHandler | None = None,
     ) -> str:
         """
-        Open the member in text mode, read it, and close the file.
+        Read the member in text mode.
 
         Parameters
         ----------
-        member: StrPath, ArchiveMember
-            Name or path of the member as present in the archive or an ArchiveMember object.
-        encoding: str, optional
+        member : StrPath, ArchiveMember
+            Name of the member or an ArchiveMember object.
+        encoding : str, optional
             Encoding used to read the file. Default is `utf-8`.
-            Setting it to None will use platform-dependent encoding.
-        errors: Literal["strict", "ignore", "replace", "backslashreplace", "surrogateescape", "xmlcharrefreplace", "namereplace"], optional
+            Setting it to `None` will use platform-dependent encoding.
+        errors : ErrorHandler, optional
             String that specifies how encoding and decoding errors are to be handled.
 
         Returns
         -------
         str
             The contents of the file as a string.
 
@@ -523,55 +630,58 @@
 
         Examples
         --------
         ```py
         from archivefile import ArchiveFile
 
         with ArchiveFile("source.zip") as archive:
-            archive.read_text("hello-world/pyproject.toml")
+            text = archive.read_text("hello-world/pyproject.toml")
+            print(text)
             # [tool.poetry]
             # name = "hello-world"
             # version = "0.1.0"
             # description = ""
             # readme = "README.md"
             # packages = [{include = "hello_world", from = "src"}]
         ```
         """
+        # Manage the tmpdir manually to support Python <3.10
         tmpdir = TemporaryDirectory()
         data = self.extract(member, destination=tmpdir.name).read_text(encoding=encoding, errors=errors)
 
         try:
             tmpdir.cleanup()
         except:  # noqa: E722; # pragma: no cover
             pass
 
         return data
 
     @validate_call
     def read_bytes(self, member: StrPath | ArchiveMember) -> bytes:
         """
-        Open the member in bytes mode, read it, and close the file.
+        Read the member in bytes mode.
 
         Parameters
         ----------
-        member: StrPath, ArchiveMember
-            Name or path of the member as present in the archive or an ArchiveMember object.
+        member : StrPath, ArchiveMember
+            Name of the member or an ArchiveMember object.
 
         Returns
         -------
         bytes
             The contents of the file as bytes.
 
         Examples
         --------
         ```py
         from archivefile import ArchiveFile
 
         with ArchiveFile("source.zip") as archive:
-            archive.read_bytes("hello-world/pyproject.toml")
+            data = archive.read_bytes("hello-world/pyproject.toml")
+            print(data)
             # b'[tool.poetry]\\r\\nname = "hello-world"\\r\\nversion = "0.1.0"\\r\\ndescription = ""\\r\\nreadme = "README.md"\\r\\npackages = [{include = "hello_world", from = "src"}]\\r\\n'
         ```
         """
         tmpdir = TemporaryDirectory()
         data = self.extract(member, destination=tmpdir.name).read_bytes()
 
         try:
@@ -581,144 +691,158 @@
 
         return data
 
     @validate_call
     def write(
         self,
         file: StrPath,
+        *,
         arcname: StrPath | None = None,
-        compression_type: ZipCompression | None = None,
-        compression_level: int | None = None,
+        compression_type: CompressionType | None = None,
+        compression_level: CompressionLevel | None = None,
     ) -> None:
         """
         Write a single file to the archive.
 
         Parameters
         ----------
         file : StrPath
-            The path of the file to be added to the archive.
+            Path of the file.
         arcname : StrPath, optional
-            The name which the file will have in the archive.
+            Name which the file will have in the archive.
             Default is the basename of the file.
-        compression_type : ZipCompression, optional
-            The compression method to be used. If None, the default compression
+        compression_type : CompressionType, optional
+            The compression method to be used. If `None`, the default compression
             method of the archive will be used.
-            This ONLY applies to zip files and has no effect on other archives.
-        compression_level : int, optional
-            The compression level to be used. If None, the default compression
+        compression_level : CompressionLevel, optional
+            The compression level to be used. If `None`, the default compression
             level of the archive will be used.
-            This ONLY applies to zip files and has no effect on other archives.
 
         Returns
         -------
         None
 
+        Notes
+        -----
+        Both the `compression_type` and `compression_level` parameters
+        only apply to zip files and have no effect on other archive formats.
+
         Examples
         --------
         ```py
-        from pathlib import Path
-
         from archivefile import ArchiveFile
 
-        file = Path("hello.txt")
-        file.write_text("world")
-
-        with ArchiveFile("newarchive.zip", "w") as archive:
-            archive.write(file)
-            archive.get_names()
-            # ('hello.txt',)
+        with ArchiveFile("example.zip", "w") as archive:
+            archive.write("/root/some/path/to/foo.txt")
+            archive.write("bar.txt", arcname="baz.txt")
+            archive.write("recipe/spam.txt", arcname="ingredients/spam.txt")
+            archive.write("recipe/eggs.txt", arcname="ingredients/eggs.txt")
+            archive.print_tree()
+            # example.zip
+            # ├── foo.txt
+            # ├── baz.txt
+            # └── ingredients
+            #     ├── spam.txt
+            #     └── eggs.txt
         ```
         """
 
-        file = file if isinstance(file, Path) else Path(file)
+        file = realpath(file)
 
         if arcname is None:
             arcname = file.name
 
         if not file.is_file():
             raise UnsupportedArchiveOperation(
                 f"The specified file '{file}' either does not exist or is not a regular file!"
             )
 
         if isinstance(self._handler, TarFile):
             self._handler.add(file, arcname=arcname)
 
         elif isinstance(self._handler, ZipFile):
+            if compression_type == CompressionType.BZIP2:
+                if compression_level == 0:
+                    compression_level = 1
+
             self._handler.write(file, arcname=arcname, compress_type=compression_type, compresslevel=compression_level)
 
         elif isinstance(self._handler, SevenZipFile):
             arcname = arcname.as_posix() if isinstance(arcname, Path) else arcname
             self._handler.write(file, arcname=arcname)
 
         else:  # pragma: no cover
-            # In reality, this can never happen since it'll exist in the constructor before ever reaching here
+            # In reality, this can never happen since it'll exit in the constructor before ever reaching here
             raise UnsupportedArchiveOperation('Cannot write a rar file. Rar files only support mode="r"!')
 
     @validate_call
     def write_text(
         self,
         data: str,
+        *,
         arcname: StrPath,
         encoding: str | None = "utf-8",
-        errors: Literal[
-            "strict", "ignore", "replace", "backslashreplace", "surrogateescape", "xmlcharrefreplace", "namereplace"
-        ]
-        | None = None,
+        errors: ErrorHandler | None = None,
         newline: Literal["", "\n", "\r", "\r\n"] | None = None,
-        compression_type: ZipCompression | None = None,
-        compression_level: int | None = None,
+        compression_type: CompressionType | None = None,
+        compression_level: CompressionLevel | None = None,
     ) -> None:
         """
         Write the string `data` to a file within the archive named `arcname`.
 
         Parameters
         ----------
-        data: str
+        data : str
             The text data to write to the archive.
         arcname : StrPath, optional
             The name which the file will have in the archive.
-        encoding: str, optional
+        encoding : str, optional
             Encoding of the given data. Default is `utf-8`.
-            Setting it to None will use platform-dependent encoding.
-        errors: Literal["strict", "ignore", "replace", "backslashreplace", "surrogateescape", "xmlcharrefreplace", "namereplace"], optional
+            Setting it to `None` will use platform-dependent encoding.
+        errors : ErrorHandler, optional
             String that specifies how encoding and decoding errors are to be handled.
-        newline: Literal['', '\\n', '\\r', '\\r\\n'], optional
-            If newline is None, any '\\n' characters written are translated to the system default line separator, `os.linesep`.
-            If newline is '' or '\\n', no translation takes place.
-            If newline is any of the other legal values, any '\\n' characters written are translated to the given string.
-        compression_type : ZipCompression, optional
-            The compression method to be used. If None, the default compression
+        newline : Literal['', '\\n', '\\r', '\\r\\n'], optional
+            If newline is `None`, any `\\n` characters written are translated to the system default line separator, [`os.linesep`][os.linesep].
+            If newline is `''` or `\\n`, no translation takes place.
+            If newline is any of the other legal values, any `\\n` characters written are translated to the given string.
+        compression_type : CompressionType, optional
+            The compression method to be used. If `None`, the default compression
             method of the archive will be used.
-            This ONLY applies to zip files and has no effect on other archives.
-        compression_level : int, optional
-            The compression level to be used. If None, the default compression
+        compression_level : CompressionLevel, optional
+            The compression level to be used. If `None`, the default compression
             level of the archive will be used.
-            This ONLY applies to zip files and has no effect on other archives.
 
         Returns
         -------
         None
 
+        Notes
+        -----
+        Both the `compression_type` and `compression_level` parameters
+        only apply to zip files and have no effect on other archive formats.
+
         References
         ----------
         - [Encodings](https://docs.python.org/3/library/codecs.html#standard-encodings)
         - [Error Handlers](https://docs.python.org/3/library/codecs.html#error-handlers)
-        - [newline](https://docs.python.org/3/library/functions.html#open)
+        - [Newline](https://docs.python.org/3/library/functions.html#open)
 
         Examples
         --------
         ```py
         from archivefile import ArchiveFile
 
         with ArchiveFile("newarchive.zip", "w") as archive:
-            archive.write_text("hello world", arcname="textworld.txt")
-            archive.get_names()
-            # ('textworld.txt',)
-            archive.read_text("textworld.txt")
-            # 'hello world'
+            archive.write_text("spam and eggs", arcname="recipe.txt")
+            members = archive.get_names()
+            print(members)
+            # ('recipe.txt',)
+            text = archive.read_text("recipe.txt")
+            print(text)
+            # 'spam and eggs'
         ```
         """
 
         arcname = Path(arcname)
         tmpdir = TemporaryDirectory()
         tmppath = Path(tmpdir.name) / arcname.parent
         tmppath.mkdir(parents=True, exist_ok=True)
@@ -733,51 +857,57 @@
         except:  # noqa: E722; # pragma: no cover
             pass
 
     @validate_call
     def write_bytes(
         self,
         data: bytes,
+        *,
         arcname: StrPath,
-        compression_type: ZipCompression | None = None,
-        compression_level: int | None = None,
+        compression_type: CompressionType | None = None,
+        compression_level: CompressionLevel | None = None,
     ) -> None:
         """
-        Write the binary `data` to a file within the archive named `arcname`.
+        Write the bytes `data` to a file within the archive named `arcname`.
 
         Parameters
         ----------
         data: str
             The bytes data to write to the archive.
         arcname : StrPath, optional
             The name which the file will have in the archive.
-        compression_type : ZipCompression, optional
-            The compression method to be used. If None, the default compression
+        compression_type : CompressionType, optional
+            The compression method to be used. If `None`, the default compression
             method of the archive will be used.
-            This ONLY applies to zip files and has no effect on other archives.
-        compression_level : int, optional
-            The compression level to be used. If None, the default compression
+        compression_level : CompressionLevel, optional
+            The compression level to be used. If `None`, the default compression
             level of the archive will be used.
-            This ONLY applies to zip files and has no effect on other archives.
 
         Returns
         -------
         None
 
+        Notes
+        -----
+        Both the `compression_type` and `compression_level` parameters
+        only apply to zip files and have no effect on other archive formats.
+
         Examples
         --------
         ```py
         from archivefile import ArchiveFile
 
-        with ArchiveFile("newarchive.zip", "w") as archive:
-            archive.write_bytes(b"hello world", arcname="bytesworld.txt")
-            archive.get_names()
-            # ('bytesworld.txt',)
-            archive.read_bytes("bytesworld.txt")
-            # b'hello world'
+        with ArchiveFile("skynet.7z", "w") as archive:
+            archive.write_bytes(b"010010100101", arcname="terminator.py")
+            members = archive.get_names()
+            print(members)
+            # ('terminator.py',)
+            data = archive.read_bytes("terminator.py")
+            print(data)
+            # b"010010100101"
         ```
         """
 
         arcname = Path(arcname)
         tmpdir = TemporaryDirectory()
         tmppath = Path(tmpdir.name) / arcname.parent
         tmppath.mkdir(parents=True, exist_ok=True)
@@ -792,80 +922,104 @@
         except:  # noqa: E722; # pragma: no cover
             pass
 
     @validate_call
     def writeall(
         self,
         dir: StrPath,
+        *,
         root: StrPath | None = None,
         glob: str = "*",
         recursive: bool = True,
-        compression_type: ZipCompression | None = None,
-        compression_level: int | None = None,
+        compression_type: CompressionType | None = None,
+        compression_level: CompressionLevel | None = None,
     ) -> None:
         """
         Write a directory to the archive.
 
         Parameters
         ----------
         dir : StrPath
-            The path of the directory to be added to the archive.
+            Path of the directory.
         root : StrPath
             Directory that will be the root directory of the archive, all paths in the archive will be relative to it.
-            This MUST be a component of given directory path. Default is the parent of the given directory.
+            This must be relative to given directory path. Default is the parent of the given directory.
         glob : str, optional
             Only write files that match this glob pattern to the archive.
         recursive : bool, optional
             Recursively write all the files in the given directory. Default is True.
-        compression_type : ZipCompression, optional
-            The compression method to be used. If None, the default compression
+        compression_type : CompressionType, optional
+            The compression method to be used. If `None`, the default compression
             method of the archive will be used.
-            This ONLY applies to zip files and has no effect on other archives.
-        compression_level : int, optional
-            The compression level to be used. If None, the default compression
+        compression_level : CompressionLevel, optional
+            The compression level to be used. If `None`, the default compression
             level of the archive will be used.
-            This ONLY applies to zip files and has no effect on other archives.
 
         Returns
         -------
         None
 
+        Notes
+        -----
+        Both the `compression_type` and `compression_level` parameters
+        only apply to zip files and have no effect on other archive formats.
+
         Examples
         --------
         ```py
         from archivefile import ArchiveFile
 
         with ArchiveFile("source.tar.gz", "w:gz") as archive:
             archive.writeall(dir="hello-world/", glob="*.py")
-            archive.tree()
-            # hello-world
-            # ├── src
-            # │   └── hello_world
-            # │       └── __init__.py
-            # └── tests
-            #     └── __init__.py
+            archive.print_tree()
+            # source.tar.gz
+            # └── hello-world
+            #     ├── pyproject.toml
+            #     ├── README.md
+            #     ├── src
+            #     │   └── hello_world
+            #     │       └── __init__.py
+            #     └── tests
+            #         └── __init__.py
         ```
         """
 
-        dir = dir.expanduser().resolve() if isinstance(dir, Path) else Path(dir).expanduser().resolve()
+        dir = realpath(dir)
 
         if not dir.is_dir():
             raise UnsupportedArchiveOperation(
                 f"The specified file '{dir}' either does not exist or is not a regular directory!"
             )
 
         if root is None:
             root = dir.parent
         else:
-            root = Path(root).expanduser().resolve()
+            root = realpath(root)
 
         if not dir.is_relative_to(root):
             raise ValueError(f"{dir} must be relative to {root}")
 
         files = tuple(dir.rglob(glob)) if recursive else tuple(dir.glob(glob))
 
         for file in files:
             arcname = file.relative_to(root)
             self.write(file, arcname=arcname, compression_type=compression_type, compression_level=compression_level)
 
     def close(self) -> None:
+        """
+        Close the archive file.
+
+        Returns
+        -------
+        None
+
+        Examples
+        --------
+        ```py
+        from archivefile import ArchiveFile
+
+        archive = ArchiveFile("skynet.zip", "w")
+        archive.write_bytes(b"01010101001", arcname="terminator.py")
+        archive.close()
+        ```
+        """
         self._handler.close()
```

### Comparing `archivefile-0.2.0/src/archivefile/_enums.py` & `archivefile-0.3.0/src/archivefile/_enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from __future__ import annotations
 
 from enum import Enum, IntEnum
 
 
-class ZipCompression(IntEnum):
+class CompressionType(IntEnum):
     """Compression algorithms for ZipFile"""
 
-    ZIP_STORED = 0
+    STORED = 0
     """The numeric constant for an uncompressed archive member."""
-    ZIP_DEFLATED = 8
-    """The numeric constant for the usual ZIP compression method. This requires the [zlib](https://docs.python.org/3/library/zlib.html#module-zlib) module."""
-    ZIP_BZIP2 = 12
-    """The numeric constant for the BZIP2 compression method. This requires the [bz2](https://docs.python.org/3/library/bz2.html#module-bz2) module."""
-    ZIP_LZMA = 14
-    """The numeric constant for the LZMA compression method. This requires the [lzma](https://docs.python.org/3/library/lzma.html#module-lzma) module."""
+    DEFLATED = 8
+    """
+    The numeric constant for the usual ZIP compression method. 
+    This requires the [zlib](https://docs.python.org/3/library/zlib.html#module-zlib) module.
+    """
+    BZIP2 = 12
+    """
+    The numeric constant for the BZIP2 compression method. 
+    This requires the [bz2](https://docs.python.org/3/library/bz2.html#module-bz2) module.
+    """
+    LZMA = 14
+    """
+    The numeric constant for the LZMA compression method. 
+    This requires the [lzma](https://docs.python.org/3/library/lzma.html#module-lzma) module.
+    """
 
 
 class CommonExtensions(tuple[str, ...], Enum):
     ZIP = (".zip", ".cbz")
     TAR = (".tar", ".tar.bz2", ".tar.gz", ".tar.xz", ".cbt")
     SEVENZIP = (".7z", ".cb7")
     RAR = (".rar", ".cbr")
```

### Comparing `archivefile-0.2.0/src/archivefile/_utils.py` & `archivefile-0.3.0/src/archivefile/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,31 @@
 from py7zr import is_7zfile
 from rarfile import is_rarfile, is_rarfile_sfx
 
 from archivefile._enums import CommonExtensions
 from archivefile._types import StrPath
 
 
+def realpath(path: StrPath) -> Path:
+    """
+    Get the real path of a given file or directory.
+
+    Parameters
+    ----------
+    path : str or Path
+        A string representing a path or a Path object.
+
+    Returns
+    -------
+    Path
+        The path after expanding the user's home directory and resolving any symbolic links.
+    """
+    return path.expanduser().resolve() if isinstance(path, Path) else Path(path).expanduser().resolve()
+
+
 def filter_kwargs(callabe: Callable[..., Any], kwargs: dict[str, Any]) -> dict[str, Any]:
     """
     Filters out keyword arguments that are not accepted by the class constructor.
 
     Parameters
     ---------
     callabe : Callable[..., Any]
@@ -50,15 +67,15 @@
         Path to the archive file.
 
     Returns
     -------
     bool
         True if the archive is supported, False otherwise.
     """
-    file = file.expanduser().resolve() if isinstance(file, Path) else Path(file).expanduser().resolve()
+    file = realpath(file)
 
     if file.exists():
         return is_tarfile(file) or is_zipfile(file) or is_rarfile(file) or is_rarfile_sfx(file) or is_7zfile(file)
     else:
         return False
```

### Comparing `archivefile-0.2.0/src/archivefile/_version.py` & `archivefile-0.3.0/src/archivefile/_version.py`

 * *Files identical despite different names*

### Comparing `archivefile-0.2.0/PKG-INFO` & `archivefile-0.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-Metadata-Version: 2.1
-Name: archivefile
-Version: 0.2.0
-Summary: Unified interface for tar, zip, sevenzip, and rar files
-Home-page: https://ravencentric.github.io/archivefile
-License: Unlicense
-Keywords: archive,zipfile,tarfile,sevenzip,rarfile,python
-Author: Raventric
-Author-email: 78981416+Ravencentric@users.noreply.github.com
-Requires-Python: >=3.9
-Classifier: License :: OSI Approved
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Typing :: Typed
-Requires-Dist: bigtree (>=0.17.2)
-Requires-Dist: brotli (>=1.1.0) ; platform_python_implementation == "CPython"
-Requires-Dist: brotlicffi (>=1.1.0.0) ; platform_python_implementation == "PyPy"
-Requires-Dist: eval-type-backport (>=0.1.3) ; python_version < "3.10"
-Requires-Dist: importlib-metadata (>=7.1.0) ; python_version < "3.10"
-Requires-Dist: multivolumefile (>=0.2.3)
-Requires-Dist: py7zr (>=0.21.0)
-Requires-Dist: pybcj (>=1.0.2)
-Requires-Dist: pycryptodomex (>=3.20.0)
-Requires-Dist: pydantic (>=2.7.0)
-Requires-Dist: pyppmd (>=1.1.0)
-Requires-Dist: rarfile (>=4.2)
-Requires-Dist: typing-extensions (>=4.11.0)
-Requires-Dist: zipfile-deflate64 (>=0.2.0,<0.3.0)
-Project-URL: Documentation, https://ravencentric.github.io/archivefile
-Project-URL: Repository, https://github.com/Ravencentric/archivefile
-Description-Content-Type: text/markdown
-
 <br/>
 <p align="center">
   <a href="https://github.com/Ravencentric/archivefile">
     <img src="https://raw.githubusercontent.com/Ravencentric/archivefile/main/docs/assets/logo.png" alt="Logo" width="400">
   </a>
   <p align="center">
     Unified interface for tar, zip, sevenzip, and rar files
@@ -74,39 +37,63 @@
 
 `archivefile` wraps the common methods from the above libraries to provide a unified interface that takes care of said differences under the hood. However, it's not as powerful as the libraries it wraps due to lack of support for features that are unique to a specific archive format and library.
 
 ## Installation
 
 `archivefile` is available on [PyPI](https://pypi.org/project/archivefile/), so you can simply use [pip](https://github.com/pypa/pip) to install it.
 
-```sh
-pip install archivefile
-```
+1. Without optional dependencies:
 
-## Usage
+    ```sh
+    pip install archivefile
+    ```
 
-`archivefile` offers a single class called `ArchiveFile` to deal with various archive formats. Some examples are given below:
+2. With optional dependencies:
 
-```py
-from archivefile import ArchiveFile
+    - Required for [`ArchiveFile.print_tree()`](https://ravencentric.github.io/archivefile/api-reference/archivefile/#archivefile.ArchiveFile.print_tree)
+
+        ```sh
+        pip install archivefile[bigtree]
+        ```
 
-with ArchiveFile("archive.tar") as archive:
-    archive.extract("member.txt") # Extract a single member of the archive
+    - Required for [`ArchiveFile.print_table()`](https://ravencentric.github.io/archivefile/api-reference/archivefile/#archivefile.ArchiveFile.print_table)
 
-with ArchiveFile("archive.zip", "w") as archive:
-    archive.extractall(destination="./archive/") # Extract all members
+        ```sh
+        pip install archivefile[rich]
+        ```
 
-with ArchiveFile("archive.cb7") as archive:
-    archive.read_text("member.txt") # Read a member of the archive
+3. With all dependencies:
 
-with ArchiveFile("archive.rar") as archive:
-    archive.get_members() # Get a tuple of all the members of the archive
+    ```sh
+    pip install archivefile[all]
+    ```
+
+## Usage
+
+`archivefile` offers a single class called `ArchiveFile` to deal with various archive formats. Some examples are given below:
+
+```py
+from archivefile import ArchiveFile
 
-with ArchiveFile("archive.zip", "w") as archive:
-    archive.write("bar.txt") # write bar.txt to archive
+with ArchiveFile("../source.zip") as archive:
+    archive.extract("pyproject.toml", destination="./dest/") # Extract a single member by it's name
+    archive.extractall(destination="./dest/") # Extract all members
+    archive.get_member("pyproject.toml")  # Get the ArchiveMember object for the member by it's name
+    archive.get_members()  # Retrieve all members from the archive as a tuple of ArchiveMember objects
+    archive.get_names()  # Retrieve names of all members in the archive as a tuple of strings
+    archive.read_bytes("pyproject.toml") # Read the contents of the member as bytes
+    archive.read_text("pyproject.toml")  # Read the contents of the member as text
+    archive.print_tree()  # Print the contents of the archive as a tree.
+    archive.print_table()  # Print the contents of the archive as a table.
+
+with ArchiveFile("../source.zip", "w") as archive:
+    archive.write("foo.txt", arcname="bar.txt")  # Write foo.txt to the archive as bar.txt
+    archive.writeall("./src/") # Recursively write the ./src/ directory to the archive
+    archive.write_text("spam and eggs", arcname="recipe.txt") # Write a string to the archive as recipe.txt
+    archive.write_bytes(b"0101001010100101", arcname="terminator.py")  # Write bytes to the archive as terminator.py
 ```
 
 Refer to the [API reference](https://ravencentric.github.io/archivefile/api-reference/archivefile/) for more details.
 
 ## Docs
 
 Checkout the complete documentation [here](https://ravencentric.github.io/archivefile/).
```

#### html2text {}

```diff
@@ -1,30 +1,8 @@
-Metadata-Version: 2.1 Name: archivefile Version: 0.2.0 Summary: Unified
-interface for tar, zip, sevenzip, and rar files Home-page: https://
-ravencentric.github.io/archivefile License: Unlicense Keywords:
-archive,zipfile,tarfile,sevenzip,rarfile,python Author: Raventric Author-email:
-78981416+Ravencentric@users.noreply.github.com Requires-Python: >=3.9
-Classifier: License :: OSI Approved Classifier: License :: OSI Approved :: The
-Unlicense (Unlicense) Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Typing :: Typed Requires-Dist: bigtree
-(>=0.17.2) Requires-Dist: brotli (>=1.1.0) ; platform_python_implementation ==
-"CPython" Requires-Dist: brotlicffi (>=1.1.0.0) ;
-platform_python_implementation == "PyPy" Requires-Dist: eval-type-backport
-(>=0.1.3) ; python_version < "3.10" Requires-Dist: importlib-metadata (>=7.1.0)
-; python_version < "3.10" Requires-Dist: multivolumefile (>=0.2.3) Requires-
-Dist: py7zr (>=0.21.0) Requires-Dist: pybcj (>=1.0.2) Requires-Dist:
-pycryptodomex (>=3.20.0) Requires-Dist: pydantic (>=2.7.0) Requires-Dist:
-pyppmd (>=1.1.0) Requires-Dist: rarfile (>=4.2) Requires-Dist: typing-
-extensions (>=4.11.0) Requires-Dist: zipfile-deflate64 (>=0.2.0,<0.3.0)
-Project-URL: Documentation, https://ravencentric.github.io/archivefile Project-
-URL: Repository, https://github.com/Ravencentric/archivefile Description-
-Content-Type: text/markdown
+
                                     _[_L_o_g_o_]
             Unified interface for tar, zip, sevenzip, and rar files
                [![PyPI - Version](https://img.shields.io/pypi/v/
  archivefile?link=https%3A%2F%2Fpypi.org%2Fproject%2Farchivefile%2F)](https://
 pypi.org/project/archivefile/) ![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/archivefile) ![License](https://img.shields.io/github/license/
    Ravencentric/archivefile) ![Checked with mypy](https://www.mypy-lang.org/
@@ -46,24 +24,40 @@
 `.zip`, `.7z`, `.cbr`, `.tar.gz`, etc because each library has a slightly
 different syntax and quirks which you need to deal with. `archivefile` wraps
 the common methods from the above libraries to provide a unified interface that
 takes care of said differences under the hood. However, it's not as powerful as
 the libraries it wraps due to lack of support for features that are unique to a
 specific archive format and library. ## Installation `archivefile` is available
 on [PyPI](https://pypi.org/project/archivefile/), so you can simply use [pip]
-(https://github.com/pypa/pip) to install it. ```sh pip install archivefile ```
-## Usage `archivefile` offers a single class called `ArchiveFile` to deal with
-various archive formats. Some examples are given below: ```py from archivefile
-import ArchiveFile with ArchiveFile("archive.tar") as archive: archive.extract
-("member.txt") # Extract a single member of the archive with ArchiveFile
-("archive.zip", "w") as archive: archive.extractall(destination="./archive/") #
-Extract all members with ArchiveFile("archive.cb7") as archive:
-archive.read_text("member.txt") # Read a member of the archive with ArchiveFile
-("archive.rar") as archive: archive.get_members() # Get a tuple of all the
-members of the archive with ArchiveFile("archive.zip", "w") as archive:
-archive.write("bar.txt") # write bar.txt to archive ``` Refer to the [API
-reference](https://ravencentric.github.io/archivefile/api-reference/
-archivefile/) for more details. ## Docs Checkout the complete documentation
-[here](https://ravencentric.github.io/archivefile/). ## License Distributed
-under the [Unlicense](https://choosealicense.com/licenses/unlicense/) License.
-See [UNLICENSE](https://github.com/Ravencentric/archivefile/blob/main/
-UNLICENSE) for more information.
+(https://github.com/pypa/pip) to install it. 1. Without optional dependencies:
+```sh pip install archivefile ``` 2. With optional dependencies: - Required for
+[`ArchiveFile.print_tree()`](https://ravencentric.github.io/archivefile/api-
+reference/archivefile/#archivefile.ArchiveFile.print_tree) ```sh pip install
+archivefile[bigtree] ``` - Required for [`ArchiveFile.print_table()`](https://
+ravencentric.github.io/archivefile/api-reference/archivefile/
+#archivefile.ArchiveFile.print_table) ```sh pip install archivefile[rich] ```
+3. With all dependencies: ```sh pip install archivefile[all] ``` ## Usage
+`archivefile` offers a single class called `ArchiveFile` to deal with various
+archive formats. Some examples are given below: ```py from archivefile import
+ArchiveFile with ArchiveFile("../source.zip") as archive: archive.extract
+("pyproject.toml", destination="./dest/") # Extract a single member by it's
+name archive.extractall(destination="./dest/") # Extract all members
+archive.get_member("pyproject.toml") # Get the ArchiveMember object for the
+member by it's name archive.get_members() # Retrieve all members from the
+archive as a tuple of ArchiveMember objects archive.get_names() # Retrieve
+names of all members in the archive as a tuple of strings archive.read_bytes
+("pyproject.toml") # Read the contents of the member as bytes archive.read_text
+("pyproject.toml") # Read the contents of the member as text archive.print_tree
+() # Print the contents of the archive as a tree. archive.print_table() # Print
+the contents of the archive as a table. with ArchiveFile("../source.zip", "w")
+as archive: archive.write("foo.txt", arcname="bar.txt") # Write foo.txt to the
+archive as bar.txt archive.writeall("./src/") # Recursively write the ./src/
+directory to the archive archive.write_text("spam and eggs",
+arcname="recipe.txt") # Write a string to the archive as recipe.txt
+archive.write_bytes(b"0101001010100101", arcname="terminator.py") # Write bytes
+to the archive as terminator.py ``` Refer to the [API reference](https://
+ravencentric.github.io/archivefile/api-reference/archivefile/) for more
+details. ## Docs Checkout the complete documentation [here](https://
+ravencentric.github.io/archivefile/). ## License Distributed under the
+[Unlicense](https://choosealicense.com/licenses/unlicense/) License. See
+[UNLICENSE](https://github.com/Ravencentric/archivefile/blob/main/UNLICENSE)
+for more information.
```

