# Comparing `tmp/wwpdb.apps.entity_transform-0.18.tar.gz` & `tmp/wwpdb_apps_entity_transform-0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.entity_transform-0.18.tar", last modified: Fri Feb  9 12:10:21 2024, max compression
+gzip compressed data, was "wwpdb_apps_entity_transform-0.19.tar", last modified: Sun May  5 20:06:48 2024, max compression
```

## Comparing `wwpdb.apps.entity_transform-0.18.tar` & `wwpdb_apps_entity_transform-0.19.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.793744 wwpdb.apps.entity_transform-0.18/
--rw-r--r--   0 vsts      (1001) docker     (127)     1099 2024-02-09 12:10:21.793744 wwpdb.apps.entity_transform-0.18/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-02-09 12:10:21.793744 wwpdb.apps.entity_transform-0.18/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2439 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.769744 wwpdb.apps.entity_transform-0.18/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.769744 wwpdb.apps.entity_transform-0.18/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.773743 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.777743 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)     3008 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/DepictBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2941 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/LinkDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8058 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19491 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1905 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11023 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/ResultDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15972 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/SeqDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16966 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/StrFormDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11163 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.777743 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/openeye_util/
--rw-r--r--   0 vsts      (1001) docker     (127)    11226 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/openeye_util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.777743 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/
--rw-r--r--   0 vsts      (1001) docker     (127)     6367 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/BuildPrd.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7726 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5529 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/CVSCommit.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12737 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/DepictPrd.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12192 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/DepictUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3149 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/HtmlUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13935 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/ReadFormUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4392 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/UpdatePrd.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.785744 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/
--rw-r--r--   0 vsts      (1001) docker     (127)     7032 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/ChopperHandler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5210 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/CombineCoord.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2337 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/EditPolymer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/MergeLigand.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1225 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/MergePolymer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2335 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/SplitPolymer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7591 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/UpdateBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5386 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/UpdateFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.789744 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     8180 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/CommandUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3003 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/CompUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6851 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/DownloadFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)      687 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/GetLogMessage.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4253 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/ImageGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6104 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/LinkUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2191 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6825 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2748 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3391 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/mmCIFUtil.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.789744 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    55807 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/webapp/EntityWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6426 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/webapp/FormPreProcess.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:07:51.000000 wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-09 12:10:21.789744 wwpdb.apps.entity_transform-0.18/wwpdb.apps.entity_transform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1099 2024-02-09 12:10:21.000000 wwpdb.apps.entity_transform-0.18/wwpdb.apps.entity_transform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2601 2024-02-09 12:10:21.000000 wwpdb.apps.entity_transform-0.18/wwpdb.apps.entity_transform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-09 12:10:21.000000 wwpdb.apps.entity_transform-0.18/wwpdb.apps.entity_transform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-09 12:10:08.000000 wwpdb.apps.entity_transform-0.18/wwpdb.apps.entity_transform.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      194 2024-02-09 12:10:21.000000 wwpdb.apps.entity_transform-0.18/wwpdb.apps.entity_transform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-02-09 12:10:21.000000 wwpdb.apps.entity_transform-0.18/wwpdb.apps.entity_transform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1099 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2439 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.499478 wwpdb_apps_entity_transform-0.19/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.503478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.503478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/
+-rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.503478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3008 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/DepictBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2941 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/LinkDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8282 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19491 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1905 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11023 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ResultDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15972 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/SeqDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17261 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/StrFormDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11305 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.503478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/openeye_util/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11226 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/openeye_util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.503478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6367 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/BuildPrd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7726 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5529 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/CVSCommit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12737 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/DepictPrd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12192 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/DepictUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3149 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/HtmlUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13935 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/ReadFormUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4392 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/UpdatePrd.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7951 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/ChopperHandler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5917 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/CombineCoord.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2337 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/EditPolymer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1229 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/MergeLigand.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1225 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/MergePolymer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2335 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/SplitPolymer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7591 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/UpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5386 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/UpdateFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8180 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/CommandUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3003 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/CompUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6851 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/DownloadFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      687 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/GetLogMessage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4253 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/ImageGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6104 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/LinkUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2191 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6825 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2748 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3391 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/mmCIFUtil.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    55983 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/EntityWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6820 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/FormPreProcess.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:04:49.000000 wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 20:06:48.507478 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1099 2024-05-05 20:06:48.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2601 2024-05-05 20:06:48.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 20:06:48.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 20:06:36.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      194 2024-05-05 20:06:48.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-05 20:06:48.000000 wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.entity_transform-0.18/PKG-INFO` & `wwpdb_apps_entity_transform-0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.entity_transform
-Version: 0.18
+Version: 0.19
 Summary: wwPDB entity transformer
 Home-page: https://github.com/rcsb/py-wwpdb_apps_entity_transform
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.entity_transform-0.18/setup.py` & `wwpdb_apps_entity_transform-0.19/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/DepictBase.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/DepictBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/LinkDepict.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/LinkDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,30 +57,33 @@
         #
         text += self.__depiction(self.__data) + '\n'
         #
         text += '<li><a class="fltlft" href="/service/entity/summary_view?' + input_data + '" target="_blank"> Access to split or merge </a></li>\n'
         #
         if self.__splitPolymerResidueFlag:
             text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data + '&type=split" target="_blank"> ' \
