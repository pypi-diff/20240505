# Comparing `tmp/djangocms-versioning-2.0.1.tar.gz` & `tmp/djangocms_versioning-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-versioning-2.0.1.tar", last modified: Fri Mar 29 13:34:36 2024, max compression
+gzip compressed data, was "djangocms_versioning-2.0.2.tar", last modified: Sun May  5 08:42:53 2024, max compression
```

## Comparing `djangocms-versioning-2.0.1.tar` & `djangocms_versioning-2.0.2.tar`

### file list

```diff
@@ -1,243 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.054170 djangocms-versioning-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-03-29 13:34:36.054170 djangocms-versioning-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.022170 djangocms-versioning-2.0.1/djangocms_versioning/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54028 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    17460 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/cms_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/cms_menus.py
--rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/cms_toolbars.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14869 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.014170 djangocms-versioning-2.0.1/djangocms_versioning/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.010170 djangocms-versioning-2.0.1/djangocms_versioning/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.022170 djangocms-versioning-2.0.1/djangocms_versioning/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13558 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.010170 djangocms-versioning-2.0.1/djangocms_versioning/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.022170 djangocms-versioning-2.0.1/djangocms_versioning/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.010170 djangocms-versioning-2.0.1/djangocms_versioning/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.022170 djangocms-versioning-2.0.1/djangocms_versioning/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13621 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.014170 djangocms-versioning-2.0.1/djangocms_versioning/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.022170 djangocms-versioning-2.0.1/djangocms_versioning/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.014170 djangocms-versioning-2.0.1/djangocms_versioning/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.026170 djangocms-versioning-2.0.1/djangocms_versioning/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13381 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.026170 djangocms-versioning-2.0.1/djangocms_versioning/management/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.026170 djangocms-versioning-2.0.1/djangocms_versioning/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/management/commands/create_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.026170 djangocms-versioning-2.0.1/djangocms_versioning/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0002_delete_campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0003_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0004_auto_20180730_1135.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0005_remove_version_label.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0006_auto_20180809_1714.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0007_auto_20180813_1407.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0008_auto_20180820_1754.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0009_cms_pagecontent_remove_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0010_version_proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0011_version_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0012_create_version_numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0013_auto_20181005_1404.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0014_version_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0015_version_modified.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0016_alter_version_content_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0016_auto_20230505_0934.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/0017_merge_20230514_1027.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/plugin_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.014170 djangocms-versioning-2.0.1/djangocms_versioning/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.014170 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.030170 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/css/source.css
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/css/versioning.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.030170 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/actions.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.030170 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/admin/versioning-actions.js
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/base.js
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/compare.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.030170 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/dist/
--rw-r--r--   0 runner    (1001) docker     (127)   944110 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/dist/bundle.prettydiff.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   132188 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/dist/bundle.versioning.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/get-dist-path.js
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/indicators.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.034170 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.034170 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/api/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4641 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/api/dom.js
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/difflib.js
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/diffview.js
--rw-r--r--   0 runner    (1001) docker     (127)    41131 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/htmldiff.js
--rw-r--r--   0 runner    (1001) docker     (127)  1178666 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/tidy.js
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/loader.js
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/prettydiff.js
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/versioning.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.034170 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/archive.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/discard.svg
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/edit.svg
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/lock.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/manage_versions.svg
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/menu.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/preview.svg
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/publish.svg
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/redo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/undo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/unpublish.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.014170 djangocms-versioning-2.0.1/djangocms_versioning/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.014170 djangocms-versioning-2.0.1/djangocms_versioning/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.038170 djangocms-versioning-2.0.1/djangocms_versioning/templates/admin/djangocms_versioning/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/admin/djangocms_versioning/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/admin/djangocms_versioning/indicator.html
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/admin/djangocms_versioning/versioning_breadcrumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.014170 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.038170 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/archive_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/compare.html
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/discard_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/grouper_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.038170 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/archive_icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/discard_icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/edit_icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/manage_versions.html
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/preview.html
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/publish_icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/revert_icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/unpublish_icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/view.html
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/lock_indicator.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.038170 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/mixin/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/preview.html
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/revert_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/unpublish_confirmation.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.038170 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/emails/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/emails/unlock-notification.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.038170 djangocms-versioning-2.0.1/djangocms_versioning/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/templatetags/djangocms_versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.042170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.042170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/blogpost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/blogpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/blogpost/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/blogpost/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/blogpost/cms_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/blogpost/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.042170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extended_polls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extended_polls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extended_polls/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.042170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extended_polls/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extended_polls/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extended_polls/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extended_polls/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.042170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.042170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extensions/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extensions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extensions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extensions/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.042170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/incorrectly_configured_blogpost/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/incorrectly_configured_blogpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/incorrectly_configured_blogpost/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/incorrectly_configured_blogpost/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/incorrectly_configured_blogpost/cms_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/incorrectly_configured_blogpost/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.042170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/people/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/people/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/people/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.046170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/cms_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/cms_wizards.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.046170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.046170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/templatetags/polls_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.046170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/text/cms_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.046170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/text/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/text/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/text/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/text/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.046170 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/unversioned_editable_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/unversioned_editable_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/unversioned_editable_app/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/unversioned_editable_app/cms_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/unversioned_editable_app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/unversioned_editable_app/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/test_utils/unversioned_editable_app/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/djangocms_versioning/versionables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.054170 djangocms-versioning-2.0.1/djangocms_versioning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-03-29 13:34:35.000000 djangocms-versioning-2.0.1/djangocms_versioning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-03-29 13:34:36.000000 djangocms-versioning-2.0.1/djangocms_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:34:35.000000 djangocms-versioning-2.0.1/djangocms_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-29 13:34:35.000000 djangocms-versioning-2.0.1/djangocms_versioning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-29 13:34:35.000000 djangocms-versioning-2.0.1/djangocms_versioning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-29 13:34:36.054170 djangocms-versioning-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:36.050170 djangocms-versioning-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_0_migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)   136435 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_automatic_version_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    20185 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_cms_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_content_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)     7864 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_indicators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_integration_with_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    37241 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_locking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_management_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    13984 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_menus.py
--rw-r--r--   0 runner    (1001) docker     (127)    19042 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_states.py
--rw-r--r--   0 runner    (1001) docker     (127)    25359 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_toolbars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_version_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-03-29 13:34:30.000000 djangocms-versioning-2.0.1/tests/test_versionables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.854955 djangocms_versioning-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-05 08:42:53.854955 djangocms_versioning-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.818955 djangocms_versioning-2.0.2/djangocms_versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54060 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17460 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/cms_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/cms_menus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/cms_toolbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14869 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.806955 djangocms_versioning-2.0.2/djangocms_versioning/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.806955 djangocms_versioning-2.0.2/djangocms_versioning/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.818955 djangocms_versioning-2.0.2/djangocms_versioning/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.806955 djangocms_versioning-2.0.2/djangocms_versioning/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.818955 djangocms_versioning-2.0.2/djangocms_versioning/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13554 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.806955 djangocms_versioning-2.0.2/djangocms_versioning/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.818955 djangocms_versioning-2.0.2/djangocms_versioning/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.806955 djangocms_versioning-2.0.2/djangocms_versioning/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.822955 djangocms_versioning-2.0.2/djangocms_versioning/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13614 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.806955 djangocms_versioning-2.0.2/djangocms_versioning/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.822955 djangocms_versioning-2.0.2/djangocms_versioning/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.806955 djangocms_versioning-2.0.2/djangocms_versioning/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.822955 djangocms_versioning-2.0.2/djangocms_versioning/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.822955 djangocms_versioning-2.0.2/djangocms_versioning/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.822955 djangocms_versioning-2.0.2/djangocms_versioning/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/management/commands/create_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.826955 djangocms_versioning-2.0.2/djangocms_versioning/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0002_delete_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0003_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0004_auto_20180730_1135.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0005_remove_version_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0006_auto_20180809_1714.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0007_auto_20180813_1407.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0008_auto_20180820_1754.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0009_cms_pagecontent_remove_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0010_version_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0011_version_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0012_create_version_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0013_auto_20181005_1404.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0014_version_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0015_version_modified.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0016_alter_version_content_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0016_auto_20230505_0934.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/0017_merge_20230514_1027.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/plugin_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.810955 djangocms_versioning-2.0.2/djangocms_versioning/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.810955 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.826955 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/css/source.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/css/versioning.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.826955 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/actions.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.826955 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/admin/versioning-actions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/base.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/compare.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.830955 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)   944110 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/dist/bundle.prettydiff.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   132188 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/dist/bundle.versioning.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/get-dist-path.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/indicators.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.830955 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.834955 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/api/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4641 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/api/dom.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/difflib.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/diffview.js
+-rw-r--r--   0 runner    (1001) docker     (127)    41131 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/htmldiff.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1178666 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/tidy.js
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/loader.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/prettydiff.js
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/utils.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/versioning.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.834955 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/archive.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/discard.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/manage_versions.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/menu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/preview.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/publish.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/unpublish.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.810955 djangocms_versioning-2.0.2/djangocms_versioning/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.810955 djangocms_versioning-2.0.2/djangocms_versioning/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.834955 djangocms_versioning-2.0.2/djangocms_versioning/templates/admin/djangocms_versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/admin/djangocms_versioning/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/admin/djangocms_versioning/indicator.html
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/admin/djangocms_versioning/versioning_breadcrumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.810955 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.838955 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/archive_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/compare.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/discard_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/grouper_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.838955 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/archive_icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/discard_icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/edit_icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/manage_versions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/preview.html
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/publish_icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/revert_icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/unpublish_icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/view.html
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/lock_indicator.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.838955 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/mixin/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/preview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/revert_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/unpublish_confirmation.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.838955 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/emails/unlock-notification.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.838955 djangocms_versioning-2.0.2/djangocms_versioning/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/templatetags/djangocms_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.842955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.842955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/blogpost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/blogpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/blogpost/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/blogpost/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/blogpost/cms_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/blogpost/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.842955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extended_polls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extended_polls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extended_polls/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.842955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extended_polls/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extended_polls/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extended_polls/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extended_polls/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.842955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.842955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extensions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extensions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extensions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extensions/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.842955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/incorrectly_configured_blogpost/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/incorrectly_configured_blogpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/incorrectly_configured_blogpost/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/incorrectly_configured_blogpost/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/incorrectly_configured_blogpost/cms_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/incorrectly_configured_blogpost/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.842955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/people/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/people/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/people/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.846955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/cms_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/cms_wizards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.846955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.846955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/templatetags/polls_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.846955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/text/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.846955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/text/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/text/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/text/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/text/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.850955 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/unversioned_editable_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/unversioned_editable_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/unversioned_editable_app/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/unversioned_editable_app/cms_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/unversioned_editable_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/unversioned_editable_app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/test_utils/unversioned_editable_app/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/djangocms_versioning/versionables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.854955 djangocms_versioning-2.0.2/djangocms_versioning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-05 08:42:53.000000 djangocms_versioning-2.0.2/djangocms_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-05 08:42:53.000000 djangocms_versioning-2.0.2/djangocms_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:42:53.000000 djangocms_versioning-2.0.2/djangocms_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 08:42:53.000000 djangocms_versioning-2.0.2/djangocms_versioning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 08:42:53.000000 djangocms_versioning-2.0.2/djangocms_versioning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-05 08:42:53.854955 djangocms_versioning-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:53.854955 djangocms_versioning-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_0_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136429 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_automatic_version_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20185 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_cms_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_integration_with_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37223 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_locking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_management_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13984 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_menus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19042 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25811 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_toolbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_version_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-05 08:42:50.000000 djangocms_versioning-2.0.2/tests/test_versionables.py
```

### Comparing `djangocms-versioning-2.0.1/LICENSE.txt` & `djangocms_versioning-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/PKG-INFO` & `djangocms_versioning-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: djangocms-versioning
-Version: 2.0.1
+Version: 2.0.2
 Home-page: http://github.com/django-cms/djangocms-versioning
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 License-File: LICENSE.txt
-Requires-Dist: Django>=1.11
-Requires-Dist: django-cms
-Requires-Dist: django-fsm
+Requires-Dist: Django>=3.2
+Requires-Dist: django-cms>=4.1.1
+Requires-Dist: django-fsm<3
 
 |django| |djangocms4|
 
 *********************
 django CMS Versioning
 *********************
