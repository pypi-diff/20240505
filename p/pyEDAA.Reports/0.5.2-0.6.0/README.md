# Comparing `tmp/pyedaa_reports-0.5.2.tar.gz` & `tmp/pyedaa_reports-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyedaa_reports-0.5.2.tar", last modified: Thu Apr 25 19:53:17 2024, max compression
+gzip compressed data, was "pyedaa_reports-0.6.0.tar", last modified: Sun May  5 18:18:47 2024, max compression
```

## Comparing `pyedaa_reports-0.5.2.tar` & `pyedaa_reports-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:17.618942 pyedaa_reports-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-25 19:53:17.614942 pyedaa_reports-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:17.606942 pyedaa_reports-0.5.2/pyEDAA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:17.606942 pyedaa_reports-0.5.2/pyEDAA/Reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:17.610942 pyedaa_reports-0.5.2/pyEDAA/Reports/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/CLI/Unittesting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:17.610942 pyedaa_reports-0.5.2/pyEDAA/Reports/Dependency/
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/Dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:17.610942 pyedaa_reports-0.5.2/pyEDAA/Reports/DocumentationCoverage/
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/DocumentationCoverage/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/DocumentationCoverage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:17.610942 pyedaa_reports-0.5.2/pyEDAA/Reports/Requirement/
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/Requirement/Python.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/Requirement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:17.610942 pyedaa_reports-0.5.2/pyEDAA/Reports/Unittesting/
--rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/Unittesting/JUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/Unittesting/OSVVM.py
--rw-r--r--   0 runner    (1001) docker     (127)    35072 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/Unittesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:17.610942 pyedaa_reports-0.5.2/pyEDAA/Reports/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/resources/Unittesting.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyEDAA/Reports/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:53:17.610942 pyedaa_reports-0.5.2/pyEDAA.Reports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-25 19:53:17.000000 pyedaa_reports-0.5.2/pyEDAA.Reports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-25 19:53:17.000000 pyedaa_reports-0.5.2/pyEDAA.Reports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:53:17.000000 pyedaa_reports-0.5.2/pyEDAA.Reports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 19:53:17.000000 pyedaa_reports-0.5.2/pyEDAA.Reports.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-25 19:53:17.000000 pyedaa_reports-0.5.2/pyEDAA.Reports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 19:53:17.000000 pyedaa_reports-0.5.2/pyEDAA.Reports.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:53:17.618942 pyedaa_reports-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-25 19:53:13.000000 pyedaa_reports-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.260588 pyedaa_reports-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 18:18:47.260588 pyedaa_reports-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.252588 pyedaa_reports-0.6.0/pyEDAA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/CLI/Unittesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/Dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/DocumentationCoverage/
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/DocumentationCoverage/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/DocumentationCoverage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/Requirement/
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Requirement/Python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Requirement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/
+-rw-r--r--   0 runner    (1001) docker     (127)    33757 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/JUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/OSVVM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA/Reports/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/resources/Unittesting.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyEDAA/Reports/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:18:47.256588 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 18:18:47.000000 pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:18:47.260588 pyedaa_reports-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-05 18:18:44.000000 pyedaa_reports-0.6.0/setup.py
```

### Comparing `pyedaa_reports-0.5.2/LICENSE.md` & `pyedaa_reports-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/PKG-INFO` & `pyedaa_reports-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.5.2
+Version: 0.6.0
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
 Project-URL: Issue Tracker, https://GitHub.com/pyEDAA/pyEDAA.Reports/issues
-Keywords: Reports,Abstract Model,Data Model,Test Case,Test Suite,OSVVM,YAML,XML
+Keywords: Reports,Abstract Model,Data Model,Unit Testing,Testcase,Testsuite,OSVVM,YAML,XML
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: lxml~=5.1
 Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: pyTooling~=6.1
-Requires-Dist: lxml~=5.1
 Provides-Extra: doc
-Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
+Requires-Dist: docutils~=0.18.1; extra == "doc"
 Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
-Requires-Dist: pyTooling~=6.1; extra == "doc"
 Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
 Requires-Dist: lxml~=5.1; extra == "doc"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
