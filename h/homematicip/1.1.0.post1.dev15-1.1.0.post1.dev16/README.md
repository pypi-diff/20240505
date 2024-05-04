# Comparing `tmp/homematicip-1.1.0.post1.dev15.tar.gz` & `tmp/homematicip-1.1.0.post1.dev16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homematicip-1.1.0.post1.dev15.tar", last modified: Fri May  3 15:09:33 2024, max compression
+gzip compressed data, was "homematicip-1.1.0.post1.dev16.tar", last modified: Sat May  4 22:36:10 2024, max compression
```

## Comparing `homematicip-1.1.0.post1.dev15.tar` & `homematicip-1.1.0.post1.dev16.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.621180 homematicip-1.1.0.post1.dev15/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.629180 homematicip-1.1.0.post1.dev15/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.github/workflows/test-on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.629180 homematicip-1.1.0.post1.dev15/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.629180 homematicip-1.1.0.post1.dev15/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.629180 homematicip-1.1.0.post1.dev15/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/api_introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/gettingstarted.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/homematicip.aio.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/homematicip.base.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/homematicip.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/requirements_docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.621180 homematicip-1.1.0.post1.dev15/sample_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.633180 homematicip-1.1.0.post1.dev15/sample_data/json_data/
--rw-r--r--   0 runner    (1001) docker     (127)   524183 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/sample_data/json_data/home.json
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/sample_data/json_data/security_journal.json
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/sample_data/json_data/unknown_types.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.625180 homematicip-1.1.0.post1.dev15/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.633180 homematicip-1.1.0.post1.dev15/src/homematicip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.633180 homematicip-1.1.0.post1.dev15/src/homematicip/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/action/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/action/action_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/action/functional_channel_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/action/group_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.637180 homematicip-1.1.0.post1.dev15/src/homematicip/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44048 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/cli/hmip_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/cli/hmip_cli_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/cli/hmip_cli_debug_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.637180 homematicip-1.1.0.post1.dev15/src/homematicip/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/configuration/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/configuration/config_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/configuration/log_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.637180 homematicip-1.1.0.post1.dev15/src/homematicip/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/connection/client_characteristics_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/connection/client_token_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/connection/rest_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.637180 homematicip-1.1.0.post1.dev15/src/homematicip/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/events/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/events/event_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/events/hmip_event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.637180 homematicip-1.1.0.post1.dev15/src/homematicip/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/exceptions/config_not_found_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/src/homematicip/model/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/anoymizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    52256 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/functional_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/hmip_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/home.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/src/homematicip/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-03 15:09:33.000000 homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/actions/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/actions/test_action_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/actions/test_group_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/tests/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/connection/test_client_characteristics_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/connection/test_rest_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/tests/events/
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/events/test_hmip_event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:09:33.641180 homematicip-1.1.0.post1.dev15/tests/model/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/model/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/model/test_functional_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-03 15:09:23.000000 homematicip-1.1.0.post1.dev15/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.545278 homematicip-1.1.0.post1.dev16/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.525278 homematicip-1.1.0.post1.dev16/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.529278 homematicip-1.1.0.post1.dev16/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.github/workflows/test-on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22313 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.529278 homematicip-1.1.0.post1.dev16/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.533278 homematicip-1.1.0.post1.dev16/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.533278 homematicip-1.1.0.post1.dev16/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/api_introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/gettingstarted.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/homematicip.aio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/homematicip.base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/homematicip.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/requirements_docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.525278 homematicip-1.1.0.post1.dev16/sample_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.533278 homematicip-1.1.0.post1.dev16/sample_data/json_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   524183 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/sample_data/json_data/home.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/sample_data/json_data/security_journal.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/sample_data/json_data/unknown_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 22:36:10.545278 homematicip-1.1.0.post1.dev16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.525278 homematicip-1.1.0.post1.dev16/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.533278 homematicip-1.1.0.post1.dev16/src/homematicip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/action/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/action/action_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/action/functional_channel_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/action/group_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/cli/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40262 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/cli/hmip_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/cli/hmip_cli_debug_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/configuration/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/configuration/config_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/configuration/log_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/connection/client_characteristics_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/connection/client_token_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/connection/rest_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/events/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/events/event_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/events/hmip_event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.537278 homematicip-1.1.0.post1.dev16/src/homematicip/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/exceptions/config_not_found_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/src/homematicip/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/anoymizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52256 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/functional_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/hmip_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/src/homematicip/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 22:36:10.000000 homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/actions/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/actions/test_action_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/actions/test_functional_channel_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/actions/test_group_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/tests/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/connection/test_client_characteristics_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/connection/test_rest_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/events/test_hmip_event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:36:10.541278 homematicip-1.1.0.post1.dev16/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/model/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/model/test_functional_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-04 22:35:57.000000 homematicip-1.1.0.post1.dev16/tests/test_runner.py
```

### Comparing `homematicip-1.1.0.post1.dev15/.github/workflows/build-docs.yml` & `homematicip-1.1.0.post1.dev16/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/.github/workflows/codeql-analysis.yml` & `homematicip-1.1.0.post1.dev16/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/.github/workflows/publish.yml` & `homematicip-1.1.0.post1.dev16/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/.github/workflows/test-on-push.yml` & `homematicip-1.1.0.post1.dev16/.github/workflows/test-on-push.yml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/.gitignore` & `homematicip-1.1.0.post1.dev16/.gitignore`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/CHANGELOG.md` & `homematicip-1.1.0.post1.dev16/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/CODE_OF_CONDUCT.md` & `homematicip-1.1.0.post1.dev16/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/LICENSE.txt` & `homematicip-1.1.0.post1.dev16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/PKG-INFO` & `homematicip-1.1.0.post1.dev16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homematicip
-Version: 1.1.0.post1.dev15
+Version: 1.1.0.post1.dev16
 Summary: An API for the homematicip cloud
 Author-email: Thomas Hahn <homematicip-rest-api@outlook.com>
 Project-URL: Homepage, https://github.com/hahn-th/homematicip-rest-api
 Project-URL: Repository, https://github.com/hahn-th/homematicip-rest-api.git
 Project-URL: Issues, https://github.com/hahn-th/homematicip-rest-api/issues
 Project-URL: Changelog, https://github.com/hahn-th/homematicip-rest-api/blob/master/CHANGELOG.md
 Keywords: homematicip cloud,homematicip
```