-                + '<span style="color:red;">Split modified residue to standard residue + modification in polymer</span> </a></li>\n'
+                  + '<span style="color:red;">Split modified residue to standard residue + modification in polymer</span> </a></li>\n'
         #
         if self.__combResidueFlag:
             text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data + '&type=merge" target="_blank"> ' \
-                + '<span style="color:red;">Merge standard amino acid residue + modification to modified amino acid residue in polymer</span> </a></li>\n'
+                  + '<span style="color:red;">Merge standard amino acid residue + modification to modified amino acid residue in polymer</span> </a></li>\n'
         #
         if self.__matchResultFlag:
             text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data \
-                + '" target="_blank"> <span style="color:red;">View All Search Result(s)</span> </a></li>\n'
+                  + '" target="_blank"> <span style="color:red;">View All Search Result(s)</span> </a></li>\n'
         #
         if self.__graphmatchResultFlag:
             text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data \
-                + '&type=match" target="_blank"> Update Coordinate File with Match Result(s) </a></li>\n'
+                  + '&type=match" target="_blank"> Update Coordinate File with Match Result(s) </a></li>\n'
         #
         text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data \
-            + '&type=input" target="_blank"> Update Coordinate File with Input IDs </a></li>\n'
+              + '&type=input" target="_blank"> Update Coordinate File with Input IDs </a></li>\n'
+        #
+        text += '<li><a class="fltlft" href="/service/entity/result_view?' + input_data + '&type=split_with_input" target="_blank"> ' \
+              + 'Split non standard residue in polymer </a></li>\n'
         #
         text += '<li><a class="fltlft" href="/service/entity/download_file?' + input_data + '" target="_blank"> Download Files </a></li>\n'
         #
         text += '</ul>\n'
         #
         return text