```

### Comparing `djangocms-versioning-2.0.1/README.rst` & `djangocms_versioning-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/admin.py` & `djangocms_versioning-2.0.2/djangocms_versioning/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,15 +487,15 @@
     def get_actions_list(self):
         """
         Collect rendered actions from implemented methods and return as list
         """
         actions = [
             self._get_preview_link,
             self._get_edit_link,
-         ]
+        ]
         if "state_indicator" not in self.versioning_list_display:
             # State indicator mixin loaded?
             actions.append(self._get_manage_versions_link)
         return actions
 
     def get_list_display(self, request):
         # get configured list_display
@@ -725,14 +725,18 @@
             name="unpublish",
             disabled=not obj.check_unpublish.as_bool(request.user),
         )
 
     def _get_edit_link(self, obj, request, disabled=False):
         """Helper function to get the html link to the edit action
         """
+
+        if not obj.check_edit_redirect.as_bool(request.user):
+            return ""
+
         # Only show if no draft exists
         if obj.state == PUBLISHED:
             pks_for_grouper = obj.versionable.for_content_grouping_values(
                 obj.content
             ).values_list("pk", flat=True)
             drafts = Version.objects.filter(
                 object_id__in=pks_for_grouper,
@@ -754,15 +758,15 @@
         )
         return self.admin_action_button(
             edit_url,
             icon=icon,
             title=_("Edit") if icon == "pencil" else _("New Draft"),
             name="edit",
             action="post",
-            disabled=not obj.check_edit_redirect.as_bool(request.user) or disabled,
+            disabled=disabled,
             keepsideframe=keepsideframe,
         )
 
     def _get_revert_link(self, obj, request, disabled=False):
         """Helper function to get the html link to the revert action
         """
         if obj.state in (PUBLISHED, DRAFT):
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/apps.py` & `djangocms_versioning-2.0.2/djangocms_versioning/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/cms_config.py` & `djangocms_versioning-2.0.2/djangocms_versioning/cms_config.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/cms_menus.py` & `djangocms_versioning-2.0.2/djangocms_versioning/cms_menus.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/cms_toolbars.py` & `djangocms_versioning-2.0.2/djangocms_versioning/cms_toolbars.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,17 +31,14 @@
 )
 from djangocms_versioning.models import Version
 
 VERSIONING_MENU_IDENTIFIER = "version"
 
 
 class VersioningToolbar(PlaceholderToolbar):
-    class Media:
-        js = ("cms/js/admin/actions.js",)
-
     def _get_versionable(self):
         """Helper method to get the versionable for the content type
         of the version
         """
         versioning_extension = apps.get_app_config("djangocms_versioning").cms_extension
         return versioning_extension.versionables_by_content[self.toolbar.obj.__class__]
 
