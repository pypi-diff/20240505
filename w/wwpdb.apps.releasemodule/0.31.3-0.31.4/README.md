# Comparing `tmp/wwpdb.apps.releasemodule-0.31.3.tar.gz` & `tmp/wwpdb_apps_releasemodule-0.31.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.releasemodule-0.31.3.tar", last modified: Sun Mar 31 13:13:24 2024, max compression
+gzip compressed data, was "wwpdb_apps_releasemodule-0.31.4.tar", last modified: Sun May  5 19:51:21 2024, max compression
```

## Comparing `wwpdb.apps.releasemodule-0.31.3.tar` & `wwpdb_apps_releasemodule-0.31.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 13:13:24.037037 wwpdb.apps.releasemodule-0.31.3/
--rw-r--r--   0 vsts      (1001) docker     (127)     1210 2024-03-31 13:13:24.037037 wwpdb.apps.releasemodule-0.31.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       52 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-03-31 13:13:24.037037 wwpdb.apps.releasemodule-0.31.3/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2539 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 13:13:24.021037 wwpdb.apps.releasemodule-0.31.3/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 13:13:24.021037 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 13:13:24.021037 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 13:13:24.025037 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/
--rw-r--r--   0 vsts      (1001) docker     (127)    10466 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/Analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/CheckResult.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15867 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/CitationFinder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5284 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/FetchMP.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35275 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/FetchResultParser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4490 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/FetchUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/MatchMP.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2569 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/MatchUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8181 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14457 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6962 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/RisCitationParser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5050 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/SearchMP.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/SearchResultParser.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3216 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/SearchUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/StringUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 13:13:24.025037 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)     2904 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19491 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7724 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19597 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7582 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4158 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4437 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6443 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictRequest.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14638 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      894 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/test_DepictCitation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 13:13:24.033037 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/
--rw-r--r--   0 vsts      (1001) docker     (127)    12660 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/AutoReRelease.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12851 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13786 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/EmReleaseUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3069 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2600 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/EntryPullProcess.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25384 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/EntryUpdateBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25079 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3537 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/InputFormParser_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18581 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4828 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/NmrDataGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21730 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23671 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/ReleaseUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3479 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3773 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/UpdateBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22156 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/UpdateFormParser.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13024 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 13:13:24.033037 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)    24098 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/CombineDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22431 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/ContentDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7405 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/DbApiUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/JournalAbbrev.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6429 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/MessageBaseClass.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9550 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1574 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/MultiProcLimit.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6170 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3456 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12760 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/Utility.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 13:13:24.037037 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    47983 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-31 13:11:00.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-31 13:13:24.037037 wwpdb.apps.releasemodule-0.31.3/wwpdb.apps.releasemodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1210 2024-03-31 13:13:23.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb.apps.releasemodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-03-31 13:13:23.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb.apps.releasemodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-31 13:13:23.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb.apps.releasemodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-31 13:13:04.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb.apps.releasemodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      252 2024-03-31 13:13:23.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb.apps.releasemodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-03-31 13:13:23.000000 wwpdb.apps.releasemodule-0.31.3/wwpdb.apps.releasemodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.580123 wwpdb_apps_releasemodule-0.31.4/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1210 2024-05-05 19:51:21.580123 wwpdb_apps_releasemodule-0.31.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       52 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-05-05 19:51:21.580123 wwpdb_apps_releasemodule-0.31.4/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2539 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.556123 wwpdb_apps_releasemodule-0.31.4/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.556123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.560123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.564123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10466 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/Analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/CheckResult.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15867 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/CitationFinder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5284 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35275 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchResultParser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4490 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MatchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2569 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MatchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8181 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14457 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6962 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/RisCitationParser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5050 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchMP.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchResultParser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3216 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/StringUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.568123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2904 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19491 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7724 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19597 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7582 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4158 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4437 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6443 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14638 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      894 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/test_DepictCitation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.572123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/
+-rw-r--r--   0 vsts      (1001) docker     (127)    12660 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/AutoReRelease.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12851 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13786 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EmReleaseUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3069 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2611 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryPullProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25384 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryUpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25079 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3574 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/InputFormParser_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18623 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4828 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/NmrDataGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21730 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23671 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/ReleaseUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3479 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3773 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22156 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateFormParser.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13024 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.576123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)    24098 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/CombineDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22431 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/ContentDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7405 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/DbApiUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/JournalAbbrev.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6429 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/MessageBaseClass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9550 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1574 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/MultiProcLimit.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6170 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3456 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12760 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/Utility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.576123 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    47983 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:49:09.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:51:21.580123 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1210 2024-05-05 19:51:21.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-05-05 19:51:21.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 19:51:21.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 19:51:00.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      252 2024-05-05 19:51:21.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-05 19:51:21.000000 wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.releasemodule-0.31.3/PKG-INFO` & `wwpdb_apps_releasemodule-0.31.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.releasemodule
-Version: 0.31.3
+Version: 0.31.4
 Summary: wwPDB sequence module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_releasemodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.releasemodule-0.31.3/setup.cfg` & `wwpdb_apps_releasemodule-0.31.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/setup.py` & `wwpdb_apps_releasemodule-0.31.4/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/Analysis.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/Analysis.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/CheckResult.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/CheckResult.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/CitationFinder.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/CitationFinder.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/FetchMP.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchMP.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/FetchResultParser.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchResultParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/FetchUtil.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/FetchUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/MatchMP.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MatchMP.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/MatchUtil.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MatchUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/MonitorCitationUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/ReadCitationFinderResult_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/RisCitationParser.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/RisCitationParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/SearchMP.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchMP.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/SearchResultParser.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchResultParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/SearchUtil.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/SearchUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/citation/StringUtil.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/citation/StringUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictAnnotatorHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictBase.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictCitationForm_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictCitation_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictEntryHistory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictReleaseInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictRemovalMark.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/DepictRequest.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/DepictRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/ReleaseOption_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/depict/test_DepictCitation.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/depict/test_DepictCitation.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/AutoReRelease.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/AutoReRelease.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/CitationFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/EmReleaseUtil.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EmReleaseUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryFormParser_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/EntryPullProcess.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryPullProcess.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             #
             for item in ('em_release', 'release', 'start_files'):
                 if item in entryPickle:
                     del entryPickle[item]
                 #
             #
         #
