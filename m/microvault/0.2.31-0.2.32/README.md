# Comparing `tmp/microvault-0.2.31.tar.gz` & `tmp/microvault-0.2.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microvault-0.2.31.tar", max compression
+gzip compressed data, was "microvault-0.2.32.tar", max compression
```

## Comparing `microvault-0.2.31.tar` & `microvault-0.2.32.tar`

### file list

```diff
@@ -1,6 +1,17 @@
--rw-r--r--   0        0        0     1091 2024-02-10 04:03:06.563439 microvault-0.2.31/LICENSE
--rw-r--r--   0        0        0      950 2024-02-12 04:21:04.503538 microvault-0.2.31/README.md
--rwxr-xr-x   0        0        0        0 2024-02-12 04:12:46.282352 microvault-0.2.31/microvault/__init__.py
--rwxr-xr-x   0        0        0      485 2024-02-10 06:09:17.402647 microvault-0.2.31/microvault/config_robot.py
--rw-r--r--   0        0        0     1512 2024-02-12 04:23:03.638433 microvault-0.2.31/pyproject.toml
--rw-r--r--   0        0        0     2338 1970-01-01 00:00:00.000000 microvault-0.2.31/PKG-INFO
+-rwxr-xr-x   0        0        0     1091 2024-03-25 20:45:41.513051 microvault-0.2.32/LICENSE
+-rwxr-xr-x   0        0        0     1688 2024-05-05 15:32:07.825264 microvault-0.2.32/README.md
+-rwxr-xr-x   0        0        0        0 2024-02-12 04:12:46.282352 microvault-0.2.32/microvault/__init__.py
+-rw-r--r--   0        0        0     9150 2024-03-30 02:34:22.554377 microvault-0.2.32/microvault/algorithm/td3.py
+-rw-r--r--   0        0        0     7301 2024-03-30 01:18:55.024986 microvault-0.2.32/microvault/components/replaybuffer.py
+-rw-r--r--   0        0        0        0 2024-02-18 03:58:03.046494 microvault-0.2.32/microvault/environment/__init__.py
+-rw-r--r--   0        0        0     7366 2024-05-05 20:54:09.818468 microvault-0.2.32/microvault/environment/continuous.py
+-rw-r--r--   0        0        0     3078 2024-05-05 20:54:09.818533 microvault-0.2.32/microvault/environment/generate.py
+-rw-r--r--   0        0        0     3144 2024-05-05 20:54:09.818587 microvault-0.2.32/microvault/environment/robot.py
+-rw-r--r--   0        0        0        0 2024-02-26 22:43:37.479679 microvault-0.2.32/microvault/environment/utils/__init__.py
+-rw-r--r--   0        0        0     1478 2024-05-05 02:41:14.387585 microvault-0.2.32/microvault/environment/utils/collision.py
+-rw-r--r--   0        0        0     5073 2024-05-05 02:42:43.352578 microvault-0.2.32/microvault/environment/utils/map2d.py
+-rw-r--r--   0        0        0     1909 2024-05-05 16:26:08.856145 microvault-0.2.32/microvault/environment/utils/world_generate.py
+-rw-r--r--   0        0        0     5201 2024-03-30 02:38:39.373181 microvault-0.2.32/microvault/network/model.py
+-rw-r--r--   0        0        0     3035 2024-03-30 02:37:48.997987 microvault-0.2.32/microvault/wrapper/wrapper.py
+-rw-r--r--   0        0        0     1806 2024-05-05 20:52:24.008344 microvault-0.2.32/pyproject.toml
+-rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 microvault-0.2.32/PKG-INFO
```

### Comparing `microvault-0.2.31/LICENSE` & `microvault-0.2.32/LICENSE`

 * *Files identical despite different names*

### Comparing `microvault-0.2.31/pyproject.toml` & `microvault-0.2.32/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,70 @@
 [tool.poetry]
 name = "microvault"
-version = "0.2.31"
-description = "MicroVault - RL for Navigation"
+version = "0.2.32"
+description = "Microvault - RL for Navigation"
 authors = ["Nicolasalan <grottimeireles@gmail.com>"]
 license = "LICENSE"
 readme = "README.md"
-packages = [{ include = "microvault"}]
+packages = [{ include = "microvault" }]
 
 [tool.poetry.urls]
 documentation = "https://microvault.vercel.app"
 bugs = "https://github.com/microvault/microvault/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 accelerate = "^0.18.0"
 fastrand = "^1.3.0"
 gymnasium = "^0.28.1"
 hydra-core = "^1.3.2"
 matplotlib = "^3.4.3"
 numpy = "^1.24.2"
 omegaconf = "^2.3.0"