@@ -75,15 +72,15 @@
                 f"admin:{proxy_model._meta.app_label}_{proxy_model.__name__.lower()}_publish",
                 args=(version.pk,),
             )
             item.add_button(
                 _("Publish"),
                 url=publish_url,
                 disabled=False,
-                extra_classes=["cms-btn-action", "js-action", "cms-form-post-method", "cms-versioning-js-publish-btn"],
+                extra_classes=["cms-btn-action", "cms-form-post-method", "cms-versioning-js-publish-btn"],
             )
             self.toolbar.add_item(item)
 
     def add_edit_button(self):
         """
         Only override the CMS versioning button when the object is versionable
         """
@@ -111,15 +108,15 @@
             draft_exists = Version.objects.filter(
                 object_id__in=pks_for_grouper, content_type=content_type, state=DRAFT
             ).exists()
             item.add_button(
                 _("Edit") if draft_exists else _("New Draft"),
                 url=edit_url,
                 disabled=disabled,
-                extra_classes=["cms-btn-action", "js-action", "cms-form-post-method", "cms-versioning-js-edit-btn"],
+                extra_classes=["cms-btn-action", "cms-form-post-method", "cms-versioning-js-edit-btn"],
             )
             self.toolbar.add_item(item)
 
     def _add_unlock_button(self):
         """Helper method to add an edit button to the toolbar
         """
         if LOCK_VERSIONS and self._is_versioned():
