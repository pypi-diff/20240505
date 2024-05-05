# Comparing `tmp/wwpdb_apps_ann_tasks_v2-0.37.3.tar.gz` & `tmp/wwpdb_apps_ann_tasks_v2-0.37.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_apps_ann_tasks_v2-0.37.3.tar", last modified: Fri Apr 12 17:50:21 2024, max compression
+gzip compressed data, was "wwpdb_apps_ann_tasks_v2-0.37.4.tar", last modified: Sun May  5 19:37:31 2024, max compression
```

## Comparing `wwpdb_apps_ann_tasks_v2-0.37.3.tar` & `wwpdb_apps_ann_tasks_v2-0.37.4.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.661778 wwpdb_apps_ann_tasks_v2-0.37.3/
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-12 17:50:21.661778 wwpdb_apps_ann_tasks_v2-0.37.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-12 17:50:21.661778 wwpdb_apps_ann_tasks_v2-0.37.3/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2540 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.645779 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/
--rw-r--r--   0 vsts      (1001) docker     (127)    39726 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46849 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/
--rw-r--r--   0 vsts      (1001) docker     (127)     5712 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/Check.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7708 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4947 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4344 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3138 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6865 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/
--rw-r--r--   0 vsts      (1001) docker     (127)     3045 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33886 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16936 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/density/
--rw-r--r--   0 vsts      (1001) docker     (127)      998 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/density/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)     3945 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/
--rw-r--r--   0 vsts      (1001) docker     (127)     2573 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4448 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4053 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19613 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5646 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/
--rw-r--r--   0 vsts      (1001) docker     (127)     6295 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14499 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2942 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3345 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12364 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12679 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/
--rw-r--r--   0 vsts      (1001) docker     (127)    10620 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12969 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18806 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11248 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/
--rw-r--r--   0 vsts      (1001) docker     (127)    15912 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9923 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/link/
--rw-r--r--   0 vsts      (1001) docker     (127)     3057 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/link/Link.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/link/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/
--rw-r--r--   0 vsts      (1001) docker     (127)     3231 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4323 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3336 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4763 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5394 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4764 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3305 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3716 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3561 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nafeatures/
--rw-r--r--   0 vsts      (1001) docker     (127)     2610 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/
--rw-r--r--   0 vsts      (1001) docker     (127)    21849 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6954 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8475 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3526 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/
--rw-r--r--   0 vsts      (1001) docker     (127)     1540 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2010 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/Related.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4025 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/
--rw-r--r--   0 vsts      (1001) docker     (127)     8209 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24946 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/
--rw-r--r--   0 vsts      (1001) docker     (127)     8612 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    81504 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33069 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/secstruct/
--rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/site/
--rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/site/Site.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/site/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/solvent/
--rw-r--r--   0 vsts      (1001) docker     (127)     3037 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/status/
--rw-r--r--   0 vsts      (1001) docker     (127)    33282 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/status/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/transformCoord/
--rw-r--r--   0 vsts      (1001) docker     (127)     3759 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     6619 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6242 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3600 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1509 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3451 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4026 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8388 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3396 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4790 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3021 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4071 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3062 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3053 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/validate/
--rw-r--r--   0 vsts      (1001) docker     (127)    10304 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/validate/Validate.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/validate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/view3d/
--rw-r--r--   0 vsts      (1001) docker     (127)     5085 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)     5627 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46092 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)   178553 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15293 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65098 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16955 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.661778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-12 17:50:21.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     5537 2024-04-12 17:50:21.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 17:50:21.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 17:49:39.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-04-12 17:50:21.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-12 17:50:21.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2540 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.502959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/
+-rw-r--r--   0 vsts      (1001) docker     (127)    39726 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46849 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5712 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/Check.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7708 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4947 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4344 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3138 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6865 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3045 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33977 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16936 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/density/
+-rw-r--r--   0 vsts      (1001) docker     (127)      998 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/density/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3945 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.506959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2573 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4448 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4053 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19613 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5646 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6295 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14499 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2942 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3345 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12364 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12679 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10620 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12969 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18806 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11248 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15912 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9923 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/link/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3057 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/link/Link.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/link/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3231 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4323 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3336 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4763 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5394 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4764 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3305 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3716 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3561 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nafeatures/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2610 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/
+-rw-r--r--   0 vsts      (1001) docker     (127)    21849 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6954 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8475 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3526 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.510959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1540 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2010 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/Related.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4025 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8902 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25640 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8612 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1983 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/LinksReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    79069 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34873 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/secstruct/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/site/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/site/Site.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/site/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/solvent/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3037 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/status/
+-rw-r--r--   0 vsts      (1001) docker     (127)    33282 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/status/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/transformCoord/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3759 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.514959 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6619 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6242 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3600 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1509 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3451 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4026 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8388 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3396 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4790 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3021 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4071 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3062 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3053 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/validate/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10304 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/validate/Validate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/validate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/view3d/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5085 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5627 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46092 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   179598 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15321 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    65098 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16955 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-05 19:35:15.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-05 19:37:31.518960 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-05 19:37:31.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5590 2024-05-05 19:37:31.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 19:37:31.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-05 19:36:48.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-05-05 19:37:31.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-05 19:37:31.000000 wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/PKG-INFO` & `wwpdb_apps_ann_tasks_v2-0.37.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ann_tasks_v2
-Version: 0.37.3
+Version: 0.37.4
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/setup.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/Check.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/Check.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,22 +568,24 @@
                 #
                 checked_count += 1
                 text += "\n" + str(checked_count) + ". " + qdir["question"] + "\n" + self.__getLigandText(qdir["text"]) + "\n"
             else:
                 if not qdir["question"] in selectD:
                     continue
                 #