-termcolor = "^1.1.0"
 torch = "^2.0.1"
-tqdm = "^4.65.0"
 transformers = "^4.36.0"
 pyyaml = "^6.0.1"
 pymunk = "^6.6.0"
 psutil = "^5.9.8"
 wget = "^3.2"
 lightning = "^2.2.0"
 scipy = "^1.12.0"
 openai = "^1.12.0"
-rich = "^13.7.0"
+cython = "^3.0.8"
+scikit-image = "*"
+numba = "^0.59.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1.0"
 black = "^24.1.1"
 isort = "^5.13.2"
 taskipy = "^1.12.2"
 ruff = "^0.2.1"
 codespell = "^2.2.6"
 commitizen = "^3.14.1"
+pre-commit = "^3.7.0"
+shapely = "^1.8.0"
+
+# [tool.poetry.group.doc.dependencies]
+# furo = "2024.4.27"
+# sphinx = "7.3.7"
+# sphinx-toolbox = "3.5.0"
+# sphinx-notfound-page = "1.0.0"
 
 [tool.pytest.ini_options]
 pythonpath = "."
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.taskipy.tasks]
-lint = "black --check --diff . && ruff check --diff . && isort --check --diff . && codespell --skip=*.css,*.js,*.map,*.scss,*.svg, *.html,*.json,*.yml,*.yaml,*.md,*.jsx,*.mdx"
+lint = "black --check --diff --exclude docs . --exclude data && ruff check --diff --exclude docs . && isort --check --diff --skip docs . && codespell --skip=*.css,*.js,*.map,*.scss,*.svg,*.html,*.json,*.yml,*.yaml,*.md,*.jsx,*.mdx,*.pyx,*.cpp,./data/map/*,./docs/*"
+docs = "mkdocs serve"
 pre_test = "task lint"
 test = "pytest -s -x --cov=microvault -vv"
 post_test = "coverage html"
 publish = "poetry publish --build -u __token__ -p $MICROVAULT_PYPI_TOKEN"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `microvault-0.2.31/PKG-INFO` & `microvault-0.2.32/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 Metadata-Version: 2.1
 Name: microvault
-Version: 0.2.31
-Summary: MicroVault - RL for Navigation
+Version: 0.2.32
+Summary: Microvault - RL for Navigation
 License: LICENSE
 Author: Nicolasalan
 Author-email: grottimeireles@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: accelerate (>=0.18.0,<0.19.0)
+Requires-Dist: cython (>=3.0.8,<4.0.0)
 Requires-Dist: fastrand (>=1.3.0,<2.0.0)
 Requires-Dist: gymnasium (>=0.28.1,<0.29.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: lightning (>=2.2.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
+Requires-Dist: numba (>=0.59.1,<0.60.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: pymunk (>=6.6.0,<7.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: rich (>=13.7.0,<14.0.0)
+Requires-Dist: scikit-image
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
-Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: transformers (>=4.36.0,<5.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Project-URL: bugs, https://github.com/microvault/microvault/issues
 Project-URL: documentation, https://microvault.vercel.app
 Description-Content-Type: text/markdown
 
 # Microvault
 
 <p align="center">
-  <a href="https://badge.fury.io/py/microvault"><img src="https://badge.fury.io/py/microvault.svg" alt="PyPI version"></a>
+  <img src="docs/_static/img.png" alt="MicroVault">
+</p>
+
+<p align="center">
+  <a href='https://microvault.readthedocs.io/en/latest/?badge=latest'><img src='https://readthedocs.org/projects/microvault/badge/?version=latest' alt='Documentation Status' /></a>
+  <a href="https://twitter.com/Microvault_"><img alt="Twiter" src="https://img.shields.io/badge/microvault-twiter-blue"></a>
+  <a href="https://pypi.org/project/microvault/"><img alt="PyPI" src="https://img.shields.io/pypi/v/microvault"></a>
   <a href="https://github.com/astral-sh/ruff"><img alt="Ruff" src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json"></a>
   <a href="https://codecov.io/gh/microvault/microvault"><img alt="codecov" src="https://codecov.io/gh/microvault/microvault/graph/badge.svg?token=WRTOBP06AW"></a>
   <a href="https://github.com/microvault/microvault/actions/workflows/main.yaml"><img alt="CI" src="https://github.com/microvault/microvault/actions/workflows/main.yaml/badge.svg"></a>
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+  <a href="https://pydantic.dev"><img alt="Pydantic v2" src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json"></a>
+<a href="https://codeclimate.com/github/microvault/microvault/maintainability"><img src="https://api.codeclimate.com/v1/badges/f121e3b57214eac38280/maintainability" /></a>
+
 </p>
 
 <div align="center">
 
-**This is a Deep Reinforcement Learning library focused on mobile robot navigation.**
+**This is a Deep Reinforcement Learning library focused on mobile service robots navigation.**
 
 </div>
```