@@ -131,15 +128,14 @@
                     f"admin:{proxy_model._meta.app_label}_{proxy_model.__name__.lower()}_unlock",
                     args=(version.pk,),
                 )
                 can_unlock = self.request.user.has_perm("djangocms_versioning.delete_versionlock")
                 if can_unlock:
                     extra_classes = [
                         "cms-btn-action",
-                        "js-action",
                         "cms-form-post-method",
                         "cms-versioning-js-unlock-btn",
                     ]
                 else:
                     extra_classes = ["cms-versioning-js-unlock-btn"]
                 item.add_button(
                     _("Unlock"),
@@ -312,15 +308,15 @@
         """
         Override the default language menu for pages that are versioned.
         The default language menu is too generic so for pages we need to replace it.
         """
         # Only override the menu if it exists and a page can be found
         language_menu = self.toolbar.get_menu(LANGUAGE_MENU_IDENTIFIER, _("Language"))
         if settings.USE_I18N and language_menu and self.page:
-            # remove_item uses `items` attribute so we have to copy object
+            # remove_item uses `items` attribute, so we have to copy object
             for _item in copy(language_menu.items):
                 language_menu.remove_item(item=_item)
 
             for code, name in get_language_tuple(self.current_site.pk):
                 # Get the page content, it could be draft too!
                 page_content = self.get_page_content(language=code)
                 if page_content:
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/conditions.py` & `djangocms_versioning-2.0.2/djangocms_versioning/conditions.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/conf.py` & `djangocms_versioning-2.0.2/djangocms_versioning/conf.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/constants.py` & `djangocms_versioning-2.0.2/djangocms_versioning/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/datastructures.py` & `djangocms_versioning-2.0.2/djangocms_versioning/datastructures.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/emails.py` & `djangocms_versioning-2.0.2/djangocms_versioning/emails.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/forms.py` & `djangocms_versioning-2.0.2/djangocms_versioning/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/handlers.py` & `djangocms_versioning-2.0.2/djangocms_versioning/handlers.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/helpers.py` & `djangocms_versioning-2.0.2/djangocms_versioning/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/indicators.py` & `djangocms_versioning-2.0.2/djangocms_versioning/indicators.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/locale/de/LC_MESSAGES/django.mo` & `djangocms_versioning-2.0.2/djangocms_versioning/locale/de/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -4,14 +4,15 @@
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2023-01-10 15:29+0000\n"
 "Last-Translator: Fabian Braun <fsbraun@gmx.de>, 2023\n"
 "Language-Team: German (https://app.transifex.com/divio/teams/58664/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "\n"
 "                    Comparing %(left)s with\n"
 "                "
 msgstr ""
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/locale/de/LC_MESSAGES/django.po` & `djangocms_versioning-2.0.2/djangocms_versioning/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# 
 # Translators:
 # Fabian Braun <fsbraun@gmx.de>, 2023
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-10-02 09:37+0200\n"
 "PO-Revision-Date: 2023-01-10 15:29+0000\n"
 "Last-Translator: Fabian Braun <fsbraun@gmx.de>, 2023\n"
 "Language-Team: German (https://app.transifex.com/divio/teams/58664/de/)\n"
-"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:164 admin.py:301 admin.py:377
 msgid "State"
 msgstr "Status"
 
 #: admin.py:192 constants.py:27
@@ -486,21 +486,19 @@
 #: templates/djangocms_versioning/emails/unlock-notification.txt:2
 #, python-format
 msgid ""
 "\n"
 "The following draft version has been unlocked by %(by_user)s for their use.\n"
 "%(version_link)s\n"
 "\n"
-"Please note you will not be able to further edit this draft. Kindly reach "
-"out to %(by_user)s in case of any concerns.\n"
+"Please note you will not be able to further edit this draft. Kindly reach out to %(by_user)s in case of any concerns.\n"
 "\n"
 "This is an automated notification from Django CMS.\n"
 msgstr ""
 "\n"
 "Der folgende Entwurf wurde von %(by_user)s entsperrt.\n"
 "\n"
 "%(version_link)s\n"
 "\n"
-"Bitte beachte, dass Du diesen Entwurf nicht mehr ändern kannst. Bitte "
-"kontaktiere %(by_user)s für Rückfragen.\n"
+"Bitte beachte, dass Du diesen Entwurf nicht mehr ändern kannst. Bitte kontaktiere %(by_user)s für Rückfragen.\n"
 "\n"
 "Dies ist eine automatisierte Nachricht von Django CMS.\n"
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/locale/en/LC_MESSAGES/django.po` & `djangocms_versioning-2.0.2/djangocms_versioning/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/locale/fr/LC_MESSAGES/django.mo` & `djangocms_versioning-2.0.2/djangocms_versioning/locale/fr/LC_MESSAGES/django.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,18 +1,18 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2023-01-10 15:29+0000\n"
-"Last-Translator: François Palmier <fp@kapt.mobi>, 2023\n"
-"Language-Team: French (https://www.transifex.com/divio/teams/58664/fr/)\n"
-"Language: fr\n"
+"Last-Translator: Frédéric Roland, 2023\n"
+"Language-Team: French (https://app.transifex.com/divio/teams/58664/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 
 msgid ""
 "\n"
 "                    Comparing %(left)s with\n"
 "                "
@@ -44,17 +44,42 @@
 "        Compare %(right)s\n"
 "        "
 msgstr ""
 "\n"
 "        Comparer %(right)s\n"
 "        "
 
+msgid ""
+"\n"
+"The following draft version has been unlocked by %(by_user)s for their use.\n"
+"%(version_link)s\n"
+"\n"
+"Please note you will not be able to further edit this draft. Kindly reach "
+"out to %(by_user)s in case of any concerns.\n"
+"\n"
+"This is an automated notification from Django CMS.\n"
+msgstr ""
+"\n"
+"Le brouillon suivant a été déverrouillé par %(by_user)s pour son usage.\n"
+"%(version_link)s\n"
+"\n"
+"Notez que vous ne pourrez pas continuer a modifier ce brouillon. Vous êtes "
+"prié de contacter %(by_user)s en cas de soucis.\n"
+"\n"
+"C'est une notification automatique de Django CMS.\n"
+
 msgid " Version number: %(version_number)s"
 msgstr " Numéro de version : %(version_number)s"
 
+msgid "Action Denied. The draft version is locked by {user}"
+msgstr "Action Refusée. Le brouillon est verrouillé par {user}"
+
+msgid "Action Denied. The latest version is locked by {user}"
+msgstr "Action Refusée. La dernière version est verrouillée par {user}"
+
 msgid "Add %(name)s"
 msgstr "Ajouter %(name)s"
 
 msgid "Add Translation"
 msgstr "Ajouter une traduction"
 
 msgid "Archive"
@@ -89,44 +114,56 @@
 
 msgid "Changed"
 msgstr "Modifié"
 
 msgid "Compare Draft to Published..."
 msgstr "Comparer le brouillon à la version publiée..."
 
+msgid "Compare to {source}"
+msgstr "Comparer à {source}"
+
 msgid "Compare versions"
 msgstr "Comparer les versions"
 
 msgid "Content"
 msgstr "Contenu"
 
 msgid "Copy all plugins"
 msgstr "Copier tous les plugins"
 
 msgid "Create new draft"
 msgstr "Créer un brouillon"
 
+msgid "Created"
+msgstr "Créée"
+
 msgid "Delete Draft"
 msgstr "Supprimer le brouillon"
 
 msgid "Discard"
 msgstr "Rejeter"
 
+msgid "Discard Changes"
+msgstr "Abandonner les modifications"
+
 msgid "Discard Confirmation"
 msgstr "Confirmation du rejet"
 
 msgid "Discard existing draft and Revert"
 msgstr "Rejeter le brouillon existant et revenir en arrière"
 
 msgid "Displaying versions of \"{grouper}\""
 msgstr "Afficher les versions de \"{grouper}\""
 
 msgid "Draft"
 msgstr "Brouillon"
 
+msgid "Draft version is not locked"
+msgstr "Le brouillon n'est pas verrouillé"
+
 msgid "Edit"
 msgstr "Éditer"
 
 msgid "Empty"
 msgstr "Vide"
 
 msgid "Exactly two versions need to be selected."
@@ -137,26 +174,32 @@
 
 msgid "Language"
 msgstr "Langue"
 
 msgid "Language must be set to a supported language!"
 msgstr "La langue doit être définie comme une langue prise en charge !"
 
+msgid "Locked by %(user)s"
+msgstr "Verrouillée par %(user)s"
+
 msgid "Manage Versions"
 msgstr "Gérer les versions"
 
 msgid "Manage Versions..."
 msgstr "Gérer les versions..."
 
 msgid "Manage versions"
 msgstr "Gérer les versions"
 
 msgid "Modified"
 msgstr "Modifié"
 
+msgid "New Draft"
+msgstr "Nouveau Brouillon"
+
 msgid "No available title"
 msgstr "Aucun titre disponible"
 
 msgid "No other language available"
 msgstr "Aucune autre langue disponible"
 
 msgid "No, take me back"
@@ -201,14 +244,23 @@
 
 msgid "The last version has been deleted"
 msgstr "La dernière version a été supprimée"
 
 msgid "This view only supports POST method."
 msgstr "Cette vue ne prend en charge que la méthode POST."
 
+msgid "Unlock"
+msgstr "Déverrouiller"
+
+msgid "Unlock (%(message)s)"
+msgstr "Déverrouiller (%(message)s)"
+
+msgid "Unlocked"
+msgstr "Déverrouillée"
+
 msgid "Unpublish"
 msgstr "Dépublier"
 
 msgid "Unpublished"
 msgstr "Non publié"
 
 msgid ""
@@ -232,14 +284,17 @@
 
 msgid "Version cannot be published"
 msgstr "La version ne peut pas être publiée"
 
 msgid "Version cannot be unpublished"
 msgstr "La version ne peut pas être dépubliée"
 
+msgid "Version is already locked"
+msgstr "La version  est déjà verrouillée"
+
 msgid "Version is not a draft"
 msgstr "La version n'est pas un brouillon"
 
 msgid "Version is not in archived or unpublished state"
 msgstr "La version n'est pas archivé ou non publié"
 
 msgid "Version is not in draft or published state"
@@ -253,14 +308,17 @@
 
 msgid "Version number: %(version_number)s"
 msgstr "Numéro de version : %(version_number)s"
 
 msgid "Version published"
 msgstr "Version publiée"
 
+msgid "Version unlocked"
+msgstr "Version déverrouillée"
+
 msgid "Version unpublished"
 msgstr "Version non publiée"
 
 msgid "Versions"
 msgstr "Versions"
 
 msgid "View Published"
@@ -274,21 +332,30 @@
 
 msgid "Yes, I'm sure"
 msgstr "Oui, je suis sûr"
 
 msgid "You do not have permission to copy these plugins."
 msgstr "Vous n'avez pas la permission de copier ces plugins."
 
+msgid "You do not have permission to remove the version lock"
+msgstr "Vous n'avez pas la permission de retirer le verrouillage de version"
+
 msgid "author"
 msgstr "auteur"
 
 msgid "django CMS Versioning"
 msgstr "django CMS Versioning"
 
 msgid "from %s"
 msgstr "de %s"
 
+msgid "locked"
+msgstr "verrouillé"
+
+msgid "locked by"
+msgstr "verrouillée par"
+
 msgid "source"
 msgstr "source"
 
 msgid "status"
 msgstr "statut"
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/locale/fr/LC_MESSAGES/django.po` & `djangocms_versioning-2.0.2/djangocms_versioning/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# 
 # Translators:
 # François Palmier <fp@kapt.mobi>, 2023
 # Frédéric Roland, 2023
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-10-02 09:37+0200\n"
 "PO-Revision-Date: 2023-01-10 15:29+0000\n"
 "Last-Translator: Frédéric Roland, 2023\n"
 "Language-Team: French (https://app.transifex.com/divio/teams/58664/fr/)\n"
-"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
-"1000000 == 0 ? 1 : 2;\n"
+"Language: fr\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: admin.py:164 admin.py:301 admin.py:377
 msgid "State"
 msgstr "État"
 
 #: admin.py:192 constants.py:27
 msgid "Empty"
@@ -489,20 +488,18 @@
 #: templates/djangocms_versioning/emails/unlock-notification.txt:2
 #, python-format
 msgid ""
 "\n"
 "The following draft version has been unlocked by %(by_user)s for their use.\n"
 "%(version_link)s\n"
 "\n"
-"Please note you will not be able to further edit this draft. Kindly reach "
-"out to %(by_user)s in case of any concerns.\n"
+"Please note you will not be able to further edit this draft. Kindly reach out to %(by_user)s in case of any concerns.\n"
 "\n"
 "This is an automated notification from Django CMS.\n"
 msgstr ""
 "\n"
 "Le brouillon suivant a été déverrouillé par %(by_user)s pour son usage.\n"
 "%(version_link)s\n"
 "\n"
-"Notez que vous ne pourrez pas continuer a modifier ce brouillon. Vous êtes "
-"prié de contacter %(by_user)s en cas de soucis.\n"
+"Notez que vous ne pourrez pas continuer a modifier ce brouillon. Vous êtes prié de contacter %(by_user)s en cas de soucis.\n"
 "\n"
 "C'est une notification automatique de Django CMS.\n"
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/locale/nl/LC_MESSAGES/django.mo` & `djangocms_versioning-2.0.2/djangocms_versioning/locale/nl/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,18 +1,18 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2023-01-10 15:29+0000\n"
 "Last-Translator: Stefan van den Eertwegh <stefan@corebyte.nl>, 2023\n"
 "Language-Team: Dutch (https://app.transifex.com/divio/teams/58664/nl/)\n"
-"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "\n"
 "                    Comparing %(left)s with\n"
 "                "
 msgstr ""
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/locale/nl/LC_MESSAGES/django.po` & `djangocms_versioning-2.0.2/djangocms_versioning/locale/nl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# 
 # Translators:
 # Fabian Braun <fsbraun@gmx.de>, 2023
 # Stefan van den Eertwegh <stefan@corebyte.nl>, 2023
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-10-02 09:37+0200\n"
 "PO-Revision-Date: 2023-01-10 15:29+0000\n"
 "Last-Translator: Stefan van den Eertwegh <stefan@corebyte.nl>, 2023\n"
 "Language-Team: Dutch (https://app.transifex.com/divio/teams/58664/nl/)\n"
-"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: nl\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:164 admin.py:301 admin.py:377
 msgid "State"
 msgstr "Status"
 
 #: admin.py:192 constants.py:27
@@ -488,20 +488,17 @@
 #: templates/djangocms_versioning/emails/unlock-notification.txt:2
 #, python-format
 msgid ""
 "\n"
 "The following draft version has been unlocked by %(by_user)s for their use.\n"
 "%(version_link)s\n"
 "\n"
-"Please note you will not be able to further edit this draft. Kindly reach "
-"out to %(by_user)s in case of any concerns.\n"
+"Please note you will not be able to further edit this draft. Kindly reach out to %(by_user)s in case of any concerns.\n"
 "\n"
 "This is an automated notification from Django CMS.\n"
 msgstr ""
 "\n"
-"De volgende concept versie is van het slot af door%(by_user)svoor hun "
-"gebruik.\n"
+"De volgende concept versie is van het slot af door%(by_user)svoor hun gebruik.\n"
 " %(version_link)s\n"
-"Let op: je kunt niet verder bewerken in dit concept. Neem asjeblieft contact "
-"op met %(by_user)s in geval van enige zorgen. \n"
+"Let op: je kunt niet verder bewerken in dit concept. Neem asjeblieft contact op met %(by_user)s in geval van enige zorgen. \n"
 "\n"
 "Dit is een geautomatiseerde notificatie van Django CMS.\n"
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/locale/sq/LC_MESSAGES/django.mo` & `djangocms_versioning-2.0.2/djangocms_versioning/locale/sq/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,18 +1,18 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2023-01-10 15:29+0000\n"
 "Last-Translator: Besnik Bleta <besnik@programeshqip.org>, 2023\n"
-"Language-Team: Albanian (https://www.transifex.com/divio/teams/58664/sq/)\n"
-"Language: sq\n"
+"Language-Team: Albanian (https://app.transifex.com/divio/teams/58664/sq/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: sq\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "\n"
 "                    Comparing %(left)s with\n"
 "                "
 msgstr ""
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/locale/sq/LC_MESSAGES/django.po` & `djangocms_versioning-2.0.2/djangocms_versioning/locale/sq/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# 
 # Translators:
 # Besnik Bleta <besnik@programeshqip.org>, 2023
-#
+# 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-10-02 09:37+0200\n"
 "PO-Revision-Date: 2023-01-10 15:29+0000\n"
 "Last-Translator: Besnik Bleta <besnik@programeshqip.org>, 2023\n"
-"Language-Team: Albanian (https://www.transifex.com/divio/teams/58664/sq/)\n"
-"Language: sq\n"
+"Language-Team: Albanian (https://app.transifex.com/divio/teams/58664/sq/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: sq\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: admin.py:164 admin.py:301 admin.py:377
 msgid "State"
 msgstr "Gjendje"
 
 #: admin.py:192 constants.py:27
@@ -72,18 +72,16 @@
 
 #: admin.py:721 indicators.py:54 indicators.py:60
 #: templates/djangocms_versioning/admin/icons/unpublish_icon.html:3
 msgid "Unpublish"
 msgstr "Hiqe nga të botuar"
 
 #: admin.py:758 cms_toolbars.py:115
-#, fuzzy
-#| msgid "Draft"
 msgid "New Draft"
-msgstr "Skicë"
+msgstr ""
 
 #: admin.py:779 cms_toolbars.py:177
 #: templates/djangocms_versioning/admin/icons/revert_icon.html:3
 msgid "Revert"
 msgstr "Riktheje"
 
 #: admin.py:798 templates/djangocms_versioning/admin/icons/discard_icon.html:3
@@ -131,24 +129,20 @@
 msgstr "Versioni u shbotua"
 
 #: admin.py:1163
 msgid "The last version has been deleted"
 msgstr "Versioni i fundit është fshirë"
 
 #: admin.py:1249
-#, fuzzy
-#| msgid "You do not have permission to copy these plugins."
 msgid "You do not have permission to remove the version lock"
-msgstr "S’keni leje të kopjoni këto shtojca."
+msgstr ""
 
 #: admin.py:1254
-#, fuzzy
-#| msgid "Version unpublished"
 msgid "Version unlocked"
-msgstr "Versioni u shbotua"
+msgstr ""
 
 #: admin.py:1303
 #, python-brace-format
 msgid "Displaying versions of \"{grouper}\""
 msgstr "Po shfaqen versione të “{grouper}”"
 
 #: apps.py:8
@@ -172,24 +166,21 @@
 msgstr "S’keni leje të kopjoni këto shtojca."
 
 #: cms_toolbars.py:207
 msgid "Manage Versions"
 msgstr "Administroni Versione"
 
 #: cms_toolbars.py:210
-#, fuzzy, python-brace-format
-#| msgid "Compare to {state} source"
+#, python-brace-format
 msgid "Compare to {source}"
-msgstr "Krahasoje me burimin {state}"
+msgstr ""
 
 #: cms_toolbars.py:226 indicators.py:66
-#, fuzzy
-#| msgid "Discard"
 msgid "Discard Changes"
-msgstr "Hidhe tej"
+msgstr ""
 
 #: cms_toolbars.py:262
 msgid "View Published"
 msgstr "Shihni të Botuarin"
 
 #: cms_toolbars.py:317
 msgid "Language"
@@ -273,18 +264,16 @@
 
 #: models.py:31
 #, python-brace-format
 msgid "Action Denied. The draft version is locked by {user}"
 msgstr ""
 
 #: models.py:86
-#, fuzzy
-#| msgid "Create new draft"
 msgid "Created"
-msgstr "Krijoni një skicë të re"
+msgstr ""
 
 #: models.py:89
 msgid "author"
 msgstr "autor"
 
 #: models.py:102
 msgid "status"
@@ -326,24 +315,20 @@
 msgstr "Versioni s’është nën gjendjen “i arkivuar” ose “i pabotuar”"
 
 #: models.py:459
 msgid "Version is not in draft or published state"
 msgstr "Versioni s’është nën gjendjen “skicë” ose “i botuar”"
 
 #: models.py:467
-#, fuzzy
-#| msgid "Version archived"
 msgid "Version is already locked"
-msgstr "Versioni u arkivua"
+msgstr ""
 
 #: models.py:473
-#, fuzzy
-#| msgid "Version is not a draft"
 msgid "Draft version is not locked"
-msgstr "Versioni s’është skicë"
+msgstr ""
 
 #: templates/admin/djangocms_versioning/versioning_breadcrumbs.html:3
 #: templates/djangocms_versioning/admin/grouper_form.html:9
 msgid "Home"
 msgstr "Kreu"
 
 #: templates/admin/djangocms_versioning/versioning_breadcrumbs.html:7
@@ -502,21 +487,11 @@
 #: templates/djangocms_versioning/emails/unlock-notification.txt:2
 #, python-format
 msgid ""
 "\n"
 "The following draft version has been unlocked by %(by_user)s for their use.\n"
 "%(version_link)s\n"
 "\n"
-"Please note you will not be able to further edit this draft. Kindly reach "
-"out to %(by_user)s in case of any concerns.\n"
+"Please note you will not be able to further edit this draft. Kindly reach out to %(by_user)s in case of any concerns.\n"
 "\n"
 "This is an automated notification from Django CMS.\n"
 msgstr ""
-
-#~ msgid "actions"
-#~ msgstr "veprime"
-
-#~ msgid "version number"
-#~ msgstr "numër versioni"
-
-#~ msgid "Delete Changes"
-#~ msgstr "Fshiji Ndryshimet"
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/management/commands/create_versions.py` & `djangocms_versioning-2.0.2/djangocms_versioning/management/commands/create_versions.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/managers.py` & `djangocms_versioning-2.0.2/djangocms_versioning/managers.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0001_initial.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0003_version.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0003_version.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0004_auto_20180730_1135.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0004_auto_20180730_1135.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0007_auto_20180813_1407.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0007_auto_20180813_1407.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0008_auto_20180820_1754.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0008_auto_20180820_1754.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0009_cms_pagecontent_remove_unique_constraint.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0009_cms_pagecontent_remove_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0010_version_proxies.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0010_version_proxies.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0012_create_version_numbers.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0012_create_version_numbers.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0014_version_source.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0014_version_source.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0015_version_modified.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0015_version_modified.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0016_alter_version_content_type.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0016_alter_version_content_type.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/migrations/0016_auto_20230505_0934.py` & `djangocms_versioning-2.0.2/djangocms_versioning/migrations/0016_auto_20230505_0934.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/models.py` & `djangocms_versioning-2.0.2/djangocms_versioning/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/operations.py` & `djangocms_versioning-2.0.2/djangocms_versioning/operations.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/plugin_rendering.py` & `djangocms_versioning-2.0.2/djangocms_versioning/plugin_rendering.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/css/source.css` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/css/source.css`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/css/versioning.css` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/css/versioning.css`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/actions.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/actions.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/admin/versioning-actions.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/admin/versioning-actions.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/base.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/base.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/compare.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/compare.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/dist/bundle.prettydiff.min.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/dist/bundle.prettydiff.min.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/dist/bundle.versioning.min.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/dist/bundle.versioning.min.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/get-dist-path.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/get-dist-path.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/indicators.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/indicators.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/api/dom.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/api/dom.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/difflib.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/difflib.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/diffview.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/diffview.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/htmldiff.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/htmldiff.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/libs/tidy.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/libs/tidy.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/prettydiff.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/prettydiff.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/js/versioning.js` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/js/versioning.js`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/discard.svg` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/discard.svg`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/manage_versions.svg` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/manage_versions.svg`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/preview.svg` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/preview.svg`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/static/djangocms_versioning/svg/unpublish.svg` & `djangocms_versioning-2.0.2/djangocms_versioning/static/djangocms_versioning/svg/unpublish.svg`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/templates/admin/djangocms_versioning/versioning_breadcrumbs.html` & `djangocms_versioning-2.0.2/djangocms_versioning/templates/admin/djangocms_versioning/versioning_breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/archive_confirmation.html` & `djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/archive_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/compare.html` & `djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/compare.html`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/discard_confirmation.html` & `djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/discard_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/grouper_form.html` & `djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/grouper_form.html`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/icons/base.html` & `djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/icons/base.html`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/revert_confirmation.html` & `djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/revert_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/templates/djangocms_versioning/admin/unpublish_confirmation.html` & `djangocms_versioning-2.0.2/djangocms_versioning/templates/djangocms_versioning/admin/unpublish_confirmation.html`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/blogpost/admin.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/blogpost/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/blogpost/cms_config.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/blogpost/cms_config.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/blogpost/models.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/blogpost/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extended_polls/migrations/0001_initial.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extended_polls/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/extensions/migrations/0001_initial.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/extensions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/factories.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/factories.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/incorrectly_configured_blogpost/cms_config.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/incorrectly_configured_blogpost/cms_config.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/admin.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/cms_config.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/cms_config.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/migrations/0001_initial.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/polls/models.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/polls/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/test_helpers.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/text/migrations/0001_initial.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/text/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/unversioned_editable_app/models.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/unversioned_editable_app/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/test_utils/unversioned_editable_app/views.py` & `djangocms_versioning-2.0.2/djangocms_versioning/test_utils/unversioned_editable_app/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning/versionables.py` & `djangocms_versioning-2.0.2/djangocms_versioning/versionables.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning.egg-info/PKG-INFO` & `djangocms_versioning-2.0.2/djangocms_versioning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: djangocms-versioning
-Version: 2.0.1
+Version: 2.0.2
 Home-page: http://github.com/django-cms/djangocms-versioning
 Author: Divio AG
 Author-email: info@divio.ch
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 License-File: LICENSE.txt
-Requires-Dist: Django>=1.11
-Requires-Dist: django-cms
-Requires-Dist: django-fsm
+Requires-Dist: Django>=3.2
+Requires-Dist: django-cms>=4.1.1
+Requires-Dist: django-fsm<3
 
 |django| |djangocms4|
 
 *********************
 django CMS Versioning
 *********************
```

### Comparing `djangocms-versioning-2.0.1/djangocms_versioning.egg-info/SOURCES.txt` & `djangocms_versioning-2.0.2/djangocms_versioning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 djangocms_versioning/signals.py
 djangocms_versioning/versionables.py
 djangocms_versioning.egg-info/PKG-INFO
 djangocms_versioning.egg-info/SOURCES.txt
 djangocms_versioning.egg-info/dependency_links.txt
 djangocms_versioning.egg-info/requires.txt
 djangocms_versioning.egg-info/top_level.txt
+djangocms_versioning/locale/ar/LC_MESSAGES/django.mo
+djangocms_versioning/locale/ar/LC_MESSAGES/django.po
 djangocms_versioning/locale/de/LC_MESSAGES/django.mo
 djangocms_versioning/locale/de/LC_MESSAGES/django.po
 djangocms_versioning/locale/en/LC_MESSAGES/django.mo
 djangocms_versioning/locale/en/LC_MESSAGES/django.po
 djangocms_versioning/locale/fr/LC_MESSAGES/django.mo
 djangocms_versioning/locale/fr/LC_MESSAGES/django.po
 djangocms_versioning/locale/nl/LC_MESSAGES/django.mo
```

### Comparing `djangocms-versioning-2.0.1/pyproject.toml` & `djangocms_versioning-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/setup.cfg` & `djangocms_versioning-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/setup.py` & `djangocms_versioning-2.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 import djangocms_versioning
 
 INSTALL_REQUIREMENTS = [
-    "Django>=1.11",
-    "django-cms",
-    "django-fsm"
+    "Django>=3.2",
+    "django-cms>=4.1.1",
+    "django-fsm<3"
 ]
 
 setup(
     name="djangocms-versioning",
     packages=find_packages(),
     include_package_data=True,
     version=djangocms_versioning.__version__,
```

### Comparing `djangocms-versioning-2.0.1/tests/test_0_migrations.py` & `djangocms_versioning-2.0.2/tests/test_0_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_admin.py` & `djangocms_versioning-2.0.2/tests/test_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,17 +524,17 @@
         )
         expected_enabled_state = (
             '<a class="btn cms-form-get-method '
             'cms-action-btn '
             'cms-action-revert '
             'js-action '
             'js-keep-sideframe" '
-            'href="%s" '
+            f'href="{draft_revert_url}" '
             'title="Revert">'
-        ) % draft_revert_url
+        )
         self.assertIn(expected_enabled_state, actual_enabled_control.replace("\n", ""))
 
     def test_revert_action_link_for_draft_state(self):
         """
         The revert url should be null for draft state
         """
         version = factories.PollVersionFactory(state=constants.DRAFT)