### Comparing `homematicip-1.1.0.post1.dev15/README.md` & `homematicip-1.1.0.post1.dev16/README.md`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/docs/Makefile` & `homematicip-1.1.0.post1.dev16/docs/Makefile`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/docs/make.bat` & `homematicip-1.1.0.post1.dev16/docs/make.bat`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/docs/source/api_introduction.rst` & `homematicip-1.1.0.post1.dev16/docs/source/api_introduction.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/docs/source/conf.py` & `homematicip-1.1.0.post1.dev16/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/docs/source/gettingstarted.rst` & `homematicip-1.1.0.post1.dev16/docs/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/docs/source/homematicip.aio.rst` & `homematicip-1.1.0.post1.dev16/docs/source/homematicip.aio.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/docs/source/homematicip.base.rst` & `homematicip-1.1.0.post1.dev16/docs/source/homematicip.base.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/docs/source/homematicip.rst` & `homematicip-1.1.0.post1.dev16/docs/source/homematicip.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/docs/source/index.rst` & `homematicip-1.1.0.post1.dev16/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/pyproject.toml` & `homematicip-1.1.0.post1.dev16/pyproject.toml`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/sample_data/json_data/home.json` & `homematicip-1.1.0.post1.dev16/sample_data/json_data/home.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/sample_data/json_data/security_journal.json` & `homematicip-1.1.0.post1.dev16/sample_data/json_data/security_journal.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/sample_data/json_data/unknown_types.json` & `homematicip-1.1.0.post1.dev16/sample_data/json_data/unknown_types.json`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/action/action.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/action/action.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/action/action_registry.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/action/action_registry.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/action/group_actions.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/action/group_actions.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/auth.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/auth.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/cli/hmip_cli.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/cli/hmip_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 
 import click
 import httpx
 from alive_progress import alive_bar
 from click import ClickException
 
 from homematicip.action.functional_channel_actions import action_set_slats_level, action_set_shutter_level, \