+                checked_count += 1
+                #
                 context = ""
                 if "text" in qdir:
                     context = qdir["text"] % self.__corresInfo
+                    context = context.replace("$$$", str(checked_count))
                 #
                 if (qdir["question"] in additionalD) and ("additional_text" in qdir) and qdir["additional_text"]:
                     context += "\n\n" + qdir["additional_text"]
                 #
-                checked_count += 1
                 text += "\n" + str(checked_count) + ". "
                 if not qdir["question"].startswith("Free text question"):
                     text += qdir["question"] + "\n\n"
                 #
                 text += context + "\n\n"
             #
         #
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/PisaReader.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/io/PisaReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/link/Link.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/link/Link.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/Related.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/Related.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 __version__ = "V0.01"
 
 import os
 import shutil
 import sys
 import traceback
 
-from wwpdb.apps.ann_tasks_v2.report.styles.PdbxIo import PdbxReportIo, PdbxGeometryReportIo, PdbxXrayExpReportIo
+from wwpdb.apps.ann_tasks_v2.report.styles.PdbxIo import PdbxReportIo, PdbxGeometryReportIo, PdbxXrayExpReportIo, PdbxLinksReportIo
 from mmcif_utils.style.PdbxGeometryReportCategoryStyle import PdbxGeometryReportCategoryStyle
 
 from wwpdb.apps.ann_tasks_v2.report.PdbxReportDepictBootstrap import PdbxReportDepictBootstrap
 from wwpdb.apps.ann_tasks_v2.report.styles.DCCReport import PdbxXrayExpReportCategoryStyle
 from wwpdb.apps.ann_tasks_v2.report.styles.ModelReport import PdbxReportCategoryStyle