@@ -595,17 +595,17 @@
 
         expected_enabled_state = (
             '<a class="btn cms-form-get-method '
             'cms-action-btn '
             'cms-action-discard '
             'js-action '
             'js-keep-sideframe" '
-            'href="%s" '
+            f'href="{draft_discard_url}" '
             'title="Discard">'
-        ) % draft_discard_url
+        )
         self.assertIn(expected_enabled_state, actual_enabled_control.replace("\n", ""))
 
     def test_discard_action_link_for_archive_state(self):
         """
         The revert url should be null for archive state
         """
         version = factories.PollVersionFactory(state=constants.ARCHIVED)
@@ -660,19 +660,19 @@
             self.versionable.version_model_proxy, "revert", archive_version.pk
         )
         expected_disabled_control = (
             '<a class="btn cms-form-get-method cms-action-btn '
             'cms-action-revert '
             'js-action '
             'js-keep-sideframe" '
-            'href="%s" '
+            f'href="{draft_revert_url}" '
             'title="Revert">'
             '<span class="cms-icon cms-icon-undo"></span>'
             '</a>'
-        ) % draft_revert_url
+        )
 
         self.assertIn(
             expected_disabled_control, actual_disabled_control.replace("\n", "")
         )
 
     def test_edit_action_link_sideframe_editing_disabled_state(self):
         """
```

### Comparing `djangocms-versioning-2.0.1/tests/test_automatic_version_generation.py` & `djangocms_versioning-2.0.2/tests/test_automatic_version_generation.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_checks.py` & `djangocms_versioning-2.0.2/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_cms_config.py` & `djangocms_versioning-2.0.2/tests/test_cms_config.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_content_models.py` & `djangocms_versioning-2.0.2/tests/test_content_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_datastructures.py` & `djangocms_versioning-2.0.2/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_extensions.py` & `djangocms_versioning-2.0.2/tests/test_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         """
         When hitting the monkeypatched save method, with a draft pagecontent, ensure that we don't see failures
         due to versioning overriding monkeypatches
         """
         poll_extension = PollTitleExtensionFactory(extended_object=self.version.content)
         model_site = PollExtensionAdmin(admin_site=admin.AdminSite(), model=PollPageContentExtension)
         test_url = admin_reverse("extended_polls_pollpagecontentextension_change", args=(poll_extension.pk,))
-        test_url += "?extended_object=%s" % self.version.content.pk
+        test_url += f"?extended_object={self.version.content.pk}"
         request = RequestFactory().post(path=test_url)
         request.user = self.get_superuser()
 
         poll_extension.votes = 1
         model_site.save_model(request, poll_extension, form=None, change=False)
 
         self.assertEqual(PollPageContentExtension._base_manager.first().votes, 1)
@@ -133,15 +133,15 @@
         the Title Extension the date modified in a version should also be updated to reflect
         the correct date timestamp.
         """
         poll_extension = PollTitleExtensionFactory(extended_object=self.version.content)
         model_site = PollExtensionAdmin(admin_site=admin.AdminSite(), model=PollPageContentExtension)
         pre_changes_date_modified = Version.objects.get(id=self.version.pk).modified
         test_url = admin_reverse("extended_polls_pollpagecontentextension_change", args=(poll_extension.pk,))