-    action_set_switch_state
+    action_set_switch_state, action_set_dim_level, action_start_impulse
 from homematicip.action.group_actions import action_set_boost, action_set_point_temperature, action_set_boost_duration, \
     action_set_active_profile, action_set_control_mode
 from homematicip.auth import Auth
-from homematicip.cli.hmip_cli_actions import get_rssi_bar_string
+from homematicip.cli.helper import get_channel_by_index_of_first
+from homematicip.cli.helper import get_rssi_bar_string
 from homematicip.configuration.config import Config, PersistentConfig
 from homematicip.configuration.config_io import ConfigIO
 from homematicip.configuration.log_helper import get_logger_filename
-from homematicip.connection.client_characteristics_builder import ClientCharacteristicsBuilder
-from homematicip.connection.client_token_builder import ClientTokenBuilder
-from homematicip.connection.rest_connection import ConnectionContext, RestResult, ConnectionUrlResolver
+from homematicip.connection.rest_connection import ConnectionContext, RestResult
 from homematicip.model.anoymizer import handle_config
 from homematicip.model.enums import ClimateControlMode
 from homematicip.runner import Runner
 
 
 async def get_initialized_runner(including_model: bool = True) -> Runner:
     config = get_config()
@@ -182,15 +181,15 @@
 def list():
     """List information about devices, groups, rssi, firmware, profiles."""
     pass
 
 
 @list.command()
 def devices():
-    """List all devices."""
+    """List all devices including the functional channels."""
     runner = asyncio.run(get_initialized_runner())
     model = runner.model
     print("Devices:")
     for device in sorted(model.devices.values(), key=lambda x: x.label):
         click.echo(f"\t({device.id}) - {device.label} - {device.type}")
 
         for channel in device.functionalChannels.values():
@@ -228,17 +227,17 @@
         if hasattr(fc, "rssiPeerValue"):
             rssi_peer_value = fc.rssiPeerValue
         if hasattr(fc, "unreach"):
             unreach = fc.unreach
         click.echo(
             "{:45s} - RSSI: {:4} {} - Peer RSSI: {:4} - {} {} permanentlyReachable: {}".format(
                 d.label,
-                rssi_device_value if rssi_device_value else 0,
+                rssi_device_value or "?",
                 get_rssi_bar_string(rssi_device_value),
-                rssi_peer_value if rssi_peer_value else 0,
+                rssi_peer_value or "?",
                 get_rssi_bar_string(rssi_peer_value),
                 "Unreachable" if unreach else "",
                 d.permanentlyReachable,
             )
         )
 
 
@@ -275,14 +274,44 @@
         return
 
     for pid, profile in group.profiles.items():
         click.echo(
             f"\t({profile['index']}) - {profile['name'] or "None"} - Visible: {profile['visible']} Enabled: {profile['enabled']}")
 
 
+@list.command
+def last_status_update():
+    """List the last status update for devices and groups."""
+    runner = asyncio.run(get_initialized_runner())
+    model = runner.model
+    click.echo("Devices:")
+    for device in sorted(model.devices.values(), key=lambda x: x.label):
+        click.echo(f"\t{device.id}\t{device.label:30s}\t{device.lastStatusUpdate}")
+
+    click.echo("Groups:")
+    for group in sorted(model.groups.values(), key=lambda x: x.label):
+        click.echo(f"\t{group.id}\t{group.label:30s}\t{group.lastStatusUpdate}")
+
+    return True
+
+
+@list.command
+def firmware():
+    """List current and available firmware information."""
+    runner = asyncio.run(get_initialized_runner())
+    model = runner.model
+    home = model.home
+    click.echo(
+        f"{"HmIP AccessPoint":30s} - Firmware: {home.currentAPVersion or "<unknown>":7} - Available Firmware: {home.availableAPVersion or "<unknown>":7} UpdateState: {home.updateState}")
+
+    for device in sorted(model.devices.values(), key=lambda x: x.label):
+        click.echo(
+            f"{device.label:30s} - Firmware: {device.firmwareVersion or "<unknown>":7} - Available Firmware: {device.availableFirmwareVersion or "<unknown>":7} UpdateState: {device.updateState} LiveUpdateState: {device.liveUpdateState}")
+
+
 @cli.group
 def run():
     """Run actions on devices, groups, home or functional channels."""
     pass
 
 
 @run.command
