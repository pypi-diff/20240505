# Comparing `tmp/emlvp-1.2.0.tar.gz` & `tmp/emlvp-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emlvp-1.2.0.tar", last modified: Tue Apr 23 03:21:05 2024, max compression
+gzip compressed data, was "emlvp-1.2.1.tar", last modified: Sun May  5 02:48:54 2024, max compression
```

## Comparing `emlvp-1.2.0.tar` & `emlvp-1.2.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-23 03:21:05.034468 emlvp-1.2.0/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    11357 2023-01-21 18:45:39.000000 emlvp-1.2.0/LICENSE
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      130 2023-02-01 23:07:16.000000 emlvp-1.2.0/MANIFEST.in
--rw-r--r--   0 servilla  (1000) servilla  (1000)    22084 2024-04-23 03:21:05.034468 emlvp-1.2.0/PKG-INFO
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8716 2024-04-23 02:54:39.000000 emlvp-1.2.0/README.md
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      766 2024-04-23 03:21:05.034468 emlvp-1.2.0/setup.cfg
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1252 2024-01-19 03:13:11.000000 emlvp-1.2.0/setup.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-23 03:21:05.022467 emlvp-1.2.0/src/
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-23 03:21:05.022467 emlvp-1.2.0/src/emlvp/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2024-04-23 03:02:43.000000 emlvp-1.2.0/src/emlvp/VERSION.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      128 2023-01-21 19:41:00.000000 emlvp-1.2.0/src/emlvp/__init__.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1145 2024-04-23 03:02:43.000000 emlvp-1.2.0/src/emlvp/changelog.md
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1814 2024-04-11 21:30:42.000000 emlvp-1.2.0/src/emlvp/dereferencer.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     9535 2024-04-23 02:54:39.000000 emlvp-1.2.0/src/emlvp/emlvp_cli.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1247 2024-04-23 02:54:39.000000 emlvp-1.2.0/src/emlvp/exceptions.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2343 2024-04-11 21:30:42.000000 emlvp-1.2.0/src/emlvp/normalizer.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8289 2024-04-11 21:30:42.000000 emlvp-1.2.0/src/emlvp/parser.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-23 03:21:05.022467 emlvp-1.2.0/src/emlvp/schemas/
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-23 03:21:05.026467 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    18447 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-access.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-entity.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-literature.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-methods.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    29487 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-party.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-physical.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-project.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    58886 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-resource.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-software.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    18745 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-text.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-view.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    19139 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:00.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/stmml.xsd
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-23 03:21:05.030467 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    20356 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-access.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-entity.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-literature.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-methods.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    29531 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-party.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-physical.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-project.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    60720 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-resource.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-software.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21204 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-text.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-view.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    19379 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:17.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/stmml.xsd
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-23 03:21:05.030467 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493311 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   102174 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-23 03:21:05.030467 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    11830 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    86976 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    27152 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    72264 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7693 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    28001 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2899 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    14949 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    58814 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21970 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    28924 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    76821 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    29309 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     4952 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    68327 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    15511 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    21403 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    46367 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   167250 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    13021 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    10334 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    32155 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd
--rwxrwxr-x   0 servilla  (1000) servilla  (1000)    23090 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7008 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    22368 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)   133761 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      579 2023-01-31 04:06:28.000000 emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      800 2024-04-11 21:27:52.000000 emlvp-1.2.0/src/emlvp/unicode_inspector.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2201 2024-04-23 03:17:57.000000 emlvp-1.2.0/src/emlvp/validator.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-23 03:21:05.030467 emlvp-1.2.0/src/emlvp.egg-info/
--rw-r--r--   0 servilla  (1000) servilla  (1000)    22084 2024-04-23 03:21:05.000000 emlvp-1.2.0/src/emlvp.egg-info/PKG-INFO
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     4468 2024-04-23 03:21:05.000000 emlvp-1.2.0/src/emlvp.egg-info/SOURCES.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        1 2024-04-23 03:21:05.000000 emlvp-1.2.0/src/emlvp.egg-info/dependency_links.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)       47 2024-04-23 03:21:05.000000 emlvp-1.2.0/src/emlvp.egg-info/entry_points.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)       41 2024-04-23 03:21:05.000000 emlvp-1.2.0/src/emlvp.egg-info/requires.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2024-04-23 03:21:05.000000 emlvp-1.2.0/src/emlvp.egg-info/top_level.txt
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-04-23 03:21:05.030467 emlvp-1.2.0/tests/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      647 2024-02-17 17:40:25.000000 emlvp-1.2.0/tests/test_dereferencer.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      584 2024-02-17 17:40:25.000000 emlvp-1.2.0/tests/test_normalizer.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2896 2023-07-22 01:19:36.000000 emlvp-1.2.0/tests/test_parser.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      610 2024-04-11 19:56:52.000000 emlvp-1.2.0/tests/test_unicode.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2064 2024-04-23 02:44:52.000000 emlvp-1.2.0/tests/test_validator.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-05-05 02:48:54.931712 emlvp-1.2.1/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    11357 2023-01-21 18:45:39.000000 emlvp-1.2.1/LICENSE
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      130 2023-02-01 23:07:16.000000 emlvp-1.2.1/MANIFEST.in
+-rw-r--r--   0 servilla  (1000) servilla  (1000)    22084 2024-05-05 02:48:54.931712 emlvp-1.2.1/PKG-INFO
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8716 2024-04-23 02:54:39.000000 emlvp-1.2.1/README.md
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      766 2024-05-05 02:48:54.931712 emlvp-1.2.1/setup.cfg
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1252 2024-01-19 03:13:11.000000 emlvp-1.2.1/setup.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-05-05 02:48:54.839711 emlvp-1.2.1/src/
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-05-05 02:48:54.843711 emlvp-1.2.1/src/emlvp/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2024-05-05 00:07:27.000000 emlvp-1.2.1/src/emlvp/VERSION.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      128 2023-01-21 19:41:00.000000 emlvp-1.2.1/src/emlvp/__init__.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1248 2024-05-05 00:07:27.000000 emlvp-1.2.1/src/emlvp/changelog.md
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1814 2024-04-11 21:30:42.000000 emlvp-1.2.1/src/emlvp/dereferencer.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     9535 2024-04-23 02:54:39.000000 emlvp-1.2.1/src/emlvp/emlvp_cli.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1247 2024-04-23 02:54:39.000000 emlvp-1.2.1/src/emlvp/exceptions.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2343 2024-04-11 21:30:42.000000 emlvp-1.2.1/src/emlvp/normalizer.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8289 2024-04-11 21:30:42.000000 emlvp-1.2.1/src/emlvp/parser.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-05-05 02:48:54.839711 emlvp-1.2.1/src/emlvp/schemas/
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-05-05 02:48:54.891711 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    18447 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-access.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-entity.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-literature.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-methods.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    29487 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-party.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-physical.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-project.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    58886 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-resource.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-software.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    18745 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-text.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-view.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    19139 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:00.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/stmml.xsd
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-05-05 02:48:54.923712 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    20356 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-access.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    91400 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    27850 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    73805 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     8750 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21841 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2873 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    14750 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-entity.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    57086 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-literature.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22970 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-methods.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    29531 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-party.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    78239 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-physical.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    23380 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-project.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     5596 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    60720 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-resource.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22084 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-software.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    46813 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   167808 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493395 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    13428 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    10813 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21204 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-text.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    48711 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    18025 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7197 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-view.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    19379 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   134968 2023-01-31 04:06:17.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/stmml.xsd
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-05-05 02:48:54.927712 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)  1493311 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   102174 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-05-05 02:48:54.927712 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    11830 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    86976 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    27152 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    72264 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7693 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    28001 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2899 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    14949 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    58814 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21970 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    28924 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    76821 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    29309 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     4952 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    68327 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    15511 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    21403 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    46367 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   167250 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    13021 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    10334 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    32155 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd
+-rwxrwxr-x   0 servilla  (1000) servilla  (1000)    23090 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7008 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    22368 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)   133761 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      579 2023-01-31 04:06:28.000000 emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      811 2024-05-04 23:59:19.000000 emlvp-1.2.1/src/emlvp/unicode_inspector.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2201 2024-04-23 03:17:57.000000 emlvp-1.2.1/src/emlvp/validator.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-05-05 02:48:54.927712 emlvp-1.2.1/src/emlvp.egg-info/
+-rw-r--r--   0 servilla  (1000) servilla  (1000)    22084 2024-05-05 02:48:54.000000 emlvp-1.2.1/src/emlvp.egg-info/PKG-INFO
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     4468 2024-05-05 02:48:54.000000 emlvp-1.2.1/src/emlvp.egg-info/SOURCES.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        1 2024-05-05 02:48:54.000000 emlvp-1.2.1/src/emlvp.egg-info/dependency_links.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)       47 2024-05-05 02:48:54.000000 emlvp-1.2.1/src/emlvp.egg-info/entry_points.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)       41 2024-05-05 02:48:54.000000 emlvp-1.2.1/src/emlvp.egg-info/requires.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2024-05-05 02:48:54.000000 emlvp-1.2.1/src/emlvp.egg-info/top_level.txt
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2024-05-05 02:48:54.927712 emlvp-1.2.1/tests/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      647 2024-02-17 17:40:25.000000 emlvp-1.2.1/tests/test_dereferencer.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      584 2024-02-17 17:40:25.000000 emlvp-1.2.1/tests/test_normalizer.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2896 2023-07-22 01:19:36.000000 emlvp-1.2.1/tests/test_parser.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      610 2024-04-11 19:56:52.000000 emlvp-1.2.1/tests/test_unicode.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     2064 2024-04-23 02:44:52.000000 emlvp-1.2.1/tests/test_validator.py
```

### Comparing `emlvp-1.2.0/LICENSE` & `emlvp-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/PKG-INFO` & `emlvp-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlvp
-Version: 1.2.0
+Version: 1.2.1
 Summary: EMLvp (validator and parser)
 Home-page: https://github.com/servilla/EMLvp
 Author: Mark Servilla
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `emlvp-1.2.0/README.md` & `emlvp-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/setup.cfg` & `emlvp-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/setup.py` & `emlvp-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/changelog.md` & `emlvp-1.2.1/src/emlvp/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # EMLvp change log
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## (1.2.1) 2024-05-5
+### Changed/Fixed
+- Set default value as "Unknown" for unicodedata.name function
+
 ## (1.2.0) 2024-04-22
 ### Changed/Fixed
 - Update for validation exception list instead of single first error
 
 ## (1.1.0) 2024-02-17
 ### Changed/Fixed
 - Catch ValueError in `process_one_document`
```

