# Comparing `tmp/litestar_granian-0.2.6.tar.gz` & `tmp/litestar_granian-0.3.0.tar.gz`

## Comparing `litestar_granian-0.2.6.tar` & `litestar_granian-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/Makefile
--rw-r--r--   0        0        0   143265 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/pdm.lock
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/CODEOWNERS
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/cd.yaml
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/docs-preview.yaml
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/pr-title.yaml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/Makefile
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/conf.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/contribution-guide.rst
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/fix_missing_references.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/index.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/reference/config.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/reference/plugin.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/usage/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/docs/usage/placeholder.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/examples/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/examples/basic.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/examples/index.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/examples/structlog.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/litestar_granian/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/litestar_granian/__metadata__.py
--rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/litestar_granian/cli.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/litestar_granian/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/litestar_granian/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/tests/docker-compose.yml
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/tests/test_cli.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/tests/test_plugin.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/LICENSE
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/README.md
--rw-r--r--   0        0        0     8132 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 litestar_granian-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/Makefile
+-rw-r--r--   0        0        0   196295 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/pdm.lock
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/.github/workflows/cd.yaml
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/.github/workflows/docs-preview.yaml
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/.github/workflows/pr-title.yaml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/docs/contribution-guide.rst
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/docs/fix_missing_references.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/docs/index.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/docs/reference/config.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/docs/reference/plugin.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/docs/usage/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/docs/usage/placeholder.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/examples/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/examples/basic.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/examples/index.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/examples/structlog.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/litestar_granian/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/litestar_granian/__metadata__.py
+-rw-r--r--   0        0        0    14120 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/litestar_granian/cli.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/litestar_granian/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/litestar_granian/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/tests/docker-compose.yml
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/README.md
+-rw-r--r--   0        0        0     8615 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 litestar_granian-0.3.0/PKG-INFO
```

### Comparing `litestar_granian-0.2.6/.pre-commit-config.yaml` & `litestar_granian-0.3.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 repos:
   - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v3.1.0
+    rev: v3.2.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.3.4"
+    rev: "v0.4.3"
     hooks:
       - id: ruff
         args: ["--fix"]
         exclude: "docs"
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v1.9.0"
+    rev: "v1.10.0"
     hooks:
       - id: mypy
         exclude: "docs"
         additional_dependencies:
           [
+            asyncpg,
+            asyncpg_stubs,
             granian,
             pytest,
             pytest-mock,
-            "litestar",
+            msgspec,
+            "litestar[sqlalchemy,jwt]",
           ]
   - repo: https://github.com/sphinx-contrib/sphinx-lint
     rev: "v0.9.1"
     hooks:
       - id: sphinx-lint
```

### Comparing `litestar_granian-0.2.6/CONTRIBUTING.rst` & `litestar_granian-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/Makefile` & `litestar_granian-0.3.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 	@if [ "$(USING_PDM)" ]; then $(PDM) config venv.in_project true && python3 -m venv --copies .venv && . $(ENV_PREFIX)/activate && $(ENV_PREFIX)/pip install --quiet -U wheel setuptools cython pip; fi
 	@if [ "$(USING_PDM)" ]; then $(PDM) install -G:all; fi
 	@echo "=> Install complete! Note: If you want to re-install re-run 'make install'"
 
 
 clean: 												## Cleanup temporary build artifacts
 	@echo "=> Cleaning working directory"
+	@if [ "$(USING_PDM)" ]; then $(PDM) run pre-commit clean; fi
 	@rm -rf .pytest_cache .ruff_cache .hypothesis build/ -rf dist/ .eggs/
 	@find . -name '*.egg-info' -exec rm -rf {} +
 	@find . -name '*.egg' -exec rm -f {} +
 	@find . -name '*.pyc' -exec rm -f {} +
 	@find . -name '*.pyo' -exec rm -f {} +
 	@find . -name '*~' -exec rm -f {} +
 	@find . -name '__pycache__' -exec rm -rf {} +
