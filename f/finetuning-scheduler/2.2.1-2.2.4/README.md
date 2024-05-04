# Comparing `tmp/finetuning-scheduler-2.2.1.tar.gz` & `tmp/finetuning_scheduler-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetuning-scheduler-2.2.1.tar", last modified: Mon Mar  4 22:11:31 2024, max compression
+gzip compressed data, was "finetuning_scheduler-2.2.4.tar", last modified: Sat May  4 22:50:28 2024, max compression
```

## Comparing `finetuning-scheduler-2.2.1.tar` & `finetuning_scheduler-2.2.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.924329 finetuning-scheduler-2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.908329 finetuning-scheduler-2.2.1/.actions/
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    18467 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-03-04 22:11:31.924329 finetuning-scheduler-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.912329 finetuning-scheduler-2.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/requirements/cli.txt
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/requirements/devel.txt
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/requirements/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/requirements/extra.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/requirements/ipynb.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/requirements/standalone_base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 22:11:31.924329 finetuning-scheduler-2.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     6973 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.908329 finetuning-scheduler-2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.912329 finetuning-scheduler-2.2.1/src/finetuning_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50091 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/fts.py
--rw-r--r--   0 runner    (1001) docker     (127)   104984 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/fts_supporters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/setup_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.912329 finetuning-scheduler-2.2.1/src/finetuning_scheduler/strategy_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/strategy_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/strategy_adapters/_wrap_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/strategy_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    47391 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/strategy_adapters/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.916329 finetuning-scheduler-2.2.1/src/finetuning_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-03-04 22:11:31.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-03-04 22:11:31.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 22:11:31.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 22:11:31.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-04 22:11:31.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-04 22:11:31.000000 finetuning-scheduler-2.2.1/src/finetuning_scheduler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.912329 finetuning-scheduler-2.2.1/src/fts_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.916329 finetuning-scheduler-2.2.1/src/fts_examples/stable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/cli_experiment_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.916329 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.908329 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.916329 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/fsdp/
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_basic_profile.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.916329 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_lr/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_lr/explicit_reinit_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.916329 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_optim_lr/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_optim_lr/explicit_reinit_optim_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_explicit_reinit_optim_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr_use_curr.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/fts_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/fts_explicit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/fts_implicit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/config/nofts_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/extended_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/src/fts_examples/stable/fts_superglue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:11:31.916329 finetuning-scheduler-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   110254 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/tests/test_finetuning_scheduler_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    42185 2024-03-04 22:11:28.000000 finetuning-scheduler-2.2.1/tests/test_fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.658239 finetuning_scheduler-2.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.646239 finetuning_scheduler-2.2.4/.actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-04 22:50:28.658239 finetuning_scheduler-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.646239 finetuning_scheduler-2.2.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/requirements/cli.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/requirements/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/requirements/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/requirements/extra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/requirements/ipynb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/requirements/standalone_base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 22:50:28.658239 finetuning_scheduler-2.2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6973 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.642239 finetuning_scheduler-2.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.650239 finetuning_scheduler-2.2.4/src/finetuning_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50091 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/fts.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104984 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/fts_supporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/setup_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.650239 finetuning_scheduler-2.2.4/src/finetuning_scheduler/strategy_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/strategy_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/strategy_adapters/_wrap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/strategy_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47391 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/strategy_adapters/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.654239 finetuning_scheduler-2.2.4/src/finetuning_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-04 22:50:28.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-04 22:50:28.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 22:50:28.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 22:50:28.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-04 22:50:28.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-04 22:50:28.000000 finetuning_scheduler-2.2.4/src/finetuning_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.650239 finetuning_scheduler-2.2.4/src/fts_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.650239 finetuning_scheduler-2.2.4/src/fts_examples/stable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/cli_experiment_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.650239 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.646239 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.650239 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/fsdp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_basic_profile.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.654239 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_lr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_lr/explicit_reinit_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.654239 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/explicit_reinit_optim_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_explicit_reinit_optim_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr_use_curr.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/fts_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/fts_explicit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/fts_implicit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/config/nofts_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/extended_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/src/fts_examples/stable/fts_superglue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:50:28.654239 finetuning_scheduler-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   110254 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/tests/test_finetuning_scheduler_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42185 2024-05-04 22:50:23.000000 finetuning_scheduler-2.2.4/tests/test_fsdp.py
```

### Comparing `finetuning-scheduler-2.2.1/.actions/assistant.py` & `finetuning_scheduler-2.2.4/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/CHANGELOG.md` & `finetuning_scheduler-2.2.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [2.2.4] - 2024-05-04
+
+### Added
+
+- Support for Lightning ``2.2.4`` and PyTorch ``2.2.2``
+
 ## [2.2.1] - 2024-03-04
 
 ### Added
 
 - Support for Lightning ``2.2.1``
 
 ## [2.2.0] - 2024-02-08