@@ -498,172 +527,81 @@
         return
 
     result = asyncio.run(action_set_control_mode(runner, runner.model.groups[id], control_mode))
     click.echo(
         f"Run set_control_mode for group {runner.model.groups[id].label or runner.model.groups[id].id} with "
         f"result: {result.status_text} ({result.status})")
 
-# import asyncio
-# import json
-# import logging
-# import signal
-# import sys
-# import time
-# import traceback
-# from argparse import ArgumentParser, RawDescriptionHelpFormatter
-# from importlib.metadata import version
-# from logging.handlers import TimedRotatingFileHandler
-#
-# from devtools import pprint
-#
-# from homematicip.cli.cli_args_parser import get_parser, get_args
-# from homematicip.cli.hmip_cli_actions import handle_list_last_status_update, handle_list_groups, handle_list_devices, \
-#     handle_list_group_ids, handle_list_rssi
-# from homematicip.configuration.config import PersistentConfig, Config
-# from homematicip.configuration.load_config import ConfigLoader
-# from homematicip.events.event_manager import EventManager
-# from homematicip.events.event_types import ModelUpdateEvent
-# from homematicip.runner import Runner
-#
-#
-# # args auswerten
-# # runner initialisieren
-# # config setzen oder lesen
-# #  -> exception, falls nicht gefunden
-# # events registrieren
-#
-#
-# def main(args=None):
-#     """Entry point for hmip_cli.
-#
-#     The setup_py entry_point wraps this in sys.exit already so this effectively
-#     becomes sys.exit(main()).
-#     The __main__ entry point similarly wraps sys.exit().
-#     """
-#     if args is None:
-#         args = sys.argv[1:]
-#
-#     parser = get_parser()
-#     parsed_args = get_args(parser, args)
-#
-#     if len(sys.argv) == 1:
-#         parser.print_help()
-#         return
-#
-#     try:
-#         asyncio.run(run_cli(parsed_args))
-#
-#     except KeyboardInterrupt:
-#         # Shell standard is 128 + signum = 130 (SIGINT = 2)
-#         sys.stdout.write("\n")
-#         return 128 + signal.SIGINT
-#     except Exception as e:
-#         # stderr and exit code 255
-#         sys.stderr.write("\n")
-#         sys.stderr.write(f"\033[91m{type(e).__name__}: {str(e)}\033[0;0m")
-#         sys.stderr.write("\n")
-#         # at this point, you're guaranteed to have args and thus log_level
-#         if parsed_args.debug_level:
-#             if parsed_args.debug_level < 10:
-#                 # traceback prints to stderr by default
-#                 traceback.print_exc()
-#
-#         return 255
-#
-#
-# async def run_cli(parsed_args):
-#     """Run the cli with the parsed args."""
-#     config = get_config(parsed_args)
-#
-#     logger = _setup_logger(
-#         config.level, parsed_args.debug_level, config.log_file
-#     )
-#     runner = Runner(_config=config)
-#     await runner.async_initialize_runner()
-#     await run(runner, parsed_args)
-#
-#
-# def get_config(parsed_args) -> Config:
-#     if parsed_args.config_file:
-#         config = ConfigLoader.from_file(parsed_args.config_file)
-#     else:
-#         config = ConfigLoader.find_config_in_well_known_locations()
-#
-#     if config is None:
-#         print("No configuration file found. Run hmip_generate_auth_token or use -c or --config-file argument to "
-#               "specify a configuration file.")
-#         sys.exit(-1)
-#
-#     return Config.from_persistent_config(config)
-#
-#
-# def _setup_logger(
-#         default_debug_level: int, argument_debug_level: int, log_file: str
-# ) -> logging.Logger:
-#     """Initialize logger. If log_file is set, log to file, otherwise to stdout. The log level """
-#     debug_level = argument_debug_level if argument_debug_level else default_debug_level
-#     logging.basicConfig(level=debug_level)
-#
-#     logger = _create_logger(debug_level, log_file)
-#     return logger
-#
-#
-# def _create_logger(level: int, file_name: str) -> logging.Logger:
-#     """Create a logger based on the level"""
-#     logger = logging.getLogger()
-#     logger.setLevel(level)
-#     handler = (
-#         TimedRotatingFileHandler(file_name, when="midnight", backupCount=5)
-#         if file_name
-#         else logging.StreamHandler()
-#     )
-#     handler.setFormatter(
-#         logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-#     )
-#     logger.addHandler(handler)
-#     return logger
-#
-#
-# async def run(runner: Runner, args):
-#     """Execution of cli commands with parsed args."""
-#     command_entered = False
-#     if args.listen:
-#         print("Listening for events. Press Ctrl+C to stop.")
-#         register_events(runner.event_manager)
-#         await runner.async_listening_for_updates()
-#
-#     # if args.server_config:
-#     #     print(
-#     #         f"Running homematicip-rest-api with fake server configuration {args.server_config}"
-#     #     )
-#     #     global server_config
-#     #     server_config = args.server_config
-#     #     home.download_configuration = fake_download_configuration
-#
-#     if args.dump_config:
-#         pass
-#         # command_entered = True
-#         # json_state = home.download_configuration()
-#         #
-#         # output = handle_config(json_state, args.anonymize)
-#         # if output:
-#         #     print(output)
-#
-#     if args.list_devices:
-#         command_entered = handle_list_devices(runner.model)
-#
-#     if args.list_groups:
-#         command_entered = handle_list_groups(runner.model)
-#
-#     if args.list_last_status_update:
-#         command_entered = handle_list_last_status_update(runner.model)
-#
-#     if args.list_group_ids:
-#         command_entered = handle_list_group_ids(runner.model)
-#
+
+@run.command
+@click.argument("id", type=str, nargs=1)
+@click.argument("dim_level", type=click.FloatRange(0.0, 1.0), nargs=1)
+@click.argument("channel", type=int, nargs=1)
+def set_dim_level(id: str, dim_level: float, channel: int = None):
+    """Set the dim level for a device.
+
+    ID is the Id of the device. Use 'list devices' to get desired Id.\n
+    DIM_LEVEL is the target dim level. Must be between 0.0 and 1.0.\n
+    CHANNEL is the channel index of the device. If the device has only one channel (excl. BaseChannel 0) this can be omitted.
+    """
+    runner = asyncio.run(get_initialized_runner())
+    model = runner.model
+
+    if id not in model.devices:
+        click.echo(f"Device with id {id} not found.", err=True, color=True)
+        return
+
+    device = model.devices[id]
+    fc = get_channel_by_index_of_first(device, channel)
+
+    if fc is None:
+        click.echo(f"Channel with index {channel} not found.", err=True, color=True)
+        return
+    result = asyncio.run(action_set_dim_level(runner, fc, dim_level))
+    click.echo(
+        f"Run set_dim_level for device {device.label or device.id} and channel {fc.index} with result: {result.status_text} ({result.status})")
+
+
+@run.command
+def toggle_garage_door(id: str, channel: int = None):
+    """Toggle the garage door.
+
+    ID is the Id of the device. Use 'list devices' to get desired Id."""
+    runner = asyncio.run(get_initialized_runner())
+    model = runner.model
+
+    if id not in model.devices:
+        click.echo(f"Device with id {id} not found.", err=True, color=True)
+        return
+
+    device = model.devices[id]
+    fc = get_channel_by_index_of_first(device, channel)
+    result = asyncio.run(action_start_impulse(runner, fc))
+    click.echo(
+        f"Run toggle_garage_door for device {device.label or device.id} with result: {result.status_text} ({result.status})")
+
+#     #         if args.toggle_garage_door is not None:
+#     #             _execute_action_for_device(
+#     #                 device,
+#     #                 args,
+#     #                 CliActions.TOGGLE_GARAGE_DOOR,
+#     #                 "send_start_impulse",
+#     #             )
+#     #             command_entered = True
+#     #
+#     #         if args.device_send_door_command is not None:
+#     #             _execute_action_for_device(
+#     #                 device,
+#     #                 args,
+#     #                 CliActions.SEND_DOOR_COMMAND,
+#     #                 "send_door_command",
+#     #                 args.device_send_door_command,
+#     #             )
+#     #             command_entered = True
+
 #     # if args.protectionmode:
 #     #     command_entered = True
 #     #     if args.protectionmode == "presence":
 #     #         home.set_security_zones_activation(False, True)
 #     #     elif args.protectionmode == "absence":
 #     #         home.set_security_zones_activation(True, True)
 #     #     elif args.protectionmode == "disable":
