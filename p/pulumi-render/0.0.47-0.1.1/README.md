# Comparing `tmp/pulumi_render-0.0.47.tar.gz` & `tmp/pulumi_render-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_render-0.0.47.tar", last modified: Sun Nov 13 16:54:01 2022, max compression
+gzip compressed data, was "pulumi_render-0.1.1.tar", last modified: Sun May  5 02:01:39 2024, max compression
```

## Comparing `pulumi_render-0.0.47.tar` & `pulumi_render-0.1.1.tar`

### file list

```diff
@@ -1,58 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 16:54:01.677936 pulumi_render-0.0.47/
--rw-r--r--   0 runner    (1001) docker     (121)     9029 2022-11-13 16:54:01.677936 pulumi_render-0.0.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8653 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 16:54:01.669937 pulumi_render-0.0.47/pulumi_render/
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8105 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 16:54:01.669937 pulumi_render-0.0.47/pulumi_render/config/
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 16:54:01.673936 pulumi_render-0.0.47/pulumi_render/owners/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/owners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/owners/_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/owners/get_owner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/owners/list_owners.py
--rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/owners/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3648 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 16:54:01.677936 pulumi_render-0.0.47/pulumi_render/services/
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4993 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)    37055 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    19297 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/background_worker.py
--rw-r--r--   0 runner    (1001) docker     (121)    19038 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/cron_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     6780 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (121)     5659 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5457 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/env_var.py
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/get_background_worker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/get_cron_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/get_custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/get_deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2185 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/get_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     2162 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/get_private_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/get_static_site.py
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/get_web_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/job.py
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/list_custom_domains.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/list_deploys.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/list_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/list_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/list_service_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/list_services.py
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/list_static_site_routes.py
--rw-r--r--   0 runner    (1001) docker     (121)    97612 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    19185 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/private_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     5227 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/scale.py
--rw-r--r--   0 runner    (1001) docker     (121)    19193 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/static_site.py
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/suspend.py
--rw-r--r--   0 runner    (1001) docker     (121)    19119 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render/services/web_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 16:54:01.669937 pulumi_render-0.0.47/pulumi_render.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9029 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1768 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/pulumi_render.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-13 16:54:01.677936 pulumi_render-0.0.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-11-13 16:54:01.000000 pulumi_render-0.0.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.073893 pulumi_render-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-05 02:01:39.073893 pulumi_render-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.065893 pulumi_render-0.1.1/pulumi_render/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.065893 pulumi_render-0.1.1/pulumi_render/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.069893 pulumi_render-0.1.1/pulumi_render/owners/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/owners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/owners/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/owners/get_owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/owners/list_owners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/owners/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.069893 pulumi_render-0.1.1/pulumi_render/registrycredentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/registrycredentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/registrycredentials/get_registry_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/registrycredentials/list_registry_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/registrycredentials/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/registrycredentials/registry_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.073893 pulumi_render-0.1.1/pulumi_render/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39491 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/auto_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19297 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/background_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/cron_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/custom_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/deploys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_background_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_cron_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_private_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_static_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/get_web_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_custom_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_deploys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/list_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99395 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/private_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/static_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/suspend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pulumi_render/services/web_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 02:01:39.073893 pulumi_render-0.1.1/pulumi_render.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-05 02:01:39.000000 pulumi_render-0.1.1/pulumi_render.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-05 02:01:39.000000 pulumi_render-0.1.1/pulumi_render.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 02:01:39.000000 pulumi_render-0.1.1/pulumi_render.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 02:01:39.000000 pulumi_render-0.1.1/pulumi_render.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 02:01:39.000000 pulumi_render-0.1.1/pulumi_render.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-05 02:01:32.000000 pulumi_render-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 02:01:39.077893 pulumi_render-0.1.1/setup.cfg
```

### Comparing `pulumi_render-0.0.47/pulumi_render/_utilities.py` & `pulumi_render-0.1.1/pulumi_render/_utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumigen. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
+import asyncio
+import importlib.metadata
 import importlib.util
 import inspect
 import json
 import os
-import pkg_resources
 import sys
 import typing
 
 import pulumi
 import pulumi.runtime
+from pulumi.runtime.sync_await import _sync_await
 
 from semver import VersionInfo as SemverVersion
 from parver import Version as PEP440Version
 
 
 def get_env(*args):
     for v in args:
@@ -66,15 +68,15 @@
     # pkg_resources uses setuptools to inspect the set of installed packages. We use it here to ask
     # for the currently installed version of the root package (i.e. us) and get its version.
 
     # Unfortunately, PEP440 and semver differ slightly in incompatible ways. The Pulumi engine expects
     # to receive a valid semver string when receiving requests from the language host, so it's our
     # responsibility as the library to convert our own PEP440 version into a valid semver string.
 