```

### Comparing `finetuning-scheduler-2.2.1/CITATION.cff` & `finetuning_scheduler-2.2.4/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 message: "If you want to cite this extension, feel free to use this 😊"
 title: "Fine-Tuning Scheduler"
 abstract: "A PyTorch Lightning extension that enhances model experimentation with flexible fine-tuning schedules."
 date-released: 2022-02-04
 authors:
   - family-names: "Dale"
     given-names: "Dan"
-version: 2.2.1
+version: 2.2.4
 identifiers:
   - description: "Fine-Tuning Scheduler (all versions)"
     type: doi
     value: 10.5281/zenodo.6463952
   - description: "Fine-Tuning Scheduler (v0.1.1)"
     type: doi
     value: 10.5281/zenodo.6463992
@@ -103,14 +103,17 @@
     value: 10.5281/zenodo.10420340
   - description: "Fine-Tuning Scheduler (v2.1.4)"
     type: doi
     value: 10.5281/zenodo.10611882
   - description: "Fine-Tuning Scheduler (v2.2.0)"
     type: doi
     value: 10.5281/zenodo.10637464
+  - description: "Fine-Tuning Scheduler (v2.2.1)"
+    type: doi
+    value: 10.5281/zenodo.10780386
 license: "Apache-2.0"
 url: "https://finetuning-scheduler.readthedocs.io/"
 repository-code: "https://github.com/speediedan/finetuning-scheduler"
 keywords:
   - machine learning
   - deep learning
   - artificial intelligence
```

### Comparing `finetuning-scheduler-2.2.1/LICENSE` & `finetuning_scheduler-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/MANIFEST.in` & `finetuning_scheduler-2.2.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/PKG-INFO` & `finetuning_scheduler-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuning-scheduler
-Version: 2.2.1
+Version: 2.2.4
 Summary: A PyTorch Lightning extension that enhances model experimentation with flexible fine-tuning schedules.
 Home-page: https://github.com/speediedan/finetuning-scheduler
 Download-URL: https://github.com/speediedan/finetuning-scheduler
 Author: Dan Dale
 Author-email: danny.dale@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/speediedan/finetuning-scheduler/issues
@@ -24,29 +24,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lightning<2.2.2,>=2.2.0
+Requires-Dist: lightning<2.2.5,>=2.2.0
 Requires-Dist: torch<2.3.0,>=1.13.0
 Provides-Extra: examples
 Requires-Dist: datasets; extra == "examples"
 Requires-Dist: evaluate; extra == "examples"
 Requires-Dist: transformers>=4.18.0; extra == "examples"
 Requires-Dist: scikit-learn; extra == "examples"
 Requires-Dist: sentencepiece; extra == "examples"
 Requires-Dist: tensorboardX>=2.2; extra == "examples"
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "examples"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "examples"
 Requires-Dist: omegaconf>=2.1.0; extra == "examples"
 Requires-Dist: hydra-core>=1.1.0; extra == "examples"
 Provides-Extra: extra
 Requires-Dist: rich>=12.3.0; extra == "extra"
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "extra"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "extra"
 Requires-Dist: omegaconf>=2.1.0; extra == "extra"
 Requires-Dist: hydra-core>=1.1.0; extra == "extra"
 Provides-Extra: test
 Requires-Dist: coverage>=6.4; extra == "test"
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: pytest-rerunfailures>=10.2; extra == "test"
 Requires-Dist: twine==3.2; extra == "test"
