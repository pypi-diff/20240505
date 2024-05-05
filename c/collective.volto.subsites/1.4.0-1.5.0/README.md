# Comparing `tmp/collective.volto.subsites-1.4.0.tar.gz` & `tmp/collective.volto.subsites-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.volto.subsites-1.4.0.tar", last modified: Sun Oct 10 17:43:58 2021, max compression
+gzip compressed data, was "collective.volto.subsites-1.5.0.tar", last modified: Sun May  5 06:33:30 2024, max compression
```

## Comparing `collective.volto.subsites-1.4.0.tar` & `collective.volto.subsites-1.5.0.tar`

### file list

```diff
@@ -1,93 +1,99 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/
--rw-r--r--   0 cekk       (501) staff       (20)      728 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       73 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      676 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)       95 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     4714 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     1703 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)       27 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/constraints.txt
--rw-r--r--   0 cekk       (501) staff       (20)      105 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/constraints_plone52.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7941 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       98 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)       50 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/requirements.txt
--rw-r--r--   0 cekk       (501) staff       (20)      321 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2524 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/
--rw-r--r--   0 cekk       (501) staff       (20)      142 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      494 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      481 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/browser/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)     1581 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/content/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/content/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2327 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/content/subsite.py
--rw-r--r--   0 cekk       (501) staff       (20)     1131 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3757 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/collective.volto.subsites.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      458 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/en/LC_MESSAGES/collective.volto.subsites.mo
--rw-r--r--   0 cekk       (501) staff       (20)     3626 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/en/LC_MESSAGES/collective.volto.subsites.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     2364 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/it/LC_MESSAGES/collective.volto.subsites.mo
--rw-r--r--   0 cekk       (501) staff       (20)     4651 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/it/LC_MESSAGES/collective.volto.subsites.po
--rw-r--r--   0 cekk       (501) staff       (20)     1597 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      512 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      347 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      200 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      572 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      182 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)      232 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      302 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/types/
--rw-r--r--   0 cekk       (501) staff       (20)     2881 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/types/Subsite.xml
--rw-r--r--   0 cekk       (501) staff       (20)      160 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/types.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      135 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      246 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/uninstall/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      220 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/services/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      268 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/services/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      462 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/services/controlpanel.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/services/subsite/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/services/subsite/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      504 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/services/subsite/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     2096 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/services/subsite/get.py
--rw-r--r--   0 cekk       (501) staff       (20)     1085 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1237 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1185 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/tests/image.png
--rw-r--r--   0 cekk       (501) staff       (20)     5947 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/tests/test_api_expansion.py
--rw-r--r--   0 cekk       (501) staff       (20)     1428 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/tests/test_controlpanel_api.py
--rw-r--r--   0 cekk       (501) staff       (20)     2953 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)      770 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/upgrades.py
--rw-r--r--   0 cekk       (501) staff       (20)      398 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/upgrades.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      978 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective/volto/subsites/vocabularies.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective.volto.subsites.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     4714 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective.volto.subsites.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3295 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective.volto.subsites.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective.volto.subsites.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      150 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective.volto.subsites.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       28 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective.volto.subsites.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective.volto.subsites.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      188 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective.volto.subsites.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2021-10-10 17:43:58.000000 collective.volto.subsites-1.4.0/src/collective.volto.subsites.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.368543 collective.volto.subsites-1.5.0/
+-rw-r--r--   0 cekk       (501) staff       (20)      927 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      130 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      676 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       95 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     3819 2024-05-05 06:33:30.368610 collective.volto.subsites-1.5.0/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     1715 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       27 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/constraints.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/constraints_plone52.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.361784 collective.volto.subsites-1.5.0/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7941 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       98 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       50 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      321 2024-05-05 06:33:30.369300 collective.volto.subsites-1.5.0/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2562 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.358668 collective.volto.subsites-1.5.0/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.361897 collective.volto.subsites-1.5.0/src/collective/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.362944 collective.volto.subsites-1.5.0/src/collective/volto/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.363960 collective.volto.subsites-1.5.0/src/collective/volto/subsites/
+-rw-r--r--   0 cekk       (501) staff       (20)      142 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.364284 collective.volto.subsites-1.5.0/src/collective/volto/subsites/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      494 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      481 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/browser/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1581 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.364493 collective.volto.subsites-1.5.0/src/collective/volto/subsites/content/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/content/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2327 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/content/subsite.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1131 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.365031 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3757 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/collective.volto.subsites.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.359165 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.365264 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/en/LC_MESSAGES/collective.volto.subsites.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     3626 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/en/LC_MESSAGES/collective.volto.subsites.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.359282 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/es/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.365506 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/es/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     2710 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/es/LC_MESSAGES/collective.volto.subsites.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     5131 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/es/LC_MESSAGES/collective.volto.subsites.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.359406 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.365741 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     2364 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/it/LC_MESSAGES/collective.volto.subsites.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     4651 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/it/LC_MESSAGES/collective.volto.subsites.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1597 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      512 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      347 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.359682 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.366760 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      200 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      572 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      237 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/diff_tool.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      182 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      232 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      241 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/repositorytool.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      302 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.366877 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/types/
+-rw-r--r--   0 cekk       (501) staff       (20)     2921 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/types/Subsite.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      160 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/types.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.367098 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      135 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      246 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/uninstall/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.367290 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      220 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.367597 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/services/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      268 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/services/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      462 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/services/controlpanel.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.367904 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/services/subsite/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/services/subsite/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      504 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/services/subsite/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     2096 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/services/subsite/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1085 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1237 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.368427 collective.volto.subsites-1.5.0/src/collective/volto/subsites/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1185 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/tests/image.png
+-rw-r--r--   0 cekk       (501) staff       (20)     5947 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/tests/test_api_expansion.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1428 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/tests/test_controlpanel_api.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2953 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1274 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)      656 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/upgrades.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      978 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective/volto/subsites/vocabularies.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:33:30.362827 collective.volto.subsites-1.5.0/src/collective.volto.subsites.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     3819 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective.volto.subsites.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3586 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective.volto.subsites.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective.volto.subsites.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      130 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective.volto.subsites.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       28 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective.volto.subsites.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective.volto.subsites.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      215 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective.volto.subsites.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       11 2024-05-05 06:33:30.000000 collective.volto.subsites-1.5.0/src/collective.volto.subsites.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.volto.subsites-1.4.0/DEVELOP.rst` & `collective.volto.subsites-1.5.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/LICENSE.GPL` & `collective.volto.subsites-1.5.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/LICENSE.rst` & `collective.volto.subsites-1.5.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/README.rst` & `collective.volto.subsites-1.5.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 Translations
 ------------
 
 This product has been translated into
 
 - Italian
 
