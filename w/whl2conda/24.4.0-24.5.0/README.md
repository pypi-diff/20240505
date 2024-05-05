# Comparing `tmp/whl2conda-24.4.0.tar.gz` & `tmp/whl2conda-24.5.0.tar.gz`

## Comparing `whl2conda-24.4.0.tar` & `whl2conda-24.5.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/VERSION
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/__about__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/__init__.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/py.typed
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/api/__init__.py
--rw-r--r--   0        0        0    33693 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/api/converter.py
--rw-r--r--   0        0        0    34867 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/api/stdrename.json
--rw-r--r--   0        0        0    10450 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/api/stdrename.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/__init__.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/build.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/common.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/config.py
--rw-r--r--   0        0        0    17551 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/convert.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/diff.py
--rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/install.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/cli/main.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/external/__init__.py
--rw-r--r--   0        0        0    26218 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/external/version.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/impl/__init__.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/impl/download.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/impl/prompt.py
--rw-r--r--   0        0        0     9907 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/impl/pyproject.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 whl2conda-24.4.0/src/whl2conda/impl/wheel.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 whl2conda-24.4.0/.gitignore
--rw-r--r--   0        0        0    11564 2020-02-02 00:00:00.000000 whl2conda-24.4.0/LICENSE.md
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 whl2conda-24.4.0/README.md
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 whl2conda-24.4.0/pyproject.toml
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 whl2conda-24.4.0/PKG-INFO
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/VERSION
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/__about__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/__init__.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/py.typed
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/settings.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/api/__init__.py
+-rw-r--r--   0        0        0    33771 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/api/converter.py
+-rw-r--r--   0        0        0    35832 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/api/stdrename.json
+-rw-r--r--   0        0        0    10450 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/api/stdrename.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/cli/__init__.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/cli/build.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/cli/common.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/cli/config.py
+-rw-r--r--   0        0        0    18433 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/cli/convert.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/cli/diff.py
+-rw-r--r--   0        0        0    11538 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/cli/install.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/cli/main.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/external/__init__.py
+-rw-r--r--   0        0        0    26218 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/external/version.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/impl/__init__.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/impl/download.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/impl/prompt.py
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/impl/pyproject.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 whl2conda-24.5.0/src/whl2conda/impl/wheel.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 whl2conda-24.5.0/.gitignore
+-rw-r--r--   0        0        0    11564 2020-02-02 00:00:00.000000 whl2conda-24.5.0/LICENSE.md
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 whl2conda-24.5.0/README.md
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 whl2conda-24.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 whl2conda-24.5.0/PKG-INFO
```

### Comparing `whl2conda-24.4.0/src/whl2conda/__about__.py` & `whl2conda-24.5.0/src/whl2conda/__about__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/__init__.py` & `whl2conda-24.5.0/src/whl2conda/__init__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/__main__.py` & `whl2conda-24.5.0/src/whl2conda/__main__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/api/__init__.py` & `whl2conda-24.5.0/src/whl2conda/api/__init__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/api/converter.py` & `whl2conda-24.5.0/src/whl2conda/api/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,22 +309,24 @@
     conda_pkg_path: Optional[Path] = None
     std_renames: dict[str, str]
 
     def __init__(
         self,
         wheel_path: Path,
         out_dir: Path,
+        *,
+        update_std_renames: bool = False,
     ):
         self.logger = logging.getLogger(__name__)
         self.wheel_path = wheel_path
         self.out_dir = out_dir
         self.dependency_rename = []
         self.extra_dependencies = []
         # TODO - option to ignore this