-Requires-Dist: docutils~=0.18.1; extra == "doc"
-Requires-Dist: sphinx~=7.3; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
 Requires-Dist: autoapi>=2.0.1; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Provides-Extra: test
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
 Requires-Dist: pytest-cov~=5.0; extra == "test"
-Requires-Dist: pytest~=8.1; extra == "test"
 Requires-Dist: Coverage~=7.5; extra == "test"
-Requires-Dist: pyTooling~=6.1; extra == "test"
-Requires-Dist: lxml~=5.1; extra == "test"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
 Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: typing_extensions~=4.11; extra == "test"
+Requires-Dist: pyTooling~=6.1; extra == "test"
+Requires-Dist: lxml~=5.1; extra == "test"
+Requires-Dist: pytest~=8.2; extra == "test"
 Provides-Extra: all
-Requires-Dist: sphinx_design>=0.5.0; extra == "all"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
-Requires-Dist: lxml~=5.1; extra == "all"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
 Requires-Dist: sphinx_reports~=0.6; extra == "all"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
-Requires-Dist: pytest~=8.1; extra == "all"
 Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: sphinx_design>=0.5.0; extra == "all"
 Requires-Dist: mypy~=1.10; extra == "all"
 Requires-Dist: typing_extensions~=4.11; extra == "all"
 Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
 Requires-Dist: pytest-cov~=5.0; extra == "all"
 Requires-Dist: docutils~=0.18.1; extra == "all"
-Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyedaa_reports-0.5.2/README.md` & `pyedaa_reports-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/CLI/Unittesting.py` & `pyedaa_reports-0.6.0/pyEDAA/Reports/CLI/Unittesting.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 from typing import List
 
 from pyTooling.Attributes.ArgParse import CommandHandler
 from pyTooling.Attributes.ArgParse.ValuedFlag import LongValuedFlag
 from pyTooling.MetaClasses import ExtendedType
 
-from pyEDAA.Reports.Unittesting import MergedTestsuiteSummary
-from pyEDAA.Reports.Unittesting.JUnit import JUnitDocument, JUnitReaderMode, UnittestException
+from pyEDAA.Reports.Unittesting       import Document, MergedTestsuiteSummary
+from pyEDAA.Reports.Unittesting.JUnit import Document, JUnitReaderMode, UnittestException
 
 
 class UnittestingHandlers(metaclass=ExtendedType, mixin=True):
 	@CommandHandler("merge-unittest", help="Merge unit testing results.", description="Merge unit testing results.")
 	@LongValuedFlag("--junit", dest="junit", metaName='JUnitFile', help="Unit testing summary file (XML).")
 	def HandleMergeUnittest(self, args: Namespace) -> None:
 		"""Handle program calls with command ``merge-unittest``."""
@@ -24,34 +24,37 @@
 
 		if returnCode != 0:
 			self.Exit(returnCode)
 
 		foundFiles = [f for f in Path.cwd().glob(args.junit)]
 		self.WriteNormal(f"Reading {len(foundFiles)} unit test summary files ...")
 
-		junitDocuments: List[JUnitDocument] = []
+		junitDocuments: List[Document] = []
 		self.WriteVerbose(f"IN (JUnit)  -> Common Data Model:      {args.junit}")
 		for file in foundFiles:
 			self.WriteVerbose(f"  reading {file}")
-			junitDocuments.append(JUnitDocument(file, parse=True, readerMode=JUnitReaderMode.DecoupleTestsuiteHierarchyAndTestcaseClassName))
+			junitDocuments.append(Document(file, parse=True, readerMode=JUnitReaderMode.DecoupleTestsuiteHierarchyAndTestcaseClassName))
 
 		self.WriteNormal(f"Merging unit test summary files to a single file ...")
 
 		merged = MergedTestsuiteSummary("PlatformTesting")
 		for summary in junitDocuments:
 			self.WriteVerbose(f"  merging {summary.Path}")
-			merged.Merge(summary)
+			merged.Merge(summary.ToTestsuiteSummary())
 
 		self.WriteNormal(f"Aggregating unit test metrics ...")
 		merged.Aggregate()
 
