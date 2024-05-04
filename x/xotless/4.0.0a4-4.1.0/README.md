# Comparing `tmp/xotless-4.0.0a4.tar.gz` & `tmp/xotless-4.1.0.tar.gz`

## Comparing `xotless-4.0.0a4.tar` & `xotless-4.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xotless-4.0.0a4/.dir-locals.el
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 xotless-4.0.0a4/.gitlab-ci.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.0.0a4/HISTORY.rst -> docs/source/history.rst
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 xotless-4.0.0a4/Makefile
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 xotless-4.0.0a4/conftest.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 xotless-4.0.0a4/mypy.ini
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 xotless-4.0.0a4/pytest.ini
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 xotless-4.0.0a4/requirements-dev-py312.lock
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 xotless-4.0.0a4/tox.ini
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 xotless-4.0.0a4/ci/cleanup.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/Makefile
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/conf.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/context.rst
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/domains.rst
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/history.rst
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/immutables.rst
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/index.rst
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/itertools.rst
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/pickablenv.rst
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/ranges.rst
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/testing.rst
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/tracing.rst
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/trees.rst
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/walk.rst
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 xotless-4.0.0a4/docs/source/_static/custom.css
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/tests/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/tests/support.py
--rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/tests/test_domains.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/tests/test_immutables.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/tests/test_interval_tree.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/tests/test_lines.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/tests/test_walk.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/_version.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/context.py
--rw-r--r--   0        0        0    15900 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/domains.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/enums.py
--rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/immutables.py
--rw-r--r--   0        0        0    11569 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/itertools.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/pickablenv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/py.typed
--rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/ranges.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/release.pyi
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/tracing.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/trees.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/types.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/walk.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/testing/strategies/__init__.py
--rw-r--r--   0        0        0    14098 2020-02-02 00:00:00.000000 xotless-4.0.0a4/src/xotless/testing/strategies/domains.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 xotless-4.0.0a4/.gitignore
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 xotless-4.0.0a4/README.rst
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 xotless-4.0.0a4/pyproject.toml
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 xotless-4.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xotless-4.1.0/.dir-locals.el
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 xotless-4.1.0/.gitlab-ci.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.1.0/HISTORY.rst -> docs/source/history.rst
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xotless-4.1.0/Makefile
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 xotless-4.1.0/conftest.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 xotless-4.1.0/mypy.ini
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 xotless-4.1.0/pytest.ini
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 xotless-4.1.0/requirements-dev-py312.lock
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 xotless-4.1.0/tox.ini
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 xotless-4.1.0/ci/cleanup.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/Makefile
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/context.rst
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/domains.rst
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/history.rst
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/immutables.rst
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/itertools.rst
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/pickablenv.rst
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/ranges.rst
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/testing.rst
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/tracing.rst
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/trees.rst
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/walk.rst
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 xotless-4.1.0/docs/source/_static/custom.css
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/support.py
+-rw-r--r--   0        0        0    26105 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/test_domains.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/test_immutables.py
+-rw-r--r--   0        0        0     5704 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/test_interval_tree.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/test_lines.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 xotless-4.1.0/src/tests/test_walk.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/_version.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/context.py
+-rw-r--r--   0        0        0    15897 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/domains.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/enums.py
+-rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/immutables.py
+-rw-r--r--   0        0        0    11569 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/itertools.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/pickablenv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/py.typed
+-rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/ranges.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/release.pyi
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/tracing.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/trees.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/types.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/walk.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/testing/strategies/__init__.py
+-rw-r--r--   0        0        0    14098 2020-02-02 00:00:00.000000 xotless-4.1.0/src/xotless/testing/strategies/domains.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 xotless-4.1.0/.gitignore
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 xotless-4.1.0/README.rst
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 xotless-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 xotless-4.1.0/PKG-INFO
```

### Comparing `xotless-4.0.0a4/.gitlab-ci.yml` & `xotless-4.1.0/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
       - pyproject.toml
       - src/**/*.py
 
 run static checks:
   <<: *run_tox_staticcheck
   parallel:
     matrix:
-      - PYTHON: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+      - PYTHON: ["3.10", "3.11", "3.12"]
   only:
     refs:
       - main
       - merge_requests
     changes:
       - tox.ini
       - pyproject.toml
```

### Comparing `xotless-4.0.0a4/Makefile` & `xotless-4.1.0/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 RYE_EXEC ?= rye run
 PYTHON_VERSION ?= 3.12
 PATH := $(HOME)/.rye/shims:$(PATH)
 
 SHELL := /bin/bash
 PYTHON_FILES := $(shell find src/ -type f -name '*.py' -o -name '*.pyi')
 
+USE_UV ?= true
 install:
-	rye self update || curl -sSf https://rye-up.com/get | bash
-	rye pin --relaxed $(PYTHON_VERSION)
-	rye sync
-	cp -f requirements-dev.lock requirements-dev-py312.lock
+	@uv --version || curl -LsSf https://astral.sh/uv/install.sh | sh
+	@rye self update || curl -sSf https://rye-up.com/get | bash
+	@rye config --set-bool behavior.use-uv=$(USE_UV)
+	@rye pin --relaxed $(PYTHON_VERSION)
+	@rye sync --no-lock
+	@cp requirements-dev.lock requirements-dev-py$$(echo $(PYTHON_VERSION) | sed "s/\.//").lock
 .PHONY: install
 
+sync:
+	@rye config --set-bool behavior.use-uv=$(USE_UV)
+	@rye pin --relaxed $(PYTHON_VERSION)
+	@rye sync --no-lock
+.PHONY: sync
+
+lock:
+	@rye config --set-bool behavior.use-uv=$(USE_UV)
+	@rye pin --relaxed $(PYTHON_VERSION)
+	@rye sync
+	@cp requirements-dev.lock requirements-dev-py$$(echo $(PYTHON_VERSION) | sed "s/\.//").lock
+.PHONY: lock
+
 
 format:
-	@$(RYE_EXEC) ruff --fix src/
+	@$(RYE_EXEC) ruff check --fix src/
 	@$(RYE_EXEC) isort src/
 	@$(RYE_EXEC) ruff format src/
 .PHONY: format
 
 lint:
-	@$(RYE_EXEC) ruff src/
+	@$(RYE_EXEC) ruff check src/
 	@$(RYE_EXEC) ruff format --check src/
 	@$(RYE_EXEC) isort --check src/
 .PHONY: lint
 
 test:
 	@$(RYE_EXEC) tox -e system-unit,system-immutables
 .PHONY: test
```

### Comparing `xotless-4.0.0a4/requirements-dev-py312.lock` & `xotless-4.1.0/requirements-dev-py312.lock`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
-alabaster==0.7.16
+alabaster==0.7.13
     # via sphinx
 attrs==23.2.0
     # via cattrs
     # via hypothesis
     # via lsprotocol
 babel==2.14.0
     # via sphinx
@@ -28,15 +28,14 @@
 chardet==5.2.0
     # via tox
 charset-normalizer==3.3.2
     # via requests
 colorama==0.4.6
     # via tox
 coverage==7.4.1
-    # via coverage
     # via pytest-cov
 distlib==0.3.8
     # via virtualenv
 docutils==0.20.1
     # via sphinx
 execnet==2.0.2
     # via pytest-xdist
@@ -55,24 +54,25 @@
 jinja2==3.1.3
     # via sphinx
 lsprotocol==2023.0.1
     # via pygls
     # via ruff-lsp
 markupsafe==2.1.5
     # via jinja2
-mypy==1.8.0
+mypy==1.10.0
 mypy-extensions==1.0.0
     # via mypy
 packaging==23.2
     # via pyproject-api
     # via pytest
     # via ruff-lsp
     # via sphinx
     # via tox
     # via xotl-tools
+pip==24.0
 platformdirs==4.2.0
     # via tox
     # via virtualenv
 pluggy==1.4.0
     # via pytest
     # via tox
 pygls==1.3.0
@@ -85,45 +85,44 @@
 pytest==8.0.1
     # via pytest-cov
     # via pytest-xdist
 pytest-cov==4.1.0
 pytest-xdist==3.5.0
 requests==2.31.0
     # via sphinx
-ruff==0.2.1
+ruff==0.4.2
     # via ruff-lsp
 ruff-lsp==0.0.52
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via hypothesis
 soupsieve==2.5
     # via beautifulsoup4
 sphinx==7.1.2
     # via furo
     # via sphinx-basic-ng
 sphinx-basic-ng==1.0.0b2
     # via furo
-sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
-sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-qthelp==1.0.3
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.10
+sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 tox==4.12.1
 typing-extensions==4.9.0
     # via mypy
     # via ruff-lsp
     # via xotl-tools
 urllib3==2.2.0
     # via requests
 virtualenv==20.25.0
     # via tox
-xotl-tools==3.0.0a5 ; python_version > "3.11"
+xotl-tools==3.0.0a5
     # via xotless
-pip==24.0
```