-        test_url += "?extended_object=%s" % self.version.content.pk
+        test_url += f"?extended_object={self.version.content.pk}"
 
         request = RequestFactory().post(path=test_url)
         request.user = self.get_superuser()
         model_site.save_model(request, poll_extension, form=None, change=False)
 
         post_changes_date_modified = Version.objects.get(id=self.version.pk).modified
 
@@ -151,11 +151,11 @@
         """
         When hitting the add view, without the monkeypatch, the pagecontent queryset will be filtered to only show
         published. Hit it with a draft, to make sure the monkeypatch works.
         """
         with self.login_user_context(self.get_superuser()):
             response = self.client.get(
                 admin_reverse("extended_polls_pollpagecontentextension_add") +
-                "?extended_object=%s" % self.version.content.pk,
+                f"?extended_object={self.version.content.pk}",
                 follow=True
             )
             self.assertEqual(response.status_code, 200)
```

### Comparing `djangocms-versioning-2.0.1/tests/test_forms.py` & `djangocms_versioning-2.0.2/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_handlers.py` & `djangocms_versioning-2.0.2/tests/test_handlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
             pv.content.save()
         pv = Version.objects.get(pk=pv.pk)
         self.assertEqual(pv.modified, dt)
 
     def test_add_plugin(self):
         version = factories.PageVersionFactory()
         placeholder = factories.PlaceholderFactory(source=version.content)