+from wwpdb.apps.ann_tasks_v2.report.styles.LinksReport import PdbxLinksReportCategoryStyle
 
 
 class PdbxReport(object):
     """PDBx report generator functions."""
 
     def __init__(self, reqObj, verbose=False, log=sys.stderr):
         """PRD report generator.
@@ -105,14 +106,20 @@
                 oL = rdd.render(dd, style=layout, leadingHtmlL=leadingHtmlL, trailingHtmlL=trailingHtmlL)
 
             if contentType in ["geometry-check-report"]:
                 self.setFilePath(filePath, fileFormat=fileFormat, idCode=idCode)
                 dd = self.doReport(contentType)
                 rdd = PdbxReportDepictBootstrap(styleObject=PdbxGeometryReportCategoryStyle(), includePath=includePath, verbose=self.__verbose, log=self.__lfh)
                 oL = rdd.render(dd, style=layout, leadingHtmlL=leadingHtmlL, trailingHtmlL=trailingHtmlL)
+            
+            if contentType in ["links-report"]:
+                self.setFilePath(filePath, fileFormat=fileFormat, idCode=idCode)
+                dd = self.doReport(contentType)
+                rdd = PdbxReportDepictBootstrap(styleObject=PdbxLinksReportCategoryStyle(), includePath=includePath, verbose=self.__verbose, log=self.__lfh)
+                oL = rdd.render(dd, style=layout, leadingHtmlL=leadingHtmlL, trailingHtmlL=trailingHtmlL)
 
             if self.__debug:
                 self.__lfh.write("+PdbxReport.makeTabularReport - generated HTML \n%s\n" % "\n".join(oL))
 
         return oL
 
     def setFilePath(self, filePath, fileFormat="cif", idCode=None):
@@ -169,14 +176,16 @@
         try:
             if contentType == "model":
                 pdbxR = PdbxReportIo(verbose=self.__verbose, log=self.__lfh)
             elif contentType == "geometry-check-report":
                 pdbxR = PdbxGeometryReportIo(verbose=self.__verbose, log=self.__lfh)
             elif contentType == "dcc-report":
                 pdbxR = PdbxXrayExpReportIo(verbose=self.__verbose, log=self.__lfh)
+            elif contentType == "links-report":
+                pdbxR = PdbxLinksReportIo(verbose=self.__verbose, log=self.__lfh)
 
             pdbxR.setFilePath(localPath, idCode=None)
             pdbxR.get()
             oD["blockId"] = pdbxR.getCurrentContainerId()
             if self.__verbose:
                 self.__lfh.write("+PdbxReport.doReport() - category name list %r \n" % pdbxR.getCurrentCategoryNameList())
             for catName in pdbxR.getCurrentCategoryNameList():
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 class PdbxReportDepictBootstrap(PdbxDepictBootstrapBase):
     """Create tabular HTML reports from PDBx data files.
 
     This version uses Bootstrap CSS framework constructs.
 
     """
+    MAX_LINES = 12
 
     def __init__(self, styleObject=None, includePath=None, verbose=False, log=sys.stderr):
         """
         :param `styleObject`:  object containing report data and formatting details.
         :param `includePath`:  path to web application html include files.
         :param `verbose`:      boolean flag to activate verbose logging.
         :param `log`:          stream for logging.
@@ -92,15 +93,14 @@
                 ("pdbx_SG_project", "Structural genomics", "row-wise"),
                 ("pdbx_database_related", "Related entries", "row-wise"),
                 ("pdbx_initial_refinement_model", "Starting models", "row-wise"),
                 ("pdbx_contact_author", "Contact authors", "row-wise"),
                 # ('citation','Primary citation','column-wise'),
                 ("pdbx_validate_close_contact", "Close contacts", "row-wise"),
                 ("pdbx_validate_symm_contact", "Close symmetry contacts", "row-wise"),
-                ("struct_conn", "Links", "row-wise"),
                 # ('symmetry', 'Symmetry', 'row-wise'),
                 # ('cell', 'Cell constants', 'row-wise'),
                 # ('exptl_crystal_grow', 'Crystallization details', 'row-wise'),
                 # ('diffrn_source','Data collection (source details)','row-wise'),
                 # ('diffrn_detector','Data collection (detector details)','row-wise'),
                 # ('reflns', 'Reflection statistics','row-wise'),
                 # ('reflns_shell','Reflection shell statistics','row-wise'),
@@ -128,14 +128,18 @@
                 ("pdbx_validate_rmsd_angle", "Bond angle RMSD", "row-wise"),
                 ("pdbx_validate_torsion", "Torsion outliers", "row-wise"),
                 ("pdbx_validate_peptide_omega", "Omega bond", "row-wise"),
                 ("pdbx_validate_main_chain_plane", "Main chain planarity", "row-wise"),
                 ("pdbx_validate_polymer_linkage", "Polymer linkages", "row-wise"),
                 ("pdbx_validate_chiral", "Chirality exceptions", "row-wise"),
             ]