@@ -54,35 +54,35 @@
 Requires-Dist: pre-commit>=1.0; extra == "test"
 Requires-Dist: protobuf<=3.20.1; extra == "test"
 Provides-Extra: ipynb
 Requires-Dist: ipython[notebook]; extra == "ipynb"
 Requires-Dist: jupytext>=1.10; extra == "ipynb"
 Requires-Dist: nbval>=0.9.6; extra == "ipynb"
 Provides-Extra: cli
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "cli"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "cli"
 Requires-Dist: omegaconf>=2.1.0; extra == "cli"
 Requires-Dist: hydra-core>=1.1.0; extra == "cli"
 Provides-Extra: dev
 Requires-Dist: rich>=12.3.0; extra == "dev"
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "dev"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "dev"
 Requires-Dist: omegaconf>=2.1.0; extra == "dev"
 Requires-Dist: hydra-core>=1.1.0; extra == "dev"
 Requires-Dist: coverage>=6.4; extra == "dev"
 Requires-Dist: pytest>=6.0; extra == "dev"
 Requires-Dist: pytest-rerunfailures>=10.2; extra == "dev"
 Requires-Dist: twine==3.2; extra == "dev"
 Requires-Dist: mypy>=0.920; extra == "dev"
 Requires-Dist: pre-commit>=1.0; extra == "dev"
 Requires-Dist: protobuf<=3.20.1; extra == "dev"
 Requires-Dist: ipython[notebook]; extra == "dev"
 Requires-Dist: jupytext>=1.10; extra == "dev"
 Requires-Dist: nbval>=0.9.6; extra == "dev"
 Provides-Extra: all
 Requires-Dist: rich>=12.3.0; extra == "all"
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "all"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "all"
 Requires-Dist: omegaconf>=2.1.0; extra == "all"
 Requires-Dist: hydra-core>=1.1.0; extra == "all"
 Requires-Dist: coverage>=6.4; extra == "all"
 Requires-Dist: pytest>=6.0; extra == "all"
 Requires-Dist: pytest-rerunfailures>=10.2; extra == "all"
 Requires-Dist: twine==3.2; extra == "all"
 Requires-Dist: mypy>=0.920; extra == "all"
@@ -93,45 +93,45 @@
 Requires-Dist: nbval>=0.9.6; extra == "all"
 Requires-Dist: datasets; extra == "all"
 Requires-Dist: evaluate; extra == "all"
 Requires-Dist: transformers>=4.18.0; extra == "all"
 Requires-Dist: scikit-learn; extra == "all"
 Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: tensorboardX>=2.2; extra == "all"
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "all"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "all"
 Requires-Dist: omegaconf>=2.1.0; extra == "all"
 Requires-Dist: hydra-core>=1.1.0; extra == "all"
 
 <div align="center">
 