-        self.std_renames = load_std_renames()
+        self.std_renames = load_std_renames(update=update_std_renames)
 
     def convert(self) -> Path:
         """
         Convert wheel to conda package
 
         Does not write any non-temporary files if dry_run is True.
```

### Comparing `whl2conda-24.4.0/src/whl2conda/api/stdrename.json` & `whl2conda-24.5.0/src/whl2conda/api/stdrename.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9617044228694714%*

 * *Differences: {"'$date'": "'Sun, 05 May 2024 14:59:33 GMT'",*

 * * "'$etag'": "'f6ebbcdb498a136a5336054beda9dcbe62fbc5f5fd90c95c42a88cdbcb3e0e1e'",*

 * * "'altair-tiles'": "'altair_tiles'",*

 * * "'amara3-iri'": "'amara3.iri'",*

 * * "'amazon-sagemaker-sql-editor'": "'amazon_sagemaker_sql_editor'",*

 * * "'aws-secretsmanager-caching'": "'aws_secretsmanager_caching'",*

 * * "'backports-tarfile'": "'backports.tarfile'",*

 * * "'cad-to-dagmc'": "'cad_to_dagmc'",*

 * * "'caf-distribute'": "'caf.distribute'",*

 * * "'compas-robots'": "'compas_robots'",*

 * * "'compas-timber' […]*

```diff
@@ -1,21 +1,24 @@
 {
-    "$date": "Sun, 28 Jan 2024 17:38:56 GMT",
-    "$etag": "f5d7c0bdb46b34790aa49f1ee2b4b393ec7af5bc331e9551d81a08278f30537d",
+    "$date": "Sun, 05 May 2024 14:59:33 GMT",
+    "$etag": "f6ebbcdb498a136a5336054beda9dcbe62fbc5f5fd90c95c42a88cdbcb3e0e1e",
     "$max-age": "300",
     "$source": "https://raw.githubusercontent.com/regro/cf-graph-countyfair/master/mappings/pypi/name_mapping.json",
     "0164e082b29777fbc56c2373b68da93d23a29a040787e7f1c65e1562f133": "django-jsoneditor",
     "33162c0a7b28a4d8c83da07bc2b12cee58c120b4a9e8bba31c41c8d35a16": "vcversioner",
     "9e118aa3f6684187e7ba3727864cfd8e8209ad2d4c59b668f1d41e76f241": "pyelastix",
     "acrv-datasets": "acrv_datasets",
     "aiida-wannier90-workflows": "aiida-wannier90_workflows",
     "alpha-vantage": "alpha_vantage",
     "altair-data-server": "altair_data_server",
     "altair-saver": "altair_saver",
+    "altair-tiles": "altair_tiles",
     "altair-viewer": "altair_viewer",
+    "amara3-iri": "amara3.iri",
+    "amazon-sagemaker-sql-editor": "amazon_sagemaker_sql_editor",
     "ann-visualizer": "ann_visualizer",
     "annoy": "python-annoy",
     "ap-features": "ap_features",
     "apache-airflow": "airflow",
     "apache-superset": "superset",
     "apoc": "apoc-backend",
     "apply-defaults": "apply_defaults",
@@ -25,15 +28,14 @@
     "array-split": "array_split",
     "arrow-odbc": "arrow_odbc",
     "art": "ascii-art",
     "asana": "python-asana",
     "asap3": "asap",
     "ascii-graph": "ascii_graph",
     "ascii-magic": "ascii_magic",
-    "asf-search": "asf_search",
     "asf-tools": "asf_tools",
     "aspy-refactor-imports": "aspy.refactor-imports",
     "assembly-stats": "assembly_stats",
     "asv-runner": "asv_runner",
     "async-generator": "async_generator",
     "asyncio-extras": "asyncio_extras",
     "atap-widgets": "atap_widgets",
@@ -88,23 +90,24 @@
     "aws-cdk-aws-stepfunctions": "aws-cdk.aws-stepfunctions",
     "aws-cdk-cloud-assembly-schema": "aws-cdk.cloud-assembly-schema",
     "aws-cdk-core": "aws-cdk.core",
     "aws-cdk-custom-resources": "aws-cdk.custom-resources",
     "aws-cdk-cx-api": "aws-cdk.cx-api",
     "aws-cdk-region-info": "aws-cdk.region-info",
     "aws-lambda-builders": "aws_lambda_builders",
+    "aws-secretsmanager-caching": "aws_secretsmanager_caching",
     "backports-abc": "backports_abc",
     "backports-cached-property": "backports.cached-property",
     "backports-csv": "backports.csv",
     "backports-entry-points-selectable": "backports.entry-points-selectable",
     "backports-functools-lru-cache": "backports.functools_lru_cache",
     "backports-shutil-get-terminal-size": "backports.shutil_get_terminal_size",
     "backports-shutil-which": "backports.shutil_which",
     "backports-ssl-match-hostname": "ssl_match_hostname",
-    "backports-strenum": "backports.strenum",
+    "backports-tarfile": "backports.tarfile",
     "backports-tempfile": "backports.tempfile",
     "backports-test-support": "backports.test.support",
     "backports-unittest-mock": "backports.unittest_mock",
     "backports-weakref": "backports.weakref",
     "backports-zoneinfo": "backports.zoneinfo",
     "backtrace": "python-backtrace",
     "bake-cli": "bake",
@@ -135,14 +138,16 @@
     "build": "python-build",
     "bullet": "bullet-python",
     "bw-migrations": "bw_migrations",
     "bw-processing": "bw_processing",
     "cache-decorator": "cache_decorator",
     "cached-interpolate": "cached_interpolate",
     "cached-property": "cached_property",
+    "cad-to-dagmc": "cad_to_dagmc",
+    "caf-distribute": "caf.distribute",
     "caf-space": "caf.space",
     "caf-toolkit": "caf.toolkit",
     "calamari-ocr": "calamari_ocr",
     "calysto-bash": "calysto_bash",
     "captest": "pvcaptest",
     "casa-formats-io": "casa_formats_io",
     "castoredc-api": "castoredc_api",
@@ -171,17 +176,19 @@
     "coloc-sat": "coloc_sat",
     "compas-cloud": "compas_cloud",
     "compas-eve": "compas_eve",
     "compas-fab": "compas_fab",
     "compas-mobile-robot-reloc": "compas_mobile_robot_reloc",
     "compas-nurbs": "compas_nurbs",
     "compas-occ": "compas_occ",
+    "compas-robots": "compas_robots",
     "compas-rrc": "compas_rrc",
     "compas-skeleton": "compas_skeleton",
     "compas-slicer": "compas_slicer",
+    "compas-timber": "compas_timber",
     "compas-tna": "compas_tna",
     "compas-view2": "compas_view2",
     "compress-json": "compress_json",
     "conda-subprocess": "conda_subprocess",
     "connection-pool": "connection_pool",
     "constructive-geometries": "constructive_geometries",
     "contact-map": "contact_map",
@@ -209,14 +216,16 @@
     "dask": "dask-core",
     "dask-traj": "dask_traj",
     "databind-core": "databind.core",
     "databind-json": "databind.json",
     "datacommons-pandas": "datacommons_pandas",
     "datadotworld": "datadotworld-py",
     "dbsp-drp": "dbsp_drp",
+    "ddd-subplots": "ddd_subplots",
+    "decoupler": "decoupler-py",
     "deflate-dict": "deflate_dict",
     "delegator-py": "delegator",
     "delft-fiat": "delft_fiat",
     "dem-stitcher": "dem_stitcher",
     "dependency-injector": "dependency_injector",
     "devtools": "python-devtools",
     "dict-hash": "dict_hash",
@@ -278,14 +287,15 @@
     "environment-settings": "environment_settings",
     "environments-utils": "environments_utils",
     "epiweeks": "epiweeks4cf",
     "eppy": "eppy-core",
     "espnet-model-zoo": "espnet_model_zoo",
     "esprima": "esprima-python",
     "et-xmlfile": "et_xmlfile",
+    "eval-type-backport": "eval_type_backport",
     "exo-puppies": "exo_puppies",
     "extract-msg": "msg-extractor",
     "face-recognition": "face_recognition",
     "face-recognition-models": "face_recognition_models",
     "facebook-business": "facebook_business",
     "factory-boy": "factory_boy",
     "fast-dp": "fast_dp",
@@ -301,17 +311,19 @@
     "flask-cors": "flask_cors",
     "flask-json": "flask_json",
     "flask-rdf": "flask_rdf",
     "flask-request-id": "flask_request_id",
     "flatbuffers": "python-flatbuffers",
     "flatten-json": "flatten_json",
     "flex": "flex-swagger",
+    "flit": "flit-core",
     "flit-install-py2": "flit_install_py2",
     "flufl-enum": "flufl.enum",
     "flufl-lock": "flufl.lock",
+    "fluidfft-mpi-with-fftw": "fluidfft-mpi_with_fftw",
     "foundry-ml": "foundry_ml",
     "freud-analysis": "freud",
     "fs-googledrivefs": "fs.googledrivefs",
     "fs-sshfs": "fs.sshfs",
     "fs-webdavfs": "fs.webdavfs",
     "func-timeout": "func_timeout",
     "funlib-geometry": "funlib.geometry",
@@ -321,15 +333,14 @@
     "gcm-filters": "gcm_filters",
     "generic-parser": "generic_parser",
     "geodemo-zw": "geodemo_zw",
     "geotiff": "python-geotiff",
     "github3-py": "github3.py",
     "giturlparse-py": "giturlparse.py",
     "glfw": "pyglfw",
-    "glow-py": "glow",
     "glpk": "pyglpk",
     "gmpyinfr-amqp": "gmpyinfr_amqp",
     "gmpyinfr-dbutils": "gmpyinfr_dbutils",
     "gmpyinfr-log": "gmpyinfr_log",
     "gmpyinfr-telegram": "gmpyinfr_telegram",
     "gms-preprocessing": "gms_preprocessing",
     "gmx-mmpbsa": "gmx_mmpbsa",
@@ -376,14 +387,15 @@
     "indexed-bzip2": "indexed_bzip2",
     "indexed-zstd": "indexed_zstd",
     "inotify-simple": "inotify_simple",
     "installer": "python-installer",
     "intake-astro": "intake-accumulo",
     "interface-meta": "interface_meta",
     "interval-tree": "interval_tree",
+    "ioos-metrics": "ioos_metrics",
     "ioos-qartod": "ioos_qartod",
     "ioos-qc": "ioos_qc",
     "ipopt": "cyipopt",
     "ipython-genutils": "ipython_genutils",
     "ipython-unittest": "ipython_unittest",
     "isal": "python-isal",
     "iteration-utilities": "iteration_utilities",
@@ -392,18 +404,21 @@
     "jaraco-context": "jaraco.context",
     "jaraco-envs": "jaraco.envs",
     "jaraco-functools": "jaraco.functools",
     "jaraco-itertools": "jaraco.itertools",
     "jaraco-logging": "jaraco.logging",
     "jaraco-stream": "jaraco.stream",
     "jaraco-text": "jaraco.text",
+    "jinja-partials": "jinja_partials",
     "jinja2-pluralize": "jinja2_pluralize",
     "jsii": "python-jsii",
     "json-stream": "json_stream",
     "json-tricks": "json_tricks",
+    "juliacall": "pyjuliacall",
+    "juliapkg": "pyjuliapkg",
     "juliaup": "pyjuliaup",
     "jupyter-app-launcher": "jupyter_app_launcher",
     "jupyter-ascending": "jupyter_ascending",
     "jupyter-bokeh": "jupyter_bokeh",
     "jupyter-client": "jupyter_client",
     "jupyter-cms": "jupyter_cms",
     "jupyter-console": "jupyter_console",
@@ -422,36 +437,36 @@
     "jupyter-qtconsole-colorschemes": "jupyter_qtconsole_colorschemes",
     "jupyter-server": "jupyter_server",
     "jupyter-server-fileid": "jupyter_server_fileid",
     "jupyter-server-terminals": "jupyter_server_terminals",
     "jupyter-server-terminals-proxy": "jupyter_server_terminals_proxy",
     "jupyter-server-xarray-leaflet": "jupyter_server_xarray_leaflet",
     "jupyter-server-ydoc": "jupyter_server_ydoc",
-    "jupyter-sphinx": "jupyter_sphinx",
     "jupyter-telemetry": "jupyter_telemetry",
     "jupyter-to-medium": "jupyter_to_medium",
     "jupyterlab-autoversion": "jupyterlab_autoversion",
     "jupyterlab-code-formatter": "jupyterlab_code_formatter",
     "jupyterlab-commands": "jupyterlab_commands",
     "jupyterlab-downloadfolder": "jupyterlab_downloadfolder",
     "jupyterlab-email": "jupyterlab_email",
     "jupyterlab-execute-time": "jupyterlab_execute_time",
     "jupyterlab-genv": "jupyterlab_genv",
     "jupyterlab-heroku": "jupyterlab_heroku",
     "jupyterlab-iframe": "jupyterlab_iframe",
     "jupyterlab-launcher": "jupyterlab_launcher",
-    "jupyterlab-nbconvert-nocode": "jupyterlab_nbconvert_nocode-meta",
+    "jupyterlab-nbconvert-nocode": "jupyterlab_nbconvert_nocode",
     "jupyterlab-omnisci": "omnisci-pytools",
     "jupyterlab-powerpoint": "jupyterlab_powerpoint",
     "jupyterlab-pygments": "jupyterlab_pygments",
     "jupyterlab-rise": "jupyterlab_rise",
     "jupyterlab-templates": "jupyterlab_templates",
     "jupyterlab-vim": "jupyterlab_vim",
     "jupyterlab-widgets": "jupyterlab_widgets",
     "kaldi-io": "kaldi_io",
+    "keras-mixed-sequence": "keras_mixed_sequence",
     "kerberos": "python-kerberos",
     "kernel-driver": "kernel_driver",
     "keyrings-alt": "keyrings.alt",
     "korean-lunar-calendar": "korean_lunar_calendar",
     "krb5": "pykrb5",
     "kubernetes": "python-kubernetes",
     "kubernetes-asyncio": "kubernetes_asyncio",
@@ -461,23 +476,26 @@
     "lazy-import": "lazy_import",
     "lazy-loader": "lazy_loader",
     "lazy-table": "lazy_table",
     "lcov-cobertura": "lcov_cobertura",
     "leveldb": "python-leveldb",
     "libaio": "python-libaio",
     "libarchive-c": "python-libarchive-c",
+    "libigl": "igl",
     "libsvm": "libsvm-python",
     "lightgbm-ray": "lightgbm_ray",
     "liknorm": "liknorm-py",
     "linear-operator": "linear_operator",
     "lit": "lit-nlp",
+    "lm-eval": "lm_eval",
     "log-symbols": "log_symbols",
     "logging-exceptions": "logging_exceptions",
     "logging-tree": "logging_tree",
     "lpython-emulation": "lpython_emulation",
+    "lrcalc": "python-lrcalc",
     "lumicks-pylake": "lumicks.pylake",
     "mac-alias": "mac_alias",
     "make-arq": "make_arq",
     "map-parallel": "map_parallel",
     "mapbox-earcut": "mapbox_earcut",
     "markdown-strings": "markdown_strings",
     "markov-draftjs": "markov_draftjs",
@@ -566,15 +584,17 @@
     "nvidia-ml-py3": "nvidia-ml",
     "ocean-data-gateway": "ocean_data_gateway",
     "octave-kernel": "octave_kernel",
     "om-pycycle": "pycycle",
     "omfit-classes": "omfit_classes",
     "openalpr": "py-openalpr",
     "opencv-python": "opencv",
+    "opencv-python-headless": "opencv",
     "openidc-client": "openidc_client",
+    "openllm": "openllm-playground",
     "openmesh": "openmesh-python",
     "openquake-engine": "openquake.engine",
     "opensarlab-lib": "opensarlab_lib",
     "opentracing-instrumentation": "opentracing_instrumentation",
     "opt-einsum-fx": "opt_einsum_fx",
     "optics-functions": "optics_functions",
     "ordered-enum": "ordered_enum",
@@ -611,14 +631,15 @@
     "pegasus-wms-api": "pegasus-wms.api",
     "pegasus-wms-common": "pegasus-wms.common",
     "pegasus-wms-dax": "pegasus-wms.dax",
     "pegasus-wms-worker": "pegasus-wms.worker",
     "perspective-parquet": "perspective_parquet",
     "perspective-python": "perspective",
     "piano-fingering": "piano_fingering",
+    "pin-pink": "pink",
     "pisces": "pisces-db",
     "planarity": "python-planarity",
     "plaster-pastedeploy": "plaster_pastedeploy",
     "plot-map": "plot_map",
     "plotly-express": "plotly_express",
     "polaris-lib": "polaris",
     "policy-sentry": "policy_sentry",
@@ -745,14 +766,15 @@
     "ruamel-yaml-jinja2": "ruamel.yaml.jinja2",
     "s-gd2": "s_gd2",
     "s1-frame-enumerator": "s1_frame_enumerator",
     "sagemaker": "sagemaker-python-sdk",
     "sagemaker-containers": "sagemaker_containers",
     "sagemaker-mxnet-training": "sagemaker_mxnet_container",
     "sagemaker-pyspark": "sagemaker_pyspark",
+    "sanitize-ml-labels": "sanitize_ml_labels",
     "sas-kernel": "sas_kernel",
     "scanning-drift-corr": "scanning_drift_corr",
     "scikits-odes": "scikits.odes",
     "sdaxen-python-utilities": "sdaxen_python_utilities",
     "seaborn": "seaborn-split",
     "seclea-ai": "seclea_ai",
     "segment-analytics-python": "analytics-python",
@@ -784,14 +806,15 @@
     "sphinxjp-themecore": "sphinxjp.themecore",
     "sphinxjp-themes-impressjs": "sphinxjp.themes.impressjs",
     "sphinxjp-themes-solarized": "sphinxjp.themes.solarized",
     "spice-hsi": "spice_hsi",
     "splunk-handler": "splunk_handler",
     "sqlalchemy-exasol": "sqlalchemy_exasol",
     "sqlalchemy-schemadisplay": "sqlalchemy_schemadisplay",
+    "sqlean-py": "sqlean.py",
     "sre-yield": "sre_yield",
     "srtm-py": "srtm.py",
     "ssh-ipykernel-interrupt": "ssh_ipykernel_interrupt",
     "ssp-detector": "ssp_detector",
     "stack-data": "stack_data",
     "start-jupyter-cm": "start_jupyter_cm",
     "stats-arrays": "stats_arrays",
@@ -803,14 +826,15 @@
     "substrait": "python-substrait",
     "suitesparse-graphblas": "python-suitesparse-graphblas",
     "super-state-machine": "super_state_machine",
     "support-developer": "support_developer",
     "svg-py": "svg.py",
     "switch-model": "switch_model",
     "sympy-plot-backends": "sympy_plot_backends",
+    "systemd-python": "python-systemd",
     "sysv-ipc": "sysv_ipc",
     "tables": "pytables",
     "taurus-pyqtgraph": "taurus_pyqtgraph",
     "termstyle": "python-termstyle",
     "testflows-asserts": "testflows.asserts",
     "tethys-dask-scheduler": "tethys_dask_scheduler",
     "tethys-dataset-services": "tethys_dataset_services",
@@ -838,14 +862,15 @@
     "typst": "typst-py",
     "tzdata": "python-tzdata",
     "ufal-udpipe": "ufal.udpipe",
     "unfccc-di-api": "unfccc_di_api",
     "universal-pathlib": "universal_pathlib",
     "update-checker": "update_checker",
     "upf-to-json": "upf_to_json",
+    "upkie-description": "upkie_description",
     "urbansim-defaults": "urbansim_defaults",
     "urbansim-templates": "urbansim_templates",
     "urwid-readline": "urwid_readline",
     "usedave": "dave",
     "va-am": "va_am",
     "validate-email": "validate_email",
     "validate-version-code": "validate_version_code",
@@ -874,14 +899,15 @@
     "wwt-kernel-data-relay": "wwt_kernel_data_relay",
     "xarray-leaflet": "xarray_leaflet",
     "xarray-mongodb": "xarray_mongodb",
     "xgboost-ray": "xgboost_ray",
     "xxhash": "python-xxhash",
     "yggdrasil-framework": "yggdrasil",
     "yoda-tools": "yodatools",
+    "zabbix-utils": "zabbix_utils",
     "zc-buildout": "zc.buildout",
     "zc-lockfile": "zc.lockfile",
     "zc-recipe-egg": "zc.recipe.egg",
     "zenodo-backpack": "zenodo_backpack",
     "zenodo-get": "zenodo_get",
     "zerorpc": "zerorpc-python",
     "zest-releaser": "zest.releaser",
```

### Comparing `whl2conda-24.4.0/src/whl2conda/api/stdrename.py` & `whl2conda-24.5.0/src/whl2conda/api/stdrename.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/cli/__init__.py` & `whl2conda-24.5.0/src/whl2conda/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/cli/build.py` & `whl2conda-24.5.0/src/whl2conda/cli/build.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/cli/common.py` & `whl2conda-24.5.0/src/whl2conda/cli/common.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/cli/convert.py` & `whl2conda-24.5.0/src/whl2conda/cli/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,37 +18,39 @@
 
 # standard lib
 import argparse
 import logging
 import subprocess
 import tempfile
 import time
+import sys
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Sequence
 
 # this project
 from ..impl.download import download_wheel
 from ..impl.prompt import is_interactive, choose_wheel
 from ..api.converter import Wheel2CondaConverter, CondaPackageFormat, DependencyRename
 from ..impl.pyproject import read_pyproject, PyProjInfo
+from ..settings import settings
 from .common import (
     add_markdown_help,
     dedent,
     existing_path,
     existing_dir,
     maybe_existing_dir,
 )
 
 __all__ = ["convert_main"]
 
 
 # pylint: disable=too-many-instance-attributes
 @dataclass
-class Whl2CondaArgs:
+class ConvertArgs:
     """
     Parsed arguments
     """
 
     build_number: Optional[int]
     build_wheel: bool
     dep_renames: Sequence[tuple[str, str]]
@@ -63,14 +65,15 @@
     name: str
     out_dir: Optional[Path]
     out_format: str
     overwrite: bool
     project_root: Optional[Path]
     python: str
     quiet: int
+    update_stdrenames: bool
     verbose: int
     wheel_dir: Optional[Path]
     wheel_or_root: Optional[Path]
     yes: bool
 
 
 def _create_argparser(prog: Optional[str] = None) -> argparse.ArgumentParser:
@@ -157,14 +160,33 @@
 
     input_opts.add_argument(
         "--ignore-pyproject",
         action="store_true",
         help="Ignore settings from pyproject.toml file, if any",
     )
 
+    if sys.version_info < (3, 9):
+        # TODO: drop when python 3.8 support is discontinued
+        input_opts.add_argument(
+            "--update-stdrenames",
+            action="store_true",
+            default=settings.auto_update_std_renames,
+            help="Update list of standard pypi to conda renames from internet.",
+        )
+    else:
+        input_opts.add_argument(
+            "--update-stdrenames",
+            action=argparse.BooleanOptionalAction,
+            default=settings.auto_update_std_renames,
+            help=dedent("""
+                Whether to update list of standard pypi to conda renames from internet. 
+                Default from settings: %(default)s
+                """),
+        )
+
     output_opts.add_argument(
         "--out-dir",
         "--out",
         dest="out_dir",
         metavar="<dir>",
         type=maybe_existing_dir,
         help=dedent("""