+        elif self.__st.getStyleId() in ["PDBX_LINKS_REPORT_V1"]:
+            self.__reportCategories = [
+                ("struct_conn", "", "row-wise"),
+            ]
 
     def render(self, eD, style="tabs", leadingHtmlL=None, trailingHtmlL=None):
         """ """
         if style in ["tabs"]:
             return self.__doRenderTabs(eD)
         elif style in ["accordion", "multiaccordion"]:
             return self.__doRenderAccordion(eD)
@@ -322,15 +326,19 @@
 
                 if isMulti:
                     oL.append('<a class="accordion-toggle" data-toggle="collapse" href="#%s"> <h4>%s</h4></a>' % (idSection, abbrev))
                 else:
                     oL.append('<a class="accordion-toggle" data-toggle="collapse" data-parent="#%s" href="#%s"><h4>%s</h4></a>' % (idTop, idSection, abbrev))
                 oL.append("</div>")
                 oL.append('<div id="%s" class="accordion-body collapse %s">' % (idSection, active))
-                oL.append('<div  class="accordion-inner">')
+
+                if len(cD[catName]) > PdbxReportDepictBootstrap.MAX_LINES:
+                    oL.append('<div  class="accordion-inner" style="max-height: 50vh; overflow-y: scroll;">')
+                else:
+                    oL.append('<div  class="accordion-inner">')
                 #
                 oL.append('<table class="table table-striped table-bordered table-condensed">')
                 if catStyle == "column-wise":
                     self.__renderTableColumnWise(catName, cD[catName][0], oL)
                 else:
                     self.__renderTableRowWise(catName, cD[catName], oL)
                 oL.append("</table>")
@@ -526,14 +534,23 @@
             if itemName in rD:
                 itemValue = rD[itemName]
                 if len(itemValue) >= 3:
                     rD[itemName] = '<a target="_blank" href="http://ligand-expo.rcsb.org/pyapps/ldHandler.py?formid=cc-index-search&operation=ccid&target=%s">%s</a>' % (
                         itemValue,
                         itemValue,
                     )
+        
+        if catName == "struct_conn":
+            itemName = "_struct_conn.id"
+            if itemName in rD:
+                itemValue = rD[itemName]
+                rD[itemName] = '<a href="#" onclick="inspect(\'%s\'); return false;">%s</button>' % (
+                    itemValue.strip(),
+                    itemValue,
+                )
 
     def __attributePart(self, name):
         i = name.find(".")
         if i == -1:
             return None
         else:
             return name[i + 1 :]
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
         ("refine_hist", "table"),
         ("struct", "table"),
         ("struct_asym", "table"),
         ("struct_biol_gen", "table"),
         ("struct_conf", "table"),
         ("struct_conf_type", "table"),
         ("pdbx_struct_mod_residue", "table"),
-        ("struct_conn", "table"),
         ("struct_conn_type", "table"),
         ("struct_ncs_oper", "table"),
         ("struct_sheet", "table"),
         ("struct_sheet_order", "table"),
         ("struct_sheet_range", "table"),
         ("pdbx_struct_sheet_hbond", "table"),
         ("diffrn_radiation_wavelength", "table"),
@@ -1023,51 +1022,14 @@
             ("_pdbx_struct_mod_residue.auth_asym_id", "%s", "str", ""),
             ("_pdbx_struct_mod_residue.auth_seq_id", "%s", "str", ""),
             ("_pdbx_struct_mod_residue.auth_comp_id", "%s", "str", ""),
             ("_pdbx_struct_mod_residue.PDB_ins_code", "%s", "str", ""),
             ("_pdbx_struct_mod_residue.parent_comp_id", "%s", "str", ""),
             ("_pdbx_struct_mod_residue.details", "%s", "str", ""),
         ],