+		self.WriteNormal(f"Flattening data structures to a single dimension ...")
+		result = merged.ToTestsuiteSummary()
+
 		self.WriteNormal(f"Writing merged unit test summaries to file ...")
 		mergedFile = Path.cwd() / Path("Unittesting.xml")
 		self.WriteVerbose(f"  Common Data Model -> OUT (JUnit):      {mergedFile}")
-		junitDocument = JUnitDocument.FromTestsuiteSummary(mergedFile, merged)
+		junitDocument = Document.FromTestsuiteSummary(mergedFile, result)
 		try:
 			junitDocument.Write(regenerate=True, overwrite=True)
 		except UnittestException as ex:
 			self.WriteError(str(ex))
 			if ex.__cause__ is not None:
 				self.WriteError(f"  {ex.__cause__}")
```

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/CLI/__init__.py` & `pyedaa_reports-0.6.0/pyEDAA/Reports/CLI/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/Dependency/__init__.py` & `pyedaa_reports-0.6.0/pyEDAA/Reports/Dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/DocumentationCoverage/Python.py` & `pyedaa_reports-0.6.0/pyEDAA/Reports/DocumentationCoverage/Python.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/DocumentationCoverage/__init__.py` & `pyedaa_reports-0.6.0/pyEDAA/Reports/DocumentationCoverage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/Requirement/Python.py` & `pyedaa_reports-0.6.0/pyEDAA/Reports/Requirement/Python.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/Requirement/__init__.py` & `pyedaa_reports-0.6.0/pyEDAA/Reports/Requirement/__init__.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/Unittesting/OSVVM.py` & `pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/OSVVM.py`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/Unittesting/__init__.py` & `pyedaa_reports-0.6.0/pyEDAA/Reports/Unittesting/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 # limitations under the License.                                                                                       #
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
 """Abstraction of testsuites and testcases."""
 from datetime              import timedelta, datetime
-from enum                  import Flag
+from enum                  import Flag, IntEnum
 from pathlib               import Path
 from typing                import Optional as Nullable, Dict, Iterable, Any, Tuple, Generator, Union, List, Generic, TypeVar
 
 from pyTooling.Decorators  import export, readonly
-from pyTooling.MetaClasses import abstractmethod, ExtendedType, mustoverride
+from pyTooling.MetaClasses import ExtendedType, abstractmethod
 from pyTooling.Tree        import Node
 
 from pyEDAA.Reports        import ReportException
 
 
 @export
 class UnittestException(ReportException):
@@ -100,14 +100,24 @@
 			resolved = self.Unknown
 
 		resolved |= (self & self.Flags) | (other & self.Flags)
 		return resolved
 
 
 @export
+class TestsuiteKind(IntEnum):
+	Root = 0
+	Logical = 1
+	Namespace = 2
+	Package = 3
+	Module = 4
+	Class = 5
+
+
+@export
 class TestsuiteStatus(Flag):
 	Unknown =    0
 	Excluded =   1                         #: testcase was permanently excluded / disabled
 	Skipped =    2                         #: testcase was temporarily skipped (e.g. based on a condition)
 	Empty =      4                         #: no tests in suite
 	Passed =     8                         #: passed testcase, because all assertions succeeded
 	Failed =    16                         #: failed testcase due to failing assertions
@@ -330,14 +340,16 @@
 
 	@readonly
 	def TestDuration(self) -> timedelta:
 		return self._testDuration
 
 	@readonly
 	def AssertionCount(self) -> int:
+		if self._assertionCount is None:
+			return 0
 		return self._assertionCount
 
 	@readonly
 	def FailedAssertionCount(self) -> int:
 		return self._failedAssertionCount
 
 	@readonly
@@ -392,14 +404,15 @@
 			f" assert/pass/fail:{self._assertionCount}/{self._passedAssertionCount}/{self._failedAssertionCount} -"
 			f" warn/error/fatal:{self._warningCount}/{self._errorCount}/{self._fatalCount}>"
 		)
 
 
 @export
 class TestsuiteBase(Base, Generic[TestsuiteType]):
+	_kind:       TestsuiteKind
 	_status:     TestsuiteStatus
 	_testsuites: Dict[str, TestsuiteType]
 
 	_tests:        int
 	_inconsistent: int
 	_excluded:     int
 	_skipped:      int