```

### Comparing `litestar_granian-0.2.6/pdm.lock` & `litestar_granian-0.3.0/pdm.lock`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [metadata]
 groups = ["default", "dev", "docs", "linting", "test"]
 strategy = ["cross_platform", "inherit_metadata"]
 lock_version = "4.4.1"
-content_hash = "sha256:7e2a07358cb4ed3a668e4cab45e60f06ac4f94facd7953c667fda0c308497828"
+content_hash = "sha256:de45462789018612d5c2045e0f0194cb384e230208d84b3cbc0f2aa1243420df"
 
 [[package]]
 name = "alabaster"
 version = "0.7.13"
 requires_python = ">=3.6"
 summary = "A configurable sidebar-enabled Sphinx theme"
 groups = ["docs"]
@@ -64,14 +64,44 @@
 ]
 files = [
     {file = "apeye_core-1.1.5-py3-none-any.whl", hash = "sha256:dc27a93f8c9e246b3b238c5ea51edf6115ab2618ef029b9f2d9a190ec8228fbf"},
     {file = "apeye_core-1.1.5.tar.gz", hash = "sha256:5de72ed3d00cc9b20fea55e54b7ab8f5ef8500eb33a5368bc162a5585e238a55"},
 ]
 
 [[package]]
+name = "auto-pytabs"
+version = "0.4.0"
+requires_python = ">=3.8,<4.0"
+summary = "Automatically generate code examples for different Python versions in mkdocs or Sphinx based documentations"
+groups = ["docs"]
+dependencies = [
+    "ruff>=0.0.260",
+]
+files = [
+    {file = "auto_pytabs-0.4.0-py3-none-any.whl", hash = "sha256:941ca4f21b218249ee4d026ebaf4a8a7788a066fdb223571f1f7b93d44ac6a74"},
+    {file = "auto_pytabs-0.4.0.tar.gz", hash = "sha256:4c596aa02ea20c6c85809e5f60a22aa60499dcaa637e52d6313d07c58c5bb61e"},
+]
+
+[[package]]
+name = "auto-pytabs"
+version = "0.4.0"
+extras = ["sphinx"]
+requires_python = ">=3.8,<4.0"
+summary = "Automatically generate code examples for different Python versions in mkdocs or Sphinx based documentations"
+groups = ["docs"]
+dependencies = [
+    "auto-pytabs==0.4.0",
+    "sphinx>=4",
+]
+files = [
+    {file = "auto_pytabs-0.4.0-py3-none-any.whl", hash = "sha256:941ca4f21b218249ee4d026ebaf4a8a7788a066fdb223571f1f7b93d44ac6a74"},
+    {file = "auto_pytabs-0.4.0.tar.gz", hash = "sha256:4c596aa02ea20c6c85809e5f60a22aa60499dcaa637e52d6313d07c58c5bb61e"},
+]
+
+[[package]]
 name = "autodocsumm"
 version = "0.2.12"
 requires_python = ">=3.7"
 summary = "Extended sphinx autodoc including automatic autosummaries"
 groups = ["docs"]
 dependencies = [
     "Sphinx<8.0,>=2.2",
@@ -79,24 +109,24 @@
 files = [
     {file = "autodocsumm-0.2.12-py3-none-any.whl", hash = "sha256:b842b53c686c07a4f174721ca4e729b027367703dbf42e2508863a3c6d6c049c"},
     {file = "autodocsumm-0.2.12.tar.gz", hash = "sha256:848fe8c38df433c6635489499b969cb47cc389ed3d7b6e75c8ccbc94d4b3bf9e"},
 ]
 
 [[package]]
 name = "babel"
-version = "2.14.0"
-requires_python = ">=3.7"
+version = "2.15.0"
+requires_python = ">=3.8"
 summary = "Internationalization utilities"
 groups = ["docs"]
 dependencies = [
     "pytz>=2015.7; python_version < \"3.9\"",
 ]
 files = [
-    {file = "Babel-2.14.0-py3-none-any.whl", hash = "sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287"},
-    {file = "Babel-2.14.0.tar.gz", hash = "sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363"},
+    {file = "Babel-2.15.0-py3-none-any.whl", hash = "sha256:08706bdad8d0a3413266ab61bd6c34d0c28d6e1e7badf40a2cebe67644e2e1fb"},
+    {file = "babel-2.15.0.tar.gz", hash = "sha256:8daf0e265d05768bc6c7a314cf1321e9a123afc328cc635c18622a2f30a04413"},
 ]
 
 [[package]]
 name = "beautifulsoup4"
 version = "4.12.3"
 requires_python = ">=3.6.0"
 summary = "Screen-scraping library"
@@ -106,14 +136,68 @@
 ]
 files = [
     {file = "beautifulsoup4-4.12.3-py3-none-any.whl", hash = "sha256:b80878c9f40111313e55da8ba20bdba06d8fa3969fc68304167741bbf9e082ed"},
     {file = "beautifulsoup4-4.12.3.tar.gz", hash = "sha256:74e3d1928edc070d21748185c46e3fb33490f22f52a3addee9aee0f4f7781051"},
 ]
 
 [[package]]
+name = "black"
+version = "24.4.2"
+requires_python = ">=3.8"
+summary = "The uncompromising code formatter."
+groups = ["docs"]
+dependencies = [
+    "click>=8.0.0",
+    "mypy-extensions>=0.4.3",
+    "packaging>=22.0",
+    "pathspec>=0.9.0",
+    "platformdirs>=2",
+    "tomli>=1.1.0; python_version < \"3.11\"",
+    "typing-extensions>=4.0.1; python_version < \"3.11\"",
+]
+files = [
+    {file = "black-24.4.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:dd1b5a14e417189db4c7b64a6540f31730713d173f0b63e55fabd52d61d8fdce"},
+    {file = "black-24.4.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:8e537d281831ad0e71007dcdcbe50a71470b978c453fa41ce77186bbe0ed6021"},
+    {file = "black-24.4.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eaea3008c281f1038edb473c1aa8ed8143a5535ff18f978a318f10302b254063"},
+    {file = "black-24.4.2-cp310-cp310-win_amd64.whl", hash = "sha256:7768a0dbf16a39aa5e9a3ded568bb545c8c2727396d063bbaf847df05b08cd96"},
+    {file = "black-24.4.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:257d724c2c9b1660f353b36c802ccece186a30accc7742c176d29c146df6e474"},
+    {file = "black-24.4.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:bdde6f877a18f24844e381d45e9947a49e97933573ac9d4345399be37621e26c"},
+    {file = "black-24.4.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e151054aa00bad1f4e1f04919542885f89f5f7d086b8a59e5000e6c616896ffb"},
+    {file = "black-24.4.2-cp311-cp311-win_amd64.whl", hash = "sha256:7e122b1c4fb252fd85df3ca93578732b4749d9be076593076ef4d07a0233c3e1"},
+    {file = "black-24.4.2-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:accf49e151c8ed2c0cdc528691838afd217c50412534e876a19270fea1e28e2d"},
+    {file = "black-24.4.2-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:88c57dc656038f1ab9f92b3eb5335ee9b021412feaa46330d5eba4e51fe49b04"},
+    {file = "black-24.4.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:be8bef99eb46d5021bf053114442914baeb3649a89dc5f3a555c88737e5e98fc"},
+    {file = "black-24.4.2-cp312-cp312-win_amd64.whl", hash = "sha256:415e686e87dbbe6f4cd5ef0fbf764af7b89f9057b97c908742b6008cc554b9c0"},
+    {file = "black-24.4.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:bf10f7310db693bb62692609b397e8d67257c55f949abde4c67f9cc574492cc7"},
+    {file = "black-24.4.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:98e123f1d5cfd42f886624d84464f7756f60ff6eab89ae845210631714f6db94"},
+    {file = "black-24.4.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:48a85f2cb5e6799a9ef05347b476cce6c182d6c71ee36925a6c194d074336ef8"},
+    {file = "black-24.4.2-cp38-cp38-win_amd64.whl", hash = "sha256:b1530ae42e9d6d5b670a34db49a94115a64596bc77710b1d05e9801e62ca0a7c"},
+    {file = "black-24.4.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:37aae07b029fa0174d39daf02748b379399b909652a806e5708199bd93899da1"},
+    {file = "black-24.4.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:da33a1a5e49c4122ccdfd56cd021ff1ebc4a1ec4e2d01594fef9b6f267a9e741"},
+    {file = "black-24.4.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ef703f83fc32e131e9bcc0a5094cfe85599e7109f896fe8bc96cc402f3eb4b6e"},
+    {file = "black-24.4.2-cp39-cp39-win_amd64.whl", hash = "sha256:b9176b9832e84308818a99a561e90aa479e73c523b3f77afd07913380ae2eab7"},
+    {file = "black-24.4.2-py3-none-any.whl", hash = "sha256:d36ed1124bb81b32f8614555b34cc4259c3fbc7eec17870e8ff8ded335b58d8c"},
+    {file = "black-24.4.2.tar.gz", hash = "sha256:c872b53057f000085da66a19c55d68f6f8ddcac2642392ad3a355878406fbd4d"},
+]
+
+[[package]]
+name = "blacken-docs"
+version = "1.16.0"
+requires_python = ">=3.8"
+summary = "Run Black on Python code blocks in documentation files."
+groups = ["docs"]
+dependencies = [
+    "black>=22.1.0",
+]
+files = [
+    {file = "blacken_docs-1.16.0-py3-none-any.whl", hash = "sha256:b0dcb84b28ebfb352a2539202d396f50e15a54211e204a8005798f1d1edb7df8"},
+    {file = "blacken_docs-1.16.0.tar.gz", hash = "sha256:b4bdc3f3d73898dfbf0166f292c6ccfe343e65fc22ddef5319c95d1a8dcc6c1c"},
+]
+
+[[package]]
 name = "cachecontrol"
 version = "0.14.0"
 requires_python = ">=3.7"
 summary = "httplib2 caching for requests"
 groups = ["docs"]
 dependencies = [
     "msgpack<2.0.0,>=0.5.2",
@@ -271,148 +355,148 @@
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "coverage"
-version = "7.4.4"
+version = "7.5.1"
 requires_python = ">=3.8"
 summary = "Code coverage measurement for Python"
 groups = ["test"]
 files = [
-    {file = "coverage-7.4.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2"},
-    {file = "coverage-7.4.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf"},
-    {file = "coverage-7.4.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8"},
-    {file = "coverage-7.4.4-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562"},
-    {file = "coverage-7.4.4-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2"},
-    {file = "coverage-7.4.4-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7"},
-    {file = "coverage-7.4.4-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87"},
-    {file = "coverage-7.4.4-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c"},
-    {file = "coverage-7.4.4-cp310-cp310-win32.whl", hash = "sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d"},
-    {file = "coverage-7.4.4-cp310-cp310-win_amd64.whl", hash = "sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f"},
-    {file = "coverage-7.4.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf"},
-    {file = "coverage-7.4.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083"},
-    {file = "coverage-7.4.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63"},
-    {file = "coverage-7.4.4-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f"},
-    {file = "coverage-7.4.4-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227"},
-    {file = "coverage-7.4.4-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd"},
-    {file = "coverage-7.4.4-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384"},
-    {file = "coverage-7.4.4-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b"},
-    {file = "coverage-7.4.4-cp311-cp311-win32.whl", hash = "sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286"},
-    {file = "coverage-7.4.4-cp311-cp311-win_amd64.whl", hash = "sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec"},
-    {file = "coverage-7.4.4-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76"},
-    {file = "coverage-7.4.4-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818"},
-    {file = "coverage-7.4.4-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978"},
-    {file = "coverage-7.4.4-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70"},
-    {file = "coverage-7.4.4-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51"},
-    {file = "coverage-7.4.4-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c"},
-    {file = "coverage-7.4.4-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48"},
-    {file = "coverage-7.4.4-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9"},
-    {file = "coverage-7.4.4-cp312-cp312-win32.whl", hash = "sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0"},
-    {file = "coverage-7.4.4-cp312-cp312-win_amd64.whl", hash = "sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e"},
-    {file = "coverage-7.4.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384"},
-    {file = "coverage-7.4.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1"},
-    {file = "coverage-7.4.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a"},
-    {file = "coverage-7.4.4-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409"},
-    {file = "coverage-7.4.4-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e"},
-    {file = "coverage-7.4.4-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd"},
-    {file = "coverage-7.4.4-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7"},
-    {file = "coverage-7.4.4-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c"},
-    {file = "coverage-7.4.4-cp38-cp38-win32.whl", hash = "sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e"},
-    {file = "coverage-7.4.4-cp38-cp38-win_amd64.whl", hash = "sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8"},
-    {file = "coverage-7.4.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d"},
-    {file = "coverage-7.4.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357"},
-    {file = "coverage-7.4.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e"},
-    {file = "coverage-7.4.4-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e"},
-    {file = "coverage-7.4.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4"},
-    {file = "coverage-7.4.4-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec"},
-    {file = "coverage-7.4.4-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd"},
-    {file = "coverage-7.4.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade"},
-    {file = "coverage-7.4.4-cp39-cp39-win32.whl", hash = "sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57"},
-    {file = "coverage-7.4.4-cp39-cp39-win_amd64.whl", hash = "sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c"},
-    {file = "coverage-7.4.4-pp38.pp39.pp310-none-any.whl", hash = "sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677"},
-    {file = "coverage-7.4.4.tar.gz", hash = "sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146"},
+    {file = "coverage-7.5.1-cp310-cp310-win32.whl", hash = "sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228"},
+    {file = "coverage-7.5.1-cp310-cp310-win_amd64.whl", hash = "sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987"},
+    {file = "coverage-7.5.1-cp311-cp311-win32.whl", hash = "sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136"},
+    {file = "coverage-7.5.1-cp311-cp311-win_amd64.whl", hash = "sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7"},
+    {file = "coverage-7.5.1-cp312-cp312-win32.whl", hash = "sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19"},
+    {file = "coverage-7.5.1-cp312-cp312-win_amd64.whl", hash = "sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596"},
+    {file = "coverage-7.5.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:e2213def81a50519d7cc56ed643c9e93e0247f5bbe0d1247d15fa520814a7cd7"},
+    {file = "coverage-7.5.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:5037f8fcc2a95b1f0e80585bd9d1ec31068a9bcb157d9750a172836e98bc7a90"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5c3721c2c9e4c4953a41a26c14f4cef64330392a6d2d675c8b1db3b645e31f0e"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca498687ca46a62ae590253fba634a1fe9836bc56f626852fb2720f334c9e4e5"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0cdcbc320b14c3e5877ee79e649677cb7d89ef588852e9583e6b24c2e5072661"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:57e0204b5b745594e5bc14b9b50006da722827f0b8c776949f1135677e88d0b8"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:8fe7502616b67b234482c3ce276ff26f39ffe88adca2acf0261df4b8454668b4"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:9e78295f4144f9dacfed4f92935fbe1780021247c2fabf73a819b17f0ccfff8d"},
+    {file = "coverage-7.5.1-cp38-cp38-win32.whl", hash = "sha256:1434e088b41594baa71188a17533083eabf5609e8e72f16ce8c186001e6b8c41"},
+    {file = "coverage-7.5.1-cp38-cp38-win_amd64.whl", hash = "sha256:0646599e9b139988b63704d704af8e8df7fa4cbc4a1f33df69d97f36cb0a38de"},
+    {file = "coverage-7.5.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4cc37def103a2725bc672f84bd939a6fe4522310503207aae4d56351644682f1"},
+    {file = "coverage-7.5.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:fc0b4d8bfeabd25ea75e94632f5b6e047eef8adaed0c2161ada1e922e7f7cece"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0d0a0f5e06881ecedfe6f3dd2f56dcb057b6dbeb3327fd32d4b12854df36bf26"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9735317685ba6ec7e3754798c8871c2f49aa5e687cc794a0b1d284b2389d1bd5"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d21918e9ef11edf36764b93101e2ae8cc82aa5efdc7c5a4e9c6c35a48496d601"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:c3e757949f268364b96ca894b4c342b41dc6f8f8b66c37878aacef5930db61be"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:79afb6197e2f7f60c4824dd4b2d4c2ec5801ceb6ba9ce5d2c3080e5660d51a4f"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:d1d0d98d95dd18fe29dc66808e1accf59f037d5716f86a501fc0256455219668"},
+    {file = "coverage-7.5.1-cp39-cp39-win32.whl", hash = "sha256:1cc0fe9b0b3a8364093c53b0b4c0c2dd4bb23acbec4c9240b5f284095ccf7981"},
+    {file = "coverage-7.5.1-cp39-cp39-win_amd64.whl", hash = "sha256:dde0070c40ea8bb3641e811c1cfbf18e265d024deff6de52c5950677a8fb1e0f"},
+    {file = "coverage-7.5.1-pp38.pp39.pp310-none-any.whl", hash = "sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312"},
+    {file = "coverage-7.5.1.tar.gz", hash = "sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c"},
 ]
 
 [[package]]
 name = "coverage"
-version = "7.4.4"
+version = "7.5.1"
 extras = ["toml"]
 requires_python = ">=3.8"
 summary = "Code coverage measurement for Python"
 groups = ["test"]
 dependencies = [
-    "coverage==7.4.4",
+    "coverage==7.5.1",
     "tomli; python_full_version <= \"3.11.0a6\"",
 ]
 files = [
-    {file = "coverage-7.4.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2"},
-    {file = "coverage-7.4.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf"},
-    {file = "coverage-7.4.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8"},
-    {file = "coverage-7.4.4-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562"},
-    {file = "coverage-7.4.4-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2"},
-    {file = "coverage-7.4.4-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7"},
-    {file = "coverage-7.4.4-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87"},
-    {file = "coverage-7.4.4-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c"},
-    {file = "coverage-7.4.4-cp310-cp310-win32.whl", hash = "sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d"},
-    {file = "coverage-7.4.4-cp310-cp310-win_amd64.whl", hash = "sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f"},
-    {file = "coverage-7.4.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf"},
-    {file = "coverage-7.4.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083"},
-    {file = "coverage-7.4.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63"},
-    {file = "coverage-7.4.4-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f"},
-    {file = "coverage-7.4.4-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227"},
-    {file = "coverage-7.4.4-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd"},
-    {file = "coverage-7.4.4-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384"},
-    {file = "coverage-7.4.4-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b"},
-    {file = "coverage-7.4.4-cp311-cp311-win32.whl", hash = "sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286"},
-    {file = "coverage-7.4.4-cp311-cp311-win_amd64.whl", hash = "sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec"},
-    {file = "coverage-7.4.4-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76"},
-    {file = "coverage-7.4.4-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818"},
-    {file = "coverage-7.4.4-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978"},
-    {file = "coverage-7.4.4-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70"},
-    {file = "coverage-7.4.4-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51"},
-    {file = "coverage-7.4.4-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c"},
-    {file = "coverage-7.4.4-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48"},
-    {file = "coverage-7.4.4-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9"},
-    {file = "coverage-7.4.4-cp312-cp312-win32.whl", hash = "sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0"},
-    {file = "coverage-7.4.4-cp312-cp312-win_amd64.whl", hash = "sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e"},
-    {file = "coverage-7.4.4-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384"},
-    {file = "coverage-7.4.4-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1"},
-    {file = "coverage-7.4.4-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a"},
-    {file = "coverage-7.4.4-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409"},
-    {file = "coverage-7.4.4-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e"},
-    {file = "coverage-7.4.4-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd"},
-    {file = "coverage-7.4.4-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7"},
-    {file = "coverage-7.4.4-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c"},
-    {file = "coverage-7.4.4-cp38-cp38-win32.whl", hash = "sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e"},
-    {file = "coverage-7.4.4-cp38-cp38-win_amd64.whl", hash = "sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8"},
-    {file = "coverage-7.4.4-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d"},
-    {file = "coverage-7.4.4-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357"},
-    {file = "coverage-7.4.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e"},
-    {file = "coverage-7.4.4-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e"},
-    {file = "coverage-7.4.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4"},
-    {file = "coverage-7.4.4-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec"},
-    {file = "coverage-7.4.4-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd"},
-    {file = "coverage-7.4.4-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade"},
-    {file = "coverage-7.4.4-cp39-cp39-win32.whl", hash = "sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57"},
-    {file = "coverage-7.4.4-cp39-cp39-win_amd64.whl", hash = "sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c"},
-    {file = "coverage-7.4.4-pp38.pp39.pp310-none-any.whl", hash = "sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677"},
-    {file = "coverage-7.4.4.tar.gz", hash = "sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c0884920835a033b78d1c73b6d3bbcda8161a900f38a488829a83982925f6c2e"},
+    {file = "coverage-7.5.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:39afcd3d4339329c5f58de48a52f6e4e50f6578dd6099961cf22228feb25f38f"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4a7b0ceee8147444347da6a66be737c9d78f3353b0681715b668b72e79203e4a"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:4a9ca3f2fae0088c3c71d743d85404cec8df9be818a005ea065495bedc33da35"},
+    {file = "coverage-7.5.1-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5fd215c0c7d7aab005221608a3c2b46f58c0285a819565887ee0b718c052aa4e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4bf0655ab60d754491004a5efd7f9cccefcc1081a74c9ef2da4735d6ee4a6223"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:61c4bf1ba021817de12b813338c9be9f0ad5b1e781b9b340a6d29fc13e7c1b5e"},
+    {file = "coverage-7.5.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:db66fc317a046556a96b453a58eced5024af4582a8dbdc0c23ca4dbc0d5b3146"},
+    {file = "coverage-7.5.1-cp310-cp310-win32.whl", hash = "sha256:b016ea6b959d3b9556cb401c55a37547135a587db0115635a443b2ce8f1c7228"},
+    {file = "coverage-7.5.1-cp310-cp310-win_amd64.whl", hash = "sha256:df4e745a81c110e7446b1cc8131bf986157770fa405fe90e15e850aaf7619bc8"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:796a79f63eca8814ca3317a1ea443645c9ff0d18b188de470ed7ccd45ae79428"},
+    {file = "coverage-7.5.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:4fc84a37bfd98db31beae3c2748811a3fa72bf2007ff7902f68746d9757f3746"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6175d1a0559986c6ee3f7fccfc4a90ecd12ba0a383dcc2da30c2b9918d67d8a3"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1fc81d5878cd6274ce971e0a3a18a8803c3fe25457165314271cf78e3aae3aa2"},
+    {file = "coverage-7.5.1-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:556cf1a7cbc8028cb60e1ff0be806be2eded2daf8129b8811c63e2b9a6c43bca"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:9981706d300c18d8b220995ad22627647be11a4276721c10911e0e9fa44c83e8"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:d7fed867ee50edf1a0b4a11e8e5d0895150e572af1cd6d315d557758bfa9c057"},
+    {file = "coverage-7.5.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:ef48e2707fb320c8f139424a596f5b69955a85b178f15af261bab871873bb987"},
+    {file = "coverage-7.5.1-cp311-cp311-win32.whl", hash = "sha256:9314d5678dcc665330df5b69c1e726a0e49b27df0461c08ca12674bcc19ef136"},
+    {file = "coverage-7.5.1-cp311-cp311-win_amd64.whl", hash = "sha256:5fa567e99765fe98f4e7d7394ce623e794d7cabb170f2ca2ac5a4174437e90dd"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:b6cf3764c030e5338e7f61f95bd21147963cf6aa16e09d2f74f1fa52013c1206"},
+    {file = "coverage-7.5.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:2ec92012fefebee89a6b9c79bc39051a6cb3891d562b9270ab10ecfdadbc0c34"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:16db7f26000a07efcf6aea00316f6ac57e7d9a96501e990a36f40c965ec7a95d"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:beccf7b8a10b09c4ae543582c1319c6df47d78fd732f854ac68d518ee1fb97fa"},
+    {file = "coverage-7.5.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8748731ad392d736cc9ccac03c9845b13bb07d020a33423fa5b3a36521ac6e4e"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:7352b9161b33fd0b643ccd1f21f3a3908daaddf414f1c6cb9d3a2fd618bf2572"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:7a588d39e0925f6a2bff87154752481273cdb1736270642aeb3635cb9b4cad07"},
+    {file = "coverage-7.5.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:68f962d9b72ce69ea8621f57551b2fa9c70509af757ee3b8105d4f51b92b41a7"},
+    {file = "coverage-7.5.1-cp312-cp312-win32.whl", hash = "sha256:f152cbf5b88aaeb836127d920dd0f5e7edff5a66f10c079157306c4343d86c19"},
+    {file = "coverage-7.5.1-cp312-cp312-win_amd64.whl", hash = "sha256:5a5740d1fb60ddf268a3811bcd353de34eb56dc24e8f52a7f05ee513b2d4f596"},
+    {file = "coverage-7.5.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:e2213def81a50519d7cc56ed643c9e93e0247f5bbe0d1247d15fa520814a7cd7"},
+    {file = "coverage-7.5.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:5037f8fcc2a95b1f0e80585bd9d1ec31068a9bcb157d9750a172836e98bc7a90"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5c3721c2c9e4c4953a41a26c14f4cef64330392a6d2d675c8b1db3b645e31f0e"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca498687ca46a62ae590253fba634a1fe9836bc56f626852fb2720f334c9e4e5"},
+    {file = "coverage-7.5.1-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0cdcbc320b14c3e5877ee79e649677cb7d89ef588852e9583e6b24c2e5072661"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:57e0204b5b745594e5bc14b9b50006da722827f0b8c776949f1135677e88d0b8"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:8fe7502616b67b234482c3ce276ff26f39ffe88adca2acf0261df4b8454668b4"},
+    {file = "coverage-7.5.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:9e78295f4144f9dacfed4f92935fbe1780021247c2fabf73a819b17f0ccfff8d"},
+    {file = "coverage-7.5.1-cp38-cp38-win32.whl", hash = "sha256:1434e088b41594baa71188a17533083eabf5609e8e72f16ce8c186001e6b8c41"},
+    {file = "coverage-7.5.1-cp38-cp38-win_amd64.whl", hash = "sha256:0646599e9b139988b63704d704af8e8df7fa4cbc4a1f33df69d97f36cb0a38de"},
+    {file = "coverage-7.5.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4cc37def103a2725bc672f84bd939a6fe4522310503207aae4d56351644682f1"},
+    {file = "coverage-7.5.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:fc0b4d8bfeabd25ea75e94632f5b6e047eef8adaed0c2161ada1e922e7f7cece"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0d0a0f5e06881ecedfe6f3dd2f56dcb057b6dbeb3327fd32d4b12854df36bf26"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9735317685ba6ec7e3754798c8871c2f49aa5e687cc794a0b1d284b2389d1bd5"},
+    {file = "coverage-7.5.1-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d21918e9ef11edf36764b93101e2ae8cc82aa5efdc7c5a4e9c6c35a48496d601"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:c3e757949f268364b96ca894b4c342b41dc6f8f8b66c37878aacef5930db61be"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:79afb6197e2f7f60c4824dd4b2d4c2ec5801ceb6ba9ce5d2c3080e5660d51a4f"},
+    {file = "coverage-7.5.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:d1d0d98d95dd18fe29dc66808e1accf59f037d5716f86a501fc0256455219668"},
+    {file = "coverage-7.5.1-cp39-cp39-win32.whl", hash = "sha256:1cc0fe9b0b3a8364093c53b0b4c0c2dd4bb23acbec4c9240b5f284095ccf7981"},
+    {file = "coverage-7.5.1-cp39-cp39-win_amd64.whl", hash = "sha256:dde0070c40ea8bb3641e811c1cfbf18e265d024deff6de52c5950677a8fb1e0f"},
+    {file = "coverage-7.5.1-pp38.pp39.pp310-none-any.whl", hash = "sha256:6537e7c10cc47c595828b8a8be04c72144725c383c4702703ff4e42e44577312"},
+    {file = "coverage-7.5.1.tar.gz", hash = "sha256:54de9ef3a9da981f7af93eafde4ede199e0846cd819eb27c88e2b712aae9708c"},
 ]
 
 [[package]]
 name = "cssutils"
-version = "2.9.0"
+version = "2.10.2"
 requires_python = ">=3.8"
 summary = "A CSS Cascading Style Sheets library for Python"
 groups = ["docs"]
 files = [
-    {file = "cssutils-2.9.0-py3-none-any.whl", hash = "sha256:f8b013169e281c0c6083207366c5005f5dd4549055f7aba840384fb06a78745c"},
-    {file = "cssutils-2.9.0.tar.gz", hash = "sha256:89477b3d17d790e97b9fb4def708767061055795aae6f7c82ae32e967c9be4cd"},
+    {file = "cssutils-2.10.2-py3-none-any.whl", hash = "sha256:4ad7d2f29270b22cf199f65a6b5e795f2c3130f3b9fb50c3d45e5054ef86e41a"},
+    {file = "cssutils-2.10.2.tar.gz", hash = "sha256:93cf92a350b1c123b17feff042e212f94d960975a3ed145743d84ebe8ccec7ab"},
 ]
 
 [[package]]
 name = "dict2css"
 version = "0.3.0.post1"
 requires_python = ">=3.6"
 summary = "A μ-library for constructing cascading style sheets from Python dictionaries."
@@ -461,118 +545,279 @@
 files = [
     {file = "domdf_python_tools-3.8.0.post2-py3-none-any.whl", hash = "sha256:ad2c763c8d00850a7fa92ad95e9891a1918281ea25322c4dbb1734fd32f905dd"},
     {file = "domdf_python_tools-3.8.0.post2.tar.gz", hash = "sha256:a1fd255ea29f767b08de462d2da39d360262304389227d980bc307ee8aa3366a"},
 ]
 
 [[package]]
 name = "exceptiongroup"
-version = "1.2.0"
+version = "1.2.1"
 requires_python = ">=3.7"
 summary = "Backport of PEP 654 (exception groups)"
 groups = ["default", "dev", "test"]
 marker = "python_version < \"3.11\""
 files = [
-    {file = "exceptiongroup-1.2.0-py3-none-any.whl", hash = "sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14"},
-    {file = "exceptiongroup-1.2.0.tar.gz", hash = "sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68"},
+    {file = "exceptiongroup-1.2.1-py3-none-any.whl", hash = "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad"},
+    {file = "exceptiongroup-1.2.1.tar.gz", hash = "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"},
 ]
 
 [[package]]
 name = "faker"
-version = "24.3.0"
+version = "25.0.1"
 requires_python = ">=3.8"
 summary = "Faker is a Python package that generates fake data for you."
 groups = ["default"]
 dependencies = [
     "python-dateutil>=2.4",
-    "typing-extensions>=3.10.0.1; python_version <= \"3.8\"",
 ]
 files = [
-    {file = "Faker-24.3.0-py3-none-any.whl", hash = "sha256:9978025e765ba79f8bf6154c9630a9c2b7f9c9b0f175d4ad5e04b19a82a8d8d6"},
-    {file = "Faker-24.3.0.tar.gz", hash = "sha256:5fb5aa9749d09971e04a41281ae3ceda9414f683d4810a694f8a8eebb8f9edec"},
+    {file = "Faker-25.0.1-py3-none-any.whl", hash = "sha256:6737cc6d591cd83421fdc5e494f6e2c1a6e32266214f158b745aa9fa15687c98"},
+    {file = "Faker-25.0.1.tar.gz", hash = "sha256:c153505618801f1704807b258a6010ea8cabf91f66f4788939bfdba83b887e76"},
 ]
 
 [[package]]
 name = "filelock"
-version = "3.13.2"
+version = "3.14.0"
 requires_python = ">=3.8"
 summary = "A platform independent file lock."
 groups = ["docs", "linting"]
 files = [
-    {file = "filelock-3.13.2-py3-none-any.whl", hash = "sha256:e4c33bc026ace328551af557d4d34f59566c98acd4ed66c13b4335f114f04f7a"},
-    {file = "filelock-3.13.2.tar.gz", hash = "sha256:9e2106260b5f65600a31bc503721e3db7e64598bb406ebc5921aeaafe441ba34"},
+    {file = "filelock-3.14.0-py3-none-any.whl", hash = "sha256:43339835842f110ca7ae60f1e1c160714c5a6afd15a2873419ab185334975c0f"},
+    {file = "filelock-3.14.0.tar.gz", hash = "sha256:6ea72da3be9b8c82afd3edcf99f2fffbb5076335a5ae4d03248bb5b6c3eae78a"},
+]
+
+[[package]]
+name = "git-cliff"
+version = "2.2.1"
+requires_python = ">=3.7"
+summary = "A highly customizable changelog generator ⛰️"
+groups = ["docs"]
+files = [
+    {file = "git_cliff-2.2.1-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:f7c6550733a60e135f821ac999ee6804f185089ae6b7bb4f91dad32a8d95a2d5"},
+    {file = "git_cliff-2.2.1-py3-none-macosx_11_0_arm64.whl", hash = "sha256:e624814e9273f8a4000fb7425842a7c062631234a84092a9d551f24520c956db"},
+    {file = "git_cliff-2.2.1-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:548c994d902e74e2e104e4603ac29419020d3d54eaf5ce3b8e17e77493448faf"},
+    {file = "git_cliff-2.2.1-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:739447e3c22c7aa964f0900b4f63234a5ff8246988797a70f3245fc37cebf1b5"},
+    {file = "git_cliff-2.2.1-py3-none-manylinux_2_28_aarch64.whl", hash = "sha256:aea2aa2250b5fff738294e7eee1c458ba4dadc81fc823d31f29eb1c689ee09d0"},
+    {file = "git_cliff-2.2.1-py3-none-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:0645822f4ff4aaf68e7fa61fd31a583ccef9793a71b0a34c50c9fac43d90a254"},
+    {file = "git_cliff-2.2.1-py3-none-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:01a02869e3b186f173d1f14db11f7c7130394195fc6e352ac0e3cd505d65104f"},
+    {file = "git_cliff-2.2.1-py3-none-win32.whl", hash = "sha256:e98bf87ee7b22eacdba0e74016f93b6d6d1fea6cb2cf67742c3aaa1614fafef9"},
+    {file = "git_cliff-2.2.1-py3-none-win_amd64.whl", hash = "sha256:e57155dbb3a895c09ed358137d0d1d30d3f15971456f3c48ede9bfd37434ce75"},
+    {file = "git_cliff-2.2.1.tar.gz", hash = "sha256:6db64534dc5ec3d7656b9be6ddf7004cfd1ddf8f815f66d41bc9330f42b61d6d"},
 ]
 
 [[package]]
 name = "granian"
-version = "1.2.0"
+version = "1.3.1"
 requires_python = ">=3.8"
 summary = "A Rust HTTP server for Python applications"
 groups = ["default"]
 dependencies = [
-    "typer>=0.4.2",
+    "click>=8.0.0",
     "uvloop~=0.18.0; sys_platform != \"win32\" and platform_python_implementation == \"CPython\"",
 ]
 files = [
-    {file = "granian-1.2.0-cp310-cp310-macosx_10_12_x86_64.whl", hash = "sha256:5281550c5afb04bc37f4700753c48402086529a2605e4193098cf06891ab8ad5"},
-    {file = "granian-1.2.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0d2b352fd0ad43da62090226258e2fc58ba6df2c3751ae5746702a4bfceb0416"},
-    {file = "granian-1.2.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:884dd7b3694fb39383b9498670093fe788cf238662ec4e77bf9792e16301ef57"},
-    {file = "granian-1.2.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f89db63f0868b80ebcafdcd2fd48fc3c678605f14fd7dcc738cbe67893dd2dd1"},
-    {file = "granian-1.2.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:7fe60c397a54702758ec35d62b49ae75cc9c3b5ba8792638da3c12d3b3ff2871"},
-    {file = "granian-1.2.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:dca886f8093258d8344770772ce5706f0ea7907fdbe794aeca19c1821cfc1d1b"},
-    {file = "granian-1.2.0-cp310-none-win_amd64.whl", hash = "sha256:81a1c7e078c47981ab2d201424f0d92266431e61e569d12fece014d268dc3d28"},
-    {file = "granian-1.2.0-cp311-cp311-macosx_10_12_x86_64.whl", hash = "sha256:b903be7fb3f8dbc4b05d52a4bbefd81a739cd5f68c86e7105f98e9af6dedec1f"},
-    {file = "granian-1.2.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:5273afdbeec6e2361eba83c1c2978cb22a94840a9d551b9f73b3bca8e9cf11e9"},
-    {file = "granian-1.2.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:dec49f94ef357d23c644f0da1d1763495bde1fbd5af043f8e40413302483afe5"},
-    {file = "granian-1.2.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dc0a48d4872a82ade351931693aeece12e195ac8b9fb9b4b57cf31bce3189c63"},
-    {file = "granian-1.2.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:ce0bb3f40d79ccec3f5e0de8d73a83b0c19737c723ec637b0d064f7407c7cfcc"},
-    {file = "granian-1.2.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:47da8e77c6a75deb7d7113174a034eaa351d78336cec7b047d2a9db14ebde55e"},
-    {file = "granian-1.2.0-cp311-none-win_amd64.whl", hash = "sha256:77eb93da378d9db4b64fab1342f5bd45f082417abadd7e339f443a8c9cb640fc"},
-    {file = "granian-1.2.0-cp312-cp312-macosx_10_12_x86_64.whl", hash = "sha256:19665980e5f467d92c641ac6cbac1923d8eec20f8818be987f9c464e596fc151"},
-    {file = "granian-1.2.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:8d137624c621d81175c37af57489b715d93ae6ca63b5693efae7dcbce998775c"},
-    {file = "granian-1.2.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:94c322b5868eb9712d40a7eec48ebd828cb37a416594e5ca146eb7f47e7d130c"},
-    {file = "granian-1.2.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eb1bacb93039cd6ae1b4fa4fdbb82da11405acd85d4074e87b866017fdb03446"},
-    {file = "granian-1.2.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:81ed88465e61652b5048295ed70c51c13007318e52b52204264bb5aa87384ba1"},
-    {file = "granian-1.2.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:677bd15e3bb817a8974c622416ff8d49a2a52055baa8dcc49cca5a94c7cebd82"},
-    {file = "granian-1.2.0-cp312-none-win_amd64.whl", hash = "sha256:7ae64f383b0931e13cbbe1c27299858935f91803cb5f640cc2a66b95973dd58a"},
-    {file = "granian-1.2.0-cp38-cp38-macosx_10_12_x86_64.whl", hash = "sha256:ab1d1acdca2d6732c32cd95d488d8062d1c0dc01ef3060665497f515777877be"},
-    {file = "granian-1.2.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:b53a31f176b8e886881958cc800540dc53cf96c04fb5a0c7b232ce9524d6f3cc"},
-    {file = "granian-1.2.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:263551e4c5ee9dfc01d451e1cf55bbd7f2c0e94255db40728f2a2dc8afd86503"},
-    {file = "granian-1.2.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c1df3cb06484b259877cf1eadfae55beb2acca73651e35ea4a5496f17c9e4566"},
-    {file = "granian-1.2.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:9bee095a33abe3a50058eef062ff23e62da1531632478f7a6465874213c0df2b"},
-    {file = "granian-1.2.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:7e97be52bd5fa173fc9f4f5a7a63888e9126508171cae8a670ce7009f1d40783"},
-    {file = "granian-1.2.0-cp38-none-win_amd64.whl", hash = "sha256:cf27e0f297f543a151eb59172b23082bd0168700f4cfb1b2020ac9ac674075fa"},
-    {file = "granian-1.2.0-cp39-cp39-macosx_10_12_x86_64.whl", hash = "sha256:71d8c169a7670662fca6f34a3c488c96cf60347dc09e4f54f8fd0e551b20ba97"},
-    {file = "granian-1.2.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:6efa84dc48bd658b60c20c9528c1160e5ac9450f312d2340092086ca246efda3"},
-    {file = "granian-1.2.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8d216084c6f6efaf8fc6237aceea97e502a305141648dfad7a563249fe4a2978"},
-    {file = "granian-1.2.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dba42bc31941c90cc8e1af97988d2a3eae5134ac145c588f0b73ad21e0caa68f"},
-    {file = "granian-1.2.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:79e30f51524cf8d61c0dabeee7092007d99c52260d517f1c7cf357a6029a0da9"},
-    {file = "granian-1.2.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:e0ed76f3feea883744ddd0ffc69795e98e7b9bdb8dd5c1c4317a24ef3319f7dd"},
-    {file = "granian-1.2.0-cp39-none-win_amd64.whl", hash = "sha256:92e69a9276e85c37e5a5087640e698820bd9d979506c58b59a4e3e79375b689c"},
-    {file = "granian-1.2.0-pp310-pypy310_pp73-macosx_10_12_x86_64.whl", hash = "sha256:7438488ed2db8f8530b461b7641c5b39588633685b46660df8f45c6ab3a0c492"},
-    {file = "granian-1.2.0-pp310-pypy310_pp73-macosx_11_0_arm64.whl", hash = "sha256:8d3e9852a16c5e3a6e53423416ff0b349861a0b5d1df4feed705d125589156f4"},
-    {file = "granian-1.2.0-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a25daacb5293f5b562e7e388b355be7c506a60bcc7dd742424f90a9885bc1f1d"},
-    {file = "granian-1.2.0-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:244a3632bd4ec75dfb5cd46e410655553a2eaf2c118696f1fb7d86f04a960ed8"},
-    {file = "granian-1.2.0-pp310-pypy310_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:130a7c5f1ed8593a7849d0325511158b531ae09f27730dbab7514ba8f8087e16"},
-    {file = "granian-1.2.0-pp310-pypy310_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:f93a5a4caba990e405a94946be1b52d977dfa18a6dd839007b12aa1c318ac1d5"},
-    {file = "granian-1.2.0-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:1f47a85d89bff4661ec67ec21640e1d24ab36cec88679aa965def241368eaf5f"},
-    {file = "granian-1.2.0-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:12178f539fca7d31f35850515f91928ede958d373cd75ef3a57de108e3613ddb"},
-    {file = "granian-1.2.0-pp38-pypy38_pp73-macosx_11_0_arm64.whl", hash = "sha256:74eb03358f80bfc3102b081ebcbd8581cdb6e22f034e62f2986ff2a03ca050f6"},
-    {file = "granian-1.2.0-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:13707a064884788ff696d9d8a5a019c7a6022d91d45dd4cfd2353ae932500a7b"},
-    {file = "granian-1.2.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8886d06cd66126b9bd67e070040be049ca84deb59a7ba5bb3541add7d7b0c24b"},
-    {file = "granian-1.2.0-pp38-pypy38_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:94a7a4d90265ff7cddb04d646a8b6d0c57c525cff9bb63f9e363cb71d92af996"},
-    {file = "granian-1.2.0-pp38-pypy38_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:c6efa7eb11f36ee909dcbb1c0b90ead50bc121a721ff891246ff127a88625148"},
-    {file = "granian-1.2.0-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:6bd5994f90926e23ef7011b319b6dd13410248cb3b972287dadc2939779cbda6"},
-    {file = "granian-1.2.0-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:6ececc06e01bf90ade3a816ea07a90fe69a46759ed28171fe993f0196f316d1b"},
-    {file = "granian-1.2.0-pp39-pypy39_pp73-macosx_11_0_arm64.whl", hash = "sha256:4acaaa2ec009ae04a7c64e1afcf892134c18c32548bc67f877f05e7dbc37e649"},
-    {file = "granian-1.2.0-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f5f825445145586bc23c03838783a8339688f68a5eb4f5c8db66b9a051664357"},
-    {file = "granian-1.2.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d569f03cd0fd149ef06e0bc901aedf0212571960ea838c7df7ccf0e8f1d88317"},
-    {file = "granian-1.2.0-pp39-pypy39_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:985f93b1f2297870aaedd55237b53c60309c757f718c19a0a3d6d0ceb738a929"},
-    {file = "granian-1.2.0-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:2112769592d7714f4205c7eecd5629a576d07bcf6d21cc14818162c924276340"},
-    {file = "granian-1.2.0-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:e3ea97a436ca18876fd4523b5d6622c833a69b07ef87b9a3e37d5f6d65969c3b"},
-    {file = "granian-1.2.0.tar.gz", hash = "sha256:c9dbbda5c66faf2717a927cf237b4691b8e07c84109a9c4cf3040c8e9fc27083"},
+    {file = "granian-1.3.1-cp310-cp310-macosx_10_12_x86_64.whl", hash = "sha256:a6c459af46ff5b3d7d2fcef6d4cae7e1d962c05d9041349efeb49c6e03a3a4ad"},
+    {file = "granian-1.3.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:6eb338e9d78f14ce9fcee8afd39691d703d26f6a17f0a31e807e790f62818cc5"},
+    {file = "granian-1.3.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7885ffa80977b9ab96308b11311cf01387c880b0ee7b39c4051f18b34706389a"},
+    {file = "granian-1.3.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5df1fa92c4789d17183810929658cf2f7969b64e04d3777c843196d73a68ce6d"},
+    {file = "granian-1.3.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:396203f11ce8406710055194ff75a54bc17703f5139cdddc86f2e9cbb80ebba2"},
+    {file = "granian-1.3.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b783057f22408b4515ddbfbd9fbd8508a9df29e7523c774c3bc3da14cc56c27e"},
+    {file = "granian-1.3.1-cp310-none-win_amd64.whl", hash = "sha256:6dd3b46a457935d01cc80e1294c22f00fd0d700c91df498030557bcd1a99c9b9"},
+    {file = "granian-1.3.1-cp311-cp311-macosx_10_12_x86_64.whl", hash = "sha256:f682b40f39286423f1ae5426ad3cbafe0b36e6521bb360cc0882385b4f11cd28"},
+    {file = "granian-1.3.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:310581f719ea7c43a9bab1c71ab9c62b09b3b91bd254fed0af8b707531d27a8f"},
+    {file = "granian-1.3.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:26bc8e9d2d13d251f442b2241cc73d53025a5a4b17a563e957286562df0bafca"},
+    {file = "granian-1.3.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75f472b93a0ed0e4a1675de465eedf96f67b9585e3ae03272bc250734ff7c5e0"},
+    {file = "granian-1.3.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:422077b6f95a0c4cc6be139c38230595de1ee3e64f5cd4a5b366ac9e94a70e1b"},
+    {file = "granian-1.3.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:a2767b4c4a2c0fdb1f5c4f1b843901063afc65d8c2be118f063b08eb28b8ac36"},
+    {file = "granian-1.3.1-cp311-none-win_amd64.whl", hash = "sha256:2c606bfdeab0709aadfff7b705c3e25fb94434dc5acc26b12531aec3baef9558"},
+    {file = "granian-1.3.1-cp312-cp312-macosx_10_12_x86_64.whl", hash = "sha256:e9f60164ba0588db3701ed4b2348893c118257e4374da1747813fb4c33870d68"},
+    {file = "granian-1.3.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:2993c8b9e3fe8e82ad60e892d7bb7ae77670038e06cff9e89f770c858937e697"},
+    {file = "granian-1.3.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7245c041a0bca32e99457f398a9c8b8774609b56e548326aa906b465fae0ec6c"},
+    {file = "granian-1.3.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3118bbb0f47c0374b968787c780f5edcde2653fd8874dd3c753b5bd6b71f6cdf"},
+    {file = "granian-1.3.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:411eb1520496f03beca7d3ab28b6adb7738d6f0ac500f2f45dbd8ea24d9639b9"},
+    {file = "granian-1.3.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:65cd2cf834dd9fe393add340c4cf2237184684aac4e503b0b447fc691c704378"},
+    {file = "granian-1.3.1-cp312-none-win_amd64.whl", hash = "sha256:54517442e7622de643444bd43a13e4b2461771e3c38313c267a9ac0e476a9abb"},
+    {file = "granian-1.3.1-cp38-cp38-macosx_10_12_x86_64.whl", hash = "sha256:3350c71e4fd36f2eb30144cad20f5e21f40b6494e6ce17fa2b6c26d3099c661a"},
+    {file = "granian-1.3.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:d4b2015e5937435016b2c25f545ac476ffcde6aa2526fa8252a2cec5c5686353"},
+    {file = "granian-1.3.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2a1e07cabc89ba015fb717232181c14405852237ded401bb962728f07642e125"},
+    {file = "granian-1.3.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50501a23c128c2f491d4454b2185f089070f6ec147f4742531c2b8460136a3b9"},
+    {file = "granian-1.3.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:5244bb8e8d404cba127b0737ad89ad2a624df00995ed471e7584f3f1b957c0df"},
+    {file = "granian-1.3.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:f7cde47ec2eecca3773806c1f63a3a71392e46be26711e1b6d988924d4acf6bf"},
+    {file = "granian-1.3.1-cp38-none-win_amd64.whl", hash = "sha256:fd3d8106d96f85e50dc128d72b94a5234e6452e9976befb258af1278124fde4f"},
+    {file = "granian-1.3.1-cp39-cp39-macosx_10_12_x86_64.whl", hash = "sha256:3ededcc3cea77077f793903ca8263149afcbefb05a04e1e8fa68110f4059aabb"},
+    {file = "granian-1.3.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:b37605f3427605599a9ac1312825b386f1c41f1896f59bbbf0ce3055ac817354"},
+    {file = "granian-1.3.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c34cd9cc12401186a4d4e54c0fdae0471d670c3d3bc555e0912ac2c45917840e"},
+    {file = "granian-1.3.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c8a936228840b9915cd153fc9dc570055df81ee43f5eea6bc30e18e73e3c5fe4"},
+    {file = "granian-1.3.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:10affc0400b257efd2509d1ce15f3eaef14b0b45fcd821b036de483b9bcae38a"},
+    {file = "granian-1.3.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:6ae60fb4b5fd3f5489bab5f5c36b2a72b1195f5f990aac90cde5ec3de1588e5a"},
+    {file = "granian-1.3.1-cp39-none-win_amd64.whl", hash = "sha256:e3132f37da4e38b85fe5ae6360e6b48ce340cb98349af148433288a6bbdf1d3e"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-macosx_10_12_x86_64.whl", hash = "sha256:5d57123c49b72d282b94a8842ac274d161016f70b289b3c08e08f2f7d8283c6e"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-macosx_11_0_arm64.whl", hash = "sha256:1cbfeeb22d95bb6cfc797f996be60f21a643d603c6e4a0eb56ebb1a4015b5e25"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b332bf511130a68cc5b17f0b8927125be6769e8cdf46ebd297fdffc9fa5d66ff"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:57019cdfbb4e5b3b1903c6b08d308732ed5341b6c441916f934cb240103729f1"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:1406d803a5f3c9b11a6848fa1abdc5fc2f39f527675f61368c77cb843b8d3bfc"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:135a61579bf2fd20dc86ea6c754117ee661c884cf8bd8917f765b47e9e6773c8"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:1aebcc9dc3556917ba5d2995165370fd3e04d533c54c1ba2ca611c2d94d036e0"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:ad6a874d56e249020ed45e1a840cbf21a3d414fde89fbe0153035ab37a16dc37"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-macosx_11_0_arm64.whl", hash = "sha256:aa42e80b54af7fa32db57d4382115c0267830c3e17eac17811e9e613c763cf45"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2132f60309eea7bf9d6a847582853a067b0ca51c0fd4927d18e54a251a8707b5"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a9592d3eaf6d0f14abfc825eccd55b62b74abd4513da8fabbab1eebd2d013b71"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:c71b18d3a6f5980ab044861678cccce9e6fd6c5e401cc53b02f7605f2f31cb9d"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:09818af44ac163d8a2c2df068f4db2d3a6032d3d22a226a309fcaf4989e6798e"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:0145fa076a6ad993498e255c67b4fd647a03803a51ee30de856ba66659dd0b1e"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:1bc2879cc56fbdf7350481f40a213ceba13360a281b1748b0e2ed1edc3d7630d"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-macosx_11_0_arm64.whl", hash = "sha256:67bac881cbcc2bb56a1a0a4190c97c73314088f8ddfdd99b9379959e432dc9d3"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:48df73ae1840a223b85e93de870c7cc8314b918e8e5af4de9220a2510c6cc2f6"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:555a573754dd8b4c01a75a75d7dcbad016e8a726c06f8fc10b530a9ea58d0c50"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:9cb51fb2b37567a24f984dc6fcd2a3ba4a40c1af6b794e2f4a74206989eda11f"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:70676812437274aab6520e11f729e870da058c894406ac6048dfb631cd90523d"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:39a7720d5bc2867863c5a9844eff8cc4ccf2a3ce916390c8015a81c31f725703"},
+    {file = "granian-1.3.1.tar.gz", hash = "sha256:4b5381a5e6eb20e702c72b8c87becdea36bc8f3e322c5fe7bfca53982c537e51"},
+]
+
+[[package]]
+name = "granian"
+version = "1.3.1"
+extras = ["all"]
+requires_python = ">=3.8"
+summary = "A Rust HTTP server for Python applications"
+groups = ["default"]
+dependencies = [
+    "granian==1.3.1",
+    "granian[pname,reload]",
+]
+files = [
+    {file = "granian-1.3.1-cp310-cp310-macosx_10_12_x86_64.whl", hash = "sha256:a6c459af46ff5b3d7d2fcef6d4cae7e1d962c05d9041349efeb49c6e03a3a4ad"},
+    {file = "granian-1.3.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:6eb338e9d78f14ce9fcee8afd39691d703d26f6a17f0a31e807e790f62818cc5"},
+    {file = "granian-1.3.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7885ffa80977b9ab96308b11311cf01387c880b0ee7b39c4051f18b34706389a"},
+    {file = "granian-1.3.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5df1fa92c4789d17183810929658cf2f7969b64e04d3777c843196d73a68ce6d"},
+    {file = "granian-1.3.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:396203f11ce8406710055194ff75a54bc17703f5139cdddc86f2e9cbb80ebba2"},
+    {file = "granian-1.3.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b783057f22408b4515ddbfbd9fbd8508a9df29e7523c774c3bc3da14cc56c27e"},
+    {file = "granian-1.3.1-cp310-none-win_amd64.whl", hash = "sha256:6dd3b46a457935d01cc80e1294c22f00fd0d700c91df498030557bcd1a99c9b9"},
+    {file = "granian-1.3.1-cp311-cp311-macosx_10_12_x86_64.whl", hash = "sha256:f682b40f39286423f1ae5426ad3cbafe0b36e6521bb360cc0882385b4f11cd28"},
+    {file = "granian-1.3.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:310581f719ea7c43a9bab1c71ab9c62b09b3b91bd254fed0af8b707531d27a8f"},
+    {file = "granian-1.3.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:26bc8e9d2d13d251f442b2241cc73d53025a5a4b17a563e957286562df0bafca"},
+    {file = "granian-1.3.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75f472b93a0ed0e4a1675de465eedf96f67b9585e3ae03272bc250734ff7c5e0"},
+    {file = "granian-1.3.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:422077b6f95a0c4cc6be139c38230595de1ee3e64f5cd4a5b366ac9e94a70e1b"},
+    {file = "granian-1.3.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:a2767b4c4a2c0fdb1f5c4f1b843901063afc65d8c2be118f063b08eb28b8ac36"},
+    {file = "granian-1.3.1-cp311-none-win_amd64.whl", hash = "sha256:2c606bfdeab0709aadfff7b705c3e25fb94434dc5acc26b12531aec3baef9558"},
+    {file = "granian-1.3.1-cp312-cp312-macosx_10_12_x86_64.whl", hash = "sha256:e9f60164ba0588db3701ed4b2348893c118257e4374da1747813fb4c33870d68"},
+    {file = "granian-1.3.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:2993c8b9e3fe8e82ad60e892d7bb7ae77670038e06cff9e89f770c858937e697"},
+    {file = "granian-1.3.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7245c041a0bca32e99457f398a9c8b8774609b56e548326aa906b465fae0ec6c"},
+    {file = "granian-1.3.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3118bbb0f47c0374b968787c780f5edcde2653fd8874dd3c753b5bd6b71f6cdf"},
+    {file = "granian-1.3.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:411eb1520496f03beca7d3ab28b6adb7738d6f0ac500f2f45dbd8ea24d9639b9"},
+    {file = "granian-1.3.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:65cd2cf834dd9fe393add340c4cf2237184684aac4e503b0b447fc691c704378"},
+    {file = "granian-1.3.1-cp312-none-win_amd64.whl", hash = "sha256:54517442e7622de643444bd43a13e4b2461771e3c38313c267a9ac0e476a9abb"},
+    {file = "granian-1.3.1-cp38-cp38-macosx_10_12_x86_64.whl", hash = "sha256:3350c71e4fd36f2eb30144cad20f5e21f40b6494e6ce17fa2b6c26d3099c661a"},
+    {file = "granian-1.3.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:d4b2015e5937435016b2c25f545ac476ffcde6aa2526fa8252a2cec5c5686353"},
+    {file = "granian-1.3.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2a1e07cabc89ba015fb717232181c14405852237ded401bb962728f07642e125"},
+    {file = "granian-1.3.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50501a23c128c2f491d4454b2185f089070f6ec147f4742531c2b8460136a3b9"},
+    {file = "granian-1.3.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:5244bb8e8d404cba127b0737ad89ad2a624df00995ed471e7584f3f1b957c0df"},
+    {file = "granian-1.3.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:f7cde47ec2eecca3773806c1f63a3a71392e46be26711e1b6d988924d4acf6bf"},
+    {file = "granian-1.3.1-cp38-none-win_amd64.whl", hash = "sha256:fd3d8106d96f85e50dc128d72b94a5234e6452e9976befb258af1278124fde4f"},
+    {file = "granian-1.3.1-cp39-cp39-macosx_10_12_x86_64.whl", hash = "sha256:3ededcc3cea77077f793903ca8263149afcbefb05a04e1e8fa68110f4059aabb"},
+    {file = "granian-1.3.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:b37605f3427605599a9ac1312825b386f1c41f1896f59bbbf0ce3055ac817354"},
+    {file = "granian-1.3.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c34cd9cc12401186a4d4e54c0fdae0471d670c3d3bc555e0912ac2c45917840e"},
+    {file = "granian-1.3.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c8a936228840b9915cd153fc9dc570055df81ee43f5eea6bc30e18e73e3c5fe4"},
+    {file = "granian-1.3.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:10affc0400b257efd2509d1ce15f3eaef14b0b45fcd821b036de483b9bcae38a"},
+    {file = "granian-1.3.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:6ae60fb4b5fd3f5489bab5f5c36b2a72b1195f5f990aac90cde5ec3de1588e5a"},
+    {file = "granian-1.3.1-cp39-none-win_amd64.whl", hash = "sha256:e3132f37da4e38b85fe5ae6360e6b48ce340cb98349af148433288a6bbdf1d3e"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-macosx_10_12_x86_64.whl", hash = "sha256:5d57123c49b72d282b94a8842ac274d161016f70b289b3c08e08f2f7d8283c6e"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-macosx_11_0_arm64.whl", hash = "sha256:1cbfeeb22d95bb6cfc797f996be60f21a643d603c6e4a0eb56ebb1a4015b5e25"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b332bf511130a68cc5b17f0b8927125be6769e8cdf46ebd297fdffc9fa5d66ff"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:57019cdfbb4e5b3b1903c6b08d308732ed5341b6c441916f934cb240103729f1"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:1406d803a5f3c9b11a6848fa1abdc5fc2f39f527675f61368c77cb843b8d3bfc"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:135a61579bf2fd20dc86ea6c754117ee661c884cf8bd8917f765b47e9e6773c8"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:1aebcc9dc3556917ba5d2995165370fd3e04d533c54c1ba2ca611c2d94d036e0"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:ad6a874d56e249020ed45e1a840cbf21a3d414fde89fbe0153035ab37a16dc37"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-macosx_11_0_arm64.whl", hash = "sha256:aa42e80b54af7fa32db57d4382115c0267830c3e17eac17811e9e613c763cf45"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2132f60309eea7bf9d6a847582853a067b0ca51c0fd4927d18e54a251a8707b5"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a9592d3eaf6d0f14abfc825eccd55b62b74abd4513da8fabbab1eebd2d013b71"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:c71b18d3a6f5980ab044861678cccce9e6fd6c5e401cc53b02f7605f2f31cb9d"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:09818af44ac163d8a2c2df068f4db2d3a6032d3d22a226a309fcaf4989e6798e"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:0145fa076a6ad993498e255c67b4fd647a03803a51ee30de856ba66659dd0b1e"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:1bc2879cc56fbdf7350481f40a213ceba13360a281b1748b0e2ed1edc3d7630d"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-macosx_11_0_arm64.whl", hash = "sha256:67bac881cbcc2bb56a1a0a4190c97c73314088f8ddfdd99b9379959e432dc9d3"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:48df73ae1840a223b85e93de870c7cc8314b918e8e5af4de9220a2510c6cc2f6"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:555a573754dd8b4c01a75a75d7dcbad016e8a726c06f8fc10b530a9ea58d0c50"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:9cb51fb2b37567a24f984dc6fcd2a3ba4a40c1af6b794e2f4a74206989eda11f"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:70676812437274aab6520e11f729e870da058c894406ac6048dfb631cd90523d"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:39a7720d5bc2867863c5a9844eff8cc4ccf2a3ce916390c8015a81c31f725703"},
+    {file = "granian-1.3.1.tar.gz", hash = "sha256:4b5381a5e6eb20e702c72b8c87becdea36bc8f3e322c5fe7bfca53982c537e51"},
+]
+
+[[package]]
+name = "granian"
+version = "1.3.1"
+extras = ["pname", "reload"]
+requires_python = ">=3.8"
+summary = "A Rust HTTP server for Python applications"
+groups = ["default"]
+dependencies = [
+    "granian==1.3.1",
+    "setproctitle~=1.3.3",
+    "watchfiles~=0.21",
+]
+files = [
+    {file = "granian-1.3.1-cp310-cp310-macosx_10_12_x86_64.whl", hash = "sha256:a6c459af46ff5b3d7d2fcef6d4cae7e1d962c05d9041349efeb49c6e03a3a4ad"},
+    {file = "granian-1.3.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:6eb338e9d78f14ce9fcee8afd39691d703d26f6a17f0a31e807e790f62818cc5"},
+    {file = "granian-1.3.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7885ffa80977b9ab96308b11311cf01387c880b0ee7b39c4051f18b34706389a"},
+    {file = "granian-1.3.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5df1fa92c4789d17183810929658cf2f7969b64e04d3777c843196d73a68ce6d"},
+    {file = "granian-1.3.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:396203f11ce8406710055194ff75a54bc17703f5139cdddc86f2e9cbb80ebba2"},
+    {file = "granian-1.3.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:b783057f22408b4515ddbfbd9fbd8508a9df29e7523c774c3bc3da14cc56c27e"},
+    {file = "granian-1.3.1-cp310-none-win_amd64.whl", hash = "sha256:6dd3b46a457935d01cc80e1294c22f00fd0d700c91df498030557bcd1a99c9b9"},
+    {file = "granian-1.3.1-cp311-cp311-macosx_10_12_x86_64.whl", hash = "sha256:f682b40f39286423f1ae5426ad3cbafe0b36e6521bb360cc0882385b4f11cd28"},
+    {file = "granian-1.3.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:310581f719ea7c43a9bab1c71ab9c62b09b3b91bd254fed0af8b707531d27a8f"},
+    {file = "granian-1.3.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:26bc8e9d2d13d251f442b2241cc73d53025a5a4b17a563e957286562df0bafca"},
+    {file = "granian-1.3.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75f472b93a0ed0e4a1675de465eedf96f67b9585e3ae03272bc250734ff7c5e0"},
+    {file = "granian-1.3.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:422077b6f95a0c4cc6be139c38230595de1ee3e64f5cd4a5b366ac9e94a70e1b"},
+    {file = "granian-1.3.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:a2767b4c4a2c0fdb1f5c4f1b843901063afc65d8c2be118f063b08eb28b8ac36"},
+    {file = "granian-1.3.1-cp311-none-win_amd64.whl", hash = "sha256:2c606bfdeab0709aadfff7b705c3e25fb94434dc5acc26b12531aec3baef9558"},
+    {file = "granian-1.3.1-cp312-cp312-macosx_10_12_x86_64.whl", hash = "sha256:e9f60164ba0588db3701ed4b2348893c118257e4374da1747813fb4c33870d68"},
+    {file = "granian-1.3.1-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:2993c8b9e3fe8e82ad60e892d7bb7ae77670038e06cff9e89f770c858937e697"},
+    {file = "granian-1.3.1-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7245c041a0bca32e99457f398a9c8b8774609b56e548326aa906b465fae0ec6c"},
+    {file = "granian-1.3.1-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3118bbb0f47c0374b968787c780f5edcde2653fd8874dd3c753b5bd6b71f6cdf"},
+    {file = "granian-1.3.1-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:411eb1520496f03beca7d3ab28b6adb7738d6f0ac500f2f45dbd8ea24d9639b9"},
+    {file = "granian-1.3.1-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:65cd2cf834dd9fe393add340c4cf2237184684aac4e503b0b447fc691c704378"},
+    {file = "granian-1.3.1-cp312-none-win_amd64.whl", hash = "sha256:54517442e7622de643444bd43a13e4b2461771e3c38313c267a9ac0e476a9abb"},
+    {file = "granian-1.3.1-cp38-cp38-macosx_10_12_x86_64.whl", hash = "sha256:3350c71e4fd36f2eb30144cad20f5e21f40b6494e6ce17fa2b6c26d3099c661a"},
+    {file = "granian-1.3.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:d4b2015e5937435016b2c25f545ac476ffcde6aa2526fa8252a2cec5c5686353"},
+    {file = "granian-1.3.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2a1e07cabc89ba015fb717232181c14405852237ded401bb962728f07642e125"},
+    {file = "granian-1.3.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50501a23c128c2f491d4454b2185f089070f6ec147f4742531c2b8460136a3b9"},
+    {file = "granian-1.3.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:5244bb8e8d404cba127b0737ad89ad2a624df00995ed471e7584f3f1b957c0df"},
+    {file = "granian-1.3.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:f7cde47ec2eecca3773806c1f63a3a71392e46be26711e1b6d988924d4acf6bf"},
+    {file = "granian-1.3.1-cp38-none-win_amd64.whl", hash = "sha256:fd3d8106d96f85e50dc128d72b94a5234e6452e9976befb258af1278124fde4f"},
+    {file = "granian-1.3.1-cp39-cp39-macosx_10_12_x86_64.whl", hash = "sha256:3ededcc3cea77077f793903ca8263149afcbefb05a04e1e8fa68110f4059aabb"},
+    {file = "granian-1.3.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:b37605f3427605599a9ac1312825b386f1c41f1896f59bbbf0ce3055ac817354"},
+    {file = "granian-1.3.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c34cd9cc12401186a4d4e54c0fdae0471d670c3d3bc555e0912ac2c45917840e"},
+    {file = "granian-1.3.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c8a936228840b9915cd153fc9dc570055df81ee43f5eea6bc30e18e73e3c5fe4"},
+    {file = "granian-1.3.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:10affc0400b257efd2509d1ce15f3eaef14b0b45fcd821b036de483b9bcae38a"},
+    {file = "granian-1.3.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:6ae60fb4b5fd3f5489bab5f5c36b2a72b1195f5f990aac90cde5ec3de1588e5a"},
+    {file = "granian-1.3.1-cp39-none-win_amd64.whl", hash = "sha256:e3132f37da4e38b85fe5ae6360e6b48ce340cb98349af148433288a6bbdf1d3e"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-macosx_10_12_x86_64.whl", hash = "sha256:5d57123c49b72d282b94a8842ac274d161016f70b289b3c08e08f2f7d8283c6e"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-macosx_11_0_arm64.whl", hash = "sha256:1cbfeeb22d95bb6cfc797f996be60f21a643d603c6e4a0eb56ebb1a4015b5e25"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b332bf511130a68cc5b17f0b8927125be6769e8cdf46ebd297fdffc9fa5d66ff"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:57019cdfbb4e5b3b1903c6b08d308732ed5341b6c441916f934cb240103729f1"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:1406d803a5f3c9b11a6848fa1abdc5fc2f39f527675f61368c77cb843b8d3bfc"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:135a61579bf2fd20dc86ea6c754117ee661c884cf8bd8917f765b47e9e6773c8"},
+    {file = "granian-1.3.1-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:1aebcc9dc3556917ba5d2995165370fd3e04d533c54c1ba2ca611c2d94d036e0"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:ad6a874d56e249020ed45e1a840cbf21a3d414fde89fbe0153035ab37a16dc37"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-macosx_11_0_arm64.whl", hash = "sha256:aa42e80b54af7fa32db57d4382115c0267830c3e17eac17811e9e613c763cf45"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2132f60309eea7bf9d6a847582853a067b0ca51c0fd4927d18e54a251a8707b5"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a9592d3eaf6d0f14abfc825eccd55b62b74abd4513da8fabbab1eebd2d013b71"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:c71b18d3a6f5980ab044861678cccce9e6fd6c5e401cc53b02f7605f2f31cb9d"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:09818af44ac163d8a2c2df068f4db2d3a6032d3d22a226a309fcaf4989e6798e"},
+    {file = "granian-1.3.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:0145fa076a6ad993498e255c67b4fd647a03803a51ee30de856ba66659dd0b1e"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:1bc2879cc56fbdf7350481f40a213ceba13360a281b1748b0e2ed1edc3d7630d"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-macosx_11_0_arm64.whl", hash = "sha256:67bac881cbcc2bb56a1a0a4190c97c73314088f8ddfdd99b9379959e432dc9d3"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:48df73ae1840a223b85e93de870c7cc8314b918e8e5af4de9220a2510c6cc2f6"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:555a573754dd8b4c01a75a75d7dcbad016e8a726c06f8fc10b530a9ea58d0c50"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:9cb51fb2b37567a24f984dc6fcd2a3ba4a40c1af6b794e2f4a74206989eda11f"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:70676812437274aab6520e11f729e870da058c894406ac6048dfb631cd90523d"},
+    {file = "granian-1.3.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:39a7720d5bc2867863c5a9844eff8cc4ccf2a3ce916390c8015a81c31f725703"},
+    {file = "granian-1.3.1.tar.gz", hash = "sha256:4b5381a5e6eb20e702c72b8c87becdea36bc8f3e322c5fe7bfca53982c537e51"},
 ]
 
 [[package]]
 name = "h11"
 version = "0.14.0"
 requires_python = ">=3.7"
 summary = "A pure-Python, bring-your-own-I/O implementation of HTTP/1.1"
@@ -595,25 +840,25 @@
 files = [
     {file = "html5lib-1.1-py2.py3-none-any.whl", hash = "sha256:0d78f8fde1c230e99fe37986a60526d7049ed4bf8a9fadbad5f00e22e58e041d"},
     {file = "html5lib-1.1.tar.gz", hash = "sha256:b2e5b40261e20f354d198eae92afc10d750afb487ed5e50f9c4eaf07c184146f"},
 ]
 
 [[package]]
 name = "httpcore"
-version = "1.0.4"
+version = "1.0.5"
 requires_python = ">=3.8"
 summary = "A minimal low-level HTTP client."
 groups = ["default"]
 dependencies = [
     "certifi",
     "h11<0.15,>=0.13",
 ]
 files = [
-    {file = "httpcore-1.0.4-py3-none-any.whl", hash = "sha256:ac418c1db41bade2ad53ae2f3834a3a0f5ae76b56cf5aa497d2d033384fc7d73"},
-    {file = "httpcore-1.0.4.tar.gz", hash = "sha256:cb2839ccfcba0d2d3c1131d3c3e26dfc327326fbe7a5dc0dbfe9f6c9151bb022"},
+    {file = "httpcore-1.0.5-py3-none-any.whl", hash = "sha256:421f18bac248b25d310f3cacd198d55b8e6125c107797b609ff9b7a6ba7991b5"},
+    {file = "httpcore-1.0.5.tar.gz", hash = "sha256:34a38e2f9291467ee3b44e89dd52615370e152954ba21721378a87b2960f7a61"},
 ]
 
 [[package]]
 name = "httpx"
 version = "0.27.0"
 requires_python = ">=3.8"
 summary = "The next generation HTTP client."
@@ -628,32 +873,32 @@
 files = [
     {file = "httpx-0.27.0-py3-none-any.whl", hash = "sha256:71d5465162c13681bff01ad59b2cc68dd838ea1f10e51574bac27103f00c91a5"},
     {file = "httpx-0.27.0.tar.gz", hash = "sha256:a0cb88a46f32dc874e04ee956e4c2764aba2aa228f650b06788ba6bda2962ab5"},
 ]
 
 [[package]]
 name = "identify"
-version = "2.5.35"
+version = "2.5.36"
 requires_python = ">=3.8"
 summary = "File identification library for Python"
 groups = ["linting"]
 files = [
-    {file = "identify-2.5.35-py2.py3-none-any.whl", hash = "sha256:c4de0081837b211594f8e877a6b4fad7ca32bbfc1a9307fdd61c28bfe923f13e"},
-    {file = "identify-2.5.35.tar.gz", hash = "sha256:10a7ca245cfcd756a554a7288159f72ff105ad233c7c4b9c6f0f4d108f5f6791"},
+    {file = "identify-2.5.36-py2.py3-none-any.whl", hash = "sha256:37d93f380f4de590500d9dba7db359d0d3da95ffe7f9de1753faa159e71e7dfa"},
+    {file = "identify-2.5.36.tar.gz", hash = "sha256:e5e00f54165f9047fbebeb4a560f9acfb8af4c88232be60a488e9b68d122745d"},
 ]
 
 [[package]]
 name = "idna"
-version = "3.6"
+version = "3.7"
 requires_python = ">=3.5"
 summary = "Internationalized Domain Names in Applications (IDNA)"
 groups = ["default", "dev", "docs"]
 files = [
-    {file = "idna-3.6-py3-none-any.whl", hash = "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"},
-    {file = "idna-3.6.tar.gz", hash = "sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca"},
+    {file = "idna-3.7-py3-none-any.whl", hash = "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"},
+    {file = "idna-3.7.tar.gz", hash = "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc"},
 ]
 
 [[package]]
 name = "imagesize"
 version = "1.4.1"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 summary = "Getting image size from png/jpeg/jpeg2000/gif file"
@@ -716,15 +961,15 @@
 files = [
     {file = "Jinja2-3.1.3-py3-none-any.whl", hash = "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa"},
     {file = "Jinja2-3.1.3.tar.gz", hash = "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"},
 ]
 
 [[package]]
 name = "litestar"
-version = "2.7.0"
+version = "2.8.2"
 requires_python = "<4.0,>=3.8"
 summary = "Litestar - A production-ready, highly performant, extensible ASGI API Framework"
 groups = ["default"]
 dependencies = [
     "anyio>=3",
     "click",
     "exceptiongroup; python_version < \"3.11\"",
@@ -736,16 +981,35 @@
     "polyfactory>=2.6.3",
     "pyyaml",
     "rich-click",
     "rich>=13.0.0",
     "typing-extensions",
 ]
 files = [
-    {file = "litestar-2.7.0-py3-none-any.whl", hash = "sha256:62eabe89c08a1a5b66063bf9d8ec7677368bf7d3593c0579fb3605dd61b486a3"},
-    {file = "litestar-2.7.0.tar.gz", hash = "sha256:30f703b513d8c8a7f82e3b5cd583b071147f7e60b929650eeeeb00ff0ff65582"},
+    {file = "litestar-2.8.2-py3-none-any.whl", hash = "sha256:c891baf8a17d66cfed5c40bef7b5bf4c02c2831babf5fca0af404f441610557a"},
+    {file = "litestar-2.8.2.tar.gz", hash = "sha256:18353cb7246ba2e7f8d4aac4fe2d8772b503c931cf5ee16efc759cbbc3a2344b"},
+]
+
+[[package]]
+name = "litestar-sphinx-theme"
+version = "0.3.1"
+requires_python = ">=3.8,<4.0"
+git = "https://github.com/litestar-org/litestar-sphinx-theme.git"
+ref = "v3"
+revision = "4799f935c3023afb222058cba8c849e8fa9ae3ba"
+summary = "A Sphinx theme for the Litestar organization"
+groups = ["docs"]
+dependencies = [
+    "blacken-docs>=1.16.0",
+    "shibuya>=2024.4.4",
+    "sphinx-autobuild>=2021.3.14",
+    "sphinx-copybutton>=0.5.2",
+    "sphinx-design<1.0.0,>=0.3.0",
+    "sphinx-togglebutton",
+    "sphinx-toolbox>=3.5.0",
 ]
 
 [[package]]
 name = "livereload"
 version = "2.6.3"
 summary = "Python LiveReload is an awesome tool for web developers"
 groups = ["docs"]
@@ -1037,59 +1301,59 @@
     {file = "multidict-6.0.5-cp39-cp39-win_amd64.whl", hash = "sha256:d6f6d4f185481c9669b9447bf9d9cf3b95a0e9df9d169bbc17e363b7d5487755"},
     {file = "multidict-6.0.5-py3-none-any.whl", hash = "sha256:0d63c74e3d7ab26de115c49bffc92cc77ed23395303d496eae515d4204a625e7"},
     {file = "multidict-6.0.5.tar.gz", hash = "sha256:f7e301075edaf50500f0b341543c41194d8df3ae5caf4702f2095f3ca73dd8da"},
 ]
 
 [[package]]
 name = "mypy"
-version = "1.9.0"
+version = "1.10.0"
 requires_python = ">=3.8"
 summary = "Optional static typing for Python"
 groups = ["linting"]
 dependencies = [
     "mypy-extensions>=1.0.0",
     "tomli>=1.1.0; python_version < \"3.11\"",
     "typing-extensions>=4.1.0",
 ]
 files = [
-    {file = "mypy-1.9.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f"},
-    {file = "mypy-1.9.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed"},
-    {file = "mypy-1.9.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150"},
-    {file = "mypy-1.9.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374"},
-    {file = "mypy-1.9.0-cp310-cp310-win_amd64.whl", hash = "sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03"},
-    {file = "mypy-1.9.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3"},
-    {file = "mypy-1.9.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc"},
-    {file = "mypy-1.9.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129"},
-    {file = "mypy-1.9.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612"},
-    {file = "mypy-1.9.0-cp311-cp311-win_amd64.whl", hash = "sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3"},
-    {file = "mypy-1.9.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd"},
-    {file = "mypy-1.9.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6"},
-    {file = "mypy-1.9.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185"},
-    {file = "mypy-1.9.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913"},
-    {file = "mypy-1.9.0-cp312-cp312-win_amd64.whl", hash = "sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6"},
-    {file = "mypy-1.9.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b"},
-    {file = "mypy-1.9.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2"},
-    {file = "mypy-1.9.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e"},
-    {file = "mypy-1.9.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04"},
-    {file = "mypy-1.9.0-cp38-cp38-win_amd64.whl", hash = "sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89"},
-    {file = "mypy-1.9.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02"},
-    {file = "mypy-1.9.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4"},
-    {file = "mypy-1.9.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d"},
-    {file = "mypy-1.9.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf"},
-    {file = "mypy-1.9.0-cp39-cp39-win_amd64.whl", hash = "sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9"},
-    {file = "mypy-1.9.0-py3-none-any.whl", hash = "sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e"},
-    {file = "mypy-1.9.0.tar.gz", hash = "sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974"},
+    {file = "mypy-1.10.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2"},
+    {file = "mypy-1.10.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:12b6bfc1b1a66095ab413160a6e520e1dc076a28f3e22f7fb25ba3b000b4ef99"},
+    {file = "mypy-1.10.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9e36fb078cce9904c7989b9693e41cb9711e0600139ce3970c6ef814b6ebc2b2"},
+    {file = "mypy-1.10.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:2b0695d605ddcd3eb2f736cd8b4e388288c21e7de85001e9f85df9187f2b50f9"},
+    {file = "mypy-1.10.0-cp310-cp310-win_amd64.whl", hash = "sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051"},
+    {file = "mypy-1.10.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3be66771aa5c97602f382230165b856c231d1277c511c9a8dd058be4784472e1"},
+    {file = "mypy-1.10.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:8b2cbaca148d0754a54d44121b5825ae71868c7592a53b7292eeb0f3fdae95ee"},
+    {file = "mypy-1.10.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1ec404a7cbe9fc0e92cb0e67f55ce0c025014e26d33e54d9e506a0f2d07fe5de"},
+    {file = "mypy-1.10.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7"},
+    {file = "mypy-1.10.0-cp311-cp311-win_amd64.whl", hash = "sha256:a87dbfa85971e8d59c9cc1fcf534efe664d8949e4c0b6b44e8ca548e746a8d53"},
+    {file = "mypy-1.10.0-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:a781f6ad4bab20eef8b65174a57e5203f4be627b46291f4589879bf4e257b97b"},
+    {file = "mypy-1.10.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:b808e12113505b97d9023b0b5e0c0705a90571c6feefc6f215c1df9381256e30"},
+    {file = "mypy-1.10.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f55583b12156c399dce2df7d16f8a5095291354f1e839c252ec6c0611e86e2e"},
+    {file = "mypy-1.10.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:4cf18f9d0efa1b16478c4c129eabec36148032575391095f73cae2e722fcf9d5"},
+    {file = "mypy-1.10.0-cp312-cp312-win_amd64.whl", hash = "sha256:bc6ac273b23c6b82da3bb25f4136c4fd42665f17f2cd850771cb600bdd2ebeda"},
+    {file = "mypy-1.10.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:9fd50226364cd2737351c79807775136b0abe084433b55b2e29181a4c3c878c0"},
+    {file = "mypy-1.10.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f90cff89eea89273727d8783fef5d4a934be2fdca11b47def50cf5d311aff727"},
+    {file = "mypy-1.10.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fcfc70599efde5c67862a07a1aaf50e55bce629ace26bb19dc17cece5dd31ca4"},
+    {file = "mypy-1.10.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:075cbf81f3e134eadaf247de187bd604748171d6b79736fa9b6c9685b4083061"},
+    {file = "mypy-1.10.0-cp38-cp38-win_amd64.whl", hash = "sha256:3f298531bca95ff615b6e9f2fc0333aae27fa48052903a0ac90215021cdcfa4f"},
+    {file = "mypy-1.10.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:fa7ef5244615a2523b56c034becde4e9e3f9b034854c93639adb667ec9ec2976"},
+    {file = "mypy-1.10.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:3236a4c8f535a0631f85f5fcdffba71c7feeef76a6002fcba7c1a8e57c8be1ec"},
+    {file = "mypy-1.10.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4a2b5cdbb5dd35aa08ea9114436e0d79aceb2f38e32c21684dcf8e24e1e92821"},
+    {file = "mypy-1.10.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:92f93b21c0fe73dc00abf91022234c79d793318b8a96faac147cd579c1671746"},
+    {file = "mypy-1.10.0-cp39-cp39-win_amd64.whl", hash = "sha256:28d0e038361b45f099cc086d9dd99c15ff14d0188f44ac883010e172ce86c38a"},
+    {file = "mypy-1.10.0-py3-none-any.whl", hash = "sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee"},
+    {file = "mypy-1.10.0.tar.gz", hash = "sha256:3d087fcbec056c4ee34974da493a826ce316947485cef3901f511848e687c131"},
 ]
 
 [[package]]
 name = "mypy-extensions"
 version = "1.0.0"
 requires_python = ">=3.5"
 summary = "Type system extensions for programs checked with the mypy type checker."
-groups = ["linting"]
+groups = ["docs", "linting"]
 files = [
     {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "natsort"
@@ -1124,33 +1388,44 @@
 groups = ["docs", "test"]
 files = [
     {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
     {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
 ]
 
 [[package]]
+name = "pathspec"
+version = "0.12.1"
+requires_python = ">=3.8"
+summary = "Utility library for gitignore style pattern matching of file paths."
+groups = ["docs"]
+files = [
+    {file = "pathspec-0.12.1-py3-none-any.whl", hash = "sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08"},
+    {file = "pathspec-0.12.1.tar.gz", hash = "sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712"},
+]
+
+[[package]]
 name = "platformdirs"
-version = "4.2.0"
+version = "4.2.1"
 requires_python = ">=3.8"
-summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
+summary = "A small Python package for determining appropriate platform-specific dirs, e.g. a `user data dir`."
 groups = ["docs", "linting"]
 files = [
-    {file = "platformdirs-4.2.0-py3-none-any.whl", hash = "sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068"},
-    {file = "platformdirs-4.2.0.tar.gz", hash = "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"},
+    {file = "platformdirs-4.2.1-py3-none-any.whl", hash = "sha256:17d5a1161b3fd67b390023cb2d3b026bbd40abde6fdb052dfbd3a29c3ba22ee1"},
+    {file = "platformdirs-4.2.1.tar.gz", hash = "sha256:031cd18d4ec63ec53e82dceaac0417d218a6863f7745dfcc9efe7793b7039bdf"},
 ]
 
 [[package]]
 name = "pluggy"
-version = "1.4.0"
+version = "1.5.0"
 requires_python = ">=3.8"
 summary = "plugin and hook calling mechanisms for python"
 groups = ["test"]
 files = [
-    {file = "pluggy-1.4.0-py3-none-any.whl", hash = "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981"},
-    {file = "pluggy-1.4.0.tar.gz", hash = "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"},
+    {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
+    {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
 ]
 
 [[package]]
 name = "polyfactory"
 version = "2.15.0"
 requires_python = "<4.0,>=3.8"
 summary = "Mock data generation factories"
@@ -1180,40 +1455,40 @@
 files = [
     {file = "pre_commit-3.5.0-py2.py3-none-any.whl", hash = "sha256:841dc9aef25daba9a0238cd27984041fa0467b4199fc4852e27950664919f660"},
     {file = "pre_commit-3.5.0.tar.gz", hash = "sha256:5804465c675b659b0862f07907f96295d490822a450c4c40e747d0b1c6ebcb32"},
 ]
 
 [[package]]
 name = "pygments"
-version = "2.17.2"
-requires_python = ">=3.7"
+version = "2.18.0"
+requires_python = ">=3.8"
 summary = "Pygments is a syntax highlighting package written in Python."
 groups = ["default", "docs"]
 files = [
-    {file = "pygments-2.17.2-py3-none-any.whl", hash = "sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c"},
-    {file = "pygments-2.17.2.tar.gz", hash = "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"},
+    {file = "pygments-2.18.0-py3-none-any.whl", hash = "sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a"},
+    {file = "pygments-2.18.0.tar.gz", hash = "sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199"},
 ]
 
 [[package]]
 name = "pytest"
-version = "8.1.1"
+version = "8.2.0"
 requires_python = ">=3.8"
 summary = "pytest: simple powerful testing with Python"
 groups = ["test"]
 dependencies = [
     "colorama; sys_platform == \"win32\"",
     "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
     "iniconfig",
     "packaging",
-    "pluggy<2.0,>=1.4",
+    "pluggy<2.0,>=1.5",
     "tomli>=1; python_version < \"3.11\"",
 ]
 files = [
-    {file = "pytest-8.1.1-py3-none-any.whl", hash = "sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7"},
-    {file = "pytest-8.1.1.tar.gz", hash = "sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044"},
+    {file = "pytest-8.2.0-py3-none-any.whl", hash = "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233"},
+    {file = "pytest-8.2.0.tar.gz", hash = "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"},
 ]
 
 [[package]]
 name = "pytest-cov"
 version = "5.0.0"
 requires_python = ">=3.8"
 summary = "Pytest plugin for measuring coverage."
@@ -1238,14 +1513,29 @@
 ]
 files = [
     {file = "pytest-mock-3.14.0.tar.gz", hash = "sha256:2719255a1efeceadbc056d6bf3df3d1c5015530fb40cf347c0f9afac88410bd0"},
     {file = "pytest_mock-3.14.0-py3-none-any.whl", hash = "sha256:0b72c38033392a5f4621342fe11e9219ac11ec9d375f8e2a0c164539e0d70f6f"},
 ]
 
 [[package]]
+name = "pytest-sugar"
+version = "1.0.0"
+summary = "pytest-sugar is a plugin for pytest that changes the default look and feel of pytest (e.g. progressbar, show tests that fail instantly)."
+groups = ["test"]
+dependencies = [
+    "packaging>=21.3",
+    "pytest>=6.2.0",
+    "termcolor>=2.1.0",
+]
+files = [
+    {file = "pytest-sugar-1.0.0.tar.gz", hash = "sha256:6422e83258f5b0c04ce7c632176c7732cab5fdb909cb39cca5c9139f81276c0a"},
+    {file = "pytest_sugar-1.0.0-py3-none-any.whl", hash = "sha256:70ebcd8fc5795dc457ff8b69d266a4e2e8a74ae0c3edc749381c64b5246c8dfd"},
+]
+
+[[package]]
 name = "python-dateutil"
 version = "2.9.0.post0"
 requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,>=2.7"
 summary = "Extensions to the standard Python datetime module"
 groups = ["default"]
 dependencies = [
     "six>=1.5",
@@ -1345,26 +1635,26 @@
 files = [
     {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
     {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
 ]
 
 [[package]]
 name = "rich-click"
-version = "1.7.4"
+version = "1.8.0"
 requires_python = ">=3.7"
 summary = "Format click help output nicely with rich"
 groups = ["default"]
 dependencies = [
     "click>=7",
-    "rich>=10.7.0",
+    "rich>=10.7",
     "typing-extensions",
 ]
 files = [
-    {file = "rich-click-1.7.4.tar.gz", hash = "sha256:7ce5de8e4dc0333aec946113529b3eeb349f2e5d2fafee96b9edf8ee36a01395"},
-    {file = "rich_click-1.7.4-py3-none-any.whl", hash = "sha256:e363655475c60fec5a3e16a1eb618118ed79e666c365a36006b107c17c93ac4e"},
+    {file = "rich_click-1.8.0-py3-none-any.whl", hash = "sha256:846f504eb83a948d864888b2d73c71e52c310490c2babceac57e388aead086e2"},
+    {file = "rich_click-1.8.0.tar.gz", hash = "sha256:f8cad0d67d286d6cd6fc9f69f2d6f25c6c4c2d99fb9d6cb3b8987b593dbe6fa8"},
 ]
 
 [[package]]
 name = "ruamel-yaml"
 version = "0.18.6"
 requires_python = ">=3.7"
 summary = "ruamel.yaml is a YAML parser/emitter that supports roundtrip preservation of comments, seq/map flow style, and map key order"
@@ -1426,61 +1716,147 @@
     {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-win32.whl", hash = "sha256:84b554931e932c46f94ab306913ad7e11bba988104c5cff26d90d03f68258cd5"},
     {file = "ruamel.yaml.clib-0.2.8-cp39-cp39-win_amd64.whl", hash = "sha256:25ac8c08322002b06fa1d49d1646181f0b2c72f5cbc15a85e80b4c30a544bb15"},
     {file = "ruamel.yaml.clib-0.2.8.tar.gz", hash = "sha256:beb2e0404003de9a4cab9753a8805a8fe9320ee6673136ed7f04255fe60bb512"},
 ]
 
 [[package]]
 name = "ruff"
-version = "0.3.4"
+version = "0.4.3"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter and code formatter, written in Rust."
-groups = ["linting"]
+groups = ["docs", "linting"]
 files = [
-    {file = "ruff-0.3.4-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:60c870a7d46efcbc8385d27ec07fe534ac32f3b251e4fc44b3cbfd9e09609ef4"},
-    {file = "ruff-0.3.4-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:6fc14fa742e1d8f24910e1fff0bd5e26d395b0e0e04cc1b15c7c5e5fe5b4af91"},
-    {file = "ruff-0.3.4-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d3ee7880f653cc03749a3bfea720cf2a192e4f884925b0cf7eecce82f0ce5854"},
-    {file = "ruff-0.3.4-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:cf133dd744f2470b347f602452a88e70dadfbe0fcfb5fd46e093d55da65f82f7"},
-    {file = "ruff-0.3.4-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3f3860057590e810c7ffea75669bdc6927bfd91e29b4baa9258fd48b540a4365"},
-    {file = "ruff-0.3.4-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:986f2377f7cf12efac1f515fc1a5b753c000ed1e0a6de96747cdf2da20a1b369"},
-    {file = "ruff-0.3.4-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:c4fd98e85869603e65f554fdc5cddf0712e352fe6e61d29d5a6fe087ec82b76c"},
-    {file = "ruff-0.3.4-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:64abeed785dad51801b423fa51840b1764b35d6c461ea8caef9cf9e5e5ab34d9"},
-    {file = "ruff-0.3.4-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:df52972138318bc7546d92348a1ee58449bc3f9eaf0db278906eb511889c4b50"},
-    {file = "ruff-0.3.4-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:98e98300056445ba2cc27d0b325fd044dc17fcc38e4e4d2c7711585bd0a958ed"},
-    {file = "ruff-0.3.4-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:519cf6a0ebed244dce1dc8aecd3dc99add7a2ee15bb68cf19588bb5bf58e0488"},
-    {file = "ruff-0.3.4-py3-none-musllinux_1_2_i686.whl", hash = "sha256:bb0acfb921030d00070539c038cd24bb1df73a2981e9f55942514af8b17be94e"},
-    {file = "ruff-0.3.4-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:cf187a7e7098233d0d0c71175375c5162f880126c4c716fa28a8ac418dcf3378"},
-    {file = "ruff-0.3.4-py3-none-win32.whl", hash = "sha256:af27ac187c0a331e8ef91d84bf1c3c6a5dea97e912a7560ac0cef25c526a4102"},
-    {file = "ruff-0.3.4-py3-none-win_amd64.whl", hash = "sha256:de0d5069b165e5a32b3c6ffbb81c350b1e3d3483347196ffdf86dc0ef9e37dd6"},
-    {file = "ruff-0.3.4-py3-none-win_arm64.whl", hash = "sha256:6810563cc08ad0096b57c717bd78aeac888a1bfd38654d9113cb3dc4d3f74232"},
-    {file = "ruff-0.3.4.tar.gz", hash = "sha256:f0f4484c6541a99862b693e13a151435a279b271cff20e37101116a21e2a1ad1"},
+    {file = "ruff-0.4.3-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:b70800c290f14ae6fcbb41bbe201cf62dfca024d124a1f373e76371a007454ce"},
+    {file = "ruff-0.4.3-py3-none-macosx_11_0_arm64.whl", hash = "sha256:08a0d6a22918ab2552ace96adeaca308833873a4d7d1d587bb1d37bae8728eb3"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:eba1f14df3c758dd7de5b55fbae7e1c8af238597961e5fb628f3de446c3c40c5"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:819fb06d535cc76dfddbfe8d3068ff602ddeb40e3eacbc90e0d1272bb8d97113"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0bfc9e955e6dc6359eb6f82ea150c4f4e82b660e5b58d9a20a0e42ec3bb6342b"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:510a67d232d2ebe983fddea324dbf9d69b71c4d2dfeb8a862f4a127536dd4cfb"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:dc9ff11cd9a092ee7680a56d21f302bdda14327772cd870d806610a3503d001f"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:29efff25bf9ee685c2c8390563a5b5c006a3fee5230d28ea39f4f75f9d0b6f2f"},
+    {file = "ruff-0.4.3-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:18b00e0bcccf0fc8d7186ed21e311dffd19761cb632241a6e4fe4477cc80ef6e"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:262f5635e2c74d80b7507fbc2fac28fe0d4fef26373bbc62039526f7722bca1b"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:7363691198719c26459e08cc17c6a3dac6f592e9ea3d2fa772f4e561b5fe82a3"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_i686.whl", hash = "sha256:eeb039f8428fcb6725bb63cbae92ad67b0559e68b5d80f840f11914afd8ddf7f"},
+    {file = "ruff-0.4.3-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:927b11c1e4d0727ce1a729eace61cee88a334623ec424c0b1c8fe3e5f9d3c865"},
+    {file = "ruff-0.4.3-py3-none-win32.whl", hash = "sha256:25cacda2155778beb0d064e0ec5a3944dcca9c12715f7c4634fd9d93ac33fd30"},
+    {file = "ruff-0.4.3-py3-none-win_amd64.whl", hash = "sha256:7a1c3a450bc6539ef00da6c819fb1b76b6b065dec585f91456e7c0d6a0bbc725"},
+    {file = "ruff-0.4.3-py3-none-win_arm64.whl", hash = "sha256:71ca5f8ccf1121b95a59649482470c5601c60a416bf189d553955b0338e34614"},
+    {file = "ruff-0.4.3.tar.gz", hash = "sha256:ff0a3ef2e3c4b6d133fbedcf9586abfbe38d076041f2dc18ffb2c7e0485d5a07"},
+]
+
+[[package]]
+name = "setproctitle"
+version = "1.3.3"
+requires_python = ">=3.7"
+summary = "A Python module to customize the process title"
+groups = ["default"]
+files = [
+    {file = "setproctitle-1.3.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:897a73208da48db41e687225f355ce993167079eda1260ba5e13c4e53be7f754"},
+    {file = "setproctitle-1.3.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:8c331e91a14ba4076f88c29c777ad6b58639530ed5b24b5564b5ed2fd7a95452"},
+    {file = "setproctitle-1.3.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:bbbd6c7de0771c84b4aa30e70b409565eb1fc13627a723ca6be774ed6b9d9fa3"},
+    {file = "setproctitle-1.3.3-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:c05ac48ef16ee013b8a326c63e4610e2430dbec037ec5c5b58fcced550382b74"},
+    {file = "setproctitle-1.3.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1342f4fdb37f89d3e3c1c0a59d6ddbedbde838fff5c51178a7982993d238fe4f"},
+    {file = "setproctitle-1.3.3-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:fc74e84fdfa96821580fb5e9c0b0777c1c4779434ce16d3d62a9c4d8c710df39"},
+    {file = "setproctitle-1.3.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:9617b676b95adb412bb69645d5b077d664b6882bb0d37bfdafbbb1b999568d85"},
+    {file = "setproctitle-1.3.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:6a249415f5bb88b5e9e8c4db47f609e0bf0e20a75e8d744ea787f3092ba1f2d0"},
+    {file = "setproctitle-1.3.3-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:38da436a0aaace9add67b999eb6abe4b84397edf4a78ec28f264e5b4c9d53cd5"},
+    {file = "setproctitle-1.3.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:da0d57edd4c95bf221b2ebbaa061e65b1788f1544977288bdf95831b6e44e44d"},
+    {file = "setproctitle-1.3.3-cp310-cp310-win32.whl", hash = "sha256:a1fcac43918b836ace25f69b1dca8c9395253ad8152b625064415b1d2f9be4fb"},
+    {file = "setproctitle-1.3.3-cp310-cp310-win_amd64.whl", hash = "sha256:200620c3b15388d7f3f97e0ae26599c0c378fdf07ae9ac5a13616e933cbd2086"},
+    {file = "setproctitle-1.3.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:334f7ed39895d692f753a443102dd5fed180c571eb6a48b2a5b7f5b3564908c8"},
+    {file = "setproctitle-1.3.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:950f6476d56ff7817a8fed4ab207727fc5260af83481b2a4b125f32844df513a"},
+    {file = "setproctitle-1.3.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:195c961f54a09eb2acabbfc90c413955cf16c6e2f8caa2adbf2237d1019c7dd8"},
+    {file = "setproctitle-1.3.3-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f05e66746bf9fe6a3397ec246fe481096664a9c97eb3fea6004735a4daf867fd"},
+    {file = "setproctitle-1.3.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b5901a31012a40ec913265b64e48c2a4059278d9f4e6be628441482dd13fb8b5"},
+    {file = "setproctitle-1.3.3-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:64286f8a995f2cd934082b398fc63fca7d5ffe31f0e27e75b3ca6b4efda4e353"},
+    {file = "setproctitle-1.3.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:184239903bbc6b813b1a8fc86394dc6ca7d20e2ebe6f69f716bec301e4b0199d"},
+    {file = "setproctitle-1.3.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:664698ae0013f986118064b6676d7dcd28fefd0d7d5a5ae9497cbc10cba48fa5"},
+    {file = "setproctitle-1.3.3-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:e5119a211c2e98ff18b9908ba62a3bd0e3fabb02a29277a7232a6fb4b2560aa0"},
+    {file = "setproctitle-1.3.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:417de6b2e214e837827067048f61841f5d7fc27926f2e43954567094051aff18"},
+    {file = "setproctitle-1.3.3-cp311-cp311-win32.whl", hash = "sha256:6a143b31d758296dc2f440175f6c8e0b5301ced3b0f477b84ca43cdcf7f2f476"},
+    {file = "setproctitle-1.3.3-cp311-cp311-win_amd64.whl", hash = "sha256:a680d62c399fa4b44899094027ec9a1bdaf6f31c650e44183b50d4c4d0ccc085"},
+    {file = "setproctitle-1.3.3-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:d4460795a8a7a391e3567b902ec5bdf6c60a47d791c3b1d27080fc203d11c9dc"},
+    {file = "setproctitle-1.3.3-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:bdfd7254745bb737ca1384dee57e6523651892f0ea2a7344490e9caefcc35e64"},
+    {file = "setproctitle-1.3.3-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:477d3da48e216d7fc04bddab67b0dcde633e19f484a146fd2a34bb0e9dbb4a1e"},
+    {file = "setproctitle-1.3.3-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ab2900d111e93aff5df9fddc64cf51ca4ef2c9f98702ce26524f1acc5a786ae7"},
+    {file = "setproctitle-1.3.3-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:088b9efc62d5aa5d6edf6cba1cf0c81f4488b5ce1c0342a8b67ae39d64001120"},
+    {file = "setproctitle-1.3.3-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a6d50252377db62d6a0bb82cc898089916457f2db2041e1d03ce7fadd4a07381"},
+    {file = "setproctitle-1.3.3-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:87e668f9561fd3a457ba189edfc9e37709261287b52293c115ae3487a24b92f6"},
+    {file = "setproctitle-1.3.3-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:287490eb90e7a0ddd22e74c89a92cc922389daa95babc833c08cf80c84c4df0a"},
+    {file = "setproctitle-1.3.3-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:4fe1c49486109f72d502f8be569972e27f385fe632bd8895f4730df3c87d5ac8"},
+    {file = "setproctitle-1.3.3-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:4a6ba2494a6449b1f477bd3e67935c2b7b0274f2f6dcd0f7c6aceae10c6c6ba3"},
+    {file = "setproctitle-1.3.3-cp312-cp312-win32.whl", hash = "sha256:2df2b67e4b1d7498632e18c56722851ba4db5d6a0c91aaf0fd395111e51cdcf4"},
+    {file = "setproctitle-1.3.3-cp312-cp312-win_amd64.whl", hash = "sha256:f38d48abc121263f3b62943f84cbaede05749047e428409c2c199664feb6abc7"},
+    {file = "setproctitle-1.3.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:ff814dea1e5c492a4980e3e7d094286077054e7ea116cbeda138819db194b2cd"},
+    {file = "setproctitle-1.3.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:accb66d7b3ccb00d5cd11d8c6e07055a4568a24c95cf86109894dcc0c134cc89"},
+    {file = "setproctitle-1.3.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:554eae5a5b28f02705b83a230e9d163d645c9a08914c0ad921df363a07cf39b1"},
+    {file = "setproctitle-1.3.3-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:a911b26264dbe9e8066c7531c0591cfab27b464459c74385b276fe487ca91c12"},
+    {file = "setproctitle-1.3.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2982efe7640c4835f7355fdb4da313ad37fb3b40f5c69069912f8048f77b28c8"},
+    {file = "setproctitle-1.3.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:df3f4274b80709d8bcab2f9a862973d453b308b97a0b423a501bcd93582852e3"},
+    {file = "setproctitle-1.3.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:af2c67ae4c795d1674a8d3ac1988676fa306bcfa1e23fddb5e0bd5f5635309ca"},
+    {file = "setproctitle-1.3.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:af4061f67fd7ec01624c5e3c21f6b7af2ef0e6bab7fbb43f209e6506c9ce0092"},
+    {file = "setproctitle-1.3.3-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:37a62cbe16d4c6294e84670b59cf7adcc73faafe6af07f8cb9adaf1f0e775b19"},
+    {file = "setproctitle-1.3.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:a83ca086fbb017f0d87f240a8f9bbcf0809f3b754ee01cec928fff926542c450"},
+    {file = "setproctitle-1.3.3-cp38-cp38-win32.whl", hash = "sha256:059f4ce86f8cc92e5860abfc43a1dceb21137b26a02373618d88f6b4b86ba9b2"},
+    {file = "setproctitle-1.3.3-cp38-cp38-win_amd64.whl", hash = "sha256:ab92e51cd4a218208efee4c6d37db7368fdf182f6e7ff148fb295ecddf264287"},
+    {file = "setproctitle-1.3.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:c7951820b77abe03d88b114b998867c0f99da03859e5ab2623d94690848d3e45"},
+    {file = "setproctitle-1.3.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:5bc94cf128676e8fac6503b37763adb378e2b6be1249d207630f83fc325d9b11"},
+    {file = "setproctitle-1.3.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1f5d9027eeda64d353cf21a3ceb74bb1760bd534526c9214e19f052424b37e42"},
+    {file = "setproctitle-1.3.3-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:2e4a8104db15d3462e29d9946f26bed817a5b1d7a47eabca2d9dc2b995991503"},
+    {file = "setproctitle-1.3.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c32c41ace41f344d317399efff4cffb133e709cec2ef09c99e7a13e9f3b9483c"},
+    {file = "setproctitle-1.3.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cbf16381c7bf7f963b58fb4daaa65684e10966ee14d26f5cc90f07049bfd8c1e"},
+    {file = "setproctitle-1.3.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:e18b7bd0898398cc97ce2dfc83bb192a13a087ef6b2d5a8a36460311cb09e775"},
+    {file = "setproctitle-1.3.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:69d565d20efe527bd8a9b92e7f299ae5e73b6c0470f3719bd66f3cd821e0d5bd"},
+    {file = "setproctitle-1.3.3-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:ddedd300cd690a3b06e7eac90ed4452348b1348635777ce23d460d913b5b63c3"},
+    {file = "setproctitle-1.3.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:415bfcfd01d1fbf5cbd75004599ef167a533395955305f42220a585f64036081"},
+    {file = "setproctitle-1.3.3-cp39-cp39-win32.whl", hash = "sha256:21112fcd2195d48f25760f0eafa7a76510871bbb3b750219310cf88b04456ae3"},
+    {file = "setproctitle-1.3.3-cp39-cp39-win_amd64.whl", hash = "sha256:5a740f05d0968a5a17da3d676ce6afefebeeeb5ce137510901bf6306ba8ee002"},
+    {file = "setproctitle-1.3.3-pp310-pypy310_pp73-macosx_10_9_x86_64.whl", hash = "sha256:6b9e62ddb3db4b5205c0321dd69a406d8af9ee1693529d144e86bd43bcb4b6c0"},
+    {file = "setproctitle-1.3.3-pp310-pypy310_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9e3b99b338598de0bd6b2643bf8c343cf5ff70db3627af3ca427a5e1a1a90dd9"},
+    {file = "setproctitle-1.3.3-pp310-pypy310_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:38ae9a02766dad331deb06855fb7a6ca15daea333b3967e214de12cfae8f0ef5"},
+    {file = "setproctitle-1.3.3-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:200ede6fd11233085ba9b764eb055a2a191fb4ffb950c68675ac53c874c22e20"},
+    {file = "setproctitle-1.3.3-pp37-pypy37_pp73-macosx_10_9_x86_64.whl", hash = "sha256:0d3a953c50776751e80fe755a380a64cb14d61e8762bd43041ab3f8cc436092f"},
+    {file = "setproctitle-1.3.3-pp37-pypy37_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e5e08e232b78ba3ac6bc0d23ce9e2bee8fad2be391b7e2da834fc9a45129eb87"},
+    {file = "setproctitle-1.3.3-pp37-pypy37_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f1da82c3e11284da4fcbf54957dafbf0655d2389cd3d54e4eaba636faf6d117a"},
+    {file = "setproctitle-1.3.3-pp37-pypy37_pp73-win_amd64.whl", hash = "sha256:aeaa71fb9568ebe9b911ddb490c644fbd2006e8c940f21cb9a1e9425bd709574"},
+    {file = "setproctitle-1.3.3-pp38-pypy38_pp73-macosx_10_9_x86_64.whl", hash = "sha256:59335d000c6250c35989394661eb6287187854e94ac79ea22315469ee4f4c244"},
+    {file = "setproctitle-1.3.3-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c3ba57029c9c50ecaf0c92bb127224cc2ea9fda057b5d99d3f348c9ec2855ad3"},
+    {file = "setproctitle-1.3.3-pp38-pypy38_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d876d355c53d975c2ef9c4f2487c8f83dad6aeaaee1b6571453cb0ee992f55f6"},
+    {file = "setproctitle-1.3.3-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:224602f0939e6fb9d5dd881be1229d485f3257b540f8a900d4271a2c2aa4e5f4"},
+    {file = "setproctitle-1.3.3-pp39-pypy39_pp73-macosx_10_9_x86_64.whl", hash = "sha256:d7f27e0268af2d7503386e0e6be87fb9b6657afd96f5726b733837121146750d"},
+    {file = "setproctitle-1.3.3-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f5e7266498cd31a4572378c61920af9f6b4676a73c299fce8ba93afd694f8ae7"},
+    {file = "setproctitle-1.3.3-pp39-pypy39_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:33c5609ad51cd99d388e55651b19148ea99727516132fb44680e1f28dd0d1de9"},
+    {file = "setproctitle-1.3.3-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:eae8988e78192fd1a3245a6f4f382390b61bce6cfcc93f3809726e4c885fa68d"},
+    {file = "setproctitle-1.3.3.tar.gz", hash = "sha256:c913e151e7ea01567837ff037a23ca8740192880198b7fbb90b16d181607caae"},
 ]
 
 [[package]]
 name = "setuptools"
-version = "69.2.0"
+version = "69.5.1"
 requires_python = ">=3.8"
 summary = "Easily download, build, install, upgrade, and uninstall Python packages"
-groups = ["linting"]
+groups = ["docs", "linting"]
 files = [
-    {file = "setuptools-69.2.0-py3-none-any.whl", hash = "sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c"},
-    {file = "setuptools-69.2.0.tar.gz", hash = "sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e"},
+    {file = "setuptools-69.5.1-py3-none-any.whl", hash = "sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32"},
+    {file = "setuptools-69.5.1.tar.gz", hash = "sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987"},
 ]
 
 [[package]]
 name = "shibuya"
-version = "2024.3.1"
+version = "2024.4.27"
 requires_python = ">=3.7"
 summary = "A clean, responsive, and customizable Sphinx documentation theme with light/dark mode."
 groups = ["docs"]
 dependencies = [
     "Sphinx",
 ]
 files = [
-    {file = "shibuya-2024.3.1-py3-none-any.whl", hash = "sha256:c70fa64120175ac782ba04ff5c45736e1fe10cc01afb74f9e305b3408af2498a"},
-    {file = "shibuya-2024.3.1.tar.gz", hash = "sha256:8dad19bb9f85a5c25270a5dea62aaf8ae97daf4fa546df476931847f1b1bbe4e"},
+    {file = "shibuya-2024.4.27-py3-none-any.whl", hash = "sha256:b0eaf3ae415eaefb898ca1ad07012c86f6ef12f43aaad73f0d8ef9a13d42bd5e"},
+    {file = "shibuya-2024.4.27.tar.gz", hash = "sha256:6c7c83d49ae3f1d56c0d4c4ccddd31f5dab4aed4e6caf8f397f4de5da5af1911"},
 ]
 
 [[package]]
 name = "six"
 version = "1.16.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 summary = "Python 2 and 3 compatibility utilities"
@@ -1577,24 +1953,24 @@
 files = [
     {file = "sphinx-autobuild-2021.3.14.tar.gz", hash = "sha256:de1ca3b66e271d2b5b5140c35034c89e47f263f2cd5db302c9217065f7443f05"},
     {file = "sphinx_autobuild-2021.3.14-py3-none-any.whl", hash = "sha256:8fe8cbfdb75db04475232f05187c776f46f6e9e04cacf1e49ce81bdac649ccac"},
 ]
 
 [[package]]
 name = "sphinx-autodoc-typehints"
-version = "2.0.0"
+version = "2.0.1"
 requires_python = ">=3.8"
 summary = "Type hints (PEP 484) support for the Sphinx autodoc extension"
 groups = ["docs"]
 dependencies = [
     "sphinx>=7.1.2",
 ]
 files = [
-    {file = "sphinx_autodoc_typehints-2.0.0-py3-none-any.whl", hash = "sha256:12c0e161f6fe191c2cdfd8fa3caea271f5387d9fbc67ebcd6f4f1f24ce880993"},
-    {file = "sphinx_autodoc_typehints-2.0.0.tar.gz", hash = "sha256:7f2cdac2e70fd9787926b6e9e541cd4ded1e838d2b46fda2a1bb0a75ec5b7f3a"},
+    {file = "sphinx_autodoc_typehints-2.0.1-py3-none-any.whl", hash = "sha256:f73ae89b43a799e587e39266672c1075b2ef783aeb382d3ebed77c38a3fc0149"},
+    {file = "sphinx_autodoc_typehints-2.0.1.tar.gz", hash = "sha256:60ed1e3b2c970acc0aa6e877be42d48029a9faec7378a17838716cacd8c10b12"},
 ]
 
 [[package]]
 name = "sphinx-click"
 version = "5.1.0"
 requires_python = ">=3.8"
 summary = "Sphinx extension that automatically documents click applications"
@@ -1649,14 +2025,27 @@
 ]
 files = [
     {file = "sphinx_jinja2_compat-0.2.0.post1-py3-none-any.whl", hash = "sha256:f9d329174bdde8db19dc12c62528367196eb2f6b46c91754eca604acd0c0f6ad"},
     {file = "sphinx_jinja2_compat-0.2.0.post1.tar.gz", hash = "sha256:974289a12a9f402108dead621e9c15f7004e945d5cfcaea8d6419e94d3fa95a3"},
 ]
 
 [[package]]
+name = "sphinx-paramlinks"
+version = "0.6.0"
+summary = "Allows param links in Sphinx function/method descriptions to be linkable"
+groups = ["docs"]
+dependencies = [
+    "Sphinx>=4.0.0",
+    "docutils",
+]
+files = [
+    {file = "sphinx-paramlinks-0.6.0.tar.gz", hash = "sha256:746a0816860aa3fff5d8d746efcbec4deead421f152687411db1d613d29f915e"},
+]
+
+[[package]]
 name = "sphinx-prompt"
 version = "1.5.0"
 summary = "Sphinx directive to add unselectable prompt"
 groups = ["docs"]
 dependencies = [
     "Sphinx",
     "pygments",
@@ -1678,14 +2067,30 @@
 ]
 files = [
     {file = "sphinx-tabs-3.4.5.tar.gz", hash = "sha256:ba9d0c1e3e37aaadd4b5678449eb08176770e0fc227e769b6ce747df3ceea531"},
     {file = "sphinx_tabs-3.4.5-py3-none-any.whl", hash = "sha256:92cc9473e2ecf1828ca3f6617d0efc0aa8acb06b08c56ba29d1413f2f0f6cf09"},
 ]
 
 [[package]]
+name = "sphinx-togglebutton"
+version = "0.3.2"
+summary = "Toggle page content and collapse admonitions in Sphinx."
+groups = ["docs"]
+dependencies = [
+    "docutils",
+    "setuptools",
+    "sphinx",
+    "wheel",
+]
+files = [
+    {file = "sphinx-togglebutton-0.3.2.tar.gz", hash = "sha256:ab0c8b366427b01e4c89802d5d078472c427fa6e9d12d521c34fa0442559dc7a"},
+    {file = "sphinx_togglebutton-0.3.2-py3-none-any.whl", hash = "sha256:9647ba7874b7d1e2d43413d8497153a85edc6ac95a3fea9a75ef9c1e08aaae2b"},
+]
+
+[[package]]
 name = "sphinx-toolbox"
 version = "3.5.0"
 requires_python = ">=3.7"
 summary = "Box of handy tools for Sphinx 🧰 📔"
 groups = ["docs"]
 dependencies = [
     "apeye>=0.4.0",
@@ -1785,19 +2190,30 @@
 groups = ["docs"]
 files = [
     {file = "tabulate-0.9.0-py3-none-any.whl", hash = "sha256:024ca478df22e9340661486f85298cff5f6dcdba14f3813e8830015b9ed1948f"},
     {file = "tabulate-0.9.0.tar.gz", hash = "sha256:0095b12bf5966de529c0feb1fa08671671b3368eec77d7ef7ab114be2c068b3c"},
 ]
 
 [[package]]
+name = "termcolor"
+version = "2.4.0"
+requires_python = ">=3.8"
+summary = "ANSI color formatting for output in terminal"
+groups = ["test"]
+files = [
+    {file = "termcolor-2.4.0-py3-none-any.whl", hash = "sha256:9297c0df9c99445c2412e832e882a7884038a25617c60cea2ad69488d4040d63"},
+    {file = "termcolor-2.4.0.tar.gz", hash = "sha256:aab9e56047c8ac41ed798fa36d892a37aca6b3e9159f3e0c24bc64a9b3ac7b7a"},
+]
+
+[[package]]
 name = "tomli"
 version = "2.0.1"
 requires_python = ">=3.7"
 summary = "A lil' TOML parser"
-groups = ["linting", "test"]
+groups = ["docs", "linting", "test"]
 marker = "python_version < \"3.11\""
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
@@ -1818,48 +2234,32 @@
     {file = "tornado-6.4-cp38-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:71ddfc23a0e03ef2df1c1397d859868d158c8276a0603b96cf86892bff58149f"},
     {file = "tornado-6.4-cp38-abi3-win32.whl", hash = "sha256:6f8a6c77900f5ae93d8b4ae1196472d0ccc2775cc1dfdc9e7727889145c45052"},
     {file = "tornado-6.4-cp38-abi3-win_amd64.whl", hash = "sha256:10aeaa8006333433da48dec9fe417877f8bcc21f48dda8d661ae79da357b2a63"},
     {file = "tornado-6.4.tar.gz", hash = "sha256:72291fa6e6bc84e626589f1c29d90a5a6d593ef5ae68052ee2ef000dfd273dee"},
 ]
 
 [[package]]
-name = "typer"
-version = "0.10.0"
-requires_python = ">=3.6"
-summary = "Typer, build great CLIs. Easy to code. Based on Python type hints."
-groups = ["default"]
-dependencies = [
-    "click<9.0.0,>=7.1.1",
-    "typing-extensions>=3.7.4.3",
-]
-files = [
-    {file = "typer-0.10.0-py3-none-any.whl", hash = "sha256:b8a587aa06d3c5422c09c2e9935eb80b4c9de8605fd5ab702b2f92d72246ca48"},
-    {file = "typer-0.10.0.tar.gz", hash = "sha256:597f974754520b091665f993f88abdd088bb81c56b3042225434ced0b50a788b"},
-]
-
-[[package]]
-name = "types-docutils"
-version = "0.20.0.20240317"
-requires_python = ">=3.8"
-summary = "Typing stubs for docutils"
-groups = ["docs"]
+name = "types-click"
+version = "7.1.8"
+summary = "Typing stubs for click"
+groups = ["linting"]
 files = [
-    {file = "types-docutils-0.20.0.20240317.tar.gz", hash = "sha256:23657aab0de58634d111914b677b1855867f16cd9a9ea110254e23b48653e1a8"},
-    {file = "types_docutils-0.20.0.20240317-py3-none-any.whl", hash = "sha256:4f11b3986b74f39169313ab528ffac101c45fca9c36c4cd22dbeec6143c99b7f"},
+    {file = "types-click-7.1.8.tar.gz", hash = "sha256:b6604968be6401dc516311ca50708a0a28baa7a0cb840efd7412f0dbbff4e092"},
+    {file = "types_click-7.1.8-py3-none-any.whl", hash = "sha256:8cb030a669e2e927461be9827375f83c16b8178c365852c060a34e24871e7e81"},
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.10.0"
+version = "4.11.0"
 requires_python = ">=3.8"
 summary = "Backported and Experimental Type Hints for Python 3.8+"
 groups = ["default", "dev", "docs", "linting"]
 files = [
-    {file = "typing_extensions-4.10.0-py3-none-any.whl", hash = "sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475"},
-    {file = "typing_extensions-4.10.0.tar.gz", hash = "sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb"},
+    {file = "typing_extensions-4.11.0-py3-none-any.whl", hash = "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"},
+    {file = "typing_extensions-4.11.0.tar.gz", hash = "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0"},
 ]
 
 [[package]]
 name = "urllib3"
 version = "2.2.1"
 requires_python = ">=3.8"
 summary = "HTTP library with thread-safe connection pooling, file post, and more."
@@ -1908,39 +2308,137 @@
     {file = "uvloop-0.18.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:4d90858f32a852988d33987d608bcfba92a1874eb9f183995def59a34229f30d"},
     {file = "uvloop-0.18.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:db1fcbad5deb9551e011ca589c5e7258b5afa78598174ac37a5f15ddcfb4ac7b"},
     {file = "uvloop-0.18.0.tar.gz", hash = "sha256:d5d1135beffe9cd95d0350f19e2716bc38be47d5df296d7cc46e3b7557c0d1ff"},
 ]
 
 [[package]]
 name = "virtualenv"
-version = "20.25.1"
+version = "20.26.1"
 requires_python = ">=3.7"
 summary = "Virtual Python Environment builder"
 groups = ["linting"]
 dependencies = [
     "distlib<1,>=0.3.7",
     "filelock<4,>=3.12.2",
     "platformdirs<5,>=3.9.1",
 ]
 files = [
-    {file = "virtualenv-20.25.1-py3-none-any.whl", hash = "sha256:961c026ac520bac5f69acb8ea063e8a4f071bcc9457b9c1f28f6b085c511583a"},
-    {file = "virtualenv-20.25.1.tar.gz", hash = "sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197"},
+    {file = "virtualenv-20.26.1-py3-none-any.whl", hash = "sha256:7aa9982a728ae5892558bff6a2839c00b9ed145523ece2274fad6f414690ae75"},
+    {file = "virtualenv-20.26.1.tar.gz", hash = "sha256:604bfdceaeece392802e6ae48e69cec49168b9c5f4a44e483963f9242eb0e78b"},
+]
+
+[[package]]
+name = "watchfiles"
+version = "0.21.0"
+requires_python = ">=3.8"
+summary = "Simple, modern and high performance file watching and code reload in python."
+groups = ["default"]
+dependencies = [
+    "anyio>=3.0.0",
+]
+files = [
+    {file = "watchfiles-0.21.0-cp310-cp310-macosx_10_7_x86_64.whl", hash = "sha256:27b4035013f1ea49c6c0b42d983133b136637a527e48c132d368eb19bf1ac6aa"},
+    {file = "watchfiles-0.21.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c81818595eff6e92535ff32825f31c116f867f64ff8cdf6562cd1d6b2e1e8f3e"},
+    {file = "watchfiles-0.21.0-cp310-cp310-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:6c107ea3cf2bd07199d66f156e3ea756d1b84dfd43b542b2d870b77868c98c03"},
+    {file = "watchfiles-0.21.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0d9ac347653ebd95839a7c607608703b20bc07e577e870d824fa4801bc1cb124"},
+    {file = "watchfiles-0.21.0-cp310-cp310-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:5eb86c6acb498208e7663ca22dbe68ca2cf42ab5bf1c776670a50919a56e64ab"},
+    {file = "watchfiles-0.21.0-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f564bf68404144ea6b87a78a3f910cc8de216c6b12a4cf0b27718bf4ec38d303"},
+    {file = "watchfiles-0.21.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:3d0f32ebfaa9c6011f8454994f86108c2eb9c79b8b7de00b36d558cadcedaa3d"},
+    {file = "watchfiles-0.21.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b6d45d9b699ecbac6c7bd8e0a2609767491540403610962968d258fd6405c17c"},
+    {file = "watchfiles-0.21.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:aff06b2cac3ef4616e26ba17a9c250c1fe9dd8a5d907d0193f84c499b1b6e6a9"},
+    {file = "watchfiles-0.21.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d9792dff410f266051025ecfaa927078b94cc7478954b06796a9756ccc7e14a9"},
+    {file = "watchfiles-0.21.0-cp310-none-win32.whl", hash = "sha256:214cee7f9e09150d4fb42e24919a1e74d8c9b8a9306ed1474ecaddcd5479c293"},
+    {file = "watchfiles-0.21.0-cp310-none-win_amd64.whl", hash = "sha256:1ad7247d79f9f55bb25ab1778fd47f32d70cf36053941f07de0b7c4e96b5d235"},
+    {file = "watchfiles-0.21.0-cp311-cp311-macosx_10_7_x86_64.whl", hash = "sha256:668c265d90de8ae914f860d3eeb164534ba2e836811f91fecc7050416ee70aa7"},
+    {file = "watchfiles-0.21.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:3a23092a992e61c3a6a70f350a56db7197242f3490da9c87b500f389b2d01eef"},
+    {file = "watchfiles-0.21.0-cp311-cp311-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:e7941bbcfdded9c26b0bf720cb7e6fd803d95a55d2c14b4bd1f6a2772230c586"},
+    {file = "watchfiles-0.21.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:11cd0c3100e2233e9c53106265da31d574355c288e15259c0d40a4405cbae317"},
+    {file = "watchfiles-0.21.0-cp311-cp311-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:d78f30cbe8b2ce770160d3c08cff01b2ae9306fe66ce899b73f0409dc1846c1b"},
+    {file = "watchfiles-0.21.0-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:6674b00b9756b0af620aa2a3346b01f8e2a3dc729d25617e1b89cf6af4a54eb1"},
+    {file = "watchfiles-0.21.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:fd7ac678b92b29ba630d8c842d8ad6c555abda1b9ef044d6cc092dacbfc9719d"},
+    {file = "watchfiles-0.21.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9c873345680c1b87f1e09e0eaf8cf6c891b9851d8b4d3645e7efe2ec20a20cc7"},
+    {file = "watchfiles-0.21.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:49f56e6ecc2503e7dbe233fa328b2be1a7797d31548e7a193237dcdf1ad0eee0"},
+    {file = "watchfiles-0.21.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:02d91cbac553a3ad141db016e3350b03184deaafeba09b9d6439826ee594b365"},
+    {file = "watchfiles-0.21.0-cp311-none-win32.whl", hash = "sha256:ebe684d7d26239e23d102a2bad2a358dedf18e462e8808778703427d1f584400"},
+    {file = "watchfiles-0.21.0-cp311-none-win_amd64.whl", hash = "sha256:4566006aa44cb0d21b8ab53baf4b9c667a0ed23efe4aaad8c227bfba0bf15cbe"},
+    {file = "watchfiles-0.21.0-cp311-none-win_arm64.whl", hash = "sha256:c550a56bf209a3d987d5a975cdf2063b3389a5d16caf29db4bdddeae49f22078"},
+    {file = "watchfiles-0.21.0-cp312-cp312-macosx_10_7_x86_64.whl", hash = "sha256:51ddac60b96a42c15d24fbdc7a4bfcd02b5a29c047b7f8bf63d3f6f5a860949a"},
+    {file = "watchfiles-0.21.0-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:511f0b034120cd1989932bf1e9081aa9fb00f1f949fbd2d9cab6264916ae89b1"},
+    {file = "watchfiles-0.21.0-cp312-cp312-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:cfb92d49dbb95ec7a07511bc9efb0faff8fe24ef3805662b8d6808ba8409a71a"},
+    {file = "watchfiles-0.21.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3f92944efc564867bbf841c823c8b71bb0be75e06b8ce45c084b46411475a915"},
+    {file = "watchfiles-0.21.0-cp312-cp312-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:642d66b75eda909fd1112d35c53816d59789a4b38c141a96d62f50a3ef9b3360"},
+    {file = "watchfiles-0.21.0-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d23bcd6c8eaa6324fe109d8cac01b41fe9a54b8c498af9ce464c1aeeb99903d6"},
+    {file = "watchfiles-0.21.0-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:18d5b4da8cf3e41895b34e8c37d13c9ed294954907929aacd95153508d5d89d7"},
+    {file = "watchfiles-0.21.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1b8d1eae0f65441963d805f766c7e9cd092f91e0c600c820c764a4ff71a0764c"},
+    {file = "watchfiles-0.21.0-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:1fd9a5205139f3c6bb60d11f6072e0552f0a20b712c85f43d42342d162be1235"},
+    {file = "watchfiles-0.21.0-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:a1e3014a625bcf107fbf38eece0e47fa0190e52e45dc6eee5a8265ddc6dc5ea7"},
+    {file = "watchfiles-0.21.0-cp312-none-win32.whl", hash = "sha256:9d09869f2c5a6f2d9df50ce3064b3391d3ecb6dced708ad64467b9e4f2c9bef3"},
+    {file = "watchfiles-0.21.0-cp312-none-win_amd64.whl", hash = "sha256:18722b50783b5e30a18a8a5db3006bab146d2b705c92eb9a94f78c72beb94094"},
+    {file = "watchfiles-0.21.0-cp312-none-win_arm64.whl", hash = "sha256:a3b9bec9579a15fb3ca2d9878deae789df72f2b0fdaf90ad49ee389cad5edab6"},
+    {file = "watchfiles-0.21.0-cp38-cp38-macosx_10_7_x86_64.whl", hash = "sha256:4ea10a29aa5de67de02256a28d1bf53d21322295cb00bd2d57fcd19b850ebd99"},
+    {file = "watchfiles-0.21.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:40bca549fdc929b470dd1dbfcb47b3295cb46a6d2c90e50588b0a1b3bd98f429"},
+    {file = "watchfiles-0.21.0-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:9b37a7ba223b2f26122c148bb8d09a9ff312afca998c48c725ff5a0a632145f7"},
+    {file = "watchfiles-0.21.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ec8c8900dc5c83650a63dd48c4d1d245343f904c4b64b48798c67a3767d7e165"},
+    {file = "watchfiles-0.21.0-cp38-cp38-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:8ad3fe0a3567c2f0f629d800409cd528cb6251da12e81a1f765e5c5345fd0137"},
+    {file = "watchfiles-0.21.0-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:9d353c4cfda586db2a176ce42c88f2fc31ec25e50212650c89fdd0f560ee507b"},
+    {file = "watchfiles-0.21.0-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:83a696da8922314ff2aec02987eefb03784f473281d740bf9170181829133765"},
+    {file = "watchfiles-0.21.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5a03651352fc20975ee2a707cd2d74a386cd303cc688f407296064ad1e6d1562"},
+    {file = "watchfiles-0.21.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:3ad692bc7792be8c32918c699638b660c0de078a6cbe464c46e1340dadb94c19"},
+    {file = "watchfiles-0.21.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:06247538e8253975bdb328e7683f8515ff5ff041f43be6c40bff62d989b7d0b0"},
+    {file = "watchfiles-0.21.0-cp38-none-win32.whl", hash = "sha256:9a0aa47f94ea9a0b39dd30850b0adf2e1cd32a8b4f9c7aa443d852aacf9ca214"},
+    {file = "watchfiles-0.21.0-cp38-none-win_amd64.whl", hash = "sha256:8d5f400326840934e3507701f9f7269247f7c026d1b6cfd49477d2be0933cfca"},
+    {file = "watchfiles-0.21.0-cp39-cp39-macosx_10_7_x86_64.whl", hash = "sha256:7f762a1a85a12cc3484f77eee7be87b10f8c50b0b787bb02f4e357403cad0c0e"},
+    {file = "watchfiles-0.21.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:6e9be3ef84e2bb9710f3f777accce25556f4a71e15d2b73223788d528fcc2052"},
+    {file = "watchfiles-0.21.0-cp39-cp39-manylinux_2_12_i686.manylinux2010_i686.whl", hash = "sha256:4c48a10d17571d1275701e14a601e36959ffada3add8cdbc9e5061a6e3579a5d"},
+    {file = "watchfiles-0.21.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6c889025f59884423428c261f212e04d438de865beda0b1e1babab85ef4c0f01"},
+    {file = "watchfiles-0.21.0-cp39-cp39-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:66fac0c238ab9a2e72d026b5fb91cb902c146202bbd29a9a1a44e8db7b710b6f"},
+    {file = "watchfiles-0.21.0-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b4a21f71885aa2744719459951819e7bf5a906a6448a6b2bbce8e9cc9f2c8128"},
+    {file = "watchfiles-0.21.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:1c9198c989f47898b2c22201756f73249de3748e0fc9de44adaf54a8b259cc0c"},
+    {file = "watchfiles-0.21.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d8f57c4461cd24fda22493109c45b3980863c58a25b8bec885ca8bea6b8d4b28"},
+    {file = "watchfiles-0.21.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:853853cbf7bf9408b404754b92512ebe3e3a83587503d766d23e6bf83d092ee6"},
+    {file = "watchfiles-0.21.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:d5b1dc0e708fad9f92c296ab2f948af403bf201db8fb2eb4c8179db143732e49"},
+    {file = "watchfiles-0.21.0-cp39-none-win32.whl", hash = "sha256:59137c0c6826bd56c710d1d2bda81553b5e6b7c84d5a676747d80caf0409ad94"},
+    {file = "watchfiles-0.21.0-cp39-none-win_amd64.whl", hash = "sha256:6cb8fdc044909e2078c248986f2fc76f911f72b51ea4a4fbbf472e01d14faa58"},
+    {file = "watchfiles-0.21.0-pp310-pypy310_pp73-macosx_10_7_x86_64.whl", hash = "sha256:ab03a90b305d2588e8352168e8c5a1520b721d2d367f31e9332c4235b30b8994"},
+    {file = "watchfiles-0.21.0-pp310-pypy310_pp73-macosx_11_0_arm64.whl", hash = "sha256:927c589500f9f41e370b0125c12ac9e7d3a2fd166b89e9ee2828b3dda20bfe6f"},
+    {file = "watchfiles-0.21.0-pp310-pypy310_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1bd467213195e76f838caf2c28cd65e58302d0254e636e7c0fca81efa4a2e62c"},
+    {file = "watchfiles-0.21.0-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:02b73130687bc3f6bb79d8a170959042eb56eb3a42df3671c79b428cd73f17cc"},
+    {file = "watchfiles-0.21.0-pp38-pypy38_pp73-macosx_10_7_x86_64.whl", hash = "sha256:08dca260e85ffae975448e344834d765983237ad6dc308231aa16e7933db763e"},
+    {file = "watchfiles-0.21.0-pp38-pypy38_pp73-macosx_11_0_arm64.whl", hash = "sha256:3ccceb50c611c433145502735e0370877cced72a6c70fd2410238bcbc7fe51d8"},
+    {file = "watchfiles-0.21.0-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:57d430f5fb63fea141ab71ca9c064e80de3a20b427ca2febcbfcef70ff0ce895"},
+    {file = "watchfiles-0.21.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0dd5fad9b9c0dd89904bbdea978ce89a2b692a7ee8a0ce19b940e538c88a809c"},
+    {file = "watchfiles-0.21.0-pp39-pypy39_pp73-macosx_10_7_x86_64.whl", hash = "sha256:be6dd5d52b73018b21adc1c5d28ac0c68184a64769052dfeb0c5d9998e7f56a2"},
+    {file = "watchfiles-0.21.0-pp39-pypy39_pp73-macosx_11_0_arm64.whl", hash = "sha256:b3cab0e06143768499384a8a5efb9c4dc53e19382952859e4802f294214f36ec"},
+    {file = "watchfiles-0.21.0-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8c6ed10c2497e5fedadf61e465b3ca12a19f96004c15dcffe4bd442ebadc2d85"},
+    {file = "watchfiles-0.21.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:43babacef21c519bc6631c5fce2a61eccdfc011b4bcb9047255e9620732c8097"},
+    {file = "watchfiles-0.21.0.tar.gz", hash = "sha256:c76c635fabf542bb78524905718c39f736a98e5ab25b23ec6d4abede1a85a6a3"},
 ]
 
 [[package]]
 name = "webencodings"
 version = "0.5.1"
 summary = "Character encoding aliases for legacy web content"
 groups = ["docs"]
 files = [
     {file = "webencodings-0.5.1-py2.py3-none-any.whl", hash = "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78"},
     {file = "webencodings-0.5.1.tar.gz", hash = "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"},
 ]
 
 [[package]]
+name = "wheel"
+version = "0.43.0"
+requires_python = ">=3.8"
+summary = "A built-package format for Python"
+groups = ["docs"]
+files = [
+    {file = "wheel-0.43.0-py3-none-any.whl", hash = "sha256:55c570405f142630c6b9f72fe09d9b67cf1477fcf543ae5b8dcb1f5b7377da81"},
+    {file = "wheel-0.43.0.tar.gz", hash = "sha256:465ef92c69fa5c5da2d1cf8ac40559a8c940886afcef87dcf14b9470862f1d85"},
+]
+
+[[package]]
 name = "zipp"
 version = "3.18.1"
 requires_python = ">=3.8"
 summary = "Backport of pathlib-compatible object wrapper for zip files"
 groups = ["default", "docs"]
 marker = "python_version < \"3.10\""
 files = [
```