-    pep440_version_string = pkg_resources.require(root_package)[0].version
+    pep440_version_string = importlib.metadata.version(root_package)
     pep440_version = PEP440Version.parse(pep440_version_string)
     (major, minor, patch) = pep440_version.release
     prerelease = None
     if pep440_version.pre_tag == 'a':
         prerelease = f"alpha.{pep440_version.pre}"
     elif pep440_version.pre_tag == 'b':
         prerelease = f"beta.{pep440_version.pre}"
@@ -242,9 +244,48 @@
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
+
+def call_plain(
+    tok: str,
+    props: pulumi.Inputs,
+    res: typing.Optional[pulumi.Resource] = None,
+    typ: typing.Optional[type] = None,
+) -> typing.Any:
+    """
+    Wraps pulumi.runtime.plain to force the output and return it plainly.
+    """
+
+    output = pulumi.runtime.call(tok, props, res, typ)
+
+    # Ingoring deps silently. They are typically non-empty, r.f() calls include r as a dependency.
+    result, known, secret, _ = _sync_await(asyncio.ensure_future(_await_output(output)))
+
+    problem = None
+    if not known:
+        problem = ' an unknown value'
+    elif secret:
+        problem = ' a secret value'
+
+    if problem:
+        raise AssertionError(
+            f"Plain resource method '{tok}' incorrectly returned {problem}. "
+            + "This is an error in the provider, please report this to the provider developer."
+        )
+
+    return result
+
+
+async def _await_output(o: pulumi.Output[typing.Any]) -> typing.Tuple[object, bool, bool, set]:
+    return (
+        await o._future,
+        await o._is_known,
+        await o._is_secret,
+        await o._resources,
+    )
+
 def get_plugin_download_url():
 	return "github://api.github.com/cloudy-sky-software/pulumi-render"
```

### Comparing `pulumi_render-0.0.47/pulumi_render/config/vars.py` & `pulumi_render-0.1.1/pulumi_render/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render/owners/get_owner.py` & `pulumi_render-0.1.1/pulumi_render/owners/get_owner.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:owners:getOwner', __args__, opts=opts, typ=GetOwnerResult).value
 
     return AwaitableGetOwnerResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_owner)
 def get_owner_output(id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOwnerResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_render-0.0.47/pulumi_render/owners/list_owners.py` & `pulumi_render-0.1.1/pulumi_render/owners/list_owners.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from . import outputs
 from ._enums import *
 
 __all__ = [
     'ListOwnersResult',
     'AwaitableListOwnersResult',
     'list_owners',
+    'list_owners_output',
 ]
 
 @pulumi.output_type
 class ListOwnersResult:
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
@@ -44,8 +45,16 @@
     Use this data source to access information about an existing resource.
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:owners:listOwners', __args__, opts=opts, typ=ListOwnersResult).value
 
     return AwaitableListOwnersResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
+
+
+@_utilities.lift_output_func(list_owners)
+def list_owners_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListOwnersResult]:
+    """
+    Use this data source to access information about an existing resource.
+    """
+    ...
```

### Comparing `pulumi_render-0.0.47/pulumi_render/owners/outputs.py` & `pulumi_render-0.1.1/pulumi_render/owners/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render/provider.py` & `pulumi_render-0.1.1/pulumi_render/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render/services/__init__.py` & `pulumi_render-0.1.1/pulumi_render/services/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,36 @@
 # *** WARNING: this file was generated by pulumigen. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from .. import _utilities
 import typing
 # Export this package's modules as members:
 from ._enums import *
+from .auto_scaling import *
 from .background_worker import *
 from .cron_job import *
-from .custom_domain import *
-from .deploy import *
-from .env_var import *
+from .custom_domains import *
+from .deploys import *
+from .env_vars import *
 from .get_background_worker import *
 from .get_cron_job import *
 from .get_custom_domain import *
 from .get_deploy import *
 from .get_job import *
 from .get_private_service import *
 from .get_static_site import *
 from .get_web_service import *
-from .job import *
+from .jobs import *
 from .list_custom_domains import *
 from .list_deploys import *
 from .list_env_vars import *
+from .list_headers import *
 from .list_jobs import *
-from .list_service_headers import *
+from .list_routes import *
 from .list_services import *