@@ -407,14 +420,15 @@
 	_weak:         int
 	_failed:       int
 	_passed:       int
 
 	def __init__(
 		self,
 		name: str,
+		kind: TestsuiteKind = TestsuiteKind.Logical,
 		startTime: Nullable[datetime] = None,
 		setupDuration: Nullable[timedelta] = None,
 		teardownDuration: Nullable[timedelta] = None,
 		totalDuration:  Nullable[timedelta] = None,
 		status: TestsuiteStatus = TestsuiteStatus.Unknown,
 		warningCount: int = 0,
 		errorCount: int = 0,
@@ -426,14 +440,15 @@
 			if not isinstance(parent, TestsuiteBase):
 				raise TypeError(f"Parameter 'parent' is not of type 'TestsuiteBase'.")
 
 			parent._testsuites[name] = self
 
 		super().__init__(name, startTime, setupDuration, teardownDuration, totalDuration, warningCount, errorCount, fatalCount, parent)
 
+		self._kind = kind
 		self._status = status
 
 		self._testsuites = {}
 		if testsuites is not None:
 			for testsuite in testsuites:
 				if testsuite._parent is not None:
 					raise ValueError(f"Testsuite '{testsuite._name}' is already part of a testsuite hierarchy.")
@@ -468,16 +483,15 @@
 
 	@readonly
 	def TestcaseCount(self) -> int:
 		return sum(testsuite.TestcaseCount for testsuite in self._testsuites.values())
 
 	@readonly
 	def AssertionCount(self) -> int:
-		raise NotImplementedError()
-		# return self._assertionCount
+		return sum(ts.AssertionCount for ts in self._testsuites.values())
 
 	@readonly
 	def FailedAssertionCount(self) -> int:
 		raise NotImplementedError()
 		# return self._assertionCount - (self._warningCount + self._errorCount + self._fatalCount)
 
 	@readonly
@@ -585,15 +599,15 @@
 		testcase._parent = self
 		self._testcases[testcase._name] = testcase
 
 	def AddTestcases(self, testcases: Iterable["Testcase"]) -> None:
 		for testcase in testcases:
 			self.AddTestcase(testcase)
 
-	@mustoverride
+	@abstractmethod
 	def Iterate(self, scheme: IterationScheme = IterationScheme.Default) -> Generator[Union[TestsuiteType, Testcase], None, None]:
 		pass
 
 	def IterateTestsuites(self, scheme: IterationScheme = IterationScheme.TestsuiteDefault) -> Generator[TestsuiteType, None, None]:
 		return self.Iterate(scheme)
 
 	def IterateTestcases(self, scheme: IterationScheme = IterationScheme.TestcaseDefault) -> Generator[Testcase, None, None]:
@@ -618,32 +632,33 @@
 			convertTestsuite(testsuite, rootNode)
 
 		return rootNode
 
 
 @export
 class Testsuite(TestsuiteBase[TestsuiteType]):
-	_testcases:  Dict[str, "Testcase"]
+	_testcases: Dict[str, "Testcase"]
 
 	def __init__(
 		self,
 		name: str,
+		kind: TestsuiteKind = TestsuiteKind.Logical,
 		startTime: Nullable[datetime] = None,
 		setupDuration: Nullable[timedelta] = None,
 		teardownDuration: Nullable[timedelta] = None,
 		totalDuration:  Nullable[timedelta] = None,
 		status: TestsuiteStatus = TestsuiteStatus.Unknown,
 		warningCount: int = 0,
 		errorCount: int = 0,
 		fatalCount: int = 0,
 		testsuites: Nullable[Iterable[TestsuiteType]] = None,
 		testcases: Nullable[Iterable["Testcase"]] = None,
 		parent: Nullable[TestsuiteType] = None
 	):
-		super().__init__(name, startTime, setupDuration, teardownDuration, totalDuration, status, warningCount, errorCount, fatalCount, testsuites, parent)
+		super().__init__(name, kind, startTime, setupDuration, teardownDuration, totalDuration, status, warningCount, errorCount, fatalCount, testsuites, parent)
 
 		# self._testDuration = testDuration
 
 		self._testcases = {}
 		if testcases is not None:
 			for testcase in testcases:
 				if testcase._parent is not None:
@@ -652,21 +667,29 @@
 				if testcase._name in self._testcases:
 					raise DuplicateTestcaseException(f"Testsuite already contains a testcase with same name '{testcase._name}'.")
 
 				testcase._parent = self
 				self._testcases[testcase._name] = testcase
 
 	@readonly
+	def Kind(self) -> TestsuiteKind:
+		return self._kind
+
+	@readonly
 	def Testcases(self) -> Dict[str, "Testcase"]:
 		return self._testcases
 
 	@readonly
 	def TestcaseCount(self) -> int:
 		return super().TestcaseCount + len(self._testcases)
 
+	@readonly
+	def AssertionCount(self) -> int:
+		return super().AssertionCount + sum(tc.AssertionCount for tc in self._testcases.values())
+
 	def Copy(self) -> "Testsuite":
 		return self.__class__(
 			self._name,
 			self._startTime,
 			self._setupDuration,
 			self._teardownDuration,
 			self._totalDuration,
@@ -778,15 +801,15 @@
 		status: TestsuiteStatus = TestsuiteStatus.Unknown,
 		warningCount: int = 0,
 		errorCount: int = 0,
 		fatalCount: int = 0,
 		testsuites: Nullable[Iterable[TestsuiteType]] = None,
 		parent: Nullable[TestsuiteType] = None
 	):
-		super().__init__(name, startTime, setupDuration, teardownDuration, totalDuration, status, warningCount, errorCount, fatalCount, testsuites, parent)
+		super().__init__(name, TestsuiteKind.Root, startTime, setupDuration, teardownDuration, totalDuration, status, warningCount, errorCount, fatalCount, testsuites, parent)
 
 	def Aggregate(self) -> TestsuiteAggregateReturnType:
 		tests, inconsistent, excluded, skipped, errored, weak, failed, passed, warningCount, errorCount, fatalCount = super().Aggregate()
 
 		self._tests = tests
 		self._inconsistent = inconsistent
 		self._excluded = excluded
@@ -968,27 +991,29 @@
 		self._mergedTestcases.append(tc)
 
 		self._warningCount += tc._warningCount
 		self._errorCount += tc._errorCount
 		self._fatalCount += tc._fatalCount
 
 	def ToTestcase(self) -> Testcase:
-		testcase = Testcase(
+		return Testcase(
 			self._name,
 			self._startTime,
 			self._setupDuration,
 			self._testDuration,
 			self._teardownDuration,
 			self._totalDuration,
 			self._status,
+			self._assertionCount,
+			self._failedAssertionCount,
+			self._passedAssertionCount,
 			self._warningCount,
 			self._errorCount,
 			self._fatalCount
 		)
-		return testcase
 
 
 @export
 class MergedTestsuite(Testsuite, Merged):
 	def __init__(
 		self,
 		testsuite: Testsuite,
@@ -997,14 +1022,15 @@
 		parent: Nullable["Testsuite"] = None
 	):
 		if testsuite is None:
 			raise TypeError(f"Parameter 'testsuite' is None.")
 
 		super().__init__(
 			testsuite._name,
+			testsuite._kind,
 			testsuite._startTime,
 			testsuite._setupDuration, testsuite._teardownDuration, testsuite._totalDuration,
 			TestsuiteStatus.Unknown,
 			testsuite._warningCount, testsuite._errorCount, testsuite._fatalCount,
 			parent
 		)
 		Merged.__init__(self)
@@ -1035,27 +1061,35 @@
 			else:
 				mergedTestcase = MergedTestcase(tc)
 				self.AddTestcase(mergedTestcase)
 
 	def ToTestsuite(self) -> Testsuite:
 		testsuite = Testsuite(
 			self._name,
+			self._kind,
 			self._startTime,
 			self._setupDuration,
 			self._teardownDuration,
 			self._totalDuration,
 			self._status,
 			self._warningCount,
 			self._errorCount,
-			self._fatalCount
+			self._fatalCount,
+			testsuites=(ts.ToTestsuite() for ts in self._testsuites.values()),
+			testcases=(tc.ToTestcase() for tc in self._testcases.values())
 		)
-		for ts in self._testsuites.values():
-			testsuite.AddTestsuite(ts.ToTestsuite())
-		for tc in self._testcases.values():
-			testsuite.AddTestcase(tc.ToTestcase())
+
+		testsuite._tests = self._tests
+		testsuite._excluded = self._excluded
+		testsuite._inconsistent = self._inconsistent
+		testsuite._skipped = self._skipped
+		testsuite._errored = self._errored
+		testsuite._weak = self._weak
+		testsuite._failed = self._failed
+		testsuite._passed = self._passed
 
 		return testsuite
 
 
 @export
 class MergedTestsuiteSummary(TestsuiteSummary, Merged):
 	_mergedFiles: Dict[Path, TestsuiteSummary]
@@ -1087,13 +1121,21 @@
 			self._startTime,
 			self._setupDuration,
 			self._teardownDuration,
 			self._totalDuration,
 			self._status,
 			self._warningCount,
 			self._errorCount,
-			self._fatalCount
+			self._fatalCount,
+			testsuites=(ts.ToTestsuite() for ts in self._testsuites.values())
 		)
-		for ts in self._testsuites.values():
-			testsuiteSummary.AddTestsuite(ts.ToTestsuite())
+
+		testsuiteSummary._tests = self._tests
+		testsuiteSummary._excluded = self._excluded
+		testsuiteSummary._inconsistent = self._inconsistent
+		testsuiteSummary._skipped = self._skipped
+		testsuiteSummary._errored = self._errored
+		testsuiteSummary._weak = self._weak
+		testsuiteSummary._failed = self._failed
+		testsuiteSummary._passed = self._passed
 
 		return testsuiteSummary
```

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/__init__.py` & `pyedaa_reports-0.6.0/pyEDAA/Reports/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 """
 Various report abstract data models and report format converters.
 """
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
 __copyright__ = "2021-2024, Electronic Design Automation Abstraction (EDA²)"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "0.5.2"
-__keywords__ =  ["Reports", "Abstract Model", "Data Model", "Test Case", "Test Suite", "OSVVM", "YAML", "XML"]
+__version__ =   "0.6.0"
+__keywords__ =  ["Reports", "Abstract Model", "Data Model", "Unit Testing", "Testcase", "Testsuite", "OSVVM", "YAML", "XML"]
 
 from enum                 import Enum
 from importlib.resources  import files
 from pathlib              import Path
 from sys                  import version_info
 from types                import ModuleType
 from typing               import List, Union
```

### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/resources/Unittesting.xsd` & `pyedaa_reports-0.6.0/pyEDAA/Reports/resources/Unittesting.xsd`

 * *Files 2% similar despite different names*

#### Comparing `pyedaa_reports-0.5.2/pyEDAA/Reports/resources/Unittesting.xsd` & `pyedaa_reports-0.6.0/pyEDAA/Reports/resources/Unittesting.xsd`

```diff
@@ -74,19 +74,19 @@
   <xsd:complexType name="testsuite">
     <xsd:sequence minOccurs="0" maxOccurs="unbounded">
       <xsd:element name="properties" type="properties" minOccurs="0" maxOccurs="1">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">Describes the result of an individual testcase.</xsd:documentation>
         </xsd:annotation>
       </xsd:element>
-      <xsd:element name="testsuite" type="testsuite" minOccurs="0" maxOccurs="unbounded">
-        <xsd:annotation>
-          <xsd:documentation xml:lang="en">Describes the result of an individual testcase.</xsd:documentation>
-        </xsd:annotation>
-      </xsd:element>
+      <!--			<xsd:element name="testsuite" type="testsuite" minOccurs="0" maxOccurs="unbounded">-->
+      <!--				<xsd:annotation>-->
+      <!--					<xsd:documentation xml:lang="en">Describes the result of an individual testcase.</xsd:documentation>-->
+      <!--				</xsd:annotation>-->
+      <!--			</xsd:element>-->
       <xsd:element name="testcase" type="testcase" minOccurs="0" maxOccurs="unbounded">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">Describes the result of an individual testcase.</xsd:documentation>
         </xsd:annotation>
       </xsd:element>
       <xsd:element name="system-out" type="literalblock" minOccurs="0">
         <xsd:annotation>
```

### Comparing `pyedaa_reports-0.5.2/pyEDAA.Reports.egg-info/PKG-INFO` & `pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 Metadata-Version: 2.1
 Name: pyEDAA.Reports
-Version: 0.5.2
+Version: 0.6.0
 Summary: Various report abstract data models and report format converters.
 Home-page: https://GitHub.com/pyEDAA/pyEDAA.Reports
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyEDAA.GitHub.io/pyEDAA.Reports
 Project-URL: Source Code, https://GitHub.com/pyEDAA/pyEDAA.Reports
 Project-URL: Issue Tracker, https://GitHub.com/pyEDAA/pyEDAA.Reports/issues
-Keywords: Reports,Abstract Model,Data Model,Test Case,Test Suite,OSVVM,YAML,XML
+Keywords: Reports,Abstract Model,Data Model,Unit Testing,Testcase,Testsuite,OSVVM,YAML,XML
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: lxml~=5.1
 Requires-Dist: ruamel.yaml~=0.18.6
 Requires-Dist: pyTooling~=6.1
-Requires-Dist: lxml~=5.1
 Provides-Extra: doc
-Requires-Dist: setuptools~=69.5; extra == "doc"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
+Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "doc"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
+Requires-Dist: docutils~=0.18.1; extra == "doc"
 Requires-Dist: colorama>=0.4.6; extra == "doc"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "doc"
 Requires-Dist: sphinx_design>=0.5.0; extra == "doc"
-Requires-Dist: sphinx-copybutton>=0.5.2; extra == "doc"
-Requires-Dist: pyTooling~=6.1; extra == "doc"
 Requires-Dist: sphinx_reports~=0.6; extra == "doc"
+Requires-Dist: pyTooling~=6.1; extra == "doc"
 Requires-Dist: lxml~=5.1; extra == "doc"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "doc"
-Requires-Dist: docutils~=0.18.1; extra == "doc"
-Requires-Dist: sphinx~=7.3; extra == "doc"
+Requires-Dist: setuptools~=69.5; extra == "doc"
 Requires-Dist: autoapi>=2.0.1; extra == "doc"
+Requires-Dist: sphinx~=7.3; extra == "doc"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "doc"
 Provides-Extra: test
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
 Requires-Dist: pytest-cov~=5.0; extra == "test"
-Requires-Dist: pytest~=8.1; extra == "test"
 Requires-Dist: Coverage~=7.5; extra == "test"
-Requires-Dist: pyTooling~=6.1; extra == "test"
-Requires-Dist: lxml~=5.1; extra == "test"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "test"
 Requires-Dist: mypy~=1.10; extra == "test"
 Requires-Dist: typing_extensions~=4.11; extra == "test"
+Requires-Dist: pyTooling~=6.1; extra == "test"
+Requires-Dist: lxml~=5.1; extra == "test"
+Requires-Dist: pytest~=8.2; extra == "test"
 Provides-Extra: all
-Requires-Dist: sphinx_design>=0.5.0; extra == "all"
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == "all"
-Requires-Dist: lxml~=5.1; extra == "all"
-Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: Coverage~=7.5; extra == "all"
 Requires-Dist: sphinx_reports~=0.6; extra == "all"
-Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
-Requires-Dist: pytest~=8.1; extra == "all"
 Requires-Dist: autoapi>=2.0.1; extra == "all"
+Requires-Dist: lxml~=5.1; extra == "all"
+Requires-Dist: ruamel.yaml~=0.18.6; extra == "all"
+Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
+Requires-Dist: colorama>=0.4.6; extra == "all"
+Requires-Dist: sphinx_design>=0.5.0; extra == "all"
 Requires-Dist: mypy~=1.10; extra == "all"
 Requires-Dist: typing_extensions~=4.11; extra == "all"
 Requires-Dist: pyTooling~=6.1; extra == "all"
-Requires-Dist: setuptools~=69.5; extra == "all"
-Requires-Dist: sphinxcontrib-mermaid>=0.9.2; extra == "all"
-Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
-Requires-Dist: colorama>=0.4.6; extra == "all"
-Requires-Dist: Coverage~=7.5; extra == "all"
+Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: pytest~=8.2; extra == "all"
 Requires-Dist: pytest-cov~=5.0; extra == "all"
 Requires-Dist: docutils~=0.18.1; extra == "all"
-Requires-Dist: sphinx~=7.3; extra == "all"
+Requires-Dist: sphinx_rtd_theme~=2.0.0; extra == "all"
+Requires-Dist: setuptools~=69.5; extra == "all"
+Requires-Dist: sphinx_autodoc_typehints~=2.1; extra == "all"
 
 <p align="center">
   <a title="edaa-org.github.io/pyEDAA.Reports" href="https://edaa-org.github.io/pyEDAA.Reports"><img height="80px" src="doc/_static/logo.svg"/></a>
 </p>
 
 [![Sourcecode on GitHub](https://img.shields.io/badge/pyEDAA-Reports-29b6f6.svg?longCache=true&style=flat-square&logo=GitHub&labelColor=0277bd)](https://GitHub.com/edaa-org/pyEDAA.Reports)
 [![Documentation](https://img.shields.io/website?longCache=true&style=flat-square&label=edaa-org.github.io%2FpyEDAA.Reports&logo=GitHub&logoColor=fff&up_color=blueviolet&up_message=Read%20now%20%E2%9E%9A&url=https%3A%2F%2Fedaa-org.github.io%2FpyEDAA.Reports%2Findex.html)](https://edaa-org.github.io/pyEDAA.Reports/)
```

### Comparing `pyedaa_reports-0.5.2/pyEDAA.Reports.egg-info/SOURCES.txt` & `pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/pyEDAA.Reports.egg-info/requires.txt` & `pyedaa_reports-0.6.0/pyEDAA.Reports.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,50 @@
+lxml~=5.1
 ruamel.yaml~=0.18.6
 pyTooling~=6.1
-lxml~=5.1
 
 [all]
-sphinx_design>=0.5.0
 sphinx-copybutton>=0.5.2
-lxml~=5.1
-ruamel.yaml~=0.18.6
+Coverage~=7.5
 sphinx_reports~=0.6
-sphinx_autodoc_typehints~=2.1
-pytest~=8.1
 autoapi>=2.0.1
+lxml~=5.1
+ruamel.yaml~=0.18.6
+sphinxcontrib-mermaid>=0.9.2
+colorama>=0.4.6
+sphinx_design>=0.5.0
 mypy~=1.10
 typing_extensions~=4.11
 pyTooling~=6.1
-setuptools~=69.5
-sphinxcontrib-mermaid>=0.9.2
-sphinx_rtd_theme~=2.0.0
-colorama>=0.4.6
-Coverage~=7.5
+sphinx~=7.3
+pytest~=8.2
 pytest-cov~=5.0
 docutils~=0.18.1
-sphinx~=7.3
+sphinx_rtd_theme~=2.0.0
+setuptools~=69.5
+sphinx_autodoc_typehints~=2.1
 
 [doc]
-setuptools~=69.5
+ruamel.yaml~=0.18.6
+sphinx-copybutton>=0.5.2
 sphinxcontrib-mermaid>=0.9.2
-sphinx_autodoc_typehints~=2.1
-sphinx_rtd_theme~=2.0.0
+docutils~=0.18.1
 colorama>=0.4.6
+sphinx_rtd_theme~=2.0.0
 sphinx_design>=0.5.0
-sphinx-copybutton>=0.5.2
-pyTooling~=6.1
 sphinx_reports~=0.6
+pyTooling~=6.1
 lxml~=5.1
-ruamel.yaml~=0.18.6
-docutils~=0.18.1
-sphinx~=7.3
+setuptools~=69.5
 autoapi>=2.0.1
+sphinx~=7.3
+sphinx_autodoc_typehints~=2.1
 
 [test]
+ruamel.yaml~=0.18.6
 pytest-cov~=5.0
-pytest~=8.1
 Coverage~=7.5
-pyTooling~=6.1
-lxml~=5.1
-ruamel.yaml~=0.18.6
 mypy~=1.10
 typing_extensions~=4.11
+pyTooling~=6.1
+lxml~=5.1
+pytest~=8.2
```

### Comparing `pyedaa_reports-0.5.2/pyproject.toml` & `pyedaa_reports-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyedaa_reports-0.5.2/setup.py` & `pyedaa_reports-0.6.0/setup.py`

 * *Files identical despite different names*