### Comparing `litestar_granian-0.2.6/.github/workflows/cd.yaml` & `litestar_granian-0.3.0/.github/workflows/cd.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/.github/workflows/ci.yaml` & `litestar_granian-0.3.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/.github/workflows/docs-preview.yaml` & `litestar_granian-0.3.0/.github/workflows/docs-preview.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/.github/workflows/docs.yaml` & `litestar_granian-0.3.0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/.github/workflows/publish.yaml` & `litestar_granian-0.3.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/docs/Makefile` & `litestar_granian-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/docs/conf.py` & `litestar_granian-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/docs/fix_missing_references.py` & `litestar_granian-0.3.0/docs/fix_missing_references.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/docs/index.rst` & `litestar_granian-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/examples/basic.py` & `litestar_granian-0.3.0/examples/basic.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/examples/structlog.py` & `litestar_granian-0.3.0/examples/structlog.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/litestar_granian/cli.py` & `litestar_granian-0.3.0/litestar_granian/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import click
 from click import Context, command, option
 from granian.constants import HTTPModes, Loops, ThreadModes
 from granian.http import HTTP1Settings, HTTP2Settings
 from litestar.cli._utils import LitestarEnv
 
 try:
-    from litestar.cli._utils import isatty  # type: ignore[attr-defined]
+    from litestar.cli._utils import isatty  # type: ignore[attr-defined,unused-ignore]
 except ImportError:  # pragma: nocover
 
     def isatty() -> bool:  # pragma: nocover
         """Detect if a terminal is TTY enabled.
 
         This was added in Litestar 2.8 and is backported for compatibility.
 
@@ -27,15 +27,15 @@
 
 
 if TYPE_CHECKING:
     from litestar import Litestar
     from litestar.cli._utils import LitestarEnv
 
 
-@command(name="run")
+@command(name="run", context_settings={"show_default": True}, help="Start application server")
 @option("-p", "--port", help="Serve under this port", type=int, default=8000, show_default=True, envvar="LITESTAR_PORT")
 @option(
     "-W",
     "--wc",
     "--web-concurrency",
     "--workers",
     help="The number of processes to start.",
@@ -177,23 +177,33 @@
 @option("-P", "--pdb", "--use-pdb", help="Drop into PDB on an exception", is_flag=True, envvar="LITESTAR_PDB")
 @option(
     "--respawn-failed-workers/--no-respawn-failed-workers",
     help="Enable workers respawn on unexpected exit",
     default=False,
     is_flag=True,
 )
-@option("-r", "--reload", help="Reload server on changes", default=False, is_flag=True, envvar="LITESTAR_RELOAD")
+@option(
+    "--respawn-interval",
+    default=3.5,
+    help="The number of seconds to sleep between workers respawn",
+)
+@option("-r", "--reload/--no-reload", help="Reload server on changes", default=False, is_flag=True)
+@option(
+    "--process-name",
+    help="Set a custom name for processes.",
+)
 def run_command(
     app: Litestar,
     reload: bool,
     port: int,
     wc: int,
     threads: int,
     blocking_threads: int,
     respawn_failed_workers: bool,
+    respawn_interval: float,
     http1_keep_alive: bool,
     http1_buffer_size: int,
     http1_pipeline_flush: bool,
     http2_adaptive_window: bool,
     http2_initial_connection_window_size: int,
     http2_initial_stream_window_size: int,
     http2_keep_alive_interval: int | None,
@@ -207,14 +217,15 @@
     backlog: int,
     threading_mode: ThreadModes,
     ssl_keyfile: Path | None,
     ssl_certificate: Path | None,
     create_self_signed_cert: bool,
     url_path_prefix: str | None,
     host: str,
+    process_name: str | None,
     debug: bool,
     pdb: bool,
     ctx: Context,
 ) -> None:  # sourcery skip: low-code-quality
     """Run a Litestar app.
 
     The app can be either passed as a module path in the form of <module name>.<submodule>:<app instance or factory>,