```

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/ResultDepict.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/ResultDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/SeqDepict.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/SeqDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/StrFormDepict.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/StrFormDepict.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,21 @@
         myD['session_url_prefix'] = os.path.join(self._rltvSessionPath, 'search', myD['instanceid'])
         myD['processing_site'] = self.__cI.get('SITE_NAME').upper()
         #
         return self._processTemplate('chopper/editor_tmplt.html', myD)
 
     def __processSplitWithChopper(self, myD):
         ciffile = self._identifier + '_model_P1.cif'
-        combObj = CombineCoord(reqObj=self._reqObj, instList=[str(self._reqObj.getValue('split_polymer_residue'))], cifFile=ciffile,
-                               verbose=self._verbose, log=self._lfh)
-        combObj.processWithCopy()
+        residueId = str(self._reqObj.getValue('split_polymer_residue'))
+        if not residueId:
+            residueId = '_'.join([str(self._reqObj.getValue('chain_id')), str(self._reqObj.getValue('res_name')), \
+                                  str(self._reqObj.getValue('res_num')), str(self._reqObj.getValue('ins_code'))])
+        #
+        combObj = CombineCoord(reqObj=self._reqObj, instList=[residueId], cifFile=ciffile, verbose=self._verbose, log=self._lfh)
+        combObj.processWithCopy(submitValue=self.__submitValue)
         message = combObj.getMessage()
         #
         if message:
             myD['data'] = message
             return 'update_form/update_result_tmplt.html', myD
         #
         instId = combObj.getInstId()
```

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,16 @@
         #
         text += '</table>\n'
         return text
 
     def __depictionLigand(self):
         text = '<table>\n'
         text += '<tr>\n'
-        text += '<th>Selection/<br/>User Defined Group ID</th>\n'
+        text += '<th>Selection/<br/>User Defined Group ID<br/><input id="ligand_select_all" value="Select All" type="button" onClick="select_ligand(' \
+              + "'ligand_select_all'" + ');" /></th>\n'
         text += '<th>3 Letter Code</th>\n'
         text += '<th>Chain ID</th>\n'
         text += '<th>ResNum</th>\n'
         text += '<th>InsertCode</th>\n'
         text += '<th>Links</th>\n'
         text += '</tr>\n'
         #