-<img src="https://github.com/speediedan/finetuning-scheduler/raw/v2.2.1/docs/source/_static/images/logos/logo_fts.png" width="401px">
+<img src="https://github.com/speediedan/finetuning-scheduler/raw/v2.2.4/docs/source/_static/images/logos/logo_fts.png" width="401px">
 
 **A PyTorch Lightning extension that enhances model experimentation with flexible fine-tuning schedules.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="https://finetuning-scheduler.readthedocs.io/en/stable/">Docs</a> •
   <a href="#Setup">Setup</a> •
   <a href="#examples">Examples</a> •
   <a href="#community">Community</a>
 </p>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/finetuning-scheduler)](https://pypi.org/project/finetuning-scheduler/)
 [![PyPI Status](https://badge.fury.io/py/finetuning-scheduler.svg)](https://badge.fury.io/py/finetuning-scheduler)\
-[![codecov](https://codecov.io/gh/speediedan/finetuning-scheduler/release/2.2.1/graph/badge.svg?flag=gpu)](https://codecov.io/gh/speediedan/finetuning-scheduler)
+[![codecov](https://codecov.io/gh/speediedan/finetuning-scheduler/release/2.2.4/graph/badge.svg?flag=gpu)](https://codecov.io/gh/speediedan/finetuning-scheduler)
 [![ReadTheDocs](https://readthedocs.org/projects/finetuning-scheduler/badge/?version=latest)](https://finetuning-scheduler.readthedocs.io/en/stable/)
 [![DOI](https://zenodo.org/badge/455666112.svg)](https://zenodo.org/badge/latestdoi/455666112)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/speediedan/finetuning-scheduler/blob/master/LICENSE)
 
 </div>
 
 ______________________________________________________________________
 
-<img width="300px" src="https://github.com/speediedan/finetuning-scheduler/raw/v2.2.1/docs/source/_static/images/fts/fts_explicit_loss_anim.gif" alt="FinetuningScheduler explicit loss animation" align="right"/>
+<img width="300px" src="https://github.com/speediedan/finetuning-scheduler/raw/v2.2.4/docs/source/_static/images/fts/fts_explicit_loss_anim.gif" alt="FinetuningScheduler explicit loss animation" align="right"/>
 
 [FinetuningScheduler](https://finetuning-scheduler.readthedocs.io/en/stable/api/finetuning_scheduler.fts.html#finetuning_scheduler.fts.FinetuningScheduler) is simple to use yet powerful, offering a number of features that facilitate model research and exploration:
 
 - easy specification of flexible fine-tuning schedules with explicit or regex-based parameter selection
   - implicit schedules for initial/naive model exploration
   - explicit schedules for performance tuning, fine-grained behavioral experimentation and computational efficiency
 - automatic restoration of best per-phase checkpoints driven by iterative application of early-stopping criteria to each fine-tuning phase
@@ -196,20 +196,20 @@
 Fine-Tuning Scheduler is rigorously tested across multiple CPUs, GPUs and against major Python and PyTorch versions. Each Fine-Tuning Scheduler minor release (major.minor.patch) is paired with a Lightning minor release (e.g. Fine-Tuning Scheduler 2.0 depends upon Lightning 2.0).
 
 To ensure maximum stability, the latest Lightning patch release fully tested with Fine-Tuning Scheduler is set as a maximum dependency in Fine-Tuning Scheduler's requirements.txt (e.g. \<= 1.7.1). If you'd like to test a specific Lightning patch version greater than that currently in Fine-Tuning Scheduler's requirements.txt, it will likely work but you should install Fine-Tuning Scheduler from source and update the requirements.txt as desired.
 
 <details>
   <summary>Current build statuses for Fine-Tuning Scheduler </summary>
 
-| System / (PyTorch/Python ver) |                                                                                                         1.13/3.8                                                                                                         |                                                                                                              2.2.1/3.8, 2.2.1/3.11                                                                                                               |
+| System / (PyTorch/Python ver) |                                                                                                         1.13/3.8                                                                                                         |                                                                                                              2.2.2/3.8, 2.2.2/3.11                                                                                                               |
 | :---------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
-|      Linux \[GPUs\*\*\]       |                                                                                                            -                                                                                                             | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/_apis/build/status/Multi-GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.2.1)](https://dev.azure.com/speediedan/finetuning-scheduler/_build/latest?definitionId=2&branchName=refs%2Ftags%2F2.2.1) |
-|     Linux (Ubuntu 20.04)      | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
-|           OSX (11)            | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
-|        Windows (2022)         | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|      Linux \[GPUs\*\*\]       |                                                                                                            -                                                                                                             | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/_apis/build/status/Multi-GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.2.4)](https://dev.azure.com/speediedan/finetuning-scheduler/_build/latest?definitionId=2&branchName=refs%2Ftags%2F2.2.4) |
+|     Linux (Ubuntu 20.04)      | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|           OSX (11)            | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|        Windows (2022)         | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
 
 - \*\* tests run on one RTX 4090 and one RTX 2070
 
 </details>
 
 ## Community
```

### Comparing `finetuning-scheduler-2.2.1/README.md` & `finetuning_scheduler-2.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 Fine-Tuning Scheduler is rigorously tested across multiple CPUs, GPUs and against major Python and PyTorch versions. Each Fine-Tuning Scheduler minor release (major.minor.patch) is paired with a Lightning minor release (e.g. Fine-Tuning Scheduler 2.0 depends upon Lightning 2.0).
 
 To ensure maximum stability, the latest Lightning patch release fully tested with Fine-Tuning Scheduler is set as a maximum dependency in Fine-Tuning Scheduler's requirements.txt (e.g. \<= 1.7.1). If you'd like to test a specific Lightning patch version greater than that currently in Fine-Tuning Scheduler's requirements.txt, it will likely work but you should install Fine-Tuning Scheduler from source and update the requirements.txt as desired.
 
 <details>
   <summary>Current build statuses for Fine-Tuning Scheduler </summary>
 
-| System / (PyTorch/Python ver) |                                                                                                         1.13/3.8                                                                                                         |                                                                                                              2.2.1/3.8, 2.2.1/3.11                                                                                                               |
+| System / (PyTorch/Python ver) |                                                                                                         1.13/3.8                                                                                                         |                                                                                                              2.2.2/3.8, 2.2.2/3.11                                                                                                               |
 | :---------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
 |      Linux \[GPUs\*\*\]       |                                                                                                            -                                                                                                             | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/_apis/build/status/Multi-GPU%20&%20Example%20Tests?branchName=main)](https://dev.azure.com/speediedan/finetuning-scheduler/_build/latest?definitionId=1&branchName=main) |
 |     Linux (Ubuntu 20.04)      | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?branch=main&event=push)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?branch=main&event=push)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
 |           OSX (11)            | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?branch=main&event=push)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?branch=main&event=push)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
 |        Windows (2022)         | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?branch=main&event=push)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?branch=main&event=push)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
 
 - \*\* tests run on one RTX 4090 and one RTX 2070
```

#### html2text {}

```diff
@@ -84,15 +84,15 @@
 ensure maximum stability, the latest Lightning patch release fully tested with
 Fine-Tuning Scheduler is set as a maximum dependency in Fine-Tuning Scheduler's
 requirements.txt (e.g. \<= 1.7.1). If you'd like to test a specific Lightning
 patch version greater than that currently in Fine-Tuning Scheduler's
 requirements.txt, it will likely work but you should install Fine-Tuning
 Scheduler from source and update the requirements.txt as desired. Current build
 statuses for Fine-Tuning Scheduler | System / (PyTorch/Python ver) | 1.13/3.8 |
-2.2.1/3.8, 2.2.1/3.11 | | :---------------------------: | :--------------------
+2.2.2/3.8, 2.2.2/3.11 | | :---------------------------: | :--------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ------------------------------------: | :--------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ------------------------------------------: | | Linux \[GPUs\*\*\] | - | [!
 [Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/_apis/
```

### Comparing `finetuning-scheduler-2.2.1/pyproject.toml` & `finetuning_scheduler-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/setup.py` & `finetuning_scheduler-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler/__about__.py` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler/__about__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 
 _this_year = time.strftime("%Y")
-__version__ = "2.2.1"
+__version__ = "2.2.4"
 __author__ = "Dan Dale"
 __author_email__ = "danny.dale@gmail.com"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2021-{_this_year}, {__author__}"
 __homepage__ = "https://github.com/speediedan/finetuning-scheduler"
 __docs_url__ = "https://finetuning-scheduler.readthedocs.io/en/latest/"
 # this has to be simple string, see: https://github.com/pypa/twine/issues/522
```

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler/__init__.py` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler/fts.py` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler/fts.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler/fts_supporters.py` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler/fts_supporters.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler/setup_tools.py` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler/setup_tools.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler/strategy_adapters/__init__.py` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler/strategy_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler/strategy_adapters/_wrap_utils.py` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler/strategy_adapters/_wrap_utils.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler/strategy_adapters/base.py` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler/strategy_adapters/base.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler/strategy_adapters/fsdp.py` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler/strategy_adapters/fsdp.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler/types.py` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler/types.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler.egg-info/PKG-INFO` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finetuning-scheduler
-Version: 2.2.1
+Version: 2.2.4
 Summary: A PyTorch Lightning extension that enhances model experimentation with flexible fine-tuning schedules.
 Home-page: https://github.com/speediedan/finetuning-scheduler
 Download-URL: https://github.com/speediedan/finetuning-scheduler
 Author: Dan Dale
 Author-email: danny.dale@gmail.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/speediedan/finetuning-scheduler/issues
@@ -24,29 +24,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lightning<2.2.2,>=2.2.0
+Requires-Dist: lightning<2.2.5,>=2.2.0
 Requires-Dist: torch<2.3.0,>=1.13.0
 Provides-Extra: examples
 Requires-Dist: datasets; extra == "examples"
 Requires-Dist: evaluate; extra == "examples"
 Requires-Dist: transformers>=4.18.0; extra == "examples"
 Requires-Dist: scikit-learn; extra == "examples"
 Requires-Dist: sentencepiece; extra == "examples"
 Requires-Dist: tensorboardX>=2.2; extra == "examples"
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "examples"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "examples"
 Requires-Dist: omegaconf>=2.1.0; extra == "examples"
 Requires-Dist: hydra-core>=1.1.0; extra == "examples"
 Provides-Extra: extra
 Requires-Dist: rich>=12.3.0; extra == "extra"
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "extra"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "extra"
 Requires-Dist: omegaconf>=2.1.0; extra == "extra"
 Requires-Dist: hydra-core>=1.1.0; extra == "extra"
 Provides-Extra: test
 Requires-Dist: coverage>=6.4; extra == "test"
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: pytest-rerunfailures>=10.2; extra == "test"
 Requires-Dist: twine==3.2; extra == "test"
@@ -54,35 +54,35 @@
 Requires-Dist: pre-commit>=1.0; extra == "test"
 Requires-Dist: protobuf<=3.20.1; extra == "test"
 Provides-Extra: ipynb
 Requires-Dist: ipython[notebook]; extra == "ipynb"
 Requires-Dist: jupytext>=1.10; extra == "ipynb"
 Requires-Dist: nbval>=0.9.6; extra == "ipynb"
 Provides-Extra: cli
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "cli"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "cli"
 Requires-Dist: omegaconf>=2.1.0; extra == "cli"
 Requires-Dist: hydra-core>=1.1.0; extra == "cli"
 Provides-Extra: dev
 Requires-Dist: rich>=12.3.0; extra == "dev"
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "dev"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "dev"
 Requires-Dist: omegaconf>=2.1.0; extra == "dev"
 Requires-Dist: hydra-core>=1.1.0; extra == "dev"
 Requires-Dist: coverage>=6.4; extra == "dev"
 Requires-Dist: pytest>=6.0; extra == "dev"
 Requires-Dist: pytest-rerunfailures>=10.2; extra == "dev"
 Requires-Dist: twine==3.2; extra == "dev"
 Requires-Dist: mypy>=0.920; extra == "dev"
 Requires-Dist: pre-commit>=1.0; extra == "dev"
 Requires-Dist: protobuf<=3.20.1; extra == "dev"
 Requires-Dist: ipython[notebook]; extra == "dev"
 Requires-Dist: jupytext>=1.10; extra == "dev"
 Requires-Dist: nbval>=0.9.6; extra == "dev"
 Provides-Extra: all
 Requires-Dist: rich>=12.3.0; extra == "all"
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "all"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "all"
 Requires-Dist: omegaconf>=2.1.0; extra == "all"
 Requires-Dist: hydra-core>=1.1.0; extra == "all"
 Requires-Dist: coverage>=6.4; extra == "all"
 Requires-Dist: pytest>=6.0; extra == "all"
 Requires-Dist: pytest-rerunfailures>=10.2; extra == "all"
 Requires-Dist: twine==3.2; extra == "all"
 Requires-Dist: mypy>=0.920; extra == "all"
@@ -93,45 +93,45 @@
 Requires-Dist: nbval>=0.9.6; extra == "all"
 Requires-Dist: datasets; extra == "all"
 Requires-Dist: evaluate; extra == "all"
 Requires-Dist: transformers>=4.18.0; extra == "all"
 Requires-Dist: scikit-learn; extra == "all"
 Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: tensorboardX>=2.2; extra == "all"
-Requires-Dist: jsonargparse[signatures]>=4.26.1; extra == "all"
+Requires-Dist: jsonargparse[signatures]>=4.27.7; extra == "all"
 Requires-Dist: omegaconf>=2.1.0; extra == "all"
 Requires-Dist: hydra-core>=1.1.0; extra == "all"
 
 <div align="center">
 
-<img src="https://github.com/speediedan/finetuning-scheduler/raw/v2.2.1/docs/source/_static/images/logos/logo_fts.png" width="401px">
+<img src="https://github.com/speediedan/finetuning-scheduler/raw/v2.2.4/docs/source/_static/images/logos/logo_fts.png" width="401px">
 
 **A PyTorch Lightning extension that enhances model experimentation with flexible fine-tuning schedules.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="https://finetuning-scheduler.readthedocs.io/en/stable/">Docs</a> •
   <a href="#Setup">Setup</a> •
   <a href="#examples">Examples</a> •
   <a href="#community">Community</a>
 </p>
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/finetuning-scheduler)](https://pypi.org/project/finetuning-scheduler/)
 [![PyPI Status](https://badge.fury.io/py/finetuning-scheduler.svg)](https://badge.fury.io/py/finetuning-scheduler)\
-[![codecov](https://codecov.io/gh/speediedan/finetuning-scheduler/release/2.2.1/graph/badge.svg?flag=gpu)](https://codecov.io/gh/speediedan/finetuning-scheduler)
+[![codecov](https://codecov.io/gh/speediedan/finetuning-scheduler/release/2.2.4/graph/badge.svg?flag=gpu)](https://codecov.io/gh/speediedan/finetuning-scheduler)
 [![ReadTheDocs](https://readthedocs.org/projects/finetuning-scheduler/badge/?version=latest)](https://finetuning-scheduler.readthedocs.io/en/stable/)
 [![DOI](https://zenodo.org/badge/455666112.svg)](https://zenodo.org/badge/latestdoi/455666112)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/speediedan/finetuning-scheduler/blob/master/LICENSE)
 
 </div>
 
 ______________________________________________________________________
 
-<img width="300px" src="https://github.com/speediedan/finetuning-scheduler/raw/v2.2.1/docs/source/_static/images/fts/fts_explicit_loss_anim.gif" alt="FinetuningScheduler explicit loss animation" align="right"/>
+<img width="300px" src="https://github.com/speediedan/finetuning-scheduler/raw/v2.2.4/docs/source/_static/images/fts/fts_explicit_loss_anim.gif" alt="FinetuningScheduler explicit loss animation" align="right"/>
 
 [FinetuningScheduler](https://finetuning-scheduler.readthedocs.io/en/stable/api/finetuning_scheduler.fts.html#finetuning_scheduler.fts.FinetuningScheduler) is simple to use yet powerful, offering a number of features that facilitate model research and exploration:
 
 - easy specification of flexible fine-tuning schedules with explicit or regex-based parameter selection
   - implicit schedules for initial/naive model exploration
   - explicit schedules for performance tuning, fine-grained behavioral experimentation and computational efficiency
 - automatic restoration of best per-phase checkpoints driven by iterative application of early-stopping criteria to each fine-tuning phase
@@ -196,20 +196,20 @@
 Fine-Tuning Scheduler is rigorously tested across multiple CPUs, GPUs and against major Python and PyTorch versions. Each Fine-Tuning Scheduler minor release (major.minor.patch) is paired with a Lightning minor release (e.g. Fine-Tuning Scheduler 2.0 depends upon Lightning 2.0).
 
 To ensure maximum stability, the latest Lightning patch release fully tested with Fine-Tuning Scheduler is set as a maximum dependency in Fine-Tuning Scheduler's requirements.txt (e.g. \<= 1.7.1). If you'd like to test a specific Lightning patch version greater than that currently in Fine-Tuning Scheduler's requirements.txt, it will likely work but you should install Fine-Tuning Scheduler from source and update the requirements.txt as desired.
 
 <details>
   <summary>Current build statuses for Fine-Tuning Scheduler </summary>
 
-| System / (PyTorch/Python ver) |                                                                                                         1.13/3.8                                                                                                         |                                                                                                              2.2.1/3.8, 2.2.1/3.11                                                                                                               |
+| System / (PyTorch/Python ver) |                                                                                                         1.13/3.8                                                                                                         |                                                                                                              2.2.2/3.8, 2.2.2/3.11                                                                                                               |
 | :---------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
-|      Linux \[GPUs\*\*\]       |                                                                                                            -                                                                                                             | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/_apis/build/status/Multi-GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.2.1)](https://dev.azure.com/speediedan/finetuning-scheduler/_build/latest?definitionId=2&branchName=refs%2Ftags%2F2.2.1) |
-|     Linux (Ubuntu 20.04)      | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
-|           OSX (11)            | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
-|        Windows (2022)         | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.1)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|      Linux \[GPUs\*\*\]       |                                                                                                            -                                                                                                             | [![Build Status](https://dev.azure.com//speediedan/finetuning-scheduler/_apis/build/status/Multi-GPU%20&%20Example%20Tests?branchName=refs%2Ftags%2F2.2.4)](https://dev.azure.com/speediedan/finetuning-scheduler/_build/latest?definitionId=2&branchName=refs%2Ftags%2F2.2.4) |
+|     Linux (Ubuntu 20.04)      | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|           OSX (11)            | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
+|        Windows (2022)         | [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml) |             [![Test](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml/badge.svg?tag=2.2.4)](https://github.com/speediedan/finetuning-scheduler/actions/workflows/ci_test-full.yml)             |
 
 - \*\* tests run on one RTX 4090 and one RTX 2070
 
 </details>
 
 ## Community
```

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler.egg-info/SOURCES.txt` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/finetuning_scheduler.egg-info/requires.txt` & `finetuning_scheduler-2.2.4/src/finetuning_scheduler.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-lightning<2.2.2,>=2.2.0
+lightning<2.2.5,>=2.2.0
 torch<2.3.0,>=1.13.0
 
 [all]
 rich>=12.3.0
-jsonargparse[signatures]>=4.26.1
+jsonargparse[signatures]>=4.27.7
 omegaconf>=2.1.0
 hydra-core>=1.1.0
 coverage>=6.4
 pytest>=6.0
 pytest-rerunfailures>=10.2
 twine==3.2
 mypy>=0.920
@@ -20,21 +20,21 @@
 evaluate
 transformers>=4.18.0
 scikit-learn
 sentencepiece
 tensorboardX>=2.2
 
 [cli]
-jsonargparse[signatures]>=4.26.1
+jsonargparse[signatures]>=4.27.7
 omegaconf>=2.1.0
 hydra-core>=1.1.0
 
 [dev]
 rich>=12.3.0
-jsonargparse[signatures]>=4.26.1
+jsonargparse[signatures]>=4.27.7
 omegaconf>=2.1.0
 hydra-core>=1.1.0
 coverage>=6.4
 pytest>=6.0
 pytest-rerunfailures>=10.2
 twine==3.2
 mypy>=0.920
@@ -47,21 +47,21 @@
 [examples]
 datasets
 evaluate
 transformers>=4.18.0
 scikit-learn
 sentencepiece
 tensorboardX>=2.2
-jsonargparse[signatures]>=4.26.1
+jsonargparse[signatures]>=4.27.7
 omegaconf>=2.1.0
 hydra-core>=1.1.0
 
 [extra]
 rich>=12.3.0
-jsonargparse[signatures]>=4.26.1
+jsonargparse[signatures]>=4.27.7
 omegaconf>=2.1.0
 hydra-core>=1.1.0
 
 [ipynb]
 ipython[notebook]
 jupytext>=1.10
 nbval>=0.9.6
```

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/cli_experiment_utils.py` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/cli_experiment_utils.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/RteBoolqModule_ft_schedule_deberta_base_fsdp.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/fsdp/fts_ddp_fsdp_baseline_profile.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_offload_profile.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_awp_overrides_profile.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_basic_profile.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/fsdp/fts_fsdp_basic_profile.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_lr/explicit_reinit_lr.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_lr/explicit_reinit_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_lr/fts_explicit_reinit_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_lr/fts_implicit_reinit_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_optim_lr/explicit_reinit_optim_lr.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/explicit_reinit_optim_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_explicit_reinit_optim_lr.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_explicit_reinit_optim_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr_use_curr.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/advanced/reinit_optim_lr/fts_implicit_reinit_optim_lr_use_curr.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/fts_defaults.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/fts_defaults.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/fts_explicit.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/fts_explicit.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/config/fts_implicit.yaml` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/config/fts_implicit.yaml`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/extended_profiler.py` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/extended_profiler.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/src/fts_examples/stable/fts_superglue.py` & `finetuning_scheduler-2.2.4/src/fts_examples/stable/fts_superglue.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/tests/test_finetuning_scheduler_callback.py` & `finetuning_scheduler-2.2.4/tests/test_finetuning_scheduler_callback.py`

 * *Files identical despite different names*

### Comparing `finetuning-scheduler-2.2.1/tests/test_fsdp.py` & `finetuning_scheduler-2.2.4/tests/test_fsdp.py`

 * *Files identical despite different names*