+        placeholder.page.get_absolute_url = lambda *args, **kwargs: "/test_page/"  # Fake URL needed for URI
         poll = factories.PollFactory()
         dt = datetime(2016, 6, 6)
         with freeze_time(dt):
             endpoint = self.get_add_plugin_uri(
                 placeholder=placeholder,
                 plugin_type="PollPlugin",
                 language=version.content.language,
@@ -41,14 +42,15 @@
         version = factories.PageVersionFactory()
         placeholder = factories.PlaceholderFactory(source=version.content)
         poll = factories.PollFactory()
 
         plugin = add_plugin(
             placeholder, "PollPlugin", version.content.language, poll=poll
         )
+        plugin.page.get_absolute_url = lambda *args, **kwargs: "/test_page/"  # Fake URL needed for URI
 
         dt = datetime(2016, 6, 6)
         with freeze_time(dt):
             endpoint = self.get_change_plugin_uri(plugin)
             data = {"poll": poll.pk}
 
             with self.login_user_context(self.get_superuser()):
@@ -57,14 +59,15 @@
 
         version = Version.objects.get(pk=version.pk)
         self.assertEqual(version.modified, dt)
 
     def test_clear_placeholder(self):
         version = factories.PageVersionFactory()
         placeholder = factories.PlaceholderFactory(source=version.content)
+        placeholder.page.get_absolute_url = lambda *args, **kwargs: "/test_page/"  # Fake URL needed for URI
 
         dt = datetime(2016, 6, 6)
         with freeze_time(dt):
             endpoint = self.get_clear_placeholder_url(placeholder)
 
             with self.login_user_context(self.get_superuser()):
                 response = self.client.post(endpoint, {"test": 0})
@@ -77,14 +80,15 @@
         version = factories.PageVersionFactory()
         placeholder = factories.PlaceholderFactory(source=version.content)
         poll = factories.PollFactory()
 
         plugin = add_plugin(
             placeholder, "PollPlugin", version.content.language, poll=poll
         )
+        plugin.page.get_absolute_url = lambda *args, **kwargs: "/test_page/"  # Fake URL needed for URI
 
         dt = datetime(2016, 6, 6)
         with freeze_time(dt):
             endpoint = self.get_delete_plugin_uri(plugin)
             data = {"poll": poll.pk}
 
             with self.login_user_context(self.get_superuser()):
@@ -99,14 +103,15 @@
         source_placeholder = factories.PlaceholderFactory(source=version.content)
         target_placeholder = factories.PlaceholderFactory(source=version.content)
         poll = factories.PollFactory()
 
         plugin = add_plugin(
             source_placeholder, "PollPlugin", version.content.language, poll=poll
         )
+        plugin.page.get_absolute_url = lambda *args, **kwargs: "/test_page/"  # Fake URL needed for URI
 
         dt = datetime(2016, 6, 6)
         with freeze_time(dt):
             endpoint = self.get_copy_plugin_uri(plugin)
             data = {
                 "source_language": version.content.language,
                 "source_placeholder_id": source_placeholder.pk,
@@ -161,15 +166,15 @@
         source_placeholder = factories.PlaceholderFactory(source=version.content)
         target_placeholder = factories.PlaceholderFactory(source=version.content)
         poll = factories.PollFactory()
 
         plugin = add_plugin(
             source_placeholder, "PollPlugin", version.content.language, poll=poll
         )
-
+        plugin.page.get_absolute_url = lambda *args, **kwargs: "/test_page/"
         dt = datetime(2016, 6, 6)
         with freeze_time(dt):
             endpoint = self.get_move_plugin_uri(plugin)
             data = {
                 "plugin_id": plugin.pk,
                 "placeholder_id": target_placeholder.pk,
                 "target_language": version.content.language,
@@ -193,14 +198,15 @@
             user=self.get_superuser(),
             clipboard=Placeholder.objects.create(slot="clipboard"),
         )
 
         plugin = add_plugin(
             placeholder, "PollPlugin", version.content.language, poll=poll
         )
+        plugin.page.get_absolute_url = lambda *args, **kwargs: "/test_page/"  # Fake URL needed for URI
 
         dt = datetime(2016, 6, 6)
         with freeze_time(dt):
             endpoint = self.get_move_plugin_uri(plugin)
             data = {
                 "plugin_id": plugin.pk,
                 "target_language": version.content.language,
@@ -219,14 +225,15 @@
         source_placeholder = factories.PlaceholderFactory(source=version.content)
         target_placeholder = factories.PlaceholderFactory(source=version.content)
         poll = factories.PollFactory()
 
         plugin = add_plugin(
             source_placeholder, "PollPlugin", version.content.language, poll=poll
         )
+        plugin.page.get_absolute_url = lambda *args, **kwargs: "/test_page/"  # Fake URL needed for URI
 
         dt = datetime(2016, 6, 6)
         with freeze_time(dt):
             endpoint = self.get_move_plugin_uri(plugin)
             data = {
                 "plugin_id": plugin.pk,
                 "target_language": version.content.language,
```

### Comparing `djangocms-versioning-2.0.1/tests/test_indicators.py` & `djangocms_versioning-2.0.2/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_integration_with_core.py` & `djangocms_versioning-2.0.2/tests/test_integration_with_core.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_locking.py` & `djangocms_versioning-2.0.2/tests/test_locking.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,20 +390,20 @@
         The edit action is disabled for a different user to the locked user
         """
         version = factories.PollVersionFactory(created_by=self.user_author, locked_by=self.user_author)
         author_request = RequestFactory()
         author_request.user = self.user_author
         otheruser_request = RequestFactory()
         otheruser_request.user = self.superuser
-        expected_disabled_state = "inactive"
+        expected_disabled_state = ""
 
         actual_disabled_state = self.version_admin._get_edit_link(version, otheruser_request)
 
         self.assertFalse(version.check_edit_redirect.as_bool(self.superuser))
-        self.assertIn(expected_disabled_state, actual_disabled_state)
+        self.assertEqual(expected_disabled_state, actual_disabled_state)
 
 
 @override_settings(DJANGOCMS_VERSIONING_LOCK_VERSIONS=True)
 class VersionLockEditActionSideFrameTestCase(CMSTestCase):
     def setUp(self):
         import importlib
         importlib.reload(conf)
@@ -835,15 +835,15 @@
         admin_url = self.get_admin_url(
             versionable.version_model_proxy, "edit_redirect", version.pk
         )
         self.assertEqual(edit_button.url, admin_url)
         self.assertFalse(edit_button.disabled)
         self.assertListEqual(
             edit_button.extra_classes,
-            ["cms-btn-action", "js-action", "cms-form-post-method", "cms-versioning-js-edit-btn"]
+            ["cms-btn-action", "cms-form-post-method", "cms-versioning-js-edit-btn"]
         )
 
     def test_lock_message_when_content_is_locked(self):
         user = self.get_superuser()
         user.first_name = "Firstname"
         user.last_name = "Lastname"
         user.save()
```

### Comparing `djangocms-versioning-2.0.1/tests/test_management_commands.py` & `djangocms_versioning-2.0.2/tests/test_management_commands.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_menus.py` & `djangocms_versioning-2.0.2/tests/test_menus.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_models.py` & `djangocms_versioning-2.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_permissions.py` & `djangocms_versioning-2.0.2/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_settings.py` & `djangocms_versioning-2.0.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_signals.py` & `djangocms_versioning-2.0.2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_states.py` & `djangocms_versioning-2.0.2/tests/test_states.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_toolbars.py` & `djangocms_versioning-2.0.2/tests/test_toolbars.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         publish_button = find_toolbar_buttons("Publish", toolbar.toolbar)[0]
         self.assertEqual(publish_button.name, "Publish")
         self.assertEqual(publish_button.url, self._get_publish_url(version))
         self.assertFalse(publish_button.disabled)
         self.assertListEqual(
             publish_button.extra_classes,
-            ["cms-btn-action", "js-action", "cms-form-post-method", "cms-versioning-js-publish-btn"],
+            ["cms-btn-action", "cms-form-post-method", "cms-versioning-js-publish-btn"],
         )
 
     def test_revert_in_toolbar_in_preview_mode(self):
         """Test for Revert button outside mode"""
 
         version = PollVersionFactory()
         version.archive(self.get_superuser())
@@ -146,15 +146,15 @@
         self.assertEqual(
             edit_button.url,
             self._get_edit_url(version, VersioningCMSConfig.versioning[0]),
         )
         self.assertFalse(edit_button.disabled)
         self.assertListEqual(
             edit_button.extra_classes,
-            ["cms-btn-action", "js-action", "cms-form-post-method", "cms-versioning-js-edit-btn"]
+            ["cms-btn-action", "cms-form-post-method", "cms-versioning-js-edit-btn"]
         )
 
     def test_edit_not_in_toolbar_in_edit_mode(self):
         version = PollVersionFactory()
         toolbar = get_toolbar(
             version.content, user=self.get_superuser(), edit_mode=True
         )
@@ -337,26 +337,40 @@
 
     def test_view_published_in_toolbar_in_edit_mode_for_published_page(self):
         """
         The 'View Published' control is only relevant for pages that
         are published
         """
         published_version = PageVersionFactory(content__language="en", state=PUBLISHED)
+        # Create URL
+        PageUrlFactory(
+            page=published_version.content.page,
+            language=published_version.content.language,
+            path=slugify("test_page"),
+            slug=slugify("test_page"),
+        )
         toolbar = get_toolbar(published_version.content, edit_mode=True)
 
         toolbar.post_template_populate()
 
         self.assertTrue(toolbar_button_exists("View Published", toolbar.toolbar))
 
     def test_view_published_in_toolbar_in_preview_mode_for_published_page(self):
         """
         The 'View Published' control is only relevant for pages that
         are published
         """
         published_version = PageVersionFactory(content__language="en", state=PUBLISHED)
+        # Create URL
+        PageUrlFactory(
+            page=published_version.content.page,
+            language=published_version.content.language,
+            path=slugify("test_page"),
+            slug=slugify("test_page"),
+        )
         toolbar = get_toolbar(published_version.content, preview_mode=True)
 
         toolbar.post_template_populate()
 
         self.assertTrue(toolbar_button_exists("View Published", toolbar.toolbar))
 
     def test_view_published_not_in_toolbar_in_edit_mode_for_draft_page(self):
```

### Comparing `djangocms-versioning-2.0.1/tests/test_version_list.py` & `djangocms_versioning-2.0.2/tests/test_version_list.py`

 * *Files identical despite different names*

### Comparing `djangocms-versioning-2.0.1/tests/test_versionables.py` & `djangocms_versioning-2.0.2/tests/test_versionables.py`

 * *Files identical despite different names*