```

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/BuildPrd.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/BuildPrd.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/CVSCommit.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/CVSCommit.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/DepictPrd.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/DepictPrd.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/DepictUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/DepictUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/HtmlUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/HtmlUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/ReadFormUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/ReadFormUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/prd/UpdatePrd.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/prd/UpdatePrd.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/ChopperHandler.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/ChopperHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 """
 __docformat__ = "restructuredtext en"
 __author__ = "Zukang Feng"
 __email__ = "zfeng@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.07"
 
+try:
+    import cPickle as pickle
+except ImportError:
+    import pickle as pickle
+#
+
 import os
 import sys
 
 from wwpdb.apps.entity_transform.utils.CommandUtil import CommandUtil
 from wwpdb.apps.entity_transform.utils.GetLogMessage import GetLogMessage
 
 
@@ -100,18 +106,37 @@
             return
         #
         self.__getLogMessage(logfile)
 
     def __searchOtherInstances(self):
         """ Get other instances list
         """
+        residue_id = ''
+        if self.__option == 'split_residue':
+            pickleFilePath = os.path.join(self.__instancePath, self.__instId + ".pkl")
+            if os.access(pickleFilePath, os.F_OK):
+                fb = open(pickleFilePath, "rb")
+                pickleD = pickle.load(fb)
+                fb.close()
+                #
+                if ('residue' in pickleD) and pickleD['residue']:
+                    residue_id = pickleD['residue']
+                #
+            #
+        #
+        self.__lfh.write("residue_id=%s\n" % residue_id)
         searchPath = os.path.join(self.__sessionPath, 'search')
         extraOptions = ' -summaryfile ' + self.__summaryFile + ' -searchpath ' + searchPath + ' -merge_cif ' + self.__instId \
             + '.merge.cif -chopper_cif ' + os.path.join(self.__instancePath, 'chopper_output.cif') + ' '
         #
+        if residue_id != '':
+            identifier = str(self.__reqObj.getValue("identifier"))
+            ciffile = os.path.join(self.__sessionPath, identifier + '_model_P1.cif')
+            extraOptions += ' -residue_id ' + residue_id + ' -model_cif ' + ciffile
+        #
         self.__cmdUtil.setSessionPath(self.__instancePath)
         self.__cmdUtil.runAnnotCmd('SearchAllInstances', '', self.__instId + '.all_instance_search.list',
                                    'search-instances.log', 'search-instances.clog', extraOptions)
         #
         filename = os.path.join(self.__instancePath, self.__instId + '.all_instance_search.list')
         if not os.access(filename, os.F_OK):
             return
```

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/CombineCoord.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/CombineCoord.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 """
 __docformat__ = "restructuredtext en"
 __author__ = "Zukang Feng"
 __email__ = "zfeng@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.07"
 
+try:
+    import cPickle as pickle
+except ImportError:
+    import pickle as pickle
+#
+
 import os
 import shutil
 import sys
 
 from wwpdb.apps.entity_transform.utils.CommandUtil import CommandUtil
 from wwpdb.apps.entity_transform.utils.GetLogMessage import GetLogMessage
 #
@@ -41,14 +47,15 @@
         self.__reqObj = reqObj
         self.__instList = instList
         self.__cifFile = cifFile
         self.__sObj = None
         self.__sessionPath = None
         self.__instId = ''
         self.__message = ''
+        self.__submitValue = ''
         #
         self.__getSession()
         self.__getInstId()
         #
         self.__instancePath = os.path.join(self.__sessionPath, self.__instId)
         #
         self.__cmdUtil = CommandUtil(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
@@ -58,15 +65,30 @@
         self.__runCombineScript()
         #
         if self.__message:
             return
         #
         self.__runUpdateScript()
 
-    def processWithCopy(self):
+    def processWithCopy(self, submitValue=''):
+        #
+        self.__submitValue = submitValue
+        #
+        if self.__submitValue and (len(self.__instList) == 1) and self.__instList[0]:
+            pickleFilePath = os.path.join(self.__instancePath, self.__instId + ".pkl")
+            if os.access(pickleFilePath, os.F_OK):
+                 os.remove(pickleFilePath)
+            #
+            pickleD = {}
+            pickleD['residue'] = self.__instList[0]
+            pickleD['submit'] = self.__submitValue
+            #
+            fb = open(pickleFilePath, "wb")
+            pickle.dump(pickleD, fb)
+            fb.close()
         #
         if not self.__runCopyScript():
             self.__runCombineScript()
         #
         if self.__message:
             return
         #
@@ -118,15 +140,14 @@
             return False
         #
         for ext in ('.orig.cif', '.merge.cif', '.comp.cif'):
             source = os.path.join(self.__sessionPath, 'search', self.__instList[0], self.__instList[0] + ext)
             if not os.access(source, os.F_OK):
                 return False
             #
-            #
             shutil.copyfile(source, os.path.join(self.__instancePath, self.__instId + ext))
         #
         return True
 
     def __runUpdateScript(self):
         """
         """
```

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/EditPolymer.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/EditPolymer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/MergeLigand.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/MergeLigand.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/MergePolymer.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/MergePolymer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/SplitPolymer.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/SplitPolymer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/UpdateBase.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/UpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/update/UpdateFile.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/update/UpdateFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/CommandUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/CommandUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/CompUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/CompUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/DownloadFile.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/DownloadFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/GetLogMessage.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/GetLogMessage.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/ImageGenerator.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/ImageGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/LinkUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/LinkUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/utils/mmCIFUtil.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/utils/mmCIFUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/webapp/EntityWebApp.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/EntityWebApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -789,47 +789,49 @@
         self.__getSession()
         self.__updateFileId()
         #
         self.__reqObj.setReturnFormat(return_format="html")
         rC = ResponseContent(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
         #
         instId = str(self.__reqObj.getValue("instanceid"))
-        type = str(self.__reqObj.getValue("type"))  # pylint: disable=redefined-builtin
+        viewType = str(self.__reqObj.getValue("type"))  # pylint: disable=redefined-builtin
         resultObj = None
         if self.__summaryCifObj:
             resultObj = ResultDepict(reqObj=self.__reqObj, summaryCifObj=self.__summaryCifObj, verbose=self.__verbose, log=self.__lfh)
         #
         myD = {}
         myD['sessionid'] = self.__sessionId
         myD['identifier'] = self.__identifier
         myD['title'] = self.__title
         myD['pdbid'] = self.__reqObj.getValue('pdbid')
         myD['label'] = self.__reqObj.getValue('label')
-        if type == 'match':
+        if viewType == 'match':
             if resultObj:
                 myD['form_data'] = resultObj.DoRenderUpdatePage()
             else:
                 myD['form_data'] = 'Can not find summary result file.'
             #
             rC.setHtmlText(self.__processTemplate('update_form/update_match_tmplt.html', myD))
-        elif type == 'input':
+        elif viewType == 'input':
             if resultObj:
                 myD['form_data'] = resultObj.DoRenderInputPage()
             else:
                 myD['form_data'] = 'Can not find summary result file.'
             #
             rC.setHtmlText(self.__processTemplate('update_form/update_user_input_tmplt.html', myD))
-        elif type == 'split':
+        elif viewType == 'split':
             if resultObj:
                 myD['form_data'] = resultObj.DoRenderSplitPage()
             else:
                 myD['form_data'] = '<tr><td colspan="6">Can not find summary result file.</td></tr>'
             #
             rC.setHtmlText(self.__processTemplate('summary_view/split_polymer_residue_tmplt.html', myD))
-        elif type == 'merge':
+        elif viewType == 'split_with_input':
+            rC.setHtmlText(self.__processTemplate('summary_view/split_polymer_residue_input_tmplt.html', myD))
+        elif viewType == 'merge':
             if resultObj:
                 myD['form_data'] = resultObj.DoRenderMergePage()
             else:
                 myD['form_data'] = '<tr><td colspan="5">Can not find summary result file.</td></tr>'
             #
             rC.setHtmlText(self.__processTemplate('update_form/update_merge_polymer_residue_tmplt.html', myD))
         else:
```

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb/apps/entity_transform/webapp/FormPreProcess.py` & `wwpdb_apps_entity_transform-0.19/wwpdb/apps/entity_transform/webapp/FormPreProcess.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,29 +34,37 @@
         #
         self.__submitValue = str(self.__reqObj.getValue('submit'))
         self.__entityList = self.__reqObj.getValueList('entity')
         self.__chainList = self.__reqObj.getValueList('chain')
         self.__ligandList = self.__reqObj.getValueList('ligand')
         self.__groupList = self.__reqObj.getValueList('group')
         self.__splitPolymerResidue = str(self.__reqObj.getValue('split_polymer_residue'))
+        self.__chainID = str(self.__reqObj.getValue('chain_id'))
+        self.__resName = str(self.__reqObj.getValue('res_name'))
+        self.__resNum = str(self.__reqObj.getValue('res_num'))
         #
         self.__errorMessage = ''
         #
         self.__labelDic = {}
         self.__valueDic = {}
         self.__preProcessForm()
         #
 
     def __preProcessForm(self):
         #
         # Check for non standard residue
         #
         if self.__submitValue == 'Split with chopper':
-            if not self.__splitPolymerResidue:
+            hasResidueSelected = False
+            if self.__splitPolymerResidue or (self.__chainID and self.__resName and self.__resNum):
+                hasResidueSelected = True
+            #
+            if not hasResidueSelected:
                 self.__errorMessage = 'No residue selected'
+            #
             return
         #
         # Check no values
         #
         if (not self.__entityList) and (not self.__chainList) and \
            (not self.__ligandList) and (not self.__groupList):
             self.__errorMessage = 'No polymer/non-polymer selected'
```

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb.apps.entity_transform.egg-info/PKG-INFO` & `wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.entity_transform
-Version: 0.18
+Version: 0.19
 Summary: wwPDB entity transformer
 Home-page: https://github.com/rcsb/py-wwpdb_apps_entity_transform
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.entity_transform-0.18/wwpdb.apps.entity_transform.egg-info/SOURCES.txt` & `wwpdb_apps_entity_transform-0.19/wwpdb.apps.entity_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