@@ -678,42 +616,16 @@
 #     #
 #     # if args.list_security_journal:
 #     #     command_entered = True
 #     #     journal = home.get_security_journal()
 #     #     for entry in journal:
 #     #         print(entry)
 #     #
-#     # if args.list_firmware:
-#     #     command_entered = True
-#     #     print(
-#     #         "{:45s} - Firmware: {:6} - Available Firmware: {:6} UpdateState: {}".format(
-#     #             "HmIP AccessPoint",
-#     #             home.currentAPVersion if home.currentAPVersion is not None else "None",
-#     #             home.availableAPVersion
-#     #             if home.availableAPVersion is not None
-#     #             else "None",
-#     #             home.updateState,
-#     #         )
-#     #     )
-#     #     sortedDevices = sorted(home.devices, key=attrgetter("deviceType", "label"))
-#     #     for d in sortedDevices:
-#     #         print(
-#     #             "{:45s} - Firmware: {:6} - Available Firmware: {:6} UpdateState: {} LiveUpdateState: {}".format(
-#     #                 d.label,
-#     #                 d.firmwareVersion,
-#     #                 d.availableFirmwareVersion
-#     #                 if d.availableFirmwareVersion is not None
-#     #                 else "None",
-#     #                 d.updateState,
-#     #                 d.liveUpdateState,
-#     #             )
-#     #         )
 #     #