-from .list_static_site_routes import *
 from .private_service import *
 from .scale import *
 from .static_site import *
 from .suspend import *
 from .web_service import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/_enums.py` & `pulumi_render-0.1.1/pulumi_render/services/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render/services/_inputs.py` & `pulumi_render-0.1.1/pulumi_render/services/_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
 
 __all__ = [
+    'AutoScalingCriteriaSpecArgs',
+    'AutoScalingCriteriaArgs',
     'BackgroundWorkerServiceDetailsParentServerPropertiesArgs',
     'BackgroundWorkerServiceDetailsArgs',
     'CronJobServiceDetailsArgs',
     'DiskArgs',
     'DockerDetailsArgs',
     'EnvVarKeyValueArgs',
     'NativeEnvironmentDetailsArgs',
@@ -27,14 +29,78 @@
     'StaticSiteServiceDetailsParentServerPropertiesArgs',
     'StaticSiteServiceDetailsArgs',
     'WebServiceServiceDetailsParentServerPropertiesArgs',
     'WebServiceServiceDetailsArgs',
 ]
 
 @pulumi.input_type
+class AutoScalingCriteriaSpecArgs:
+    def __init__(__self__, *,
+                 enabled: Optional[pulumi.Input[bool]] = None,
+                 percentage: Optional[pulumi.Input[float]] = None):
+        """
+        :param pulumi.Input[float] percentage: Determines when your service will be scaled. If the average resource utilization is significantly above/below the target, we will increase/decrease the number of instances.
+        """
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if percentage is not None:
+            pulumi.set(__self__, "percentage", percentage)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "enabled")
+
+    @enabled.setter
+    def enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "enabled", value)
+
+    @property
+    @pulumi.getter
+    def percentage(self) -> Optional[pulumi.Input[float]]:
+        """
+        Determines when your service will be scaled. If the average resource utilization is significantly above/below the target, we will increase/decrease the number of instances.
+        """
+        return pulumi.get(self, "percentage")
+
+    @percentage.setter
+    def percentage(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "percentage", value)
+
+
+@pulumi.input_type
+class AutoScalingCriteriaArgs:
+    def __init__(__self__, *,
+                 cpu: Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']] = None,
+                 memory: Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']] = None):
+        if cpu is not None:
+            pulumi.set(__self__, "cpu", cpu)
+        if memory is not None:
+            pulumi.set(__self__, "memory", memory)
+
+    @property
+    @pulumi.getter
+    def cpu(self) -> Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']]:
+        return pulumi.get(self, "cpu")
+
+    @cpu.setter
+    def cpu(self, value: Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']]):
+        pulumi.set(self, "cpu", value)
+
+    @property
+    @pulumi.getter
+    def memory(self) -> Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']]:
+        return pulumi.get(self, "memory")
+
+    @memory.setter
+    def memory(self, value: Optional[pulumi.Input['AutoScalingCriteriaSpecArgs']]):
+        pulumi.set(self, "memory", value)
+
+
+@pulumi.input_type
 class BackgroundWorkerServiceDetailsParentServerPropertiesArgs:
     def __init__(__self__, *,
                  id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/background_worker.py` & `pulumi_render-0.1.1/pulumi_render/services/background_worker.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render/services/cron_job.py` & `pulumi_render-0.1.1/pulumi_render/services/cron_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render/services/custom_domain.py` & `pulumi_render-0.1.1/pulumi_render/services/custom_domains.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 
-__all__ = ['CustomDomainArgs', 'CustomDomain']
+__all__ = ['CustomDomainsArgs', 'CustomDomains']
 
 @pulumi.input_type
-class CustomDomainArgs:
+class CustomDomainsArgs:
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a CustomDomain resource.
+        The set of arguments for constructing a CustomDomains resource.
         :param pulumi.Input[str] service_id: (Required) The ID of the service
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if service_id is not None:
             pulumi.set(__self__, "service_id", service_id)
 
@@ -45,43 +45,43 @@
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class CustomDomain(pulumi.CustomResource):
+class CustomDomains(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a CustomDomain resource with the given unique name, props, and options.
+        Create a CustomDomains resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] service_id: (Required) The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[CustomDomainArgs] = None,
+                 args: Optional[CustomDomainsArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a CustomDomain resource with the given unique name, props, and options.
+        Create a CustomDomains resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param CustomDomainArgs args: The arguments to use to populate this resource's properties.
+        :param CustomDomainsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CustomDomainArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CustomDomainsArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -91,54 +91,54 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CustomDomainArgs.__new__(CustomDomainArgs)
+            __props__ = CustomDomainsArgs.__new__(CustomDomainsArgs)
 
             __props__.__dict__["name"] = name
             __props__.__dict__["service_id"] = service_id
             __props__.__dict__["created_at"] = None
             __props__.__dict__["domain_type"] = None
             __props__.__dict__["public_suffix"] = None
             __props__.__dict__["redirect_for_name"] = None
             __props__.__dict__["server"] = None
             __props__.__dict__["verification_status"] = None
-        super(CustomDomain, __self__).__init__(
-            'render:services:CustomDomain',
+        super(CustomDomains, __self__).__init__(
+            'render:services:CustomDomains',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'CustomDomain':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'CustomDomains':
         """
-        Get an existing CustomDomain resource's state with the given name, id, and optional extra
+        Get an existing CustomDomains resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = CustomDomainArgs.__new__(CustomDomainArgs)
+        __props__ = CustomDomainsArgs.__new__(CustomDomainsArgs)
 
         __props__.__dict__["created_at"] = None
         __props__.__dict__["domain_type"] = None
         __props__.__dict__["name"] = None
         __props__.__dict__["public_suffix"] = None
         __props__.__dict__["redirect_for_name"] = None
         __props__.__dict__["server"] = None
         __props__.__dict__["verification_status"] = None
-        return CustomDomain(resource_name, opts=opts, __props__=__props__)
+        return CustomDomains(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "created_at")
 
     @property
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/deploy.py` & `pulumi_render-0.1.1/pulumi_render/services/deploys.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 
-__all__ = ['DeployArgs', 'Deploy']
+__all__ = ['DeploysArgs', 'Deploys']
 
 @pulumi.input_type
-class DeployArgs:
+class DeploysArgs:
     def __init__(__self__, *,
                  clear_cache: Optional[pulumi.Input['ClearCache']] = None,
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Deploy resource.
+        The set of arguments for constructing a Deploys resource.
         :param pulumi.Input[str] service_id: (Required) The ID of the service
         """
         if clear_cache is None:
             clear_cache = 'do_not_clear'
         if clear_cache is not None:
             pulumi.set(__self__, "clear_cache", clear_cache)
         if service_id is not None:
@@ -47,43 +47,43 @@
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class Deploy(pulumi.CustomResource):
+class Deploys(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  clear_cache: Optional[pulumi.Input['ClearCache']] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Deploy resource with the given unique name, props, and options.
+        Create a Deploys resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] service_id: (Required) The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[DeployArgs] = None,
+                 args: Optional[DeploysArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Deploy resource with the given unique name, props, and options.
+        Create a Deploys resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param DeployArgs args: The arguments to use to populate this resource's properties.
+        :param DeploysArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DeployArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(DeploysArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -93,46 +93,46 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DeployArgs.__new__(DeployArgs)
+            __props__ = DeploysArgs.__new__(DeploysArgs)
 
             if clear_cache is None:
                 clear_cache = 'do_not_clear'
             __props__.__dict__["clear_cache"] = clear_cache
             __props__.__dict__["service_id"] = service_id
             __props__.__dict__["commit"] = None
-        super(Deploy, __self__).__init__(
-            'render:services:Deploy',
+        super(Deploys, __self__).__init__(
+            'render:services:Deploys',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'Deploy':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'Deploys':
         """
-        Get an existing Deploy resource's state with the given name, id, and optional extra
+        Get an existing Deploys resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = DeployArgs.__new__(DeployArgs)
+        __props__ = DeploysArgs.__new__(DeploysArgs)
 
         __props__.__dict__["clear_cache"] = None
         __props__.__dict__["commit"] = None
-        return Deploy(resource_name, opts=opts, __props__=__props__)
+        return Deploys(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="clearCache")
     def clear_cache(self) -> pulumi.Output[Optional['ClearCache']]:
         return pulumi.get(self, "clear_cache")
 
     @property
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/env_var.py` & `pulumi_render-0.1.1/pulumi_render/services/env_vars.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 from ._inputs import *
 
-__all__ = ['EnvVarArgs', 'EnvVar']
+__all__ = ['EnvVarsArgs', 'EnvVars']
 
 @pulumi.input_type
-class EnvVarArgs:
+class EnvVarsArgs:
     def __init__(__self__, *,
                  env_vars: Optional[pulumi.Input[Sequence[pulumi.Input['EnvVarKeyValueArgs']]]] = None,
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a EnvVar resource.
+        The set of arguments for constructing a EnvVars resource.
         :param pulumi.Input[str] service_id: (Required) The ID of the service
         """
         if env_vars is not None:
             pulumi.set(__self__, "env_vars", env_vars)
         if service_id is not None:
             pulumi.set(__self__, "service_id", service_id)
 
@@ -46,43 +46,43 @@
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class EnvVar(pulumi.CustomResource):
+class EnvVars(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  env_vars: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['EnvVarKeyValueArgs']]]]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a EnvVar resource with the given unique name, props, and options.
+        Create a EnvVars resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] service_id: (Required) The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[EnvVarArgs] = None,
+                 args: Optional[EnvVarsArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a EnvVar resource with the given unique name, props, and options.
+        Create a EnvVars resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param EnvVarArgs args: The arguments to use to populate this resource's properties.
+        :param EnvVarsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(EnvVarArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(EnvVarsArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -92,41 +92,41 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = EnvVarArgs.__new__(EnvVarArgs)
+            __props__ = EnvVarsArgs.__new__(EnvVarsArgs)
 
             __props__.__dict__["env_vars"] = env_vars
             __props__.__dict__["service_id"] = service_id
-        super(EnvVar, __self__).__init__(
-            'render:services:EnvVar',
+        super(EnvVars, __self__).__init__(
+            'render:services:EnvVars',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'EnvVar':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'EnvVars':
         """
-        Get an existing EnvVar resource's state with the given name, id, and optional extra
+        Get an existing EnvVars resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = EnvVarArgs.__new__(EnvVarArgs)
+        __props__ = EnvVarsArgs.__new__(EnvVarsArgs)
 
         __props__.__dict__["env_vars"] = None
-        return EnvVar(resource_name, opts=opts, __props__=__props__)
+        return EnvVars(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="envVars")
     def env_vars(self) -> pulumi.Output[Optional[Sequence['outputs.EnvVarKeyValue']]]:
         return pulumi.get(self, "env_vars")
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/get_background_worker.py` & `pulumi_render-0.1.1/pulumi_render/services/get_background_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getBackgroundWorker', __args__, opts=opts, typ=GetBackgroundWorkerResult).value
 
     return AwaitableGetBackgroundWorkerResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_background_worker)
 def get_background_worker_output(id: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBackgroundWorkerResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/get_cron_job.py` & `pulumi_render-0.1.1/pulumi_render/services/get_cron_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getCronJob', __args__, opts=opts, typ=GetCronJobResult).value
 
     return AwaitableGetCronJobResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_cron_job)
 def get_cron_job_output(id: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCronJobResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/get_custom_domain.py` & `pulumi_render-0.1.1/pulumi_render/services/get_custom_domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getCustomDomain', __args__, opts=opts, typ=GetCustomDomainResult).value
 
     return AwaitableGetCustomDomainResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_custom_domain)
 def get_custom_domain_output(id: Optional[pulumi.Input[str]] = None,
                              service_id: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCustomDomainResult]:
     """
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/get_deploy.py` & `pulumi_render-0.1.1/pulumi_render/services/get_deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getDeploy', __args__, opts=opts, typ=GetDeployResult).value
 
     return AwaitableGetDeployResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_deploy)
 def get_deploy_output(id: Optional[pulumi.Input[str]] = None,
                       service_id: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDeployResult]:
     """
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/get_job.py` & `pulumi_render-0.1.1/pulumi_render/services/get_job.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getJob', __args__, opts=opts, typ=GetJobResult).value
 
     return AwaitableGetJobResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_job)
 def get_job_output(id: Optional[pulumi.Input[str]] = None,
                    service_id: Optional[pulumi.Input[str]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetJobResult]:
     """
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/get_private_service.py` & `pulumi_render-0.1.1/pulumi_render/services/get_private_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getPrivateService', __args__, opts=opts, typ=GetPrivateServiceResult).value
 
     return AwaitableGetPrivateServiceResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_private_service)
 def get_private_service_output(id: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPrivateServiceResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/get_static_site.py` & `pulumi_render-0.1.1/pulumi_render/services/get_static_site.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getStaticSite', __args__, opts=opts, typ=GetStaticSiteResult).value
 
     return AwaitableGetStaticSiteResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_static_site)
 def get_static_site_output(id: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetStaticSiteResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/get_web_service.py` & `pulumi_render-0.1.1/pulumi_render/services/get_web_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:getWebService', __args__, opts=opts, typ=GetWebServiceResult).value
 
     return AwaitableGetWebServiceResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(get_web_service)
 def get_web_service_output(id: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetWebServiceResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/job.py` & `pulumi_render-0.1.1/pulumi_render/services/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
-__all__ = ['JobArgs', 'Job']
+__all__ = ['JobsArgs', 'Jobs']
 
 @pulumi.input_type
-class JobArgs:
+class JobsArgs:
     def __init__(__self__, *,
                  plan_id: pulumi.Input[str],
                  start_command: pulumi.Input[str],
                  service_id: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Job resource.
+        The set of arguments for constructing a Jobs resource.
         :param pulumi.Input[str] service_id: (Required) The ID of the service
         """
         pulumi.set(__self__, "plan_id", plan_id)
         pulumi.set(__self__, "start_command", start_command)
         if service_id is not None:
             pulumi.set(__self__, "service_id", service_id)
 
@@ -53,44 +53,44 @@
         return pulumi.get(self, "service_id")
 
     @service_id.setter
     def service_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_id", value)
 
 
-class Job(pulumi.CustomResource):
+class Jobs(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  plan_id: Optional[pulumi.Input[str]] = None,
                  service_id: Optional[pulumi.Input[str]] = None,
                  start_command: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a Job resource with the given unique name, props, and options.
+        Create a Jobs resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] service_id: (Required) The ID of the service
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: JobArgs,
+                 args: JobsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a Job resource with the given unique name, props, and options.
+        Create a Jobs resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param JobArgs args: The arguments to use to populate this resource's properties.
+        :param JobsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(JobArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(JobsArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -101,56 +101,56 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = JobArgs.__new__(JobArgs)
+            __props__ = JobsArgs.__new__(JobsArgs)
 
             if plan_id is None and not opts.urn:
                 raise TypeError("Missing required property 'plan_id'")
             __props__.__dict__["plan_id"] = plan_id
             __props__.__dict__["service_id"] = service_id
             if start_command is None and not opts.urn:
                 raise TypeError("Missing required property 'start_command'")
             __props__.__dict__["start_command"] = start_command
             __props__.__dict__["created_at"] = None
             __props__.__dict__["finished_at"] = None
             __props__.__dict__["started_at"] = None
             __props__.__dict__["status"] = None
-        super(Job, __self__).__init__(
-            'render:services:Job',
+        super(Jobs, __self__).__init__(
+            'render:services:Jobs',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
-            opts: Optional[pulumi.ResourceOptions] = None) -> 'Job':
+            opts: Optional[pulumi.ResourceOptions] = None) -> 'Jobs':
         """
-        Get an existing Job resource's state with the given name, id, and optional extra
+        Get an existing Jobs resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = JobArgs.__new__(JobArgs)
+        __props__ = JobsArgs.__new__(JobsArgs)
 
         __props__.__dict__["created_at"] = None
         __props__.__dict__["finished_at"] = None
         __props__.__dict__["plan_id"] = None
         __props__.__dict__["start_command"] = None
         __props__.__dict__["started_at"] = None
         __props__.__dict__["status"] = None
-        return Job(resource_name, opts=opts, __props__=__props__)
+        return Jobs(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="createdAt")
     def created_at(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "created_at")
 
     @property
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/list_custom_domains.py` & `pulumi_render-0.1.1/pulumi_render/services/list_custom_domains.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     __args__ = dict()
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:listCustomDomains', __args__, opts=opts, typ=ListCustomDomainsResult).value
 
     return AwaitableListCustomDomainsResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(list_custom_domains)
 def list_custom_domains_output(service_id: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListCustomDomainsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/list_deploys.py` & `pulumi_render-0.1.1/pulumi_render/services/list_deploys.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     __args__ = dict()
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:listDeploys', __args__, opts=opts, typ=ListDeploysResult).value
 
     return AwaitableListDeploysResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(list_deploys)
 def list_deploys_output(service_id: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListDeploysResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/list_env_vars.py` & `pulumi_render-0.1.1/pulumi_render/services/list_env_vars.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
     __args__ = dict()
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:listEnvVars', __args__, opts=opts, typ=ListEnvVarsResult).value
 
     return AwaitableListEnvVarsResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(list_env_vars)
 def list_env_vars_output(service_id: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListEnvVarsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/list_jobs.py` & `pulumi_render-0.1.1/pulumi_render/services/list_jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     """
     __args__ = dict()
     __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('render:services:listJobs', __args__, opts=opts, typ=ListJobsResult).value
 
     return AwaitableListJobsResult(
-        items=__ret__.items)
+        items=pulumi.get(__ret__, 'items'))
 
 
 @_utilities.lift_output_func(list_jobs)
 def list_jobs_output(service_id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListJobsResult]:
     """
     Use this data source to access information about an existing resource.
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/list_service_headers.py` & `pulumi_render-0.1.1/pulumi_render/services/list_services.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,62 +5,56 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from ._enums import *
 
 __all__ = [
-    'ListServiceHeadersResult',
-    'AwaitableListServiceHeadersResult',
-    'list_service_headers',
-    'list_service_headers_output',
+    'ListServicesResult',
+    'AwaitableListServicesResult',
+    'list_services',
+    'list_services_output',
 ]
 
 @pulumi.output_type
-class ListServiceHeadersResult:
+class ListServicesResult:
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> Sequence['outputs.ListServiceHeadersResponse']:
+    def items(self) -> Sequence['outputs.ListServiceResponse']:
         return pulumi.get(self, "items")
 
 
-class AwaitableListServiceHeadersResult(ListServiceHeadersResult):
+class AwaitableListServicesResult(ListServicesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return ListServiceHeadersResult(
+        return ListServicesResult(
             items=self.items)
 
 
-def list_service_headers(service_id: Optional[str] = None,
-                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListServiceHeadersResult:
+def list_services(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListServicesResult:
     """
     Use this data source to access information about an existing resource.
-
-    :param str service_id: (Required) The ID of the service
     """
     __args__ = dict()
-    __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('render:services:listServiceHeaders', __args__, opts=opts, typ=ListServiceHeadersResult).value
+    __ret__ = pulumi.runtime.invoke('render:services:listServices', __args__, opts=opts, typ=ListServicesResult).value
 
-    return AwaitableListServiceHeadersResult(
-        items=__ret__.items)
+    return AwaitableListServicesResult(
+        items=pulumi.get(__ret__, 'items'))
 
 
-@_utilities.lift_output_func(list_service_headers)
-def list_service_headers_output(service_id: Optional[pulumi.Input[str]] = None,
-                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListServiceHeadersResult]:
+@_utilities.lift_output_func(list_services)
+def list_services_output(opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListServicesResult]:
     """
     Use this data source to access information about an existing resource.
-
-    :param str service_id: (Required) The ID of the service
     """
     ...
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/list_services.py` & `pulumi_render-0.1.1/pulumi_render/services/list_routes.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,44 +8,60 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 
 __all__ = [
-    'ListServicesResult',
-    'AwaitableListServicesResult',
-    'list_services',
+    'ListRoutesResult',
+    'AwaitableListRoutesResult',
+    'list_routes',
+    'list_routes_output',
 ]
 
 @pulumi.output_type
-class ListServicesResult:
+class ListRoutesResult:
     def __init__(__self__, items=None):
         if items and not isinstance(items, list):
             raise TypeError("Expected argument 'items' to be a list")
         pulumi.set(__self__, "items", items)
 
     @property
     @pulumi.getter
-    def items(self) -> Sequence['outputs.ListServiceResponse']:
+    def items(self) -> Sequence['outputs.ListStaticSiteRoutesResponse']:
         return pulumi.get(self, "items")
 
 
-class AwaitableListServicesResult(ListServicesResult):
+class AwaitableListRoutesResult(ListRoutesResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return ListServicesResult(
+        return ListRoutesResult(
             items=self.items)
 
 
-def list_services(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListServicesResult:
+def list_routes(service_id: Optional[str] = None,
+                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableListRoutesResult:
     """
     Use this data source to access information about an existing resource.
+
+    :param str service_id: (Required) The ID of the service
     """
     __args__ = dict()
+    __args__['serviceId'] = service_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('render:services:listServices', __args__, opts=opts, typ=ListServicesResult).value
+    __ret__ = pulumi.runtime.invoke('render:services:listRoutes', __args__, opts=opts, typ=ListRoutesResult).value
+
+    return AwaitableListRoutesResult(
+        items=pulumi.get(__ret__, 'items'))
 
-    return AwaitableListServicesResult(
-        items=__ret__.items)
+
+@_utilities.lift_output_func(list_routes)
+def list_routes_output(service_id: Optional[pulumi.Input[str]] = None,
+                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[ListRoutesResult]:
+    """
+    Use this data source to access information about an existing resource.
+
+    :param str service_id: (Required) The ID of the service
+    """
+    ...
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/outputs.py` & `pulumi_render-0.1.1/pulumi_render/services/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
 from ._enums import *
 
 __all__ = [
+    'AutoScalingCriteria',
+    'AutoScalingCriteriaSpec',
     'BackgroundWorker',
     'BackgroundWorkerServiceDetails',
     'BackgroundWorkerServiceDetailsParentServerProperties',
     'Commit',
     'CronJob',
     'CronJobServiceDetails',
     'CustomDomain',
@@ -51,14 +53,62 @@
     'StaticSiteServiceDetailsParentServerProperties',
     'WebService',
     'WebServiceServiceDetails',
     'WebServiceServiceDetailsParentServerProperties',
 ]
 
 @pulumi.output_type
+class AutoScalingCriteria(dict):
+    def __init__(__self__, *,
+                 cpu: Optional['outputs.AutoScalingCriteriaSpec'] = None,
+                 memory: Optional['outputs.AutoScalingCriteriaSpec'] = None):
+        if cpu is not None:
+            pulumi.set(__self__, "cpu", cpu)
+        if memory is not None:
+            pulumi.set(__self__, "memory", memory)
+
+    @property
+    @pulumi.getter
+    def cpu(self) -> Optional['outputs.AutoScalingCriteriaSpec']:
+        return pulumi.get(self, "cpu")
+
+    @property
+    @pulumi.getter
+    def memory(self) -> Optional['outputs.AutoScalingCriteriaSpec']:
+        return pulumi.get(self, "memory")
+
+
+@pulumi.output_type
+class AutoScalingCriteriaSpec(dict):
+    def __init__(__self__, *,
+                 enabled: Optional[bool] = None,
+                 percentage: Optional[float] = None):
+        """
+        :param float percentage: Determines when your service will be scaled. If the average resource utilization is significantly above/below the target, we will increase/decrease the number of instances.
+        """
+        if enabled is not None:
+            pulumi.set(__self__, "enabled", enabled)
+        if percentage is not None:
+            pulumi.set(__self__, "percentage", percentage)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> Optional[bool]:
+        return pulumi.get(self, "enabled")
+
+    @property
+    @pulumi.getter
+    def percentage(self) -> Optional[float]:
+        """
+        Determines when your service will be scaled. If the average resource utilization is significantly above/below the target, we will increase/decrease the number of instances.
+        """
+        return pulumi.get(self, "percentage")
+
+
+@pulumi.output_type
 class BackgroundWorker(dict):
     """
     A background worker service
     """
     def __init__(__self__, *,
                  name: str,
                  owner_id: str,
```

### Comparing `pulumi_render-0.0.47/pulumi_render/services/private_service.py` & `pulumi_render-0.1.1/pulumi_render/services/private_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render/services/scale.py` & `pulumi_render-0.1.1/pulumi_render/services/scale.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render/services/static_site.py` & `pulumi_render-0.1.1/pulumi_render/services/static_site.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render/services/suspend.py` & `pulumi_render-0.1.1/pulumi_render/services/suspend.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render/services/web_service.py` & `pulumi_render-0.1.1/pulumi_render/services/web_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_render-0.0.47/pulumi_render.egg-info/SOURCES.txt` & `pulumi_render-0.1.1/pulumi_render.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 README.md
-setup.py
+pyproject.toml
 pulumi_render/__init__.py
 pulumi_render/_utilities.py
 pulumi_render/provider.py
 pulumi_render/pulumi-plugin.json
 pulumi_render/py.typed
 pulumi_render.egg-info/PKG-INFO
 pulumi_render.egg-info/SOURCES.txt
 pulumi_render.egg-info/dependency_links.txt
-pulumi_render.egg-info/not-zip-safe
 pulumi_render.egg-info/requires.txt
 pulumi_render.egg-info/top_level.txt
 pulumi_render/config/__init__.py
+pulumi_render/config/__init__.pyi
 pulumi_render/config/vars.py
 pulumi_render/owners/__init__.py
 pulumi_render/owners/_enums.py
 pulumi_render/owners/get_owner.py
 pulumi_render/owners/list_owners.py
 pulumi_render/owners/outputs.py
+pulumi_render/registrycredentials/__init__.py
+pulumi_render/registrycredentials/get_registry_credential.py
+pulumi_render/registrycredentials/list_registry_credentials.py
+pulumi_render/registrycredentials/outputs.py
+pulumi_render/registrycredentials/registry_credential.py
 pulumi_render/services/__init__.py
 pulumi_render/services/_enums.py
 pulumi_render/services/_inputs.py
+pulumi_render/services/auto_scaling.py
 pulumi_render/services/background_worker.py
 pulumi_render/services/cron_job.py
-pulumi_render/services/custom_domain.py
-pulumi_render/services/deploy.py
-pulumi_render/services/env_var.py
+pulumi_render/services/custom_domains.py
+pulumi_render/services/deploys.py
+pulumi_render/services/env_vars.py
 pulumi_render/services/get_background_worker.py
 pulumi_render/services/get_cron_job.py
 pulumi_render/services/get_custom_domain.py
 pulumi_render/services/get_deploy.py
 pulumi_render/services/get_job.py
 pulumi_render/services/get_private_service.py
 pulumi_render/services/get_static_site.py
 pulumi_render/services/get_web_service.py
-pulumi_render/services/job.py
+pulumi_render/services/jobs.py
 pulumi_render/services/list_custom_domains.py
 pulumi_render/services/list_deploys.py
 pulumi_render/services/list_env_vars.py
+pulumi_render/services/list_headers.py
 pulumi_render/services/list_jobs.py
-pulumi_render/services/list_service_headers.py
+pulumi_render/services/list_routes.py
 pulumi_render/services/list_services.py
-pulumi_render/services/list_static_site_routes.py
 pulumi_render/services/outputs.py
 pulumi_render/services/private_service.py
 pulumi_render/services/scale.py
 pulumi_render/services/static_site.py
 pulumi_render/services/suspend.py
 pulumi_render/services/web_service.py
```