@@ -271,27 +282,29 @@
             wc=workers,
             threads=threads,
             http=http,
             opt=opt,
             backlog=backlog,
             blocking_threads=blocking_threads,
             respawn_failed_workers=respawn_failed_workers,
+            respawn_interval=respawn_interval,
             http1_buffer_size=http1_buffer_size,
             http1_keep_alive=http1_keep_alive,
             http1_pipeline_flush=http1_pipeline_flush,
             http2_adaptive_window=http2_adaptive_window,
             http2_initial_connection_window_size=http2_initial_connection_window_size,
             http2_initial_stream_window_size=http2_initial_stream_window_size,
             http2_keep_alive_interval=http2_keep_alive_interval,
             http2_keep_alive_timeout=http2_keep_alive_timeout,
             http2_max_concurrent_streams=http2_max_concurrent_streams,
             http2_max_frame_size=http2_max_frame_size,
             http2_max_headers_size=http2_max_headers_size,
             http2_max_send_buffer_size=http2_max_send_buffer_size,
             threading_mode=threading_mode,
+            process_name=process_name,
             ssl_keyfile=ssl_keyfile,
             ssl_certificate=ssl_certificate,
             url_path_prefix=url_path_prefix,
             host=host,
         )
 
 
@@ -320,27 +333,29 @@
     wc: int,
     threads: int,
     http: HTTPModes,
     opt: bool,
     backlog: int,
     blocking_threads: int,
     respawn_failed_workers: bool,