@@ -299,17 +321,17 @@
     add_markdown_help(info_opts)
 
     return parser
 
 
 def _parse_args(
     parser: argparse.ArgumentParser, args: Optional[Sequence[str]]
-) -> Whl2CondaArgs:
+) -> ConvertArgs:
     """Parse and return arguments"""
-    return Whl2CondaArgs(**vars(parser.parse_args(args)))
+    return ConvertArgs(**vars(parser.parse_args(args)))
 
 
 def _is_project_root(path: Path) -> bool:
     return any(path.joinpath(f).is_file() for f in ["pyproject.toml", "setup.py"])
 
 
 # pylint: disable=too-many-statements,too-many-branches,too-many-locals
@@ -448,15 +470,15 @@
         elif fmtname in ("V2", "conda"):
             out_fmt = CondaPackageFormat.V2
         else:
             out_fmt = CondaPackageFormat.TREE
     elif pyproj_info.conda_format:
         out_fmt = pyproj_info.conda_format
     else:
-        out_fmt = CondaPackageFormat.V2
+        out_fmt = settings.conda_format
 
     if verbosity < -1:
         level = logging.ERROR
     elif verbosity < 0:
         level = logging.WARNING
     elif verbosity == 0:
         level = logging.INFO
@@ -486,15 +508,19 @@
                     no_deps=build_no_deps,
                     dry_run=dry_run,
                     capture_output=level > logging.INFO,
                 )
 
         assert wheel_file
 