-#     if args.list_rssi:
-#         command_entered = handle_list_rssi(runner.model)
+
 #
 #     # if args.list_rules:
 #     #     command_entered = True
 #     #     sortedRules = sorted(home.rules, key=attrgetter("ruleType", "label"))
 #     #     for d in sortedRules:
 #     #         print("{} {}".format(d.id, str(d)))
 #     #
@@ -742,24 +654,14 @@
 #     #                 args,
 #     #                 CliActions.SET_SWITCH_STATE,
 #     #                 "set_switch_state",
 #     #                 args.device_switch_state,
 #     #             )
 #     #             command_entered = True
 #     #
-#     #         if args.device_dim_level is not None:
-#     #             _execute_action_for_device(
-#     #                 device,
-#     #                 args,
-#     #                 CliActions.SET_DIM_LEVEL,
-#     #                 "set_dim_level",
-#     #                 args.device_dim_level,
-#     #             )
-#     #             command_entered = True
-#     #
 #     #         if args.device_set_lock_state is not None:
 #     #             targetLockState = LockState.from_str(args.device_set_lock_state)
 #     #             if targetLockState not in LockState:
 #     #                 logger.error("%s is not a lock state.", args.device_set_lock_state)
 #     #
 #     #             else:
 #     #                 pin = args.pin[0] if len(args.pin) > 0 else ""
@@ -769,32 +671,14 @@
 #     #                     CliActions.SET_LOCK_STATE,
 #     #                     "set_lock_state",
 #     #                     targetLockState,
 #     #                     pin,
 #     #                 )
 #     #             command_entered = True
 #     #
-#     #         if args.toggle_garage_door is not None:
-#     #             _execute_action_for_device(
-#     #                 device,
-#     #                 args,
-#     #                 CliActions.TOGGLE_GARAGE_DOOR,
-#     #                 "send_start_impulse",
-#     #             )
-#     #             command_entered = True
-#     #
-#     #         if args.device_send_door_command is not None:
-#     #             _execute_action_for_device(
-#     #                 device,
-#     #                 args,
-#     #                 CliActions.SEND_DOOR_COMMAND,
-#     #                 "send_door_command",
-#     #                 args.device_send_door_command,
-#     #             )
-#     #             command_entered = True
 #     #
 #     #         if args.device_shutter_level is not None:
 #     #             _execute_action_for_device(
 #     #                 device,
 #     #                 args,
 #     #                 CliActions.SET_SHUTTER_LEVEL,
 #     #                 "set_shutter_level",