-        self._insertEntryMessage(errType='all', errMessage='Pulled off from release.', messageType='info', uniqueFlag=True)
+        self._insertEntryMessage(errType='all', errMessage='Entry has been pulled from release.', messageType='info', uniqueFlag=True)
         self._updateDataBase()
         self._removeExistingForReleaseDirectories()
         self._finishAndDumpPickleFiles(entryPickle)
 
     def __rollArchivalFileBacktoSartingVersion(self, startFilesMap):
         for typeList in self._fileTypeList:
             if not typeList[3] in startFilesMap:
```

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/EntryUpdateBase.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryUpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/EntryUpdateProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/InputFormParser_v2.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/InputFormParser_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,10 +106,11 @@
             #
         #
         return False
 
     def __cleanString(self, val):
         val = val.replace(',', ' ')
         val = val.replace('\n', ' ')
+        val = val.replace('\r', ' ')
         val = val.replace('\t', ' ')
         val = val.strip()
         return val
```

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/MultiUpdateProcess.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
         annoIndexPickle['entryDir'] = entryDirs
         annoIndexPickle['eventList'] = eventLists
         self._dumpAnnotatorPickle(annoIndexPickle)
         self.__loadContentDataBase(dbLoadFileList)
         self.__updatePullbackEntryStatus(pullEntryIdList)
 
     def __getReturnContentForPullEntries(self):
+        self.__returnContent = "Task: " + self.__task
         for entryData in self.__updateList:
             self.__returnContent += '\n\nEntry ' + entryData['entry']
             if ('comb_ids' in entryData) and entryData['comb_ids']:
                 self.__returnContent += ' (' + entryData['comb_ids'] + ')'
             elif ('pdb_id' in entryData) and entryData['pdb_id']:
                 self.__returnContent += ' (' + entryData['pdb_id'] + ')'
             #
@@ -308,15 +309,15 @@
             #
         #
         self.__loadContentDataBase(dbLoadFileList)
         #
         if (not allSysErrors) and (not allContents):
             self.__errorContent += 'No update list found\n'
         else:
-            self.__returnContent = str(self._reqObj.getValue('task'))
+            self.__returnContent = "Task: " + self.__task
             if allSysErrors:
                 _msgType, msgText = self._getConcatMessageContent(allSysErrors)
                 self.__returnContent += '\n\nSystem related error:\n' + msgText
             #
             if allContents:
                 self.__returnContent += allContents
             #
```

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/NmrDataGenerator.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/NmrDataGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/ReleaseDpUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/ReleaseUtil.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/ReleaseUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/RunAutoReReleaseProcess.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/UpdateBase.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/UpdateFormParser.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateFormParser.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/update/UpdateUtil_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/CombineDbApi.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/CombineDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/ContentDbApi.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/ContentDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/DbApiUtil.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/DbApiUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/JournalAbbrev.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/JournalAbbrev.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/MessageBaseClass.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/MessageBaseClass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/ModuleBaseClass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/MultiProcLimit.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/MultiProcLimit.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/StatusDbApi_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/TimeUtil.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/utils/Utility.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/utils/Utility.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py` & `wwpdb_apps_releasemodule-0.31.4/wwpdb/apps/releasemodule/webapp/ReleaseWebApp_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb.apps.releasemodule.egg-info/PKG-INFO` & `wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.releasemodule
-Version: 0.31.3
+Version: 0.31.4
 Summary: wwPDB sequence module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_releasemodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.releasemodule-0.31.3/wwpdb.apps.releasemodule.egg-info/SOURCES.txt` & `wwpdb_apps_releasemodule-0.31.4/wwpdb.apps.releasemodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