-        converter = Wheel2CondaConverter(wheel_file, out_dir)
+        converter = Wheel2CondaConverter(
+            wheel_file,
+            out_dir,
+            update_std_renames=parsed.update_stdrenames,
+        )
         converter.dry_run = parsed.dry_run
         converter.package_name = (
             parsed.name or pyproj_info.conda_name or pyproj_info.name
         )
         converter.out_format = out_fmt
         converter.overwrite = parsed.overwrite
         converter.keep_pip_dependencies = parsed.keep_pip_deps
```

### Comparing `whl2conda-24.4.0/src/whl2conda/cli/diff.py` & `whl2conda-24.5.0/src/whl2conda/cli/diff.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/cli/install.py` & `whl2conda-24.5.0/src/whl2conda/cli/install.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/cli/main.py` & `whl2conda-24.5.0/src/whl2conda/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2023 Christopher Barber
+#  Copyright 2023-2024 Christopher Barber
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,18 +16,20 @@
 Main whl2conda CLI
 """
 
 from __future__ import annotations
 
 import argparse
 import sys
+from pathlib import Path
 from typing import Optional, Sequence
 
 from ..__about__ import __version__
 from .common import dedent, Subcommands, add_markdown_help
+from ..settings import settings
 
 __all__ = ["main"]
 
 
 def main(args: Optional[Sequence[str]] = None, prog: Optional[str] = None) -> None:
     """
     Main command line interface for whl2conda