#### html2text {}

```diff
@@ -1,22 +1,25 @@
-Metadata-Version: 2.1 Name: microvault Version: 0.2.31 Summary: MicroVault - RL
+Metadata-Version: 2.1 Name: microvault Version: 0.2.32 Summary: Microvault - RL
 for Navigation License: LICENSE Author: Nicolasalan Author-email:
 grottimeireles@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: accelerate (>=0.18.0,<0.19.0) Requires-Dist: fastrand
-(>=1.3.0,<2.0.0) Requires-Dist: gymnasium (>=0.28.1,<0.29.0) Requires-Dist:
-hydra-core (>=1.3.2,<2.0.0) Requires-Dist: lightning (>=2.2.0,<3.0.0) Requires-
-Dist: matplotlib (>=3.4.3,<4.0.0) Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: omegaconf (>=2.3.0,<3.0.0) Requires-Dist: openai
-(>=1.12.0,<2.0.0) Requires-Dist: psutil (>=5.9.8,<6.0.0) Requires-Dist: pymunk
-(>=6.6.0,<7.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: rich
-(>=13.7.0,<14.0.0) Requires-Dist: scipy (>=1.12.0,<2.0.0) Requires-Dist:
-termcolor (>=1.1.0,<2.0.0) Requires-Dist: torch (>=2.0.1,<3.0.0) Requires-Dist:
-tqdm (>=4.65.0,<5.0.0) Requires-Dist: transformers (>=4.36.0,<5.0.0) Requires-
-Dist: wget (>=3.2,<4.0) Project-URL: bugs, https://github.com/microvault/
-microvault/issues Project-URL: documentation, https://microvault.vercel.app
-Description-Content-Type: text/markdown # Microvault
-             _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_R_u_f_f_]_[_c_o_d_e_c_o_v_]_[_C_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
-    **This is a Deep Reinforcement Learning library focused on mobile robot
-                                 navigation.**
+Requires-Dist: accelerate (>=0.18.0,<0.19.0) Requires-Dist: cython
+(>=3.0.8,<4.0.0) Requires-Dist: fastrand (>=1.3.0,<2.0.0) Requires-Dist:
+gymnasium (>=0.28.1,<0.29.0) Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
+Requires-Dist: lightning (>=2.2.0,<3.0.0) Requires-Dist: matplotlib
+(>=3.4.3,<4.0.0) Requires-Dist: numba (>=0.59.1,<0.60.0) Requires-Dist: numpy
+(>=1.24.2,<2.0.0) Requires-Dist: omegaconf (>=2.3.0,<3.0.0) Requires-Dist:
+openai (>=1.12.0,<2.0.0) Requires-Dist: psutil (>=5.9.8,<6.0.0) Requires-Dist:
+pymunk (>=6.6.0,<7.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist:
+scikit-image Requires-Dist: scipy (>=1.12.0,<2.0.0) Requires-Dist: torch
+(>=2.0.1,<3.0.0) Requires-Dist: transformers (>=4.36.0,<5.0.0) Requires-Dist:
+wget (>=3.2,<4.0) Project-URL: bugs, https://github.com/microvault/microvault/
+issues Project-URL: documentation, https://microvault.vercel.app Description-
+Content-Type: text/markdown # Microvault
+                                 [MicroVault]
+  _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_w_i_t_e_r_]_[_P_y_P_I_]_[_R_u_f_f_]_[_c_o_d_e_c_o_v_]_[_C_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]
+   _[_P_y_d_a_n_t_i_c_ _v_2_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_f_1_2_1_e_3_b_5_7_2_1_4_e_a_c_3_8_2_8_0_/
+                               _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]
+   **This is a Deep Reinforcement Learning library focused on mobile service
+                             robots navigation.**
```