### Comparing `xotless-4.0.0a4/tox.ini` & `xotless-4.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/ci/cleanup.yml` & `xotless-4.1.0/ci/cleanup.yml`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/docs/Makefile` & `xotless-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/docs/source/conf.py` & `xotless-4.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/docs/source/domains.rst` & `xotless-4.1.0/docs/source/domains.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/docs/source/history.rst` & `xotless-4.1.0/docs/source/history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 =========
  History
 =========
 
 Releases 4.x
 ============
 
-2024-02-18.  Release 4.0.0a2
-----------------------------
+2024-05-05.  Release 4.1.0
+--------------------------
+
+- Make `~xotless.domains.EquivalentSet`:class: type hint be compatible with
+  iterables.
+
+
+2024-02-29.  Release 4.0.0
+--------------------------
 
 - Use `rye`_ to develop.
 
 - Add support for Python 3.11 and 3.12.
 
   The list of supported Python versions is: 3.8, 3.9, 3.10, 3.11, and 3.12.
```

### Comparing `xotless-4.0.0a4/docs/source/index.rst` & `xotless-4.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/docs/source/pickablenv.rst` & `xotless-4.1.0/docs/source/pickablenv.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/docs/source/ranges.rst` & `xotless-4.1.0/docs/source/ranges.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/docs/source/testing.rst` & `xotless-4.1.0/docs/source/testing.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/docs/source/trees.rst` & `xotless-4.1.0/docs/source/trees.rst`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/tests/support.py` & `xotless-4.1.0/src/tests/support.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/tests/test_domains.py` & `xotless-4.1.0/src/tests/test_domains.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from hypothesis import HealthCheck, example, given, settings
 from hypothesis import strategies as st
 from hypothesis.strategies import SearchStrategy
 from xotl.tools.infinity import Infinity
 
 from xotless.domains import EquivalenceSet, IntervalSet
 from xotless.ranges import Bound, Excluded, Included, Range, RangeKind
-
 from xotless.testing.strategies.domains import (
     date_ranges,
     equivalence_sets,
     float_ranges,
     get_date_member_strategy,
     many_date_ranges,
     many_float_ranges,
```

### Comparing `xotless-4.0.0a4/src/tests/test_immutables.py` & `xotless-4.1.0/src/tests/test_immutables.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/tests/test_interval_tree.py` & `xotless-4.1.0/src/tests/test_interval_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 import pickle
 from datetime import datetime
 
 from hypothesis import given
 from hypothesis import strategies as st
 
 from xotless.ranges import Range
-from xotless.trees import Cell, IntervalTree
-
 from xotless.testing.strategies.domains import (
     FloatRangeHelper,
     date_ranges,
     float_ranges,
     many_date_ranges,
     many_float_ranges,
     members_of_date_ranges,
     members_of_float_ranges,
 )