-        "struct_conn": [
-            # ('_struct_conn.id', '%s', 'str', ''),
-            ("_struct_conn.conn_type_id", "%s", "str", ""),
-            ("_struct_conn.pdbx_dist_value", "%s", "str", ""),
-            # ('_struct_conn.pdbx_PDB_id', '%s', 'str', ''),
-            # ('_struct_conn.pdbx_ptnr1_mod_name', '%s', 'str', ''),
-            # ('_struct_conn.pdbx_ptnr1_replaced_atom', '%s', 'str', ''),
-            ("_struct_conn.ptnr1_label_asym_id", "%s", "str", ""),
-            ("_struct_conn.ptnr1_label_comp_id", "%s", "str", ""),
-            # ('_struct_conn.ptnr1_label_seq_id', '%s', 'str', ''),
-            ("_struct_conn.ptnr1_auth_seq_id", "%s", "str", ""),
-            ("_struct_conn.ptnr1_label_atom_id", "%s", "str", ""),
-            # ('_struct_conn.pdbx_ptnr1_standard_comp_id', '%s', 'str', ''),
-            ("_struct_conn.ptnr1_symmetry", "%s", "str", ""),
-            ("_struct_conn.ptnr2_label_asym_id", "%s", "str", ""),
-            ("_struct_conn.ptnr2_label_comp_id", "%s", "str", ""),
-            ("_struct_conn.ptnr2_auth_seq_id", "%s", "str", ""),
-            # ('_struct_conn.ptnr2_label_seq_id', '%s', 'str', ''),
-            ("_struct_conn.ptnr2_label_atom_id", "%s", "str", ""),
-            ("_struct_conn.ptnr2_symmetry", "%s", "str", ""),
-            ("_struct_conn.pdbx_ptnr1_label_alt_loc", "%s", "str", ""),
-            ("_struct_conn.pdbx_ptnr1_label_ins_code", "%s", "str", ""),
-            ("_struct_conn.pdbx_ptnr2_label_alt_loc", "%s", "str", ""),
-            ("_struct_conn.pdbx_ptnr2_label_ins_code", "%s", "str", ""),
-            ("_struct_conn.ptnr1_auth_asym_id", "%s", "str", ""),
-            ("_struct_conn.ptnr1_auth_comp_id", "%s", "str", ""),
-            ("_struct_conn.ptnr2_auth_asym_id", "%s", "str", ""),
-            ("_struct_conn.ptnr2_auth_comp_id", "%s", "str", ""),
-            # ('_struct_conn.pdbx_ptnr3_label_atom_id', '%s', 'str', ''),
-            # ('_struct_conn.pdbx_ptnr3_label_seq_id', '%s', 'str', ''),
-            # ('_struct_conn.pdbx_ptnr3_label_comp_id', '%s', 'str', ''),
-            # ('_struct_conn.pdbx_ptnr3_label_asym_id', '%s', 'str', ''),
-            # ('_struct_conn.pdbx_ptnr3_label_alt_loc', '%s', 'str', ''),
-            # ('_struct_conn.pdbx_ptnr3_label_ins_code', '%s', 'str', ''),
-            ("_struct_conn.details", "%s", "str", ""),
-            ("_struct_conn.pdbx_value_order", "%s", "str", ""),
-        ],
         "struct_conn_type": [("_struct_conn_type.id", "%s", "str", ""), ("_struct_conn_type.criteria", "%s", "str", ""), ("_struct_conn_type.reference", "%s", "str", "")],
         "struct_ncs_oper": [
             ("_struct_ncs_oper.id", "%s", "str", ""),
             ("_struct_ncs_oper.code", "%s", "str", ""),
             ("_struct_ncs_oper.details", "%s", "str", ""),
             ("_struct_ncs_oper.matrix[1][1]", "%s", "str", ""),
             ("_struct_ncs_oper.matrix[1][2]", "%s", "str", ""),
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from mmcif_utils.style.PdbxStyleIoUtil import PdbxStyleIoUtil
 
 # from mmcif_utils.style.PdbxXrayExpReportCategoryStyle import PdbxXrayExpReportCategoryStyle
 from wwpdb.apps.ann_tasks_v2.report.styles.DCCReport import PdbxXrayExpReportCategoryStyle
 
 # from mmcif_utils.style.PdbxReportCategoryStyle import PdbxReportCategoryStyle
 from wwpdb.apps.ann_tasks_v2.report.styles.ModelReport import PdbxReportCategoryStyle
+from wwpdb.apps.ann_tasks_v2.report.styles.LinksReport import PdbxLinksReportCategoryStyle
 
 logger = logging.getLogger()
 
 
 class PdbxReportIo(PdbxStyleIoUtil):
     """Methods for reading PDBx data files for reporting applications including style details."""
 
@@ -129,14 +130,64 @@
             vals = catObj.selectValuesWhere("contour_level", mapId, "type")
             return self._firstOrDefault(vals, default="")
         except Exception as e:
             logging.error(e)
             return ""
 
 
+class PdbxLinksReportIo(PdbxStyleIoUtil):
+    """Methods for reading PDBx data files for reporting including style details. Specific to link information."""
+
+    def __init__(self, verbose=True, log=sys.stderr):
+        super(PdbxLinksReportIo, self).__init__(styleObject=PdbxLinksReportCategoryStyle(), verbose=verbose, log=log)
+        self.__lfh = log
+        self.__filePath = None
+        self.__idCode = None
+
+    def getCategory(self, catName="entity"):
+        return self.getItemDictList(catName)
+
+    def setFilePath(self, filePath, idCode=None):
+        """Specify the file path for the target and optionally provide an identifier
+        for the data section within the file.
+        """
+        self.__filePath = filePath
+        self.__idCode = idCode
+        if self.readFile(self.__filePath):
+            if self.__idCode is not None:
+                return self.setContainer(containerName=self.__idCode)
+            else:
+                return self.setContainer(containerIndex=0)
+        else:
+            return False
+
+    def get(self):
+        """
+        Check for a valid current data container.
+
+        Returns True for success or False otherwise.
+        """
+        return self.getCurrentContainerId() is not None
+
+    def complyStyle(self):
+        return self.testStyleComplete(self.__lfh)
+
+    def setBlock(self, blockId):
+        return self.setContainer(containerName=blockId)
+
+    def newBlock(self, blockId):
+        return self.newContainer(containerName=blockId)
+
+    def update(self, catName, attributeName, value, iRow=0):
+        return self.updateAttribute(catName, attributeName, value, iRow=iRow)
+
+    def write(self, filePath):
+        return self.writeFile(filePath)
+
+
 class PdbxGeometryReportIo(PdbxStyleIoUtil):
     """Methods for reading PDBx geometry data files for reporting applications including style details."""
 
     def __init__(self, verbose=True, log=sys.stderr):
         super(PdbxGeometryReportIo, self).__init__(styleObject=PdbxGeometryReportCategoryStyle(), verbose=verbose, log=log)
 
         # self.__verbose = verbose
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/site/Site.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/site/Site.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/validate/Validate.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/validate/Validate.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,17 +195,17 @@
             #
             if self.__validateArgs is not None:
                 dp.addInput(name="validate_arguments", value=self.__validateArgs)
             dp.op("annot-wwpdb-validate-all-sf")
             dp.expLog(logPath)
             dp.expList(dstPathList=[resultPdfPath, resultXmlPath, resultFullPdfPath, resultPngPath, resultSvgPath, resultImageTarPath, resultCifPath, resultFoPath, result2FoPath])
 
+            self.addDownloadPath(resultFullPdfPath)
             self.addDownloadPath(resultPdfPath)
             self.addDownloadPath(resultXmlPath)
-            self.addDownloadPath(resultFullPdfPath)
             self.addDownloadPath(resultPngPath)
             self.addDownloadPath(resultSvgPath)
             self.addDownloadPath(resultImageTarPath)
             self.addDownloadPath(resultCifPath)
             self.addDownloadPath(resultFoPath)
             self.addDownloadPath(result2FoPath)
             self.addDownloadPath(logPath)
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1489,27 +1489,37 @@
             #
             fList = []
             for pth in pthList:
                 (_dir, fileName) = os.path.split(pth)
                 fList.append(fileName)
             rC.set("specialpositionreportfiles", fList)
 
+            # Validation file downloads
             fpattern = self._sessionPath + "/" + entryId + "_val-report*"
             pthList = []
             pthList = glob.glob(fpattern)
             fpattern = self._sessionPath + "/" + entryId + "_val-data*"
 
             pthList.extend(glob.glob(fpattern))
             #
             fList = []
             for pth in pthList:
                 (_dir, fileName) = os.path.split(pth)
                 fList.append(fileName)
-            rC.set("valreportfiles", fList)
 
+            # Special handling of flist, the desire for full validation pdf to come first...
+            # We need to find first substring list matches, and then rest
+            tlist = []
+            for t in ["val-report-full_P1", "val-report_P1"]:
+                tlist += [v for v in fList if t in v]
+            olist = [v for v in fList if v not in tlist]
+
+            rC.set("valreportfiles", tlist + olist)
+
+            # Map files
             fpattern = self._sessionPath + "/" + entryId + "_map-*"
             pthList = []
             pthList = glob.glob(fpattern)
             #
             fList = []
             mapDisplayFlag = False
             omitMapDisplayFlag = False
@@ -2090,14 +2100,15 @@
         layout = "multiaccordion"
         #
         myD = {}
         for ky in [
             "model",
             "dcc-report",
             "geometry-check-report",
+            "links-report",
             "misc-check-report",
             "format-check-report",
             "dict-check-report",
             "dict-check-report-r4",
             "dict-check-report-next",
             "xml-check-report",
             "special-position-report",
@@ -2171,14 +2182,23 @@
                 if ok:
                     downloadPath = du.getDownloadPath()
                     aTagList.append(du.getAnchorTag())
                     myD[cT] = "\n".join(pR.makeTabularReport(filePath=downloadPath, contentType="geometry-check-report", idCode=entryId, layout=layout))
                 else:
                     # myD[cT] = self.__getMessageTextWithMarkup('No geometry issues.')
                     myD[cT] = self.__getMessageTextWithMarkup("")
+            elif cT == "links-report":
+                # Links report
+                ok = du.fetchId(entryId, contentType="model", formatType="pdbx", fileSource=fileSource, instance=instance, versionId=versionId)
+                if ok:
+                    downloadPath = du.getDownloadPath()
+                    aTagList.append(du.getAnchorTag())
+                    myD[cT] = "\n".join(pR.makeTabularReport(filePath=downloadPath, contentType="links-report", idCode=entryId, layout=layout))
+                else:
+                    myD[cT] = self.__getMessageTextWithMarkup("")
             elif cT == "misc-check-report":
                 # Misc check report
                 ok = du.fetchId(entryId, contentType="misc-check-report", formatType="txt", fileSource=fileSource, instance=instance)
                 if ok:
                     downloadPath = du.getDownloadPath()
                     aTagList.append(du.getAnchorTag())
                     myD[cT] = self.__getFileTextWithMarkup(downloadPath)
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,14 +328,15 @@
             self._lfh.write("\n\n+ReviewDataWebAppWorker._generateFullHtmlCheckReport() idCode %s generating reports from data files in fileSource %s\n" % (idCode, fileSource))
         #
         cTL = [
             "model",
             "dcc-report",
             "special-position-report",
             "geometry-check-report",
+            "links-report",
             "misc-check-report",
             "format-check-report",
             "dict-check-report",
             "xml-check-report",
             # 'model-pdb',
             "emd-xml-header-report",
             "em-map-check-report",
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ann_tasks_v2
-Version: 0.37.3
+Version: 0.37.4
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt` & `wwpdb_apps_ann_tasks_v2-0.37.4/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 wwpdb/apps/ann_tasks_v2/related/Related.py
 wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
 wwpdb/apps/ann_tasks_v2/related/__init__.py
 wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
 wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
 wwpdb/apps/ann_tasks_v2/report/__init__.py
 wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
+wwpdb/apps/ann_tasks_v2/report/styles/LinksReport.py
 wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
 wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
 wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
 wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
 wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
 wwpdb/apps/ann_tasks_v2/site/Site.py
 wwpdb/apps/ann_tasks_v2/site/__init__.py
```