+- Spanish
+
 
 Installation
 ------------
 
 Install collective.volto.subsites by adding it to your buildout::
 
     [buildout]
@@ -75,8 +77,8 @@
 Authors
 =======
 
 This product was developed by **RedTurtle Technology** team.
 
 .. image:: https://avatars1.githubusercontent.com/u/1087171?s=100&v=4
    :alt: RedTurtle Technology Site
-   :target: http://www.redturtle.it/
+   :target: https://www.redturtle.it/
```

### Comparing `collective.volto.subsites-1.4.0/docs/conf.py` & `collective.volto.subsites-1.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/setup.py` & `collective.volto.subsites-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="collective.volto.subsites",
-    version="1.4.0",
+    version="1.5.0",
     description="Add Subsite content-type for Volto",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
@@ -50,14 +50,15 @@
     python_requires=">=3.6",
     install_requires=[
         "setuptools",
         # -*- Extra requirements: -*-
         "plone.api>=1.8.4",
         "plone.restapi",
         "plone.app.dexterity",
+        "plone.app.caching>=3.0.0a1",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
```

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/configure.zcml` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/content/subsite.py` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/content/subsite.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/interfaces.py` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/README.rst` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/collective.volto.subsites.pot` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/collective.volto.subsites.pot`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/en/LC_MESSAGES/collective.volto.subsites.po` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/en/LC_MESSAGES/collective.volto.subsites.po`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/it/LC_MESSAGES/collective.volto.subsites.mo` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/it/LC_MESSAGES/collective.volto.subsites.mo`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/it/LC_MESSAGES/collective.volto.subsites.po` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/it/LC_MESSAGES/collective.volto.subsites.po`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/update.py` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/locales/update.sh` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/locales/update.sh`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/controlpanel.xml` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/types/Subsite.xml` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/types/Subsite.xml`

 * *Files 1% similar despite different names*

#### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/profiles/default/types/Subsite.xml` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/profiles/default/types/Subsite.xml`

```diff
@@ -27,14 +27,15 @@
     <element value="plone.constraintypes"/>
     <element value="plone.relateditems"/>
     <element value="plone.nextprevioustoggle"/>
     <element value="plone.leadimage"/>
     <element value="volto.blocks"/>
     <element value="plone.translatable"/>
     <element value="kitconcept.seo"/>
+    <element value="plone.versioning"/>
   </property>
   <!-- View information -->
   <property name="add_view_expr">string:${folder_url}/++add++Subsite</property>
   <property name="default_view">view</property>
   <property name="default_view_fallback">False</property>
   <property name="immediate_view">view</property>
   <property name="view_methods">
```

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/restapi/services/subsite/get.py` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/restapi/services/subsite/get.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/setuphandlers.py` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/testing.py` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/testing.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/tests/image.png` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/tests/image.png`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/tests/test_api_expansion.py` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/tests/test_api_expansion.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/tests/test_controlpanel_api.py` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/tests/test_controlpanel_api.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/tests/test_setup.py` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective/volto/subsites/vocabularies.py` & `collective.volto.subsites-1.5.0/src/collective/volto/subsites/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.volto.subsites-1.4.0/src/collective.volto.subsites.egg-info/SOURCES.txt` & `collective.volto.subsites-1.5.0/src/collective.volto.subsites.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -39,21 +39,25 @@
 src/collective/volto/subsites/locales/README.rst
 src/collective/volto/subsites/locales/__init__.py
 src/collective/volto/subsites/locales/collective.volto.subsites.pot
 src/collective/volto/subsites/locales/update.py
 src/collective/volto/subsites/locales/update.sh
 src/collective/volto/subsites/locales/en/LC_MESSAGES/collective.volto.subsites.mo
 src/collective/volto/subsites/locales/en/LC_MESSAGES/collective.volto.subsites.po
+src/collective/volto/subsites/locales/es/LC_MESSAGES/collective.volto.subsites.mo
+src/collective/volto/subsites/locales/es/LC_MESSAGES/collective.volto.subsites.po
 src/collective/volto/subsites/locales/it/LC_MESSAGES/collective.volto.subsites.mo
 src/collective/volto/subsites/locales/it/LC_MESSAGES/collective.volto.subsites.po
 src/collective/volto/subsites/profiles/default/browserlayer.xml
 src/collective/volto/subsites/profiles/default/catalog.xml
 src/collective/volto/subsites/profiles/default/controlpanel.xml
+src/collective/volto/subsites/profiles/default/diff_tool.xml
 src/collective/volto/subsites/profiles/default/metadata.xml
 src/collective/volto/subsites/profiles/default/registry.xml
+src/collective/volto/subsites/profiles/default/repositorytool.xml
 src/collective/volto/subsites/profiles/default/rolemap.xml
 src/collective/volto/subsites/profiles/default/types.xml
 src/collective/volto/subsites/profiles/default/types/Subsite.xml
 src/collective/volto/subsites/profiles/uninstall/browserlayer.xml
 src/collective/volto/subsites/profiles/uninstall/registry.xml
 src/collective/volto/subsites/restapi/__init__.py
 src/collective/volto/subsites/restapi/configure.zcml
```