+    respawn_interval: float,
     http1_buffer_size: int,
     http1_keep_alive: bool,
     http1_pipeline_flush: bool,
     http2_adaptive_window: bool,
     http2_initial_connection_window_size: int,
     http2_initial_stream_window_size: int,
     http2_keep_alive_interval: int | None,
     http2_keep_alive_timeout: int,
     http2_max_concurrent_streams: int,
     http2_max_frame_size: int,
     http2_max_headers_size: int,
     http2_max_send_buffer_size: int,
     threading_mode: ThreadModes,
+    process_name: str | None,
     ssl_keyfile: Path | None,
     ssl_certificate: Path | None,
     url_path_prefix: str | None,
 ) -> None:
     from granian.constants import Interfaces
 
     process_args: dict[str, Any] = {
@@ -352,14 +367,15 @@
         "threads": threads,
         "workers": wc,
         "threading-mode": threading_mode.value,
         "blocking-threads": blocking_threads,
         "loop": Loops.auto.value,
         "opt": opt,
         "respawn-failed-workers": respawn_failed_workers,
+        "respawn-interval": respawn_interval,
         "backlog": backlog,
     }
     if http.value in {HTTPModes.http1.value, HTTPModes.auto.value}:
         process_args["http1-keep-alive"] = http1_keep_alive
         process_args["http1-buffer-size"] = http1_buffer_size
         process_args["http1-pipeline-flush"] = http1_pipeline_flush
     if http.value == HTTPModes.http2.value:
@@ -377,11 +393,13 @@
         process_args["websockets"] = False
     if url_path_prefix is not None:
         process_args["url-path-prefix"] = url_path_prefix
     if ssl_certificate is not None:
         process_args["ssl-certfile"] = ssl_certificate
     if ssl_keyfile is not None:
         process_args["ssl-keyfile"] = ssl_keyfile
+    if process_name is not None:
+        process_args["process-name"] = process_name
     subprocess.run(
         [sys.executable, "-m", "granian", env.app_path, *_convert_granian_args(process_args)],  # noqa: S603
         check=True,
     )
```

### Comparing `litestar_granian-0.2.6/litestar_granian/plugin.py` & `litestar_granian-0.3.0/litestar_granian/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     __slots__ = ()
 
     def on_cli_init(self, cli: Group) -> None:
         from litestar.cli.main import litestar_group as cli
 
         cli.add_command(run_command)
-        return super().on_cli_init(cli)
 
     def on_app_init(self, app_config: AppConfig) -> AppConfig:
         if app_config.logging_config is not None and isinstance(app_config.logging_config, LoggingConfig):
             if app_config.logging_config.loggers.get("_granian", None) is None:
                 app_config.logging_config.loggers.update(
                     {"_granian": {"level": "INFO", "handlers": ["queue_listener"], "propagate": False}},
                 )