### Comparing `emlvp-1.2.0/src/emlvp/dereferencer.py` & `emlvp-1.2.1/src/emlvp/dereferencer.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/emlvp_cli.py` & `emlvp-1.2.1/src/emlvp/emlvp_cli.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/exceptions.py` & `emlvp-1.2.1/src/emlvp/exceptions.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/normalizer.py` & `emlvp-1.2.1/src/emlvp/normalizer.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/parser.py` & `emlvp-1.2.1/src/emlvp/parser.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-access.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-access.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-attribute.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-constraint.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-coverage.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-dataTable.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-dataset.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-documentation.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-entity.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-entity.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-literature.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-literature.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-methods.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-methods.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-party.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-party.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-physical.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-physical.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-project.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-project.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-protocol.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-resource.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-resource.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-software.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-software.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-spatialRaster.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-spatialReference.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-spatialReferenceDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-spatialVector.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-storedProcedure.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-text.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-text.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-unitDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-unitTypeDefinitions.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml-view.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml-view.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/eml.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/eml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.0/stmml.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.0/stmml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-access.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-access.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-attribute.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-constraint.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-coverage.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-dataTable.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-dataset.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-documentation.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-entity.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-entity.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-literature.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-literature.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-methods.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-methods.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-party.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-party.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-physical.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-physical.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-project.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-project.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-protocol.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-resource.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-resource.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-software.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-software.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-spatialRaster.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-spatialReference.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-spatialReferenceDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-spatialVector.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-storedProcedure.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-text.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-text.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-unitDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-unitTypeDefinitions.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml-view.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml-view.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/eml.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/eml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.1.1/stmml.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.1.1/stmml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/eml-spatialReferenceDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/eml-unitDictionary.xml`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-access.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-attribute.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-constraint.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-coverage.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-dataTable.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-dataset.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-documentation.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-entity.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-literature.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-methods.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-party.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-physical.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-project.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-protocol.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-resource.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-semantics.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-software.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialRaster.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialReference.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-spatialVector.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-storedProcedure.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-text.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-unitTypeDefinitions.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml-view.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/eml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/stmml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd` & `emlvp-1.2.1/src/emlvp/schemas/EML2.2.0/xsd/xml.xsd`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp/unicode_inspector.py` & `emlvp-1.2.1/src/emlvp/unicode_inspector.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,11 +31,11 @@
         for c in range(len(line)):
             i = line[c]
             if ord(i) >= 127:
                 row = n
                 col = c + 1
                 char = i
                 cp = ord(i)
-                name = unicodedata.name(i)
+                name = unicodedata.name(i, "Unknown")
                 unicodes.append((row, col, char, cp, name))
 
     return unicodes
```

### Comparing `emlvp-1.2.0/src/emlvp/validator.py` & `emlvp-1.2.1/src/emlvp/validator.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/src/emlvp.egg-info/PKG-INFO` & `emlvp-1.2.1/src/emlvp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emlvp
-Version: 1.2.0
+Version: 1.2.1
 Summary: EMLvp (validator and parser)
 Home-page: https://github.com/servilla/EMLvp
 Author: Mark Servilla
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `emlvp-1.2.0/src/emlvp.egg-info/SOURCES.txt` & `emlvp-1.2.1/src/emlvp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/tests/test_dereferencer.py` & `emlvp-1.2.1/tests/test_dereferencer.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/tests/test_normalizer.py` & `emlvp-1.2.1/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/tests/test_parser.py` & `emlvp-1.2.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/tests/test_unicode.py` & `emlvp-1.2.1/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `emlvp-1.2.0/tests/test_validator.py` & `emlvp-1.2.1/tests/test_validator.py`

 * *Files identical despite different names*