@@ -79,17 +81,26 @@
             print(" ".join(subcmds.subcommands))
             sys.exit(0)
 
     parser.add_argument(
         "--list-subcommands", action=ListSubcommands, nargs=0, help=argparse.SUPPRESS
     )
 
+    parser.add_argument(
+        "--settings",
+        metavar="<filepath>",
+        help="Override default settings file",
+    )
+
     add_markdown_help(parser)
     parser.add_argument("--version", action="version", version=__version__)
 
     parsed = parser.parse_args(args)
 
+    if parsed.settings:
+        settings.load(Path(parsed.settings).expanduser())
+
     subcmds.run(parsed)
 
 
 if __name__ == "__main__":  # pragma: no cover
     main()
```

### Comparing `whl2conda-24.4.0/src/whl2conda/external/__init__.py` & `whl2conda-24.5.0/src/whl2conda/external/__init__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/external/version.py` & `whl2conda-24.5.0/src/whl2conda/external/version.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/impl/__init__.py` & `whl2conda-24.5.0/src/whl2conda/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/impl/download.py` & `whl2conda-24.5.0/src/whl2conda/impl/download.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,26 +14,54 @@
 #
 """
 Support for downloading wheels
 """
 
 from __future__ import annotations
 
+import configparser
 import shutil
 import subprocess
 import sys
 import tempfile
 from pathlib import Path
 from typing import Optional
 