```

### Comparing `litestar_granian-0.2.6/tests/test_cli.py` & `litestar_granian-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/tests/test_plugin.py` & `litestar_granian-0.3.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/.gitignore` & `litestar_granian-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/LICENSE` & `litestar_granian-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/README.md` & `litestar_granian-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `litestar_granian-0.2.6/pyproject.toml` & `litestar_granian-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-authors = [{ name = "Cody Fincher", email = "cody.fincher@gmail.com" }]
+authors = [{ name = "Cody Fincher", email = "cody@litestar.dev" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Web Environment",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.8",
@@ -13,51 +13,67 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python",
   "Topic :: Software Development",
   "Typing :: Typed",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
 ]
-dependencies = ["litestar>=2.0.1", "granian>=1.0.0"]
+dependencies = ["litestar>=2.0.1", "granian[all]>=1.3.0"]
 description = "Granian plugin for Litestar"
 keywords = ["litestar", "granian", "asgi"]
 license = { text = "MIT" }
 name = "litestar-granian"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.2.6"
+version = "0.3.0"
 
 [project.urls]
 Changelog = "https://cofin.github.io/litesatr-granian/latest/changelog"
 Discord = "https://discord.gg/X3FJqy8d2j"
 Documentation = "https://cofin.github.io/litesatr-granian/latest/"
 Homepage = "https://cofin.github.io/litesatr-granian/latest/"
 Issue = "https://github.com/cofin/litestar-granian/issues/"
 Source = "https://github.com/cofin/litestar-granian"
 
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
+[tool.pdm]
+ignore_package_warnings = [
+  "alabaster",
+  "sphinxcontrib-*",
+  "sphinx-*",
+  "sphinx",
+  "pre-commit",
+  "pydata-sphinx-*",
+  "slotscheck",
+]
+
 [tool.pdm.dev-dependencies]
 dev = ["anyio"]
 docs = [
   "sphinx>=7.1.2",
   "sphinx-autobuild>=2021.3.14",
   "sphinx-copybutton>=0.5.2",
-  "shibuya>=2023.9.3",
   "sphinx-click>=5.0.1",
   "sphinx-toolbox>=3.5.0",
   "sphinx-design>=0.5.0",
-  "types-docutils",
+  "sphinx-paramlinks>=0.6.0",
+  "sphinx-togglebutton>=0.3.2",
+  #    "litestar-sphinx-theme @ {root:uri}/../litestar-sphinx-theme", # only needed when working on the theme
+  "litestar-sphinx-theme @ git+https://github.com/litestar-org/litestar-sphinx-theme.git@v3",
+  "auto-pytabs[sphinx]>=0.4.0",
+  "git-cliff>=2.2.1",
 ]
-linting = ["pre-commit>=3.4.0", "mypy>=1.5.1", "ruff>=0.0.287", "sourcery"]
-test = ["pytest>=7.4.1", "pytest-cov", "coverage", "pytest-mock>=3.11.1"]
+linting = ["pre-commit>=3.4.0", "mypy>=1.5.1", "ruff>=0.0.287", "sourcery", "types-click"]
+test = ["pytest>=7.4.1", "pytest-cov", "coverage", "pytest-mock>=3.11.1", "pytest-sugar"]
 
 [tool.pytest.ini_options]
+addopts = ["-ra"]
 filterwarnings = ["ignore::DeprecationWarning:pkg_resources.*"]
 testpaths = ["tests"]
 
 [tool.coverage.report]
 exclude_lines = [
   'if TYPE_CHECKING:',
   'pragma: no cover',
```

### Comparing `litestar_granian-0.2.6/PKG-INFO` & `litestar_granian-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: litestar-granian
-Version: 0.2.6
+Version: 0.3.0
 Summary: Granian plugin for Litestar
 Project-URL: Changelog, https://cofin.github.io/litesatr-granian/latest/changelog
 Project-URL: Discord, https://discord.gg/X3FJqy8d2j
 Project-URL: Documentation, https://cofin.github.io/litesatr-granian/latest/
 Project-URL: Homepage, https://cofin.github.io/litesatr-granian/latest/
 Project-URL: Issue, https://github.com/cofin/litestar-granian/issues/
 Project-URL: Source, https://github.com/cofin/litestar-granian
-Author-email: Cody Fincher <cody.fincher@gmail.com>
+Author-email: Cody Fincher <cody@litestar.dev>
 License: MIT
 License-File: LICENSE
 Keywords: asgi,granian,litestar
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: granian>=1.0.0
+Requires-Dist: granian[all]>=1.3.0
 Requires-Dist: litestar>=2.0.1
 Description-Content-Type: text/markdown
 
 # Litestar Granian Plugin
 
 ## Installation
```