```

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/configuration/config.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/configuration/config.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/configuration/config_io.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/configuration/config_io.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/configuration/log_helper.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/configuration/log_helper.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/connection/client_characteristics_builder.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/connection/client_characteristics_builder.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/connection/rest_connection.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/connection/rest_connection.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/events/event_manager.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/events/hmip_event_handler.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/events/hmip_event_handler.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/model/anoymizer.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/model/anoymizer.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/model/devices.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/model/devices.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/model/enums.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/model/enums.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/model/functional_channels.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/model/functional_channels.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/model/home.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/model/home.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip/runner.py` & `homematicip-1.1.0.post1.dev16/src/homematicip/runner.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/PKG-INFO` & `homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homematicip
-Version: 1.1.0.post1.dev15
+Version: 1.1.0.post1.dev16
 Summary: An API for the homematicip cloud
 Author-email: Thomas Hahn <homematicip-rest-api@outlook.com>
 Project-URL: Homepage, https://github.com/hahn-th/homematicip-rest-api
 Project-URL: Repository, https://github.com/hahn-th/homematicip-rest-api.git
 Project-URL: Issues, https://github.com/hahn-th/homematicip-rest-api/issues
 Project-URL: Changelog, https://github.com/hahn-th/homematicip-rest-api/blob/master/CHANGELOG.md
 Keywords: homematicip cloud,homematicip
```

### Comparing `homematicip-1.1.0.post1.dev15/src/homematicip.egg-info/SOURCES.txt` & `homematicip-1.1.0.post1.dev16/src/homematicip.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 src/homematicip.egg-info/top_level.txt
 src/homematicip/action/__init__.py
 src/homematicip/action/action.py
 src/homematicip/action/action_registry.py
 src/homematicip/action/functional_channel_actions.py
 src/homematicip/action/group_actions.py
 src/homematicip/cli/__init__.py
+src/homematicip/cli/helper.py
 src/homematicip/cli/hmip_cli.py
-src/homematicip/cli/hmip_cli_actions.py
 src/homematicip/cli/hmip_cli_debug_wrapper.py
 src/homematicip/configuration/__init__.py
 src/homematicip/configuration/config.py
 src/homematicip/configuration/config_io.py
 src/homematicip/configuration/log_helper.py
 src/homematicip/connection/__init__.py
 src/homematicip/connection/client_characteristics_builder.py
@@ -75,14 +75,15 @@
 src/homematicip/model/home.py
 src/homematicip/model/model.py
 tests/conftest.py
 tests/test_auth.py
 tests/test_runner.py
 tests/actions/conftest.py
 tests/actions/test_action_decorator.py
+tests/actions/test_functional_channel_actions.py
 tests/actions/test_group_actions.py
 tests/connection/test_client_characteristics_builder.py
 tests/connection/test_rest_connection.py
 tests/events/test_hmip_event_handler.py
 tests/model/conftest.py
 tests/model/test_functional_channel.py
 tests/model/test_model.py
```

### Comparing `homematicip-1.1.0.post1.dev15/tests/actions/test_action_decorator.py` & `homematicip-1.1.0.post1.dev16/tests/actions/test_action_decorator.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/tests/actions/test_group_actions.py` & `homematicip-1.1.0.post1.dev16/tests/actions/test_group_actions.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/tests/conftest.py` & `homematicip-1.1.0.post1.dev16/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/tests/connection/test_rest_connection.py` & `homematicip-1.1.0.post1.dev16/tests/connection/test_rest_connection.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/tests/events/test_hmip_event_handler.py` & `homematicip-1.1.0.post1.dev16/tests/events/test_hmip_event_handler.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/tests/model/test_model.py` & `homematicip-1.1.0.post1.dev16/tests/model/test_model.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/tests/test_auth.py` & `homematicip-1.1.0.post1.dev16/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `homematicip-1.1.0.post1.dev15/tests/test_runner.py` & `homematicip-1.1.0.post1.dev16/tests/test_runner.py`

 * *Files identical despite different names*