+from ..settings import settings
+
 __all__ = [
     "download_wheel",
+    "lookup_pypi_index",
 ]
 
 
+def lookup_pypi_index(index: str) -> str:
+    """
+    Translate index aliases
+
+    First looks for exact match in user settings
+    pyproject_indexes table and then looks for
+    matching entry in the ~/.pypirc file.
+
+    Otherwise returns the original string
+    """
+    if new_index := settings.pypi_indexes.get(index):
+        return new_index
+
+    pypirc_path = Path("~/.pypirc").expanduser()
+    if pypirc_path.exists():
+        pypirc = configparser.ConfigParser()
+        pypirc.read(pypirc_path)
+        try:
+            return pypirc[index]["repository"]
+        except Exception:
+            pass
+    return index
+
+
 def download_wheel(
     spec: str,
     index: str = "",
     into: Optional[Path] = None,
 ) -> Path:
     """
     Downloads wheel with given specification from pypi index.
@@ -58,14 +86,16 @@
             ":all:",
             "--no-deps",
             "--ignore-requires-python",  # TODO: support specific python version
             "--implementation",
             "py",
         ]
         if index:
+            index = lookup_pypi_index(index)
+        if index:
             cmd.extend(["-i", index])
         cmd.extend(["-d", str(tmpdirname)])
         cmd.append(spec)
 
         p = subprocess.run(cmd, check=True, stderr=subprocess.PIPE)
         if p.stderr:
             print(p.stderr, file=sys.stderr)
```

### Comparing `whl2conda-24.4.0/src/whl2conda/impl/prompt.py` & `whl2conda-24.5.0/src/whl2conda/impl/prompt.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/src/whl2conda/impl/pyproject.py` & `whl2conda-24.5.0/src/whl2conda/impl/pyproject.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "CondaPackageFormat",
     "PyProjInfo",
     "add_pyproject_defaults",
     "read_pyproject",
 ]
 
 
-class CondaPackageFormat(enum.Enum):
+class CondaPackageFormat(str, enum.Enum):
     """
     Supported output package formats
 
     * V1: original conda format as .tar.bz2 file
     * V2: newer .conda format
     * TREE: dumps package out as a directory tree (for debugging)
     """
```

### Comparing `whl2conda-24.4.0/src/whl2conda/impl/wheel.py` & `whl2conda-24.5.0/src/whl2conda/impl/wheel.py`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/LICENSE.md` & `whl2conda-24.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/README.md` & `whl2conda-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `whl2conda-24.4.0/pyproject.toml` & `whl2conda-24.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -51,14 +51,29 @@
 [tool.hatch.version]
 path = "src/whl2conda/VERSION"
 pattern = "\\s*(?P<version>[\\w.]*)"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/whl2conda"]
 
+# TODO: Using coverage config in pyproject is resulting in
+#    INTERNALERROR> coverage.exceptions.DataError: Can't combine line data with arc data
+#
+#[tool.coverage.run]
+#branch = true
+#
+#[tool.coverage.report]
+#include = ["src/whl2conda/*"]
+#omit = ["src/whl2conda/external/*"]
+#exclude_also = [
+#    "pragma: no cover",
+#    "raise AssertionError",
+#    "raise NotImplementedError"
+#]
+
 [tool.black]
 line-length = 88
 skip-string-normalization = true
 
 [tool.mypy]
 check_untyped_defs = true
 mypy_path = "src"
```

### Comparing `whl2conda-24.4.0/PKG-INFO` & `whl2conda-24.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: whl2conda
-Version: 24.4.0
+Version: 24.5.0
 Summary: Build conda packages directly from pure python wheels
 Project-URL: homepage, https://github.com/analog-cbarber/whl2conda
 Project-URL: repository, https://github.com/analog-cbarber/whl2conda
 Project-URL: documentation, https://zuzukin.github.io/whl2conda/
 Author-email: Christopher Barber <christopher.barber@analog.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
```