+from xotless.trees import Cell, IntervalTree
 
 MORE_THAN_ONE_LIFETIME = Range.new_open_right(datetime(1978, 10, 21), datetime(9078, 10, 21))
 
 
 @given(st.data(), many_date_ranges(5, outer=MORE_THAN_ONE_LIFETIME))
 def test_date_interval_trees_finds_the_right_interval(data, intervals):
     cells = [Cell.from_range(r, i) for i, r in enumerate(intervals)]
```

### Comparing `xotless-4.0.0a4/src/tests/test_lines.py` & `xotless-4.1.0/src/tests/test_lines.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/tests/test_walk.py` & `xotless-4.1.0/src/tests/test_walk.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/context.py` & `xotless-4.1.0/src/xotless/context.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/domains.py` & `xotless-4.1.0/src/xotless/domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 @dataclass(init=False, unsafe_hash=True)
 class EquivalenceSet(Generic[TEq]):
     "A simple wrapper over a Python set for items with EqTypeClass"
 
     values: AbstractSet[TEq]
     __slots__ = ("values", "_sample")
 
-    def __init__(self, values: AbstractSet[TEq]) -> None:
+    def __init__(self, values: Iterable[TEq]) -> None:
         self.values = frozenset(values)
 
     def to_interval_set(self) -> "IntervalSet[TOrd]":
         """Convert to a semantically-equivalent interval set.
 
         This should only be applied for equivalence sets containing orderable
         (Ord) items.
```

### Comparing `xotless-4.0.0a4/src/xotless/immutables.py` & `xotless-4.1.0/src/xotless/immutables.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/itertools.py` & `xotless-4.1.0/src/xotless/itertools.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/pickablenv.py` & `xotless-4.1.0/src/xotless/pickablenv.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/ranges.py` & `xotless-4.1.0/src/xotless/ranges.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/release.py` & `xotless-4.1.0/src/xotless/release.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/tracing.py` & `xotless-4.1.0/src/xotless/tracing.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/trees.py` & `xotless-4.1.0/src/xotless/trees.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/types.py` & `xotless-4.1.0/src/xotless/types.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/walk.py` & `xotless-4.1.0/src/xotless/walk.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/src/xotless/testing/strategies/domains.py` & `xotless-4.1.0/src/xotless/testing/strategies/domains.py`

 * *Files identical despite different names*

### Comparing `xotless-4.0.0a4/pyproject.toml` & `xotless-4.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -33,29 +33,28 @@
 
 [tool.hatch.metadata.hooks.vcs]
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "sphinx~=7.1.2",
-    "ruff==0.2.1",
+    "ruff==0.4.2",
     "ruff-lsp>=0.0.52",
     "furo~=2024.1.29",
     "hypothesis~=6.98.6",
     "tox>=4.12.1",
     "isort>=5.13.2",
     "pip>=24.0",
-    "mypy>=1.8.0",
+    "mypy==1.10.0",
     "pytest>=8.0.1",
     "pytest-cov>=4.1.0",
     "pytest-xdist>=3.5.0",
 ]
 
 [tool.ruff]
-required-version = "0.2.1"
 line-length = 100
 target-version = "py311"
 
 [tool.ruff.lint]
 ignore = [
   "E501", # line-length is left to the formatter
 ]
```

### Comparing `xotless-4.0.0a4/PKG-INFO` & `xotless-4.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: xotless
-Version: 4.0.0a4
+Version: 4.1.0
 Summary: Collection of small utilities that have not yet being promoted to xotl.tools.
 Author-email: "Merchise Autrement [~º/~]" <info@merchise.de>
 License-Expression: MIT
 Requires-Python: >=3.8
 Requires-Dist: xotl-tools<4.0,>=2.2.1; python_version <= '3.11'
 Requires-Dist: xotl-tools<4.0,>=3.0.0a5; python_version > '3.11'
 Provides-Extra: immutables
```

