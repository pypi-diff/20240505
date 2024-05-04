# Comparing `tmp/django_formset-1.4.tar.gz` & `tmp/django_formset-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_formset-1.4.tar", last modified: Wed May  1 11:04:01 2024, max compression
+gzip compressed data, was "django_formset-1.4.1.tar", last modified: Sat May  4 22:05:05 2024, max compression
```

## Comparing `django_formset-1.4.tar` & `django_formset-1.4.1.tar`

### file list

```diff
@@ -1,470 +1,470 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.019567 django_formset-1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-01 11:03:36.000000 django_formset-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-01 11:03:36.000000 django_formset-1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-05-01 11:04:01.019567 django_formset-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-01 11:03:36.000000 django_formset-1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.015567 django_formset-1.4/django_formset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-05-01 11:04:00.000000 django_formset-1.4/django_formset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-01 11:04:00.000000 django_formset-1.4/django_formset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:04:00.000000 django_formset-1.4/django_formset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:04:00.000000 django_formset-1.4/django_formset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 11:04:00.000000 django_formset-1.4/django_formset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 11:04:00.000000 django_formset-1.4/django_formset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.963567 django_formset-1.4/formset/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-01 11:03:36.000000 django_formset-1.4/formset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-01 11:03:36.000000 django_formset-1.4/formset/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-01 11:03:36.000000 django_formset-1.4/formset/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    23321 2024-05-01 11:03:36.000000 django_formset-1.4/formset/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-01 11:03:36.000000 django_formset-1.4/formset/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-01 11:03:36.000000 django_formset-1.4/formset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-01 11:03:36.000000 django_formset-1.4/formset/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-01 11:03:36.000000 django_formset-1.4/formset/fieldset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.943567 django_formset-1.4/formset/locale/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.963567 django_formset-1.4/formset/locale/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/af/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/af/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.943567 django_formset-1.4/formset/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.963567 django_formset-1.4/formset/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.943567 django_formset-1.4/formset/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.963567 django_formset-1.4/formset/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/bg/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/bg/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.943567 django_formset-1.4/formset/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.963567 django_formset-1.4/formset/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/ca/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/ca/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.943567 django_formset-1.4/formset/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.963567 django_formset-1.4/formset/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.943567 django_formset-1.4/formset/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.963567 django_formset-1.4/formset/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/da/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/da/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.943567 django_formset-1.4/formset/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.963567 django_formset-1.4/formset/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.943567 django_formset-1.4/formset/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/eo/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/et/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/et/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/eu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/eu/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/eu_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/fa/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/fa/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/fi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/fi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/he/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/he/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/he_IL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.967567 django_formset-1.4/formset/locale/he_IL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/he_IL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/he_IL/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.971567 django_formset-1.4/formset/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/hr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/hr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.971567 django_formset-1.4/formset/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/hu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/hu/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.971567 django_formset-1.4/formset/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/hy/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/hy/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.971567 django_formset-1.4/formset/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/it/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/it/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.971567 django_formset-1.4/formset/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/ja/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/ja/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.971567 django_formset-1.4/formset/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.971567 django_formset-1.4/formset/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/lt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/lt/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.947567 django_formset-1.4/formset/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.971567 django_formset-1.4/formset/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/lv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.971567 django_formset-1.4/formset/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/mn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.971567 django_formset-1.4/formset/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/nb/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/nl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/ro/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/sk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/sk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/sl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/sl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/sr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/sr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/sr_Latn_BA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.975567 django_formset-1.4/formset/locale/sr_Latn_BA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.979567 django_formset-1.4/formset/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/sv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/sv/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.979567 django_formset-1.4/formset/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.979567 django_formset-1.4/formset/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    12914 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/uk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.979567 django_formset-1.4/formset/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.979567 django_formset-1.4/formset/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.951567 django_formset-1.4/formset/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.979567 django_formset-1.4/formset/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-01 11:03:59.000000 django_formset-1.4/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-01 11:03:36.000000 django_formset-1.4/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-01 11:03:36.000000 django_formset-1.4/formset/ranges.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.979567 django_formset-1.4/formset/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-01 11:03:36.000000 django_formset-1.4/formset/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-01 11:03:36.000000 django_formset-1.4/formset/renderers/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-01 11:03:36.000000 django_formset-1.4/formset/renderers/bulma.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-01 11:03:36.000000 django_formset-1.4/formset/renderers/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-01 11:03:36.000000 django_formset-1.4/formset/renderers/foundation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-01 11:03:36.000000 django_formset-1.4/formset/renderers/tailwind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-01 11:03:36.000000 django_formset-1.4/formset/renderers/uikit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.983567 django_formset-1.4/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:03:36.000000 django_formset-1.4/formset/richtext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-05-01 11:03:36.000000 django_formset-1.4/formset/richtext/controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-01 11:03:36.000000 django_formset-1.4/formset/richtext/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-01 11:03:36.000000 django_formset-1.4/formset/richtext/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-01 11:03:36.000000 django_formset-1.4/formset/richtext/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.955567 django_formset-1.4/formset/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.955567 django_formset-1.4/formset/static/formset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.983567 django_formset-1.4/formset/static/formset/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-01 11:03:56.000000 django_formset-1.4/formset/static/formset/css/bootstrap5-extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-01 11:03:56.000000 django_formset-1.4/formset/static/formset/css/bootstrap5-extra.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-01 11:03:56.000000 django_formset-1.4/formset/static/formset/css/collections.css
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-01 11:03:56.000000 django_formset-1.4/formset/static/formset/css/collections.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-05-01 11:03:57.000000 django_formset-1.4/formset/static/formset/css/tailwind.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.983567 django_formset-1.4/formset/static/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/icons/file-audio.svg
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/icons/file-empty.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/icons/file-font.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/icons/file-missing.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/icons/file-pdf.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/icons/file-picture.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/icons/file-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/icons/file-video.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/icons/file-zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.987567 django_formset-1.4/formset/static/formset/js/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/Calendar-JILYT5ID.js
--rw-r--r--   0 runner    (1001) docker     (127)    44541 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/CountrySelectize-ZVZPUZGO.js
--rw-r--r--   0 runner    (1001) docker     (127)    17740 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/DateTime-2OODDTX3.js
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/DjangoSelectize-YB6QRNYJ.js
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/DjangoSlug-SHZN726V.js
--rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/DualSelector-ZHU2XXXL.js
--rw-r--r--   0 runner    (1001) docker     (127)   270582 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/PhoneNumber-IX6JTWS7.js
--rw-r--r--   0 runner    (1001) docker     (127)   311954 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/RichtextArea-VJIDTE2W.js
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/SortableSelect-7PAIJDN5.js
--rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-3KEXNODE.js
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-65OJRBX6.js
--rw-r--r--   0 runner    (1001) docker     (127)    68979 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-EQH4AZSI.js
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-FDUUONAQ.js
--rw-r--r--   0 runner    (1001) docker     (127)    57776 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-INHB3J7K.js
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-N376VWFX.js
--rw-r--r--   0 runner    (1001) docker     (127)    44439 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-NOGHTXP6.js
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-P2VM2T3G.js
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-RQ46AVYK.js
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-SERXULES.js
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/chunk-W5RPWA2M.js
--rw-r--r--   0 runner    (1001) docker     (127)    63708 2024-05-01 11:03:58.000000 django_formset-1.4/formset/static/formset/js/django-formset.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.991567 django_formset-1.4/formset/static/formset/tiptap-extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/tiptap-extensions/footnote.js
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/tiptap-extensions/procurator.js
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/tiptap-extensions/simple_image.js
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 11:03:36.000000 django_formset-1.4/formset/static/formset/tiptap-extensions/simple_link.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.955567 django_formset-1.4/formset/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.955567 django_formset-1.4/formset/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.991567 django_formset-1.4/formset/templates/admin/formset/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/admin/formset/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.991567 django_formset-1.4/formset/templates/calendar/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/calendar/hours.html
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/calendar/months.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/calendar/range.html
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/calendar/weeks.html
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/calendar/years.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.991567 django_formset-1.4/formset/templates/formset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.991567 django_formset-1.4/formset/templates/formset/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.991567 django_formset-1.4/formset/templates/formset/bootstrap/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/buttons/richtext_align.html
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/buttons/richtext_color.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/buttons/richtext_heading.html
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.995567 django_formset-1.4/formset/templates/formset/bootstrap/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bootstrap/widgets/richtextarea.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.995567 django_formset-1.4/formset/templates/formset/bulma/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.995567 django_formset-1.4/formset/templates/formset/bulma/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bulma/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bulma/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bulma/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bulma/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.995567 django_formset-1.4/formset/templates/formset/bulma/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bulma/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bulma/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bulma/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bulma/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bulma/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/bulma/widgets/select.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.995567 django_formset-1.4/formset/templates/formset/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.999567 django_formset-1.4/formset/templates/formset/default/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/buttons/move_all_left.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/buttons/move_all_right.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/buttons/move_selected_left.html
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/buttons/move_selected_right.html
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/buttons/redo_selected.html
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/buttons/undo_selected.html
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/detached_field.html
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/field_errors.html
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/form.html
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/form_dialog.html
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.999567 django_formset-1.4/formset/templates/formset/default/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/widgets/button.html
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/widgets/calendar.html
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/widgets/country_selectize.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/widgets/datetime.html
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/widgets/richtextarea.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/default/widgets/selectize.html
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/form_attrs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.999567 django_formset-1.4/formset/templates/formset/foundation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.999567 django_formset-1.4/formset/templates/formset/foundation/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/foundation/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/foundation/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/foundation/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/foundation/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:00.999567 django_formset-1.4/formset/templates/formset/foundation/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/foundation/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/foundation/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/foundation/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/foundation/widgets/inlined_input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/foundation/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.007567 django_formset-1.4/formset/templates/formset/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/activator.svg
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/add-fill.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/align-center.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/align-justify.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/align-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/align-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/arrow-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/arrow-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/arrow-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/blockquote.svg
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/bold.svg
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/bulletlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/calendar-today.svg
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/chevron-double-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/clearformat.svg
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/codeblock.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/decreasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/delete-back.svg
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/double-chevron-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/double-chevron-right.svg
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/footnote.svg
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/hardbreak.svg
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/heading.svg
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/heading1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/heading2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/heading3.svg
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/heading4.svg
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/heading5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/heading6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/horizontalrule.svg
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/image.svg
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/increasemargin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/indentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/italic.svg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/letters.svg
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/link.svg
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/orderedlist.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/outdentfirstline.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/placeholder.svg
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/questionmark.svg
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/redo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/reset.svg
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/send.svg
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/separator.svg
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/strike.svg
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/subscript.svg
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/superscript.svg
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/textcolor.svg
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/trash.svg
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/underline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/undo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/icons/unlink.svg
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/non_field_errors.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.011567 django_formset-1.4/formset/templates/formset/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/richtext/align.html
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/richtext/color.html
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/richtext/control.html
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/richtext/dialog_control.html
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/richtext/form_dialog.html
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/richtext/separator.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.011567 django_formset-1.4/formset/templates/formset/tailwind/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.011567 django_formset-1.4/formset/templates/formset/tailwind/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/form.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/help_text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.011567 django_formset-1.4/formset/templates/formset/tailwind/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/widgets/dual_selector.html
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/tailwind/widgets/radio.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.011567 django_formset-1.4/formset/templates/formset/uikit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.011567 django_formset-1.4/formset/templates/formset/uikit/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/uikit/buttons/add_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/uikit/buttons/remove_collection.html
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/uikit/field_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/uikit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.011567 django_formset-1.4/formset/templates/formset/uikit/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/uikit/widgets/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/uikit/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/uikit/widgets/input_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/formset/uikit/widgets/multiple_input.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.015567 django_formset-1.4/formset/templates/richtext/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/bulletlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/doc.html
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/footnote.html
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/footnote_ref.html
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/footnotes_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/horizontalrule.html
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/listitem.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.015567 django_formset-1.4/formset/templates/richtext/marks/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/marks/bold.html
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/marks/code.html
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/marks/italic.html
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/marks/procurator.html
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/marks/simple_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/marks/textcolor.html
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/marks/underline.html
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/orderedlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/paragraph.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templates/richtext/text.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:04:01.015567 django_formset-1.4/formset/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templatetags/formsetify.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templatetags/phonenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-01 11:03:36.000000 django_formset-1.4/formset/templatetags/richtext.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-01 11:03:36.000000 django_formset-1.4/formset/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-01 11:03:36.000000 django_formset-1.4/formset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-01 11:03:36.000000 django_formset-1.4/formset/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-05-01 11:03:36.000000 django_formset-1.4/formset/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-05-01 11:03:36.000000 django_formset-1.4/formset/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:04:01.019567 django_formset-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-01 11:03:36.000000 django_formset-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.294127 django_formset-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-04 22:04:34.000000 django_formset-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-04 22:04:34.000000 django_formset-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-04 22:05:05.294127 django_formset-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-05-04 22:04:34.000000 django_formset-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.294127 django_formset-1.4.1/django_formset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-04 22:05:05.000000 django_formset-1.4.1/django_formset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15360 2024-05-04 22:05:05.000000 django_formset-1.4.1/django_formset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 22:05:05.000000 django_formset-1.4.1/django_formset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 22:05:04.000000 django_formset-1.4.1/django_formset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 22:05:05.000000 django_formset-1.4.1/django_formset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 22:05:05.000000 django_formset-1.4.1/django_formset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23321 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/locale/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11275 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/af/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/af/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13577 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/bg/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ca/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ca/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.234125 django_formset-1.4.1/formset/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/cs/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/da/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/da/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10481 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13101 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/eo/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/et/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/et/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/eu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/eu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.238125 django_formset-1.4.1/formset/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/eu_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/fa/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/fa/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.214125 django_formset-1.4.1/formset/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/fi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/fi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11382 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12714 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/he/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/he/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/he_IL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/he_IL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/he_IL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/he_IL/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/hr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/hr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/hu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/hu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/hy/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/hy/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.242125 django_formset-1.4.1/formset/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/it/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/it/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12836 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ja/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ja/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ko_KR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/lt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/lt/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/lv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/mn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/nb/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11205 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.218125 django_formset-1.4.1/formset/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.246126 django_formset-1.4.1/formset/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ro/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12976 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sr_Latn_BA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sr_Latn_BA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/sv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/sv/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.250126 django_formset-1.4.1/formset/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    12914 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/uk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.222125 django_formset-1.4.1/formset/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/ranges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/bulma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/tailwind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/renderers/uikit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.254126 django_formset-1.4.1/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/richtext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7894 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/richtext/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/richtext/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/richtext/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/richtext/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.226125 django_formset-1.4.1/formset/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.226125 django_formset-1.4.1/formset/static/formset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.258126 django_formset-1.4.1/formset/static/formset/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-04 22:05:00.000000 django_formset-1.4.1/formset/static/formset/css/bootstrap5-extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-04 22:05:00.000000 django_formset-1.4.1/formset/static/formset/css/bootstrap5-extra.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-04 22:05:00.000000 django_formset-1.4.1/formset/static/formset/css/collections.css
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-04 22:05:00.000000 django_formset-1.4.1/formset/static/formset/css/collections.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-05-04 22:05:01.000000 django_formset-1.4.1/formset/static/formset/css/tailwind.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.258126 django_formset-1.4.1/formset/static/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-audio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-font.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-missing.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-picture.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-video.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/icons/file-zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/static/formset/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/Calendar-SME4CT3M.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44541 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/CountrySelectize-6YQ6A6VY.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17740 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/DateTime-4XMVQT2P.js
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/DjangoSelectize-JMSV2QXX.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/DjangoSlug-SHZN726V.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/DualSelector-233VL6HH.js
+-rw-r--r--   0 runner    (1001) docker     (127)   270393 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/PhoneNumber-KCJABOET.js
+-rw-r--r--   0 runner    (1001) docker     (127)   313209 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/RichtextArea-QY2VVCDL.js
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/SortableSelect-27BKOQAW.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-65OJRBX6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58061 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-CRVLB3K3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-FDUUONAQ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-NIKVGHIO.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44439 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-NOGHTXP6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-P2VM2T3G.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-QHDAXJJP.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15239 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-RLE6ONWJ.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-SERXULES.js
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-W5RPWA2M.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68979 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/chunk-XQYS6DVW.js
+-rw-r--r--   0 runner    (1001) docker     (127)    63654 2024-05-04 22:05:02.000000 django_formset-1.4.1/formset/static/formset/js/django-formset.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/static/formset/tiptap-extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/tiptap-extensions/footnote.js
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/tiptap-extensions/procurator.js
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/tiptap-extensions/simple_image.js
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/static/formset/tiptap-extensions/simple_link.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.230125 django_formset-1.4.1/formset/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.226125 django_formset-1.4.1/formset/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/templates/admin/formset/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/admin/formset/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/templates/calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/calendar/hours.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/calendar/months.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/calendar/range.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/calendar/weeks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/calendar/years.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/templates/formset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.266126 django_formset-1.4.1/formset/templates/formset/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.270126 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/richtext_align.html
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/richtext_color.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/buttons/richtext_heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.270126 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/richtextarea.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.270126 django_formset-1.4.1/formset/templates/formset/bulma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.270126 django_formset-1.4.1/formset/templates/formset/bulma/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.270126 django_formset-1.4.1/formset/templates/formset/bulma/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/bulma/widgets/select.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.274126 django_formset-1.4.1/formset/templates/formset/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.274126 django_formset-1.4.1/formset/templates/formset/default/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/move_all_left.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/move_all_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/move_selected_left.html
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/move_selected_right.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/redo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/buttons/undo_selected.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/detached_field.html
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/field_errors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/form_dialog.html
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.278126 django_formset-1.4.1/formset/templates/formset/default/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/country_selectize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/datetime.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/richtextarea.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/default/widgets/selectize.html
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/form_attrs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.278126 django_formset-1.4.1/formset/templates/formset/foundation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.278126 django_formset-1.4.1/formset/templates/formset/foundation/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.278126 django_formset-1.4.1/formset/templates/formset/foundation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/widgets/inlined_input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/foundation/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.286127 django_formset-1.4.1/formset/templates/formset/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/activator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/add-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/align-center.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/align-justify.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/align-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/align-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/blockquote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/bold.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/bulletlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/calendar-today.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/chevron-double-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/clearformat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/codeblock.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/decreasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/delete-back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/double-chevron-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/double-chevron-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/footnote.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/hardbreak.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/heading6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/horizontalrule.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/image.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/increasemargin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/indentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/italic.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/letters.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/link.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/orderedlist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/outdentfirstline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/placeholder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/questionmark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/reset.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/send.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/separator.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/strike.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/subscript.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/superscript.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/textcolor.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/underline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/icons/unlink.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/non_field_errors.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/align.html
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/color.html
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/control.html
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/dialog_control.html
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/form_dialog.html
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/richtext/separator.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/tailwind/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/tailwind/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/help_text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/dual_selector.html
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/tailwind/widgets/radio.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/uikit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/uikit/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/buttons/add_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/buttons/remove_collection.html
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/field_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.290127 django_formset-1.4.1/formset/templates/formset/uikit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/widgets/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/widgets/input_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/formset/uikit/widgets/multiple_input.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.294127 django_formset-1.4.1/formset/templates/richtext/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/bulletlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/footnote.html
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/footnote_ref.html
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/footnotes_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/horizontalrule.html
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/listitem.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.294127 django_formset-1.4.1/formset/templates/richtext/marks/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/bold.html
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/code.html
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/italic.html
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/procurator.html
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/simple_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/textcolor.html
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/marks/underline.html
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/orderedlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templates/richtext/text.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 22:05:05.294127 django_formset-1.4.1/formset/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templatetags/formsetify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templatetags/phonenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/templatetags/richtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21407 2024-05-04 22:04:34.000000 django_formset-1.4.1/formset/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 22:05:05.294127 django_formset-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-04 22:04:34.000000 django_formset-1.4.1/setup.py
```

### Comparing `django_formset-1.4/LICENSE` & `django_formset-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/PKG-INFO` & `django_formset-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.4
+Version: 1.4.1
 Summary: The missing widgets and form manipulation library for Django
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django_formset-1.4/README.md` & `django_formset-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/django_formset.egg-info/PKG-INFO` & `django_formset-1.4.1/django_formset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-formset
-Version: 1.4
+Version: 1.4.1
 Summary: The missing widgets and form manipulation library for Django
 Home-page: https://github.com/jrief/django-formset
 Author: Jacob Rief
 Author-email: jacob.rief@gmail.com
 License: MIT
 Keywords: Django Forms,webcomponent
 Platform: OS Independent
```

### Comparing `django_formset-1.4/django_formset.egg-info/SOURCES.txt` & `django_formset-1.4.1/django_formset.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -136,34 +136,34 @@
 formset/static/formset/icons/file-font.svg
 formset/static/formset/icons/file-missing.svg
 formset/static/formset/icons/file-pdf.svg
 formset/static/formset/icons/file-picture.svg
 formset/static/formset/icons/file-unknown.svg
 formset/static/formset/icons/file-video.svg
 formset/static/formset/icons/file-zip.svg
-formset/static/formset/js/Calendar-JILYT5ID.js
-formset/static/formset/js/CountrySelectize-ZVZPUZGO.js
-formset/static/formset/js/DateTime-2OODDTX3.js
-formset/static/formset/js/DjangoSelectize-YB6QRNYJ.js
+formset/static/formset/js/Calendar-SME4CT3M.js
+formset/static/formset/js/CountrySelectize-6YQ6A6VY.js
+formset/static/formset/js/DateTime-4XMVQT2P.js
+formset/static/formset/js/DjangoSelectize-JMSV2QXX.js
 formset/static/formset/js/DjangoSlug-SHZN726V.js
-formset/static/formset/js/DualSelector-ZHU2XXXL.js
-formset/static/formset/js/PhoneNumber-IX6JTWS7.js
-formset/static/formset/js/RichtextArea-VJIDTE2W.js
-formset/static/formset/js/SortableSelect-7PAIJDN5.js
-formset/static/formset/js/chunk-3KEXNODE.js
+formset/static/formset/js/DualSelector-233VL6HH.js
+formset/static/formset/js/PhoneNumber-KCJABOET.js
+formset/static/formset/js/RichtextArea-QY2VVCDL.js
+formset/static/formset/js/SortableSelect-27BKOQAW.js
 formset/static/formset/js/chunk-65OJRBX6.js
-formset/static/formset/js/chunk-EQH4AZSI.js
+formset/static/formset/js/chunk-CRVLB3K3.js
 formset/static/formset/js/chunk-FDUUONAQ.js
-formset/static/formset/js/chunk-INHB3J7K.js
-formset/static/formset/js/chunk-N376VWFX.js
+formset/static/formset/js/chunk-NIKVGHIO.js
 formset/static/formset/js/chunk-NOGHTXP6.js
 formset/static/formset/js/chunk-P2VM2T3G.js
-formset/static/formset/js/chunk-RQ46AVYK.js
+formset/static/formset/js/chunk-QHDAXJJP.js
+formset/static/formset/js/chunk-RLE6ONWJ.js
 formset/static/formset/js/chunk-SERXULES.js
 formset/static/formset/js/chunk-W5RPWA2M.js
+formset/static/formset/js/chunk-XQYS6DVW.js
 formset/static/formset/js/django-formset.js
 formset/static/formset/tiptap-extensions/footnote.js
 formset/static/formset/tiptap-extensions/procurator.js
 formset/static/formset/tiptap-extensions/simple_image.js
 formset/static/formset/tiptap-extensions/simple_link.js
 formset/templates/admin/formset/change_form.html
 formset/templates/calendar/hours.html
```

### Comparing `django_formset-1.4/formset/boundfield.py` & `django_formset-1.4.1/formset/boundfield.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/calendar.py` & `django_formset-1.4.1/formset/calendar.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/collection.py` & `django_formset-1.4.1/formset/collection.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/dialog.py` & `django_formset-1.4.1/formset/dialog.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/fields.py` & `django_formset-1.4.1/formset/fields.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/fieldset.py` & `django_formset-1.4.1/formset/fieldset.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/af/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/af/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/af/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/af/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ar/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ar/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/bg/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/bg/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ca/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/ca/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ca/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/ca/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/cs/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/cs/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/da/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/da/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/da/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/da/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/de/LC_MESSAGES/django.mo` & `django_formset-1.4.1/formset/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/de/LC_MESSAGES/django.po` & `django_formset-1.4.1/formset/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/de/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/de/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/el/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/el/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/el/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/eo/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/eo/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/es/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/es/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/et/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/et/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/et/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/et/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/eu/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/eu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/eu/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/eu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/eu_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/eu_ES/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/eu_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/fa/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/fa/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/fa/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/fi/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/fi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/fi/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/fi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/fr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/fr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/he/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/he/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/he/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/he/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/he_IL/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/he_IL/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/he_IL/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/he_IL/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/hr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/hr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/hr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/hr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/hu/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/hu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/hu/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/hu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/hy/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/hy/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/hy/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/hy/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/it/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/it/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ja/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/ja/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ja/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/ko_KR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ko_KR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/lt/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/lt/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/lt/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/lt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/lv/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/lv/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/mn/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/mn/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/nb/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/nb/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/nl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/nl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/pl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/pl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/pt_BR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/pt_PT/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ro/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ro/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ru/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/ru/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sk/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/sk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sk/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/sk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sl/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sl/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sr/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/sr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sr/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/sr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/sr_Latn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/sr_Latn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/sr_Latn_BA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sv/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/sv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/sv/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/sv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/tr_TR/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/uk/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/uk/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/zh_CN/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/zh_Hans/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo` & `django_formset-1.4.1/formset/locale/zh_Hant/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po` & `django_formset-1.4.1/formset/locale/zh_Hant/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/ranges.py` & `django_formset-1.4.1/formset/ranges.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/renderers/__init__.py` & `django_formset-1.4.1/formset/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/renderers/bootstrap.py` & `django_formset-1.4.1/formset/renderers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/renderers/bulma.py` & `django_formset-1.4.1/formset/renderers/bulma.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/renderers/default.py` & `django_formset-1.4.1/formset/renderers/default.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/renderers/foundation.py` & `django_formset-1.4.1/formset/renderers/foundation.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/renderers/tailwind.py` & `django_formset-1.4.1/formset/renderers/tailwind.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/renderers/uikit.py` & `django_formset-1.4.1/formset/renderers/uikit.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/richtext/controls.py` & `django_formset-1.4.1/formset/richtext/controls.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/richtext/dialogs.py` & `django_formset-1.4.1/formset/richtext/dialogs.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/richtext/widgets.py` & `django_formset-1.4.1/formset/richtext/widgets.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/css/bootstrap5-extra.css` & `django_formset-1.4.1/formset/static/formset/css/bootstrap5-extra.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/css/bootstrap5-extra.css.map` & `django_formset-1.4.1/formset/static/formset/css/bootstrap5-extra.css.map`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/css/collections.css` & `django_formset-1.4.1/formset/static/formset/css/collections.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/css/tailwind.css` & `django_formset-1.4.1/formset/static/formset/css/tailwind.css`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/icons/file-audio.svg` & `django_formset-1.4.1/formset/static/formset/icons/file-audio.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/icons/file-empty.svg` & `django_formset-1.4.1/formset/static/formset/icons/file-empty.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/icons/file-font.svg` & `django_formset-1.4.1/formset/static/formset/icons/file-font.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/icons/file-missing.svg` & `django_formset-1.4.1/formset/static/formset/icons/file-missing.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/icons/file-pdf.svg` & `django_formset-1.4.1/formset/static/formset/icons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/icons/file-picture.svg` & `django_formset-1.4.1/formset/static/formset/icons/file-picture.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/icons/file-unknown.svg` & `django_formset-1.4.1/formset/static/formset/icons/file-unknown.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/icons/file-video.svg` & `django_formset-1.4.1/formset/static/formset/icons/file-video.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/icons/file-zip.svg` & `django_formset-1.4.1/formset/static/formset/icons/file-zip.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/CountrySelectize-ZVZPUZGO.js` & `django_formset-1.4.1/formset/static/formset/js/CountrySelectize-6YQ6A6VY.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     a as c
-} from "./chunk-INHB3J7K.js";
+} from "./chunk-CRVLB3K3.js";
 import "./chunk-SERXULES.js";
 import "./chunk-W5RPWA2M.js";
 import {
     a as r
 } from "./chunk-FDUUONAQ.js";
 import "./chunk-65OJRBX6.js";
 import {
```

### Comparing `django_formset-1.4/formset/static/formset/js/DateTime-2OODDTX3.js` & `django_formset-1.4.1/formset/static/formset/js/DateTime-4XMVQT2P.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 import {
     a as v
-} from "./chunk-3KEXNODE.js";
+} from "./chunk-QHDAXJJP.js";
 import {
     b as m
 } from "./chunk-W5RPWA2M.js";
 import {
     a as x,
     c as f,
     d as g,
     e as y
-} from "./chunk-RQ46AVYK.js";
+} from "./chunk-RLE6ONWJ.js";
 import {
     a as c
 } from "./chunk-65OJRBX6.js";
 import "./chunk-P2VM2T3G.js";
 var E = '[is^=django-date]{--dummy-style: none}[is^=django-date]+[role=textbox]{position:relative}[is^=django-date]+[role=textbox].focus{--dummy-style: none}[is^=django-date]+[role=textbox]>.calendar-picker-indicator{display:flex;align-items:center;position:absolute;top:0;left:.5rem;bottom:0;cursor:pointer}[is^=django-date]+[role=textbox]>.calendar-picker-indicator svg{scale:.75}[is^=django-date]+[role=textbox]>.datetime-edit{display:flex;overflow-x:hidden}[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-delimiter{color:#606060;margin:0 -1px}[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-delimiter.wide{margin:0;padding:0 .125rem}[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-year-field,[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-month-field,[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-day-field,[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-hour-field,[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-minute-field{padding:.125rem;cursor:text;caret-color:rgba(0,0,0,0)}[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-year-field:focus-visible,[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-month-field:focus-visible,[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-day-field:focus-visible,[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-hour-field:focus-visible,[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-minute-field:focus-visible{border-radius:3px;outline:none;background-color:#0d6efd;color:#fff}[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-year-field:empty::after{content:"yyyy";color:#d3d3d3}[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-month-field:empty::after{content:"mm";color:#d3d3d3}[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-day-field:empty::after{content:"dd";color:#d3d3d3}[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-hour-field:empty::after{content:"HH";color:#d3d3d3}[is^=django-date]+[role=textbox]>.datetime-edit>.datetime-edit-minute-field:empty::after{content:"MM";color:#d3d3d3}:is([is=django-datepicker],[is=django-datetimepicker],[is=django-daterangepicker],[is=django-datetimerangepicker])+[role=textbox]>.datetime-edit{margin-left:calc(1rem + .6em)}';
 var F = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<path d="M17 3H21C21.5523 3 22 3.44772 22 4V20C22 20.5523 21.5523 21 21 21H3C2.44772 21 2 20.5523 2 20V4C2 3.44772 2.44772 3 3 3H7V1H9V3H15V1H17V3ZM4 9V19H20V9H4ZM6 11H8V13H6V11ZM11 11H13V13H11V11ZM16 11H18V13H16V11Z"></path>
```

### Comparing `django_formset-1.4/formset/static/formset/js/DjangoSlug-SHZN726V.js` & `django_formset-1.4.1/formset/static/formset/js/DjangoSlug-SHZN726V.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/DualSelector-ZHU2XXXL.js` & `django_formset-1.4.1/formset/static/formset/js/DualSelector-233VL6HH.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as d
 } from "./chunk-SERXULES.js";
 import "./chunk-W5RPWA2M.js";
 import {
     a as p
-} from "./chunk-N376VWFX.js";
+} from "./chunk-NIKVGHIO.js";
 import "./chunk-NOGHTXP6.js";
 import {
     a as v
 } from "./chunk-FDUUONAQ.js";
 import {
     a as r
 } from "./chunk-65OJRBX6.js";
```

### Comparing `django_formset-1.4/formset/static/formset/js/PhoneNumber-IX6JTWS7.js` & `django_formset-1.4.1/formset/static/formset/js/PhoneNumber-KCJABOET.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     a as $d,
     b as md,
     e as hd
-} from "./chunk-RQ46AVYK.js";
+} from "./chunk-RLE6ONWJ.js";
 import {
     a as y
 } from "./chunk-65OJRBX6.js";
 import "./chunk-P2VM2T3G.js";
 var R = {
     version: 4,
     country_calling_codes: {
@@ -608,15 +608,15 @@
             [
                 ["(\\d{2})(\\d{2})(\\d{3})", "$1 $2 $3", ["88"], "0$1"],
                 ["(\\d{2})(\\d{5})", "$1 $2", ["[1-6]"], "0$1"],
                 ["(\\d{2})(\\d{3})(\\d{4})", "$1 $2 $3", ["1"], "0$1"],
                 ["(\\d{3})(\\d{3})(\\d{3})", "$1 $2 $3", ["[89]"], "0$1"]
             ], "0", 0, 0, 0, 0, 0, [
                 ["12\\d{7}|[1-6]\\d{6}"],
-                ["88\\d{5}|(?:8[0-59]|9[017-9])\\d{7}"]
+                ["88\\d{5}|(?:8[0-69]|9[017-9])\\d{7}"]
             ]
         ],
         CF: ["236", "00", "(?:[27]\\d{3}|8776)\\d{4}", [8],
             [
                 ["(\\d{2})(\\d{2})(\\d{2})(\\d{2})", "$1 $2 $3 $4", ["[278]"]]
             ], 0, 0, 0, 0, 0, 0, [
                 ["2[12]\\d{6}"],
@@ -1040,15 +1040,15 @@
             [
                 ["(\\d{3})(\\d{3})(\\d{3})", "$1 $2 $3", ["70"], "0$1"],
                 ["(\\d{2})(\\d{3})(\\d{2})(\\d{2})", "$1 $2 $3 $4", ["32"], "0$1"],
                 ["(\\d{3})(\\d{2})(\\d{2})(\\d{2})", "$1 $2 $3 $4", ["[57]"]],
                 ["(\\d{3})(\\d{2})(\\d{2})(\\d{2})", "$1 $2 $3 $4", ["[348]"], "0$1"]
             ], "0", 0, 0, 0, 0, 0, [
                 ["(?:3(?:[256]\\d|4[124-9]|7[0-4])|4(?:1\\d|2[2-7]|3[1-79]|4[2-8]|7[239]|9[1-7]))\\d{6}"],
-                ["5(?:(?:(?:0555|1(?:[17]77|555))[5-9]|757(?:7[7-9]|8[01]))\\d|22252[0-4])\\d\\d|(?:5(?:0(?:0(?:0\\d|11|22|33|44|5[05]|77|88|9[09])|111)|1(?:1(?:00|[124]\\d|3[01])|4\\d\\d)|(?:44|68)\\d\\d|5(?:[0157-9]\\d\\d|200)|7(?:[0147-9]\\d\\d|5(?:00|[57]5))|8(?:0(?:[018]\\d|2[0-4])|58[89]|8(?:55|88))|9(?:090|[1-35-9]\\d\\d))|790\\d\\d)\\d{4}|5(?:0(?:0[17]0|505)|1(?:0[01]0|1(?:07|33|51))|2(?:0[02]0|2[25]2)|3(?:0[03]0|3[35]3)|(?:40[04]|900)0|5222)[0-4]\\d{3}"],
+                ["5(?:(?:(?:0555|1(?:[17]77|555))[5-9]|757(?:7[7-9]|8[01]))\\d|22252[0-4])\\d\\d|(?:5(?:0(?:0(?:0\\d|11|22|33|44|5[05]|77|88|9[09])|111)|1(?:1(?:[03][01]|[124]\\d)|4\\d\\d)|(?:44|6[89])\\d\\d|5(?:[0157-9]\\d\\d|200)|7(?:[0147-9]\\d\\d|5(?:00|[57]5))|8(?:0(?:[018]\\d|2[0-4])|58[89]|8(?:55|88))|9(?:090|[1-35-9]\\d\\d))|790\\d\\d)\\d{4}|5(?:0(?:0[17]0|505)|1(?:0[01]0|1(?:07|33|51))|2(?:0[02]0|2[25]2)|3(?:0[03]0|3[35]3)|(?:40[04]|900)0|5222)[0-4]\\d{3}"],
                 ["800\\d{6}"], 0, 0, 0, 0, 0, ["70[67]\\d{6}"]
             ]
         ],
         GF: ["594", "00", "[56]94\\d{6}|(?:80|9\\d)\\d{7}", [9],
             [
                 ["(\\d{3})(\\d{2})(\\d{2})(\\d{2})", "$1 $2 $3 $4", ["[56]|9[47]"], "0$1"],
                 ["(\\d{3})(\\d{2})(\\d{2})(\\d{2})", "$1 $2 $3 $4", ["[89]"], "0$1"]
@@ -1174,15 +1174,15 @@
             ]
         ],
         GY: ["592", "001", "(?:[2-8]\\d{3}|9008)\\d{3}", [7],
             [
                 ["(\\d{3})(\\d{4})", "$1 $2", ["[2-9]"]]
             ], 0, 0, 0, 0, 0, 0, [
                 ["(?:2(?:1[6-9]|2[0-35-9]|3[1-4]|5[3-9]|6\\d|7[0-79])|3(?:2[25-9]|3\\d)|4(?:4[0-24]|5[56])|50[0-6]|77[1-57])\\d{4}"],
-                ["(?:510|6\\d\\d|7(?:[01]\\d|2[156]|3[12]|49))\\d{4}"],
+                ["(?:510|6\\d\\d|7(?:[01]\\d|2[1256]|3[12]|49))\\d{4}"],
                 ["(?:289|8(?:00|6[28]|88|99))\\d{4}"],
                 ["9008\\d{3}"], 0, 0, 0, 0, ["515\\d{4}"]
             ]
         ],
         HK: ["852", "00(?:30|5[09]|[126-9]?)", "8[0-46-9]\\d{6,7}|9\\d{4,7}|(?:[2-7]|9\\d{3})\\d{7}", [5, 6, 7, 8, 9, 11],
             [
                 ["(\\d{3})(\\d{2,5})", "$1 $2", ["900", "9003"]],
@@ -1548,15 +1548,15 @@
         LA: ["856", "00", "[23]\\d{9}|3\\d{8}|(?:[235-8]\\d|41)\\d{6}", [8, 9, 10],
             [
                 ["(\\d{2})(\\d{3})(\\d{3})", "$1 $2 $3", ["2[13]|3[14]|[4-8]"], "0$1"],
                 ["(\\d{2})(\\d{2})(\\d{2})(\\d{3})", "$1 $2 $3 $4", ["30[013-9]"], "0$1"],
                 ["(\\d{2})(\\d{2})(\\d{3})(\\d{3})", "$1 $2 $3 $4", ["[23]"], "0$1"]
             ], "0", 0, 0, 0, 0, 0, [
                 ["(?:2[13]|[35-7][14]|41|8[1468])\\d{6}", [8]],
-                ["2088\\d{6}|(?:20[23579]|302)\\d{7}", [10]], 0, 0, 0, 0, ["30[013-9]\\d{6}", [9]]
+                ["(?:20(?:[23579]\\d|88)|30(?:2\\d|4))\\d{6}", [9, 10]], 0, 0, 0, 0, ["30[0135-9]\\d{6}", [9]]
             ]
         ],
         LB: ["961", "00", "[27-9]\\d{7}|[13-9]\\d{6}", [7, 8],
             [
                 ["(\\d)(\\d{3})(\\d{3})", "$1 $2 $3", ["[13-69]|7(?:[2-57]|62|8[0-7]|9[04-9])|8[02-9]"], "0$1"],
                 ["(\\d{2})(\\d{3})(\\d{3})", "$1 $2 $3", ["[27-9]"]]
             ], "0", 0, 0, 0, 0, 0, [
@@ -2194,15 +2194,15 @@
         ],
         PT: ["351", "00", "1693\\d{5}|(?:[26-9]\\d|30)\\d{7}", [9],
             [
                 ["(\\d{2})(\\d{3})(\\d{4})", "$1 $2 $3", ["2[12]"]],
                 ["(\\d{3})(\\d{3})(\\d{3})", "$1 $2 $3", ["16|[236-9]"]]
             ], 0, 0, 0, 0, 0, 0, [
                 ["2(?:[12]\\d|3[1-689]|4[1-59]|[57][1-9]|6[1-35689]|8[1-69]|9[1256])\\d{6}"],
-                ["6(?:[06]92(?:30|9\\d)|[35]92(?:3[034]|9\\d))\\d{3}|(?:(?:16|6[0356])93|9(?:[1-36]\\d\\d|480))\\d{5}"],
+                ["6(?:[06]92(?:30|9\\d)|[35]92(?:[049]\\d|3[034]))\\d{3}|(?:(?:16|6[0356])93|9(?:[1-36]\\d\\d|480))\\d{5}"],
                 ["80[02]\\d{6}"],
                 ["(?:6(?:0[178]|4[68])\\d|76(?:0[1-57]|1[2-47]|2[237]))\\d{5}"],
                 ["884[0-4689]\\d{5}"], 0, ["70(?:38[01]|596|(?:7\\d|8[17])\\d)\\d{4}"],
                 ["6(?:222\\d|8988)\\d{4}"],
                 ["30\\d{7}"],
                 ["80(?:8\\d|9[1579])\\d{5}"]
             ]
@@ -2256,15 +2256,15 @@
             [
                 ["(\\d{3})(\\d{3})", "$1 $2", ["2[3-6]", "2[3-6]\\d9"], "0$1"],
                 ["(\\d{2})(\\d{4})", "$1 $2", ["219|31"], "0$1"],
                 ["(\\d{2})(\\d{3})(\\d{4})", "$1 $2 $3", ["[23]1"], "0$1"],
                 ["(\\d{3})(\\d{3})(\\d{3})", "$1 $2 $3", ["[236-9]"], "0$1"]
             ], "0", 0, 0, 0, 0, 0, [
                 ["[23][13-6]\\d{7}|(?:2(?:19\\d|[3-6]\\d9)|31\\d\\d)\\d\\d"],
-                ["7020\\d{5}|(?:6(?:2\\d|40)|7(?:0[013-9]|1[0-3]|[2-7]\\d|8[03-8]|9[0-39]))\\d{6}", [9]],
+                ["7020\\d{5}|(?:6(?:[04]0|2\\d)|7(?:0[013-9]|1[0-3]|[2-7]\\d|8[03-8]|9[0-39]))\\d{6}", [9]],
                 ["800\\d{6}", [9]],
                 ["90[0136]\\d{6}", [9]], 0, 0, ["(?:37\\d|80[578])\\d{6}", [9]], 0, 0, ["801\\d{6}", [9]]
             ], 0, " int "
         ],
         RS: ["381", "00", "38[02-9]\\d{6,9}|6\\d{7,9}|90\\d{4,8}|38\\d{5,6}|(?:7\\d\\d|800)\\d{3,9}|(?:[12]\\d|3[0-79])\\d{5,10}", [6, 7, 8, 9, 10, 11, 12],
             [
                 ["(\\d{3})(\\d{3,9})", "$1 $2", ["(?:2[389]|39)0|[7-9]"], "0$1"],
@@ -2370,15 +2370,15 @@
             [
                 ["(\\d{4})(\\d{4})", "$1 $2", ["[369]|8(?:0[1-9]|[1-9])"]],
                 ["(\\d{3})(\\d{3})(\\d{4})", "$1 $2 $3", ["8"]],
                 ["(\\d{4})(\\d{4})(\\d{3})", "$1 $2 $3", ["7"]],
                 ["(\\d{4})(\\d{3})(\\d{4})", "$1 $2 $3", ["1"]]
             ], 0, 0, 0, 0, 0, 0, [
                 ["662[0-24-9]\\d{4}|6(?:[0-578]\\d|6[013-57-9]|9[0-35-9])\\d{5}", [8]],
-                ["8(?:09|95)[0-2]\\d{4}|(?:8(?:0[1-8]|[1-8]\\d|9[0-4])|9[0-8]\\d)\\d{5}", [8]],
+                ["8(?:09[0-24]|95[0-2])\\d{4}|(?:8(?:0[1-8]|[1-8]\\d|9[0-4])|9[0-8]\\d)\\d{5}", [8]],
                 ["(?:18|8)00\\d{7}", [10, 11]],
                 ["1900\\d{7}", [11]], 0, 0, ["7000\\d{7}", [11]], 0, ["(?:3[12]\\d|666)\\d{5}", [8]]
             ]
         ],
         SH: ["290", "00", "(?:[256]\\d|8)\\d{3}", [4, 5], 0, 0, 0, 0, 0, 0, "[256]", [
             ["2(?:[0-57-9]\\d|6[4-9])\\d\\d"],
             ["[56]\\d{4}", [5]], 0, 0, 0, 0, 0, 0, ["262\\d\\d", [5]]
@@ -2539,15 +2539,15 @@
             ["52(?:3(?:[2-46-9][02-9]\\d|5(?:[02-46-9]\\d|5[0-46-9]))|4(?:[2-478][02-9]\\d|5(?:[034]\\d|2[024-9]|5[0-46-9])|6(?:0[1-9]|[2-9]\\d)|9(?:[05-9]\\d|2[0-5]|49)))\\d{4}|52[34][2-9]1[02-9]\\d{4}|5(?:00|2[125-9]|33|44|66|77|88)[2-9]\\d{6}"], 0, 0, 0, ["649(?:71[01]|966)\\d{4}"]
         ]],
         TD: ["235", "00|16", "(?:22|[69]\\d|77)\\d{6}", [8],
             [
                 ["(\\d{2})(\\d{2})(\\d{2})(\\d{2})", "$1 $2 $3 $4", ["[2679]"]]
             ], 0, 0, 0, 0, 0, 0, [
                 ["22(?:[37-9]0|5[0-5]|6[89])\\d{4}"],
-                ["(?:6[0235689]|77|9\\d)\\d{6}"]
+                ["(?:6[0-689]|77|9\\d)\\d{6}"]
             ], "00"
         ],
         TG: ["228", "00", "[279]\\d{7}", [8],
             [
                 ["(\\d{2})(\\d{2})(\\d{2})(\\d{2})", "$1 $2 $3 $4", ["[279]"]]
             ], 0, 0, 0, 0, 0, 0, [
                 ["2(?:2[2-7]|3[23]|4[45]|55|6[67]|77)\\d{5}"],
@@ -5869,40 +5869,41 @@
         }
         transferStyles() {
             let t = document.createElement("style"),
                 d = !1;
             t.innerText = l0, document.head.appendChild(t), this.inputElement.style.transition = "none";
             for (let a = 0; t.sheet && a < t.sheet.cssRules.length; a++) {
                 let i = t.sheet.cssRules.item(a),
-                    n;
+                    n = "";
                 switch (i.selectorText.trim()) {
                     case this.baseSelector:
                         d = !0;
                         break;
                     case `${this.baseSelector} + [role="textbox"]`:
-                        n = y.extractStyles(this.inputElement, ["background-color", "border", "border-radius", "color", "outline", "height", "line-height", "padding"]), t.sheet.insertRule(`${i.selectorText}{${n}}`, ++a);
+                        n = y.extractStyles(this.inputElement, ["background-color", "border", "border-radius", "color", "outline", "height", "line-height", "padding"]);
                         break;
                     case `${this.baseSelector} + [role="textbox"].focus`:
-                        this.inputElement.classList.add("-focus-"), n = y.extractStyles(this.inputElement, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), this.inputElement.classList.remove("-focus-"), t.sheet.insertRule(`${i.selectorText}{${n}}`, ++a);
+                        this.inputElement.classList.add("-focus-"), n = y.extractStyles(this.inputElement, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), this.inputElement.classList.remove("-focus-");
                         break;
                     case `${this.baseSelector} + [role="textbox"][aria-haspopup="dialog"] + [role="dialog"]`:
-                        n = y.extractStyles(this.inputElement, ["background-color", "border-radius", "color", "line-height", "padding"]), t.sheet.insertRule(`${i.selectorText}{${n}}`, ++a);
+                        n = y.extractStyles(this.inputElement, ["background-color", "border-radius", "color", "line-height", "padding"]);
                         break;
                     case `${this.baseSelector} + [role="textbox"][aria-haspopup="dialog"] + [role="dialog"] input[type="search"]`:
-                        n = y.extractStyles(this.inputElement, ["background-color", "border", "border-radius", "color", "line-height", "padding"]), t.sheet.insertRule(`${i.selectorText}{${n}`, ++a);
+                        n = y.extractStyles(this.inputElement, ["background-color", "border", "border-radius", "color", "line-height", "padding"]);
                         break;
                     case `${this.baseSelector} + [role="textbox"][aria-haspopup="dialog"] + [role="dialog"] input[type="search"]:focus`:
-                        this.inputElement.classList.add("-focus-"), n = y.extractStyles(this.inputElement, ["border", "box-shadow", "outline", "transition"]), this.inputElement.classList.remove("-focus-"), t.sheet.insertRule(`${i.selectorText}{${n}`, ++a);
+                        this.inputElement.classList.add("-focus-"), n = y.extractStyles(this.inputElement, ["border", "box-shadow", "outline", "transition"]), this.inputElement.classList.remove("-focus-");
                         break;
                     case `${this.baseSelector} + [role="textbox"][aria-haspopup="dialog"] + [role="dialog"] ul`:
-                        t.sheet.insertRule(`${i.selectorText}{height:${Math.floor(window.innerHeight/3)}px;}`, ++a);
+                        n = `${i.selectorText}{height:${Math.floor(window.innerHeight/3)}px;}`;
                         break;
                     default:
                         break
                 }
+                n && t.sheet.insertRule(`${i.selectorText}{${n}}`, ++a)
             }
             if (this.inputElement.style.transition = "", !d) throw new Error(`Could not load styles for ${this.baseSelector}`)
         }
         transferClasses() {
             this.inputElement.classList.remove(...this.inputElement.classList), this.inputElement.style.transition = "", this.inputElement.hidden = !0
         }
         initialize() {
```

### Comparing `django_formset-1.4/formset/static/formset/js/RichtextArea-VJIDTE2W.js` & `django_formset-1.4.1/formset/static/formset/js/RichtextArea-QY2VVCDL.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 import {
-    a as ua,
-    b as fa,
-    c as ha,
+    a as fa,
+    b as ha,
+    c as pa,
     f as Vi
-} from "./chunk-EQH4AZSI.js";
+} from "./chunk-XQYS6DVW.js";
 import {
-    a as pa
+    a as ma
 } from "./chunk-FDUUONAQ.js";
 import {
     e as ji
-} from "./chunk-RQ46AVYK.js";
+} from "./chunk-RLE6ONWJ.js";
 import {
     a as ve
 } from "./chunk-65OJRBX6.js";
 import {
     b as tn
 } from "./chunk-P2VM2T3G.js";
 var Ji = '.dj-richtext-wrapper{--button-active: rgba(0, 0, 0, 0.1);--button-opacity: 0.5;position:relative;overflow:auto}.dj-richtext-wrapper [role=menubar]{border:none;position:absolute;inset:0 0 auto 0;padding:.125rem .25rem}.dj-richtext-wrapper [role=menubar] [role=separator]{display:inline-block;padding:.25rem 0;vertical-align:middle}.dj-richtext-wrapper [role=menubar] button{display:inline-block;text-align:center;text-decoration:none;vertical-align:middle;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;user-select:none;border:none;border-radius:.25rem;padding:.25rem;background-color:inherit;opacity:var(--button-opacity)}.dj-richtext-wrapper [role=menubar] button:hover{opacity:1}.dj-richtext-wrapper [role=menubar] button.active{opacity:1;background-color:var(--button-active)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]:after{border-bottom:0;border-left:.3em solid rgba(0,0,0,0);border-right:.3em solid rgba(0,0,0,0);border-top:.3em solid;margin-right:.125rem;content:"";display:inline-block;transition:transform 250ms ease-in-out}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true][aria-expanded=true]:after{transform:scaleY(-1)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]{display:none;position:absolute;width:max-content;top:0;left:0;padding:inherit;list-style:none;background-color:inherit;border-color:#000}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li{background-color:inherit;opacity:var(--button-opacity)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li:hover{opacity:1}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true]+ul[role=menu]>li.active{color:inherit;opacity:1;background-color:var(--button-active)}.dj-richtext-wrapper [role=menubar] button[aria-haspopup=true][aria-expanded=true]+ul[role=menu]{display:block}.dj-richtext-wrapper [role=menubar] button>svg{vertical-align:middle;display:inline}.dj-richtext-wrapper .character-count{position:absolute;bottom:3px;right:6px;color:rgba(0,0,0,.2)}.dj-richtext-wrapper .ProseMirror{border:none;position:absolute;left:0;right:0;bottom:0;word-wrap:break-word;white-space:break-spaces;font-variant-ligatures:none;font-feature-settings:"liga" 0;overflow:hidden}.dj-richtext-wrapper .ProseMirror[contenteditable=false]{white-space:normal}.dj-richtext-wrapper .ProseMirror p{margin-bottom:.5rem}.dj-richtext-wrapper .ProseMirror p.is-editor-empty:first-child::before{color:rgba(0,0,0,.2);content:attr(data-placeholder);float:left;height:0;pointer-events:none}.dj-richtext-wrapper .ProseMirror p[data-text=indent]{text-indent:3em}.dj-richtext-wrapper .ProseMirror p[data-text=outdent]{text-indent:-3em;padding-left:3em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="1"]{margin-left:2em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="2"]{margin-left:4em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="3"]{margin-left:6em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="4"]{margin-left:8em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="5"]{margin-left:10em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="6"]{margin-left:12em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="7"]{margin-left:14em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="8"]{margin-left:16em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="9"]{margin-left:18em}.dj-richtext-wrapper .ProseMirror p[data-text-indent="10"]{margin-left:20em}.dj-richtext-wrapper .ProseMirror li>p{margin:0}.dj-richtext-wrapper .ProseMirror:focus-visible{outline:none}.dj-richtext-wrapper .ProseMirror blockquote{border-left:3px solid rgba(0,0,0,.2);padding-left:1rem}.dj-richtext-wrapper .ProseMirror output[role=placeholder]{background-color:rgba(0,0,0,.03);box-shadow:inset 0 0 5px rgba(0,0,0,.7);border-radius:.125rem;padding-left:.25rem;padding-right:.25rem}.dj-richtext-wrapper .ProseMirror span[role=note]{display:inline-block;margin-left:.125em;margin-right:.125em}.dj-richtext-wrapper .ProseMirror span[role=note]::after{content:"[*]";font-weight:500;font-size:75%;vertical-align:super;color:#0d6efd}.dj-richtext-wrapper .ProseMirror pre{padding:.5rem 1rem;background-color:rgba(0,0,0,.03);font-family:monospace}.dj-richtext-wrapper .ProseMirror pre{white-space:pre-wrap}.dj-richtext-wrapper.focused{opacity:1}.dj-submitted .dj-richtext-wrapper.focused.invalid{opacity:1}.dj-richtext-wrapper:not(.focused).invalid{border-color:var(--django-formset-color-invalid)}.dj-richtext-wrapper:not(.focused).valid{border-color:var(--django-formset-color-valid)}';
@@ -85,15 +85,15 @@
 re.from = function(n) {
     if (n instanceof re) return n;
     var e = [];
     if (n)
         for (var t in n) e.push(t, n[t]);
     return new re(e)
 };
-var _n = re;
+var Gn = re;
 
 function Yi(n, e, t) {
     for (let r = 0;; r++) {
         if (r == n.childCount || r == e.childCount) return n.childCount == e.childCount ? null : t;
         let i = n.child(r),
             s = e.child(r);
         if (i == s) {
@@ -142,15 +142,15 @@
         if (o.content.size || l.content.size) {
             let c = Xi(o.content, l.content, t - 1, r - 1);
             if (c) return c
         }
         t -= a, r -= a
     }
 }
-var M = class n {
+var w = class n {
     constructor(e, t) {
         if (this.content = e, this.size = t || 0, t == null)
             for (let r = 0; r < e.length; r++) this.size += e[r].nodeSize
     }
     nodesBetween(e, t, r, i = 0, s) {
         for (let o = 0, l = 0; l < t; o++) {
             let a = this.content[o],
@@ -284,22 +284,22 @@
         if (!e) return n.empty;
         if (e instanceof n) return e;
         if (Array.isArray(e)) return this.fromArray(e);
         if (e.attrs) return new n([e], e.nodeSize);
         throw new RangeError("Can not convert " + e + " to a Fragment" + (e.nodesBetween ? " (looks like multiple versions of prosemirror-model were loaded)" : ""))
     }
 };
-M.empty = new M([], 0);
-var Gn = {
+w.empty = new w([], 0);
+var Yn = {
     index: 0,
     offset: 0
 };
 
 function nn(n, e) {
-    return Gn.index = n, Gn.offset = e, Gn
+    return Yn.index = n, Yn.offset = e, Yn
 }
 
 function rn(n, e) {
     if (n === e) return !0;
     if (!(n && typeof n == "object") || !(e && typeof e == "object")) return !1;
     let t = Array.isArray(n);
     if (Array.isArray(e) != t) return !1;
@@ -405,25 +405,25 @@
             return this.openStart > 0 && (e.openStart = this.openStart), this.openEnd > 0 && (e.openEnd = this.openEnd), e
         }
         static fromJSON(e, t) {
             if (!t) return n.empty;
             let r = t.openStart || 0,
                 i = t.openEnd || 0;
             if (typeof r != "number" || typeof i != "number") throw new RangeError("Invalid input for Slice.fromJSON");
-            return new n(M.fromJSON(e, t.content), r, i)
+            return new n(w.fromJSON(e, t.content), r, i)
         }
         static maxOpen(e, t = !0) {
             let r = 0,
                 i = 0;
             for (let s = e.firstChild; s && !s.isLeaf && (t || !s.type.spec.isolating); s = s.firstChild) r++;
             for (let s = e.lastChild; s && !s.isLeaf && (t || !s.type.spec.isolating); s = s.lastChild) i++;
             return new n(e, r, i)
         }
     };
-E.empty = new E(M.empty, 0, 0);
+E.empty = new E(w.empty, 0, 0);
 
 function Zi(n, e, t) {
     let {
         index: r,
         offset: i
     } = n.findIndex(e), s = n.maybeChild(r), {
         index: o,
@@ -443,15 +443,15 @@
         offset: s
     } = n.findIndex(e), o = n.maybeChild(i);
     if (s == e || o.isText) return r && !r.canReplace(i, i, t) ? null : n.cut(0, e).append(t).append(n.cut(e));
     let l = Qi(o.content, e - s - 1, t);
     return l && n.replaceChild(i, o.copy(l))
 }
 
-function ga(n, e, t) {
+function ya(n, e, t) {
     if (t.openStart > n.depth) throw new Ye("Inserted content deeper than insertion position");
     if (n.depth - t.openStart != e.depth - t.openEnd) throw new Ye("Inconsistent open depths");
     return es(n, e, t, 0)
 }
 
 function es(n, e, t, r) {
     let i = n.index(r),
@@ -464,25 +464,25 @@
             let o = n.parent,
                 l = o.content;
             return Ge(o, l.cut(0, n.parentOffset).append(t.content).append(l.cut(e.parentOffset)))
         } else {
             let {
                 start: o,
                 end: l
-            } = ya(t, n);
+            } = xa(t, n);
             return Ge(s, ns(n, o, l, e, r))
         }
     else return Ge(s, sn(n, e, r))
 }
 
 function ts(n, e) {
     if (!e.type.compatibleContent(n.type)) throw new Ye("Cannot join " + e.type.name + " onto " + n.type.name)
 }
 
-function Qn(n, e, t) {
+function er(n, e, t) {
     let r = n.node(t);
     return ts(r, e.node(t)), r
 }
 
 function _e(n, e) {
     let t = e.length - 1;
     t >= 0 && n.isText && n.sameMarkup(e[t]) ? e[t] = n.withText(e[t].text + n.text) : e.push(n)
@@ -498,33 +498,33 @@
 }
 
 function Ge(n, e) {
     return n.type.checkContent(e), n.copy(e)
 }
 
 function ns(n, e, t, r, i) {
-    let s = n.depth > i && Qn(n, e, i + 1),
-        o = r.depth > i && Qn(t, r, i + 1),
+    let s = n.depth > i && er(n, e, i + 1),
+        o = r.depth > i && er(t, r, i + 1),
         l = [];
-    return Nt(null, n, i, l), s && o && e.index(i) == t.index(i) ? (ts(s, o), _e(Ge(s, ns(n, e, t, r, i + 1)), l)) : (s && _e(Ge(s, sn(n, e, i + 1)), l), Nt(e, t, i, l), o && _e(Ge(o, sn(t, r, i + 1)), l)), Nt(r, null, i, l), new M(l)
+    return Nt(null, n, i, l), s && o && e.index(i) == t.index(i) ? (ts(s, o), _e(Ge(s, ns(n, e, t, r, i + 1)), l)) : (s && _e(Ge(s, sn(n, e, i + 1)), l), Nt(e, t, i, l), o && _e(Ge(o, sn(t, r, i + 1)), l)), Nt(r, null, i, l), new w(l)
 }
 
 function sn(n, e, t) {
     let r = [];
     if (Nt(null, n, t, r), n.depth > t) {
-        let i = Qn(n, e, t + 1);
+        let i = er(n, e, t + 1);
         _e(Ge(i, sn(n, e, t + 1)), r)
     }
-    return Nt(e, null, t, r), new M(r)
+    return Nt(e, null, t, r), new w(r)
 }
 
-function ya(n, e) {
+function xa(n, e) {
     let t = e.depth - n.openStart,
         i = e.node(t).copy(n.content);
-    for (let s = t - 1; s >= 0; s--) i = e.node(s).copy(M.from(i));
+    for (let s = t - 1; s >= 0; s--) i = e.node(s).copy(w.from(i));
     return {
         start: i.resolveNoCache(n.openStart + t),
         end: i.resolveNoCache(i.content.size - n.openEnd - t)
     }
 }
 var on = class n {
         constructor(e, t, r) {
@@ -645,25 +645,25 @@
                 } = o.content.findIndex(s), c = s - a;
                 if (r.push(o, l, i + a), !c || (o = o.child(l), o.isText)) break;
                 s = c - 1, i += a + 1
             }
             return new n(t, r, s)
         }
         static resolveCached(e, t) {
-            for (let i = 0; i < Yn.length; i++) {
-                let s = Yn[i];
+            for (let i = 0; i < Xn.length; i++) {
+                let s = Xn[i];
                 if (s.pos == t && s.doc == e) return s
             }
-            let r = Yn[Xn] = n.resolve(e, t);
-            return Xn = (Xn + 1) % xa, r
+            let r = Xn[Zn] = n.resolve(e, t);
+            return Zn = (Zn + 1) % ba, r
         }
     },
-    Yn = [],
-    Xn = 0,
-    xa = 12,
+    Xn = [],
+    Zn = 0,
+    ba = 12,
     Xe = class {
         constructor(e, t, r) {
             this.$from = e, this.$to = t, this.depth = r
         }
         get start() {
             return this.$from.before(this.depth + 1)
         }
@@ -676,18 +676,18 @@
         get startIndex() {
             return this.$from.index(this.depth)
         }
         get endIndex() {
             return this.$to.indexAfter(this.depth)
         }
     },
-    ba = Object.create(null),
+    ka = Object.create(null),
     ye = class n {
         constructor(e, t, r, i = j.none) {
-            this.type = e, this.attrs = t, this.marks = i, this.content = r || M.empty
+            this.type = e, this.attrs = t, this.marks = i, this.content = r || w.empty
         }
         get nodeSize() {
             return this.isLeaf ? 1 : 2 + this.content.size
         }
         get childCount() {
             return this.content.childCount
         }
@@ -721,15 +721,15 @@
         eq(e) {
             return this == e || this.sameMarkup(e) && this.content.eq(e.content)
         }
         sameMarkup(e) {
             return this.hasMarkup(e.type, e.attrs, e.marks)
         }
         hasMarkup(e, t, r) {
-            return this.type == e && rn(this.attrs, t || e.defaultAttrs || ba) && j.sameSet(this.marks, r || j.none)
+            return this.type == e && rn(this.attrs, t || e.defaultAttrs || ka) && j.sameSet(this.marks, r || j.none)
         }
         copy(e = null) {
             return e == this.content ? this : new n(this.type, this.attrs, e, this.marks)
         }
         mark(e) {
             return e == this.marks ? this : new n(this.type, this.attrs, this.content, e)
         }
@@ -742,15 +742,15 @@
                 s = this.resolve(t),
                 o = r ? 0 : i.sharedDepth(t),
                 l = i.start(o),
                 c = i.node(o).content.cut(i.pos - l, s.pos - l);
             return new E(c, i.depth - o, s.depth - o)
         }
         replace(e, t, r) {
-            return ga(this.resolve(e), this.resolve(t), r)
+            return ya(this.resolve(e), this.resolve(t), r)
         }
         nodeAt(e) {
             for (let t = this;;) {
                 let {
                     index: r,
                     offset: i
                 } = t.content.findIndex(e);
@@ -829,15 +829,15 @@
             return this.content.size && (e += "(" + this.content.toStringInner() + ")"), rs(this.marks, e)
         }
         contentMatchAt(e) {
             let t = this.type.contentMatch.matchFragment(this.content, 0, e);
             if (!t) throw new Error("Called contentMatchAt on a node with invalid content");
             return t
         }
-        canReplace(e, t, r = M.empty, i = 0, s = r.childCount) {
+        canReplace(e, t, r = w.empty, i = 0, s = r.childCount) {
             let o = this.contentMatchAt(e).matchFragment(r, i, s),
                 l = o && o.matchFragment(this.content, t);
             if (!l || !l.validEnd) return !1;
             for (let a = i; a < s; a++)
                 if (!this.type.allowsMarks(r.child(a).marks)) return !1;
             return !0
         }
@@ -874,20 +874,20 @@
                 if (!Array.isArray(t.marks)) throw new RangeError("Invalid mark data for Node.fromJSON");
                 r = t.marks.map(e.markFromJSON)
             }
             if (t.type == "text") {
                 if (typeof t.text != "string") throw new RangeError("Invalid text node in JSON");
                 return e.text(t.text, r)
             }
-            let i = M.fromJSON(e, t.content);
+            let i = w.fromJSON(e, t.content);
             return e.nodeType(t.type).create(t.attrs, i, r)
         }
     };
 ye.prototype.text = void 0;
-var er = class n extends ye {
+var tr = class n extends ye {
     constructor(e, t, r, i) {
         if (super(e, t, null, i), !r) throw new RangeError("Empty text nodes are not allowed");
         this.text = r
     }
     toString() {
         return this.type.spec.toDebugString ? this.type.spec.toDebugString(this) : rs(this.marks, JSON.stringify(this.text))
     }
@@ -923,20 +923,20 @@
     return e
 }
 var Ze = class n {
     constructor(e) {
         this.validEnd = e, this.next = [], this.wrapCache = []
     }
     static parse(e, t) {
-        let r = new tr(e, t);
+        let r = new nr(e, t);
         if (r.next == null) return n.empty;
         let i = is(r);
         r.next && r.err("Unexpected trailing text");
-        let s = Ta(Ca(i));
-        return Aa(s, r), s
+        let s = Aa(Ta(i));
+        return va(s, r), s
     }
     matchType(e) {
         for (let t = 0; t < this.next.length; t++)
             if (this.next[t].type == e) return this.next[t].next;
         return null
     }
     matchFragment(e, t = 0, r = e.childCount) {
@@ -963,15 +963,15 @@
         return !1
     }
     fillBefore(e, t = !1, r = 0) {
         let i = [this];
 
         function s(o, l) {
             let a = o.matchFragment(e, r);
-            if (a && (!t || a.validEnd)) return M.from(l.map(c => c.createAndFill()));
+            if (a && (!t || a.validEnd)) return w.from(l.map(c => c.createAndFill()));
             for (let c = 0; c < o.next.length; c++) {
                 let {
                     type: d,
                     next: u
                 } = o.next[c];
                 if (!(d.isText || d.hasRequiredAttrs()) && i.indexOf(u) == -1) {
                     i.push(u);
@@ -1037,15 +1037,15 @@
             for (let o = 0; o < r.next.length; o++) s += (o ? ", " : "") + r.next[o].type.name + "->" + e.indexOf(r.next[o].next);
             return s
         }).join(`
 `)
     }
 };
 Ze.empty = new Ze(!0);
-var tr = class {
+var nr = class {
     constructor(e, t) {
         this.string = e, this.nodeTypes = t, this.inline = null, this.pos = 0, this.tokens = e.split(/\s*(?=\b|\W|$)/), this.tokens[this.tokens.length - 1] == "" && this.tokens.pop(), this.tokens[0] == "" && this.tokens.shift()
     }
     get next() {
         return this.tokens[this.pos]
     }
     eat(e) {
@@ -1054,97 +1054,97 @@
     err(e) {
         throw new SyntaxError(e + " (in content expression '" + this.string + "')")
     }
 };
 
 function is(n) {
     let e = [];
-    do e.push(ka(n)); while (n.eat("|"));
+    do e.push(Sa(n)); while (n.eat("|"));
     return e.length == 1 ? e[0] : {
         type: "choice",
         exprs: e
     }
 }
 
-function ka(n) {
+function Sa(n) {
     let e = [];
-    do e.push(Sa(n)); while (n.next && n.next != ")" && n.next != "|");
+    do e.push(Ma(n)); while (n.next && n.next != ")" && n.next != "|");
     return e.length == 1 ? e[0] : {
         type: "seq",
         exprs: e
     }
 }
 
-function Sa(n) {
-    let e = Ea(n);
+function Ma(n) {
+    let e = Ca(n);
     for (;;)
         if (n.eat("+")) e = {
             type: "plus",
             expr: e
         };
         else if (n.eat("*")) e = {
         type: "star",
         expr: e
     };
     else if (n.eat("?")) e = {
         type: "opt",
         expr: e
     };
-    else if (n.eat("{")) e = Ma(n, e);
+    else if (n.eat("{")) e = wa(n, e);
     else break;
     return e
 }
 
 function qi(n) {
     /\D/.test(n.next) && n.err("Expected number, got '" + n.next + "'");
     let e = Number(n.next);
     return n.pos++, e
 }
 
-function Ma(n, e) {
+function wa(n, e) {
     let t = qi(n),
         r = t;
     return n.eat(",") && (n.next != "}" ? r = qi(n) : r = -1), n.eat("}") || n.err("Unclosed braced range"), {
         type: "range",
         min: t,
         max: r,
         expr: e
     }
 }
 
-function wa(n, e) {
+function Ea(n, e) {
     let t = n.nodeTypes,
         r = t[e];
     if (r) return [r];
     let i = [];
     for (let s in t) {
         let o = t[s];
         o.groups.indexOf(e) > -1 && i.push(o)
     }
     return i.length == 0 && n.err("No node type or group '" + e + "' found"), i
 }
 
-function Ea(n) {
+function Ca(n) {
     if (n.eat("(")) {
         let e = is(n);
         return n.eat(")") || n.err("Missing closing paren"), e
     } else if (/\W/.test(n.next)) n.err("Unexpected token '" + n.next + "'");
     else {
-        let e = wa(n, n.next).map(t => (n.inline == null ? n.inline = t.isInline : n.inline != t.isInline && n.err("Mixing inline and block content"), {
+        let e = Ea(n, n.next).map(t => (n.inline == null ? n.inline = t.isInline : n.inline != t.isInline && n.err("Mixing inline and block content"), {
             type: "name",
             value: t
         }));
         return n.pos++, e.length == 1 ? e[0] : {
             type: "choice",
             exprs: e
         }
     }
 }
 
-function Ca(n) {
+function Ta(n) {
     let e = [
         []
     ];
     return i(s(n, 0), t()), e;
 
     function t() {
         return e.push([]) - 1
@@ -1216,15 +1216,15 @@
                 to: a
             } = s[o];
             !l && t.indexOf(a) == -1 && r(a)
         }
     }
 }
 
-function Ta(n) {
+function Aa(n) {
     let e = Object.create(null);
     return t(Wi(n, 0));
 
     function t(r) {
         let i = [];
         r.forEach(o => {
             n[o].forEach(({
@@ -1247,15 +1247,15 @@
                 next: e[l.join(",")] || t(l)
             })
         }
         return s
     }
 }
 
-function Aa(n, e) {
+function va(n, e) {
     for (let t = 0, r = [n]; t < r.length; t++) {
         let i = r[t],
             s = !i.validEnd,
             o = [];
         for (let l = 0; l < i.next.length; l++) {
             let {
                 type: a,
@@ -1290,15 +1290,15 @@
     }
     return t
 }
 
 function cs(n) {
     let e = Object.create(null);
     if (n)
-        for (let t in n) e[t] = new nr(n[t]);
+        for (let t in n) e[t] = new rr(n[t]);
     return e
 }
 var ln = class n {
         constructor(e, t, r) {
             this.name = e, this.schema = t, this.spec = r, this.markSet = null, this.groups = r.group ? r.group.split(" ") : [], this.attrs = cs(r.attrs), this.defaultAttrs = ls(this.attrs), this.contentMatch = null, this.inlineContent = null, this.isBlock = !(r.inline || e == "text"), this.isText = e == "text"
         }
         get isInline() {
@@ -1325,27 +1325,27 @@
             return this == e || this.contentMatch.compatible(e.contentMatch)
         }
         computeAttrs(e) {
             return !e && this.defaultAttrs ? this.defaultAttrs : as(this.attrs, e)
         }
         create(e = null, t, r) {
             if (this.isText) throw new Error("NodeType.create can't construct text nodes");
-            return new ye(this, this.computeAttrs(e), M.from(t), j.setFrom(r))
+            return new ye(this, this.computeAttrs(e), w.from(t), j.setFrom(r))
         }
         createChecked(e = null, t, r) {
-            return t = M.from(t), this.checkContent(t), new ye(this, this.computeAttrs(e), t, j.setFrom(r))
+            return t = w.from(t), this.checkContent(t), new ye(this, this.computeAttrs(e), t, j.setFrom(r))
         }
         createAndFill(e = null, t, r) {
-            if (e = this.computeAttrs(e), t = M.from(t), t.size) {
+            if (e = this.computeAttrs(e), t = w.from(t), t.size) {
                 let o = this.contentMatch.fillBefore(t);
                 if (!o) return null;
                 t = o.append(t)
             }
             let i = this.contentMatch.matchFragment(t),
-                s = i && i.fillBefore(M.empty, !0);
+                s = i && i.fillBefore(w.empty, !0);
             return s ? new ye(this, e, t.append(s), j.setFrom(r)) : null
         }
         validContent(e) {
             let t = this.contentMatch.matchFragment(e);
             if (!t || !t.validEnd) return !1;
             for (let r = 0; r < e.childCount; r++)
                 if (!this.allowsMarks(e.child(r).marks)) return !1;
@@ -1375,15 +1375,15 @@
             let i = t.spec.topNode || "doc";
             if (!r[i]) throw new RangeError("Schema is missing its top node type ('" + i + "')");
             if (!r.text) throw new RangeError("Every schema needs a 'text' type");
             for (let s in r.text.attrs) throw new RangeError("The text node type should not have attributes");
             return r
         }
     },
-    nr = class {
+    rr = class {
         constructor(e) {
             this.hasDefault = Object.prototype.hasOwnProperty.call(e, "default"), this.default = e.default
         }
         get isRequired() {
             return !this.hasDefault
         }
     },
@@ -1414,15 +1414,15 @@
         }
     },
     an = class {
         constructor(e) {
             this.cached = Object.create(null);
             let t = this.spec = {};
             for (let i in e) t[i] = e[i];
-            t.nodes = _n.from(e.nodes), t.marks = _n.from(e.marks || {}), this.nodes = ln.compile(this.spec.nodes, this), this.marks = It.compile(this.spec.marks, this);
+            t.nodes = Gn.from(e.nodes), t.marks = Gn.from(e.marks || {}), this.nodes = ln.compile(this.spec.nodes, this), this.marks = It.compile(this.spec.marks, this);
             let r = Object.create(null);
             for (let i in this.nodes) {
                 if (i in this.marks) throw new RangeError(i + " can not be both a node and a mark");
                 let s = this.nodes[i],
                     o = s.spec.content || "",
                     l = s.spec.marks;
                 s.contentMatch = r[o] || (r[o] = Ze.parse(o, this.nodes)), s.inlineContent = s.contentMatch.inlineContent, s.markSet = l == "_" ? null : l ? Ki(this, l.split(" ")) : l == "" || !s.inlineContent ? [] : null
@@ -1439,15 +1439,15 @@
             else if (e instanceof ln) {
                 if (e.schema != this) throw new RangeError("Node type from different schema used (" + e.name + ")")
             } else throw new RangeError("Invalid node type: " + e);
             return e.createChecked(t, r, i)
         }
         text(e, t) {
             let r = this.nodes.text;
-            return new er(r, r.defaultAttrs, e, j.setFrom(t))
+            return new tr(r, r.defaultAttrs, e, j.setFrom(t))
         }
         mark(e, t) {
             return typeof e == "string" && (e = this.marks[e]), e.create(t)
         }
         nodeFromJSON(e) {
             return ye.fromJSON(this, e)
         }
@@ -1473,18 +1473,26 @@
                 let a = n.marks[l];
                 (i == "_" || a.spec.group && a.spec.group.split(" ").indexOf(i) > -1) && t.push(o = a)
             }
         if (!o) throw new SyntaxError("Unknown mark type: '" + e[r] + "'")
     }
     return t
 }
+
+function Oa(n) {
+    return n.tag != null
+}
+
+function Na(n) {
+    return n.style != null
+}
 var Qe = class n {
         constructor(e, t) {
             this.schema = e, this.rules = t, this.tags = [], this.styles = [], t.forEach(r => {
-                r.tag ? this.tags.push(r) : r.style && this.styles.push(r)
+                Oa(r) ? this.tags.push(r) : Na(r) && this.styles.push(r)
             }), this.normalizeLists = !this.tags.some(r => {
                 if (!/^(ul|ol)\b/.test(r.tag) || !r.node) return !1;
                 let i = e.nodes[r.node];
                 return i.contentMatch.matchType(i)
             })
         }
         parse(e, t = {}) {
@@ -1494,15 +1502,15 @@
         parseSlice(e, t = {}) {
             let r = new un(this, t, !0);
             return r.addAll(e, t.from, t.to), E.maxOpen(r.finish())
         }
         matchTag(e, t, r) {
             for (let i = r ? this.tags.indexOf(r) + 1 : 0; i < this.tags.length; i++) {
                 let s = this.tags[i];
-                if (Na(e, s.tag) && (s.namespace === void 0 || e.namespaceURI == s.namespace) && (!s.context || t.matchesContext(s.context))) {
+                if (Pa(e, s.tag) && (s.namespace === void 0 || e.namespaceURI == s.namespace) && (!s.context || t.matchesContext(s.context))) {
                     if (s.getAttrs) {
                         let o = s.getAttrs(e);
                         if (o === !1) continue;
                         s.attrs = o || void 0
                     }
                     return s
                 }
@@ -1582,15 +1590,15 @@
         p: !0,
         pre: !0,
         section: !0,
         table: !0,
         tfoot: !0,
         ul: !0
     },
-    va = {
+    Da = {
         head: !0,
         noscript: !0,
         object: !0,
         script: !0,
         style: !0,
         title: !0
     },
@@ -1608,15 +1616,15 @@
 var pt = class {
         constructor(e, t, r, i, s, o, l) {
             this.type = e, this.attrs = t, this.marks = r, this.pendingMarks = i, this.solid = s, this.options = l, this.content = [], this.activeMarks = j.none, this.stashMarks = [], this.match = o || (l & Dt ? null : e.contentMatch)
         }
         findWrapping(e) {
             if (!this.match) {
                 if (!this.type) return [];
-                let t = this.type.contentMatch.fillBefore(M.from(e));
+                let t = this.type.contentMatch.fillBefore(w.from(e));
                 if (t) this.match = this.type.contentMatch.matchFragment(t);
                 else {
                     let r = this.type.contentMatch,
                         i;
                     return (i = r.findWrapping(e.type)) ? (this.match = r, i) : null
                 }
             }
@@ -1627,25 +1635,25 @@
                 let r = this.content[this.content.length - 1],
                     i;
                 if (r && r.isText && (i = /[ \t\r\n\u000c]+$/.exec(r.text))) {
                     let s = r;
                     r.text.length == i[0].length ? this.content.pop() : this.content[this.content.length - 1] = s.withText(s.text.slice(0, s.text.length - i[0].length))
                 }
             }
-            let t = M.from(this.content);
-            return !e && this.match && (t = t.append(this.match.fillBefore(M.empty, !0))), this.type ? this.type.create(this.attrs, t, this.marks) : t
+            let t = w.from(this.content);
+            return !e && this.match && (t = t.append(this.match.fillBefore(w.empty, !0))), this.type ? this.type.create(this.attrs, t, this.marks) : t
         }
         popFromStashMark(e) {
             for (let t = this.stashMarks.length - 1; t >= 0; t--)
                 if (e.eq(this.stashMarks[t])) return this.stashMarks.splice(t, 1)[0]
         }
         applyPending(e) {
             for (let t = 0, r = this.pendingMarks; t < r.length; t++) {
                 let i = r[t];
-                (this.type ? this.type.allowsMarkType(i.type) : Ia(i.type, e)) && !i.isInSet(this.activeMarks) && (this.activeMarks = i.addToSet(this.activeMarks), this.pendingMarks = i.removeFromSet(this.pendingMarks))
+                (this.type ? this.type.allowsMarkType(i.type) : La(i.type, e)) && !i.isInSet(this.activeMarks) && (this.activeMarks = i.addToSet(this.activeMarks), this.pendingMarks = i.removeFromSet(this.pendingMarks))
             }
         }
         inlineContext(e) {
             return this.type ? this.type.inlineContent : this.content.length ? this.content[0].isInline : e.parentNode && !ds.hasOwnProperty(e.parentNode.nodeName.toLowerCase())
         }
     },
     un = class {
@@ -1660,15 +1668,15 @@
         }
         addDOM(e) {
             e.nodeType == 3 ? this.addTextNode(e) : e.nodeType == 1 && this.addElement(e)
         }
         withStyleRules(e, t) {
             let r = e.getAttribute("style");
             if (!r) return t();
-            let i = this.readStyles(Da(r));
+            let i = this.readStyles(Ra(r));
             if (!i) return;
             let [s, o] = i, l = this.top;
             for (let a = 0; a < o.length; a++) this.removePendingMark(o[a], l);
             for (let a = 0; a < s.length; a++) this.addPendingMark(s[a]);
             t();
             for (let a = 0; a < s.length; a++) this.removePendingMark(s[a], l);
             for (let a = 0; a < o.length; a++) this.addPendingMark(o[a])
@@ -1686,17 +1694,17 @@
                 }
                 t && this.insertNode(this.parser.schema.text(t)), this.findInText(e)
             } else this.findInside(e)
         }
         addElement(e, t) {
             let r = e.nodeName.toLowerCase(),
                 i;
-            us.hasOwnProperty(r) && this.parser.normalizeLists && Oa(e);
+            us.hasOwnProperty(r) && this.parser.normalizeLists && Ia(e);
             let s = this.options.ruleFromNode && this.options.ruleFromNode(e) || (i = this.parser.matchTag(e, this, t));
-            if (s ? s.ignore : va.hasOwnProperty(r)) this.findInside(e), this.ignoreFallback(e);
+            if (s ? s.ignore : Da.hasOwnProperty(r)) this.findInside(e), this.ignoreFallback(e);
             else if (!s || s.skip || s.closeParent) {
                 s && s.closeParent ? this.open = Math.max(0, this.open - 1) : s && s.skip.nodeType && (e = s.skip);
                 let o, l = this.top,
                     a = this.needsBlock;
                 if (ds.hasOwnProperty(r)) l.content.length && l.content[0].isInline && this.open && (this.open--, l = this.top), o = !0, l.type || (this.needsBlock = !0);
                 else if (!e.firstChild) {
                     this.leafFallback(e);
@@ -1859,15 +1867,15 @@
                 }
             for (let t in this.parser.schema.nodes) {
                 let r = this.parser.schema.nodes[t];
                 if (r.isTextblock && r.defaultAttrs) return r
             }
         }
         addPendingMark(e) {
-            let t = Pa(e, this.top.pendingMarks);
+            let t = Ba(e, this.top.pendingMarks);
             t && this.top.stashMarks.push(t), this.top.pendingMarks = e.addToSet(this.top.pendingMarks)
         }
         removePendingMark(e, t) {
             for (let r = this.open; r >= 0; r--) {
                 let i = this.nodes[r];
                 if (i.pendingMarks.lastIndexOf(e) > -1) i.pendingMarks = e.removeFromSet(i.pendingMarks);
                 else {
@@ -1876,39 +1884,39 @@
                     o && i.type && i.type.allowsMarkType(o.type) && (i.activeMarks = o.addToSet(i.activeMarks))
                 }
                 if (i == t) break
             }
         }
     };
 
-function Oa(n) {
+function Ia(n) {
     for (let e = n.firstChild, t = null; e; e = e.nextSibling) {
         let r = e.nodeType == 1 ? e.nodeName.toLowerCase() : null;
         r && us.hasOwnProperty(r) && t ? (t.appendChild(e), e = t) : r == "li" ? t = e : r && (t = null)
     }
 }
 
-function Na(n, e) {
+function Pa(n, e) {
     return (n.matches || n.msMatchesSelector || n.webkitMatchesSelector || n.mozMatchesSelector).call(n, e)
 }
 
-function Da(n) {
+function Ra(n) {
     let e = /\s*([\w-]+)\s*:\s*([^;]+)/g,
         t, r = [];
     for (; t = e.exec(n);) r.push(t[1], t[2].trim());
     return r
 }
 
 function _i(n) {
     let e = {};
     for (let t in n) e[t] = n[t];
     return e
 }
 
-function Ia(n, e) {
+function La(n, e) {
     let t = e.schema.nodes;
     for (let r in t) {
         let i = t[r];
         if (!i.allowsMarkType(n)) continue;
         let s = [],
             o = l => {
                 s.push(l);
@@ -1920,24 +1928,24 @@
                     if (c == e || s.indexOf(d) < 0 && o(d)) return !0
                 }
             };
         if (o(i.contentMatch)) return !0
     }
 }
 
-function Pa(n, e) {
+function Ba(n, e) {
     for (let t = 0; t < e.length; t++)
         if (n.eq(e[t])) return e[t]
 }
 var Oe = class n {
     constructor(e, t) {
         this.nodes = e, this.marks = t
     }
     serializeFragment(e, t = {}, r) {
-        r || (r = Zn(t).createDocumentFragment());
+        r || (r = Qn(t).createDocumentFragment());
         let i = r,
             s = [];
         return e.forEach(o => {
             if (s.length || o.marks.length) {
                 let l = 0,
                     a = 0;
                 for (; l < s.length && a < o.marks.length;) {
@@ -1959,15 +1967,15 @@
             i.appendChild(this.serializeNodeInner(o, t))
         }), r
     }
     serializeNodeInner(e, t) {
         let {
             dom: r,
             contentDOM: i
-        } = n.renderSpec(Zn(t), this.nodes[e.type.name](e));
+        } = n.renderSpec(Qn(t), this.nodes[e.type.name](e));
         if (i) {
             if (e.isLeaf) throw new RangeError("Content hole not allowed in a leaf node spec");
             this.serializeFragment(e.content, t, i)
         }
         return r
     }
     serializeNode(e, t = {}) {
@@ -1976,15 +1984,15 @@
             let s = this.serializeMark(e.marks[i], e.isInline, t);
             s && ((s.contentDOM || s.dom).appendChild(r), r = s.dom)
         }
         return r
     }
     serializeMark(e, t, r = {}) {
         let i = this.marks[e.type.name];
-        return i && n.renderSpec(Zn(r), i(e, t))
+        return i && n.renderSpec(Qn(r), i(e, t))
     }
     static renderSpec(e, t, r = null) {
         if (typeof t == "string") return {
             dom: e.createTextNode(t)
         };
         if (t.nodeType != null) return {
             dom: t
@@ -2045,29 +2053,29 @@
     for (let t in n) {
         let r = n[t].spec.toDOM;
         r && (e[t] = r)
     }
     return e
 }
 
-function Zn(n) {
+function Qn(n) {
     return n.document || window.document
 }
 var ps = 65535,
     ms = Math.pow(2, 16);
 
-function Ra(n, e) {
+function Fa(n, e) {
     return n + e * ms
 }
 
 function fs(n) {
     return n & ps
 }
 
-function La(n) {
+function za(n) {
     return (n - (n & ps)) / ms
 }
 var gs = 1,
     ys = 2,
     fn = 4,
     xs = 8,
     Lt = class {
@@ -2092,15 +2100,15 @@
             if (this.ranges = e, this.inverted = t, !e.length && n.empty) return n.empty
         }
         recover(e) {
             let t = 0,
                 r = fs(e);
             if (!this.inverted)
                 for (let i = 0; i < r; i++) t += this.ranges[i * 3 + 2] - this.ranges[i * 3 + 1];
-            return this.ranges[r * 3] + t + La(e)
+            return this.ranges[r * 3] + t + za(e)
         }
         mapResult(e, t = 1) {
             return this._map(e, t, !1)
         }
         map(e, t = 1) {
             return this._map(e, t, !0)
         }
@@ -2114,15 +2122,15 @@
                 let c = this.ranges[l + s],
                     d = this.ranges[l + o],
                     u = a + c;
                 if (e <= u) {
                     let f = c ? e == a ? -1 : e == u ? 1 : t : t,
                         h = a + i + (f < 0 ? 0 : d);
                     if (r) return h;
-                    let p = e == (t < 0 ? a : u) ? null : Ra(l / 3, e - a),
+                    let p = e == (t < 0 ? a : u) ? null : Fa(l / 3, e - a),
                         m = e == a ? ys : e == u ? gs : fn;
                     return (t < 0 ? e != a : e != u) && (m |= xs), new Lt(h, m, p)
                 }
                 i += d - c
             }
             return r ? e + i : new Lt(e + i, 0, null)
         }
@@ -2223,31 +2231,31 @@
                     }
                 }
                 i |= l.delInfo, e = l.pos
             }
             return r ? e : new Lt(e, i, null)
         }
     },
-    rr = Object.create(null),
+    ir = Object.create(null),
     X = class {
         getMap() {
             return Ne.empty
         }
         merge(e) {
             return null
         }
         static fromJSON(e, t) {
             if (!t || !t.stepType) throw new RangeError("Invalid input for Step.fromJSON");
-            let r = rr[t.stepType];
+            let r = ir[t.stepType];
             if (!r) throw new RangeError(`No step type ${t.stepType} defined`);
             return r.fromJSON(e, t)
         }
         static jsonID(e, t) {
-            if (e in rr) throw new RangeError("Duplicate use of step JSON ID " + e);
-            return rr[e] = t, t.prototype.jsonID = e, t
+            if (e in ir) throw new RangeError("Duplicate use of step JSON ID " + e);
+            return ir[e] = t, t.prototype.jsonID = e, t
         }
     },
     Q = class n {
         constructor(e, t) {
             this.doc = e, this.failed = t
         }
         static ok(e) {
@@ -2262,31 +2270,31 @@
             } catch (s) {
                 if (s instanceof Ye) return n.fail(s.message);
                 throw s
             }
         }
     };
 
-function ar(n, e, t) {
+function cr(n, e, t) {
     let r = [];
     for (let i = 0; i < n.childCount; i++) {
         let s = n.child(i);
-        s.content.size && (s = s.copy(ar(s.content, e, s))), s.isInline && (s = e(s, t, i)), r.push(s)
+        s.content.size && (s = s.copy(cr(s.content, e, s))), s.isInline && (s = e(s, t, i)), r.push(s)
     }
-    return M.fromArray(r)
+    return w.fromArray(r)
 }
 var Ft = class n extends X {
     constructor(e, t, r) {
         super(), this.from = e, this.to = t, this.mark = r
     }
     apply(e) {
         let t = e.slice(this.from, this.to),
             r = e.resolve(this.from),
             i = r.node(r.sharedDepth(this.to)),
-            s = new E(ar(t.content, (o, l) => !o.isAtom || !l.type.allowsMarkType(this.mark.type) ? o : o.mark(this.mark.addToSet(o.marks)), i), t.openStart, t.openEnd);
+            s = new E(cr(t.content, (o, l) => !o.isAtom || !l.type.allowsMarkType(this.mark.type) ? o : o.mark(this.mark.addToSet(o.marks)), i), t.openStart, t.openEnd);
         return Q.fromReplace(e, this.from, this.to, s)
     }
     invert() {
         return new et(this.from, this.to, this.mark)
     }
     map(e) {
         let t = e.mapResult(this.from, 1),
@@ -2312,15 +2320,15 @@
 X.jsonID("addMark", Ft);
 var et = class n extends X {
     constructor(e, t, r) {
         super(), this.from = e, this.to = t, this.mark = r
     }
     apply(e) {
         let t = e.slice(this.from, this.to),
-            r = new E(ar(t.content, i => i.mark(this.mark.removeFromSet(i.marks)), e), t.openStart, t.openEnd);
+            r = new E(cr(t.content, i => i.mark(this.mark.removeFromSet(i.marks)), e), t.openStart, t.openEnd);
         return Q.fromReplace(e, this.from, this.to, r)
     }
     invert() {
         return new Ft(this.from, this.to, this.mark)
     }
     map(e) {
         let t = e.mapResult(this.from, 1),
@@ -2348,15 +2356,15 @@
     constructor(e, t) {
         super(), this.pos = e, this.mark = t
     }
     apply(e) {
         let t = e.nodeAt(this.pos);
         if (!t) return Q.fail("No node at mark step's position");
         let r = t.type.create(t.attrs, null, this.mark.addToSet(t.marks));
-        return Q.fromReplace(e, this.pos, this.pos + 1, new E(M.from(r), 0, t.isLeaf ? 0 : 1))
+        return Q.fromReplace(e, this.pos, this.pos + 1, new E(w.from(r), 0, t.isLeaf ? 0 : 1))
     }
     invert(e) {
         let t = e.nodeAt(this.pos);
         if (t) {
             let r = this.mark.addToSet(t.marks);
             if (r.length == t.marks.length) {
                 for (let i = 0; i < t.marks.length; i++)
@@ -2387,15 +2395,15 @@
     constructor(e, t) {
         super(), this.pos = e, this.mark = t
     }
     apply(e) {
         let t = e.nodeAt(this.pos);
         if (!t) return Q.fail("No node at mark step's position");
         let r = t.type.create(t.attrs, null, this.mark.removeFromSet(t.marks));
-        return Q.fromReplace(e, this.pos, this.pos + 1, new E(M.from(r), 0, t.isLeaf ? 0 : 1))
+        return Q.fromReplace(e, this.pos, this.pos + 1, new E(w.from(r), 0, t.isLeaf ? 0 : 1))
     }
     invert(e) {
         let t = e.nodeAt(this.pos);
         return !t || !this.mark.isInSet(t.marks) ? this : new zt(this.pos, this.mark)
     }
     map(e) {
         let t = e.mapResult(this.pos, 1);
@@ -2415,15 +2423,15 @@
 };
 X.jsonID("removeNodeMark", $t);
 var ie = class n extends X {
     constructor(e, t, r, i = !1) {
         super(), this.from = e, this.to = t, this.slice = r, this.structure = i
     }
     apply(e) {
-        return this.structure && or(e, this.from, this.to) ? Q.fail("Structure replace would overwrite content") : Q.fromReplace(e, this.from, this.to, this.slice)
+        return this.structure && lr(e, this.from, this.to) ? Q.fail("Structure replace would overwrite content") : Q.fromReplace(e, this.from, this.to, this.slice)
     }
     getMap() {
         return new Ne([this.from, this.to - this.from, this.slice.size])
     }
     invert(e) {
         return new n(this.from, this.from + this.slice.size, e.slice(this.from, this.to))
     }
@@ -2457,15 +2465,15 @@
 };
 X.jsonID("replace", ie);
 var U = class n extends X {
     constructor(e, t, r, i, s, o, l = !1) {
         super(), this.from = e, this.to = t, this.gapFrom = r, this.gapTo = i, this.slice = s, this.insert = o, this.structure = l
     }
     apply(e) {
-        if (this.structure && (or(e, this.from, this.gapFrom) || or(e, this.gapTo, this.to))) return Q.fail("Structure gap-replace would overwrite content");
+        if (this.structure && (lr(e, this.from, this.gapFrom) || lr(e, this.gapTo, this.to))) return Q.fail("Structure gap-replace would overwrite content");
         let t = e.slice(this.gapFrom, this.gapTo);
         if (t.openStart || t.openEnd) return Q.fail("Gap is not a flat range");
         let r = this.slice.insertAt(this.insert, t.content);
         return r ? Q.fromReplace(e, this.from, this.to, r) : Q.fail("Content does not fit in gap")
     }
     getMap() {
         return new Ne([this.from, this.gapFrom - this.from, this.insert, this.gapTo, this.to - this.gapTo, this.slice.size - this.insert])
@@ -2495,30 +2503,30 @@
     static fromJSON(e, t) {
         if (typeof t.from != "number" || typeof t.to != "number" || typeof t.gapFrom != "number" || typeof t.gapTo != "number" || typeof t.insert != "number") throw new RangeError("Invalid input for ReplaceAroundStep.fromJSON");
         return new n(t.from, t.to, t.gapFrom, t.gapTo, E.fromJSON(e, t.slice), t.insert, !!t.structure)
     }
 };
 X.jsonID("replaceAround", U);
 
-function or(n, e, t) {
+function lr(n, e, t) {
     let r = n.resolve(e),
         i = t - e,
         s = r.depth;
     for (; i > 0 && s > 0 && r.indexAfter(s) == r.node(s).childCount;) s--, i--;
     if (i > 0) {
         let o = r.node(s).maybeChild(r.indexAfter(s));
         for (; i > 0;) {
             if (!o || o.isLeaf) return !0;
             o = o.firstChild, i--
         }
     }
     return !1
 }
 
-function Ba(n, e, t, r) {
+function $a(n, e, t, r) {
     let i = [],
         s = [],
         o, l;
     n.doc.nodesBetween(e, t, (a, c, d) => {
         if (!a.isInline) return;
         let u = a.marks;
         if (!r.isInSet(u) && d.type.allowsMarkType(r.type)) {
@@ -2527,15 +2535,15 @@
                 p = r.addToSet(u);
             for (let m = 0; m < u.length; m++) u[m].isInSet(p) || (o && o.to == f && o.mark.eq(u[m]) ? o.to = h : i.push(o = new et(f, h, u[m])));
             l && l.to == f ? l.to = h : s.push(l = new Ft(f, h, r))
         }
     }), i.forEach(a => n.step(a)), s.forEach(a => n.step(a))
 }
 
-function Fa(n, e, t, r) {
+function Ha(n, e, t, r) {
     let i = [],
         s = 0;
     n.doc.nodesBetween(e, t, (o, l) => {
         if (!o.isInline) return;
         s++;
         let a = null;
         if (r instanceof It) {
@@ -2559,151 +2567,151 @@
                     step: s
                 })
             }
         }
     }), i.forEach(o => n.step(new et(o.from, o.to, o.style)))
 }
 
-function za(n, e, t, r = t.contentMatch) {
+function Va(n, e, t, r = t.contentMatch) {
     let i = n.doc.nodeAt(e),
         s = [],
         o = e + 1;
     for (let l = 0; l < i.childCount; l++) {
         let a = i.child(l),
             c = o + a.nodeSize,
             d = r.matchType(a.type);
         if (!d) s.push(new ie(o, c, E.empty));
         else {
             r = d;
             for (let u = 0; u < a.marks.length; u++) t.allowsMarkType(a.marks[u].type) || n.step(new et(o, c, a.marks[u]));
             if (a.isText && !t.spec.code) {
                 let u, f = /\r?\n|\r/g,
                     h;
-                for (; u = f.exec(a.text);) h || (h = new E(M.from(t.schema.text(" ", t.allowedMarks(a.marks))), 0, 0)), s.push(new ie(o + u.index, o + u.index + u[0].length, h))
+                for (; u = f.exec(a.text);) h || (h = new E(w.from(t.schema.text(" ", t.allowedMarks(a.marks))), 0, 0)), s.push(new ie(o + u.index, o + u.index + u[0].length, h))
             }
         }
         o = c
     }
     if (!r.validEnd) {
-        let l = r.fillBefore(M.empty, !0);
+        let l = r.fillBefore(w.empty, !0);
         n.replace(o, o, new E(l, 0, 0))
     }
     for (let l = s.length - 1; l >= 0; l--) n.step(s[l])
 }
 
-function $a(n, e, t) {
+function ja(n, e, t) {
     return (e == 0 || n.canReplace(e, n.childCount)) && (t == n.childCount || n.canReplace(0, t))
 }
 
 function De(n) {
     let t = n.parent.content.cutByIndex(n.startIndex, n.endIndex);
     for (let r = n.depth;; --r) {
         let i = n.$from.node(r),
             s = n.$from.index(r),
             o = n.$to.indexAfter(r);
         if (r < n.depth && i.canReplace(s, o, t)) return r;
-        if (r == 0 || i.type.spec.isolating || !$a(i, s, o)) break
+        if (r == 0 || i.type.spec.isolating || !ja(i, s, o)) break
     }
     return null
 }
 
-function Ha(n, e, t) {
+function Ja(n, e, t) {
     let {
         $from: r,
         $to: i,
         depth: s
-    } = e, o = r.before(s + 1), l = i.after(s + 1), a = o, c = l, d = M.empty, u = 0;
-    for (let p = s, m = !1; p > t; p--) m || r.index(p) > 0 ? (m = !0, d = M.from(r.node(p).copy(d)), u++) : a--;
-    let f = M.empty,
+    } = e, o = r.before(s + 1), l = i.after(s + 1), a = o, c = l, d = w.empty, u = 0;
+    for (let p = s, m = !1; p > t; p--) m || r.index(p) > 0 ? (m = !0, d = w.from(r.node(p).copy(d)), u++) : a--;
+    let f = w.empty,
         h = 0;
-    for (let p = s, m = !1; p > t; p--) m || i.after(p + 1) < i.end(p) ? (m = !0, f = M.from(i.node(p).copy(f)), h++) : c++;
+    for (let p = s, m = !1; p > t; p--) m || i.after(p + 1) < i.end(p) ? (m = !0, f = w.from(i.node(p).copy(f)), h++) : c++;
     n.step(new U(a, c, o, l, new E(d.append(f), u, h), d.size - u, !0))
 }
 
 function gt(n, e, t = null, r = n) {
-    let i = Va(n, e),
-        s = i && ja(r, e);
+    let i = qa(n, e),
+        s = i && Wa(r, e);
     return s ? i.map(hs).concat({
         type: e,
         attrs: t
     }).concat(s.map(hs)) : null
 }
 
 function hs(n) {
     return {
         type: n,
         attrs: null
     }
 }
 
-function Va(n, e) {
+function qa(n, e) {
     let {
         parent: t,
         startIndex: r,
         endIndex: i
     } = n, s = t.contentMatchAt(r).findWrapping(e);
     if (!s) return null;
     let o = s.length ? s[0] : e;
     return t.canReplaceWith(r, i, o) ? s : null
 }
 
-function ja(n, e) {
+function Wa(n, e) {
     let {
         parent: t,
         startIndex: r,
         endIndex: i
     } = n, s = t.child(r), o = e.contentMatch.findWrapping(s.type);
     if (!o) return null;
     let a = (o.length ? o[o.length - 1] : e).contentMatch;
     for (let c = r; a && c < i; c++) a = a.matchType(t.child(c).type);
     return !a || !a.validEnd ? null : o
 }
 
-function Ja(n, e, t) {
-    let r = M.empty;
+function Ka(n, e, t) {
+    let r = w.empty;
     for (let o = t.length - 1; o >= 0; o--) {
         if (r.size) {
             let l = t[o].type.contentMatch.matchFragment(r);
             if (!l || !l.validEnd) throw new RangeError("Wrapper type given to Transform.wrap does not form valid content of its parent wrapper")
         }
-        r = M.from(t[o].type.create(t[o].attrs, r))
+        r = w.from(t[o].type.create(t[o].attrs, r))
     }
     let i = e.start,
         s = e.end;
     n.step(new U(i, s, i, s, new E(r, 0, 0), t.length, !0))
 }
 
-function qa(n, e, t, r, i) {
+function Ua(n, e, t, r, i) {
     if (!r.isTextblock) throw new RangeError("Type given to setBlockType should be a textblock");
     let s = n.steps.length;
     n.doc.nodesBetween(e, t, (o, l) => {
-        if (o.isTextblock && !o.hasMarkup(r, i) && Wa(n.doc, n.mapping.slice(s).map(l), r)) {
+        if (o.isTextblock && !o.hasMarkup(r, i) && _a(n.doc, n.mapping.slice(s).map(l), r)) {
             n.clearIncompatible(n.mapping.slice(s).map(l, 1), r);
             let a = n.mapping.slice(s),
                 c = a.map(l, 1),
                 d = a.map(l + o.nodeSize, 1);
-            return n.step(new U(c, d, c + 1, d - 1, new E(M.from(r.create(i, null, o.marks)), 0, 0), 1, !0)), !1
+            return n.step(new U(c, d, c + 1, d - 1, new E(w.from(r.create(i, null, o.marks)), 0, 0), 1, !0)), !1
         }
     })
 }
 
-function Wa(n, e, t) {
+function _a(n, e, t) {
     let r = n.resolve(e),
         i = r.index();
     return r.parent.canReplaceWith(i, i + 1, t)
 }
 
-function Ka(n, e, t, r, i) {
+function Ga(n, e, t, r, i) {
     let s = n.doc.nodeAt(e);
     if (!s) throw new RangeError("No node at given position");
     t || (t = s.type);
     let o = t.create(r, null, i || s.marks);
     if (s.isLeaf) return n.replaceWith(e, e + s.nodeSize, o);
     if (!t.validContent(s.content)) throw new RangeError("Invalid content for node type " + t.name);
-    n.step(new U(e, e + s.nodeSize, e + 1, e + s.nodeSize - 1, new E(M.from(o), 0, 0), 1, !0))
+    n.step(new U(e, e + s.nodeSize, e + 1, e + s.nodeSize - 1, new E(w.from(o), 0, 0), 1, !0))
 }
 
 function pe(n, e, t = 1, r) {
     let i = n.resolve(e),
         s = i.depth - t,
         o = r && r[r.length - 1] || i.parent;
     if (s < 0 || i.parent.type.spec.isolating || !i.parent.canReplace(i.index(), i.parent.childCount) || !o.type.validContent(i.parent.content.cutByIndex(i.index(), i.parent.childCount))) return !1;
@@ -2718,22 +2726,22 @@
         if (!u.canReplace(f + 1, u.childCount) || !m.type.validContent(h)) return !1
     }
     let l = i.indexAfter(s),
         a = r && r[0];
     return i.node(s).canReplaceWith(l, l, a ? a.type : i.node(s + 1).type)
 }
 
-function Ua(n, e, t = 1, r) {
+function Ya(n, e, t = 1, r) {
     let i = n.doc.resolve(e),
-        s = M.empty,
-        o = M.empty;
+        s = w.empty,
+        o = w.empty;
     for (let l = i.depth, a = i.depth - t, c = t - 1; l > a; l--, c--) {
-        s = M.from(i.node(l).copy(s));
+        s = w.from(i.node(l).copy(s));
         let d = r && r[c];
-        o = M.from(d ? d.type.create(d.attrs, o) : i.node(l).copy(o))
+        o = w.from(d ? d.type.create(d.attrs, o) : i.node(l).copy(o))
     }
     n.step(new ie(e, e, new E(s.append(o), t, t), !0))
 }
 
 function xe(n, e) {
     let t = n.resolve(e),
         r = t.index();
@@ -2750,20 +2758,20 @@
         let s, o, l = r.index(i);
         if (i == r.depth ? (s = r.nodeBefore, o = r.nodeAfter) : t > 0 ? (s = r.node(i + 1), l++, o = r.node(i).maybeChild(l)) : (s = r.node(i).maybeChild(l - 1), o = r.node(i + 1)), s && !s.isTextblock && bs(s, o) && r.node(i).canReplace(l, l + 1)) return e;
         if (i == 0) break;
         e = t < 0 ? r.before(i) : r.after(i)
     }
 }
 
-function _a(n, e, t) {
+function Xa(n, e, t) {
     let r = new ie(e - t, e + t, E.empty, !0);
     n.step(r)
 }
 
-function Ga(n, e, t) {
+function Za(n, e, t) {
     let r = n.resolve(e);
     if (r.parent.canReplaceWith(r.index(), r.index(), t)) return e;
     if (r.parentOffset == 0)
         for (let i = r.depth - 1; i >= 0; i--) {
             let s = r.index(i);
             if (r.node(i).canReplaceWith(s, s, t)) return r.before(i + 1);
             if (s > 0) return null
@@ -2798,31 +2806,31 @@
     return null
 }
 
 function Vt(n, e, t = e, r = E.empty) {
     if (e == t && !r.size) return null;
     let i = n.resolve(e),
         s = n.resolve(t);
-    return Ss(i, s, r) ? new ie(e, t, r) : new lr(i, s, r).fit()
+    return Ss(i, s, r) ? new ie(e, t, r) : new ar(i, s, r).fit()
 }
 
 function Ss(n, e, t) {
     return !t.openStart && !t.openEnd && n.start() == e.start() && n.parent.canReplace(n.index(), e.index(), t.content)
 }
-var lr = class {
+var ar = class {
     constructor(e, t, r) {
-        this.$from = e, this.$to = t, this.unplaced = r, this.frontier = [], this.placed = M.empty;
+        this.$from = e, this.$to = t, this.unplaced = r, this.frontier = [], this.placed = w.empty;
         for (let i = 0; i <= e.depth; i++) {
             let s = e.node(i);
             this.frontier.push({
                 type: s.type,
                 match: s.contentMatchAt(e.indexAfter(i))
             })
         }
-        for (let i = e.depth; i > 0; i--) this.placed = M.from(e.node(i).copy(this.placed))
+        for (let i = e.depth; i > 0; i--) this.placed = w.from(e.node(i).copy(this.placed))
     }
     get depth() {
         return this.frontier.length - 1
     }
     fit() {
         for (; this.unplaced.size;) {
             let c = this.findFittable();
@@ -2849,22 +2857,22 @@
                 break
             }
             t = s.content
         }
         for (let t = 1; t <= 2; t++)
             for (let r = t == 1 ? e : this.unplaced.openStart; r >= 0; r--) {
                 let i, s = null;
-                r ? (s = ir(this.unplaced.content, r - 1).firstChild, i = s.content) : i = this.unplaced.content;
+                r ? (s = sr(this.unplaced.content, r - 1).firstChild, i = s.content) : i = this.unplaced.content;
                 let o = i.firstChild;
                 for (let l = this.depth; l >= 0; l--) {
                     let {
                         type: a,
                         match: c
                     } = this.frontier[l], d, u = null;
-                    if (t == 1 && (o ? c.matchType(o.type) || (u = c.fillBefore(M.from(o), !1)) : s && a.compatibleContent(s.type))) return {
+                    if (t == 1 && (o ? c.matchType(o.type) || (u = c.fillBefore(w.from(o), !1)) : s && a.compatibleContent(s.type))) return {
                         sliceDepth: r,
                         frontierDepth: l,
                         parent: s,
                         inject: u
                     };
                     if (t == 2 && o && (d = c.findWrapping(o.type))) return {
                         sliceDepth: r,
@@ -2877,23 +2885,23 @@
             }
     }
     openMore() {
         let {
             content: e,
             openStart: t,
             openEnd: r
-        } = this.unplaced, i = ir(e, t);
+        } = this.unplaced, i = sr(e, t);
         return !i.childCount || i.firstChild.isLeaf ? !1 : (this.unplaced = new E(e, t + 1, Math.max(r, i.size + t >= e.size - r ? t + 1 : 0)), !0)
     }
     dropNode() {
         let {
             content: e,
             openStart: t,
             openEnd: r
-        } = this.unplaced, i = ir(e, t);
+        } = this.unplaced, i = sr(e, t);
         if (i.childCount <= 1 && t > 0) {
             let s = e.size - t <= t + i.size;
             this.unplaced = new E(Pt(e, t - 1, 1), t - 1, s ? t - 1 : r)
         } else this.unplaced = new E(Pt(e, t, 1), t, r)
     }
     placeNodes({
         sliceDepth: e,
@@ -2922,47 +2930,47 @@
         for (; c < l.childCount;) {
             let m = l.child(c),
                 g = u.matchType(m.type);
             if (!g) break;
             c++, (c > 1 || a == 0 || m.content.size) && (u = g, d.push(Ms(m.mark(f.allowedMarks(m.marks)), c == 1 ? a : 0, c == l.childCount ? h : -1)))
         }
         let p = c == l.childCount;
-        p || (h = -1), this.placed = Rt(this.placed, t, M.from(d)), this.frontier[t].match = u, p && h < 0 && r && r.type == this.frontier[this.depth].type && this.frontier.length > 1 && this.closeFrontierNode();
+        p || (h = -1), this.placed = Rt(this.placed, t, w.from(d)), this.frontier[t].match = u, p && h < 0 && r && r.type == this.frontier[this.depth].type && this.frontier.length > 1 && this.closeFrontierNode();
         for (let m = 0, g = l; m < h; m++) {
             let k = g.lastChild;
             this.frontier.push({
                 type: k.type,
                 match: k.contentMatchAt(k.childCount)
             }), g = k.content
         }
         this.unplaced = p ? e == 0 ? E.empty : new E(Pt(o.content, e - 1, 1), e - 1, h < 0 ? o.openEnd : e - 1) : new E(Pt(o.content, e, c), o.openStart, o.openEnd)
     }
     mustMoveInline() {
         if (!this.$to.parent.isTextblock) return -1;
         let e = this.frontier[this.depth],
             t;
-        if (!e.type.isTextblock || !sr(this.$to, this.$to.depth, e.type, e.match, !1) || this.$to.depth == this.depth && (t = this.findCloseLevel(this.$to)) && t.depth == this.depth) return -1;
+        if (!e.type.isTextblock || !or(this.$to, this.$to.depth, e.type, e.match, !1) || this.$to.depth == this.depth && (t = this.findCloseLevel(this.$to)) && t.depth == this.depth) return -1;
         let {
             depth: r
         } = this.$to, i = this.$to.after(r);
         for (; r > 1 && i == this.$to.end(--r);) ++i;
         return i
     }
     findCloseLevel(e) {
         e: for (let t = Math.min(this.depth, e.depth); t >= 0; t--) {
             let {
                 match: r,
                 type: i
-            } = this.frontier[t], s = t < e.depth && e.end(t + 1) == e.pos + (e.depth - (t + 1)), o = sr(e, t, i, r, s);
+            } = this.frontier[t], s = t < e.depth && e.end(t + 1) == e.pos + (e.depth - (t + 1)), o = or(e, t, i, r, s);
             if (o) {
                 for (let l = t - 1; l >= 0; l--) {
                     let {
                         match: a,
                         type: c
-                    } = this.frontier[l], d = sr(e, l, c, a, !0);
+                    } = this.frontier[l], d = or(e, l, c, a, !0);
                     if (!d || d.childCount) continue e
                 }
                 return {
                     depth: t,
                     fit: o,
                     move: s ? e.doc.resolve(e.after(t + 1)) : e
                 }
@@ -2979,63 +2987,63 @@
                 s = i.type.contentMatch.fillBefore(i.content, !0, e.index(r));
             this.openFrontierNode(i.type, i.attrs, s)
         }
         return e
     }
     openFrontierNode(e, t = null, r) {
         let i = this.frontier[this.depth];
-        i.match = i.match.matchType(e), this.placed = Rt(this.placed, this.depth, M.from(e.create(t, r))), this.frontier.push({
+        i.match = i.match.matchType(e), this.placed = Rt(this.placed, this.depth, w.from(e.create(t, r))), this.frontier.push({
             type: e,
             match: e.contentMatch
         })
     }
     closeFrontierNode() {
-        let t = this.frontier.pop().match.fillBefore(M.empty, !0);
+        let t = this.frontier.pop().match.fillBefore(w.empty, !0);
         t.childCount && (this.placed = Rt(this.placed, this.frontier.length, t))
     }
 };
 
 function Pt(n, e, t) {
     return e == 0 ? n.cutByIndex(t, n.childCount) : n.replaceChild(0, n.firstChild.copy(Pt(n.firstChild.content, e - 1, t)))
 }
 
 function Rt(n, e, t) {
     return e == 0 ? n.append(t) : n.replaceChild(n.childCount - 1, n.lastChild.copy(Rt(n.lastChild.content, e - 1, t)))
 }
 
-function ir(n, e) {
+function sr(n, e) {
     for (let t = 0; t < e; t++) n = n.firstChild.content;
     return n
 }
 
 function Ms(n, e, t) {
     if (e <= 0) return n;
     let r = n.content;
-    return e > 1 && (r = r.replaceChild(0, Ms(r.firstChild, e - 1, r.childCount == 1 ? t - 1 : 0))), e > 0 && (r = n.type.contentMatch.fillBefore(r).append(r), t <= 0 && (r = r.append(n.type.contentMatch.matchFragment(r).fillBefore(M.empty, !0)))), n.copy(r)
+    return e > 1 && (r = r.replaceChild(0, Ms(r.firstChild, e - 1, r.childCount == 1 ? t - 1 : 0))), e > 0 && (r = n.type.contentMatch.fillBefore(r).append(r), t <= 0 && (r = r.append(n.type.contentMatch.matchFragment(r).fillBefore(w.empty, !0)))), n.copy(r)
 }
 
-function sr(n, e, t, r, i) {
+function or(n, e, t, r, i) {
     let s = n.node(e),
         o = i ? n.indexAfter(e) : n.index(e);
     if (o == s.childCount && !t.compatibleContent(s.type)) return null;
     let l = r.fillBefore(s.content, !0, o);
-    return l && !Ya(t, s.content, o) ? l : null
+    return l && !Qa(t, s.content, o) ? l : null
 }
 
-function Ya(n, e, t) {
+function Qa(n, e, t) {
     for (let r = t; r < e.childCount; r++)
         if (!n.allowsMarks(e.child(r).marks)) return !0;
     return !1
 }
 
-function Xa(n) {
+function ec(n) {
     return n.spec.defining || n.spec.definingForContent
 }
 
-function Za(n, e, t, r) {
+function tc(n, e, t, r) {
     if (!r.size) return n.deleteRange(e, t);
     let i = n.doc.resolve(e),
         s = n.doc.resolve(t);
     if (Ss(i, s, r)) return n.step(new ie(e, t, r));
     let o = Es(i, n.doc.resolve(t));
     o[o.length - 1] == 0 && o.pop();
     let l = -(i.depth + 1);
@@ -3051,29 +3059,29 @@
     for (let f = r.content, h = 0;; h++) {
         let p = f.firstChild;
         if (c.push(p), h == r.openStart) break;
         f = p.content
     }
     for (let f = d - 1; f >= 0; f--) {
         let h = c[f],
-            p = Xa(h.type);
+            p = ec(h.type);
         if (p && !h.sameMarkup(i.node(Math.abs(l) - 1))) d = f;
         else if (p || !h.type.isTextblock) break
     }
     for (let f = r.openStart; f >= 0; f--) {
         let h = (f + d + 1) % (r.openStart + 1),
             p = c[h];
         if (p)
             for (let m = 0; m < o.length; m++) {
                 let g = o[(m + a) % o.length],
                     k = !0;
                 g < 0 && (k = !1, g = -g);
                 let R = i.node(g - 1),
-                    H = i.index(g - 1);
-                if (R.canReplaceWith(H, H, p.type, p.marks)) return n.replace(i.before(g), k ? s.after(g) : t, new E(ws(r.content, 0, r.openStart, h), h, r.openEnd))
+                    $ = i.index(g - 1);
+                if (R.canReplaceWith($, $, p.type, p.marks)) return n.replace(i.before(g), k ? s.after(g) : t, new E(ws(r.content, 0, r.openStart, h), h, r.openEnd))
             }
     }
     let u = n.steps.length;
     for (let f = o.length - 1; f >= 0 && (n.replace(e, t, r), !(n.steps.length > u)); f--) {
         let h = o[f];
         h < 0 || (e = i.before(h), t = s.after(h))
     }
@@ -3083,28 +3091,28 @@
     if (e < t) {
         let s = n.firstChild;
         n = n.replaceChild(0, s.copy(ws(s.content, e + 1, t, r, s)))
     }
     if (e > r) {
         let s = i.contentMatchAt(0),
             o = s.fillBefore(n).append(n);
-        n = o.append(s.matchFragment(o).fillBefore(M.empty, !0))
+        n = o.append(s.matchFragment(o).fillBefore(w.empty, !0))
     }
     return n
 }
 
-function Qa(n, e, t, r) {
+function nc(n, e, t, r) {
     if (!r.isInline && e == t && n.doc.resolve(e).parent.content.size) {
-        let i = Ga(n.doc, e, r.type);
+        let i = Za(n.doc, e, r.type);
         i != null && (e = t = i)
     }
-    n.replaceRange(e, t, new E(M.from(r), 0, 0))
+    n.replaceRange(e, t, new E(w.from(r), 0, 0))
 }
 
-function ec(n, e, t) {
+function rc(n, e, t) {
     let r = n.doc.resolve(e),
         i = n.doc.resolve(t),
         s = Es(r, i);
     for (let o = 0; o < s.length; o++) {
         let l = s[o],
             a = o == s.length - 1;
         if (a && l == 0 || r.node(l).type.contentMatch.validEnd) return n.delete(r.start(l), i.end(l));
@@ -3132,15 +3140,15 @@
     apply(e) {
         let t = e.nodeAt(this.pos);
         if (!t) return Q.fail("No node at attribute step's position");
         let r = Object.create(null);
         for (let s in t.attrs) r[s] = t.attrs[s];
         r[this.attr] = this.value;
         let i = t.type.create(r, null, t.marks);
-        return Q.fromReplace(e, this.pos, this.pos + 1, new E(M.from(i), 0, t.isLeaf ? 0 : 1))
+        return Q.fromReplace(e, this.pos, this.pos + 1, new E(w.from(i), 0, t.isLeaf ? 0 : 1))
     }
     getMap() {
         return Ne.empty
     }
     invert(e) {
         return new n(this.pos, this.attr, e.nodeAt(this.pos).attrs[this.attr])
     }
@@ -3226,45 +3234,45 @@
         this.docs.push(this.doc), this.steps.push(e), this.mapping.appendMap(e.getMap()), this.doc = t
     }
     replace(e, t = e, r = E.empty) {
         let i = Vt(this.doc, e, t, r);
         return i && this.step(i), this
     }
     replaceWith(e, t, r) {
-        return this.replace(e, t, new E(M.from(r), 0, 0))
+        return this.replace(e, t, new E(w.from(r), 0, 0))
     }
     delete(e, t) {
         return this.replace(e, t, E.empty)
     }
     insert(e, t) {
         return this.replaceWith(e, e, t)
     }
     replaceRange(e, t, r) {
-        return Za(this, e, t, r), this
+        return tc(this, e, t, r), this
     }
     replaceRangeWith(e, t, r) {
-        return Qa(this, e, t, r), this
+        return nc(this, e, t, r), this
     }
     deleteRange(e, t) {
-        return ec(this, e, t), this
+        return rc(this, e, t), this
     }
     lift(e, t) {
-        return Ha(this, e, t), this
+        return Ja(this, e, t), this
     }
     join(e, t = 1) {
-        return _a(this, e, t), this
+        return Xa(this, e, t), this
     }
     wrap(e, t) {
-        return Ja(this, e, t), this
+        return Ka(this, e, t), this
     }
     setBlockType(e, t = e, r, i = null) {
-        return qa(this, e, t, r, i), this
+        return Ua(this, e, t, r, i), this
     }
     setNodeMarkup(e, t, r = null, i) {
-        return Ka(this, e, t, r, i), this
+        return Ga(this, e, t, r, i), this
     }
     setNodeAttribute(e, t, r) {
         return this.step(new hn(e, t, r)), this
     }
     setDocAttribute(e, t) {
         return this.step(new pn(e, t)), this
     }
@@ -3276,30 +3284,30 @@
             let r = this.doc.nodeAt(e);
             if (!r) throw new RangeError("No node at position " + e);
             if (t = t.isInSet(r.marks), !t) return this
         }
         return this.step(new $t(e, t)), this
     }
     split(e, t = 1, r) {
-        return Ua(this, e, t, r), this
+        return Ya(this, e, t, r), this
     }
     addMark(e, t, r) {
-        return Ba(this, e, t, r), this
+        return $a(this, e, t, r), this
     }
     removeMark(e, t, r) {
-        return Fa(this, e, t, r), this
+        return Ha(this, e, t, r), this
     }
     clearIncompatible(e, t, r) {
-        return za(this, e, t, r), this
+        return Va(this, e, t, r), this
     }
 };
-var cr = Object.create(null),
+var dr = Object.create(null),
     L = class {
         constructor(e, t, r) {
-            this.$anchor = e, this.$head = t, this.ranges = r || [new ur(e.min(t), e.max(t))]
+            this.$anchor = e, this.$head = t, this.ranges = r || [new fr(e.min(t), e.max(t))]
         }
         get anchor() {
             return this.$anchor.pos
         }
         get head() {
             return this.$head.pos
         }
@@ -3365,28 +3373,28 @@
             return xt(e, e, 0, 0, 1) || new fe(e)
         }
         static atEnd(e) {
             return xt(e, e, e.content.size, e.childCount, -1) || new fe(e)
         }
         static fromJSON(e, t) {
             if (!t || !t.type) throw new RangeError("Invalid input for Selection.fromJSON");
-            let r = cr[t.type];
+            let r = dr[t.type];
             if (!r) throw new RangeError(`No selection type ${t.type} defined`);
             return r.fromJSON(e, t)
         }
         static jsonID(e, t) {
-            if (e in cr) throw new RangeError("Duplicate use of selection JSON ID " + e);
-            return cr[e] = t, t.prototype.jsonID = e, t
+            if (e in dr) throw new RangeError("Duplicate use of selection JSON ID " + e);
+            return dr[e] = t, t.prototype.jsonID = e, t
         }
         getBookmark() {
             return P.between(this.$anchor, this.$head).getBookmark()
         }
     };
 L.prototype.visible = !0;
-var ur = class {
+var fr = class {
         constructor(e, t) {
             this.$from = e, this.$to = t
         }
     },
     Cs = !1;
 
 function Ts(n) {
@@ -3464,42 +3472,42 @@
             let {
                 deleted: r,
                 pos: i
             } = t.mapResult(this.anchor), s = e.resolve(i);
             return r ? L.near(s) : new n(s)
         }
         content() {
-            return new E(M.from(this.node), 0, 0)
+            return new E(w.from(this.node), 0, 0)
         }
         eq(e) {
             return e instanceof n && e.anchor == this.anchor
         }
         toJSON() {
             return {
                 type: "node",
                 anchor: this.anchor
             }
         }
         getBookmark() {
-            return new fr(this.anchor)
+            return new hr(this.anchor)
         }
         static fromJSON(e, t) {
             if (typeof t.anchor != "number") throw new RangeError("Invalid input for NodeSelection.fromJSON");
             return new n(e.resolve(t.anchor))
         }
         static create(e, t) {
             return new n(e.resolve(t))
         }
         static isSelectable(e) {
             return !e.isText && e.type.spec.selectable !== !1
         }
     };
 O.prototype.visible = !1;
 L.jsonID("node", O);
-var fr = class n {
+var hr = class n {
         constructor(e) {
             this.anchor = e
         }
         map(e) {
             let {
                 deleted: t,
                 pos: r
@@ -3534,19 +3542,19 @@
         map(e) {
             return new n(e)
         }
         eq(e) {
             return e instanceof n
         }
         getBookmark() {
-            return tc
+            return ic
         }
     };
 L.jsonID("all", fe);
-var tc = {
+var ic = {
     map() {
         return this
     },
     resolve(n) {
         return new fe(n)
     }
 };
@@ -3576,15 +3584,15 @@
     s.forEach((l, a, c, d) => {
         o == null && (o = d)
     }), n.setSelection(L.near(n.doc.resolve(o), t))
 }
 var vs = 1,
     mn = 2,
     Os = 4,
-    hr = class extends Ht {
+    pr = class extends Ht {
         constructor(e) {
             super(e.doc), this.curSelectionFor = 0, this.updated = 0, this.meta = Object.create(null), this.time = Date.now(), this.curSelection = e.selection, this.storedMarks = e.storedMarks
         }
         get selection() {
             return this.curSelectionFor < this.steps.length && (this.curSelection = this.curSelection.map(this.doc, this.mapping.slice(this.curSelectionFor)), this.curSelectionFor = this.steps.length), this.curSelection
         }
         setSelection(e) {
@@ -3660,15 +3668,15 @@
     return !e || !n ? n : n.bind(e)
 }
 var tt = class {
         constructor(e, t, r) {
             this.name = e, this.init = Ns(t.init, r), this.apply = Ns(t.apply, r)
         }
     },
-    nc = [new tt("doc", {
+    sc = [new tt("doc", {
         init(n) {
             return n.doc || n.schema.topNodeType.createAndFill()
         },
         apply(n) {
             return n.doc
         }
     }), new tt("selection", {
@@ -3691,15 +3699,15 @@
         },
         apply(n, e) {
             return n.scrolledIntoView ? e + 1 : e
         }
     })],
     jt = class {
         constructor(e, t) {
-            this.schema = e, this.plugins = [], this.pluginsByKey = Object.create(null), this.fields = nc.slice(), t && t.forEach(r => {
+            this.schema = e, this.plugins = [], this.pluginsByKey = Object.create(null), this.fields = sc.slice(), t && t.forEach(r => {
                 if (this.pluginsByKey[r.key]) throw new RangeError("Adding different instances of a keyed plugin (" + r.key + ")");
                 this.plugins.push(r), this.pluginsByKey[r.key] = r, r.spec.state && this.fields.push(new tt(r.key, r.spec.state, r))
             })
         }
     },
     yn = class n {
         constructor(e) {
@@ -3769,15 +3777,15 @@
             for (let i = 0; i < r.length; i++) {
                 let s = r[i];
                 t[s.name] = s.apply(e, this[s.name], this, t)
             }
             return t
         }
         get tr() {
-            return new hr(this)
+            return new pr(this)
         }
         static create(e) {
             let t = new jt(e.doc ? e.doc.type.schema : e.schema, e.plugins),
                 r = new n(t);
             for (let i = 0; i < t.fields.length; i++) r[t.fields[i].name] = t.fields[i].init(e, r);
             return r
         }
@@ -3841,18 +3849,18 @@
         constructor(e) {
             this.spec = e, this.props = {}, e.props && Ds(e.props, this, this.props), this.key = e.key ? e.key.key : Is("plugin")
         }
         getState(e) {
             return e[this.key]
         }
     },
-    dr = Object.create(null);
+    ur = Object.create(null);
 
 function Is(n) {
-    return n in dr ? n + "$" + ++dr[n] : (dr[n] = 0, n + "$")
+    return n in ur ? n + "$" + ++ur[n] : (ur[n] = 0, n + "$")
 }
 var Y = class {
     constructor(e = "key") {
         this.key = Is(e)
     }
     get(e) {
         return e.config.pluginsByKey[this.key]
@@ -3865,68 +3873,68 @@
         for (var e = 0;; e++)
             if (n = n.previousSibling, !n) return e
     },
     Kt = function(n) {
         let e = n.assignedSlot || n.parentNode;
         return e && e.nodeType == 11 ? e.host : e
     },
-    xr = null,
+    br = null,
     Pe = function(n, e, t) {
-        let r = xr || (xr = document.createRange());
+        let r = br || (br = document.createRange());
         return r.setEnd(n, t ?? n.nodeValue.length), r.setStart(n, e || 0), r
     },
-    rc = function() {
-        xr = null
+    oc = function() {
+        br = null
     },
     at = function(n, e, t, r) {
         return t && (Ps(n, e, t, r, -1) || Ps(n, e, t, r, 1))
     },
-    ic = /^(img|br|input|textarea|hr)$/i;
+    lc = /^(img|br|input|textarea|hr)$/i;
 
 function Ps(n, e, t, r, i) {
     for (;;) {
         if (n == t && e == r) return !0;
         if (e == (i < 0 ? 0 : Se(n))) {
             let s = n.parentNode;
-            if (!s || s.nodeType != 1 || Yt(n) || ic.test(n.nodeName) || n.contentEditable == "false") return !1;
+            if (!s || s.nodeType != 1 || Yt(n) || lc.test(n.nodeName) || n.contentEditable == "false") return !1;
             e = ee(n) + (i < 0 ? 0 : 1), n = s
         } else if (n.nodeType == 1) {
             if (n = n.childNodes[e + (i < 0 ? -1 : 0)], n.contentEditable == "false") return !1;
             e = i < 0 ? Se(n) : 0
         } else return !1
     }
 }
 
 function Se(n) {
     return n.nodeType == 3 ? n.nodeValue.length : n.childNodes.length
 }
 
-function sc(n, e) {
+function ac(n, e) {
     for (;;) {
         if (n.nodeType == 3 && e) return n;
         if (n.nodeType == 1 && e > 0) {
             if (n.contentEditable == "false") return null;
             n = n.childNodes[e - 1], e = Se(n)
         } else if (n.parentNode && !Yt(n)) e = ee(n), n = n.parentNode;
         else return null
     }
 }
 
-function oc(n, e) {
+function cc(n, e) {
     for (;;) {
         if (n.nodeType == 3 && e < n.nodeValue.length) return n;
         if (n.nodeType == 1 && e < n.childNodes.length) {
             if (n.contentEditable == "false") return null;
             n = n.childNodes[e], e = 0
         } else if (n.parentNode && !Yt(n)) e = ee(n) + 1, n = n.parentNode;
         else return null
     }
 }
 
-function lc(n, e, t) {
+function dc(n, e, t) {
     for (let r = e == 0, i = e == Se(n); r || i;) {
         if (n == t) return !0;
         let s = ee(n);
         if (n = n.parentNode, !n) return !1;
         r = r && s == 0, i = i && s == Se(n)
     }
 }
@@ -3941,21 +3949,21 @@
 };
 
 function nt(n, e) {
     let t = document.createEvent("Event");
     return t.initEvent("keydown", !0, !0), t.keyCode = n, t.key = t.code = e, t
 }
 
-function ac(n) {
+function uc(n) {
     let e = n.activeElement;
     for (; e && e.shadowRoot;) e = e.shadowRoot.activeElement;
     return e
 }
 
-function cc(n, e, t) {
+function fc(n, e, t) {
     if (n.caretPositionFromPoint) try {
         let r = n.caretPositionFromPoint(e, t);
         if (r) return {
             node: r.offsetNode,
             offset: r.offset
         }
     } catch {}
@@ -3966,33 +3974,33 @@
             offset: r.startOffset
         }
     }
 }
 var Me = typeof navigator < "u" ? navigator : null,
     Rs = typeof document < "u" ? document : null,
     Je = Me && Me.userAgent || "",
-    br = /Edge\/(\d+)/.exec(Je),
-    fo = /MSIE \d/.exec(Je),
-    kr = /Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(Je),
-    de = !!(fo || kr || br),
-    Ve = fo ? document.documentMode : kr ? +kr[1] : br ? +br[1] : 0,
+    kr = /Edge\/(\d+)/.exec(Je),
+    ho = /MSIE \d/.exec(Je),
+    Sr = /Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(Je),
+    de = !!(ho || Sr || kr),
+    Ve = ho ? document.documentMode : Sr ? +Sr[1] : kr ? +kr[1] : 0,
     ke = !de && /gecko\/(\d+)/i.test(Je);
 ke && +(/Firefox\/(\d+)/.exec(Je) || [0, 0])[1];
-var Sr = !de && /Chrome\/(\d+)/.exec(Je),
-    oe = !!Sr,
-    dc = Sr ? +Sr[1] : 0,
+var Mr = !de && /Chrome\/(\d+)/.exec(Je),
+    oe = !!Mr,
+    hc = Mr ? +Mr[1] : 0,
     le = !de && !!Me && /Apple Computer/.test(Me.vendor),
     wt = le && (/Mobile\/\w+/.test(Je) || !!Me && Me.maxTouchPoints > 2),
     me = wt || (Me ? /Mac/.test(Me.platform) : !1),
-    uc = Me ? /Win/.test(Me.platform) : !1,
+    pc = Me ? /Win/.test(Me.platform) : !1,
     be = /Android \d/.test(Je),
     Xt = !!Rs && "webkitFontSmoothing" in Rs.documentElement.style,
-    fc = Xt ? +(/\bAppleWebKit\/(\d+)/.exec(navigator.userAgent) || [0, 0])[1] : 0;
+    mc = Xt ? +(/\bAppleWebKit\/(\d+)/.exec(navigator.userAgent) || [0, 0])[1] : 0;
 
-function hc(n) {
+function gc(n) {
     let e = n.defaultView && n.defaultView.visualViewport;
     return e ? {
         left: 0,
         right: e.width,
         top: 0,
         bottom: e.height
     } : {
@@ -4003,15 +4011,15 @@
     }
 }
 
 function Ie(n, e) {
     return typeof n == "number" ? n : n[e]
 }
 
-function pc(n) {
+function yc(n) {
     let e = n.getBoundingClientRect(),
         t = e.width / n.offsetWidth || 1,
         r = e.height / n.offsetHeight || 1;
     return {
         left: e.left,
         right: e.left + n.clientWidth * t,
         top: e.top,
@@ -4023,15 +4031,15 @@
     let r = n.someProp("scrollThreshold") || 0,
         i = n.someProp("scrollMargin") || 5,
         s = n.dom.ownerDocument;
     for (let o = t || n.dom; o; o = Kt(o)) {
         if (o.nodeType != 1) continue;
         let l = o,
             a = l == s.body,
-            c = a ? hc(s) : pc(l),
+            c = a ? gc(s) : yc(l),
             d = 0,
             u = 0;
         if (e.top < c.top + Ie(r, "top") ? u = -(c.top - e.top + Ie(i, "top")) : e.bottom > c.bottom - Ie(r, "bottom") && (u = e.bottom - e.top > c.bottom - c.top ? e.top + Ie(i, "top") - c.top : e.bottom - c.bottom + Ie(i, "bottom")), e.left < c.left + Ie(r, "left") ? d = -(c.left - e.left + Ie(i, "left")) : e.right > c.right - Ie(r, "right") && (d = e.right - c.right + Ie(i, "right")), d || u)
             if (a) s.defaultView.scrollBy(d, u);
             else {
                 let f = l.scrollLeft,
                     h = l.scrollTop;
@@ -4044,15 +4052,15 @@
                     right: e.right - p,
                     bottom: e.bottom - m
                 }
             } if (a || /^(fixed|sticky)$/.test(getComputedStyle(o).position)) break
     }
 }
 
-function mc(n) {
+function xc(n) {
     let e = n.dom.getBoundingClientRect(),
         t = Math.max(0, e.top),
         r, i;
     for (let s = (e.left + e.right) / 2, o = t + 1; o < Math.min(innerHeight, e.bottom); o += 5) {
         let l = n.root.elementFromPoint(s, o);
         if (!l || l == n.dom || !n.dom.contains(l)) continue;
         let a = l.getBoundingClientRect();
@@ -4060,64 +4068,64 @@
             r = l, i = a.top;
             break
         }
     }
     return {
         refDOM: r,
         refTop: i,
-        stack: ho(n.dom)
+        stack: po(n.dom)
     }
 }
 
-function ho(n) {
+function po(n) {
     let e = [],
         t = n.ownerDocument;
     for (let r = n; r && (e.push({
             dom: r,
             top: r.scrollTop,
             left: r.scrollLeft
         }), n != t); r = Kt(r));
     return e
 }
 
-function gc({
+function bc({
     refDOM: n,
     refTop: e,
     stack: t
 }) {
     let r = n ? n.getBoundingClientRect().top : 0;
-    po(t, r == 0 ? 0 : r - e)
+    mo(t, r == 0 ? 0 : r - e)
 }
 
-function po(n, e) {
+function mo(n, e) {
     for (let t = 0; t < n.length; t++) {
         let {
             dom: r,
             top: i,
             left: s
         } = n[t];
         r.scrollTop != i + e && (r.scrollTop = i + e), r.scrollLeft != s && (r.scrollLeft = s)
     }
 }
 var bt = null;
 
-function yc(n) {
+function kc(n) {
     if (n.setActive) return n.setActive();
     if (bt) return n.focus(bt);
-    let e = ho(n);
+    let e = po(n);
     n.focus(bt == null ? {
         get preventScroll() {
             return bt = {
                 preventScroll: !0
             }, !0
         }
-    } : void 0), bt || (bt = !1, po(e, 0))
+    } : void 0), bt || (bt = !1, mo(e, 0))
 }
 
-function mo(n, e) {
+function go(n, e) {
     let t, r = 2e8,
         i, s = 0,
         o = e.top,
         l = e.top,
         a, c;
     for (let d = n.firstChild, u = 0; d; d = d.nextSibling, u++) {
         let f;
@@ -4139,115 +4147,115 @@
             } else p.top > e.top && !a && p.left <= e.left && p.right >= e.left && (a = d, c = {
                 left: Math.max(p.left, Math.min(p.right, e.left)),
                 top: p.top
             });
             !t && (e.left >= p.right && e.top >= p.top || e.left >= p.left && e.top >= p.bottom) && (s = u + 1)
         }
     }
-    return !t && a && (t = a, i = c, r = 0), t && t.nodeType == 3 ? xc(t, i) : !t || r && t.nodeType == 1 ? {
+    return !t && a && (t = a, i = c, r = 0), t && t.nodeType == 3 ? Sc(t, i) : !t || r && t.nodeType == 1 ? {
         node: n,
         offset: s
-    } : mo(t, i)
+    } : go(t, i)
 }
 
-function xc(n, e) {
+function Sc(n, e) {
     let t = n.nodeValue.length,
         r = document.createRange();
     for (let i = 0; i < t; i++) {
         r.setEnd(n, i + 1), r.setStart(n, i);
         let s = ze(r, 1);
-        if (s.top != s.bottom && Fr(e, s)) return {
+        if (s.top != s.bottom && zr(e, s)) return {
             node: n,
             offset: i + (e.left >= (s.left + s.right) / 2 ? 1 : 0)
         }
     }
     return {
         node: n,
         offset: 0
     }
 }
 
-function Fr(n, e) {
+function zr(n, e) {
     return n.left >= e.left - 1 && n.left <= e.right + 1 && n.top >= e.top - 1 && n.top <= e.bottom + 1
 }
 
-function bc(n, e) {
+function Mc(n, e) {
     let t = n.parentNode;
     return t && /^li$/i.test(t.nodeName) && e.left < n.getBoundingClientRect().left ? t : n
 }
 
-function kc(n, e, t) {
+function wc(n, e, t) {
     let {
         node: r,
         offset: i
-    } = mo(e, t), s = -1;
+    } = go(e, t), s = -1;
     if (r.nodeType == 1 && !r.firstChild) {
         let o = r.getBoundingClientRect();
         s = o.left != o.right && t.left > (o.left + o.right) / 2 ? 1 : -1
     }
     return n.docView.posFromDOM(r, i, s)
 }
 
-function Sc(n, e, t, r) {
+function Ec(n, e, t, r) {
     let i = -1;
     for (let s = e, o = !1; s != n.dom;) {
         let l = n.docView.nearestDesc(s, !0);
         if (!l) return null;
         if (l.dom.nodeType == 1 && (l.node.isBlock && l.parent && !o || !l.contentDOM)) {
             let a = l.dom.getBoundingClientRect();
             if (l.node.isBlock && l.parent && !o && (o = !0, a.left > r.left || a.top > r.top ? i = l.posBefore : (a.right < r.left || a.bottom < r.top) && (i = l.posAfter)), !l.contentDOM && i < 0 && !l.node.isText) return (l.node.isBlock ? r.top < (a.top + a.bottom) / 2 : r.left < (a.left + a.right) / 2) ? l.posBefore : l.posAfter
         }
         s = l.dom.parentNode
     }
     return i > -1 ? i : n.docView.posFromDOM(e, t, -1)
 }
 
-function go(n, e, t) {
+function yo(n, e, t) {
     let r = n.childNodes.length;
     if (r && t.top < t.bottom)
         for (let i = Math.max(0, Math.min(r - 1, Math.floor(r * (e.top - t.top) / (t.bottom - t.top)) - 2)), s = i;;) {
             let o = n.childNodes[s];
             if (o.nodeType == 1) {
                 let l = o.getClientRects();
                 for (let a = 0; a < l.length; a++) {
                     let c = l[a];
-                    if (Fr(e, c)) return go(o, e, c)
+                    if (zr(e, c)) return yo(o, e, c)
                 }
             }
             if ((s = (s + 1) % r) == i) break
         }
     return n
 }
 
-function Mc(n, e) {
+function Cc(n, e) {
     let t = n.dom.ownerDocument,
         r, i = 0,
-        s = cc(t, e.left, e.top);
+        s = fc(t, e.left, e.top);
     s && ({
         node: r,
         offset: i
     } = s);
     let o = (n.root.elementFromPoint ? n.root : t).elementFromPoint(e.left, e.top),
         l;
     if (!o || !n.dom.contains(o.nodeType != 1 ? o.parentNode : o)) {
         let c = n.dom.getBoundingClientRect();
-        if (!Fr(e, c) || (o = go(n.dom, e, c), !o)) return null
+        if (!zr(e, c) || (o = yo(n.dom, e, c), !o)) return null
     }
     if (le)
         for (let c = o; r && c; c = Kt(c)) c.draggable && (r = void 0);
-    if (o = bc(o, e), r) {
+    if (o = Mc(o, e), r) {
         if (ke && r.nodeType == 1 && (i = Math.min(i, r.childNodes.length), i < r.childNodes.length)) {
             let d = r.childNodes[i],
                 u;
             d.nodeName == "IMG" && (u = d.getBoundingClientRect()).right <= e.left && u.bottom > e.top && i++
         }
         let c;
-        Xt && i && r.nodeType == 1 && (c = r.childNodes[i - 1]).nodeType == 1 && c.contentEditable == "false" && c.getBoundingClientRect().top >= e.top && i--, r == n.dom && i == r.childNodes.length - 1 && r.lastChild.nodeType == 1 && e.top > r.lastChild.getBoundingClientRect().bottom ? l = n.state.doc.content.size : (i == 0 || r.nodeType != 1 || r.childNodes[i - 1].nodeName != "BR") && (l = Sc(n, r, i, e))
+        Xt && i && r.nodeType == 1 && (c = r.childNodes[i - 1]).nodeType == 1 && c.contentEditable == "false" && c.getBoundingClientRect().top >= e.top && i--, r == n.dom && i == r.childNodes.length - 1 && r.lastChild.nodeType == 1 && e.top > r.lastChild.getBoundingClientRect().bottom ? l = n.state.doc.content.size : (i == 0 || r.nodeType != 1 || r.childNodes[i - 1].nodeName != "BR") && (l = Ec(n, r, i, e))
     }
-    l == null && (l = kc(n, o, e));
+    l == null && (l = wc(n, o, e));
     let a = n.docView.nearestDesc(o, !0);
     return {
         pos: l,
         inside: a ? a.posAtStart - a.border : -1
     }
 }
 
@@ -4259,24 +4267,24 @@
     let t = n.getClientRects();
     if (t.length) {
         let r = t[e < 0 ? 0 : t.length - 1];
         if (Bs(r)) return r
     }
     return Array.prototype.find.call(t, Bs) || n.getBoundingClientRect()
 }
-var wc = /[\u0590-\u05f4\u0600-\u06ff\u0700-\u08ac]/;
+var Tc = /[\u0590-\u05f4\u0600-\u06ff\u0700-\u08ac]/;
 
-function yo(n, e, t) {
+function xo(n, e, t) {
     let {
         node: r,
         offset: i,
         atom: s
     } = n.docView.domFromPos(e, t < 0 ? -1 : 1), o = Xt || ke;
     if (r.nodeType == 3)
-        if (o && (wc.test(r.nodeValue) || (t < 0 ? !i : i == r.nodeValue.length))) {
+        if (o && (Tc.test(r.nodeValue) || (t < 0 ? !i : i == r.nodeValue.length))) {
             let a = ze(Pe(r, i, i), t);
             if (ke && i && /\s/.test(r.nodeValue[i - 1]) && i < r.nodeValue.length) {
                 let c = ze(Pe(r, i - 1, i - 1), -1);
                 if (c.top == a.top) {
                     let d = ze(Pe(r, i, i + 1), -1);
                     if (d.top != a.top) return Jt(d, d.left < c.left)
                 }
@@ -4286,21 +4294,21 @@
             let a = i,
                 c = i,
                 d = t < 0 ? 1 : -1;
             return t < 0 && !i ? (c++, d = -1) : t >= 0 && i == r.nodeValue.length ? (a--, d = 1) : t < 0 ? a-- : c++, Jt(ze(Pe(r, a, c), d), d < 0)
         } if (!n.state.doc.resolve(e - (s || 0)).parent.inlineContent) {
         if (s == null && i && (t < 0 || i == Se(r))) {
             let a = r.childNodes[i - 1];
-            if (a.nodeType == 1) return pr(a.getBoundingClientRect(), !1)
+            if (a.nodeType == 1) return mr(a.getBoundingClientRect(), !1)
         }
         if (s == null && i < Se(r)) {
             let a = r.childNodes[i];
-            if (a.nodeType == 1) return pr(a.getBoundingClientRect(), !0)
+            if (a.nodeType == 1) return mr(a.getBoundingClientRect(), !0)
         }
-        return pr(r.getBoundingClientRect(), t >= 0)
+        return mr(r.getBoundingClientRect(), t >= 0)
     }
     if (s == null && i && (t < 0 || i == Se(r))) {
         let a = r.childNodes[i - 1],
             c = a.nodeType == 3 ? Pe(a, Se(a) - (o ? 0 : 1)) : a.nodeType == 1 && (a.nodeName != "BR" || !a.nextSibling) ? a : null;
         if (c) return Jt(ze(c, 1), !1)
     }
     if (s == null && i < Se(r)) {
@@ -4319,78 +4327,78 @@
         top: n.top,
         bottom: n.bottom,
         left: t,
         right: t
     }
 }
 
-function pr(n, e) {
+function mr(n, e) {
     if (n.height == 0) return n;
     let t = e ? n.top : n.bottom;
     return {
         top: t,
         bottom: t,
         left: n.left,
         right: n.right
     }
 }
 
-function xo(n, e, t) {
+function bo(n, e, t) {
     let r = n.state,
         i = n.root.activeElement;
     r != e && n.updateState(e), i != n.dom && n.focus();
     try {
         return t()
     } finally {
         r != e && n.updateState(r), i != n.dom && i && i.focus()
     }
 }
 
-function Ec(n, e, t) {
+function Ac(n, e, t) {
     let r = e.selection,
         i = t == "up" ? r.$from : r.$to;
-    return xo(n, e, () => {
+    return bo(n, e, () => {
         let {
             node: s
         } = n.docView.domFromPos(i.pos, t == "up" ? -1 : 1);
         for (;;) {
             let l = n.docView.nearestDesc(s, !0);
             if (!l) break;
             if (l.node.isBlock) {
                 s = l.contentDOM || l.dom;
                 break
             }
             s = l.dom.parentNode
         }
-        let o = yo(n, i.pos, 1);
+        let o = xo(n, i.pos, 1);
         for (let l = s.firstChild; l; l = l.nextSibling) {
             let a;
             if (l.nodeType == 1) a = l.getClientRects();
             else if (l.nodeType == 3) a = Pe(l, 0, l.nodeValue.length).getClientRects();
             else continue;
             for (let c = 0; c < a.length; c++) {
                 let d = a[c];
                 if (d.bottom > d.top + 1 && (t == "up" ? o.top - d.top > (d.bottom - o.top) * 2 : d.bottom - o.bottom > (o.bottom - d.top) * 2)) return !1
             }
         }
         return !0
     })
 }
-var Cc = /[\u0590-\u08ac]/;
+var vc = /[\u0590-\u08ac]/;
 
-function Tc(n, e, t) {
+function Oc(n, e, t) {
     let {
         $head: r
     } = e.selection;
     if (!r.parent.isTextblock) return !1;
     let i = r.parentOffset,
         s = !i,
         o = i == r.parent.content.size,
         l = n.domSelection();
-    return !Cc.test(r.parent.textContent) || !l.modify ? t == "left" || t == "backward" ? s : o : xo(n, e, () => {
+    return !vc.test(r.parent.textContent) || !l.modify ? t == "left" || t == "backward" ? s : o : bo(n, e, () => {
         let {
             focusNode: a,
             focusOffset: c,
             anchorNode: d,
             anchorOffset: u
         } = n.domSelectionRange(), f = l.caretBidiLevel;
         l.modify("move", t, "character");
@@ -4406,16 +4414,16 @@
         return f != null && (l.caretBidiLevel = f), g
     })
 }
 var Fs = null,
     zs = null,
     $s = !1;
 
-function Ac(n, e, t) {
-    return Fs == e && zs == t ? $s : (Fs = e, zs = t, $s = t == "up" || t == "down" ? Ec(n, e, t) : Tc(n, e, t))
+function Nc(n, e, t) {
+    return Fs == e && zs == t ? $s : (Fs = e, zs = t, $s = t == "up" || t == "down" ? Ac(n, e, t) : Oc(n, e, t))
 }
 var ge = 0,
     Hs = 1,
     rt = 2,
     we = 3,
     ct = class {
         constructor(e, t, r, i) {
@@ -4777,15 +4785,15 @@
         get domAtom() {
             return !0
         }
         get side() {
             return this.widget.type.side
         }
     },
-    Mr = class extends ct {
+    wr = class extends ct {
         constructor(e, t, r, i) {
             super(e, [], t, null), this.textDOM = r, this.text = i
         }
         get size() {
             return this.text.length
         }
         localPosFromDOM(e, t) {
@@ -4827,15 +4835,15 @@
                 r.dirty < this.dirty && (r.dirty = this.dirty), this.dirty = ge
             }
         }
         slice(e, t, r) {
             let i = n.create(this.parent, this.mark, !0, r),
                 s = this.children,
                 o = this.size;
-            t < o && (s = Ar(s, t, o, r)), e > 0 && (s = Ar(s, 0, e, r));
+            t < o && (s = vr(s, t, o, r)), e > 0 && (s = vr(s, 0, e, r));
             for (let l = 0; l < s.length; l++) s[l].parent = i;
             return i.children = s, i
         }
     },
     je = class n extends ct {
         constructor(e, t, r, i, s, o, l, a, c) {
             super(e, [], s, o), this.node = t, this.outerDeco = r, this.innerDeco = i, this.nodeDOM = l
@@ -4853,15 +4861,15 @@
                 else if (d.nodeType != 3) throw new RangeError("Text must be rendered as a DOM text node")
             } else d || ({
                 dom: d,
                 contentDOM: u
             } = Oe.renderSpec(document, t.type.spec.toDOM(t)));
             !u && !t.isText && d.nodeName != "BR" && (d.hasAttribute("contenteditable") || (d.contentEditable = "false"), t.type.spec.draggable && (d.draggable = !0));
             let f = d;
-            return d = So(d, r, t), c ? a = new wr(e, t, r, i, d, u || null, f, c, s, o + 1) : t.isText ? new bn(e, t, r, i, d, f, s) : new n(e, t, r, i, d, u || null, f, s, o + 1)
+            return d = Mo(d, r, t), c ? a = new Er(e, t, r, i, d, u || null, f, c, s, o + 1) : t.isText ? new bn(e, t, r, i, d, f, s) : new n(e, t, r, i, d, u || null, f, s, o + 1)
         }
         parseRule() {
             if (this.node.type.spec.reparseInView) return null;
             let e = {
                 node: this.node.type.name,
                 attrs: this.node.attrs
             };
@@ -4871,53 +4879,53 @@
                 for (let t = this.children.length - 1; t >= 0; t--) {
                     let r = this.children[t];
                     if (this.dom.contains(r.dom.parentNode)) {
                         e.contentElement = r.dom.parentNode;
                         break
                     }
                 }
-                e.contentElement || (e.getContent = () => M.empty)
+                e.contentElement || (e.getContent = () => w.empty)
             }
             return e
         }
         matchesNode(e, t, r) {
-            return this.dirty == ge && e.eq(this.node) && Cr(t, this.outerDeco) && r.eq(this.innerDeco)
+            return this.dirty == ge && e.eq(this.node) && Tr(t, this.outerDeco) && r.eq(this.innerDeco)
         }
         get size() {
             return this.node.nodeSize
         }
         get border() {
             return this.node.isLeaf ? 0 : 1
         }
         updateChildren(e, t) {
             let r = this.node.inlineContent,
                 i = t,
                 s = e.composing ? this.localCompositionInfo(e, t) : null,
                 o = s && s.pos > -1 ? s : null,
                 l = s && s.pos < 0,
-                a = new Tr(this, o && o.node, e);
-            Dc(this.node, this.innerDeco, (c, d, u) => {
+                a = new Ar(this, o && o.node, e);
+            Rc(this.node, this.innerDeco, (c, d, u) => {
                 c.spec.marks ? a.syncToMarks(c.spec.marks, r, e) : c.type.side >= 0 && !u && a.syncToMarks(d == this.node.childCount ? j.none : this.node.child(d).marks, r, e), a.placeWidget(c, e, i)
             }, (c, d, u, f) => {
                 a.syncToMarks(c.marks, r, e);
                 let h;
                 a.findNodeMatch(c, d, u, f) || l && e.state.selection.from > i && e.state.selection.to < i + c.nodeSize && (h = a.findIndexWithChild(s.node)) > -1 && a.updateNodeAt(c, d, u, h, e) || a.updateNextNode(c, d, u, e, f, i) || a.addNode(c, d, u, e, i), i += c.nodeSize
-            }), a.syncToMarks([], r, e), this.node.isTextblock && a.addTextblockHacks(), a.destroyRest(), (a.changed || this.dirty == rt) && (o && this.protectLocalComposition(e, o), bo(this.contentDOM, this.children, e), wt && Ic(this.dom))
+            }), a.syncToMarks([], r, e), this.node.isTextblock && a.addTextblockHacks(), a.destroyRest(), (a.changed || this.dirty == rt) && (o && this.protectLocalComposition(e, o), ko(this.contentDOM, this.children, e), wt && Lc(this.dom))
         }
         localCompositionInfo(e, t) {
             let {
                 from: r,
                 to: i
             } = e.state.selection;
             if (!(e.state.selection instanceof P) || r < t || i > t + this.node.content.size) return null;
             let s = e.input.compositionNode;
             if (!s || !this.dom.contains(s.parentNode)) return null;
             if (this.node.inlineContent) {
                 let o = s.nodeValue,
-                    l = Pc(this.node.content, o, r - t, i - t);
+                    l = Bc(this.node.content, o, r - t, i - t);
                 return l < 0 ? null : {
                     node: s,
                     pos: l,
                     text: o
                 }
             } else return {
                 node: s,
@@ -4933,42 +4941,42 @@
             if (this.getDesc(t)) return;
             let s = t;
             for (; s.parentNode != this.contentDOM; s = s.parentNode) {
                 for (; s.previousSibling;) s.parentNode.removeChild(s.previousSibling);
                 for (; s.nextSibling;) s.parentNode.removeChild(s.nextSibling);
                 s.pmViewDesc && (s.pmViewDesc = void 0)
             }
-            let o = new Mr(this, s, t, i);
-            e.input.compositionNodes.push(o), this.children = Ar(this.children, r, r + i.length, e, o)
+            let o = new wr(this, s, t, i);
+            e.input.compositionNodes.push(o), this.children = vr(this.children, r, r + i.length, e, o)
         }
         update(e, t, r, i) {
             return this.dirty == we || !e.sameMarkup(this.node) ? !1 : (this.updateInner(e, t, r, i), !0)
         }
         updateInner(e, t, r, i) {
             this.updateOuterDeco(t), this.node = e, this.innerDeco = r, this.contentDOM && this.updateChildren(i, this.posAtStart), this.dirty = ge
         }
         updateOuterDeco(e) {
-            if (Cr(e, this.outerDeco)) return;
+            if (Tr(e, this.outerDeco)) return;
             let t = this.nodeDOM.nodeType != 1,
                 r = this.dom;
-            this.dom = ko(this.dom, this.nodeDOM, Er(this.outerDeco, this.node, t), Er(e, this.node, t)), this.dom != r && (r.pmViewDesc = void 0, this.dom.pmViewDesc = this), this.outerDeco = e
+            this.dom = So(this.dom, this.nodeDOM, Cr(this.outerDeco, this.node, t), Cr(e, this.node, t)), this.dom != r && (r.pmViewDesc = void 0, this.dom.pmViewDesc = this), this.outerDeco = e
         }
         selectNode() {
             this.nodeDOM.nodeType == 1 && this.nodeDOM.classList.add("ProseMirror-selectednode"), (this.contentDOM || !this.node.type.spec.draggable) && (this.dom.draggable = !0)
         }
         deselectNode() {
             this.nodeDOM.nodeType == 1 && this.nodeDOM.classList.remove("ProseMirror-selectednode"), (this.contentDOM || !this.node.type.spec.draggable) && this.dom.removeAttribute("draggable")
         }
         get domAtom() {
             return this.node.isAtom
         }
     };
 
 function Vs(n, e, t, r, i) {
-    So(r, e, n);
+    Mo(r, e, n);
     let s = new je(void 0, n, e, t, r, r, r, i, 0);
     return s.contentDOM && s.updateChildren(i, 0), s
 }
 var bn = class n extends je {
         constructor(e, t, r, i, s, o, l) {
             super(e, t, r, i, s, null, o, l, 0)
         }
@@ -5027,15 +5035,15 @@
         get domAtom() {
             return !0
         }
         get ignoreForCoords() {
             return this.dom.nodeName == "IMG"
         }
     },
-    wr = class extends je {
+    Er = class extends je {
         constructor(e, t, r, i, s, o, l, a, c, d) {
             super(e, t, r, i, s, o, l, c, d), this.spec = a
         }
         update(e, t, r, i) {
             if (this.dirty == we) return !1;
             if (this.spec.update) {
                 let s = this.spec.update(e, t, r);
@@ -5058,39 +5066,39 @@
             return this.spec.stopEvent ? this.spec.stopEvent(e) : !1
         }
         ignoreMutation(e) {
             return this.spec.ignoreMutation ? this.spec.ignoreMutation(e) : super.ignoreMutation(e)
         }
     };
 
-function bo(n, e, t) {
+function ko(n, e, t) {
     let r = n.firstChild,
         i = !1;
     for (let s = 0; s < e.length; s++) {
         let o = e[s],
             l = o.dom;
         if (l.parentNode == n) {
             for (; l != r;) r = js(r), i = !0;
             r = r.nextSibling
         } else i = !0, n.insertBefore(l, r);
         if (o instanceof Et) {
             let a = r ? r.previousSibling : n.lastChild;
-            bo(o.contentDOM, o.children, t), r = a ? a.nextSibling : n.firstChild
+            ko(o.contentDOM, o.children, t), r = a ? a.nextSibling : n.firstChild
         }
     }
     for (; r;) r = js(r), i = !0;
     i && t.trackWrites == n && (t.trackWrites = null)
 }
 var qt = function(n) {
     n && (this.nodeName = n)
 };
 qt.prototype = Object.create(null);
 var it = [new qt];
 
-function Er(n, e, t) {
+function Cr(n, e, t) {
     if (n.length == 0) return it;
     let r = t ? it[0] : new qt,
         i = [r];
     for (let s = 0; s < n.length; s++) {
         let o = n[s].type.attrs;
         if (o) {
             o.nodeName && i.push(r = new qt(o.nodeName));
@@ -5099,30 +5107,30 @@
                 a != null && (t && i.length == 1 && i.push(r = new qt(e.isInline ? "span" : "div")), l == "class" ? r.class = (r.class ? r.class + " " : "") + a : l == "style" ? r.style = (r.style ? r.style + ";" : "") + a : l != "nodeName" && (r[l] = a))
             }
         }
     }
     return i
 }
 
-function ko(n, e, t, r) {
+function So(n, e, t, r) {
     if (t == it && r == it) return e;
     let i = e;
     for (let s = 0; s < r.length; s++) {
         let o = r[s],
             l = t[s];
         if (s) {
             let a;
             l && l.nodeName == o.nodeName && i != n && (a = i.parentNode) && a.nodeName.toLowerCase() == o.nodeName || (a = document.createElement(o.nodeName), a.pmIsDeco = !0, a.appendChild(i), l = it[0]), i = a
         }
-        vc(i, l || it[0], o)
+        Dc(i, l || it[0], o)
     }
     return i
 }
 
-function vc(n, e, t) {
+function Dc(n, e, t) {
     for (let r in e) r != "class" && r != "style" && r != "nodeName" && !(r in t) && n.removeAttribute(r);
     for (let r in t) r != "class" && r != "style" && r != "nodeName" && t[r] != e[r] && n.setAttribute(r, t[r]);
     if (e.class != t.class) {
         let r = e.class ? e.class.split(" ").filter(Boolean) : [],
             i = t.class ? t.class.split(" ").filter(Boolean) : [];
         for (let s = 0; s < r.length; s++) i.indexOf(r[s]) == -1 && n.classList.remove(r[s]);
         for (let s = 0; s < i.length; s++) r.indexOf(i[s]) == -1 && n.classList.add(i[s]);
@@ -5134,32 +5142,32 @@
                 i;
             for (; i = r.exec(e.style);) n.style.removeProperty(i[1])
         }
         t.style && (n.style.cssText += t.style)
     }
 }
 
-function So(n, e, t) {
-    return ko(n, n, it, Er(e, t, n.nodeType != 1))
+function Mo(n, e, t) {
+    return So(n, n, it, Cr(e, t, n.nodeType != 1))
 }
 
-function Cr(n, e) {
+function Tr(n, e) {
     if (n.length != e.length) return !1;
     for (let t = 0; t < n.length; t++)
         if (!n[t].type.eq(e[t].type)) return !1;
     return !0
 }
 
 function js(n) {
     let e = n.nextSibling;
     return n.parentNode.removeChild(n), e
 }
-var Tr = class {
+var Ar = class {
     constructor(e, t, r) {
-        this.lock = t, this.view = r, this.index = 0, this.stack = [], this.changed = !1, this.top = e, this.preMatch = Oc(e.node.content, e)
+        this.lock = t, this.view = r, this.index = 0, this.stack = [], this.changed = !1, this.top = e, this.preMatch = Ic(e.node.content, e)
     }
     destroyBetween(e, t) {
         if (e != t) {
             for (let r = e; r < t; r++) this.top.children[r].destroy();
             this.top.children.splice(e, t - e), this.changed = !0
         }
     }
@@ -5226,15 +5234,15 @@
     updateNextNode(e, t, r, i, s, o) {
         for (let l = this.index; l < this.top.children.length; l++) {
             let a = this.top.children[l];
             if (a instanceof je) {
                 let c = this.preMatch.matched.get(a);
                 if (c != null && c != s) return !1;
                 let d = a.dom,
-                    u, f = this.isLocked(d) && !(e.isText && a.node && a.node.isText && a.nodeDOM.nodeValue == e.text && a.dirty != we && Cr(t, a.outerDeco));
+                    u, f = this.isLocked(d) && !(e.isText && a.node && a.node.isText && a.nodeDOM.nodeValue == e.text && a.dirty != we && Tr(t, a.outerDeco));
                 if (!f && a.update(e, t, r, i)) return this.destroyBetween(this.index, l), a.dom != d && (this.changed = !0), this.index++, !0;
                 if (!f && (u = this.recreateWrapper(a, e, t, r, i, o))) return this.top.children[this.index] = u, u.contentDOM && (u.dirty = rt, u.updateChildren(i, o + 1), u.dirty = ge), this.changed = !0, this.index++, !0;
                 break
             }
         }
         return !1
     }
@@ -5275,15 +5283,15 @@
         }
     }
     isLocked(e) {
         return this.lock && (e == this.lock || e.nodeType == 1 && e.contains(this.lock.parentNode))
     }
 };
 
-function Oc(n, e) {
+function Ic(n, e) {
     let t = e,
         r = t.children.length,
         i = n.childCount,
         s = new Map,
         o = [];
     e: for (; i > 0;) {
         let l;
@@ -5307,19 +5315,19 @@
     return {
         index: i,
         matched: s,
         matches: o.reverse()
     }
 }
 
-function Nc(n, e) {
+function Pc(n, e) {
     return n.type.side - e.type.side
 }
 
-function Dc(n, e, t, r) {
+function Rc(n, e, t, r) {
     let i = e.locals(n),
         s = 0;
     if (i.length == 0) {
         for (let c = 0; c < n.childCount; c++) {
             let d = n.child(c);
             r(d, i, e.forChild(s, d), c), s += d.nodeSize
         }
@@ -5332,15 +5340,15 @@
         let d, u;
         for (; o < i.length && i[o].to == s;) {
             let g = i[o++];
             g.widget && (d ? (u || (u = [d])).push(g) : d = g)
         }
         if (d)
             if (u) {
-                u.sort(Nc);
+                u.sort(Pc);
                 for (let g = 0; g < u.length; g++) t(u[g], c, !!a)
             } else t(d, c, !!a);
         let f, h;
         if (a) h = -1, f = a, a = null;
         else if (c < n.childCount) h = c, f = n.child(c++);
         else break;
         for (let g = 0; g < l.length; g++) l[g].to <= s && l.splice(g--, 1);
@@ -5354,22 +5362,22 @@
         } else
             for (; o < i.length && i[o].to < p;) o++;
         let m = f.isInline && !f.isLeaf ? l.filter(g => !g.inline) : l.slice();
         r(f, m, e.forChild(s, f), h), s = p
     }
 }
 
-function Ic(n) {
+function Lc(n) {
     if (n.nodeName == "UL" || n.nodeName == "OL") {
         let e = n.style.cssText;
         n.style.cssText = e + "; list-style: square !important", window.getComputedStyle(n).listStyle, n.style.cssText = e
     }
 }
 
-function Pc(n, e, t, r) {
+function Bc(n, e, t, r) {
     for (let i = 0, s = 0; i < n.childCount && s <= r;) {
         let o = n.child(i++),
             l = s;
         if (s += o.nodeSize, !o.isText) continue;
         let a = o.text;
         for (; i < n.childCount;) {
             let c = n.child(i++);
@@ -5382,159 +5390,159 @@
             if (c >= 0 && c + e.length + l >= t) return l + c;
             if (t == r && a.length >= r + e.length - l && a.slice(r - l, r - l + e.length) == e) return r
         }
     }
     return -1
 }
 
-function Ar(n, e, t, r, i) {
+function vr(n, e, t, r, i) {
     let s = [];
     for (let o = 0, l = 0; o < n.length; o++) {
         let a = n[o],
             c = l,
             d = l += a.size;
         c >= t || d <= e ? s.push(a) : (c < e && s.push(a.slice(0, e - c, r)), i && (s.push(i), i = void 0), d > t && s.push(a.slice(t - c, a.size, r)))
     }
     return s
 }
 
-function zr(n, e = null) {
+function $r(n, e = null) {
     let t = n.domSelectionRange(),
         r = n.state.doc;
     if (!t.focusNode) return null;
     let i = n.docView.nearestDesc(t.focusNode),
         s = i && i.size == 0,
         o = n.docView.posFromDOM(t.focusNode, t.focusOffset, 1);
     if (o < 0) return null;
     let l = r.resolve(o),
         a, c;
     if (vn(t)) {
         for (a = l; i && !i.node;) i = i.parent;
         let d = i.node;
-        if (i && d.isAtom && O.isSelectable(d) && i.parent && !(d.isInline && lc(t.focusNode, t.focusOffset, i.dom))) {
+        if (i && d.isAtom && O.isSelectable(d) && i.parent && !(d.isInline && dc(t.focusNode, t.focusOffset, i.dom))) {
             let u = i.posBefore;
             c = new O(o == u ? l : r.resolve(u))
         }
     } else {
         let d = n.docView.posFromDOM(t.anchorNode, t.anchorOffset, 1);
         if (d < 0) return null;
         a = r.resolve(d)
     }
     if (!c) {
         let d = e == "pointer" || n.state.selection.head < l.pos && !s ? 1 : -1;
-        c = $r(n, a, l, d)
+        c = Hr(n, a, l, d)
     }
     return c
 }
 
-function Mo(n) {
-    return n.editable ? n.hasFocus() : Eo(n) && document.activeElement && document.activeElement.contains(n.dom)
+function wo(n) {
+    return n.editable ? n.hasFocus() : Co(n) && document.activeElement && document.activeElement.contains(n.dom)
 }
 
 function Re(n, e = !1) {
     let t = n.state.selection;
-    if (wo(n, t), !!Mo(n)) {
+    if (Eo(n, t), !!wo(n)) {
         if (!e && n.input.mouseDown && n.input.mouseDown.allowDefault && oe) {
             let r = n.domSelectionRange(),
                 i = n.domObserver.currentSelection;
             if (r.anchorNode && i.anchorNode && at(r.anchorNode, r.anchorOffset, i.anchorNode, i.anchorOffset)) {
                 n.input.mouseDown.delayedSelectionSync = !0, n.domObserver.setCurSelection();
                 return
             }
         }
-        if (n.domObserver.disconnectSelection(), n.cursorWrapper) Lc(n);
+        if (n.domObserver.disconnectSelection(), n.cursorWrapper) zc(n);
         else {
             let {
                 anchor: r,
                 head: i
             } = t, s, o;
-            Js && !(t instanceof P) && (t.$from.parent.inlineContent || (s = qs(n, t.from)), !t.empty && !t.$from.parent.inlineContent && (o = qs(n, t.to))), n.docView.setSelection(r, i, n.root, e), Js && (s && Ws(s), o && Ws(o)), t.visible ? n.dom.classList.remove("ProseMirror-hideselection") : (n.dom.classList.add("ProseMirror-hideselection"), "onselectionchange" in document && Rc(n))
+            Js && !(t instanceof P) && (t.$from.parent.inlineContent || (s = qs(n, t.from)), !t.empty && !t.$from.parent.inlineContent && (o = qs(n, t.to))), n.docView.setSelection(r, i, n.root, e), Js && (s && Ws(s), o && Ws(o)), t.visible ? n.dom.classList.remove("ProseMirror-hideselection") : (n.dom.classList.add("ProseMirror-hideselection"), "onselectionchange" in document && Fc(n))
         }
         n.domObserver.setCurSelection(), n.domObserver.connectSelection()
     }
 }
-var Js = le || oe && dc < 63;
+var Js = le || oe && hc < 63;
 
 function qs(n, e) {
     let {
         node: t,
         offset: r
     } = n.docView.domFromPos(e, 0), i = r < t.childNodes.length ? t.childNodes[r] : null, s = r ? t.childNodes[r - 1] : null;
-    if (le && i && i.contentEditable == "false") return mr(i);
+    if (le && i && i.contentEditable == "false") return gr(i);
     if ((!i || i.contentEditable == "false") && (!s || s.contentEditable == "false")) {
-        if (i) return mr(i);
-        if (s) return mr(s)
+        if (i) return gr(i);
+        if (s) return gr(s)
     }
 }
 
-function mr(n) {
+function gr(n) {
     return n.contentEditable = "true", le && n.draggable && (n.draggable = !1, n.wasDraggable = !0), n
 }
 
 function Ws(n) {
     n.contentEditable = "false", n.wasDraggable && (n.draggable = !0, n.wasDraggable = null)
 }
 
-function Rc(n) {
+function Fc(n) {
     let e = n.dom.ownerDocument;
     e.removeEventListener("selectionchange", n.input.hideSelectionGuard);
     let t = n.domSelectionRange(),
         r = t.anchorNode,
         i = t.anchorOffset;
     e.addEventListener("selectionchange", n.input.hideSelectionGuard = () => {
         (t.anchorNode != r || t.anchorOffset != i) && (e.removeEventListener("selectionchange", n.input.hideSelectionGuard), setTimeout(() => {
-            (!Mo(n) || n.state.selection.visible) && n.dom.classList.remove("ProseMirror-hideselection")
+            (!wo(n) || n.state.selection.visible) && n.dom.classList.remove("ProseMirror-hideselection")
         }, 20))
     })
 }
 
-function Lc(n) {
+function zc(n) {
     let e = n.domSelection(),
         t = document.createRange(),
         r = n.cursorWrapper.dom,
         i = r.nodeName == "IMG";
     i ? t.setEnd(r.parentNode, ee(r) + 1) : t.setEnd(r, 0), t.collapse(!1), e.removeAllRanges(), e.addRange(t), !i && !n.state.selection.visible && de && Ve <= 11 && (r.disabled = !0, r.disabled = !1)
 }
 
-function wo(n, e) {
+function Eo(n, e) {
     if (e instanceof O) {
         let t = n.docView.descAt(e.from);
         t != n.lastSelectedViewDesc && (Ks(n), t && t.selectNode(), n.lastSelectedViewDesc = t)
     } else Ks(n)
 }
 
 function Ks(n) {
     n.lastSelectedViewDesc && (n.lastSelectedViewDesc.parent && n.lastSelectedViewDesc.deselectNode(), n.lastSelectedViewDesc = void 0)
 }
 
-function $r(n, e, t, r) {
+function Hr(n, e, t, r) {
     return n.someProp("createSelectionBetween", i => i(n, e, t)) || P.between(e, t, r)
 }
 
 function Us(n) {
-    return n.editable && !n.hasFocus() ? !1 : Eo(n)
+    return n.editable && !n.hasFocus() ? !1 : Co(n)
 }
 
-function Eo(n) {
+function Co(n) {
     let e = n.domSelectionRange();
     if (!e.anchorNode) return !1;
     try {
         return n.dom.contains(e.anchorNode.nodeType == 3 ? e.anchorNode.parentNode : e.anchorNode) && (n.editable || n.dom.contains(e.focusNode.nodeType == 3 ? e.focusNode.parentNode : e.focusNode))
     } catch {
         return !1
     }
 }
 
-function Bc(n) {
+function $c(n) {
     let e = n.docView.domFromPos(n.state.selection.anchor, 0),
         t = n.domSelectionRange();
     return at(e.node, e.offset, t.anchorNode, t.anchorOffset)
 }
 
-function vr(n, e) {
+function Or(n, e) {
     let {
         $anchor: t,
         $head: r
     } = n.selection, i = e > 0 ? t.max(r) : t.min(r), s = i.parent.inlineContent ? i.depth ? n.doc.resolve(e > 0 ? i.after() : i.before()) : null : i;
     return s && L.findFrom(s, e)
 }
 
@@ -5550,29 +5558,29 @@
                 $head: i
             } = r, s = i.textOffset ? null : e < 0 ? i.nodeBefore : i.nodeAfter;
             if (!s || s.isText || !s.isLeaf) return !1;
             let o = n.state.doc.resolve(i.pos + s.nodeSize * (e < 0 ? -1 : 1));
             return $e(n, new P(r.$anchor, o))
         } else if (r.empty) {
         if (n.endOfTextblock(e > 0 ? "forward" : "backward")) {
-            let i = vr(n.state, e);
+            let i = Or(n.state, e);
             return i && i instanceof O ? $e(n, i) : !1
         } else if (!(me && t.indexOf("m") > -1)) {
             let i = r.$head,
                 s = i.textOffset ? null : e < 0 ? i.nodeBefore : i.nodeAfter,
                 o;
             if (!s || s.isText) return !1;
             let l = e < 0 ? i.pos - s.nodeSize : i.pos;
             return s.isAtom || (o = n.docView.descAt(l)) && !o.contentDOM ? O.isSelectable(s) ? $e(n, new O(e < 0 ? n.state.doc.resolve(i.pos - s.nodeSize) : i)) : Xt ? $e(n, new P(n.state.doc.resolve(e < 0 ? l : l + s.nodeSize))) : !1 : !1
         }
     } else return !1;
     else {
         if (r instanceof O && r.node.isInline) return $e(n, new P(e > 0 ? r.$to : r.$from));
         {
-            let i = vr(n.state, e);
+            let i = Or(n.state, e);
             return i ? $e(n, i) : !1
         }
     }
 }
 
 function Sn(n) {
     return n.nodeType == 3 ? n.nodeValue.length : n.childNodes.length
@@ -5580,18 +5588,18 @@
 
 function Wt(n, e) {
     let t = n.pmViewDesc;
     return t && t.size == 0 && (e < 0 || n.nextSibling || n.nodeName != "BR")
 }
 
 function kt(n, e) {
-    return e < 0 ? Fc(n) : zc(n)
+    return e < 0 ? Hc(n) : Vc(n)
 }
 
-function Fc(n) {
+function Hc(n) {
     let e = n.domSelectionRange(),
         t = e.focusNode,
         r = e.focusOffset;
     if (!t) return;
     let i, s, o = !1;
     for (ke && t.nodeType == 1 && r < Sn(t) && Wt(t.childNodes[r], -1) && (o = !0);;)
         if (r > 0) {
@@ -5599,83 +5607,83 @@
             {
                 let l = t.childNodes[r - 1];
                 if (Wt(l, -1)) i = t, s = --r;
                 else if (l.nodeType == 3) t = l, r = t.nodeValue.length;
                 else break
             }
         } else {
-            if (Co(t)) break;
+            if (To(t)) break;
             {
                 let l = t.previousSibling;
                 for (; l && Wt(l, -1);) i = t.parentNode, s = ee(l), l = l.previousSibling;
                 if (l) t = l, r = Sn(t);
                 else {
                     if (t = t.parentNode, t == n.dom) break;
                     r = 0
                 }
             }
-        } o ? Or(n, t, r) : i && Or(n, i, s)
+        } o ? Nr(n, t, r) : i && Nr(n, i, s)
 }
 
-function zc(n) {
+function Vc(n) {
     let e = n.domSelectionRange(),
         t = e.focusNode,
         r = e.focusOffset;
     if (!t) return;
     let i = Sn(t),
         s, o;
     for (;;)
         if (r < i) {
             if (t.nodeType != 1) break;
             let l = t.childNodes[r];
             if (Wt(l, 1)) s = t, o = ++r;
             else break
         } else {
-            if (Co(t)) break;
+            if (To(t)) break;
             {
                 let l = t.nextSibling;
                 for (; l && Wt(l, 1);) s = l.parentNode, o = ee(l) + 1, l = l.nextSibling;
                 if (l) t = l, r = 0, i = Sn(t);
                 else {
                     if (t = t.parentNode, t == n.dom) break;
                     r = i = 0
                 }
             }
-        } s && Or(n, s, o)
+        } s && Nr(n, s, o)
 }
 
-function Co(n) {
+function To(n) {
     let e = n.pmViewDesc;
     return e && e.node && e.node.isBlock
 }
 
-function $c(n, e) {
+function jc(n, e) {
     for (; n && e == n.childNodes.length && !Yt(n);) e = ee(n) + 1, n = n.parentNode;
     for (; n && e < n.childNodes.length;) {
         let t = n.childNodes[e];
         if (t.nodeType == 3) return t;
         if (t.nodeType == 1 && t.contentEditable == "false") break;
         n = t, e = 0
     }
 }
 
-function Hc(n, e) {
+function Jc(n, e) {
     for (; n && !e && !Yt(n);) e = ee(n), n = n.parentNode;
     for (; n && e;) {
         let t = n.childNodes[e - 1];
         if (t.nodeType == 3) return t;
         if (t.nodeType == 1 && t.contentEditable == "false") break;
         n = t, e = n.childNodes.length
     }
 }
 
-function Or(n, e, t) {
+function Nr(n, e, t) {
     if (e.nodeType != 3) {
         let s, o;
-        (o = $c(e, t)) ? (e = o, t = 0) : (s = Hc(e, t)) && (e = s, t = s.nodeValue.length)
+        (o = jc(e, t)) ? (e = o, t = 0) : (s = Jc(e, t)) && (e = s, t = s.nodeValue.length)
     }
     let r = n.domSelection();
     if (vn(r)) {
         let s = document.createRange();
         s.setEnd(e, t), s.setStart(e, t), r.removeAllRanges(), r.addRange(s)
     } else r.extend && r.extend(e, t);
     n.domObserver.setCurSelection();
@@ -5685,15 +5693,15 @@
     setTimeout(() => {
         n.state == i && Re(n)
     }, 50)
 }
 
 function Gs(n, e) {
     let t = n.state.doc.resolve(e);
-    if (!(oe || uc) && t.parent.inlineContent) {
+    if (!(oe || pc) && t.parent.inlineContent) {
         let i = n.coordsAtPos(e);
         if (e > t.start()) {
             let s = n.coordsAtPos(e - 1),
                 o = (s.top + s.bottom) / 2;
             if (o > i.top && o < i.bottom && Math.abs(s.left - i.left) > 1) return s.left < i.left ? "ltr" : "rtl"
         }
         if (e < t.end()) {
@@ -5709,15 +5717,15 @@
     let r = n.state.selection;
     if (r instanceof P && !r.empty || t.indexOf("s") > -1 || me && t.indexOf("m") > -1) return !1;
     let {
         $from: i,
         $to: s
     } = r;
     if (!i.parent.inlineContent || n.endOfTextblock(e < 0 ? "up" : "down")) {
-        let o = vr(n.state, e);
+        let o = Or(n.state, e);
         if (o && o instanceof O) return $e(n, o)
     }
     if (!i.parent.inlineContent) {
         let o = e < 0 ? i : s,
             l = r instanceof fe ? L.near(o, e) : L.findFrom(o, e);
         return l ? $e(n, l) : !1
     }
@@ -5742,53 +5750,53 @@
     return !1
 }
 
 function Zs(n, e, t) {
     n.domObserver.stop(), e.contentEditable = t, n.domObserver.start()
 }
 
-function Vc(n) {
+function qc(n) {
     if (!le || n.state.selection.$head.parentOffset > 0) return !1;
     let {
         focusNode: e,
         focusOffset: t
     } = n.domSelectionRange();
     if (e && e.nodeType == 1 && t == 0 && e.firstChild && e.firstChild.contentEditable == "false") {
         let r = e.firstChild;
         Zs(n, r, "true"), setTimeout(() => Zs(n, r, "false"), 20)
     }
     return !1
 }
 
-function jc(n) {
+function Wc(n) {
     let e = "";
     return n.ctrlKey && (e += "c"), n.metaKey && (e += "m"), n.altKey && (e += "a"), n.shiftKey && (e += "s"), e
 }
 
-function Jc(n, e) {
+function Kc(n, e) {
     let t = e.keyCode,
-        r = jc(e);
+        r = Wc(e);
     if (t == 8 || me && t == 72 && r == "c") return Xs(n, -1) || kt(n, -1);
     if (t == 46 && !e.shiftKey || me && t == 68 && r == "c") return Xs(n, 1) || kt(n, 1);
     if (t == 13 || t == 27) return !0;
     if (t == 37 || me && t == 66 && r == "c") {
         let i = t == 37 ? Gs(n, n.state.selection.from) == "ltr" ? -1 : 1 : -1;
         return _s(n, i, r) || kt(n, i)
     } else if (t == 39 || me && t == 70 && r == "c") {
         let i = t == 39 ? Gs(n, n.state.selection.from) == "ltr" ? 1 : -1 : 1;
         return _s(n, i, r) || kt(n, i)
     } else {
         if (t == 38 || me && t == 80 && r == "c") return Ys(n, -1, r) || kt(n, -1);
-        if (t == 40 || me && t == 78 && r == "c") return Vc(n) || Ys(n, 1, r) || kt(n, 1);
+        if (t == 40 || me && t == 78 && r == "c") return qc(n) || Ys(n, 1, r) || kt(n, 1);
         if (r == (me ? "m" : "c") && (t == 66 || t == 73 || t == 89 || t == 90)) return !0
     }
     return !1
 }
 
-function To(n, e) {
+function Ao(n, e) {
     n.someProp("transformCopied", h => {
         e = h(e, n)
     });
     let t = [],
         {
             content: r,
             openStart: i,
@@ -5796,48 +5804,49 @@
         } = e;
     for (; i > 1 && s > 1 && r.childCount == 1 && r.firstChild.childCount == 1;) {
         i--, s--;
         let h = r.firstChild;
         t.push(h.type.name, h.attrs != h.type.defaultAttrs ? h.attrs : null), r = h.content
     }
     let o = n.someProp("clipboardSerializer") || Oe.fromSchema(n.state.schema),
-        l = Io(),
+        l = Po(),
         a = l.createElement("div");
     a.appendChild(o.serializeFragment(r, {
         document: l
     }));
     let c = a.firstChild,
         d, u = 0;
-    for (; c && c.nodeType == 1 && (d = Do[c.nodeName.toLowerCase()]);) {
+    for (; c && c.nodeType == 1 && (d = Io[c.nodeName.toLowerCase()]);) {
         for (let h = d.length - 1; h >= 0; h--) {
             let p = l.createElement(d[h]);
             for (; a.firstChild;) p.appendChild(a.firstChild);
             a.appendChild(p), u++
         }
         c = a.firstChild
     }
     c && c.nodeType == 1 && c.setAttribute("data-pm-slice", `${i} ${s}${u?` -${u}`:""} ${JSON.stringify(t)}`);
     let f = n.someProp("clipboardTextSerializer", h => h(e, n)) || e.content.textBetween(0, e.content.size, `
 
 `);
     return {
         dom: a,
-        text: f
+        text: f,
+        slice: e
     }
 }
 
-function Ao(n, e, t, r, i) {
+function vo(n, e, t, r, i) {
     let s = i.parent.type.spec.code,
         o, l;
     if (!t && !e) return null;
     let a = e && (r || s || !t);
     if (a) {
         if (n.someProp("transformPastedText", f => {
                 e = f(e, s || r, n)
-            }), s) return e ? new E(M.from(n.state.schema.text(e.replace(/\r\n?/g, `
+            }), s) return e ? new E(w.from(n.state.schema.text(e.replace(/\r\n?/g, `
 `))), 0, 0) : E.empty;
         let u = n.someProp("clipboardTextParser", f => f(e, i, r, n));
         if (u) l = u;
         else {
             let f = i.marks(),
                 {
                     schema: h
@@ -5846,133 +5855,133 @@
             o = document.createElement("div"), e.split(/(?:\r\n?|\n)+/).forEach(m => {
                 let g = o.appendChild(document.createElement("p"));
                 m && g.appendChild(p.serializeNode(h.text(m, f)))
             })
         }
     } else n.someProp("transformPastedHTML", u => {
         t = u(t, n)
-    }), o = Kc(t), Xt && Uc(o);
+    }), o = Gc(t), Xt && Yc(o);
     let c = o && o.querySelector("[data-pm-slice]"),
         d = c && /^(\d+) (\d+)(?: -(\d+))? (.*)/.exec(c.getAttribute("data-pm-slice") || "");
     if (d && d[3])
         for (let u = +d[3]; u > 0; u--) {
             let f = o.firstChild;
             for (; f && f.nodeType != 1;) f = f.nextSibling;
             if (!f) break;
             o = f
         }
     if (l || (l = (n.someProp("clipboardParser") || n.someProp("domParser") || Qe.fromSchema(n.state.schema)).parseSlice(o, {
             preserveWhitespace: !!(a || d),
             context: i,
             ruleFromNode(f) {
-                return f.nodeName == "BR" && !f.nextSibling && f.parentNode && !qc.test(f.parentNode.nodeName) ? {
+                return f.nodeName == "BR" && !f.nextSibling && f.parentNode && !Uc.test(f.parentNode.nodeName) ? {
                     ignore: !0
                 } : null
             }
-        })), d) l = _c(Qs(l, +d[1], +d[2]), d[4]);
-    else if (l = E.maxOpen(Wc(l.content, i), !0), l.openStart || l.openEnd) {
+        })), d) l = Xc(Qs(l, +d[1], +d[2]), d[4]);
+    else if (l = E.maxOpen(_c(l.content, i), !0), l.openStart || l.openEnd) {
         let u = 0,
             f = 0;
         for (let h = l.content.firstChild; u < l.openStart && !h.type.spec.isolating; u++, h = h.firstChild);
         for (let h = l.content.lastChild; f < l.openEnd && !h.type.spec.isolating; f++, h = h.lastChild);
         l = Qs(l, u, f)
     }
     return n.someProp("transformPasted", u => {
         l = u(l, n)
     }), l
 }
-var qc = /^(a|abbr|acronym|b|cite|code|del|em|i|ins|kbd|label|output|q|ruby|s|samp|span|strong|sub|sup|time|u|tt|var)$/i;
+var Uc = /^(a|abbr|acronym|b|cite|code|del|em|i|ins|kbd|label|output|q|ruby|s|samp|span|strong|sub|sup|time|u|tt|var)$/i;
 
-function Wc(n, e) {
+function _c(n, e) {
     if (n.childCount < 2) return n;
     for (let t = e.depth; t >= 0; t--) {
         let i = e.node(t).contentMatchAt(e.index(t)),
             s, o = [];
         if (n.forEach(l => {
                 if (!o) return;
                 let a = i.findWrapping(l.type),
                     c;
                 if (!a) return o = null;
-                if (c = o.length && s.length && Oo(a, s, l, o[o.length - 1], 0)) o[o.length - 1] = c;
+                if (c = o.length && s.length && No(a, s, l, o[o.length - 1], 0)) o[o.length - 1] = c;
                 else {
-                    o.length && (o[o.length - 1] = No(o[o.length - 1], s.length));
-                    let d = vo(l, a);
+                    o.length && (o[o.length - 1] = Do(o[o.length - 1], s.length));
+                    let d = Oo(l, a);
                     o.push(d), i = i.matchType(d.type), s = a
                 }
-            }), o) return M.from(o)
+            }), o) return w.from(o)
     }
     return n
 }
 
-function vo(n, e, t = 0) {
-    for (let r = e.length - 1; r >= t; r--) n = e[r].create(null, M.from(n));
+function Oo(n, e, t = 0) {
+    for (let r = e.length - 1; r >= t; r--) n = e[r].create(null, w.from(n));
     return n
 }
 
-function Oo(n, e, t, r, i) {
+function No(n, e, t, r, i) {
     if (i < n.length && i < e.length && n[i] == e[i]) {
-        let s = Oo(n, e, t, r.lastChild, i + 1);
+        let s = No(n, e, t, r.lastChild, i + 1);
         if (s) return r.copy(r.content.replaceChild(r.childCount - 1, s));
-        if (r.contentMatchAt(r.childCount).matchType(i == n.length - 1 ? t.type : n[i + 1])) return r.copy(r.content.append(M.from(vo(t, n, i + 1))))
+        if (r.contentMatchAt(r.childCount).matchType(i == n.length - 1 ? t.type : n[i + 1])) return r.copy(r.content.append(w.from(Oo(t, n, i + 1))))
     }
 }
 
-function No(n, e) {
+function Do(n, e) {
     if (e == 0) return n;
-    let t = n.content.replaceChild(n.childCount - 1, No(n.lastChild, e - 1)),
-        r = n.contentMatchAt(n.childCount).fillBefore(M.empty, !0);
+    let t = n.content.replaceChild(n.childCount - 1, Do(n.lastChild, e - 1)),
+        r = n.contentMatchAt(n.childCount).fillBefore(w.empty, !0);
     return n.copy(t.append(r))
 }
 
-function Nr(n, e, t, r, i, s) {
+function Dr(n, e, t, r, i, s) {
     let o = e < 0 ? n.firstChild : n.lastChild,
         l = o.content;
-    return n.childCount > 1 && (s = 0), i < r - 1 && (l = Nr(l, e, t, r, i + 1, s)), i >= t && (l = e < 0 ? o.contentMatchAt(0).fillBefore(l, s <= i).append(l) : l.append(o.contentMatchAt(o.childCount).fillBefore(M.empty, !0))), n.replaceChild(e < 0 ? 0 : n.childCount - 1, o.copy(l))
+    return n.childCount > 1 && (s = 0), i < r - 1 && (l = Dr(l, e, t, r, i + 1, s)), i >= t && (l = e < 0 ? o.contentMatchAt(0).fillBefore(l, s <= i).append(l) : l.append(o.contentMatchAt(o.childCount).fillBefore(w.empty, !0))), n.replaceChild(e < 0 ? 0 : n.childCount - 1, o.copy(l))
 }
 
 function Qs(n, e, t) {
-    return e < n.openStart && (n = new E(Nr(n.content, -1, e, n.openStart, 0, n.openEnd), e, n.openEnd)), t < n.openEnd && (n = new E(Nr(n.content, 1, t, n.openEnd, 0, 0), n.openStart, t)), n
+    return e < n.openStart && (n = new E(Dr(n.content, -1, e, n.openStart, 0, n.openEnd), e, n.openEnd)), t < n.openEnd && (n = new E(Dr(n.content, 1, t, n.openEnd, 0, 0), n.openStart, t)), n
 }
-var Do = {
+var Io = {
         thead: ["table"],
         tbody: ["table"],
         tfoot: ["table"],
         caption: ["table"],
         colgroup: ["table"],
         col: ["table", "colgroup"],
         tr: ["table", "tbody"],
         td: ["table", "tbody", "tr"],
         th: ["table", "tbody", "tr"]
     },
     eo = null;
 
-function Io() {
+function Po() {
     return eo || (eo = document.implementation.createHTMLDocument("title"))
 }
 
-function Kc(n) {
+function Gc(n) {
     let e = /^(\s*<meta [^>]*>)*/.exec(n);
     e && (n = n.slice(e[0].length));
-    let t = Io().createElement("div"),
+    let t = Po().createElement("div"),
         r = /<([a-z][^>\s]+)/i.exec(n),
         i;
-    if ((i = r && Do[r[1].toLowerCase()]) && (n = i.map(s => "<" + s + ">").join("") + n + i.map(s => "</" + s + ">").reverse().join("")), t.innerHTML = n, i)
+    if ((i = r && Io[r[1].toLowerCase()]) && (n = i.map(s => "<" + s + ">").join("") + n + i.map(s => "</" + s + ">").reverse().join("")), t.innerHTML = n, i)
         for (let s = 0; s < i.length; s++) t = t.querySelector(i[s]) || t;
     return t
 }
 
-function Uc(n) {
+function Yc(n) {
     let e = n.querySelectorAll(oe ? "span:not([class]):not([style])" : "span.Apple-converted-space");
     for (let t = 0; t < e.length; t++) {
         let r = e[t];
         r.childNodes.length == 1 && r.textContent == "\xA0" && r.parentNode && r.parentNode.replaceChild(n.ownerDocument.createTextNode(" "), r)
     }
 }
 
-function _c(n, e) {
+function Xc(n, e) {
     if (!n.size) return n;
     let t = n.content.firstChild.type.schema,
         r;
     try {
         r = JSON.parse(e)
     } catch {
         return n
@@ -5981,97 +5990,97 @@
         content: i,
         openStart: s,
         openEnd: o
     } = n;
     for (let l = r.length - 2; l >= 0; l -= 2) {
         let a = t.nodes[r[l]];
         if (!a || a.hasRequiredAttrs()) break;
-        i = M.from(a.create(r[l + 1], i)), s++, o++
+        i = w.from(a.create(r[l + 1], i)), s++, o++
     }
     return new E(i, s, o)
 }
 var ae = {},
     ce = {},
-    Gc = {
+    Zc = {
         touchstart: !0,
         touchmove: !0
     },
-    Dr = class {
+    Ir = class {
         constructor() {
             this.shiftKey = !1, this.mouseDown = null, this.lastKeyCode = null, this.lastKeyCodeTime = 0, this.lastClick = {
                 time: 0,
                 x: 0,
                 y: 0,
                 type: ""
             }, this.lastSelectionOrigin = null, this.lastSelectionTime = 0, this.lastIOSEnter = 0, this.lastIOSEnterFallbackTimeout = -1, this.lastFocus = 0, this.lastTouch = 0, this.lastAndroidDelete = 0, this.composing = !1, this.compositionNode = null, this.composingTimeout = -1, this.compositionNodes = [], this.compositionEndedAt = -2e8, this.compositionID = 1, this.compositionPendingChanges = 0, this.domChangeCount = 0, this.eventHandlers = Object.create(null), this.hideSelectionGuard = null
         }
     };
 
-function Yc(n) {
+function Qc(n) {
     for (let e in ae) {
         let t = ae[e];
         n.dom.addEventListener(e, n.input.eventHandlers[e] = r => {
-            Zc(n, r) && !Hr(n, r) && (n.editable || !(r.type in ce)) && t(n, r)
-        }, Gc[e] ? {
+            td(n, r) && !Vr(n, r) && (n.editable || !(r.type in ce)) && t(n, r)
+        }, Zc[e] ? {
             passive: !0
         } : void 0)
     }
-    le && n.dom.addEventListener("input", () => null), Ir(n)
+    le && n.dom.addEventListener("input", () => null), Pr(n)
 }
 
 function He(n, e) {
     n.input.lastSelectionOrigin = e, n.input.lastSelectionTime = Date.now()
 }
 
-function Xc(n) {
+function ed(n) {
     n.domObserver.stop();
     for (let e in n.input.eventHandlers) n.dom.removeEventListener(e, n.input.eventHandlers[e]);
     clearTimeout(n.input.composingTimeout), clearTimeout(n.input.lastIOSEnterFallbackTimeout)
 }
 
-function Ir(n) {
+function Pr(n) {
     n.someProp("handleDOMEvents", e => {
-        for (let t in e) n.input.eventHandlers[t] || n.dom.addEventListener(t, n.input.eventHandlers[t] = r => Hr(n, r))
+        for (let t in e) n.input.eventHandlers[t] || n.dom.addEventListener(t, n.input.eventHandlers[t] = r => Vr(n, r))
     })
 }
 
-function Hr(n, e) {
+function Vr(n, e) {
     return n.someProp("handleDOMEvents", t => {
         let r = t[e.type];
         return r ? r(n, e) || e.defaultPrevented : !1
     })
 }
 
-function Zc(n, e) {
+function td(n, e) {
     if (!e.bubbles) return !0;
     if (e.defaultPrevented) return !1;
     for (let t = e.target; t != n.dom; t = t.parentNode)
         if (!t || t.nodeType == 11 || t.pmViewDesc && t.pmViewDesc.stopEvent(e)) return !1;
     return !0
 }
 
-function Qc(n, e) {
-    !Hr(n, e) && ae[e.type] && (n.editable || !(e.type in ce)) && ae[e.type](n, e)
+function nd(n, e) {
+    !Vr(n, e) && ae[e.type] && (n.editable || !(e.type in ce)) && ae[e.type](n, e)
 }
 ce.keydown = (n, e) => {
     let t = e;
-    if (n.input.shiftKey = t.keyCode == 16 || t.shiftKey, !Ro(n, t) && (n.input.lastKeyCode = t.keyCode, n.input.lastKeyCodeTime = Date.now(), !(be && oe && t.keyCode == 13)))
+    if (n.input.shiftKey = t.keyCode == 16 || t.shiftKey, !Lo(n, t) && (n.input.lastKeyCode = t.keyCode, n.input.lastKeyCodeTime = Date.now(), !(be && oe && t.keyCode == 13)))
         if (t.keyCode != 229 && n.domObserver.forceFlush(), wt && t.keyCode == 13 && !t.ctrlKey && !t.altKey && !t.metaKey) {
             let r = Date.now();
             n.input.lastIOSEnter = r, n.input.lastIOSEnterFallbackTimeout = setTimeout(() => {
                 n.input.lastIOSEnter == r && (n.someProp("handleKeyDown", i => i(n, nt(13, "Enter"))), n.input.lastIOSEnter = 0)
             }, 200)
-        } else n.someProp("handleKeyDown", r => r(n, t)) || Jc(n, t) ? t.preventDefault() : He(n, "key")
+        } else n.someProp("handleKeyDown", r => r(n, t)) || Kc(n, t) ? t.preventDefault() : He(n, "key")
 };
 ce.keyup = (n, e) => {
     e.keyCode == 16 && (n.input.shiftKey = !1)
 };
 ce.keypress = (n, e) => {
     let t = e;
-    if (Ro(n, t) || !t.charCode || t.ctrlKey && !t.altKey || me && t.metaKey) return;
+    if (Lo(n, t) || !t.charCode || t.ctrlKey && !t.altKey || me && t.metaKey) return;
     if (n.someProp("handleKeyPress", i => i(n, t))) {
         t.preventDefault();
         return
     }
     let r = n.state.selection;
     if (!(r instanceof P) || !r.$from.sameParent(r.$to)) {
         let i = String.fromCharCode(t.charCode);
@@ -6082,42 +6091,42 @@
 function On(n) {
     return {
         left: n.clientX,
         top: n.clientY
     }
 }
 
-function ed(n, e) {
+function rd(n, e) {
     let t = e.x - n.clientX,
         r = e.y - n.clientY;
     return t * t + r * r < 100
 }
 
-function Vr(n, e, t, r, i) {
+function jr(n, e, t, r, i) {
     if (r == -1) return !1;
     let s = n.state.doc.resolve(r);
     for (let o = s.depth + 1; o > 0; o--)
         if (n.someProp(e, l => o > s.depth ? l(n, t, s.nodeAfter, s.before(o), i, !0) : l(n, t, s.node(o), s.before(o), i, !1))) return !0;
     return !1
 }
 
 function Mt(n, e, t) {
     n.focused || n.focus();
     let r = n.state.tr.setSelection(e);
     t == "pointer" && r.setMeta("pointer", !0), n.dispatch(r)
 }
 
-function td(n, e) {
+function id(n, e) {
     if (e == -1) return !1;
     let t = n.state.doc.resolve(e),
         r = t.nodeAfter;
     return r && r.isAtom && O.isSelectable(r) ? (Mt(n, new O(t), "pointer"), !0) : !1
 }
 
-function nd(n, e) {
+function sd(n, e) {
     if (e == -1) return !1;
     let t = n.state.selection,
         r, i;
     t instanceof O && (r = t.node);
     let s = n.state.doc.resolve(e);
     for (let o = s.depth + 1; o > 0; o--) {
         let l = o > s.depth ? s.nodeAfter : s.node(o);
@@ -6125,63 +6134,63 @@
             r && t.$from.depth > 0 && o >= t.$from.depth && s.before(t.$from.depth + 1) == t.$from.pos ? i = s.before(t.$from.depth) : i = s.before(o);
             break
         }
     }
     return i != null ? (Mt(n, O.create(n.state.doc, i), "pointer"), !0) : !1
 }
 
-function rd(n, e, t, r, i) {
-    return Vr(n, "handleClickOn", e, t, r) || n.someProp("handleClick", s => s(n, e, r)) || (i ? nd(n, t) : td(n, t))
+function od(n, e, t, r, i) {
+    return jr(n, "handleClickOn", e, t, r) || n.someProp("handleClick", s => s(n, e, r)) || (i ? sd(n, t) : id(n, t))
 }
 
-function id(n, e, t, r) {
-    return Vr(n, "handleDoubleClickOn", e, t, r) || n.someProp("handleDoubleClick", i => i(n, e, r))
+function ld(n, e, t, r) {
+    return jr(n, "handleDoubleClickOn", e, t, r) || n.someProp("handleDoubleClick", i => i(n, e, r))
 }
 
-function sd(n, e, t, r) {
-    return Vr(n, "handleTripleClickOn", e, t, r) || n.someProp("handleTripleClick", i => i(n, e, r)) || od(n, t, r)
+function ad(n, e, t, r) {
+    return jr(n, "handleTripleClickOn", e, t, r) || n.someProp("handleTripleClick", i => i(n, e, r)) || cd(n, t, r)
 }
 
-function od(n, e, t) {
+function cd(n, e, t) {
     if (t.button != 0) return !1;
     let r = n.state.doc;
     if (e == -1) return r.inlineContent ? (Mt(n, P.create(r, 0, r.content.size), "pointer"), !0) : !1;
     let i = r.resolve(e);
     for (let s = i.depth + 1; s > 0; s--) {
         let o = s > i.depth ? i.nodeAfter : i.node(s),
             l = i.before(s);
         if (o.inlineContent) Mt(n, P.create(r, l + 1, l + 1 + o.content.size), "pointer");
         else if (O.isSelectable(o)) Mt(n, O.create(r, l), "pointer");
         else continue;
         return !0
     }
 }
 
-function jr(n) {
+function Jr(n) {
     return Mn(n)
 }
-var Po = me ? "metaKey" : "ctrlKey";
+var Ro = me ? "metaKey" : "ctrlKey";
 ae.mousedown = (n, e) => {
     let t = e;
     n.input.shiftKey = t.shiftKey;
-    let r = jr(n),
+    let r = Jr(n),
         i = Date.now(),
         s = "singleClick";
-    i - n.input.lastClick.time < 500 && ed(t, n.input.lastClick) && !t[Po] && (n.input.lastClick.type == "singleClick" ? s = "doubleClick" : n.input.lastClick.type == "doubleClick" && (s = "tripleClick")), n.input.lastClick = {
+    i - n.input.lastClick.time < 500 && rd(t, n.input.lastClick) && !t[Ro] && (n.input.lastClick.type == "singleClick" ? s = "doubleClick" : n.input.lastClick.type == "doubleClick" && (s = "tripleClick")), n.input.lastClick = {
         time: i,
         x: t.clientX,
         y: t.clientY,
         type: s
     };
     let o = n.posAtCoords(On(t));
-    o && (s == "singleClick" ? (n.input.mouseDown && n.input.mouseDown.done(), n.input.mouseDown = new Pr(n, o, t, !!r)) : (s == "doubleClick" ? id : sd)(n, o.pos, o.inside, t) ? t.preventDefault() : He(n, "pointer"))
+    o && (s == "singleClick" ? (n.input.mouseDown && n.input.mouseDown.done(), n.input.mouseDown = new Rr(n, o, t, !!r)) : (s == "doubleClick" ? ld : ad)(n, o.pos, o.inside, t) ? t.preventDefault() : He(n, "pointer"))
 };
-var Pr = class {
+var Rr = class {
     constructor(e, t, r, i) {
-        this.view = e, this.pos = t, this.event = r, this.flushed = i, this.delayedSelectionSync = !1, this.mightDrag = null, this.startDoc = e.state.doc, this.selectNode = !!r[Po], this.allowDefault = r.shiftKey;
+        this.view = e, this.pos = t, this.event = r, this.flushed = i, this.delayedSelectionSync = !1, this.mightDrag = null, this.startDoc = e.state.doc, this.selectNode = !!r[Ro], this.allowDefault = r.shiftKey;
         let s, o;
         if (t.inside > -1) s = e.state.doc.nodeAt(t.inside), o = t.inside;
         else {
             let d = e.state.doc.resolve(t.pos);
             s = d.parent, o = d.depth ? d.before() : 0
         }
         let l = i ? null : r.target,
@@ -6201,35 +6210,35 @@
     }
     done() {
         this.view.root.removeEventListener("mouseup", this.up), this.view.root.removeEventListener("mousemove", this.move), this.mightDrag && this.target && (this.view.domObserver.stop(), this.mightDrag.addAttr && this.target.removeAttribute("draggable"), this.mightDrag.setUneditable && this.target.removeAttribute("contentEditable"), this.view.domObserver.start()), this.delayedSelectionSync && setTimeout(() => Re(this.view)), this.view.input.mouseDown = null
     }
     up(e) {
         if (this.done(), !this.view.dom.contains(e.target)) return;
         let t = this.pos;
-        this.view.state.doc != this.startDoc && (t = this.view.posAtCoords(On(e))), this.updateAllowDefault(e), this.allowDefault || !t ? He(this.view, "pointer") : rd(this.view, t.pos, t.inside, e, this.selectNode) ? e.preventDefault() : e.button == 0 && (this.flushed || le && this.mightDrag && !this.mightDrag.node.isAtom || oe && !this.view.state.selection.visible && Math.min(Math.abs(t.pos - this.view.state.selection.from), Math.abs(t.pos - this.view.state.selection.to)) <= 2) ? (Mt(this.view, L.near(this.view.state.doc.resolve(t.pos)), "pointer"), e.preventDefault()) : He(this.view, "pointer")
+        this.view.state.doc != this.startDoc && (t = this.view.posAtCoords(On(e))), this.updateAllowDefault(e), this.allowDefault || !t ? He(this.view, "pointer") : od(this.view, t.pos, t.inside, e, this.selectNode) ? e.preventDefault() : e.button == 0 && (this.flushed || le && this.mightDrag && !this.mightDrag.node.isAtom || oe && !this.view.state.selection.visible && Math.min(Math.abs(t.pos - this.view.state.selection.from), Math.abs(t.pos - this.view.state.selection.to)) <= 2) ? (Mt(this.view, L.near(this.view.state.doc.resolve(t.pos)), "pointer"), e.preventDefault()) : He(this.view, "pointer")
     }
     move(e) {
         this.updateAllowDefault(e), He(this.view, "pointer"), e.buttons == 0 && this.done()
     }
     updateAllowDefault(e) {
         !this.allowDefault && (Math.abs(this.event.x - e.clientX) > 4 || Math.abs(this.event.y - e.clientY) > 4) && (this.allowDefault = !0)
     }
 };
 ae.touchstart = n => {
-    n.input.lastTouch = Date.now(), jr(n), He(n, "pointer")
+    n.input.lastTouch = Date.now(), Jr(n), He(n, "pointer")
 };
 ae.touchmove = n => {
     n.input.lastTouch = Date.now(), He(n, "pointer")
 };
-ae.contextmenu = n => jr(n);
+ae.contextmenu = n => Jr(n);
 
-function Ro(n, e) {
+function Lo(n, e) {
     return n.composing ? !0 : le && Math.abs(e.timeStamp - n.input.compositionEndedAt) < 500 ? (n.input.compositionEndedAt = -2e8, !0) : !1
 }
-var ld = be ? 5e3 : -1;
+var dd = be ? 5e3 : -1;
 ce.compositionstart = ce.compositionupdate = n => {
     if (!n.composing) {
         n.domObserver.flush();
         let {
             state: e
         } = n, t = e.selection.$from;
         if (e.selection.empty && (e.storedMarks || !t.textOffset && t.parentOffset && t.nodeBefore.marks.some(r => r.type.spec.inclusive === !1))) n.markCursor = n.state.storedMarks || t.marks(), Mn(n, !0), n.markCursor = null;
@@ -6242,147 +6251,148 @@
                     n.domSelection().collapse(o, o.nodeValue.length);
                     break
                 } else i = o, s = -1
             }
         }
         n.input.composing = !0
     }
-    Lo(n, ld)
+    Bo(n, dd)
 };
 ce.compositionend = (n, e) => {
-    n.composing && (n.input.composing = !1, n.input.compositionEndedAt = e.timeStamp, n.input.compositionPendingChanges = n.domObserver.pendingRecords().length ? n.input.compositionID : 0, n.input.compositionNode = null, n.input.compositionPendingChanges && Promise.resolve().then(() => n.domObserver.flush()), n.input.compositionID++, Lo(n, 20))
+    n.composing && (n.input.composing = !1, n.input.compositionEndedAt = e.timeStamp, n.input.compositionPendingChanges = n.domObserver.pendingRecords().length ? n.input.compositionID : 0, n.input.compositionNode = null, n.input.compositionPendingChanges && Promise.resolve().then(() => n.domObserver.flush()), n.input.compositionID++, Bo(n, 20))
 };
 
-function Lo(n, e) {
+function Bo(n, e) {
     clearTimeout(n.input.composingTimeout), e > -1 && (n.input.composingTimeout = setTimeout(() => Mn(n), e))
 }
 
-function Bo(n) {
-    for (n.composing && (n.input.composing = !1, n.input.compositionEndedAt = cd()); n.input.compositionNodes.length > 0;) n.input.compositionNodes.pop().markParentsDirty()
+function Fo(n) {
+    for (n.composing && (n.input.composing = !1, n.input.compositionEndedAt = fd()); n.input.compositionNodes.length > 0;) n.input.compositionNodes.pop().markParentsDirty()
 }
 
-function ad(n) {
+function ud(n) {
     let e = n.domSelectionRange();
     if (!e.focusNode) return null;
-    let t = sc(e.focusNode, e.focusOffset),
-        r = oc(e.focusNode, e.focusOffset);
+    let t = ac(e.focusNode, e.focusOffset),
+        r = cc(e.focusNode, e.focusOffset);
     if (t && r && t != r) {
         let i = r.pmViewDesc;
         if (!i || !i.isText(r.nodeValue)) return r;
         if (n.input.compositionNode == r) {
             let s = t.pmViewDesc;
             if (!(!s || !s.isText(t.nodeValue))) return r
         }
     }
-    return t
+    return t || r
 }
 
-function cd() {
+function fd() {
     let n = document.createEvent("Event");
     return n.initEvent("event", !0, !0), n.timeStamp
 }
 
 function Mn(n, e = !1) {
     if (!(be && n.domObserver.flushingSoon >= 0)) {
-        if (n.domObserver.forceFlush(), Bo(n), e || n.docView && n.docView.dirty) {
-            let t = zr(n);
+        if (n.domObserver.forceFlush(), Fo(n), e || n.docView && n.docView.dirty) {
+            let t = $r(n);
             return t && !t.eq(n.state.selection) ? n.dispatch(n.state.tr.setSelection(t)) : n.updateState(n.state), !0
         }
         return !1
     }
 }
 
-function dd(n, e) {
+function hd(n, e) {
     if (!n.dom.parentNode) return;
     let t = n.dom.parentNode.appendChild(document.createElement("div"));
     t.appendChild(e), t.style.cssText = "position: fixed; left: -10000px; top: 10px";
     let r = getSelection(),
         i = document.createRange();
     i.selectNodeContents(e), n.dom.blur(), r.removeAllRanges(), r.addRange(i), setTimeout(() => {
         t.parentNode && t.parentNode.removeChild(t), n.focus()
     }, 50)
 }
-var Ut = de && Ve < 15 || wt && fc < 604;
+var Ut = de && Ve < 15 || wt && mc < 604;
 ae.copy = ce.cut = (n, e) => {
     let t = e,
         r = n.state.selection,
         i = t.type == "cut";
     if (r.empty) return;
     let s = Ut ? null : t.clipboardData,
         o = r.content(),
         {
             dom: l,
             text: a
-        } = To(n, o);
-    s ? (t.preventDefault(), s.clearData(), s.setData("text/html", l.innerHTML), s.setData("text/plain", a)) : dd(n, l), i && n.dispatch(n.state.tr.deleteSelection().scrollIntoView().setMeta("uiEvent", "cut"))
+        } = Ao(n, o);
+    s ? (t.preventDefault(), s.clearData(), s.setData("text/html", l.innerHTML), s.setData("text/plain", a)) : hd(n, l), i && n.dispatch(n.state.tr.deleteSelection().scrollIntoView().setMeta("uiEvent", "cut"))
 };
 
-function ud(n) {
+function pd(n) {
     return n.openStart == 0 && n.openEnd == 0 && n.content.childCount == 1 ? n.content.firstChild : null
 }
 
-function fd(n, e) {
+function md(n, e) {
     if (!n.dom.parentNode) return;
     let t = n.input.shiftKey || n.state.selection.$from.parent.type.spec.code,
         r = n.dom.parentNode.appendChild(document.createElement(t ? "textarea" : "div"));
     t || (r.contentEditable = "true"), r.style.cssText = "position: fixed; left: -10000px; top: 10px", r.focus();
     let i = n.input.shiftKey && n.input.lastKeyCode != 45;
     setTimeout(() => {
         n.focus(), r.parentNode && r.parentNode.removeChild(r), t ? _t(n, r.value, null, i, e) : _t(n, r.textContent, r.innerHTML, i, e)
     }, 50)
 }
 
 function _t(n, e, t, r, i) {
-    let s = Ao(n, e, t, r, n.state.selection.$from);
+    let s = vo(n, e, t, r, n.state.selection.$from);
     if (n.someProp("handlePaste", a => a(n, i, s || E.empty))) return !0;
     if (!s) return !1;
-    let o = ud(s),
+    let o = pd(s),
         l = o ? n.state.tr.replaceSelectionWith(o, r) : n.state.tr.replaceSelection(s);
     return n.dispatch(l.scrollIntoView().setMeta("paste", !0).setMeta("uiEvent", "paste")), !0
 }
 
-function Fo(n) {
+function zo(n) {
     let e = n.getData("text/plain") || n.getData("Text");
     if (e) return e;
     let t = n.getData("text/uri-list");
     return t ? t.replace(/\r?\n/g, " ") : ""
 }
 ce.paste = (n, e) => {
     let t = e;
     if (n.composing && !be) return;
     let r = Ut ? null : t.clipboardData,
         i = n.input.shiftKey && n.input.lastKeyCode != 45;
-    r && _t(n, Fo(r), r.getData("text/html"), i, t) ? t.preventDefault() : fd(n, t)
+    r && _t(n, zo(r), r.getData("text/html"), i, t) ? t.preventDefault() : md(n, t)
 };
 var wn = class {
         constructor(e, t, r) {
             this.slice = e, this.move = t, this.node = r
         }
     },
-    zo = me ? "altKey" : "ctrlKey";
+    $o = me ? "altKey" : "ctrlKey";
 ae.dragstart = (n, e) => {
     let t = e,
         r = n.input.mouseDown;
     if (r && r.done(), !t.dataTransfer) return;
     let i = n.state.selection,
         s = i.empty ? null : n.posAtCoords(On(t)),
         o;
     if (!(s && s.pos >= i.from && s.pos <= (i instanceof O ? i.to - 1 : i.to))) {
         if (r && r.mightDrag) o = O.create(n.state.doc, r.mightDrag.pos);
         else if (t.target && t.target.nodeType == 1) {
-            let d = n.docView.nearestDesc(t.target, !0);
-            d && d.node.type.spec.draggable && d != n.docView && (o = O.create(n.state.doc, d.posBefore))
+            let u = n.docView.nearestDesc(t.target, !0);
+            u && u.node.type.spec.draggable && u != n.docView && (o = O.create(n.state.doc, u.posBefore))
         }
     }
     let l = (o || n.state.selection).content(),
         {
             dom: a,
-            text: c
-        } = To(n, l);
-    t.dataTransfer.clearData(), t.dataTransfer.setData(Ut ? "Text" : "text/html", a.innerHTML), t.dataTransfer.effectAllowed = "copyMove", Ut || t.dataTransfer.setData("text/plain", c), n.dragging = new wn(l, !t[zo], o)
+            text: c,
+            slice: d
+        } = Ao(n, l);
+    t.dataTransfer.clearData(), t.dataTransfer.setData(Ut ? "Text" : "text/html", a.innerHTML), t.dataTransfer.effectAllowed = "copyMove", Ut || t.dataTransfer.setData("text/plain", c), n.dragging = new wn(d, !t[$o], o)
 };
 ae.dragend = n => {
     let e = n.dragging;
     window.setTimeout(() => {
         n.dragging == e && (n.dragging = null)
     }, 50)
 };
@@ -6393,16 +6403,16 @@
     if (n.dragging = null, !t.dataTransfer) return;
     let i = n.posAtCoords(On(t));
     if (!i) return;
     let s = n.state.doc.resolve(i.pos),
         o = r && r.slice;
     o ? n.someProp("transformPasted", p => {
         o = p(o, n)
-    }) : o = Ao(n, Fo(t.dataTransfer), Ut ? null : t.dataTransfer.getData("text/html"), !1, s);
-    let l = !!(r && !t[zo]);
+    }) : o = vo(n, zo(t.dataTransfer), Ut ? null : t.dataTransfer.getData("text/html"), !1, s);
+    let l = !!(r && !t[$o]);
     if (n.someProp("handleDrop", p => p(n, t, o || E.empty, l))) {
         t.preventDefault();
         return
     }
     if (!o) return;
     t.preventDefault();
     let a = o ? ks(n.state.doc, s.pos, o) : s.pos;
@@ -6418,15 +6428,15 @@
         u = o.openStart == 0 && o.openEnd == 0 && o.content.childCount == 1,
         f = c.doc;
     if (u ? c.replaceRangeWith(d, d, o.content.firstChild) : c.replaceRange(d, d, o), c.doc.eq(f)) return;
     let h = c.doc.resolve(d);
     if (u && O.isSelectable(o.content.firstChild) && h.nodeAfter && h.nodeAfter.sameMarkup(o.content.firstChild)) c.setSelection(new O(h));
     else {
         let p = c.mapping.map(a);
-        c.mapping.maps[c.mapping.maps.length - 1].forEach((m, g, k, R) => p = R), c.setSelection($r(n, h, c.doc.resolve(p)))
+        c.mapping.maps[c.mapping.maps.length - 1].forEach((m, g, k, R) => p = R), c.setSelection(Hr(n, h, c.doc.resolve(p)))
     }
     n.focus(), n.dispatch(c.setMeta("uiEvent", "drop"))
 };
 ae.focus = n => {
     n.input.lastFocus = Date.now(), n.focused || (n.domObserver.stop(), n.dom.classList.add("ProseMirror-focused"), n.domObserver.start(), n.focused = !0, setTimeout(() => {
         n.docView && n.hasFocus() && !n.domObserver.currentSelection.eq(n.domSelectionRange()) && Re(n)
     }, 20))
@@ -6497,15 +6507,15 @@
             return this == e || e instanceof n && Gt(this.attrs, e.attrs) && Gt(this.spec, e.spec)
         }
         static is(e) {
             return e.type instanceof n
         }
         destroy() {}
     },
-    Rr = class n {
+    Lr = class n {
         constructor(e, t) {
             this.attrs = e, this.spec = t || ot
         }
         map(e, t, r, i) {
             let s = e.mapResult(t.from + i, 1);
             if (s.deleted) return null;
             let o = e.mapResult(t.to + i, -1);
@@ -6539,15 +6549,15 @@
         static widget(e, t, r) {
             return new n(e, e, new En(t, r))
         }
         static inline(e, t, r, i) {
             return new n(e, t, new st(r, i))
         }
         static node(e, t, r, i) {
-            return new n(e, t, new Rr(r, i))
+            return new n(e, t, new Lr(r, i))
         }
         get spec() {
             return this.type.spec
         }
         get inline() {
             return this.type instanceof st
         }
@@ -6584,30 +6594,30 @@
         }
         mapInner(e, t, r, i, s) {
             let o;
             for (let l = 0; l < this.local.length; l++) {
                 let a = this.local[l].map(e, r, i);
                 a && a.type.valid(t, a) ? (o || (o = [])).push(a) : s.onRemove && s.onRemove(this.local[l].spec)
             }
-            return this.children.length ? hd(this.children, o || [], e, t, r, i, s) : o ? new n(o.sort(lt), St) : se
+            return this.children.length ? gd(this.children, o || [], e, t, r, i, s) : o ? new n(o.sort(lt), St) : se
         }
         add(e, t) {
             return t.length ? this == se ? n.create(e, t) : this.addInner(e, t, 0) : this
         }
         addInner(e, t, r) {
             let i, s = 0;
             e.forEach((l, a) => {
                 let c = a + r,
                     d;
-                if (d = Ho(t, l, c)) {
+                if (d = Vo(t, l, c)) {
                     for (i || (i = this.children.slice()); s < i.length && i[s] < a;) s += 3;
                     i[s] == a ? i[s + 2] = i[s + 2].addInner(l, d, c + 1) : i.splice(s, 0, a, a + l.nodeSize, Tn(d, l, c + 1, ot)), s += 3
                 }
             });
-            let o = $o(s ? Vo(t) : t, -r);
+            let o = Ho(s ? jo(t) : t, -r);
             for (let l = 0; l < o.length; l++) o[l].type.valid(e, o[l]) || o.splice(l--, 1);
             return new n(o.length ? this.local.concat(o).sort(lt) : this.local, i || this.children)
         }
         remove(e) {
             return e.length == 0 || this == se ? this : this.removeInner(e, 0)
         }
         removeInner(e, t) {
@@ -6659,26 +6669,26 @@
             for (let t = 0; t < this.local.length; t++)
                 if (!this.local[t].eq(e.local[t])) return !1;
             for (let t = 0; t < this.children.length; t += 3)
                 if (this.children[t] != e.children[t] || this.children[t + 1] != e.children[t + 1] || !this.children[t + 2].eq(e.children[t + 2])) return !1;
             return !0
         }
         locals(e) {
-            return Jr(this.localsInner(e))
+            return qr(this.localsInner(e))
         }
         localsInner(e) {
             if (this == se) return St;
             if (e.inlineContent || !this.local.some(st.is)) return this.local;
             let t = [];
             for (let r = 0; r < this.local.length; r++) this.local[r].type instanceof st || t.push(this.local[r]);
             return t
         }
     };
 ue.empty = new ue([], []);
-ue.removeOverlap = Jr;
+ue.removeOverlap = qr;
 var se = ue.empty,
     Cn = class n {
         constructor(e) {
             this.members = e
         }
         map(e, t) {
             let r = this.members.map(i => i.map(e, t, ot));
@@ -6706,39 +6716,39 @@
                 if (s.length)
                     if (!t) t = s;
                     else {
                         r && (t = t.slice(), r = !1);
                         for (let o = 0; o < s.length; o++) t.push(s[o])
                     }
             }
-            return t ? Jr(r ? t : t.sort(lt)) : St
+            return t ? qr(r ? t : t.sort(lt)) : St
         }
         static from(e) {
             switch (e.length) {
                 case 0:
                     return se;
                 case 1:
                     return e[0];
                 default:
                     return new n(e.every(t => t instanceof ue) ? e : e.reduce((t, r) => t.concat(r instanceof ue ? r : r.members), []))
             }
         }
     };
 
-function hd(n, e, t, r, i, s, o) {
+function gd(n, e, t, r, i, s, o) {
     let l = n.slice();
     for (let c = 0, d = s; c < t.maps.length; c++) {
         let u = 0;
         t.maps[c].forEach((f, h, p, m) => {
             let g = m - p - (h - f);
             for (let k = 0; k < l.length; k += 3) {
                 let R = l[k + 1];
                 if (R < 0 || f > R + d - u) continue;
-                let H = l[k] + d - u;
-                h >= H ? l[k + 1] = f <= H ? -2 : -1 : f >= d && g && (l[k] += g, l[k + 1] += g)
+                let $ = l[k] + d - u;
+                h >= $ ? l[k + 1] = f <= $ ? -2 : -1 : f >= d && g && (l[k] += g, l[k + 1] += g)
             }
             u += g
         }), d = t.maps[c].map(d, -1)
     }
     let a = !1;
     for (let c = 0; c < l.length; c += 3)
         if (l[c + 1] < 0) {
@@ -6760,84 +6770,84 @@
                 } = r.content.findIndex(u),
                 g = r.maybeChild(p);
             if (g && m == u && m + g.nodeSize == h) {
                 let k = l[c + 2].mapInner(t, g, d + 1, n[c] + s + 1, o);
                 k != se ? (l[c] = u, l[c + 1] = h, l[c + 2] = k) : (l[c + 1] = -2, a = !0)
             } else a = !0
         } if (a) {
-        let c = pd(l, n, e, t, i, s, o),
+        let c = yd(l, n, e, t, i, s, o),
             d = Tn(c, r, 0, o);
         e = d.local;
         for (let u = 0; u < l.length; u += 3) l[u + 1] < 0 && (l.splice(u, 3), u -= 3);
         for (let u = 0, f = 0; u < d.children.length; u += 3) {
             let h = d.children[u];
             for (; f < l.length && l[f] < h;) f += 3;
             l.splice(f, 0, d.children[u], d.children[u + 1], d.children[u + 2])
         }
     }
     return new ue(e.sort(lt), l)
 }
 
-function $o(n, e) {
+function Ho(n, e) {
     if (!e || !n.length) return n;
     let t = [];
     for (let r = 0; r < n.length; r++) {
         let i = n[r];
         t.push(new Ee(i.from + e, i.to + e, i.type))
     }
     return t
 }
 
-function pd(n, e, t, r, i, s, o) {
+function yd(n, e, t, r, i, s, o) {
     function l(a, c) {
         for (let d = 0; d < a.local.length; d++) {
             let u = a.local[d].map(r, i, c);
             u ? t.push(u) : o.onRemove && o.onRemove(a.local[d].spec)
         }
         for (let d = 0; d < a.children.length; d += 3) l(a.children[d + 2], a.children[d] + c + 1)
     }
     for (let a = 0; a < n.length; a += 3) n[a + 1] == -1 && l(n[a + 2], e[a] + s + 1);
     return t
 }
 
-function Ho(n, e, t) {
+function Vo(n, e, t) {
     if (e.isLeaf) return null;
     let r = t + e.nodeSize,
         i = null;
     for (let s = 0, o; s < n.length; s++)(o = n[s]) && o.from > t && o.to < r && ((i || (i = [])).push(o), n[s] = null);
     return i
 }
 
-function Vo(n) {
+function jo(n) {
     let e = [];
     for (let t = 0; t < n.length; t++) n[t] != null && e.push(n[t]);
     return e
 }
 
 function Tn(n, e, t, r) {
     let i = [],
         s = !1;
     e.forEach((l, a) => {
-        let c = Ho(n, l, a + t);
+        let c = Vo(n, l, a + t);
         if (c) {
             s = !0;
             let d = Tn(c, l, t + a + 1, r);
             d != se && i.push(a, a + l.nodeSize, d)
         }
     });
-    let o = $o(s ? Vo(n) : n, -t).sort(lt);
+    let o = Ho(s ? jo(n) : n, -t).sort(lt);
     for (let l = 0; l < o.length; l++) o[l].type.valid(e, o[l]) || (r.onRemove && r.onRemove(o[l].spec), o.splice(l--, 1));
     return o.length || i.length ? new ue(o, i) : se
 }
 
 function lt(n, e) {
     return n.from - e.from || n.to - e.to
 }
 
-function Jr(n) {
+function qr(n) {
     let e = n;
     for (let t = 0; t < e.length - 1; t++) {
         let r = e[t];
         if (r.from != r.to)
             for (let i = t + 1; i < e.length; i++) {
                 let s = e[i];
                 if (s.from == r.from) {
@@ -6853,50 +6863,50 @@
 }
 
 function to(n, e, t) {
     for (; e < n.length && lt(t, n[e]) > 0;) e++;
     n.splice(e, 0, t)
 }
 
-function gr(n) {
+function yr(n) {
     let e = [];
     return n.someProp("decorations", t => {
         let r = t(n.state);
         r && r != se && e.push(r)
     }), n.cursorWrapper && e.push(ue.create(n.state.doc, [n.cursorWrapper.deco])), Cn.from(e)
 }
-var md = {
+var xd = {
         childList: !0,
         characterData: !0,
         characterDataOldValue: !0,
         attributes: !0,
         attributeOldValue: !0,
         subtree: !0
     },
-    gd = de && Ve <= 11,
-    Lr = class {
+    bd = de && Ve <= 11,
+    Br = class {
         constructor() {
             this.anchorNode = null, this.anchorOffset = 0, this.focusNode = null, this.focusOffset = 0
         }
         set(e) {
             this.anchorNode = e.anchorNode, this.anchorOffset = e.anchorOffset, this.focusNode = e.focusNode, this.focusOffset = e.focusOffset
         }
         clear() {
             this.anchorNode = this.focusNode = null
         }
         eq(e) {
             return e.anchorNode == this.anchorNode && e.anchorOffset == this.anchorOffset && e.focusNode == this.focusNode && e.focusOffset == this.focusOffset
         }
     },
-    Br = class {
+    Fr = class {
         constructor(e, t) {
-            this.view = e, this.handleDOMChange = t, this.queue = [], this.flushingSoon = -1, this.observer = null, this.currentSelection = new Lr, this.onCharData = null, this.suppressingSelectionUpdates = !1, this.observer = window.MutationObserver && new window.MutationObserver(r => {
+            this.view = e, this.handleDOMChange = t, this.queue = [], this.flushingSoon = -1, this.observer = null, this.currentSelection = new Br, this.onCharData = null, this.suppressingSelectionUpdates = !1, this.observer = window.MutationObserver && new window.MutationObserver(r => {
                 for (let i = 0; i < r.length; i++) this.queue.push(r[i]);
                 de && Ve <= 11 && r.some(i => i.type == "childList" && i.removedNodes.length || i.type == "characterData" && i.oldValue.length > i.target.nodeValue.length) ? this.flushSoon() : this.flush()
-            }), gd && (this.onCharData = r => {
+            }), bd && (this.onCharData = r => {
                 this.queue.push({
                     target: r.target,
                     type: "characterData",
                     oldValue: r.prevValue
                 }), this.flushSoon()
             }), this.onSelectionChange = this.onSelectionChange.bind(this)
         }
@@ -6905,15 +6915,15 @@
                 this.flushingSoon = -1, this.flush()
             }, 20))
         }
         forceFlush() {
             this.flushingSoon > -1 && (window.clearTimeout(this.flushingSoon), this.flushingSoon = -1, this.flush())
         }
         start() {
-            this.observer && (this.observer.takeRecords(), this.observer.observe(this.view.dom, md)), this.onCharData && this.view.dom.addEventListener("DOMCharacterDataModified", this.onCharData), this.connectSelection()
+            this.observer && (this.observer.takeRecords(), this.observer.observe(this.view.dom, xd)), this.onCharData && this.view.dom.addEventListener("DOMCharacterDataModified", this.onCharData), this.connectSelection()
         }
         stop() {
             if (this.observer) {
                 let e = this.observer.takeRecords();
                 if (e.length) {
                     for (let t = 0; t < e.length; t++) this.queue.push(e[t]);
                     window.setTimeout(() => this.flush(), 20)
@@ -6987,15 +6997,15 @@
                 if (d.length == 2) {
                     let u = d[0],
                         f = d[1];
                     u.parentNode && u.parentNode.parentNode == f.parentNode ? f.remove() : u.remove()
                 }
             }
             let c = null;
-            s < 0 && i && e.input.lastFocus > Date.now() - 200 && Math.max(e.input.lastTouch, e.input.lastClick.time) < Date.now() - 300 && vn(r) && (c = zr(e)) && c.eq(L.near(e.state.doc.resolve(0), 1)) ? (e.input.lastFocus = 0, Re(e), this.currentSelection.set(r), e.scrollToSelection()) : (s > -1 || i) && (s > -1 && (e.docView.markDirty(s, o), yd(e)), this.handleDOMChange(s, o, l, a), e.docView && e.docView.dirty ? e.updateState(e.state) : this.currentSelection.eq(r) || Re(e), this.currentSelection.set(r))
+            s < 0 && i && e.input.lastFocus > Date.now() - 200 && Math.max(e.input.lastTouch, e.input.lastClick.time) < Date.now() - 300 && vn(r) && (c = $r(e)) && c.eq(L.near(e.state.doc.resolve(0), 1)) ? (e.input.lastFocus = 0, Re(e), this.currentSelection.set(r), e.scrollToSelection()) : (s > -1 || i) && (s > -1 && (e.docView.markDirty(s, o), kd(e)), this.handleDOMChange(s, o, l, a), e.docView && e.docView.dirty ? e.updateState(e.state) : this.currentSelection.eq(r) || Re(e), this.currentSelection.set(r))
         }
         registerMutation(e, t) {
             if (t.indexOf(e.target) > -1) return null;
             let r = this.view.docView.nearestDesc(e.target);
             if (e.type == "attributes" && (r == this.view.docView || e.attributeName == "contenteditable" || e.attributeName == "style" && !e.oldValue && !e.target.getAttribute("style")) || !r || r.ignoreMutation(e)) return null;
             if (e.type == "childList") {
                 for (let d = 0; d < e.addedNodes.length; d++) t.push(e.addedNodes[d]);
@@ -7030,42 +7040,49 @@
                 typeOver: e.target.nodeValue == e.oldValue
             }
         }
     },
     no = new WeakMap,
     ro = !1;
 
-function yd(n) {
+function kd(n) {
     if (!no.has(n) && (no.set(n, null), ["normal", "nowrap", "pre-line"].indexOf(getComputedStyle(n.dom).whiteSpace) !== -1)) {
         if (n.requiresGeckoHackNode = ke, ro) return;
         console.warn("ProseMirror expects the CSS white-space property to be set, preferably to 'pre-wrap'. It is recommended to load style/prosemirror.css from the prosemirror-view package."), ro = !0
     }
 }
 
-function xd(n) {
-    let e;
+function io(n, e) {
+    let t = e.startContainer,
+        r = e.startOffset,
+        i = e.endContainer,
+        s = e.endOffset,
+        o = n.domAtPos(n.state.selection.anchor);
+    return at(o.node, o.offset, i, s) && ([t, r, i, s] = [i, s, t, r]), {
+        anchorNode: t,
+        anchorOffset: r,
+        focusNode: i,
+        focusOffset: s
+    }
+}
 
-    function t(a) {
-        a.preventDefault(), a.stopImmediatePropagation(), e = a.getTargetRanges()[0]
+function Sd(n, e) {
+    if (e.getComposedRanges) {
+        let i = e.getComposedRanges(n.root)[0];
+        if (i) return io(n, i)
     }
-    n.dom.addEventListener("beforeinput", t, !0), document.execCommand("indent"), n.dom.removeEventListener("beforeinput", t, !0);
-    let r = e.startContainer,
-        i = e.startOffset,
-        s = e.endContainer,
-        o = e.endOffset,
-        l = n.domAtPos(n.state.selection.anchor);
-    return at(l.node, l.offset, s, o) && ([r, i, s, o] = [s, o, r, i]), {
-        anchorNode: r,
-        anchorOffset: i,
-        focusNode: s,
-        focusOffset: o
+    let t;
+
+    function r(i) {
+        i.preventDefault(), i.stopImmediatePropagation(), t = i.getTargetRanges()[0]
     }
+    return n.dom.addEventListener("beforeinput", r, !0), document.execCommand("indent"), n.dom.removeEventListener("beforeinput", r, !0), t ? io(n, t) : null
 }
 
-function bd(n, e, t) {
+function Md(n, e, t) {
     let {
         node: r,
         fromOffset: i,
         toOffset: s,
         from: o,
         to: l
     } = n.docView.parseRange(e, t), a = n.domSelectionRange(), c, d = a.anchorNode;
@@ -7093,15 +7110,15 @@
             topNode: h.parent,
             topMatch: h.parent.contentMatchAt(h.index()),
             topOpen: !0,
             from: i,
             to: s,
             preserveWhitespace: h.parent.type.whitespace == "pre" ? "full" : !0,
             findPositions: c,
-            ruleFromNode: kd,
+            ruleFromNode: wd,
             context: h
         });
     if (c && c[0].pos != null) {
         let g = c[0].pos,
             k = c[1] && c[1].pos;
         k == null && (k = g), p = {
             anchor: g + o,
@@ -7112,15 +7129,15 @@
         doc: m,
         sel: p,
         from: o,
         to: l
     }
 }
 
-function kd(n) {
+function wd(n) {
     let e = n.pmViewDesc;
     if (e) return e.parseRule();
     if (n.nodeName == "BR" && n.parentNode) {
         if (le && /^(ul|ol)$/i.test(n.parentNode.nodeName)) {
             let t = document.createElement("div");
             return t.appendChild(document.createElement("li")), {
                 skip: t
@@ -7129,192 +7146,192 @@
             ignore: !0
         }
     } else if (n.nodeName == "IMG" && n.getAttribute("mark-placeholder")) return {
         ignore: !0
     };
     return null
 }
-var Sd = /^(a|abbr|acronym|b|bd[io]|big|br|button|cite|code|data(list)?|del|dfn|em|i|ins|kbd|label|map|mark|meter|output|q|ruby|s|samp|small|span|strong|su[bp]|time|u|tt|var)$/i;
+var Ed = /^(a|abbr|acronym|b|bd[io]|big|br|button|cite|code|data(list)?|del|dfn|em|i|ins|kbd|label|map|mark|meter|output|q|ruby|s|samp|small|span|strong|su[bp]|time|u|tt|var)$/i;
 
-function Md(n, e, t, r, i) {
+function Cd(n, e, t, r, i) {
     let s = n.input.compositionPendingChanges || (n.composing ? n.input.compositionID : 0);
     if (n.input.compositionPendingChanges = 0, e < 0) {
         let x = n.input.lastSelectionTime > Date.now() - 50 ? n.input.lastSelectionOrigin : null,
-            N = zr(n, x);
+            N = $r(n, x);
         if (N && !n.state.selection.eq(N)) {
             if (oe && be && n.input.lastKeyCode === 13 && Date.now() - 100 < n.input.lastKeyCodeTime && n.someProp("handleKeyDown", ne => ne(n, nt(13, "Enter")))) return;
             let V = n.state.tr.setSelection(N);
             x == "pointer" ? V.setMeta("pointer", !0) : x == "key" && V.scrollIntoView(), s && V.setMeta("composition", s), n.dispatch(V)
         }
         return
     }
     let o = n.state.doc.resolve(e),
         l = o.sharedDepth(t);
     e = o.before(l + 1), t = n.state.doc.resolve(t).after(l + 1);
     let a = n.state.selection,
-        c = bd(n, e, t),
+        c = Md(n, e, t),
         d = n.state.doc,
         u = d.slice(c.from, c.to),
         f, h;
     n.input.lastKeyCode === 8 && Date.now() - 100 < n.input.lastKeyCodeTime ? (f = n.state.selection.to, h = "end") : (f = n.state.selection.from, h = "start"), n.input.lastKeyCode = null;
-    let p = Cd(u.content, c.doc.content, c.from, f, h);
-    if ((wt && n.input.lastIOSEnter > Date.now() - 225 || be) && i.some(x => x.nodeType == 1 && !Sd.test(x.nodeName)) && (!p || p.endA >= p.endB) && n.someProp("handleKeyDown", x => x(n, nt(13, "Enter")))) {
+    let p = vd(u.content, c.doc.content, c.from, f, h);
+    if ((wt && n.input.lastIOSEnter > Date.now() - 225 || be) && i.some(x => x.nodeType == 1 && !Ed.test(x.nodeName)) && (!p || p.endA >= p.endB) && n.someProp("handleKeyDown", x => x(n, nt(13, "Enter")))) {
         n.input.lastIOSEnter = 0;
         return
     }
     if (!p)
         if (r && a instanceof P && !a.empty && a.$head.sameParent(a.$anchor) && !n.composing && !(c.sel && c.sel.anchor != c.sel.head)) p = {
             start: a.from,
             endA: a.to,
             endB: a.to
         };
         else {
             if (c.sel) {
-                let x = io(n, n.state.doc, c.sel);
+                let x = so(n, n.state.doc, c.sel);
                 if (x && !x.eq(n.state.selection)) {
                     let N = n.state.tr.setSelection(x);
                     s && N.setMeta("composition", s), n.dispatch(N)
                 }
             }
             return
         } n.input.domChangeCount++, n.state.selection.from < n.state.selection.to && p.start == p.endB && n.state.selection instanceof P && (p.start > n.state.selection.from && p.start <= n.state.selection.from + 2 && n.state.selection.from >= c.from ? p.start = n.state.selection.from : p.endA < n.state.selection.to && p.endA >= n.state.selection.to - 2 && n.state.selection.to <= c.to && (p.endB += n.state.selection.to - p.endA, p.endA = n.state.selection.to)), de && Ve <= 11 && p.endB == p.start + 1 && p.endA == p.start && p.start > c.from && c.doc.textBetween(p.start - c.from - 1, p.start - c.from + 1) == " \xA0" && (p.start--, p.endA--, p.endB--);
     let m = c.doc.resolveNoCache(p.start - c.from),
         g = c.doc.resolveNoCache(p.endB - c.from),
         k = d.resolve(p.start),
         R = m.sameParent(g) && m.parent.inlineContent && k.end() >= p.endA,
-        H;
-    if ((wt && n.input.lastIOSEnter > Date.now() - 225 && (!R || i.some(x => x.nodeName == "DIV" || x.nodeName == "P")) || !R && m.pos < c.doc.content.size && !m.sameParent(g) && (H = L.findFrom(c.doc.resolve(m.pos + 1), 1, !0)) && H.head == g.pos) && n.someProp("handleKeyDown", x => x(n, nt(13, "Enter")))) {
+        $;
+    if ((wt && n.input.lastIOSEnter > Date.now() - 225 && (!R || i.some(x => x.nodeName == "DIV" || x.nodeName == "P")) || !R && m.pos < c.doc.content.size && !m.sameParent(g) && ($ = L.findFrom(c.doc.resolve(m.pos + 1), 1, !0)) && $.head == g.pos) && n.someProp("handleKeyDown", x => x(n, nt(13, "Enter")))) {
         n.input.lastIOSEnter = 0;
         return
     }
-    if (n.state.selection.anchor > p.start && Ed(d, p.start, p.endA, m, g) && n.someProp("handleKeyDown", x => x(n, nt(8, "Backspace")))) {
+    if (n.state.selection.anchor > p.start && Ad(d, p.start, p.endA, m, g) && n.someProp("handleKeyDown", x => x(n, nt(8, "Backspace")))) {
         be && oe && n.domObserver.suppressSelectionUpdates();
         return
     }
     oe && be && p.endB == p.start && (n.input.lastAndroidDelete = Date.now()), be && !R && m.start() != g.start() && g.parentOffset == 0 && m.depth == g.depth && c.sel && c.sel.anchor == c.sel.head && c.sel.head == p.endA && (p.endB -= 2, g = c.doc.resolveNoCache(p.endB - c.from), setTimeout(() => {
         n.someProp("handleKeyDown", function(x) {
             return x(n, nt(13, "Enter"))
         })
     }, 20));
     let b = p.start,
         A = p.endA,
-        v, y, w;
+        v, y, M;
     if (R) {
         if (m.pos == g.pos) de && Ve <= 11 && m.parentOffset == 0 && (n.domObserver.suppressSelectionUpdates(), setTimeout(() => Re(n), 20)), v = n.state.tr.delete(b, A), y = d.resolve(p.start).marksAcross(d.resolve(p.endA));
-        else if (p.endA == p.endB && (w = wd(m.parent.content.cut(m.parentOffset, g.parentOffset), k.parent.content.cut(k.parentOffset, p.endA - k.start())))) v = n.state.tr, w.type == "add" ? v.addMark(b, A, w.mark) : v.removeMark(b, A, w.mark);
+        else if (p.endA == p.endB && (M = Td(m.parent.content.cut(m.parentOffset, g.parentOffset), k.parent.content.cut(k.parentOffset, p.endA - k.start())))) v = n.state.tr, M.type == "add" ? v.addMark(b, A, M.mark) : v.removeMark(b, A, M.mark);
         else if (m.parent.child(m.index()).isText && m.index() == g.index() - (g.textOffset ? 0 : 1)) {
             let x = m.parent.textBetween(m.parentOffset, g.parentOffset);
             if (n.someProp("handleTextInput", N => N(n, b, A, x))) return;
             v = n.state.tr.insertText(x, b, A)
         }
     }
     if (v || (v = n.state.tr.replace(b, A, c.doc.slice(p.start - c.from, p.endB - c.from))), c.sel) {
-        let x = io(n, v.doc, c.sel);
+        let x = so(n, v.doc, c.sel);
         x && !(oe && be && n.composing && x.empty && (p.start != p.endB || n.input.lastAndroidDelete < Date.now() - 100) && (x.head == b || x.head == v.mapping.map(A) - 1) || de && x.empty && x.head == b) && v.setSelection(x)
     }
     y && v.ensureMarks(y), s && v.setMeta("composition", s), n.dispatch(v.scrollIntoView())
 }
 
-function io(n, e, t) {
-    return Math.max(t.anchor, t.head) > e.content.size ? null : $r(n, e.resolve(t.anchor), e.resolve(t.head))
+function so(n, e, t) {
+    return Math.max(t.anchor, t.head) > e.content.size ? null : Hr(n, e.resolve(t.anchor), e.resolve(t.head))
 }
 
-function wd(n, e) {
+function Td(n, e) {
     let t = n.firstChild.marks,
         r = e.firstChild.marks,
         i = t,
         s = r,
         o, l, a;
     for (let d = 0; d < r.length; d++) i = r[d].removeFromSet(i);
     for (let d = 0; d < t.length; d++) s = t[d].removeFromSet(s);
     if (i.length == 1 && s.length == 0) l = i[0], o = "add", a = d => d.mark(l.addToSet(d.marks));
     else if (i.length == 0 && s.length == 1) l = s[0], o = "remove", a = d => d.mark(l.removeFromSet(d.marks));
     else return null;
     let c = [];
     for (let d = 0; d < e.childCount; d++) c.push(a(e.child(d)));
-    if (M.from(c).eq(n)) return {
+    if (w.from(c).eq(n)) return {
         mark: l,
         type: o
     }
 }
 
-function Ed(n, e, t, r, i) {
-    if (t - e <= i.pos - r.pos || yr(r, !0, !1) < i.pos) return !1;
+function Ad(n, e, t, r, i) {
+    if (t - e <= i.pos - r.pos || xr(r, !0, !1) < i.pos) return !1;
     let s = n.resolve(e);
     if (!r.parent.isTextblock) {
         let l = s.nodeAfter;
         return l != null && t == e + l.nodeSize
     }
     if (s.parentOffset < s.parent.content.size || !s.parent.isTextblock) return !1;
-    let o = n.resolve(yr(s, !0, !0));
-    return !o.parent.isTextblock || o.pos > t || yr(o, !0, !1) < t ? !1 : r.parent.content.cut(r.parentOffset).eq(o.parent.content)
+    let o = n.resolve(xr(s, !0, !0));
+    return !o.parent.isTextblock || o.pos > t || xr(o, !0, !1) < t ? !1 : r.parent.content.cut(r.parentOffset).eq(o.parent.content)
 }
 
-function yr(n, e, t) {
+function xr(n, e, t) {
     let r = n.depth,
         i = e ? n.end() : n.pos;
     for (; r > 0 && (e || n.indexAfter(r) == n.node(r).childCount);) r--, i++, e = !1;
     if (t) {
         let s = n.node(r).maybeChild(n.indexAfter(r));
         for (; s && !s.isLeaf;) s = s.firstChild, i++
     }
     return i
 }
 
-function Cd(n, e, t, r, i) {
+function vd(n, e, t, r, i) {
     let s = n.findDiffStart(e, t);
     if (s == null) return null;
     let {
         a: o,
         b: l
     } = n.findDiffEnd(e, t + n.size, t + e.size);
     if (i == "end") {
         let a = Math.max(0, s - Math.min(o, l));
         r -= o + a - s
     }
     if (o < s && n.size < e.size) {
         let a = r <= s && r >= o ? s - r : 0;
-        s -= a, s && s < e.size && so(e.textBetween(s - 1, s + 1)) && (s += a ? 1 : -1), l = s + (l - o), o = s
+        s -= a, s && s < e.size && oo(e.textBetween(s - 1, s + 1)) && (s += a ? 1 : -1), l = s + (l - o), o = s
     } else if (l < s) {
         let a = r <= s && r >= l ? s - r : 0;
-        s -= a, s && s < n.size && so(n.textBetween(s - 1, s + 1)) && (s += a ? 1 : -1), o = s + (o - l), l = s
+        s -= a, s && s < n.size && oo(n.textBetween(s - 1, s + 1)) && (s += a ? 1 : -1), o = s + (o - l), l = s
     }
     return {
         start: s,
         endA: o,
         endB: l
     }
 }
 
-function so(n) {
+function oo(n) {
     if (n.length != 2) return !1;
     let e = n.charCodeAt(0),
         t = n.charCodeAt(1);
     return e >= 56320 && e <= 57343 && t >= 55296 && t <= 56319
 }
 var An = class {
     constructor(e, t) {
-        this._root = null, this.focused = !1, this.trackWrites = null, this.mounted = !1, this.markCursor = null, this.cursorWrapper = null, this.lastSelectedViewDesc = void 0, this.input = new Dr, this.prevDirectPlugins = [], this.pluginViews = [], this.requiresGeckoHackNode = !1, this.dragging = null, this._props = t, this.state = t.state, this.directPlugins = t.plugins || [], this.directPlugins.forEach(uo), this.dispatch = this.dispatch.bind(this), this.dom = e && e.mount || document.createElement("div"), e && (e.appendChild ? e.appendChild(this.dom) : typeof e == "function" ? e(this.dom) : e.mount && (this.mounted = !0)), this.editable = ao(this), lo(this), this.nodeViews = co(this), this.docView = Vs(this.state.doc, oo(this), gr(this), this.dom, this), this.domObserver = new Br(this, (r, i, s, o) => Md(this, r, i, s, o)), this.domObserver.start(), Yc(this), this.updatePluginViews()
+        this._root = null, this.focused = !1, this.trackWrites = null, this.mounted = !1, this.markCursor = null, this.cursorWrapper = null, this.lastSelectedViewDesc = void 0, this.input = new Ir, this.prevDirectPlugins = [], this.pluginViews = [], this.requiresGeckoHackNode = !1, this.dragging = null, this._props = t, this.state = t.state, this.directPlugins = t.plugins || [], this.directPlugins.forEach(fo), this.dispatch = this.dispatch.bind(this), this.dom = e && e.mount || document.createElement("div"), e && (e.appendChild ? e.appendChild(this.dom) : typeof e == "function" ? e(this.dom) : e.mount && (this.mounted = !0)), this.editable = co(this), ao(this), this.nodeViews = uo(this), this.docView = Vs(this.state.doc, lo(this), yr(this), this.dom, this), this.domObserver = new Fr(this, (r, i, s, o) => Cd(this, r, i, s, o)), this.domObserver.start(), Qc(this), this.updatePluginViews()
     }
     get composing() {
         return this.input.composing
     }
     get props() {
         if (this._props.state != this.state) {
             let e = this._props;
             this._props = {};
             for (let t in e) this._props[t] = e[t];
             this._props.state = this.state
         }
         return this._props
     }
     update(e) {
-        e.handleDOMEvents != this._props.handleDOMEvents && Ir(this);
+        e.handleDOMEvents != this._props.handleDOMEvents && Pr(this);
         let t = this._props;
-        this._props = e, e.plugins && (e.plugins.forEach(uo), this.directPlugins = e.plugins), this.updateStateInner(e.state, t)
+        this._props = e, e.plugins && (e.plugins.forEach(fo), this.directPlugins = e.plugins), this.updateStateInner(e.state, t)
     }
     setProps(e) {
         let t = {};
         for (let r in this._props) t[r] = this._props[r];
         t.state = this.state;
         for (let r in e) t[r] = e[r];
         this.update(t)
@@ -7323,36 +7340,36 @@
         this.updateStateInner(e, this._props)
     }
     updateStateInner(e, t) {
         var r;
         let i = this.state,
             s = !1,
             o = !1;
-        e.storedMarks && this.composing && (Bo(this), o = !0), this.state = e;
+        e.storedMarks && this.composing && (Fo(this), o = !0), this.state = e;
         let l = i.plugins != e.plugins || this._props.plugins != t.plugins;
         if (l || this._props.plugins != t.plugins || this._props.nodeViews != t.nodeViews) {
-            let h = co(this);
-            Ad(h, this.nodeViews) && (this.nodeViews = h, s = !0)
-        }(l || t.handleDOMEvents != this._props.handleDOMEvents) && Ir(this), this.editable = ao(this), lo(this);
-        let a = gr(this),
-            c = oo(this),
+            let h = uo(this);
+            Nd(h, this.nodeViews) && (this.nodeViews = h, s = !0)
+        }(l || t.handleDOMEvents != this._props.handleDOMEvents) && Pr(this), this.editable = co(this), ao(this);
+        let a = yr(this),
+            c = lo(this),
             d = i.plugins != e.plugins && !i.doc.eq(e.doc) ? "reset" : e.scrollToSelection > i.scrollToSelection ? "to selection" : "preserve",
             u = s || !this.docView.matchesNode(e.doc, c, a);
         (u || !e.selection.eq(i.selection)) && (o = !0);
-        let f = d == "preserve" && o && this.dom.style.overflowAnchor == null && mc(this);
+        let f = d == "preserve" && o && this.dom.style.overflowAnchor == null && xc(this);
         if (o) {
             this.domObserver.stop();
-            let h = u && (de || oe) && !this.composing && !i.selection.empty && !e.selection.empty && Td(i.selection, e.selection);
+            let h = u && (de || oe) && !this.composing && !i.selection.empty && !e.selection.empty && Od(i.selection, e.selection);
             if (u) {
                 let p = oe ? this.trackWrites = this.domSelectionRange().focusNode : null;
-                this.composing && (this.input.compositionNode = ad(this)), (s || !this.docView.update(e.doc, c, a, this)) && (this.docView.updateOuterDeco(c), this.docView.destroy(), this.docView = Vs(e.doc, c, a, this.dom, this)), p && !this.trackWrites && (h = !0)
+                this.composing && (this.input.compositionNode = ud(this)), (s || !this.docView.update(e.doc, c, a, this)) && (this.docView.updateOuterDeco(c), this.docView.destroy(), this.docView = Vs(e.doc, c, a, this.dom, this)), p && !this.trackWrites && (h = !0)
             }
-            h || !(this.input.mouseDown && this.domObserver.currentSelection.eq(this.domSelectionRange()) && Bc(this)) ? Re(this, h) : (wo(this, e.selection), this.domObserver.setCurSelection()), this.domObserver.start()
+            h || !(this.input.mouseDown && this.domObserver.currentSelection.eq(this.domSelectionRange()) && $c(this)) ? Re(this, h) : (Eo(this, e.selection), this.domObserver.setCurSelection()), this.domObserver.start()
         }
-        this.updatePluginViews(i), !((r = this.dragging) === null || r === void 0) && r.node && !i.doc.eq(e.doc) && this.updateDraggedNode(this.dragging, i), d == "reset" ? this.dom.scrollTop = 0 : d == "to selection" ? this.scrollToSelection() : f && gc(f)
+        this.updatePluginViews(i), !((r = this.dragging) === null || r === void 0) && r.node && !i.doc.eq(e.doc) && this.updateDraggedNode(this.dragging, i), d == "reset" ? this.dom.scrollTop = 0 : d == "to selection" ? this.scrollToSelection() : f && bc(f)
     }
     scrollToSelection() {
         let e = this.domSelectionRange().focusNode;
         if (!this.someProp("handleScrollToSelection", t => t(this)))
             if (this.state.selection instanceof O) {
                 let t = this.docView.domAfterPos(this.state.selection.from);
                 t.nodeType == 1 && Ls(this, t.getBoundingClientRect(), e)
@@ -7414,126 +7431,127 @@
                 e = e.parentElement
             }
             return !0
         }
         return this.root.activeElement == this.dom
     }
     focus() {
-        this.domObserver.stop(), this.editable && yc(this.dom), Re(this), this.domObserver.start()
+        this.domObserver.stop(), this.editable && kc(this.dom), Re(this), this.domObserver.start()
     }
     get root() {
         let e = this._root;
         if (e == null) {
             for (let t = this.dom.parentNode; t; t = t.parentNode)
                 if (t.nodeType == 9 || t.nodeType == 11 && t.host) return t.getSelection || (Object.getPrototypeOf(t).getSelection = () => t.ownerDocument.getSelection()), this._root = t
         }
         return e || document
     }
     updateRoot() {
         this._root = null
     }
     posAtCoords(e) {
-        return Mc(this, e)
+        return Cc(this, e)
     }
     coordsAtPos(e, t = 1) {
-        return yo(this, e, t)
+        return xo(this, e, t)
     }
     domAtPos(e, t = 0) {
         return this.docView.domFromPos(e, t)
     }
     nodeDOM(e) {
         let t = this.docView.descAt(e);
         return t ? t.nodeDOM : null
     }
     posAtDOM(e, t, r = -1) {
         let i = this.docView.posFromDOM(e, t, r);
         if (i == null) throw new RangeError("DOM position not inside the editor");
         return i
     }
     endOfTextblock(e, t) {
-        return Ac(this, t || this.state, e)
+        return Nc(this, t || this.state, e)
     }
     pasteHTML(e, t) {
         return _t(this, "", e, !1, t || new ClipboardEvent("paste"))
     }
     pasteText(e, t) {
         return _t(this, e, null, !0, t || new ClipboardEvent("paste"))
     }
     destroy() {
-        this.docView && (Xc(this), this.destroyPluginViews(), this.mounted ? (this.docView.update(this.state.doc, [], gr(this), this), this.dom.textContent = "") : this.dom.parentNode && this.dom.parentNode.removeChild(this.dom), this.docView.destroy(), this.docView = null, rc())
+        this.docView && (ed(this), this.destroyPluginViews(), this.mounted ? (this.docView.update(this.state.doc, [], yr(this), this), this.dom.textContent = "") : this.dom.parentNode && this.dom.parentNode.removeChild(this.dom), this.docView.destroy(), this.docView = null, oc())
     }
     get isDestroyed() {
         return this.docView == null
     }
     dispatchEvent(e) {
-        return Qc(this, e)
+        return nd(this, e)
     }
     dispatch(e) {
         let t = this._props.dispatchTransaction;
         t ? t.call(this, e) : this.updateState(this.state.apply(e))
     }
     domSelectionRange() {
-        return le && this.root.nodeType === 11 && ac(this.dom.ownerDocument) == this.dom ? xd(this) : this.domSelection()
+        let e = this.domSelection();
+        return le && this.root.nodeType === 11 && uc(this.dom.ownerDocument) == this.dom && Sd(this, e) || e
     }
     domSelection() {
         return this.root.getSelection()
     }
 };
 
-function oo(n) {
+function lo(n) {
     let e = Object.create(null);
     return e.class = "ProseMirror", e.contenteditable = String(n.editable), n.someProp("attributes", t => {
         if (typeof t == "function" && (t = t(n.state)), t)
             for (let r in t) r == "class" ? e.class += " " + t[r] : r == "style" ? e.style = (e.style ? e.style + ";" : "") + t[r] : !e[r] && r != "contenteditable" && r != "nodeName" && (e[r] = String(t[r]))
     }), e.translate || (e.translate = "no"), [Ee.node(0, n.state.doc.content.size, e)]
 }
 
-function lo(n) {
+function ao(n) {
     if (n.markCursor) {
         let e = document.createElement("img");
         e.className = "ProseMirror-separator", e.setAttribute("mark-placeholder", "true"), e.setAttribute("alt", ""), n.cursorWrapper = {
             dom: e,
             deco: Ee.widget(n.state.selection.head, e, {
                 raw: !0,
                 marks: n.markCursor
             })
         }
     } else n.cursorWrapper = null
 }
 
-function ao(n) {
+function co(n) {
     return !n.someProp("editable", e => e(n.state) === !1)
 }
 
-function Td(n, e) {
+function Od(n, e) {
     let t = Math.min(n.$anchor.sharedDepth(n.head), e.$anchor.sharedDepth(e.head));
     return n.$anchor.start(t) != e.$anchor.start(t)
 }
 
-function co(n) {
+function uo(n) {
     let e = Object.create(null);
 
     function t(r) {
         for (let i in r) Object.prototype.hasOwnProperty.call(e, i) || (e[i] = r[i])
     }
     return n.someProp("nodeViews", t), n.someProp("markViews", t), e
 }
 
-function Ad(n, e) {
+function Nd(n, e) {
     let t = 0,
         r = 0;
     for (let i in n) {
         if (n[i] != e[i]) return !0;
         t++
     }
     for (let i in e) r++;
     return t != r
 }
 
-function uo(n) {
+function fo(n) {
     if (n.spec.state || n.spec.filterTransaction || n.spec.appendTransaction) throw new RangeError("Plugins passed directly to the view must not have a state component")
 }
 var Le = {
         8: "Backspace",
         9: "Tab",
         10: "Enter",
         12: "NumLock",
@@ -7608,131 +7626,131 @@
         191: "?",
         192: "~",
         219: "{",
         220: "|",
         221: "}",
         222: '"'
     },
-    vd = typeof navigator < "u" && /Mac/.test(navigator.platform),
-    Od = typeof navigator < "u" && /MSIE \d|Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(navigator.userAgent);
+    Dd = typeof navigator < "u" && /Mac/.test(navigator.platform),
+    Id = typeof navigator < "u" && /MSIE \d|Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(navigator.userAgent);
 for (_ = 0; _ < 10; _++) Le[48 + _] = Le[96 + _] = String(_);
 var _;
 for (_ = 1; _ <= 24; _++) Le[_ + 111] = "F" + _;
 var _;
 for (_ = 65; _ <= 90; _++) Le[_] = String.fromCharCode(_ + 32), Dn[_] = String.fromCharCode(_);
 var _;
 for (Nn in Le) Dn.hasOwnProperty(Nn) || (Dn[Nn] = Le[Nn]);
 var Nn;
 
-function jo(n) {
-    var e = vd && n.metaKey && n.shiftKey && !n.ctrlKey && !n.altKey || Od && n.shiftKey && n.key && n.key.length == 1 || n.key == "Unidentified",
+function Jo(n) {
+    var e = Dd && n.metaKey && n.shiftKey && !n.ctrlKey && !n.altKey || Id && n.shiftKey && n.key && n.key.length == 1 || n.key == "Unidentified",
         t = !e && n.key || (n.shiftKey ? Dn : Le)[n.keyCode] || n.key || "Unidentified";
     return t == "Esc" && (t = "Escape"), t == "Del" && (t = "Delete"), t == "Left" && (t = "ArrowLeft"), t == "Up" && (t = "ArrowUp"), t == "Right" && (t = "ArrowRight"), t == "Down" && (t = "ArrowDown"), t
 }
-var Nd = typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : !1;
+var Pd = typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : !1;
 
-function Dd(n) {
+function Rd(n) {
     let e = n.split(/-(?!$)/),
         t = e[e.length - 1];
     t == "Space" && (t = " ");
     let r, i, s, o;
     for (let l = 0; l < e.length - 1; l++) {
         let a = e[l];
         if (/^(cmd|meta|m)$/i.test(a)) o = !0;
         else if (/^a(lt)?$/i.test(a)) r = !0;
         else if (/^(c|ctrl|control)$/i.test(a)) i = !0;
         else if (/^s(hift)?$/i.test(a)) s = !0;
-        else if (/^mod$/i.test(a)) Nd ? o = !0 : i = !0;
+        else if (/^mod$/i.test(a)) Pd ? o = !0 : i = !0;
         else throw new Error("Unrecognized modifier name: " + a)
     }
     return r && (t = "Alt-" + t), i && (t = "Ctrl-" + t), o && (t = "Meta-" + t), s && (t = "Shift-" + t), t
 }
 
-function Id(n) {
+function Ld(n) {
     let e = Object.create(null);
-    for (let t in n) e[Dd(t)] = n[t];
+    for (let t in n) e[Rd(t)] = n[t];
     return e
 }
 
-function qr(n, e, t = !0) {
+function Wr(n, e, t = !0) {
     return e.altKey && (n = "Alt-" + n), e.ctrlKey && (n = "Ctrl-" + n), e.metaKey && (n = "Meta-" + n), t && e.shiftKey && (n = "Shift-" + n), n
 }
 
-function Jo(n) {
+function qo(n) {
     return new W({
         props: {
-            handleKeyDown: Pd(n)
+            handleKeyDown: Bd(n)
         }
     })
 }
 
-function Pd(n) {
-    let e = Id(n);
+function Bd(n) {
+    let e = Ld(n);
     return function(t, r) {
-        let i = jo(r),
-            s, o = e[qr(i, r)];
+        let i = Jo(r),
+            s, o = e[Wr(i, r)];
         if (o && o(t.state, t.dispatch, t)) return !0;
         if (i.length == 1 && i != " ") {
             if (r.shiftKey) {
-                let l = e[qr(i, r, !1)];
+                let l = e[Wr(i, r, !1)];
                 if (l && l(t.state, t.dispatch, t)) return !0
             }
             if ((r.shiftKey || r.altKey || r.metaKey || i.charCodeAt(0) > 127) && (s = Le[r.keyCode]) && s != i) {
-                let l = e[qr(s, r)];
+                let l = e[Wr(s, r)];
                 if (l && l(t.state, t.dispatch, t)) return !0
             }
         }
         return !1
     }
 }
 var In = (n, e) => n.selection.empty ? !1 : (e && e(n.tr.deleteSelection().scrollIntoView()), !0);
 
-function Wo(n, e) {
+function Ko(n, e) {
     let {
         $cursor: t
     } = n.selection;
     return !t || (e ? !e.endOfTextblock("backward", n) : t.parentOffset > 0) ? null : t
 }
-var Kr = (n, e, t) => {
-        let r = Wo(n, t);
+var Ur = (n, e, t) => {
+        let r = Ko(n, t);
         if (!r) return !1;
-        let i = _r(r);
+        let i = Gr(r);
         if (!i) {
             let o = r.blockRange(),
                 l = o && De(o);
             return l == null ? !1 : (e && e(n.tr.lift(o, l).scrollIntoView()), !0)
         }
         let s = i.nodeBefore;
-        if (!s.type.spec.isolating && el(n, i, e)) return !0;
+        if (!s.type.spec.isolating && tl(n, i, e)) return !0;
         if (r.parent.content.size == 0 && (Ct(s, "end") || O.isSelectable(s))) {
             let o = Vt(n.doc, r.before(), r.after(), E.empty);
             if (o && o.slice.size < o.to - o.from) {
                 if (e) {
                     let l = n.tr.step(o);
                     l.setSelection(Ct(s, "end") ? L.findFrom(l.doc.resolve(l.mapping.map(i.pos, -1)), -1) : O.create(l.doc, i.pos - s.nodeSize)), e(l.scrollIntoView())
                 }
                 return !0
             }
         }
         return s.isAtom && i.depth == r.depth - 1 ? (e && e(n.tr.delete(i.pos - s.nodeSize, i.pos).scrollIntoView()), !0) : !1
     },
-    Ko = (n, e, t) => {
-        let r = Wo(n, t);
+    Uo = (n, e, t) => {
+        let r = Ko(n, t);
         if (!r) return !1;
-        let i = _r(r);
-        return i ? _o(n, i, e) : !1
+        let i = Gr(r);
+        return i ? Go(n, i, e) : !1
     },
-    Uo = (n, e, t) => {
-        let r = Go(n, t);
+    _o = (n, e, t) => {
+        let r = Yo(n, t);
         if (!r) return !1;
-        let i = Xr(r);
-        return i ? _o(n, i, e) : !1
+        let i = Zr(r);
+        return i ? Go(n, i, e) : !1
     };
 
-function _o(n, e, t) {
+function Go(n, e, t) {
     let r = e.nodeBefore,
         i = r,
         s = e.pos - 1;
     for (; !i.isTextblock; s--) {
         if (i.type.spec.isolating) return !1;
         let d = i.lastChild;
         if (!d) return !1;
@@ -7759,193 +7777,193 @@
 function Ct(n, e, t = !1) {
     for (let r = n; r; r = e == "start" ? r.firstChild : r.lastChild) {
         if (r.isTextblock) return !0;
         if (t && r.childCount != 1) return !1
     }
     return !1
 }
-var Ur = (n, e, t) => {
+var _r = (n, e, t) => {
     let {
         $head: r,
         empty: i
     } = n.selection, s = r;
     if (!i) return !1;
     if (r.parent.isTextblock) {
         if (t ? !t.endOfTextblock("backward", n) : r.parentOffset > 0) return !1;
-        s = _r(r)
+        s = Gr(r)
     }
     let o = s && s.nodeBefore;
     return !o || !O.isSelectable(o) ? !1 : (e && e(n.tr.setSelection(O.create(n.doc, s.pos - o.nodeSize)).scrollIntoView()), !0)
 };
 
-function _r(n) {
+function Gr(n) {
     if (!n.parent.type.spec.isolating)
         for (let e = n.depth - 1; e >= 0; e--) {
             if (n.index(e) > 0) return n.doc.resolve(n.before(e + 1));
             if (n.node(e).type.spec.isolating) break
         }
     return null
 }
 
-function Go(n, e) {
+function Yo(n, e) {
     let {
         $cursor: t
     } = n.selection;
     return !t || (e ? !e.endOfTextblock("forward", n) : t.parentOffset < t.parent.content.size) ? null : t
 }
-var Gr = (n, e, t) => {
-        let r = Go(n, t);
+var Yr = (n, e, t) => {
+        let r = Yo(n, t);
         if (!r) return !1;
-        let i = Xr(r);
+        let i = Zr(r);
         if (!i) return !1;
         let s = i.nodeAfter;
-        if (el(n, i, e)) return !0;
+        if (tl(n, i, e)) return !0;
         if (r.parent.content.size == 0 && (Ct(s, "start") || O.isSelectable(s))) {
             let o = Vt(n.doc, r.before(), r.after(), E.empty);
             if (o && o.slice.size < o.to - o.from) {
                 if (e) {
                     let l = n.tr.step(o);
                     l.setSelection(Ct(s, "start") ? L.findFrom(l.doc.resolve(l.mapping.map(i.pos)), 1) : O.create(l.doc, l.mapping.map(i.pos))), e(l.scrollIntoView())
                 }
                 return !0
             }
         }
         return s.isAtom && i.depth == r.depth - 1 ? (e && e(n.tr.delete(i.pos, i.pos + s.nodeSize).scrollIntoView()), !0) : !1
     },
-    Yr = (n, e, t) => {
+    Xr = (n, e, t) => {
         let {
             $head: r,
             empty: i
         } = n.selection, s = r;
         if (!i) return !1;
         if (r.parent.isTextblock) {
             if (t ? !t.endOfTextblock("forward", n) : r.parentOffset < r.parent.content.size) return !1;
-            s = Xr(r)
+            s = Zr(r)
         }
         let o = s && s.nodeAfter;
         return !o || !O.isSelectable(o) ? !1 : (e && e(n.tr.setSelection(O.create(n.doc, s.pos)).scrollIntoView()), !0)
     };
 
-function Xr(n) {
+function Zr(n) {
     if (!n.parent.type.spec.isolating)
         for (let e = n.depth - 1; e >= 0; e--) {
             let t = n.node(e);
             if (n.index(e) + 1 < t.childCount) return n.doc.resolve(n.after(e + 1));
             if (t.type.spec.isolating) break
         }
     return null
 }
-var Yo = (n, e) => {
+var Xo = (n, e) => {
         let t = n.selection,
             r = t instanceof O,
             i;
         if (r) {
             if (t.node.isTextblock || !xe(n.doc, t.from)) return !1;
             i = t.from
         } else if (i = yt(n.doc, t.from, -1), i == null) return !1;
         if (e) {
             let s = n.tr.join(i);
             r && s.setSelection(O.create(s.doc, i - n.doc.resolve(i).nodeBefore.nodeSize)), e(s.scrollIntoView())
         }
         return !0
     },
-    Xo = (n, e) => {
+    Zo = (n, e) => {
         let t = n.selection,
             r;
         if (t instanceof O) {
             if (t.node.isTextblock || !xe(n.doc, t.to)) return !1;
             r = t.to
         } else if (r = yt(n.doc, t.to, 1), r == null) return !1;
         return e && e(n.tr.join(r).scrollIntoView()), !0
     },
-    Zo = (n, e) => {
+    Qo = (n, e) => {
         let {
             $from: t,
             $to: r
         } = n.selection, i = t.blockRange(r), s = i && De(i);
         return s == null ? !1 : (e && e(n.tr.lift(i, s).scrollIntoView()), !0)
     },
-    Zr = (n, e) => {
+    Qr = (n, e) => {
         let {
             $head: t,
             $anchor: r
         } = n.selection;
         return !t.parent.type.spec.code || !t.sameParent(r) ? !1 : (e && e(n.tr.insertText(`
 `).scrollIntoView()), !0)
     };
 
-function Qr(n) {
+function ei(n) {
     for (let e = 0; e < n.edgeCount; e++) {
         let {
             type: t
         } = n.edge(e);
         if (t.isTextblock && !t.hasRequiredAttrs()) return t
     }
     return null
 }
-var ei = (n, e) => {
+var ti = (n, e) => {
         let {
             $head: t,
             $anchor: r
         } = n.selection;
         if (!t.parent.type.spec.code || !t.sameParent(r)) return !1;
         let i = t.node(-1),
             s = t.indexAfter(-1),
-            o = Qr(i.contentMatchAt(s));
+            o = ei(i.contentMatchAt(s));
         if (!o || !i.canReplaceWith(s, s, o)) return !1;
         if (e) {
             let l = t.after(),
                 a = n.tr.replaceWith(l, l, o.createAndFill());
             a.setSelection(L.near(a.doc.resolve(l), 1)), e(a.scrollIntoView())
         }
         return !0
     },
-    ti = (n, e) => {
+    ni = (n, e) => {
         let t = n.selection,
             {
                 $from: r,
                 $to: i
             } = t;
         if (t instanceof fe || r.parent.inlineContent || i.parent.inlineContent) return !1;
-        let s = Qr(i.parent.contentMatchAt(i.indexAfter()));
+        let s = ei(i.parent.contentMatchAt(i.indexAfter()));
         if (!s || !s.isTextblock) return !1;
         if (e) {
             let o = (!r.parentOffset && i.index() < i.parent.childCount ? r : i).pos,
                 l = n.tr.insert(o, s.createAndFill());
             l.setSelection(P.create(l.doc, o + 1)), e(l.scrollIntoView())
         }
         return !0
     },
-    ni = (n, e) => {
+    ri = (n, e) => {
         let {
             $cursor: t
         } = n.selection;
         if (!t || t.parent.content.size) return !1;
         if (t.depth > 1 && t.after() != t.end(-1)) {
             let s = t.before();
             if (pe(n.doc, s)) return e && e(n.tr.split(s).scrollIntoView()), !0
         }
         let r = t.blockRange(),
             i = r && De(r);
         return i == null ? !1 : (e && e(n.tr.lift(r, i).scrollIntoView()), !0)
     };
 
-function Rd(n) {
+function Fd(n) {
     return (e, t) => {
         let {
             $from: r,
             $to: i
         } = e.selection;
         if (e.selection instanceof O && e.selection.node.isBlock) return !r.parentOffset || !pe(e.doc, r.pos) ? !1 : (t && t(e.tr.split(r.pos).scrollIntoView()), !0);
         if (!r.parent.isBlock) return !1;
         if (t) {
             let s = i.parentOffset == i.parent.content.size,
                 o = e.tr;
             (e.selection instanceof P || e.selection instanceof fe) && o.deleteSelection();
-            let l = r.depth == 0 ? null : Qr(r.node(-1).contentMatchAt(r.indexAfter(-1))),
+            let l = r.depth == 0 ? null : ei(r.node(-1).contentMatchAt(r.indexAfter(-1))),
                 a = n && n(i.parent, s),
                 c = a ? [a] : s && l ? [{
                     type: l
                 }] : void 0,
                 d = pe(o.doc, o.mapping.map(r.pos), 1, c);
             if (!c && !d && pe(o.doc, o.mapping.map(r.pos), 1, l ? [{
                     type: l
@@ -7957,44 +7975,44 @@
                 l && r.node(-1).canReplaceWith(f.index(), f.index() + 1, l) && o.setNodeMarkup(o.mapping.map(r.before()), l)
             }
             t(o.scrollIntoView())
         }
         return !0
     }
 }
-var Ld = Rd();
-var Qo = (n, e) => {
+var zd = Fd();
+var el = (n, e) => {
         let {
             $from: t,
             to: r
         } = n.selection, i, s = t.sharedDepth(r);
         return s == 0 ? !1 : (i = t.before(s), e && e(n.tr.setSelection(O.create(n.doc, i))), !0)
     },
-    Bd = (n, e) => (e && e(n.tr.setSelection(new fe(n.doc))), !0);
+    $d = (n, e) => (e && e(n.tr.setSelection(new fe(n.doc))), !0);
 
-function Fd(n, e, t) {
+function Hd(n, e, t) {
     let r = e.nodeBefore,
         i = e.nodeAfter,
         s = e.index();
     return !r || !i || !r.type.compatibleContent(i.type) ? !1 : !r.content.size && e.parent.canReplace(s - 1, s) ? (t && t(n.tr.delete(e.pos - r.nodeSize, e.pos).scrollIntoView()), !0) : !e.parent.canReplace(s, s + 1) || !(i.isTextblock || xe(n.doc, e.pos)) ? !1 : (t && t(n.tr.clearIncompatible(e.pos, r.type, r.contentMatchAt(r.childCount)).join(e.pos).scrollIntoView()), !0)
 }
 
-function el(n, e, t) {
+function tl(n, e, t) {
     let r = e.nodeBefore,
         i = e.nodeAfter,
         s, o;
     if (r.type.spec.isolating || i.type.spec.isolating) return !1;
-    if (Fd(n, e, t)) return !0;
+    if (Hd(n, e, t)) return !0;
     let l = e.parent.canReplace(e.index(), e.index() + 1);
     if (l && (s = (o = r.contentMatchAt(r.childCount)).findWrapping(i.type)) && o.matchType(s[0] || i.type).validEnd) {
         if (t) {
             let u = e.pos + i.nodeSize,
-                f = M.empty;
-            for (let m = s.length - 1; m >= 0; m--) f = M.from(s[m].create(null, f));
-            f = M.from(r.copy(f));
+                f = w.empty;
+            for (let m = s.length - 1; m >= 0; m--) f = w.from(s[m].create(null, f));
+            f = w.from(r.copy(f));
             let h = n.tr.step(new U(e.pos - 1, u, e.pos, u, new E(f, 1, 0), s.length, !0)),
                 p = u + 2 * s.length;
             xe(h.doc, p) && h.join(p), t(h.scrollIntoView())
         }
         return !0
     }
     let a = L.findFrom(e, 1),
@@ -8006,51 +8024,51 @@
             f = [];
         for (; f.push(u), !u.isTextblock;) u = u.lastChild;
         let h = i,
             p = 1;
         for (; !h.isTextblock; h = h.firstChild) p++;
         if (u.canReplace(u.childCount, u.childCount, h.content)) {
             if (t) {
-                let m = M.empty;
-                for (let k = f.length - 1; k >= 0; k--) m = M.from(f[k].copy(m));
+                let m = w.empty;
+                for (let k = f.length - 1; k >= 0; k--) m = w.from(f[k].copy(m));
                 let g = n.tr.step(new U(e.pos - f.length, e.pos + i.nodeSize, e.pos + p, e.pos + i.nodeSize - p, new E(m, f.length, 0), 0, !0));
                 t(g.scrollIntoView())
             }
             return !0
         }
     }
     return !1
 }
 
-function tl(n) {
+function nl(n) {
     return function(e, t) {
         let r = e.selection,
             i = n < 0 ? r.$from : r.$to,
             s = i.depth;
         for (; i.node(s).isInline;) {
             if (!s) return !1;
             s--
         }
         return i.node(s).isTextblock ? (t && t(e.tr.setSelection(P.create(e.doc, n < 0 ? i.start(s) : i.end(s)))), !0) : !1
     }
 }
-var ri = tl(-1),
-    ii = tl(1);
+var ii = nl(-1),
+    si = nl(1);
 
-function nl(n, e = null) {
+function rl(n, e = null) {
     return function(t, r) {
         let {
             $from: i,
             $to: s
         } = t.selection, o = i.blockRange(s), l = o && gt(o, n, e);
         return l ? (r && r(t.tr.wrap(o, l).scrollIntoView()), !0) : !1
     }
 }
 
-function si(n, e = null) {
+function oi(n, e = null) {
     return function(t, r) {
         let i = !1;
         for (let s = 0; s < t.selection.ranges.length && !i; s++) {
             let {
                 $from: {
                     pos: o
                 },
@@ -8085,140 +8103,140 @@
             }
             r(s.scrollIntoView())
         }
         return !0
     }
 }
 
-function oi(...n) {
+function li(...n) {
     return function(e, t, r) {
         for (let i = 0; i < n.length; i++)
             if (n[i](e, t, r)) return !0;
         return !1
     }
 }
-var Wr = oi(In, Kr, Ur),
-    qo = oi(In, Gr, Yr),
+var Kr = li(In, Ur, _r),
+    Wo = li(In, Yr, Xr),
     qe = {
-        Enter: oi(Zr, ti, ni, Ld),
-        "Mod-Enter": ei,
-        Backspace: Wr,
-        "Mod-Backspace": Wr,
-        "Shift-Backspace": Wr,
-        Delete: qo,
-        "Mod-Delete": qo,
-        "Mod-a": Bd
+        Enter: li(Qr, ni, ri, zd),
+        "Mod-Enter": ti,
+        Backspace: Kr,
+        "Mod-Backspace": Kr,
+        "Shift-Backspace": Kr,
+        Delete: Wo,
+        "Mod-Delete": Wo,
+        "Mod-a": $d
     },
-    zd = {
+    Vd = {
         "Ctrl-h": qe.Backspace,
         "Alt-Backspace": qe["Mod-Backspace"],
         "Ctrl-d": qe.Delete,
         "Ctrl-Alt-Backspace": qe["Mod-Delete"],
         "Alt-Delete": qe["Mod-Delete"],
         "Alt-d": qe["Mod-Delete"],
-        "Ctrl-a": ri,
-        "Ctrl-e": ii
+        "Ctrl-a": ii,
+        "Ctrl-e": si
     };
-for (let n in qe) zd[n] = qe[n];
-var Dh = typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : typeof os < "u" && os.platform ? os.platform() == "darwin" : !1;
+for (let n in qe) Vd[n] = qe[n];
+var Rh = typeof navigator < "u" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : typeof os < "u" && os.platform ? os.platform() == "darwin" : !1;
 
-function rl(n, e = null) {
+function il(n, e = null) {
     return function(t, r) {
         let {
             $from: i,
             $to: s
         } = t.selection, o = i.blockRange(s), l = !1, a = o;
         if (!o) return !1;
         if (o.depth >= 2 && i.node(o.depth - 1).type.compatibleContent(n) && o.startIndex == 0) {
             if (i.index(o.depth - 1) == 0) return !1;
             let d = t.doc.resolve(o.start - 2);
             a = new Xe(d, d, o.depth), o.endIndex < o.parent.childCount && (o = new Xe(i, t.doc.resolve(s.end(o.depth)), o.depth)), l = !0
         }
         let c = gt(a, n, e, o);
-        return c ? (r && r($d(t.tr, o, c, l, n).scrollIntoView()), !0) : !1
+        return c ? (r && r(jd(t.tr, o, c, l, n).scrollIntoView()), !0) : !1
     }
 }
 
-function $d(n, e, t, r, i) {
-    let s = M.empty;
-    for (let d = t.length - 1; d >= 0; d--) s = M.from(t[d].type.create(t[d].attrs, s));
+function jd(n, e, t, r, i) {
+    let s = w.empty;
+    for (let d = t.length - 1; d >= 0; d--) s = w.from(t[d].type.create(t[d].attrs, s));
     n.step(new U(e.start - (r ? 2 : 0), e.end, e.start, e.end, new E(s, 0, 0), t.length, !0));
     let o = 0;
     for (let d = 0; d < t.length; d++) t[d].type == i && (o = d + 1);
     let l = t.length - o,
         a = e.start + t.length - (r ? 2 : 0),
         c = e.parent;
     for (let d = e.startIndex, u = e.endIndex, f = !0; d < u; d++, f = !1) !f && pe(n.doc, a, l) && (n.split(a, l), a += 2 * l), a += c.child(d).nodeSize;
     return n
 }
 
-function il(n) {
+function sl(n) {
     return function(e, t) {
         let {
             $from: r,
             $to: i
         } = e.selection, s = r.blockRange(i, o => o.childCount > 0 && o.firstChild.type == n);
-        return s ? t ? r.node(s.depth - 1).type == n ? Hd(e, t, n, s) : Vd(e, t, s) : !0 : !1
+        return s ? t ? r.node(s.depth - 1).type == n ? Jd(e, t, n, s) : qd(e, t, s) : !0 : !1
     }
 }
 
-function Hd(n, e, t, r) {
+function Jd(n, e, t, r) {
     let i = n.tr,
         s = r.end,
         o = r.$to.end(r.depth);
-    s < o && (i.step(new U(s - 1, o, s, o, new E(M.from(t.create(null, r.parent.copy())), 1, 0), 1, !0)), r = new Xe(i.doc.resolve(r.$from.pos), i.doc.resolve(o), r.depth));
+    s < o && (i.step(new U(s - 1, o, s, o, new E(w.from(t.create(null, r.parent.copy())), 1, 0), 1, !0)), r = new Xe(i.doc.resolve(r.$from.pos), i.doc.resolve(o), r.depth));
     let l = De(r);
     if (l == null) return !1;
     i.lift(r, l);
     let a = i.mapping.map(s, -1) - 1;
     return xe(i.doc, a) && i.join(a), e(i.scrollIntoView()), !0
 }
 
-function Vd(n, e, t) {
+function qd(n, e, t) {
     let r = n.tr,
         i = t.parent;
     for (let h = t.end, p = t.endIndex - 1, m = t.startIndex; p > m; p--) h -= i.child(p).nodeSize, r.delete(h - 1, h + 1);
     let s = r.doc.resolve(t.start),
         o = s.nodeAfter;
     if (r.mapping.map(t.end) != t.start + s.nodeAfter.nodeSize) return !1;
     let l = t.startIndex == 0,
         a = t.endIndex == i.childCount,
         c = s.node(-1),
         d = s.index(-1);
-    if (!c.canReplace(d + (l ? 0 : 1), d + 1, o.content.append(a ? M.empty : M.from(i)))) return !1;
+    if (!c.canReplace(d + (l ? 0 : 1), d + 1, o.content.append(a ? w.empty : w.from(i)))) return !1;
     let u = s.pos,
         f = u + o.nodeSize;
-    return r.step(new U(u - (l ? 1 : 0), f + (a ? 1 : 0), u + 1, f - 1, new E((l ? M.empty : M.from(i.copy(M.empty))).append(a ? M.empty : M.from(i.copy(M.empty))), l ? 0 : 1, a ? 0 : 1), l ? 0 : 1)), e(r.scrollIntoView()), !0
+    return r.step(new U(u - (l ? 1 : 0), f + (a ? 1 : 0), u + 1, f - 1, new E((l ? w.empty : w.from(i.copy(w.empty))).append(a ? w.empty : w.from(i.copy(w.empty))), l ? 0 : 1, a ? 0 : 1), l ? 0 : 1)), e(r.scrollIntoView()), !0
 }
 
-function sl(n) {
+function ol(n) {
     return function(e, t) {
         let {
             $from: r,
             $to: i
         } = e.selection, s = r.blockRange(i, c => c.childCount > 0 && c.firstChild.type == n);
         if (!s) return !1;
         let o = s.startIndex;
         if (o == 0) return !1;
         let l = s.parent,
             a = l.child(o - 1);
         if (a.type != n) return !1;
         if (t) {
             let c = a.lastChild && a.lastChild.type == l.type,
-                d = M.from(c ? n.create() : null),
-                u = new E(M.from(n.create(null, M.from(l.type.create(null, d)))), c ? 3 : 1, 0),
+                d = w.from(c ? n.create() : null),
+                u = new E(w.from(n.create(null, w.from(l.type.create(null, d)))), c ? 3 : 1, 0),
                 f = s.start,
                 h = s.end;
             t(e.tr.step(new U(f - (c ? 3 : 1), h, f, h, u, 1, !0)).scrollIntoView())
         }
         return !0
     }
 }
 
-function Fn(n) {
+function zn(n) {
     let {
         state: e,
         transaction: t
     } = n, {
         selection: r
     } = t, {
         doc: i
@@ -8315,15 +8333,15 @@
                 state: s
             } = this, {
                 view: o
             } = i, l = {
                 tr: e,
                 editor: i,
                 view: o,
-                state: Fn({
+                state: zn({
                     state: s,
                     transaction: e
                 }),
                 dispatch: t ? () => {} : void 0,
                 chain: () => this.createChain(e, t),
                 can: () => this.createCan(e),
                 get commands() {
@@ -8356,31 +8374,31 @@
 function T(n, e, t) {
     return n.config[e] === void 0 && n.parent ? T(n.parent, e, t) : typeof n.config[e] == "function" ? n.config[e].bind({
         ...t,
         parent: n.parent ? T(n.parent, e, t) : null
     }) : n.config[e]
 }
 
-function zn(n) {
+function $n(n) {
     let e = n.filter(i => i.type === "extension"),
         t = n.filter(i => i.type === "node"),
         r = n.filter(i => i.type === "mark");
     return {
         baseExtensions: e,
         nodeExtensions: t,
         markExtensions: r
     }
 }
 
-function hl(n) {
+function pl(n) {
     let e = [],
         {
             nodeExtensions: t,
             markExtensions: r
-        } = zn(n),
+        } = $n(n),
         i = [...t, ...r],
         s = {
             default: null,
             rendered: !0,
             renderHTML: null,
             parseHTML: null,
             keepOnSplit: !0,
@@ -8461,79 +8479,79 @@
 
 function hi(n, e) {
     return e.filter(t => t.attribute.rendered).map(t => t.attribute.renderHTML ? t.attribute.renderHTML(n.attrs) || {} : {
         [t.name]: n.attrs[t.name]
     }).reduce((t, r) => z(t, r), {})
 }
 
-function pl(n) {
+function ml(n) {
     return typeof n == "function"
 }
 
 function B(n, e = void 0, ...t) {
-    return pl(n) ? e ? n.bind(e)(...t) : n(...t) : n
+    return ml(n) ? e ? n.bind(e)(...t) : n(...t) : n
 }
 
-function jd(n = {}) {
+function Wd(n = {}) {
     return Object.keys(n).length === 0 && n.constructor === Object
 }
 
-function Jd(n) {
+function Kd(n) {
     return typeof n != "string" ? n : n.match(/^[+-]?(?:\d*\.)?\d+$/) ? Number(n) : n === "true" ? !0 : n === "false" ? !1 : n
 }
 
-function ol(n, e) {
+function ll(n, e) {
     return n.style ? n : {
         ...n,
         getAttrs: t => {
             let r = n.getAttrs ? n.getAttrs(t) : n.attrs;
             if (r === !1) return !1;
             let i = e.reduce((s, o) => {
-                let l = o.attribute.parseHTML ? o.attribute.parseHTML(t) : Jd(t.getAttribute(o.name));
+                let l = o.attribute.parseHTML ? o.attribute.parseHTML(t) : Kd(t.getAttribute(o.name));
                 return l == null ? s : {
                     ...s,
                     [o.name]: l
                 }
             }, {});
             return {
                 ...r,
                 ...i
             }
         }
     }
 }
 
-function ll(n) {
-    return Object.fromEntries(Object.entries(n).filter(([e, t]) => e === "attrs" && jd(t) ? !1 : t != null))
+function al(n) {
+    return Object.fromEntries(Object.entries(n).filter(([e, t]) => e === "attrs" && Wd(t) ? !1 : t != null))
 }
 
-function qd(n, e) {
+function Ud(n, e) {
     var t;
-    let r = hl(n),
+    let r = pl(n),
         {
             nodeExtensions: i,
             markExtensions: s
-        } = zn(n),
+        } = $n(n),
         o = (t = i.find(c => T(c, "topNode"))) === null || t === void 0 ? void 0 : t.name,
         l = Object.fromEntries(i.map(c => {
             let d = r.filter(k => k.type === c.name),
                 u = {
                     name: c.name,
                     options: c.options,
                     storage: c.storage,
                     editor: e
                 },
                 f = n.reduce((k, R) => {
-                    let H = T(R, "extendNodeSchema", u);
+                    let $ = T(R, "extendNodeSchema", u);
                     return {
                         ...k,
-                        ...H ? H(c) : {}
+                        ...$ ? $(c) : {}
                     }
                 }, {}),
-                h = ll({
+                h = al({
                     ...f,
                     content: B(T(c, "content", u)),
                     marks: B(T(c, "marks", u)),
                     group: B(T(c, "group", u)),
                     inline: B(T(c, "inline", u)),
                     atom: B(T(c, "atom", u)),
                     selectable: B(T(c, "selectable", u)),
@@ -8545,15 +8563,15 @@
                         var R;
                         return [k.name, {
                             default: (R = k == null ? void 0 : k.attribute) === null || R === void 0 ? void 0 : R.default
                         }]
                     }))
                 }),
                 p = B(T(c, "parseHTML", u));
-            p && (h.parseDOM = p.map(k => ol(k, d)));
+            p && (h.parseDOM = p.map(k => ll(k, d)));
             let m = T(c, "renderHTML", u);
             m && (h.toDOM = k => m({
                 node: k,
                 HTMLAttributes: hi(k, d)
             }));
             let g = T(c, "renderText", u);
             return g && (h.toText = g), [c.name, h]
@@ -8569,51 +8587,51 @@
                 f = n.reduce((g, k) => {
                     let R = T(k, "extendMarkSchema", u);
                     return {
                         ...g,
                         ...R ? R(c) : {}
                     }
                 }, {}),
-                h = ll({
+                h = al({
                     ...f,
                     inclusive: B(T(c, "inclusive", u)),
                     excludes: B(T(c, "excludes", u)),
                     group: B(T(c, "group", u)),
                     spanning: B(T(c, "spanning", u)),
                     code: B(T(c, "code", u)),
                     attrs: Object.fromEntries(d.map(g => {
                         var k;
                         return [g.name, {
                             default: (k = g == null ? void 0 : g.attribute) === null || k === void 0 ? void 0 : k.default
                         }]
                     }))
                 }),
                 p = B(T(c, "parseHTML", u));
-            p && (h.parseDOM = p.map(g => ol(g, d)));
+            p && (h.parseDOM = p.map(g => ll(g, d)));
             let m = T(c, "renderHTML", u);
             return m && (h.toDOM = g => m({
                 mark: g,
                 HTMLAttributes: hi(g, d)
             })), [c.name, h]
         }));
     return new an({
         topNode: o,
         nodes: l,
         marks: a
     })
 }
 
-function li(n, e) {
+function ai(n, e) {
     return e.nodes[n] || e.marks[n] || null
 }
 
-function al(n, e) {
+function cl(n, e) {
     return Array.isArray(e) ? e.some(t => (typeof t == "string" ? t : t.name) === n.name) : e
 }
-var Wd = (n, e = 500) => {
+var _d = (n, e = 500) => {
     let t = "",
         r = n.parentOffset;
     return n.parent.nodesBetween(Math.max(0, r - e), r, (i, s, o, l) => {
         var a, c;
         let d = ((c = (a = i.type.spec).toText) === null || c === void 0 ? void 0 : c.call(a, {
             node: i,
             pos: s,
@@ -8628,23 +8646,23 @@
     return Object.prototype.toString.call(n) === "[object RegExp]"
 }
 var At = class {
         constructor(e) {
             this.find = e.find, this.handler = e.handler
         }
     },
-    Kd = (n, e) => {
+    Gd = (n, e) => {
         if (bi(e)) return e.exec(n);
         let t = e(n);
         if (!t) return null;
         let r = [t.text];
         return r.index = t.index, r.input = n, r.data = t.data, t.replaceWith && (t.text.includes(t.replaceWith) || console.warn('[tiptap warn]: "inputRuleMatch.replaceWith" must be part of "inputRuleMatch.text".'), r.push(t.replaceWith)), r
     };
 
-function ai(n) {
+function Pn(n) {
     var e;
     let {
         editor: t,
         from: r,
         to: i,
         text: s,
         rules: o,
@@ -8652,98 +8670,113 @@
     } = n, {
         view: a
     } = t;
     if (a.composing) return !1;
     let c = a.state.doc.resolve(r);
     if (c.parent.type.spec.code || !((e = c.nodeBefore || c.nodeAfter) === null || e === void 0) && e.marks.find(f => f.type.spec.code)) return !1;
     let d = !1,
-        u = Wd(c) + s;
+        u = _d(c) + s;
     return o.forEach(f => {
         if (d) return;
-        let h = Kd(u, f.find);
+        let h = Gd(u, f.find);
         if (!h) return;
         let p = a.state.tr,
-            m = Fn({
+            m = zn({
                 state: a.state,
                 transaction: p
             }),
             g = {
                 from: r - (h[0].length - s.length),
                 to: i
             },
             {
                 commands: k,
                 chain: R,
-                can: H
+                can: $
             } = new Tt({
                 editor: t,
                 state: m
             });
         f.handler({
             state: m,
             range: g,
             match: h,
             commands: k,
             chain: R,
-            can: H
+            can: $
         }) === null || !p.steps.length || (p.setMeta(l, {
             transform: p,
             from: r,
             to: i,
             text: s
         }), a.dispatch(p), d = !0)
     }), d
 }
 
-function Ud(n) {
+function Yd(n) {
     let {
         editor: e,
         rules: t
     } = n, r = new W({
         state: {
             init() {
                 return null
             },
             apply(i, s) {
                 let o = i.getMeta(r);
-                return o || (i.selectionSet || i.docChanged ? null : s)
+                if (o) return o;
+                let l = i.getMeta("applyInputRules");
+                return !!l && setTimeout(() => {
+                    let {
+                        from: c,
+                        text: d
+                    } = l, u = c + d.length;
+                    Pn({
+                        editor: e,
+                        from: c,
+                        to: u,
+                        text: d,
+                        rules: t,
+                        plugin: r
+                    })
+                }), i.selectionSet || i.docChanged ? null : s
             }
         },
         props: {
             handleTextInput(i, s, o, l) {
-                return ai({
+                return Pn({
                     editor: e,
                     from: s,
                     to: o,
                     text: l,
                     rules: t,
                     plugin: r
                 })
             },
             handleDOMEvents: {
                 compositionend: i => (setTimeout(() => {
                     let {
                         $cursor: s
                     } = i.state.selection;
-                    s && ai({
+                    s && Pn({
                         editor: e,
                         from: s.pos,
                         to: s.pos,
                         text: "",
                         rules: t,
                         plugin: r
                     })
                 }), !1)
             },
             handleKeyDown(i, s) {
                 if (s.key !== "Enter") return !1;
                 let {
                     $cursor: o
                 } = i.state.selection;
-                return o ? ai({
+                return o ? Pn({
                     editor: e,
                     from: o.pos,
                     to: o.pos,
                     text: `
 `,
                     rules: t,
                     plugin: r
@@ -8751,32 +8784,32 @@
             }
         },
         isInputRules: !0
     });
     return r
 }
 
-function _d(n) {
+function Xd(n) {
     return typeof n == "number"
 }
 var pi = class {
         constructor(e) {
             this.find = e.find, this.handler = e.handler
         }
     },
-    Gd = (n, e, t) => {
+    Zd = (n, e, t) => {
         if (bi(e)) return [...n.matchAll(e)];
         let r = e(n, t);
         return r ? r.map(i => {
             let s = [i.text];
             return s.index = i.index, s.input = n, s.data = i.data, i.replaceWith && (i.text.includes(i.replaceWith) || console.warn('[tiptap warn]: "pasteRuleMatch.replaceWith" must be part of "pasteRuleMatch.text".'), s.push(i.replaceWith)), s
         }) : []
     };
 
-function Yd(n) {
+function Qd(n) {
     let {
         editor: e,
         state: t,
         from: r,
         to: i,
         rule: s,
         pasteEvent: o,
@@ -8790,105 +8823,142 @@
         state: t
     }), u = [];
     return t.doc.nodesBetween(r, i, (h, p) => {
         if (!h.isTextblock || h.type.spec.code) return;
         let m = Math.max(r, p),
             g = Math.min(i, p + h.content.size),
             k = h.textBetween(m - p, g - p, void 0, "\uFFFC");
-        Gd(k, s.find, o).forEach(H => {
-            if (H.index === void 0) return;
-            let b = m + H.index + 1,
-                A = b + H[0].length,
+        Zd(k, s.find, o).forEach($ => {
+            if ($.index === void 0) return;
+            let b = m + $.index + 1,
+                A = b + $[0].length,
                 v = {
                     from: t.tr.mapping.map(b),
                     to: t.tr.mapping.map(A)
                 },
                 y = s.handler({
                     state: t,
                     range: v,
-                    match: H,
+                    match: $,
                     commands: a,
                     chain: c,
                     can: d,
                     pasteEvent: o,
                     dropEvent: l
                 });
             u.push(y)
         })
     }), u.every(h => h !== null)
 }
+var eu = n => {
+    var e;
+    let t = new ClipboardEvent("paste", {
+        clipboardData: new DataTransfer
+    });
+    return (e = t.clipboardData) === null || e === void 0 || e.setData("text/html", n), t
+};
 
-function Xd(n) {
+function tu(n) {
     let {
         editor: e,
         rules: t
-    } = n, r = null, i = !1, s = !1, o = typeof ClipboardEvent < "u" ? new ClipboardEvent("paste") : null, l = typeof DragEvent < "u" ? new DragEvent("drop") : null;
-    return t.map(c => new W({
-        view(d) {
-            let u = f => {
-                var h;
-                r = !((h = d.dom.parentElement) === null || h === void 0) && h.contains(f.target) ? d.dom.parentElement : null
+    } = n, r = null, i = !1, s = !1, o = typeof ClipboardEvent < "u" ? new ClipboardEvent("paste") : null, l = typeof DragEvent < "u" ? new DragEvent("drop") : null, a = ({
+        state: d,
+        from: u,
+        to: f,
+        rule: h,
+        pasteEvt: p
+    }) => {
+        let m = d.tr,
+            g = zn({
+                state: d,
+                transaction: m
+            });
+        if (!(!Qd({
+                editor: e,
+                state: g,
+                from: Math.max(u - 1, 0),
+                to: f.b - 1,
+                rule: h,
+                pasteEvent: p,
+                dropEvent: l
+            }) || !m.steps.length)) return l = typeof DragEvent < "u" ? new DragEvent("drop") : null, o = typeof ClipboardEvent < "u" ? new ClipboardEvent("paste") : null, m
+    };
+    return t.map(d => new W({
+        view(u) {
+            let f = h => {
+                var p;
+                r = !((p = u.dom.parentElement) === null || p === void 0) && p.contains(h.target) ? u.dom.parentElement : null
             };
-            return window.addEventListener("dragstart", u), {
+            return window.addEventListener("dragstart", f), {
                 destroy() {
-                    window.removeEventListener("dragstart", u)
+                    window.removeEventListener("dragstart", f)
                 }
             }
         },
         props: {
             handleDOMEvents: {
-                drop: (d, u) => (s = r === d.dom.parentElement, l = u, !1),
-                paste: (d, u) => {
-                    var f;
-                    let h = (f = u.clipboardData) === null || f === void 0 ? void 0 : f.getData("text/html");
-                    return o = u, i = !!(h != null && h.includes("data-pm-slice")), !1
+                drop: (u, f) => (s = r === u.dom.parentElement, l = f, !1),
+                paste: (u, f) => {
+                    var h;
+                    let p = (h = f.clipboardData) === null || h === void 0 ? void 0 : h.getData("text/html");
+                    return o = f, i = !!(p != null && p.includes("data-pm-slice")), !1
                 }
             }
         },
-        appendTransaction: (d, u, f) => {
-            let h = d[0],
-                p = h.getMeta("uiEvent") === "paste" && !i,
-                m = h.getMeta("uiEvent") === "drop" && !s;
-            if (!p && !m) return;
-            let g = u.doc.content.findDiffStart(f.doc.content),
-                k = u.doc.content.findDiffEnd(f.doc.content);
-            if (!_d(g) || !k || g === k.b) return;
-            let R = f.tr,
-                H = Fn({
-                    state: f,
-                    transaction: R
-                });
-            if (!(!Yd({
-                    editor: e,
-                    state: H,
-                    from: Math.max(g - 1, 0),
-                    to: k.b - 1,
-                    rule: c,
-                    pasteEvent: o,
-                    dropEvent: l
-                }) || !R.steps.length)) return l = typeof DragEvent < "u" ? new DragEvent("drop") : null, o = typeof ClipboardEvent < "u" ? new ClipboardEvent("paste") : null, R
+        appendTransaction: (u, f, h) => {
+            let p = u[0],
+                m = p.getMeta("uiEvent") === "paste" && !i,
+                g = p.getMeta("uiEvent") === "drop" && !s,
+                k = p.getMeta("applyPasteRules"),
+                R = !!k;
+            if (!m && !g && !R) return;
+            if (R) {
+                let {
+                    from: A,
+                    text: v
+                } = k, y = A + v.length, M = eu(v);
+                return a({
+                    rule: d,
+                    state: h,
+                    from: A,
+                    to: {
+                        b: y
+                    },
+                    pasteEvt: M
+                })
+            }
+            let $ = f.doc.content.findDiffStart(h.doc.content),
+                b = f.doc.content.findDiffEnd(h.doc.content);
+            if (!(!Xd($) || !b || $ === b.b)) return a({
+                rule: d,
+                state: h,
+                from: $,
+                to: b,
+                pasteEvt: o
+            })
         }
     }))
 }
 
-function Zd(n) {
+function nu(n) {
     let e = n.filter((t, r) => n.indexOf(t) !== r);
     return [...new Set(e)]
 }
 var mi = class n {
     constructor(e, t) {
-        this.splittableMarks = [], this.editor = t, this.extensions = n.resolve(e), this.schema = qd(this.extensions, t), this.extensions.forEach(r => {
+        this.splittableMarks = [], this.editor = t, this.extensions = n.resolve(e), this.schema = Ud(this.extensions, t), this.extensions.forEach(r => {
             var i;
             this.editor.extensionStorage[r.name] = r.storage;
             let s = {
                 name: r.name,
                 options: r.options,
                 storage: r.storage,
                 editor: this.editor,
-                type: li(r.name, this.schema)
+                type: ai(r.name, this.schema)
             };
             r.type === "mark" && (!((i = B(T(r, "keepOnSplit", s))) !== null && i !== void 0) || i) && this.splittableMarks.push(r.name);
             let o = T(r, "onBeforeCreate", s);
             o && this.editor.on("beforeCreate", o);
             let l = T(r, "onCreate", s);
             l && this.editor.on("create", l);
             let a = T(r, "onUpdate", s);
@@ -8903,15 +8973,15 @@
             f && this.editor.on("blur", f);
             let h = T(r, "onDestroy", s);
             h && this.editor.on("destroy", h)
         })
     }
     static resolve(e) {
         let t = n.sort(n.flatten(e)),
-            r = Zd(t.map(i => i.name));
+            r = nu(t.map(i => i.name));
         return r.length && console.warn(`[tiptap warn]: Duplicate extension names found: [${r.map(i=>`'${i}'`).join(", ")}]. This can lead to issues.`), t
     }
     static flatten(e) {
         return e.map(t => {
             let r = {
                     name: t.name,
                     options: t.options,
@@ -8931,15 +9001,15 @@
     get commands() {
         return this.extensions.reduce((e, t) => {
             let r = {
                     name: t.name,
                     options: t.options,
                     storage: t.storage,
                     editor: this.editor,
-                    type: li(t.name, this.schema)
+                    type: ai(t.name, this.schema)
                 },
                 i = T(t, "addCommands", r);
             return i ? {
                 ...e,
                 ...i()
             } : e
         }, {})
@@ -8949,15 +9019,15 @@
             editor: e
         } = this, t = n.sort([...this.extensions].reverse()), r = [], i = [], s = t.map(o => {
             let l = {
                     name: o.name,
                     options: o.options,
                     storage: o.storage,
                     editor: e,
-                    type: li(o.name, this.schema)
+                    type: ai(o.name, this.schema)
                 },
                 a = [],
                 c = T(o, "addKeyboardShortcuts", l),
                 d = {};
             if (o.type === "mark" && o.config.exitable && (d.ArrowRight = () => q.handleExit({
                     editor: e,
                     mark: o
@@ -8966,44 +9036,44 @@
                     editor: e
                 })]));
                 d = {
                     ...d,
                     ...m
                 }
             }
-            let u = Jo(d);
+            let u = qo(d);
             a.push(u);
             let f = T(o, "addInputRules", l);
-            al(o, e.options.enableInputRules) && f && r.push(...f());
+            cl(o, e.options.enableInputRules) && f && r.push(...f());
             let h = T(o, "addPasteRules", l);
-            al(o, e.options.enablePasteRules) && h && i.push(...h());
+            cl(o, e.options.enablePasteRules) && h && i.push(...h());
             let p = T(o, "addProseMirrorPlugins", l);
             if (p) {
                 let m = p();
                 a.push(...m)
             }
             return a
         }).flat();
-        return [Ud({
+        return [Yd({
             editor: e,
             rules: r
-        }), ...Xd({
+        }), ...tu({
             editor: e,
             rules: i
         }), ...s]
     }
     get attributes() {
-        return hl(this.extensions)
+        return pl(this.extensions)
     }
     get nodeViews() {
         let {
             editor: e
         } = this, {
             nodeExtensions: t
-        } = zn(this.extensions);
+        } = $n(this.extensions);
         return Object.fromEntries(t.filter(r => !!T(r, "addNodeView")).map(r => {
             let i = this.attributes.filter(a => a.type === r.name),
                 s = {
                     name: r.name,
                     options: r.options,
                     storage: r.storage,
                     editor: e,
@@ -9023,28 +9093,28 @@
                 })
             };
             return [r.name, l]
         }))
     }
 };
 
-function Qd(n) {
+function ru(n) {
     return Object.prototype.toString.call(n).slice(8, -1)
 }
 
 function ci(n) {
-    return Qd(n) !== "Object" ? !1 : n.constructor === Object && Object.getPrototypeOf(n) === Object.prototype
+    return ru(n) !== "Object" ? !1 : n.constructor === Object && Object.getPrototypeOf(n) === Object.prototype
 }
 
-function $n(n, e) {
+function Hn(n, e) {
     let t = {
         ...n
     };
     return ci(n) && ci(e) && Object.keys(e).forEach(r => {
-        ci(e[r]) ? r in n ? t[r] = $n(n[r], e[r]) : Object.assign(t, {
+        ci(e[r]) ? r in n ? t[r] = Hn(n[r], e[r]) : Object.assign(t, {
             [r]: e[r]
         }) : Object.assign(t, {
             [r]: e[r]
         })
     }), t
 }
 var G = class n {
@@ -9063,15 +9133,15 @@
         })) || {}
     }
     static create(e = {}) {
         return new n(e)
     }
     configure(e = {}) {
         let t = this.extend();
-        return t.options = $n(this.options, e), t.storage = B(T(t, "addStorage", {
+        return t.options = Hn(this.options, e), t.storage = B(T(t, "addStorage", {
             name: t.name,
             options: t.options
         })), t
     }
     extend(e = {}) {
         let t = new n({
             ...this.config,
@@ -9082,15 +9152,15 @@
         })), t.storage = B(T(t, "addStorage", {
             name: t.name,
             options: t.options
         })), t
     }
 };
 
-function ml(n, e, t) {
+function gl(n, e, t) {
     let {
         from: r,
         to: i
     } = e, {
         blockSeparator: s = `
 
 `,
@@ -9106,19 +9176,24 @@
             index: f,
             range: e
         })), !1;
         c.isText ? (l += (h = c == null ? void 0 : c.text) === null || h === void 0 ? void 0 : h.slice(Math.max(r, d) - d, i - d), a = !1) : c.isBlock && !a && (l += s, a = !0)
     }), l
 }
 
-function gl(n) {
+function yl(n) {
     return Object.fromEntries(Object.entries(n.nodes).filter(([, e]) => e.spec.toText).map(([e, t]) => [e, t.spec.toText]))
 }
-var eu = G.create({
+var iu = G.create({
         name: "clipboardTextSerializer",
+        addOptions() {
+            return {
+                blockSeparator: void 0
+            }
+        },
         addProseMirrorPlugins() {
             return [new W({
                 key: new Y("clipboardTextSerializer"),
                 props: {
                     clipboardTextSerializer: () => {
                         let {
                             editor: n
@@ -9126,37 +9201,40 @@
                             state: e,
                             schema: t
                         } = n, {
                             doc: r,
                             selection: i
                         } = e, {
                             ranges: s
-                        } = i, o = Math.min(...s.map(d => d.$from.pos)), l = Math.max(...s.map(d => d.$to.pos)), a = gl(t);
-                        return ml(r, {
+                        } = i, o = Math.min(...s.map(d => d.$from.pos)), l = Math.max(...s.map(d => d.$to.pos)), a = yl(t);
+                        return gl(r, {
                             from: o,
                             to: l
                         }, {
+                            ...this.options.blockSeparator !== void 0 ? {
+                                blockSeparator: this.options.blockSeparator
+                            } : {},
                             textSerializers: a
                         })
                     }
                 }
             })]
         }
     }),
-    tu = () => ({
+    su = () => ({
         editor: n,
         view: e
     }) => (requestAnimationFrame(() => {
         var t;
         n.isDestroyed || (e.dom.blur(), (t = window == null ? void 0 : window.getSelection()) === null || t === void 0 || t.removeAllRanges())
     }), !0),
-    nu = (n = !1) => ({
+    ou = (n = !1) => ({
         commands: e
     }) => e.setContent("", n),
-    ru = () => ({
+    lu = () => ({
         state: n,
         tr: e,
         dispatch: t
     }) => {
         let {
             selection: r
         } = e, {
@@ -9179,31 +9257,31 @@
                         defaultType: m
                     } = u.parent.contentMatchAt(u.index());
                     e.setNodeMarkup(h.start, m)
                 }(p || p === 0) && e.lift(h, p)
             })
         }), !0
     },
-    iu = n => e => n(e),
-    su = () => ({
+    au = n => e => n(e),
+    cu = () => ({
         state: n,
         dispatch: e
-    }) => ti(n, e),
-    ou = (n, e) => ({
+    }) => ni(n, e),
+    du = (n, e) => ({
         editor: t,
         tr: r
     }) => {
         let {
             state: i
         } = t, s = i.doc.slice(n.from, n.to);
         r.deleteRange(n.from, n.to);
         let o = r.mapping.map(e);
         return r.insert(o, s.content), r.setSelection(new P(r.doc.resolve(o - 1))), !0
     },
-    lu = () => ({
+    uu = () => ({
         tr: n,
         dispatch: e
     }) => {
         let {
             selection: t
         } = n, r = t.$anchor.node();
         if (r.content.size > 0) return !1;
@@ -9214,15 +9292,15 @@
                     let l = i.before(s),
                         a = i.after(s);
                     n.delete(l, a).scrollIntoView()
                 }
                 return !0
             } return !1
     },
-    au = n => ({
+    fu = n => ({
         tr: e,
         state: t,
         dispatch: r
     }) => {
         let i = Z(n, t.schema),
             s = e.selection.$anchor;
         for (let o = s.depth; o > 0; o -= 1)
@@ -9231,77 +9309,77 @@
                     let a = s.before(o),
                         c = s.after(o);
                     e.delete(a, c).scrollIntoView()
                 }
                 return !0
             } return !1
     },
-    cu = n => ({
+    hu = n => ({
         tr: e,
         dispatch: t
     }) => {
         let {
             from: r,
             to: i
         } = n;
         return t && e.delete(r, i), !0
     },
-    du = () => ({
+    pu = () => ({
         state: n,
         dispatch: e
     }) => In(n, e),
-    uu = () => ({
+    mu = () => ({
         commands: n
     }) => n.keyboardShortcut("Enter"),
-    fu = () => ({
+    gu = () => ({
         state: n,
         dispatch: e
-    }) => ei(n, e);
+    }) => ti(n, e);
 
-function Rn(n, e, t = {
+function Ln(n, e, t = {
     strict: !0
 }) {
     let r = Object.keys(e);
     return r.length ? r.every(i => t.strict ? e[i] === n[i] : bi(e[i]) ? e[i].test(n[i]) : e[i] === n[i]) : !0
 }
 
 function gi(n, e, t = {}) {
-    return n.find(r => r.type === e && Rn(r.attrs, t))
+    return n.find(r => r.type === e && Ln(r.attrs, t))
 }
 
-function hu(n, e, t = {}) {
+function yu(n, e, t = {}) {
     return !!gi(n, e, t)
 }
 
 function ki(n, e, t = {}) {
     if (!n || !e) return;
     let r = n.parent.childAfter(n.parentOffset);
     if (n.parentOffset === r.offset && r.offset !== 0 && (r = n.parent.childBefore(n.parentOffset)), !r.node) return;
     let i = gi([...r.node.marks], e, t);
     if (!i) return;
     let s = r.index,
         o = n.start() + r.offset,
         l = s + 1,
         a = o + r.node.nodeSize;
     for (gi([...r.node.marks], e, t); s > 0 && i.isInSet(n.parent.child(s - 1).marks);) s -= 1, o -= n.parent.child(s).nodeSize;
-    for (; l < n.parent.childCount && hu([...n.parent.child(l).marks], e, t);) a += n.parent.child(l).nodeSize, l += 1;
+    for (; l < n.parent.childCount && yu([...n.parent.child(l).marks], e, t);) a += n.parent.child(l).nodeSize, l += 1;
     return {
         from: o,
         to: a
     }
 }
 
 function We(n, e) {
     if (typeof n == "string") {
         if (!e.marks[n]) throw Error(`There is no mark type named '${n}'. Maybe you forgot to add the extension?`);
         return e.marks[n]
     }
     return n
 }
-var pu = (n, e = {}) => ({
+var xu = (n, e = {}) => ({
         tr: t,
         state: r,
         dispatch: i
     }) => {
         let s = We(n, r.schema),
             {
                 doc: o,
@@ -9317,44 +9395,44 @@
             if (u && u.from <= c && u.to >= d) {
                 let f = P.create(o, u.from, u.to);
                 t.setSelection(f)
             }
         }
         return !0
     },
-    mu = n => e => {
+    bu = n => e => {
         let t = typeof n == "function" ? n(e) : n;
         for (let r = 0; r < t.length; r += 1)
             if (t[r](e)) return !0;
         return !1
     };
 
-function yl(n) {
+function xl(n) {
     return n instanceof P
 }
 
 function dt(n = 0, e = 0, t = 0) {
     return Math.min(Math.max(n, e), t)
 }
 
-function xl(n, e = null) {
+function bl(n, e = null) {
     if (!e) return null;
     let t = L.atStart(n),
         r = L.atEnd(n);
     if (e === "start" || e === !0) return t;
     if (e === "end") return r;
     let i = t.from,
         s = r.to;
     return e === "all" ? P.create(n, dt(0, i, s), dt(n.content.size, i, s)) : P.create(n, dt(e, i, s), dt(e, i, s))
 }
 
 function Si() {
     return ["iPad Simulator", "iPhone Simulator", "iPod Simulator", "iPad", "iPhone", "iPod"].includes(navigator.platform) || navigator.userAgent.includes("Mac") && "ontouchend" in document
 }
-var gu = (n = null, e = {}) => ({
+var ku = (n = null, e = {}) => ({
         editor: t,
         view: r,
         tr: i,
         dispatch: s
     }) => {
         e = {
             scrollIntoView: !0,
@@ -9362,86 +9440,88 @@
         };
         let o = () => {
             Si() && r.dom.focus(), requestAnimationFrame(() => {
                 t.isDestroyed || (r.focus(), e != null && e.scrollIntoView && t.commands.scrollIntoView())
             })
         };
         if (r.hasFocus() && n === null || n === !1) return !0;
-        if (s && n === null && !yl(t.state.selection)) return o(), !0;
-        let l = xl(i.doc, n) || t.state.selection,
+        if (s && n === null && !xl(t.state.selection)) return o(), !0;
+        let l = bl(i.doc, n) || t.state.selection,
             a = t.state.selection.eq(l);
         return s && (a || i.setSelection(l), a && i.storedMarks && i.setStoredMarks(i.storedMarks), o()), !0
     },
-    yu = (n, e) => t => n.every((r, i) => e(r, {
+    Su = (n, e) => t => n.every((r, i) => e(r, {
         ...t,
         index: i
     })),
-    xu = (n, e) => ({
+    Mu = (n, e) => ({
         tr: t,
         commands: r
     }) => r.insertContentAt({
         from: t.selection.from,
         to: t.selection.to
     }, n, e),
-    bl = n => {
+    kl = n => {
         let e = n.childNodes;
         for (let t = e.length - 1; t >= 0; t -= 1) {
             let r = e[t];
-            r.nodeType === 3 && r.nodeValue && /^(\n\s\s|\n)$/.test(r.nodeValue) ? n.removeChild(r) : r.nodeType === 1 && bl(r)
+            r.nodeType === 3 && r.nodeValue && /^(\n\s\s|\n)$/.test(r.nodeValue) ? n.removeChild(r) : r.nodeType === 1 && kl(r)
         }
         return n
     };
 
-function cl(n) {
+function dl(n) {
     let e = `<body>${n}</body>`,
         t = new window.DOMParser().parseFromString(e, "text/html").body;
-    return bl(t)
+    return kl(t)
 }
 
-function Ln(n, e, t) {
+function Bn(n, e, t) {
     if (t = {
             slice: !0,
             parseOptions: {},
             ...t
         }, typeof n == "object" && n !== null) try {
-        return Array.isArray(n) && n.length > 0 ? M.fromArray(n.map(r => e.nodeFromJSON(r))) : e.nodeFromJSON(n)
+        return Array.isArray(n) && n.length > 0 ? w.fromArray(n.map(r => e.nodeFromJSON(r))) : e.nodeFromJSON(n)
     } catch (r) {
-        return console.warn("[tiptap warn]: Invalid content.", "Passed value:", n, "Error:", r), Ln("", e, t)
+        return console.warn("[tiptap warn]: Invalid content.", "Passed value:", n, "Error:", r), Bn("", e, t)
     }
     if (typeof n == "string") {
         let r = Qe.fromSchema(e);
-        return t.slice ? r.parseSlice(cl(n), t.parseOptions).content : r.parse(cl(n), t.parseOptions)
+        return t.slice ? r.parseSlice(dl(n), t.parseOptions).content : r.parse(dl(n), t.parseOptions)
     }
-    return Ln("", e, t)
+    return Bn("", e, t)
 }
 
-function bu(n, e, t) {
+function wu(n, e, t) {
     let r = n.steps.length - 1;
     if (r < e) return;
     let i = n.steps[r];
     if (!(i instanceof ie || i instanceof U)) return;
     let s = n.mapping.maps[r],
         o = 0;
     s.forEach((l, a, c, d) => {
         o === 0 && (o = d)
     }), n.setSelection(L.near(n.doc.resolve(o), t))
 }
-var ku = n => n.toString().startsWith("<"),
-    Su = (n, e, t) => ({
+var Eu = n => n.toString().startsWith("<"),
+    Cu = (n, e, t) => ({
         tr: r,
         dispatch: i,
         editor: s
     }) => {
         if (i) {
             t = {
                 parseOptions: {},
                 updateSelection: !0,
+                applyInputRules: !1,
+                applyPasteRules: !1,
                 ...t
             };
-            let o = Ln(e, s.schema, {
+            let o = Bn(e, s.schema, {
                 parseOptions: {
                     preserveWhitespace: "full",
                     ...t.parseOptions
                 }
             });
             if (o.toString() === "<>") return !0;
             let {
@@ -9450,102 +9530,109 @@
             } = typeof n == "number" ? {
                 from: n,
                 to: n
             } : {
                 from: n.from,
                 to: n.to
             }, c = !0, d = !0;
-            if ((ku(o) ? o : [o]).forEach(f => {
-                    f.check(), c = c ? f.isText && f.marks.length === 0 : !1, d = d ? f.isBlock : !1
+            if ((Eu(o) ? o : [o]).forEach(h => {
+                    h.check(), c = c ? h.isText && h.marks.length === 0 : !1, d = d ? h.isBlock : !1
                 }), l === a && d) {
                 let {
-                    parent: f
+                    parent: h
                 } = r.doc.resolve(l);
-                f.isTextblock && !f.type.spec.code && !f.childCount && (l -= 1, a += 1)
+                h.isTextblock && !h.type.spec.code && !h.childCount && (l -= 1, a += 1)
             }
-            c ? Array.isArray(e) ? r.insertText(e.map(f => f.text || "").join(""), l, a) : typeof e == "object" && e && e.text ? r.insertText(e.text, l, a) : r.insertText(e, l, a) : r.replaceWith(l, a, o), t.updateSelection && bu(r, r.steps.length - 1, -1)
+            let f;
+            c ? (Array.isArray(e) ? f = e.map(h => h.text || "").join("") : typeof e == "object" && e && e.text ? f = e.text : f = e, r.insertText(f, l, a)) : (f = o, r.replaceWith(l, a, f)), t.updateSelection && wu(r, r.steps.length - 1, -1), t.applyInputRules && r.setMeta("applyInputRules", {
+                from: l,
+                text: f
+            }), t.applyPasteRules && r.setMeta("applyPasteRules", {
+                from: l,
+                text: f
+            })
         }
         return !0
     },
-    Mu = () => ({
+    Tu = () => ({
         state: n,
         dispatch: e
-    }) => Yo(n, e),
-    wu = () => ({
+    }) => Xo(n, e),
+    Au = () => ({
         state: n,
         dispatch: e
-    }) => Xo(n, e),
-    Eu = () => ({
+    }) => Zo(n, e),
+    vu = () => ({
         state: n,
         dispatch: e
-    }) => Kr(n, e),
-    Cu = () => ({
+    }) => Ur(n, e),
+    Ou = () => ({
         state: n,
         dispatch: e
-    }) => Gr(n, e),
-    Tu = () => ({
+    }) => Yr(n, e),
+    Nu = () => ({
         tr: n,
         state: e,
         dispatch: t
     }) => {
         try {
             let r = yt(e.doc, e.selection.$from.pos, -1);
             return r == null ? !1 : (n.join(r, 2), t && t(n), !0)
         } catch {
             return !1
         }
     },
-    Au = () => ({
+    Du = () => ({
         state: n,
         dispatch: e,
         tr: t
     }) => {
         try {
             let r = yt(n.doc, n.selection.$from.pos, 1);
             return r == null ? !1 : (t.join(r, 2), e && e(t), !0)
         } catch {
             return !1
         }
     },
-    vu = () => ({
+    Iu = () => ({
         state: n,
         dispatch: e
-    }) => Ko(n, e),
-    Ou = () => ({
+    }) => Uo(n, e),
+    Pu = () => ({
         state: n,
         dispatch: e
-    }) => Uo(n, e);
+    }) => _o(n, e);
 
-function Hn() {
+function Vn() {
     return typeof navigator < "u" ? /Mac/.test(navigator.platform) : !1
 }
 
-function Nu(n) {
+function Ru(n) {
     let e = n.split(/-(?!$)/),
         t = e[e.length - 1];
     t === "Space" && (t = " ");
     let r, i, s, o;
     for (let l = 0; l < e.length - 1; l += 1) {
         let a = e[l];
         if (/^(cmd|meta|m)$/i.test(a)) o = !0;
         else if (/^a(lt)?$/i.test(a)) r = !0;
         else if (/^(c|ctrl|control)$/i.test(a)) i = !0;
         else if (/^s(hift)?$/i.test(a)) s = !0;
-        else if (/^mod$/i.test(a)) Si() || Hn() ? o = !0 : i = !0;
+        else if (/^mod$/i.test(a)) Si() || Vn() ? o = !0 : i = !0;
         else throw new Error(`Unrecognized modifier name: ${a}`)
     }
     return r && (t = `Alt-${t}`), i && (t = `Ctrl-${t}`), o && (t = `Meta-${t}`), s && (t = `Shift-${t}`), t
 }
-var Du = n => ({
+var Lu = n => ({
     editor: e,
     view: t,
     tr: r,
     dispatch: i
 }) => {
-    let s = Nu(n).split(/-(?!$)/),
+    let s = Ru(n).split(/-(?!$)/),
         o = s.find(c => !["Alt", "Ctrl", "Meta", "Shift"].includes(c)),
         l = new KeyboardEvent("keydown", {
             key: o === "Space" ? " " : o,
             altKey: s.includes("Alt"),
             ctrlKey: s.includes("Ctrl"),
             metaKey: s.includes("Meta"),
             shiftKey: s.includes("Shift"),
@@ -9574,112 +9661,112 @@
         l.push({
             node: u,
             from: h,
             to: p
         })
     });
     let a = i - r,
-        c = l.filter(u => o ? o.name === u.node.type.name : !0).filter(u => Rn(u.node.attrs, t, {
+        c = l.filter(u => o ? o.name === u.node.type.name : !0).filter(u => Ln(u.node.attrs, t, {
             strict: !1
         }));
     return s ? !!c.length : c.reduce((u, f) => u + f.to - f.from, 0) >= a
 }
-var Iu = (n, e = {}) => ({
+var Bu = (n, e = {}) => ({
         state: t,
         dispatch: r
     }) => {
         let i = Z(n, t.schema);
-        return Zt(t, i, e) ? Zo(t, r) : !1
+        return Zt(t, i, e) ? Qo(t, r) : !1
     },
-    Pu = () => ({
+    Fu = () => ({
         state: n,
         dispatch: e
-    }) => ni(n, e),
-    Ru = n => ({
+    }) => ri(n, e),
+    zu = n => ({
         state: e,
         dispatch: t
     }) => {
         let r = Z(n, e.schema);
-        return il(r)(e, t)
+        return sl(r)(e, t)
     },
-    Lu = () => ({
+    $u = () => ({
         state: n,
         dispatch: e
-    }) => Zr(n, e);
+    }) => Qr(n, e);
 
-function Vn(n, e) {
+function jn(n, e) {
     return e.nodes[n] ? "node" : e.marks[n] ? "mark" : null
 }
 
-function dl(n, e) {
+function ul(n, e) {
     let t = typeof e == "string" ? [e] : e;
     return Object.keys(n).reduce((r, i) => (t.includes(i) || (r[i] = n[i]), r), {})
 }
-var Bu = (n, e) => ({
+var Hu = (n, e) => ({
         tr: t,
         state: r,
         dispatch: i
     }) => {
         let s = null,
             o = null,
-            l = Vn(typeof n == "string" ? n : n.name, r.schema);
+            l = jn(typeof n == "string" ? n : n.name, r.schema);
         return l ? (l === "node" && (s = Z(n, r.schema)), l === "mark" && (o = We(n, r.schema)), i && t.selection.ranges.forEach(a => {
             r.doc.nodesBetween(a.$from.pos, a.$to.pos, (c, d) => {
-                s && s === c.type && t.setNodeMarkup(d, void 0, dl(c.attrs, e)), o && c.marks.length && c.marks.forEach(u => {
-                    o === u.type && t.addMark(d, d + c.nodeSize, o.create(dl(u.attrs, e)))
+                s && s === c.type && t.setNodeMarkup(d, void 0, ul(c.attrs, e)), o && c.marks.length && c.marks.forEach(u => {
+                    o === u.type && t.addMark(d, d + c.nodeSize, o.create(ul(u.attrs, e)))
                 })
             })
         }), !0) : !1
     },
-    Fu = () => ({
+    Vu = () => ({
         tr: n,
         dispatch: e
     }) => (e && n.scrollIntoView(), !0),
-    zu = () => ({
+    ju = () => ({
         tr: n,
         commands: e
     }) => e.setTextSelection({
         from: 0,
         to: n.doc.content.size
     }),
-    $u = () => ({
+    Ju = () => ({
         state: n,
         dispatch: e
-    }) => Ur(n, e),
-    Hu = () => ({
+    }) => _r(n, e),
+    qu = () => ({
         state: n,
         dispatch: e
-    }) => Yr(n, e),
-    Vu = () => ({
+    }) => Xr(n, e),
+    Wu = () => ({
         state: n,
         dispatch: e
-    }) => Qo(n, e),
-    ju = () => ({
+    }) => el(n, e),
+    Ku = () => ({
         state: n,
         dispatch: e
-    }) => ii(n, e),
-    Ju = () => ({
+    }) => si(n, e),
+    Uu = () => ({
         state: n,
         dispatch: e
-    }) => ri(n, e);
+    }) => ii(n, e);
 
-function kl(n, e, t = {}) {
-    return Ln(n, e, {
+function Sl(n, e, t = {}) {
+    return Bn(n, e, {
         slice: !1,
         parseOptions: t
     })
 }
-var qu = (n, e = !1, t = {}) => ({
+var _u = (n, e = !1, t = {}) => ({
     tr: r,
     editor: i,
     dispatch: s
 }) => {
     let {
         doc: o
-    } = r, l = kl(n, i.schema, t);
+    } = r, l = Sl(n, i.schema, t);
     return s && r.replaceWith(0, o.content.size, l).setMeta("preventUpdate", !e), !0
 };
 
 function vt(n, e) {
     let t = We(e, n.schema),
         {
             from: r,
@@ -9692,55 +9779,55 @@
     });
     let l = o.find(a => a.type.name === t.name);
     return l ? {
         ...l.attrs
     } : {}
 }
 
-function Wu(n) {
+function Gu(n) {
     for (let e = 0; e < n.edgeCount; e += 1) {
         let {
             type: t
         } = n.edge(e);
         if (t.isTextblock && !t.hasRequiredAttrs()) return t
     }
     return null
 }
 
-function Ku(n, e) {
+function Yu(n, e) {
     for (let t = n.depth; t > 0; t -= 1) {
         let r = n.node(t);
         if (e(r)) return {
             pos: t > 0 ? n.before(t) : 0,
             start: n.start(t),
             depth: t,
             node: r
         }
     }
 }
 
 function Mi(n) {
-    return e => Ku(e.$from, n)
+    return e => Yu(e.$from, n)
 }
 
-function Uu(n, e) {
+function Xu(n, e) {
     let t = Oe.fromSchema(e).serializeFragment(n),
         i = document.implementation.createHTMLDocument().createElement("div");
     return i.appendChild(t), i.innerHTML
 }
 
-function _u(n, e) {
+function Zu(n, e) {
     let t = {
         from: 0,
         to: n.content.size
     };
-    return ml(n, t, e)
+    return gl(n, t, e)
 }
 
-function Gu(n, e) {
+function Qu(n, e) {
     let t = Z(e, n.schema),
         {
             from: r,
             to: i
         } = n.selection,
         s = [];
     n.doc.nodesBetween(r, i, l => {
@@ -9749,19 +9836,19 @@
     let o = s.reverse().find(l => l.type.name === t.name);
     return o ? {
         ...o.attrs
     } : {}
 }
 
 function wi(n, e) {
-    let t = Vn(typeof e == "string" ? e : e.name, n.schema);
-    return t === "node" ? Gu(n, e) : t === "mark" ? vt(n, e) : {}
+    let t = jn(typeof e == "string" ? e : e.name, n.schema);
+    return t === "node" ? Qu(n, e) : t === "mark" ? vt(n, e) : {}
 }
 
-function Sl(n, e, t) {
+function Ml(n, e, t) {
     let r = [];
     return n === e ? t.resolve(n).marks().forEach(i => {
         let s = t.resolve(n - 1),
             o = ki(s, i.type);
         o && r.push({
             mark: i,
             ...o
@@ -9771,89 +9858,89 @@
             from: s,
             to: s + i.nodeSize,
             mark: o
         })))
     }), r
 }
 
-function Pn(n, e, t) {
+function Rn(n, e, t) {
     return Object.fromEntries(Object.entries(t).filter(([r]) => {
         let i = n.find(s => s.type === e && s.name === r);
         return i ? i.attribute.keepOnSplit : !1
     }))
 }
 
 function yi(n, e, t = {}) {
     let {
         empty: r,
         ranges: i
     } = n.selection, s = e ? We(e, n.schema) : null;
-    if (r) return !!(n.storedMarks || n.selection.$from.marks()).filter(u => s ? s.name === u.type.name : !0).find(u => Rn(u.attrs, t, {
+    if (r) return !!(n.storedMarks || n.selection.$from.marks()).filter(u => s ? s.name === u.type.name : !0).find(u => Ln(u.attrs, t, {
         strict: !1
     }));
     let o = 0,
         l = [];
     if (i.forEach(({
             $from: u,
             $to: f
         }) => {
             let h = u.pos,
                 p = f.pos;
             n.doc.nodesBetween(h, p, (m, g) => {
                 if (!m.isText && !m.marks.length) return;
                 let k = Math.max(h, g),
                     R = Math.min(p, g + m.nodeSize),
-                    H = R - k;
-                o += H, l.push(...m.marks.map(b => ({
+                    $ = R - k;
+                o += $, l.push(...m.marks.map(b => ({
                     mark: b,
                     from: k,
                     to: R
                 })))
             })
         }), o === 0) return !1;
-    let a = l.filter(u => s ? s.name === u.mark.type.name : !0).filter(u => Rn(u.mark.attrs, t, {
+    let a = l.filter(u => s ? s.name === u.mark.type.name : !0).filter(u => Ln(u.mark.attrs, t, {
             strict: !1
         })).reduce((u, f) => u + f.to - f.from, 0),
         c = l.filter(u => s ? u.mark.type !== s && u.mark.type.excludes(s) : !0).reduce((u, f) => u + f.to - f.from, 0);
     return (a > 0 ? a + c : a) >= o
 }
 
-function Yu(n, e, t = {}) {
+function ef(n, e, t = {}) {
     if (!e) return Zt(n, null, t) || yi(n, null, t);
-    let r = Vn(e, n.schema);
+    let r = jn(e, n.schema);
     return r === "node" ? Zt(n, e, t) : r === "mark" ? yi(n, e, t) : !1
 }
 
-function ul(n, e) {
+function fl(n, e) {
     let {
         nodeExtensions: t
-    } = zn(e), r = t.find(o => o.name === n);
+    } = $n(e), r = t.find(o => o.name === n);
     if (!r) return !1;
     let i = {
             name: r.name,
             options: r.options,
             storage: r.storage
         },
         s = B(T(r, "group", i));
     return typeof s != "string" ? !1 : s.split(" ").includes("list")
 }
 
-function Xu(n) {
+function tf(n) {
     var e;
     let t = (e = n.type.createAndFill()) === null || e === void 0 ? void 0 : e.toJSON(),
         r = n.toJSON();
     return JSON.stringify(t) === JSON.stringify(r)
 }
 
-function Zu(n, e, t) {
+function nf(n, e, t) {
     var r;
     let {
         selection: i
     } = e, s = null;
-    if (yl(i) && (s = i.$cursor), s) {
+    if (xl(i) && (s = i.$cursor), s) {
         let l = (r = n.storedMarks) !== null && r !== void 0 ? r : s.marks();
         return !!t.isInSet(l) || !l.some(a => a.type.excludes(t))
     }
     let {
         ranges: o
     } = i;
     return o.some(({
@@ -9868,15 +9955,15 @@
                     p = !!t.isInSet(d.marks) || !d.marks.some(m => m.type.excludes(t));
                 c = h && p
             }
             return !c
         }), c
     })
 }
-var Qu = (n, e = {}) => ({
+var rf = (n, e = {}) => ({
         tr: t,
         state: r,
         dispatch: i
     }) => {
         let {
             selection: s
         } = t, {
@@ -9900,44 +9987,44 @@
                         a === k.type && t.addMark(p, m, a.create({
                             ...k.attrs,
                             ...e
                         }))
                     }) : t.addMark(p, m, a.create(e))
                 })
             });
-        return Zu(r, t, a)
+        return nf(r, t, a)
     },
-    ef = (n, e) => ({
+    sf = (n, e) => ({
         tr: t
     }) => (t.setMeta(n, e), !0),
-    tf = (n, e = {}) => ({
+    of = (n, e = {}) => ({
         state: t,
         dispatch: r,
         chain: i
     }) => {
         let s = Z(n, t.schema);
         return s.isTextblock ? i().command(({
             commands: o
-        }) => si(s, e)(t) ? !0 : o.clearNodes()).command(({
+        }) => oi(s, e)(t) ? !0 : o.clearNodes()).command(({
             state: o
-        }) => si(s, e)(o, r)).run() : (console.warn('[tiptap warn]: Currently "setNode()" only supports text block nodes.'), !1)
+        }) => oi(s, e)(o, r)).run() : (console.warn('[tiptap warn]: Currently "setNode()" only supports text block nodes.'), !1)
     },
-    nf = n => ({
+    lf = n => ({
         tr: e,
         dispatch: t
     }) => {
         if (t) {
             let {
                 doc: r
             } = e, i = dt(n, 0, r.content.size), s = O.create(r, i);
             e.setSelection(s)
         }
         return !0
     },
-    rf = n => ({
+    af = n => ({
         tr: e,
         dispatch: t
     }) => {
         if (t) {
             let {
                 doc: r
             } = e, {
@@ -9947,634 +10034,647 @@
                 from: n,
                 to: n
             } : n, o = P.atStart(r).from, l = P.atEnd(r).to, a = dt(i, o, l), c = dt(s, o, l), d = P.create(r, a, c);
             e.setSelection(d)
         }
         return !0
     },
-    sf = n => ({
+    cf = n => ({
         state: e,
         dispatch: t
     }) => {
         let r = Z(n, e.schema);
-        return sl(r)(e, t)
+        return ol(r)(e, t)
     };
 
-function fl(n, e) {
+function hl(n, e) {
     let t = n.storedMarks || n.selection.$to.parentOffset && n.selection.$from.marks();
     if (t) {
         let r = t.filter(i => e == null ? void 0 : e.includes(i.type.name));
         n.tr.ensureMarks(r)
     }
 }
-var of = ({
-    keepMarks: n = !0
-} = {}) => ({
-    tr: e,
-    state: t,
-    dispatch: r,
-    editor: i
-}) => {
-    let {
-        selection: s,
-        doc: o
-    } = e, {
-        $from: l,
-        $to: a
-    } = s, c = i.extensionManager.attributes, d = Pn(c, l.node().type.name, l.node().attrs);
-    if (s instanceof O && s.node.isBlock) return !l.parentOffset || !pe(o, l.pos) ? !1 : (r && (n && fl(t, i.extensionManager.splittableMarks), e.split(l.pos).scrollIntoView()), !0);
-    if (!l.parent.isBlock) return !1;
-    if (r) {
-        let u = a.parentOffset === a.parent.content.size;
-        s instanceof P && e.deleteSelection();
-        let f = l.depth === 0 ? void 0 : Wu(l.node(-1).contentMatchAt(l.indexAfter(-1))),
-            h = u && f ? [{
-                type: f,
-                attrs: d
-            }] : void 0,
-            p = pe(e.doc, e.mapping.map(l.pos), 1, h);
-        if (!h && !p && pe(e.doc, e.mapping.map(l.pos), 1, f ? [{
-                type: f
-            }] : void 0) && (p = !0, h = f ? [{
-                type: f,
-                attrs: d
-            }] : void 0), p && (e.split(e.mapping.map(l.pos), 1, h), f && !u && !l.parentOffset && l.parent.type !== f)) {
-            let m = e.mapping.map(l.before()),
-                g = e.doc.resolve(m);
-            l.node(-1).canReplaceWith(g.index(), g.index() + 1, f) && e.setNodeMarkup(e.mapping.map(l.before()), f)
-        }
-        n && fl(t, i.extensionManager.splittableMarks), e.scrollIntoView()
-    }
-    return !0
-}, lf = n => ({
-    tr: e,
-    state: t,
-    dispatch: r,
-    editor: i
-}) => {
-    var s;
-    let o = Z(n, t.schema),
-        {
+var df = ({
+        keepMarks: n = !0
+    } = {}) => ({
+        tr: e,
+        state: t,
+        dispatch: r,
+        editor: i
+    }) => {
+        let {
+            selection: s,
+            doc: o
+        } = e, {
             $from: l,
             $to: a
-        } = t.selection,
-        c = t.selection.node;
-    if (c && c.isBlock || l.depth < 2 || !l.sameParent(a)) return !1;
-    let d = l.node(-1);
-    if (d.type !== o) return !1;
-    let u = i.extensionManager.attributes;
-    if (l.parent.content.size === 0 && l.node(-1).childCount === l.indexAfter(-1)) {
-        if (l.depth === 2 || l.node(-3).type !== o || l.index(-2) !== l.node(-2).childCount - 1) return !1;
+        } = s, c = i.extensionManager.attributes, d = Rn(c, l.node().type.name, l.node().attrs);
+        if (s instanceof O && s.node.isBlock) return !l.parentOffset || !pe(o, l.pos) ? !1 : (r && (n && hl(t, i.extensionManager.splittableMarks), e.split(l.pos).scrollIntoView()), !0);
+        if (!l.parent.isBlock) return !1;
         if (r) {
-            let g = M.empty,
-                k = l.index(-1) ? 1 : l.index(-2) ? 2 : 3;
-            for (let y = l.depth - k; y >= l.depth - 3; y -= 1) g = M.from(l.node(y).copy(g));
-            let R = l.indexAfter(-1) < l.node(-2).childCount ? 1 : l.indexAfter(-2) < l.node(-3).childCount ? 2 : 3,
-                H = Pn(u, l.node().type.name, l.node().attrs),
-                b = ((s = o.contentMatch.defaultType) === null || s === void 0 ? void 0 : s.createAndFill(H)) || void 0;
-            g = g.append(M.from(o.createAndFill(null, b) || void 0));
-            let A = l.before(l.depth - (k - 1));
-            e.replace(A, l.after(-R), new E(g, 4 - k, 0));
-            let v = -1;
-            e.doc.nodesBetween(A, e.doc.content.size, (y, w) => {
-                if (v > -1) return !1;
-                y.isTextblock && y.content.size === 0 && (v = w + 1)
-            }), v > -1 && e.setSelection(P.near(e.doc.resolve(v))), e.scrollIntoView()
+            let u = a.parentOffset === a.parent.content.size;
+            s instanceof P && e.deleteSelection();
+            let f = l.depth === 0 ? void 0 : Gu(l.node(-1).contentMatchAt(l.indexAfter(-1))),
+                h = u && f ? [{
+                    type: f,
+                    attrs: d
+                }] : void 0,
+                p = pe(e.doc, e.mapping.map(l.pos), 1, h);
+            if (!h && !p && pe(e.doc, e.mapping.map(l.pos), 1, f ? [{
+                    type: f
+                }] : void 0) && (p = !0, h = f ? [{
+                    type: f,
+                    attrs: d
+                }] : void 0), p && (e.split(e.mapping.map(l.pos), 1, h), f && !u && !l.parentOffset && l.parent.type !== f)) {
+                let m = e.mapping.map(l.before()),
+                    g = e.doc.resolve(m);
+                l.node(-1).canReplaceWith(g.index(), g.index() + 1, f) && e.setNodeMarkup(e.mapping.map(l.before()), f)
+            }
+            n && hl(t, i.extensionManager.splittableMarks), e.scrollIntoView()
         }
         return !0
-    }
-    let f = a.pos === l.end() ? d.contentMatchAt(0).defaultType : null,
-        h = Pn(u, d.type.name, d.attrs),
-        p = Pn(u, l.node().type.name, l.node().attrs);
-    e.delete(l.pos, a.pos);
-    let m = f ? [{
-        type: o,
-        attrs: h
-    }, {
-        type: f,
-        attrs: p
-    }] : [{
-        type: o,
-        attrs: h
-    }];
-    if (!pe(e.doc, l.pos, 2)) return !1;
-    if (r) {
-        let {
-            selection: g,
-            storedMarks: k
-        } = t, {
-            splittableMarks: R
-        } = i.extensionManager, H = k || g.$to.parentOffset && g.$from.marks();
-        if (e.split(l.pos, 2, m).scrollIntoView(), !H || !r) return !0;
-        let b = H.filter(A => R.includes(A.type.name));
-        e.ensureMarks(b)
-    }
-    return !0
-}, di = (n, e) => {
-    let t = Mi(o => o.type === e)(n.selection);
-    if (!t) return !0;
-    let r = n.doc.resolve(Math.max(0, t.pos - 1)).before(t.depth);
-    if (r === void 0) return !0;
-    let i = n.doc.nodeAt(r);
-    return t.node.type === (i == null ? void 0 : i.type) && xe(n.doc, t.pos) && n.join(t.pos), !0
-}, ui = (n, e) => {
-    let t = Mi(o => o.type === e)(n.selection);
-    if (!t) return !0;
-    let r = n.doc.resolve(t.start).after(t.depth);
-    if (r === void 0) return !0;
-    let i = n.doc.nodeAt(r);
-    return t.node.type === (i == null ? void 0 : i.type) && xe(n.doc, r) && n.join(r), !0
-}, af = (n, e, t, r = {}) => ({
-    editor: i,
-    tr: s,
-    state: o,
-    dispatch: l,
-    chain: a,
-    commands: c,
-    can: d
-}) => {
-    let {
-        extensions: u,
-        splittableMarks: f
-    } = i.extensionManager, h = Z(n, o.schema), p = Z(e, o.schema), {
-        selection: m,
-        storedMarks: g
-    } = o, {
-        $from: k,
-        $to: R
-    } = m, H = k.blockRange(R), b = g || m.$to.parentOffset && m.$from.marks();
-    if (!H) return !1;
-    let A = Mi(v => ul(v.type.name, u))(m);
-    if (H.depth >= 1 && A && H.depth - A.depth <= 1) {
-        if (A.node.type === h) return c.liftListItem(p);
-        if (ul(A.node.type.name, u) && h.validContent(A.node.content) && l) return a().command(() => (s.setNodeMarkup(A.pos, h), !0)).command(() => di(s, h)).command(() => ui(s, h)).run()
-    }
-    return !t || !b || !l ? a().command(() => d().wrapInList(h, r) ? !0 : c.clearNodes()).wrapInList(h, r).command(() => di(s, h)).command(() => ui(s, h)).run() : a().command(() => {
-        let v = d().wrapInList(h, r),
-            y = b.filter(w => f.includes(w.type.name));
-        return s.ensureMarks(y), v ? !0 : c.clearNodes()
-    }).wrapInList(h, r).command(() => di(s, h)).command(() => ui(s, h)).run()
-}, cf = (n, e = {}, t = {}) => ({
-    state: r,
-    commands: i
-}) => {
-    let {
-        extendEmptyMarkRange: s = !1
-    } = t, o = We(n, r.schema);
-    return yi(r, o, e) ? i.unsetMark(o, {
-        extendEmptyMarkRange: s
-    }) : i.setMark(o, e)
-}, df = (n, e, t = {}) => ({
-    state: r,
-    commands: i
-}) => {
-    let s = Z(n, r.schema),
-        o = Z(e, r.schema);
-    return Zt(r, s, t) ? i.setNode(o) : i.setNode(s, t)
-}, uf = (n, e = {}) => ({
-    state: t,
-    commands: r
-}) => {
-    let i = Z(n, t.schema);
-    return Zt(t, i, e) ? r.lift(i) : r.wrapIn(i, e)
-}, ff = () => ({
-    state: n,
-    dispatch: e
-}) => {
-    let t = n.plugins;
-    for (let r = 0; r < t.length; r += 1) {
-        let i = t[r],
-            s;
-        if (i.spec.isInputRules && (s = i.getState(n))) {
-            if (e) {
-                let o = n.tr,
-                    l = s.transform;
-                for (let a = l.steps.length - 1; a >= 0; a -= 1) o.step(l.steps[a].invert(l.docs[a]));
-                if (s.text) {
-                    let a = o.doc.resolve(s.from).marks();
-                    o.replaceWith(s.from, s.to, n.schema.text(s.text, a))
-                } else o.delete(s.from, s.to)
+    },
+    uf = n => ({
+        tr: e,
+        state: t,
+        dispatch: r,
+        editor: i
+    }) => {
+        var s;
+        let o = Z(n, t.schema),
+            {
+                $from: l,
+                $to: a
+            } = t.selection,
+            c = t.selection.node;
+        if (c && c.isBlock || l.depth < 2 || !l.sameParent(a)) return !1;
+        let d = l.node(-1);
+        if (d.type !== o) return !1;
+        let u = i.extensionManager.attributes;
+        if (l.parent.content.size === 0 && l.node(-1).childCount === l.indexAfter(-1)) {
+            if (l.depth === 2 || l.node(-3).type !== o || l.index(-2) !== l.node(-2).childCount - 1) return !1;
+            if (r) {
+                let g = w.empty,
+                    k = l.index(-1) ? 1 : l.index(-2) ? 2 : 3;
+                for (let y = l.depth - k; y >= l.depth - 3; y -= 1) g = w.from(l.node(y).copy(g));
+                let R = l.indexAfter(-1) < l.node(-2).childCount ? 1 : l.indexAfter(-2) < l.node(-3).childCount ? 2 : 3,
+                    $ = Rn(u, l.node().type.name, l.node().attrs),
+                    b = ((s = o.contentMatch.defaultType) === null || s === void 0 ? void 0 : s.createAndFill($)) || void 0;
+                g = g.append(w.from(o.createAndFill(null, b) || void 0));
+                let A = l.before(l.depth - (k - 1));
+                e.replace(A, l.after(-R), new E(g, 4 - k, 0));
+                let v = -1;
+                e.doc.nodesBetween(A, e.doc.content.size, (y, M) => {
+                    if (v > -1) return !1;
+                    y.isTextblock && y.content.size === 0 && (v = M + 1)
+                }), v > -1 && e.setSelection(P.near(e.doc.resolve(v))), e.scrollIntoView()
             }
             return !0
         }
-    }
-    return !1
-}, hf = () => ({
-    tr: n,
-    dispatch: e
-}) => {
-    let {
-        selection: t
-    } = n, {
-        empty: r,
-        ranges: i
-    } = t;
-    return r || e && i.forEach(s => {
-        n.removeMark(s.$from.pos, s.$to.pos)
-    }), !0
-}, pf = (n, e = {}) => ({
-    tr: t,
-    state: r,
-    dispatch: i
-}) => {
-    var s;
-    let {
-        extendEmptyMarkRange: o = !1
-    } = e, {
-        selection: l
-    } = t, a = We(n, r.schema), {
-        $from: c,
-        empty: d,
-        ranges: u
-    } = l;
-    if (!i) return !0;
-    if (d && o) {
+        let f = a.pos === l.end() ? d.contentMatchAt(0).defaultType : null,
+            h = Rn(u, d.type.name, d.attrs),
+            p = Rn(u, l.node().type.name, l.node().attrs);
+        e.delete(l.pos, a.pos);
+        let m = f ? [{
+            type: o,
+            attrs: h
+        }, {
+            type: f,
+            attrs: p
+        }] : [{
+            type: o,
+            attrs: h
+        }];
+        if (!pe(e.doc, l.pos, 2)) return !1;
+        if (r) {
+            let {
+                selection: g,
+                storedMarks: k
+            } = t, {
+                splittableMarks: R
+            } = i.extensionManager, $ = k || g.$to.parentOffset && g.$from.marks();
+            if (e.split(l.pos, 2, m).scrollIntoView(), !$ || !r) return !0;
+            let b = $.filter(A => R.includes(A.type.name));
+            e.ensureMarks(b)
+        }
+        return !0
+    },
+    di = (n, e) => {
+        let t = Mi(o => o.type === e)(n.selection);
+        if (!t) return !0;
+        let r = n.doc.resolve(Math.max(0, t.pos - 1)).before(t.depth);
+        if (r === void 0) return !0;
+        let i = n.doc.nodeAt(r);
+        return t.node.type === (i == null ? void 0 : i.type) && xe(n.doc, t.pos) && n.join(t.pos), !0
+    },
+    ui = (n, e) => {
+        let t = Mi(o => o.type === e)(n.selection);
+        if (!t) return !0;
+        let r = n.doc.resolve(t.start).after(t.depth);
+        if (r === void 0) return !0;
+        let i = n.doc.nodeAt(r);
+        return t.node.type === (i == null ? void 0 : i.type) && xe(n.doc, r) && n.join(r), !0
+    },
+    ff = (n, e, t, r = {}) => ({
+        editor: i,
+        tr: s,
+        state: o,
+        dispatch: l,
+        chain: a,
+        commands: c,
+        can: d
+    }) => {
         let {
-            from: f,
-            to: h
-        } = l, p = (s = c.marks().find(g => g.type === a)) === null || s === void 0 ? void 0 : s.attrs, m = ki(c, a, p);
-        m && (f = m.from, h = m.to), t.removeMark(f, h, a)
-    } else u.forEach(f => {
-        t.removeMark(f.$from.pos, f.$to.pos, a)
-    });
-    return t.removeStoredMark(a), !0
-}, mf = (n, e = {}) => ({
-    tr: t,
-    state: r,
-    dispatch: i
-}) => {
-    let s = null,
-        o = null,
-        l = Vn(typeof n == "string" ? n : n.name, r.schema);
-    return l ? (l === "node" && (s = Z(n, r.schema)), l === "mark" && (o = We(n, r.schema)), i && t.selection.ranges.forEach(a => {
-        let c = a.$from.pos,
-            d = a.$to.pos;
-        r.doc.nodesBetween(c, d, (u, f) => {
-            s && s === u.type && t.setNodeMarkup(f, void 0, {
-                ...u.attrs,
-                ...e
-            }), o && u.marks.length && u.marks.forEach(h => {
-                if (o === h.type) {
-                    let p = Math.max(f, c),
-                        m = Math.min(f + u.nodeSize, d);
-                    t.addMark(p, m, o.create({
-                        ...h.attrs,
-                        ...e
-                    }))
+            extensions: u,
+            splittableMarks: f
+        } = i.extensionManager, h = Z(n, o.schema), p = Z(e, o.schema), {
+            selection: m,
+            storedMarks: g
+        } = o, {
+            $from: k,
+            $to: R
+        } = m, $ = k.blockRange(R), b = g || m.$to.parentOffset && m.$from.marks();
+        if (!$) return !1;
+        let A = Mi(v => fl(v.type.name, u))(m);
+        if ($.depth >= 1 && A && $.depth - A.depth <= 1) {
+            if (A.node.type === h) return c.liftListItem(p);
+            if (fl(A.node.type.name, u) && h.validContent(A.node.content) && l) return a().command(() => (s.setNodeMarkup(A.pos, h), !0)).command(() => di(s, h)).command(() => ui(s, h)).run()
+        }
+        return !t || !b || !l ? a().command(() => d().wrapInList(h, r) ? !0 : c.clearNodes()).wrapInList(h, r).command(() => di(s, h)).command(() => ui(s, h)).run() : a().command(() => {
+            let v = d().wrapInList(h, r),
+                y = b.filter(M => f.includes(M.type.name));
+            return s.ensureMarks(y), v ? !0 : c.clearNodes()
+        }).wrapInList(h, r).command(() => di(s, h)).command(() => ui(s, h)).run()
+    },
+    hf = (n, e = {}, t = {}) => ({
+        state: r,
+        commands: i
+    }) => {
+        let {
+            extendEmptyMarkRange: s = !1
+        } = t, o = We(n, r.schema);
+        return yi(r, o, e) ? i.unsetMark(o, {
+            extendEmptyMarkRange: s
+        }) : i.setMark(o, e)
+    },
+    pf = (n, e, t = {}) => ({
+        state: r,
+        commands: i
+    }) => {
+        let s = Z(n, r.schema),
+            o = Z(e, r.schema);
+        return Zt(r, s, t) ? i.setNode(o) : i.setNode(s, t)
+    },
+    mf = (n, e = {}) => ({
+        state: t,
+        commands: r
+    }) => {
+        let i = Z(n, t.schema);
+        return Zt(t, i, e) ? r.lift(i) : r.wrapIn(i, e)
+    },
+    gf = () => ({
+        state: n,
+        dispatch: e
+    }) => {
+        let t = n.plugins;
+        for (let r = 0; r < t.length; r += 1) {
+            let i = t[r],
+                s;
+            if (i.spec.isInputRules && (s = i.getState(n))) {
+                if (e) {
+                    let o = n.tr,
+                        l = s.transform;
+                    for (let a = l.steps.length - 1; a >= 0; a -= 1) o.step(l.steps[a].invert(l.docs[a]));
+                    if (s.text) {
+                        let a = o.doc.resolve(s.from).marks();
+                        o.replaceWith(s.from, s.to, n.schema.text(s.text, a))
+                    } else o.delete(s.from, s.to)
                 }
-            })
-        })
-    }), !0) : !1
-}, gf = (n, e = {}) => ({
-    state: t,
-    dispatch: r
-}) => {
-    let i = Z(n, t.schema);
-    return nl(i, e)(t, r)
-}, yf = (n, e = {}) => ({
-    state: t,
-    dispatch: r
-}) => {
-    let i = Z(n, t.schema);
-    return rl(i, e)(t, r)
-}, xf = Object.freeze({
-    __proto__: null,
-    blur: tu,
-    clearContent: nu,
-    clearNodes: ru,
-    command: iu,
-    createParagraphNear: su,
-    cut: ou,
-    deleteCurrentNode: lu,
-    deleteNode: au,
-    deleteRange: cu,
-    deleteSelection: du,
-    enter: uu,
-    exitCode: fu,
-    extendMarkRange: pu,
-    first: mu,
-    focus: gu,
-    forEach: yu,
-    insertContent: xu,
-    insertContentAt: Su,
-    joinUp: Mu,
-    joinDown: wu,
-    joinBackward: Eu,
-    joinForward: Cu,
-    joinItemBackward: Tu,
-    joinItemForward: Au,
-    joinTextblockBackward: vu,
-    joinTextblockForward: Ou,
-    keyboardShortcut: Du,
-    lift: Iu,
-    liftEmptyBlock: Pu,
-    liftListItem: Ru,
-    newlineInCode: Lu,
-    resetAttributes: Bu,
-    scrollIntoView: Fu,
-    selectAll: zu,
-    selectNodeBackward: $u,
-    selectNodeForward: Hu,
-    selectParentNode: Vu,
-    selectTextblockEnd: ju,
-    selectTextblockStart: Ju,
-    setContent: qu,
-    setMark: Qu,
-    setMeta: ef,
-    setNode: tf,
-    setNodeSelection: nf,
-    setTextSelection: rf,
-    sinkListItem: sf,
-    splitBlock: of,
-    splitListItem: lf,
-    toggleList: af,
-    toggleMark: cf,
-    toggleNode: df,
-    toggleWrap: uf,
-    undoInputRule: ff,
-    unsetAllMarks: hf,
-    unsetMark: pf,
-    updateAttributes: mf,
-    wrapIn: gf,
-    wrapInList: yf
-}), bf = G.create({
-    name: "commands",
-    addCommands() {
-        return {
-            ...xf
-        }
-    }
-}), kf = G.create({
-    name: "editable",
-    addProseMirrorPlugins() {
-        return [new W({
-            key: new Y("editable"),
-            props: {
-                editable: () => this.editor.options.editable
+                return !0
             }
-        })]
-    }
-}), Sf = G.create({
-    name: "focusEvents",
-    addProseMirrorPlugins() {
+        }
+        return !1
+    },
+    yf = () => ({
+        tr: n,
+        dispatch: e
+    }) => {
         let {
-            editor: n
-        } = this;
-        return [new W({
-            key: new Y("focusEvents"),
-            props: {
-                handleDOMEvents: {
-                    focus: (e, t) => {
-                        n.isFocused = !0;
-                        let r = n.state.tr.setMeta("focus", {
-                            event: t
-                        }).setMeta("addToHistory", !1);
-                        return e.dispatch(r), !1
-                    },
-                    blur: (e, t) => {
-                        n.isFocused = !1;
-                        let r = n.state.tr.setMeta("blur", {
-                            event: t
-                        }).setMeta("addToHistory", !1);
-                        return e.dispatch(r), !1
+            selection: t
+        } = n, {
+            empty: r,
+            ranges: i
+        } = t;
+        return r || e && i.forEach(s => {
+            n.removeMark(s.$from.pos, s.$to.pos)
+        }), !0
+    },
+    xf = (n, e = {}) => ({
+        tr: t,
+        state: r,
+        dispatch: i
+    }) => {
+        var s;
+        let {
+            extendEmptyMarkRange: o = !1
+        } = e, {
+            selection: l
+        } = t, a = We(n, r.schema), {
+            $from: c,
+            empty: d,
+            ranges: u
+        } = l;
+        if (!i) return !0;
+        if (d && o) {
+            let {
+                from: f,
+                to: h
+            } = l, p = (s = c.marks().find(g => g.type === a)) === null || s === void 0 ? void 0 : s.attrs, m = ki(c, a, p);
+            m && (f = m.from, h = m.to), t.removeMark(f, h, a)
+        } else u.forEach(f => {
+            t.removeMark(f.$from.pos, f.$to.pos, a)
+        });
+        return t.removeStoredMark(a), !0
+    },
+    bf = (n, e = {}) => ({
+        tr: t,
+        state: r,
+        dispatch: i
+    }) => {
+        let s = null,
+            o = null,
+            l = jn(typeof n == "string" ? n : n.name, r.schema);
+        return l ? (l === "node" && (s = Z(n, r.schema)), l === "mark" && (o = We(n, r.schema)), i && t.selection.ranges.forEach(a => {
+            let c = a.$from.pos,
+                d = a.$to.pos;
+            r.doc.nodesBetween(c, d, (u, f) => {
+                s && s === u.type && t.setNodeMarkup(f, void 0, {
+                    ...u.attrs,
+                    ...e
+                }), o && u.marks.length && u.marks.forEach(h => {
+                    if (o === h.type) {
+                        let p = Math.max(f, c),
+                            m = Math.min(f + u.nodeSize, d);
+                        t.addMark(p, m, o.create({
+                            ...h.attrs,
+                            ...e
+                        }))
                     }
-                }
-            }
-        })]
-    }
-}), Mf = G.create({
-    name: "keymap",
-    addKeyboardShortcuts() {
-        let n = () => this.editor.commands.first(({
-                commands: o
-            }) => [() => o.undoInputRule(), () => o.command(({
-                tr: l
-            }) => {
-                let {
-                    selection: a,
-                    doc: c
-                } = l, {
-                    empty: d,
-                    $anchor: u
-                } = a, {
-                    pos: f,
-                    parent: h
-                } = u, p = u.parent.isTextblock && f > 0 ? l.doc.resolve(f - 1) : u, m = p.parent.type.spec.isolating, g = u.pos - u.parentOffset, k = m && p.parent.childCount === 1 ? g === u.pos : L.atStart(c).from === f;
-                return !d || !k || !h.type.isTextblock || h.textContent.length ? !1 : o.clearNodes()
-            }), () => o.deleteSelection(), () => o.joinBackward(), () => o.selectNodeBackward()]),
-            e = () => this.editor.commands.first(({
-                commands: o
-            }) => [() => o.deleteSelection(), () => o.deleteCurrentNode(), () => o.joinForward(), () => o.selectNodeForward()]),
-            r = {
-                Enter: () => this.editor.commands.first(({
-                    commands: o
-                }) => [() => o.newlineInCode(), () => o.createParagraphNear(), () => o.liftEmptyBlock(), () => o.splitBlock()]),
-                "Mod-Enter": () => this.editor.commands.exitCode(),
-                Backspace: n,
-                "Mod-Backspace": n,
-                "Shift-Backspace": n,
-                Delete: e,
-                "Mod-Delete": e,
-                "Mod-a": () => this.editor.commands.selectAll()
-            },
-            i = {
-                ...r
-            },
-            s = {
-                ...r,
-                "Ctrl-h": n,
-                "Alt-Backspace": n,
-                "Ctrl-d": e,
-                "Ctrl-Alt-Backspace": e,
-                "Alt-Delete": e,
-                "Alt-d": e,
-                "Ctrl-a": () => this.editor.commands.selectTextblockStart(),
-                "Ctrl-e": () => this.editor.commands.selectTextblockEnd()
-            };
-        return Si() || Hn() ? s : i
+                })
+            })
+        }), !0) : !1
     },
-    addProseMirrorPlugins() {
-        return [new W({
-            key: new Y("clearDocument"),
-            appendTransaction: (n, e, t) => {
-                if (!(n.some(p => p.docChanged) && !e.doc.eq(t.doc))) return;
-                let {
-                    empty: i,
-                    from: s,
-                    to: o
-                } = e.selection, l = L.atStart(e.doc).from, a = L.atEnd(e.doc).to;
-                if (i || !(s === l && o === a) || !(t.doc.textBetween(0, t.doc.content.size, " ", " ").length === 0)) return;
-                let u = t.tr,
-                    f = Fn({
-                        state: t,
-                        transaction: u
-                    }),
-                    {
-                        commands: h
-                    } = new Tt({
-                        editor: this.editor,
-                        state: f
-                    });
-                if (h.clearNodes(), !!u.steps.length) return u
+    kf = (n, e = {}) => ({
+        state: t,
+        dispatch: r
+    }) => {
+        let i = Z(n, t.schema);
+        return rl(i, e)(t, r)
+    },
+    Sf = (n, e = {}) => ({
+        state: t,
+        dispatch: r
+    }) => {
+        let i = Z(n, t.schema);
+        return il(i, e)(t, r)
+    },
+    Mf = Object.freeze({
+        __proto__: null,
+        blur: su,
+        clearContent: ou,
+        clearNodes: lu,
+        command: au,
+        createParagraphNear: cu,
+        cut: du,
+        deleteCurrentNode: uu,
+        deleteNode: fu,
+        deleteRange: hu,
+        deleteSelection: pu,
+        enter: mu,
+        exitCode: gu,
+        extendMarkRange: xu,
+        first: bu,
+        focus: ku,
+        forEach: Su,
+        insertContent: Mu,
+        insertContentAt: Cu,
+        joinUp: Tu,
+        joinDown: Au,
+        joinBackward: vu,
+        joinForward: Ou,
+        joinItemBackward: Nu,
+        joinItemForward: Du,
+        joinTextblockBackward: Iu,
+        joinTextblockForward: Pu,
+        keyboardShortcut: Lu,
+        lift: Bu,
+        liftEmptyBlock: Fu,
+        liftListItem: zu,
+        newlineInCode: $u,
+        resetAttributes: Hu,
+        scrollIntoView: Vu,
+        selectAll: ju,
+        selectNodeBackward: Ju,
+        selectNodeForward: qu,
+        selectParentNode: Wu,
+        selectTextblockEnd: Ku,
+        selectTextblockStart: Uu,
+        setContent: _u,
+        setMark: rf,
+        setMeta: sf,
+        setNode: of,
+        setNodeSelection: lf,
+        setTextSelection: af,
+        sinkListItem: cf,
+        splitBlock: df,
+        splitListItem: uf,
+        toggleList: ff,
+        toggleMark: hf,
+        toggleNode: pf,
+        toggleWrap: mf,
+        undoInputRule: gf,
+        unsetAllMarks: yf,
+        unsetMark: xf,
+        updateAttributes: bf,
+        wrapIn: kf,
+        wrapInList: Sf
+    }),
+    wf = G.create({
+        name: "commands",
+        addCommands() {
+            return {
+                ...Mf
             }
-        })]
-    }
-}), wf = G.create({
-    name: "tabindex",
-    addProseMirrorPlugins() {
-        return [new W({
-            key: new Y("tabindex"),
-            props: {
-                attributes: this.editor.isEditable ? {
-                    tabindex: "0"
-                } : {}
+        }
+    }),
+    Ef = G.create({
+        name: "editable",
+        addProseMirrorPlugins() {
+            return [new W({
+                key: new Y("editable"),
+                props: {
+                    editable: () => this.editor.options.editable
+                }
+            })]
+        }
+    }),
+    Cf = G.create({
+        name: "focusEvents",
+        addProseMirrorPlugins() {
+            let {
+                editor: n
+            } = this;
+            return [new W({
+                key: new Y("focusEvents"),
+                props: {
+                    handleDOMEvents: {
+                        focus: (e, t) => {
+                            n.isFocused = !0;
+                            let r = n.state.tr.setMeta("focus", {
+                                event: t
+                            }).setMeta("addToHistory", !1);
+                            return e.dispatch(r), !1
+                        },
+                        blur: (e, t) => {
+                            n.isFocused = !1;
+                            let r = n.state.tr.setMeta("blur", {
+                                event: t
+                            }).setMeta("addToHistory", !1);
+                            return e.dispatch(r), !1
+                        }
+                    }
+                }
+            })]
+        }
+    }),
+    Tf = G.create({
+        name: "keymap",
+        addKeyboardShortcuts() {
+            let n = () => this.editor.commands.first(({
+                    commands: o
+                }) => [() => o.undoInputRule(), () => o.command(({
+                    tr: l
+                }) => {
+                    let {
+                        selection: a,
+                        doc: c
+                    } = l, {
+                        empty: d,
+                        $anchor: u
+                    } = a, {
+                        pos: f,
+                        parent: h
+                    } = u, p = u.parent.isTextblock && f > 0 ? l.doc.resolve(f - 1) : u, m = p.parent.type.spec.isolating, g = u.pos - u.parentOffset, k = m && p.parent.childCount === 1 ? g === u.pos : L.atStart(c).from === f;
+                    return !d || !k || !h.type.isTextblock || h.textContent.length ? !1 : o.clearNodes()
+                }), () => o.deleteSelection(), () => o.joinBackward(), () => o.selectNodeBackward()]),
+                e = () => this.editor.commands.first(({
+                    commands: o
+                }) => [() => o.deleteSelection(), () => o.deleteCurrentNode(), () => o.joinForward(), () => o.selectNodeForward()]),
+                r = {
+                    Enter: () => this.editor.commands.first(({
+                        commands: o
+                    }) => [() => o.newlineInCode(), () => o.createParagraphNear(), () => o.liftEmptyBlock(), () => o.splitBlock()]),
+                    "Mod-Enter": () => this.editor.commands.exitCode(),
+                    Backspace: n,
+                    "Mod-Backspace": n,
+                    "Shift-Backspace": n,
+                    Delete: e,
+                    "Mod-Delete": e,
+                    "Mod-a": () => this.editor.commands.selectAll()
+                },
+                i = {
+                    ...r
+                },
+                s = {
+                    ...r,
+                    "Ctrl-h": n,
+                    "Alt-Backspace": n,
+                    "Ctrl-d": e,
+                    "Ctrl-Alt-Backspace": e,
+                    "Alt-Delete": e,
+                    "Alt-d": e,
+                    "Ctrl-a": () => this.editor.commands.selectTextblockStart(),
+                    "Ctrl-e": () => this.editor.commands.selectTextblockEnd()
+                };
+            return Si() || Vn() ? s : i
+        },
+        addProseMirrorPlugins() {
+            return [new W({
+                key: new Y("clearDocument"),
+                appendTransaction: (n, e, t) => {
+                    if (!(n.some(p => p.docChanged) && !e.doc.eq(t.doc))) return;
+                    let {
+                        empty: i,
+                        from: s,
+                        to: o
+                    } = e.selection, l = L.atStart(e.doc).from, a = L.atEnd(e.doc).to;
+                    if (i || !(s === l && o === a) || !(t.doc.textBetween(0, t.doc.content.size, " ", " ").length === 0)) return;
+                    let u = t.tr,
+                        f = zn({
+                            state: t,
+                            transaction: u
+                        }),
+                        {
+                            commands: h
+                        } = new Tt({
+                            editor: this.editor,
+                            state: f
+                        });
+                    if (h.clearNodes(), !!u.steps.length) return u
+                }
+            })]
+        }
+    }),
+    Af = G.create({
+        name: "tabindex",
+        addProseMirrorPlugins() {
+            return [new W({
+                key: new Y("tabindex"),
+                props: {
+                    attributes: this.editor.isEditable ? {
+                        tabindex: "0"
+                    } : {}
+                }
+            })]
+        }
+    });
+var xi = class n {
+        constructor(e, t, r = !1, i = null) {
+            this.currentNode = null, this.actualDepth = null, this.isBlock = r, this.resolvedPos = e, this.editor = t, this.currentNode = i
+        }
+        get name() {
+            return this.node.type.name
+        }
+        get node() {
+            return this.currentNode || this.resolvedPos.node()
+        }
+        get element() {
+            return this.editor.view.domAtPos(this.pos).node
+        }
+        get depth() {
+            var e;
+            return (e = this.actualDepth) !== null && e !== void 0 ? e : this.resolvedPos.depth
+        }
+        get pos() {
+            return this.resolvedPos.pos
+        }
+        get content() {
+            return this.node.content
+        }
+        set content(e) {
+            let t = this.from,
+                r = this.to;
+            if (this.isBlock) {
+                if (this.content.size === 0) {
+                    console.error(`You can\u2019t set content on a block node. Tried to set content on ${this.name} at ${this.pos}`);
+                    return
+                }
+                t = this.from + 1, r = this.to - 1
             }
-        })]
-    }
-}), Ef = Object.freeze({
-    __proto__: null,
-    ClipboardTextSerializer: eu,
-    Commands: bf,
-    Editable: kf,
-    FocusEvents: Sf,
-    Keymap: Mf,
-    Tabindex: wf
-}), xi = class n {
-    constructor(e, t, r = !1, i = null) {
-        this.currentNode = null, this.actualDepth = null, this.isBlock = r, this.resolvedPos = e, this.editor = t, this.currentNode = i
-    }
-    get name() {
-        return this.node.type.name
-    }
-    get node() {
-        return this.currentNode || this.resolvedPos.node()
-    }
-    get element() {
-        return this.editor.view.domAtPos(this.pos).node
-    }
-    get depth() {
-        var e;
-        return (e = this.actualDepth) !== null && e !== void 0 ? e : this.resolvedPos.depth
-    }
-    get pos() {
-        return this.resolvedPos.pos
-    }
-    get content() {
-        return this.node.content
-    }
-    set content(e) {
-        let t = this.from,
-            r = this.to;
-        if (this.isBlock) {
-            if (this.content.size === 0) {
-                console.error(`You can\u2019t set content on a block node. Tried to set content on ${this.name} at ${this.pos}`);
-                return
+            this.editor.commands.insertContentAt({
+                from: t,
+                to: r
+            }, e)
+        }
+        get attributes() {
+            return this.node.attrs
+        }
+        get textContent() {
+            return this.node.textContent
+        }
+        get size() {
+            return this.node.nodeSize
+        }
+        get from() {
+            return this.isBlock ? this.pos : this.resolvedPos.start(this.resolvedPos.depth)
+        }
+        get range() {
+            return {
+                from: this.from,
+                to: this.to
             }
-            t = this.from + 1, r = this.to - 1
         }
-        this.editor.commands.insertContentAt({
-            from: t,
-            to: r
-        }, e)
-    }
-    get attributes() {
-        return this.node.attrs
-    }
-    get textContent() {
-        return this.node.textContent
-    }
-    get size() {
-        return this.node.nodeSize
-    }
-    get from() {
-        return this.isBlock ? this.pos : this.resolvedPos.start(this.resolvedPos.depth)
-    }
-    get range() {
-        return {
-            from: this.from,
-            to: this.to
+        get to() {
+            return this.isBlock ? this.pos + this.size : this.resolvedPos.end(this.resolvedPos.depth) + (this.node.isText ? 0 : 1)
         }
-    }
-    get to() {
-        return this.isBlock ? this.pos + this.size : this.resolvedPos.end(this.resolvedPos.depth) + (this.node.isText ? 0 : 1)
-    }
-    get parent() {
-        if (this.depth === 0) return null;
-        let e = this.resolvedPos.start(this.resolvedPos.depth - 1),
-            t = this.resolvedPos.doc.resolve(e);
-        return new n(t, this.editor)
-    }
-    get before() {
-        let e = this.resolvedPos.doc.resolve(this.from - (this.isBlock ? 1 : 2));
-        return e.depth !== this.depth && (e = this.resolvedPos.doc.resolve(this.from - 3)), new n(e, this.editor)
-    }
-    get after() {
-        let e = this.resolvedPos.doc.resolve(this.to + (this.isBlock ? 2 : 1));
-        return e.depth !== this.depth && (e = this.resolvedPos.doc.resolve(this.to + 3)), new n(e, this.editor)
-    }
-    get children() {
-        let e = [];
-        return this.node.content.forEach((t, r) => {
-            let i = t.isBlock && !t.isTextblock,
-                s = this.pos + r + (i ? 0 : 1),
-                o = this.resolvedPos.doc.resolve(s);
-            if (!i && o.depth <= this.depth) return;
-            let l = new n(o, this.editor, i, i ? t : null);
-            i && (l.actualDepth = this.depth + 1), e.push(new n(o, this.editor, i, i ? t : null))
-        }), e
-    }
-    get firstChild() {
-        return this.children[0] || null
-    }
-    get lastChild() {
-        let e = this.children;
-        return e[e.length - 1] || null
-    }
-    closest(e, t = {}) {
-        let r = null,
-            i = this.parent;
-        for (; i && !r;) {
-            if (i.node.type.name === e)
-                if (Object.keys(t).length > 0) {
-                    let s = i.node.attrs,
-                        o = Object.keys(t);
-                    for (let l = 0; l < o.length; l += 1) {
-                        let a = o[l];
-                        if (s[a] !== t[a]) break
-                    }
-                } else r = i;
-            i = i.parent
+        get parent() {
+            if (this.depth === 0) return null;
+            let e = this.resolvedPos.start(this.resolvedPos.depth - 1),
+                t = this.resolvedPos.doc.resolve(e);
+            return new n(t, this.editor)
+        }
+        get before() {
+            let e = this.resolvedPos.doc.resolve(this.from - (this.isBlock ? 1 : 2));
+            return e.depth !== this.depth && (e = this.resolvedPos.doc.resolve(this.from - 3)), new n(e, this.editor)
+        }
+        get after() {
+            let e = this.resolvedPos.doc.resolve(this.to + (this.isBlock ? 2 : 1));
+            return e.depth !== this.depth && (e = this.resolvedPos.doc.resolve(this.to + 3)), new n(e, this.editor)
+        }
+        get children() {
+            let e = [];
+            return this.node.content.forEach((t, r) => {
+                let i = t.isBlock && !t.isTextblock,
+                    s = this.pos + r + 1,
+                    o = this.resolvedPos.doc.resolve(s);
+                if (!i && o.depth <= this.depth) return;
+                let l = new n(o, this.editor, i, i ? t : null);
+                i && (l.actualDepth = this.depth + 1), e.push(new n(o, this.editor, i, i ? t : null))
+            }), e
         }
-        return r
-    }
-    querySelector(e, t = {}) {
-        return this.querySelectorAll(e, t, !0)[0] || null
-    }
-    querySelectorAll(e, t = {}, r = !1) {
-        let i = [];
-        return this.isBlock || !this.children || this.children.length === 0 || this.children.forEach(s => {
-            if (s.node.type.name === e) {
-                if (Object.keys(t).length > 0) {
-                    let o = s.node.attrs,
-                        l = Object.keys(t);
-                    for (let a = 0; a < l.length; a += 1) {
-                        let c = l[a];
-                        if (o[c] !== t[c]) return
+        get firstChild() {
+            return this.children[0] || null
+        }
+        get lastChild() {
+            let e = this.children;
+            return e[e.length - 1] || null
+        }
+        closest(e, t = {}) {
+            let r = null,
+                i = this.parent;
+            for (; i && !r;) {
+                if (i.node.type.name === e)
+                    if (Object.keys(t).length > 0) {
+                        let s = i.node.attrs,
+                            o = Object.keys(t);
+                        for (let l = 0; l < o.length; l += 1) {
+                            let a = o[l];
+                            if (s[a] !== t[a]) break
+                        }
+                    } else r = i;
+                i = i.parent
+            }
+            return r
+        }
+        querySelector(e, t = {}) {
+            return this.querySelectorAll(e, t, !0)[0] || null
+        }
+        querySelectorAll(e, t = {}, r = !1) {
+            let i = [];
+            return !this.children || this.children.length === 0 || this.children.forEach(s => {
+                if (s.node.type.name === e) {
+                    if (Object.keys(t).length > 0) {
+                        let o = s.node.attrs,
+                            l = Object.keys(t);
+                        for (let a = 0; a < l.length; a += 1) {
+                            let c = l[a];
+                            if (o[c] !== t[c]) return
+                        }
                     }
+                    if (i.push(s), r) return
                 }
-                if (i.push(s), r) return
-            }
-            i = i.concat(s.querySelectorAll(e))
-        }), i
-    }
-    setAttribute(e) {
-        let t = this.editor.state.selection;
-        this.editor.chain().setTextSelection(this.from).updateAttributes(this.node.type.name, e).setTextSelection(t.from).run()
-    }
-}, Cf = `.ProseMirror {
+                i = i.concat(s.querySelectorAll(e))
+            }), i
+        }
+        setAttribute(e) {
+            let t = this.editor.state.selection;
+            this.editor.chain().setTextSelection(this.from).updateAttributes(this.node.type.name, e).setTextSelection(t.from).run()
+        }
+    },
+    vf = `.ProseMirror {
   position: relative;
 }
 
 .ProseMirror {
   word-wrap: break-word;
   white-space: pre-wrap;
   white-space: break-spaces;
@@ -10642,32 +10742,33 @@
   display: block;
 }
 
 .tippy-box[data-animation=fade][data-state=hidden] {
   opacity: 0
 }`;
 
-function Tf(n, e, t) {
+function Of(n, e, t) {
     let r = document.querySelector(`style[data-tiptap-style${t?`-${t}`:""}]`);
     if (r !== null) return r;
     let i = document.createElement("style");
     return e && i.setAttribute("nonce", e), i.setAttribute(`data-tiptap-style${t?`-${t}`:""}`, ""), i.innerHTML = n, document.getElementsByTagName("head")[0].appendChild(i), i
 }
-var Bn = class extends fi {
+var Fn = class extends fi {
     constructor(e = {}) {
         super(), this.isFocused = !1, this.extensionStorage = {}, this.options = {
             element: document.createElement("div"),
             content: "",
             injectCSS: !0,
             injectNonce: void 0,
             extensions: [],
             autofocus: !1,
             editable: !0,
             editorProps: {},
             parseOptions: {},
+            coreExtensionOptions: {},
             enableInputRules: !0,
             enablePasteRules: !0,
             enableCoreExtensions: !0,
             onBeforeCreate: () => null,
             onCreate: () => null,
             onUpdate: () => null,
             onSelectionUpdate: () => null,
@@ -10692,15 +10793,15 @@
     chain() {
         return this.commandManager.chain()
     }
     can() {
         return this.commandManager.can()
     }
     injectCSS() {
-        this.options.injectCSS && document && (this.css = Tf(Cf, this.options.injectNonce))
+        this.options.injectCSS && document && (this.css = Of(vf, this.options.injectNonce))
     }
     setOptions(e = {}) {
         this.options = {
             ...this.options,
             ...e
         }, !(!this.view || !this.state || this.isDestroyed) && (this.options.editorProps && this.view.setProps(this.options.editorProps), this.view.updateState(this.state))
     }
@@ -10715,43 +10816,46 @@
     get isEditable() {
         return this.options.editable && this.view && this.view.editable
     }
     get state() {
         return this.view.state
     }
     registerPlugin(e, t) {
-        let r = pl(t) ? t(e, [...this.state.plugins]) : [...this.state.plugins, e],
+        let r = ml(t) ? t(e, [...this.state.plugins]) : [...this.state.plugins, e],
             i = this.state.reconfigure({
                 plugins: r
             });
         this.view.updateState(i)
     }
     unregisterPlugin(e) {
         if (this.isDestroyed) return;
         let t = typeof e == "string" ? `${e}$` : e.key,
             r = this.state.reconfigure({
                 plugins: this.state.plugins.filter(i => !i.key.startsWith(t))
             });
         this.view.updateState(r)
     }
     createExtensionManager() {
-        let t = [...this.options.enableCoreExtensions ? Object.values(Ef) : [], ...this.options.extensions].filter(r => ["extension", "node", "mark"].includes(r == null ? void 0 : r.type));
-        this.extensionManager = new mi(t, this)
+        var e, t;
+        let i = [...this.options.enableCoreExtensions ? [Ef, iu.configure({
+            blockSeparator: (t = (e = this.options.coreExtensionOptions) === null || e === void 0 ? void 0 : e.clipboardTextSerializer) === null || t === void 0 ? void 0 : t.blockSeparator
+        }), wf, Cf, Tf, Af] : [], ...this.options.extensions].filter(s => ["extension", "node", "mark"].includes(s == null ? void 0 : s.type));
+        this.extensionManager = new mi(i, this)
     }
     createCommandManager() {
         this.commandManager = new Tt({
             editor: this
         })
     }
     createSchema() {
         this.schema = this.extensionManager.schema
     }
     createView() {
-        let e = kl(this.options.content, this.schema, this.options.parseOptions),
-            t = xl(e, this.options.autofocus);
+        let e = Sl(this.options.content, this.schema, this.options.parseOptions),
+            t = bl(e, this.options.autofocus);
         this.view = new An(this.options.element, {
             ...this.options.editorProps,
             dispatchTransaction: this.dispatchTransaction.bind(this),
             state: yn.create({
                 doc: e,
                 selection: t || void 0
             })
@@ -10815,39 +10919,39 @@
     }
     getAttributes(e) {
         return wi(this.state, e)
     }
     isActive(e, t) {
         let r = typeof e == "string" ? e : null,
             i = typeof e == "string" ? t : e;
-        return Yu(this.state, r, i)
+        return ef(this.state, r, i)
     }
     getJSON() {
         return this.state.doc.toJSON()
     }
     getHTML() {
-        return Uu(this.state.doc.content, this.schema)
+        return Xu(this.state.doc.content, this.schema)
     }
     getText(e) {
         let {
             blockSeparator: t = `
 
 `,
             textSerializers: r = {}
         } = e || {};
-        return _u(this.state.doc, {
+        return Zu(this.state.doc, {
             blockSeparator: t,
             textSerializers: {
-                ...gl(this.schema),
+                ...yl(this.schema),
                 ...r
             }
         })
     }
     get isEmpty() {
-        return Xu(this.state.doc)
+        return tf(this.state.doc)
     }
     getCharacterCount() {
         return console.warn('[tiptap warn]: "editor.getCharacterCount()" is deprecated. Please use "editor.storage.characterCount.characters()" instead.'), this.state.doc.content.size - 2
     }
     destroy() {
         this.emit("destroy"), this.view && this.view.destroy(), this.removeAllListeners()
     }
@@ -10885,24 +10989,24 @@
             let {
                 tr: s
             } = e, o = r[r.length - 1], l = r[0];
             if (o) {
                 let a = l.search(/\S/),
                     c = t.from + l.indexOf(o),
                     d = c + o.length;
-                if (Sl(t.from, t.to, e.doc).filter(h => h.mark.type.excluded.find(m => m === n.type && m !== h.mark.type)).filter(h => h.to > c).length) return null;
+                if (Ml(t.from, t.to, e.doc).filter(h => h.mark.type.excluded.find(m => m === n.type && m !== h.mark.type)).filter(h => h.to > c).length) return null;
                 d < t.to && s.delete(d, t.to), c > t.from && s.delete(t.from + a, c);
                 let f = t.from + a + o.length;
                 s.addMark(t.from + a, f, n.type.create(i || {})), s.removeStoredMark(n.type)
             }
         }
     })
 }
 
-function Ml(n) {
+function wl(n) {
     return new At({
         find: n.find,
         handler: ({
             state: e,
             range: t,
             match: r
         }) => {
@@ -10992,15 +11096,15 @@
             })) || {}
         }
         static create(e = {}) {
             return new n(e)
         }
         configure(e = {}) {
             let t = this.extend();
-            return t.options = $n(this.options, e), t.storage = B(T(t, "addStorage", {
+            return t.options = Hn(this.options, e), t.storage = B(T(t, "addStorage", {
                 name: t.name,
                 options: t.options
             })), t
         }
         extend(e = {}) {
             let t = new n({
                 ...this.config,
@@ -11045,15 +11149,15 @@
             })) || {}
         }
         static create(e = {}) {
             return new n(e)
         }
         configure(e = {}) {
             let t = this.extend();
-            return t.options = $n(this.options, e), t.storage = B(T(t, "addStorage", {
+            return t.options = Hn(this.options, e), t.storage = B(T(t, "addStorage", {
                 name: t.name,
                 options: t.options
             })), t
         }
         extend(e = {}) {
             let t = new n({
                 ...this.config,
@@ -11082,22 +11186,22 @@
             let {
                 tr: o
             } = e, l = r[r.length - 1], a = r[0], c = t.to;
             if (l) {
                 let d = a.search(/\S/),
                     u = t.from + a.indexOf(l),
                     f = u + l.length;
-                if (Sl(t.from, t.to, e.doc).filter(p => p.mark.type.excluded.find(g => g === n.type && g !== p.mark.type)).filter(p => p.to > u).length) return null;
+                if (Ml(t.from, t.to, e.doc).filter(p => p.mark.type.excluded.find(g => g === n.type && g !== p.mark.type)).filter(p => p.to > u).length) return null;
                 f < t.to && o.delete(f, t.to), u > t.from && o.delete(t.from + d, u), c = t.from + d + l.length, o.addMark(t.from + d, c, n.type.create(s || {})), o.removeStoredMark(n.type)
             }
         }
     })
 }
-var Af = /^\s*>\s$/,
-    wl = J.create({
+var Nf = /^\s*>\s$/,
+    El = J.create({
         name: "blockquote",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         content: "block+",
@@ -11129,24 +11233,24 @@
         addKeyboardShortcuts() {
             return {
                 "Mod-Shift-b": () => this.editor.commands.toggleBlockquote()
             }
         },
         addInputRules() {
             return [Ue({
-                find: Af,
+                find: Nf,
                 type: this.type
             })]
         }
     });
-var vf = /(?:^|\s)(\*\*(?!\s+\*\*)((?:[^*]+))\*\*(?!\s+\*\*))$/,
-    Of = /(?:^|\s)(\*\*(?!\s+\*\*)((?:[^*]+))\*\*(?!\s+\*\*))/g,
-    Nf = /(?:^|\s)(__(?!\s+__)((?:[^_]+))__(?!\s+__))$/,
-    Df = /(?:^|\s)(__(?!\s+__)((?:[^_]+))__(?!\s+__))/g,
-    El = q.create({
+var Df = /(?:^|\s)(\*\*(?!\s+\*\*)((?:[^*]+))\*\*(?!\s+\*\*))$/,
+    If = /(?:^|\s)(\*\*(?!\s+\*\*)((?:[^*]+))\*\*(?!\s+\*\*))/g,
+    Pf = /(?:^|\s)(__(?!\s+__)((?:[^_]+))__(?!\s+__))$/,
+    Rf = /(?:^|\s)(__(?!\s+__)((?:[^_]+))__(?!\s+__))/g,
+    Cl = q.create({
         name: "bold",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -11182,32 +11286,32 @@
             return {
                 "Mod-b": () => this.editor.commands.toggleBold(),
                 "Mod-B": () => this.editor.commands.toggleBold()
             }
         },
         addInputRules() {
             return [Ke({
-                find: vf,
+                find: Df,
                 type: this.type
             }), Ke({
-                find: Nf,
+                find: Pf,
                 type: this.type
             })]
         },
         addPasteRules() {
             return [Ce({
-                find: Of,
+                find: If,
                 type: this.type
             }), Ce({
-                find: Df,
+                find: Rf,
                 type: this.type
             })]
         }
     });
-var If = J.create({
+var Lf = J.create({
         name: "listItem",
         addOptions() {
             return {
                 HTMLAttributes: {},
                 bulletListTypeName: "bulletList",
                 orderedListTypeName: "orderedList"
             }
@@ -11228,15 +11332,15 @@
             return {
                 Enter: () => this.editor.commands.splitListItem(this.name),
                 Tab: () => this.editor.commands.sinkListItem(this.name),
                 "Shift-Tab": () => this.editor.commands.liftListItem(this.name)
             }
         }
     }),
-    Cl = q.create({
+    Tl = q.create({
         name: "textStyle",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -11258,16 +11362,16 @@
                 }) => {
                     let t = vt(n, this.type);
                     return Object.entries(t).some(([, i]) => !!i) ? !0 : e.unsetMark(this.name)
                 }
             }
         }
     }),
-    Tl = /^\s*([-+*])\s$/,
-    Al = J.create({
+    Al = /^\s*([-+*])\s$/,
+    vl = J.create({
         name: "bulletList",
         addOptions() {
             return {
                 itemTypeName: "listItem",
                 HTMLAttributes: {},
                 keepMarks: !1,
                 keepAttributes: !1
@@ -11288,38 +11392,38 @@
             return ["ul", z(this.options.HTMLAttributes, n), 0]
         },
         addCommands() {
             return {
                 toggleBulletList: () => ({
                     commands: n,
                     chain: e
-                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(If.name, this.editor.getAttributes(Cl.name)).run() : n.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
+                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(Lf.name, this.editor.getAttributes(Tl.name)).run() : n.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
             }
         },
         addKeyboardShortcuts() {
             return {
                 "Mod-Shift-8": () => this.editor.commands.toggleBulletList()
             }
         },
         addInputRules() {
             let n = Ue({
-                find: Tl,
+                find: Al,
                 type: this.type
             });
             return (this.options.keepMarks || this.options.keepAttributes) && (n = Ue({
-                find: Tl,
+                find: Al,
                 type: this.type,
                 keepMarks: this.options.keepMarks,
                 keepAttributes: this.options.keepAttributes,
-                getAttributes: () => this.editor.getAttributes(Cl.name),
+                getAttributes: () => this.editor.getAttributes(Tl.name),
                 editor: this.editor
             })), [n]
         }
     });
-var vl = G.create({
+var Ol = G.create({
     name: "characterCount",
     addOptions() {
         return {
             limit: null,
             mode: "textSize"
         }
     },
@@ -11359,17 +11463,17 @@
                 return n.deleteRange(a, c), !(this.storage.characters({
                     node: n.doc
                 }) > t)
             }
         })]
     }
 });
-var Pf = /^```([a-z]+)?[\s\n]$/,
-    Rf = /^~~~([a-z]+)?[\s\n]$/,
-    Ol = J.create({
+var Bf = /^```([a-z]+)?[\s\n]$/,
+    Ff = /^~~~([a-z]+)?[\s\n]$/,
+    Nl = J.create({
         name: "codeBlock",
         addOptions() {
             return {
                 languageClassPrefix: "language-",
                 exitOnTripleEnter: !0,
                 exitOnArrowDown: !0,
                 HTMLAttributes: {}
@@ -11467,21 +11571,21 @@
                     let l = i.after();
                     return l === void 0 || r.nodeAt(l) ? !1 : n.commands.exitCode()
                 }
             }
         },
         addInputRules() {
             return [Qt({
-                find: Pf,
+                find: Bf,
                 type: this.type,
                 getAttributes: n => ({
                     language: n[1]
                 })
             }), Qt({
-                find: Rf,
+                find: Ff,
                 type: this.type,
                 getAttributes: n => ({
                     language: n[1]
                 })
             })]
         },
         addProseMirrorPlugins() {
@@ -11494,29 +11598,31 @@
                             r = e.clipboardData.getData("vscode-editor-data"),
                             i = r ? JSON.parse(r) : void 0,
                             s = i == null ? void 0 : i.mode;
                         if (!t || !s) return !1;
                         let {
                             tr: o
                         } = n.state;
-                        return o.replaceSelectionWith(this.type.create({
+                        return n.state.selection.from === n.state.doc.nodeSize - (1 + n.state.selection.$to.depth * 2) ? o.insert(n.state.selection.from - 1, this.type.create({
+                            language: s
+                        })) : o.replaceSelectionWith(this.type.create({
                             language: s
                         })), o.setSelection(P.near(o.doc.resolve(Math.max(0, o.selection.from - 2)))), o.insertText(t.replace(/\r\n?/g, `
 `)), o.setMeta("paste", !0), n.dispatch(o), !0
                     }
                 }
             })]
         }
     });
-var Nl = J.create({
+var Dl = J.create({
     name: "doc",
     topNode: !0,
     content: "block+"
 });
-var Dl = J.create({
+var Il = J.create({
     name: "hardBreak",
     addOptions() {
         return {
             keepMarks: !0,
             HTMLAttributes: {}
         }
     },
@@ -11573,15 +11679,15 @@
     addKeyboardShortcuts() {
         return {
             "Mod-Enter": () => this.editor.commands.setHardBreak(),
             "Shift-Enter": () => this.editor.commands.setHardBreak()
         }
     }
 });
-var Il = J.create({
+var Pl = J.create({
     name: "heading",
     addOptions() {
         return {
             levels: [1, 2, 3, 4, 5, 6],
             HTMLAttributes: {}
         }
     },
@@ -11634,24 +11740,24 @@
             type: this.type,
             getAttributes: {
                 level: n
             }
         }))
     }
 });
-var jn = 200,
+var Jn = 200,
     te = function() {};
 te.prototype.append = function(e) {
-    return e.length ? (e = te.from(e), !this.length && e || e.length < jn && this.leafAppend(e) || this.length < jn && e.leafPrepend(this) || this.appendInner(e)) : this
+    return e.length ? (e = te.from(e), !this.length && e || e.length < Jn && this.leafAppend(e) || this.length < Jn && e.leafPrepend(this) || this.appendInner(e)) : this
 };
 te.prototype.prepend = function(e) {
     return e.length ? te.from(e).append(this) : this
 };
 te.prototype.appendInner = function(e) {
-    return new Lf(this, e)
+    return new zf(this, e)
 };
 te.prototype.slice = function(e, t) {
     return e === void 0 && (e = 0), t === void 0 && (t = this.length), e >= t ? te.empty : this.sliceInner(Math.max(0, e), Math.min(this.length, t))
 };
 te.prototype.get = function(e) {
     if (!(e < 0 || e >= this.length)) return this.getInner(e)
 };
@@ -11662,17 +11768,17 @@
     t === void 0 && (t = 0), r === void 0 && (r = this.length);
     var i = [];
     return this.forEach(function(s, o) {
         return i.push(e(s, o))
     }, t, r), i
 };
 te.from = function(e) {
-    return e instanceof te ? e : e && e.length ? new Pl(e) : te.empty
+    return e instanceof te ? e : e && e.length ? new Rl(e) : te.empty
 };
-var Pl = function(n) {
+var Rl = function(n) {
     function e(r) {
         n.call(this), this.values = r
     }
     n && (e.__proto__ = n), e.prototype = Object.create(n && n.prototype), e.prototype.constructor = e;
     var t = {
         length: {
             configurable: !0
@@ -11690,25 +11796,25 @@
     }, e.prototype.forEachInner = function(i, s, o, l) {
         for (var a = s; a < o; a++)
             if (i(this.values[a], l + a) === !1) return !1
     }, e.prototype.forEachInvertedInner = function(i, s, o, l) {
         for (var a = s - 1; a >= o; a--)
             if (i(this.values[a], l + a) === !1) return !1
     }, e.prototype.leafAppend = function(i) {
-        if (this.length + i.length <= jn) return new e(this.values.concat(i.flatten()))
+        if (this.length + i.length <= Jn) return new e(this.values.concat(i.flatten()))
     }, e.prototype.leafPrepend = function(i) {
-        if (this.length + i.length <= jn) return new e(i.flatten().concat(this.values))
+        if (this.length + i.length <= Jn) return new e(i.flatten().concat(this.values))
     }, t.length.get = function() {
         return this.values.length
     }, t.depth.get = function() {
         return 0
     }, Object.defineProperties(e.prototype, t), e
 }(te);
-te.empty = new Pl([]);
-var Lf = function(n) {
+te.empty = new Rl([]);
+var zf = function(n) {
         function e(t, r) {
             n.call(this), this.left = t, this.right = r, this.length = t.length + r.length, this.depth = Math.max(t.depth, r.depth) + 1
         }
         return n && (e.__proto__ = n), e.prototype = Object.create(n && n.prototype), e.prototype.constructor = e, e.prototype.flatten = function() {
             return this.left.flatten().concat(this.right.flatten())
         }, e.prototype.getInner = function(r) {
             return r < this.left.length ? this.left.get(r) : this.right.get(r - this.left.length)
@@ -11729,15 +11835,15 @@
             var i = this.left.leafPrepend(r);
             if (i) return new e(i, this.right)
         }, e.prototype.appendInner = function(r) {
             return this.left.depth >= Math.max(this.right.depth, r.depth) + 1 ? new e(this.left, new e(this.right, r)) : new e(this, r)
         }, e
     }(te),
     Ei = te;
-var Bf = 500,
+var $f = 500,
     ft = class n {
         constructor(e, t) {
             this.items = e, this.eventCount = t
         }
         popEvent(e, t) {
             if (this.eventCount == 0) return null;
             let r = this.items.length;
@@ -11776,15 +11882,15 @@
             for (let d = 0; d < e.steps.length; d++) {
                 let u = e.steps[d].invert(e.docs[d]),
                     f = new Te(e.mapping.maps[d], u, t),
                     h;
                 (h = a && a.merge(f)) && (f = h, d ? s.pop() : l = l.slice(0, l.length - 1)), s.push(f), t && (o++, t = void 0), i || (a = f)
             }
             let c = o - r.depth;
-            return c > zf && (l = Ff(l, c), o -= c), new n(l.append(s), o)
+            return c > Vf && (l = Hf(l, c), o -= c), new n(l.append(s), o)
         }
         remapping(e, t) {
             let r = new Bt;
             return this.items.forEach((i, s) => {
                 let o = i.mirrorOffset != null && s - i.mirrorOffset >= e ? r.maps.length - i.mirrorOffset : void 0;
                 r.appendMap(i.map, o)
             }, e, t), r
@@ -11814,15 +11920,15 @@
                     g && l++, r.push(new Te(p, m, g))
                 } else r.push(new Te(p))
             }, i);
             let c = [];
             for (let f = t; f < o; f++) c.push(new Te(s.maps[f]));
             let d = this.items.slice(0, i).append(c).append(r),
                 u = new n(d, l);
-            return u.emptyItemCount() > Bf && (u = u.compress(this.items.length - r.length)), u
+            return u.emptyItemCount() > $f && (u = u.compress(this.items.length - r.length)), u
         }
         emptyItemCount() {
             let e = 0;
             return this.items.forEach(t => {
                 t.step || e++
             }), e
         }
@@ -11845,15 +11951,15 @@
                     }
                 } else o.map && r--
             }, this.items.length, 0), new n(Ei.from(i.reverse()), s)
         }
     };
 ft.empty = new ft(Ei.empty, 0);
 
-function Ff(n, e) {
+function Hf(n, e) {
     let t;
     return n.forEach((r, i) => {
         if (r.selection && e-- == 0) return t = i, !1
     }), n.slice(t)
 }
 var Te = class n {
         constructor(e, t, r, i) {
@@ -11867,42 +11973,42 @@
         }
     },
     Ae = class {
         constructor(e, t, r, i, s) {
             this.done = e, this.undone = t, this.prevRanges = r, this.prevTime = i, this.prevComposition = s
         }
     },
-    zf = 20;
+    Vf = 20;
 
-function $f(n, e, t, r) {
+function jf(n, e, t, r) {
     let i = t.getMeta(ut),
         s;
     if (i) return i.historyState;
-    t.getMeta(jf) && (n = new Ae(n.done, n.undone, null, 0, -1));
+    t.getMeta(Wf) && (n = new Ae(n.done, n.undone, null, 0, -1));
     let o = t.getMeta("appendedTransaction");
     if (t.steps.length == 0) return n;
-    if (o && o.getMeta(ut)) return o.getMeta(ut).redo ? new Ae(n.done.addTransform(t, void 0, r, Jn(e)), n.undone, Rl(t.mapping.maps[t.steps.length - 1]), n.prevTime, n.prevComposition) : new Ae(n.done, n.undone.addTransform(t, void 0, r, Jn(e)), null, n.prevTime, n.prevComposition);
+    if (o && o.getMeta(ut)) return o.getMeta(ut).redo ? new Ae(n.done.addTransform(t, void 0, r, qn(e)), n.undone, Ll(t.mapping.maps[t.steps.length - 1]), n.prevTime, n.prevComposition) : new Ae(n.done, n.undone.addTransform(t, void 0, r, qn(e)), null, n.prevTime, n.prevComposition);
     if (t.getMeta("addToHistory") !== !1 && !(o && o.getMeta("addToHistory") === !1)) {
         let l = t.getMeta("composition"),
-            a = n.prevTime == 0 || !o && n.prevComposition != l && (n.prevTime < (t.time || 0) - r.newGroupDelay || !Hf(t, n.prevRanges)),
-            c = o ? Ci(n.prevRanges, t.mapping) : Rl(t.mapping.maps[t.steps.length - 1]);
-        return new Ae(n.done.addTransform(t, a ? e.selection.getBookmark() : void 0, r, Jn(e)), ft.empty, c, t.time, l ?? n.prevComposition)
+            a = n.prevTime == 0 || !o && n.prevComposition != l && (n.prevTime < (t.time || 0) - r.newGroupDelay || !Jf(t, n.prevRanges)),
+            c = o ? Ci(n.prevRanges, t.mapping) : Ll(t.mapping.maps[t.steps.length - 1]);
+        return new Ae(n.done.addTransform(t, a ? e.selection.getBookmark() : void 0, r, qn(e)), ft.empty, c, t.time, l ?? n.prevComposition)
     } else return (s = t.getMeta("rebased")) ? new Ae(n.done.rebased(t, s), n.undone.rebased(t, s), Ci(n.prevRanges, t.mapping), n.prevTime, n.prevComposition) : new Ae(n.done.addMaps(t.mapping.maps), n.undone.addMaps(t.mapping.maps), Ci(n.prevRanges, t.mapping), n.prevTime, n.prevComposition)
 }
 
-function Hf(n, e) {
+function Jf(n, e) {
     if (!e) return !1;
     if (!n.docChanged) return !0;
     let t = !1;
     return n.mapping.maps[0].forEach((r, i) => {
         for (let s = 0; s < e.length; s += 2) r <= e[s + 1] && i >= e[s] && (t = !0)
     }), t
 }
 
-function Rl(n) {
+function Ll(n) {
     let e = [];
     return n.forEach((t, r, i, s) => e.push(i, s)), e
 }
 
 function Ci(n, e) {
     if (!n) return null;
     let t = [];
@@ -11910,57 +12016,57 @@
         let i = e.map(n[r], 1),
             s = e.map(n[r + 1], -1);
         i <= s && t.push(i, s)
     }
     return t
 }
 
-function Vf(n, e, t) {
-    let r = Jn(e),
+function qf(n, e, t) {
+    let r = qn(e),
         i = ut.get(e).spec.config,
         s = (t ? n.undone : n.done).popEvent(e, r);
     if (!s) return null;
     let o = s.selection.resolve(s.transform.doc),
         l = (t ? n.done : n.undone).addTransform(s.transform, e.selection.getBookmark(), i, r),
         a = new Ae(t ? l : s.remaining, t ? s.remaining : l, null, 0, -1);
     return s.transform.setSelection(o).setMeta(ut, {
         redo: t,
         historyState: a
     })
 }
 var Ti = !1,
-    Ll = null;
+    Bl = null;
 
-function Jn(n) {
+function qn(n) {
     let e = n.plugins;
-    if (Ll != e) {
-        Ti = !1, Ll = e;
+    if (Bl != e) {
+        Ti = !1, Bl = e;
         for (let t = 0; t < e.length; t++)
             if (e[t].spec.historyPreserveItems) {
                 Ti = !0;
                 break
             }
     }
     return Ti
 }
 var ut = new Y("history"),
-    jf = new Y("closeHistory");
+    Wf = new Y("closeHistory");
 
-function Bl(n = {}) {
+function Fl(n = {}) {
     return n = {
         depth: n.depth || 100,
         newGroupDelay: n.newGroupDelay || 500
     }, new W({
         key: ut,
         state: {
             init() {
                 return new Ae(ft.empty, ft.empty, null, 0, -1)
             },
             apply(e, t, r) {
-                return $f(t, r, e, n)
+                return jf(t, r, e, n)
             }
         },
         config: n,
         props: {
             handleDOMEvents: {
                 beforeinput(e, t) {
                     let r = t.inputType,
@@ -11968,29 +12074,29 @@
                     return i ? (t.preventDefault(), i(e.state, e.dispatch)) : !1
                 }
             }
         }
     })
 }
 
-function qn(n, e) {
+function Wn(n, e) {
     return (t, r) => {
         let i = ut.getState(t);
         if (!i || (n ? i.undone : i.done).eventCount == 0) return !1;
         if (r) {
-            let s = Vf(i, t, n);
+            let s = qf(i, t, n);
             s && r(e ? s.scrollIntoView() : s)
         }
         return !0
     }
 }
-var Ai = qn(!1, !0),
-    vi = qn(!0, !0),
-    gp = qn(!1, !1),
-    yp = qn(!0, !1);
+var Ai = Wn(!1, !0),
+    vi = Wn(!0, !0),
+    bp = Wn(!1, !1),
+    kp = Wn(!0, !1);
 var Oi = G.create({
     name: "history",
     addOptions() {
         return {
             depth: 100,
             newGroupDelay: 500
         }
@@ -12004,27 +12110,27 @@
             redo: () => ({
                 state: n,
                 dispatch: e
             }) => vi(n, e)
         }
     },
     addProseMirrorPlugins() {
-        return [Bl(this.options)]
+        return [Fl(this.options)]
     },
     addKeyboardShortcuts() {
         return {
             "Mod-z": () => this.editor.commands.undo(),
             "Shift-Mod-z": () => this.editor.commands.redo(),
             "Mod-y": () => this.editor.commands.redo(),
             "Mod-\u044F": () => this.editor.commands.undo(),
             "Shift-Mod-\u044F": () => this.editor.commands.redo()
         }
     }
 });
-var Fl = J.create({
+var zl = J.create({
     name: "horizontalRule",
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
     group: "block",
@@ -12069,25 +12175,25 @@
                     }
                     return !0
                 }).run()
             }
         }
     },
     addInputRules() {
-        return [Ml({
+        return [wl({
             find: /^(?:---|—-|___\s|\*\*\*\s)$/,
             type: this.type
         })]
     }
 });
-var Jf = /(?:^|\s)(\*(?!\s+\*)((?:[^*]+))\*(?!\s+\*))$/,
-    qf = /(?:^|\s)(\*(?!\s+\*)((?:[^*]+))\*(?!\s+\*))/g,
-    Wf = /(?:^|\s)(_(?!\s+_)((?:[^_]+))_(?!\s+_))$/,
-    Kf = /(?:^|\s)(_(?!\s+_)((?:[^_]+))_(?!\s+_))/g,
-    zl = q.create({
+var Kf = /(?:^|\s)(\*(?!\s+\*)((?:[^*]+))\*(?!\s+\*))$/,
+    Uf = /(?:^|\s)(\*(?!\s+\*)((?:[^*]+))\*(?!\s+\*))/g,
+    _f = /(?:^|\s)(_(?!\s+_)((?:[^_]+))_(?!\s+_))$/,
+    Gf = /(?:^|\s)(_(?!\s+_)((?:[^_]+))_(?!\s+_))/g,
+    $l = q.create({
         name: "italic",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -12122,27 +12228,27 @@
             return {
                 "Mod-i": () => this.editor.commands.toggleItalic(),
                 "Mod-I": () => this.editor.commands.toggleItalic()
             }
         },
         addInputRules() {
             return [Ke({
-                find: Jf,
+                find: Kf,
                 type: this.type
             }), Ke({
-                find: Wf,
+                find: _f,
                 type: this.type
             })]
         },
         addPasteRules() {
             return [Ce({
-                find: qf,
+                find: Uf,
                 type: this.type
             }), Ce({
-                find: Kf,
+                find: Gf,
                 type: this.type
             })]
         }
     });
 var Ni = J.create({
     name: "listItem",
     addOptions() {
@@ -12168,15 +12274,15 @@
         return {
             Enter: () => this.editor.commands.splitListItem(this.name),
             Tab: () => this.editor.commands.sinkListItem(this.name),
             "Shift-Tab": () => this.editor.commands.liftListItem(this.name)
         }
     }
 });
-var Uf = J.create({
+var Yf = J.create({
         name: "listItem",
         addOptions() {
             return {
                 HTMLAttributes: {},
                 bulletListTypeName: "bulletList",
                 orderedListTypeName: "orderedList"
             }
@@ -12197,15 +12303,15 @@
             return {
                 Enter: () => this.editor.commands.splitListItem(this.name),
                 Tab: () => this.editor.commands.sinkListItem(this.name),
                 "Shift-Tab": () => this.editor.commands.liftListItem(this.name)
             }
         }
     }),
-    $l = q.create({
+    Hl = q.create({
         name: "textStyle",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -12227,16 +12333,16 @@
                 }) => {
                     let t = vt(n, this.type);
                     return Object.entries(t).some(([, i]) => !!i) ? !0 : e.unsetMark(this.name)
                 }
             }
         }
     }),
-    Hl = /^(\d+)\.\s$/,
-    Vl = J.create({
+    Vl = /^(\d+)\.\s$/,
+    jl = J.create({
         name: "orderedList",
         addOptions() {
             return {
                 itemTypeName: "listItem",
                 HTMLAttributes: {},
                 keepMarks: !1,
                 keepAttributes: !1
@@ -12269,46 +12375,46 @@
             return e === 1 ? ["ol", z(this.options.HTMLAttributes, t), 0] : ["ol", z(this.options.HTMLAttributes, n), 0]
         },
         addCommands() {
             return {
                 toggleOrderedList: () => ({
                     commands: n,
                     chain: e
-                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(Uf.name, this.editor.getAttributes($l.name)).run() : n.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
+                }) => this.options.keepAttributes ? e().toggleList(this.name, this.options.itemTypeName, this.options.keepMarks).updateAttributes(Yf.name, this.editor.getAttributes(Hl.name)).run() : n.toggleList(this.name, this.options.itemTypeName, this.options.keepMarks)
             }
         },
         addKeyboardShortcuts() {
             return {
                 "Mod-Shift-7": () => this.editor.commands.toggleOrderedList()
             }
         },
         addInputRules() {
             let n = Ue({
-                find: Hl,
+                find: Vl,
                 type: this.type,
                 getAttributes: e => ({
                     start: +e[1]
                 }),
                 joinPredicate: (e, t) => t.childCount + t.attrs.start === +e[1]
             });
             return (this.options.keepMarks || this.options.keepAttributes) && (n = Ue({
-                find: Hl,
+                find: Vl,
                 type: this.type,
                 keepMarks: this.options.keepMarks,
                 keepAttributes: this.options.keepAttributes,
                 getAttributes: e => ({
                     start: +e[1],
-                    ...this.editor.getAttributes($l.name)
+                    ...this.editor.getAttributes(Hl.name)
                 }),
                 joinPredicate: (e, t) => t.childCount + t.attrs.start === +e[1],
                 editor: this.editor
             })), [n]
         }
     });
-var jl = J.create({
+var Jl = J.create({
     name: "paragraph",
     priority: 1e3,
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
@@ -12333,15 +12439,15 @@
     },
     addKeyboardShortcuts() {
         return {
             "Mod-Alt-0": () => this.editor.commands.setParagraph()
         }
     }
 });
-var Jl = G.create({
+var ql = G.create({
     name: "placeholder",
     addOptions() {
         return {
             emptyEditorClass: "is-editor-empty",
             emptyNodeClass: "is-empty",
             placeholder: "Write something \u2026",
             showOnlyWhenEditable: !0,
@@ -12388,17 +12494,17 @@
                         return this.options.includeChildren
                     }), ue.create(n, s)
                 }
             }
         })]
     }
 });
-var _f = /(?:^|\s)(~~(?!\s+~~)((?:[^~]+))~~(?!\s+~~))$/,
-    Gf = /(?:^|\s)(~~(?!\s+~~)((?:[^~]+))~~(?!\s+~~))/g,
-    ql = q.create({
+var Xf = /(?:^|\s)(~~(?!\s+~~)((?:[^~]+))~~(?!\s+~~))$/,
+    Zf = /(?:^|\s)(~~(?!\s+~~)((?:[^~]+))~~(?!\s+~~))/g,
+    Wl = q.create({
         name: "strike",
         addOptions() {
             return {
                 HTMLAttributes: {}
             }
         },
         parseHTML() {
@@ -12430,30 +12536,30 @@
                 unsetStrike: () => ({
                     commands: n
                 }) => n.unsetMark(this.name)
             }
         },
         addKeyboardShortcuts() {
             let n = {};
-            return Hn() ? n["Mod-Shift-s"] = () => this.editor.commands.toggleStrike() : n["Ctrl-Shift-s"] = () => this.editor.commands.toggleStrike(), n
+            return Vn() ? n["Mod-Shift-s"] = () => this.editor.commands.toggleStrike() : n["Ctrl-Shift-s"] = () => this.editor.commands.toggleStrike(), n
         },
         addInputRules() {
             return [Ke({
-                find: _f,
+                find: Xf,
                 type: this.type
             })]
         },
         addPasteRules() {
             return [Ce({
-                find: Gf,
+                find: Zf,
                 type: this.type
             })]
         }
     });
-var Wl = q.create({
+var Kl = q.create({
     name: "subscript",
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
     parseHTML() {
@@ -12486,15 +12592,15 @@
     },
     addKeyboardShortcuts() {
         return {
             "Mod-,": () => this.editor.commands.toggleSubscript()
         }
     }
 });
-var Kl = q.create({
+var Ul = q.create({
     name: "superscript",
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
     parseHTML() {
@@ -12527,19 +12633,19 @@
     },
     addKeyboardShortcuts() {
         return {
             "Mod-.": () => this.editor.commands.toggleSuperscript()
         }
     }
 });
-var Ul = J.create({
+var _l = J.create({
     name: "text",
     group: "inline"
 });
-var _l = G.create({
+var Gl = G.create({
     name: "textAlign",
     addOptions() {
         return {
             types: [],
             alignments: ["left", "center", "right", "justify"],
             defaultAlignment: "left"
         }
@@ -12575,15 +12681,15 @@
             "Mod-Shift-l": () => this.editor.commands.setTextAlign("left"),
             "Mod-Shift-e": () => this.editor.commands.setTextAlign("center"),
             "Mod-Shift-r": () => this.editor.commands.setTextAlign("right"),
             "Mod-Shift-j": () => this.editor.commands.setTextAlign("justify")
         }
     }
 });
-var Gl = q.create({
+var Yl = q.create({
     name: "underline",
     addOptions() {
         return {
             HTMLAttributes: {}
         }
     },
     parseHTML() {
@@ -12616,15 +12722,15 @@
     addKeyboardShortcuts() {
         return {
             "Mod-u": () => this.editor.commands.toggleUnderline(),
             "Mod-U": () => this.editor.commands.toggleUnderline()
         }
     }
 });
-var Yl = G.create({
+var Xl = G.create({
     name: "textIndent",
     addOptions() {
         return {
             types: []
         }
     },
     addGlobalAttributes() {
@@ -12650,15 +12756,15 @@
             })),
             unsetTextIndent: () => ({
                 commands: n
             }) => this.options.types.every(e => n.resetAttributes(e, ["textIndent"]))
         }
     }
 });
-var Xl = G.create({
+var Zl = G.create({
     name: "textMargin",
     addOptions() {
         return {
             types: [],
             maxIndentLevel: 8
         }
     },
@@ -12696,15 +12802,15 @@
             },
             unsetTextMargin: () => ({
                 commands: n
             }) => this.options.types.every(e => n.resetAttributes(e, ["textMargin"]))
         }
     }
 });
-var Zl = q.create({
+var Ql = q.create({
     name: "textColor",
     addOptions() {
         return {
             allowedClasses: []
         }
     },
     addAttributes() {
@@ -12755,15 +12861,15 @@
             }),
             unsetColor: () => ({
                 commands: n
             }) => n.unsetMark(this.name)
         }
     }
 });
-var ta = tn(pa());
+var na = tn(ma());
 var Di = function() {
     "use strict";
 
     function n(i, s) {
         function o() {
             this.constructor = i
         }
@@ -12881,41 +12987,41 @@
             l = s.grammarSource,
             a = {
                 FunctionCode: zi
             },
             c = zi,
             d = "//",
             u = /^[\n\r\u2028\u2029]/,
-            f = oa(),
-            h = ia("//", !1),
-            p = sa([`
+            f = la(),
+            h = sa("//", !1),
+            p = oa([`
 `, "\r", "\u2028", "\u2029"], !1, !1),
             m = function(S) {
                 return S.replaceAll(new RegExp("[	]+", "g"), " ")
             },
             g = function(S, C, I) {
-                return I && C.push(I), C.reduce((F, $) => `${F} ${$}`, S).replaceAll(new RegExp("[	]+", "g"), " ")
+                return I && C.push(I), C.reduce((F, H) => `${F} ${H}`, S).replaceAll(new RegExp("[	]+", "g"), " ")
             },
             k = function(S) {
                 return S
             },
             R = function(S) {
                 return S
             },
-            H = function(S) {
+            $ = function(S) {
                 return S
             },
             b = 0,
             A = 0,
             v = [{
                 line: 1,
                 column: 1
             }],
             y = 0,
-            w = [],
+            M = [],
             x = 0,
             N;
         if ("startRule" in s) {
             if (!(s.startRule in a)) throw new Error(`Can't start parsing from rule "` + s.startRule + '".');
             c = a[s.startRule]
         }
 
@@ -12923,64 +13029,64 @@
             return i.substring(A, b)
         }
 
         function ne() {
             return A
         }
 
-        function Yf() {
+        function Qf() {
             return {
                 source: l,
                 start: A,
                 end: b
             }
         }
 
-        function Xf() {
+        function eh() {
             return Ot(A, b)
         }
 
-        function Zf(S, C) {
-            throw C = C !== void 0 ? C : Ot(A, b), Fi([aa(S)], i.substring(A, b), C)
+        function th(S, C) {
+            throw C = C !== void 0 ? C : Ot(A, b), Fi([ca(S)], i.substring(A, b), C)
         }
 
-        function Qf(S, C) {
-            throw C = C !== void 0 ? C : Ot(A, b), ca(S, C)
+        function nh(S, C) {
+            throw C = C !== void 0 ? C : Ot(A, b), da(S, C)
         }
 
-        function ia(S, C) {
+        function sa(S, C) {
             return {
                 type: "literal",
                 text: S,
                 ignoreCase: C
             }
         }
 
-        function sa(S, C, I) {
+        function oa(S, C, I) {
             return {
                 type: "class",
                 parts: S,
                 inverted: C,
                 ignoreCase: I
             }
         }
 
-        function oa() {
+        function la() {
             return {
                 type: "any"
             }
         }
 
-        function la() {
+        function aa() {
             return {
                 type: "end"
             }
         }
 
-        function aa(S) {
+        function ca(S) {
             return {
                 type: "other",
                 description: S
             }
         }
 
         function Bi(S) {
@@ -12994,112 +13100,112 @@
                 }; I < S;) i.charCodeAt(I) === 10 ? (C.line++, C.column = 1) : C.column++, I++;
             return v[S] = C, C
         }
 
         function Ot(S, C, I) {
             var D = Bi(S),
                 F = Bi(C),
-                $ = {
+                H = {
                     source: l,
                     start: {
                         offset: S,
                         line: D.line,
                         column: D.column
                     },
                     end: {
                         offset: C,
                         line: F.line,
                         column: F.column
                     }
                 };
-            return I && l && typeof l.offset == "function" && ($.start = l.offset($.start), $.end = l.offset($.end)), $
+            return I && l && typeof l.offset == "function" && (H.start = l.offset(H.start), H.end = l.offset(H.end)), H
         }
 
         function Be(S) {
-            b < y || (b > y && (y = b, w = []), w.push(S))
+            b < y || (b > y && (y = b, M = []), M.push(S))
         }
 
-        function ca(S, C) {
+        function da(S, C) {
             return new e(S, null, null, C)
         }
 
         function Fi(S, C, I) {
             return new e(e.buildMessage(S, C), S, C, I)
         }
 
         function zi() {
             var S, C;
-            return S = Wn(), S === o && (S = b, C = $i(), C !== o && (A = S, C = m(C)), S = C), S
+            return S = Kn(), S === o && (S = b, C = $i(), C !== o && (A = S, C = m(C)), S = C), S
         }
 
-        function Wn() {
+        function Kn() {
             var S, C, I, D;
-            if (S = b, C = da(), C !== o) {
-                for (I = [], D = Wn(); D !== o;) I.push(D), D = Wn();
+            if (S = b, C = ua(), C !== o) {
+                for (I = [], D = Kn(); D !== o;) I.push(D), D = Kn();
                 D = $i(), D !== o ? (A = S, S = g(C, I, D)) : (b = S, S = o)
             } else b = S, S = o;
             return S
         }
 
-        function da() {
+        function ua() {
             var S, C, I;
-            return S = b, C = Hi(), C !== o ? (I = Fe(), I !== o ? (A = S, S = k(C)) : (b = S, S = o)) : (b = S, S = o), S === o && (S = b, C = Un(), I = Fe(), I !== o ? (A = S, S = R(C)) : (b = S, S = o)), S
+            return S = b, C = Hi(), C !== o ? (I = Fe(), I !== o ? (A = S, S = k(C)) : (b = S, S = o)) : (b = S, S = o), S === o && (S = b, C = _n(), I = Fe(), I !== o ? (A = S, S = R(C)) : (b = S, S = o)), S
         }
 
         function $i() {
             var S;
-            return S = Hi(), S === o && (S = Un()), S
+            return S = Hi(), S === o && (S = _n()), S
         }
 
         function Hi() {
-            var S, C, I, D, F, $, he;
-            for (S = b, C = b, I = [], D = b, F = b, x++, $ = Kn(), x--, $ === o ? F = void 0 : (b = F, F = o), F !== o ? ($ = b, x++, he = Fe(), x--, he === o ? $ = void 0 : (b = $, $ = o), $ !== o ? (i.length > b ? (he = i.charAt(b), b++) : (he = o, x === 0 && Be(f)), he !== o ? (F = [F, $, he], D = F) : (b = D, D = o)) : (b = D, D = o)) : (b = D, D = o); D !== o;) I.push(D), D = b, F = b, x++, $ = Kn(), x--, $ === o ? F = void 0 : (b = F, F = o), F !== o ? ($ = b, x++, he = Fe(), x--, he === o ? $ = void 0 : (b = $, $ = o), $ !== o ? (i.length > b ? (he = i.charAt(b), b++) : (he = o, x === 0 && Be(f)), he !== o ? (F = [F, $, he], D = F) : (b = D, D = o)) : (b = D, D = o)) : (b = D, D = o);
-            return C = i.substring(C, b), I = Kn(), I !== o ? (D = Un(), A = S, S = H(C)) : (b = S, S = o), S
+            var S, C, I, D, F, H, he;
+            for (S = b, C = b, I = [], D = b, F = b, x++, H = Un(), x--, H === o ? F = void 0 : (b = F, F = o), F !== o ? (H = b, x++, he = Fe(), x--, he === o ? H = void 0 : (b = H, H = o), H !== o ? (i.length > b ? (he = i.charAt(b), b++) : (he = o, x === 0 && Be(f)), he !== o ? (F = [F, H, he], D = F) : (b = D, D = o)) : (b = D, D = o)) : (b = D, D = o); D !== o;) I.push(D), D = b, F = b, x++, H = Un(), x--, H === o ? F = void 0 : (b = F, F = o), F !== o ? (H = b, x++, he = Fe(), x--, he === o ? H = void 0 : (b = H, H = o), H !== o ? (i.length > b ? (he = i.charAt(b), b++) : (he = o, x === 0 && Be(f)), he !== o ? (F = [F, H, he], D = F) : (b = D, D = o)) : (b = D, D = o)) : (b = D, D = o);
+            return C = i.substring(C, b), I = Un(), I !== o ? (D = _n(), A = S, S = $(C)) : (b = S, S = o), S
         }
 
-        function Kn() {
+        function Un() {
             var S;
             return i.substr(b, 2) === d ? (S = d, b += 2) : (S = o, x === 0 && Be(h)), S
         }
 
-        function Un() {
-            var S, C, I, D, F, $;
-            if (S = b, C = [], I = b, D = b, x++, F = [], $ = Fe(), $ !== o)
-                for (; $ !== o;) F.push($), $ = Fe();
+        function _n() {
+            var S, C, I, D, F, H;
+            if (S = b, C = [], I = b, D = b, x++, F = [], H = Fe(), H !== o)
+                for (; H !== o;) F.push(H), H = Fe();
             else F = o;
             for (x--, F === o ? D = void 0 : (b = D, D = o), D !== o ? (i.length > b ? (F = i.charAt(b), b++) : (F = o, x === 0 && Be(f)), F !== o ? (D = [D, F], I = D) : (b = I, I = o)) : (b = I, I = o); I !== o;) {
-                if (C.push(I), I = b, D = b, x++, F = [], $ = Fe(), $ !== o)
-                    for (; $ !== o;) F.push($), $ = Fe();
+                if (C.push(I), I = b, D = b, x++, F = [], H = Fe(), H !== o)
+                    for (; H !== o;) F.push(H), H = Fe();
                 else F = o;
                 x--, F === o ? D = void 0 : (b = D, D = o), D !== o ? (i.length > b ? (F = i.charAt(b), b++) : (F = o, x === 0 && Be(f)), F !== o ? (D = [D, F], I = D) : (b = I, I = o)) : (b = I, I = o)
             }
             return S = i.substring(S, b), S
         }
 
         function Fe() {
             var S, C;
             if (S = [], u.test(i.charAt(b)) ? (C = i.charAt(b), b++) : (C = o, x === 0 && Be(p)), C !== o)
                 for (; C !== o;) S.push(C), u.test(i.charAt(b)) ? (C = i.charAt(b), b++) : (C = o, x === 0 && Be(p));
             else S = o;
             return S
         }
         if (N = c(), N !== o && b === i.length) return N;
-        throw N !== o && b < i.length && Be(la()), Fi(w, y < i.length ? i.charAt(y) : null, y < i.length ? Ot(y, y + 1) : Ot(y, y))
+        throw N !== o && b < i.length && Be(aa()), Fi(M, y < i.length ? i.charAt(y) : null, y < i.length ? Ot(y, y + 1) : Ot(y, y))
     }
     return {
         SyntaxError: e,
         parse: r
     }
 }();
 Di.SyntaxError.prototype.name = "PeggySyntaxError";
-var Ql = Di.parse,
-    rm = Di.SyntaxError;
-var na = tn(ha()),
-    ra = tn(fa()),
-    Ii = tn(ua()),
+var ea = Di.parse,
+    om = Di.SyntaxError;
+var ra = tn(pa()),
+    ia = tn(ha()),
+    Ii = tn(fa()),
     K = class {
         constructor(e, t, r) {
             this.extensions = [];
             this.name = t, this.button = r
         }
         installEventHandler(e) {
             this.button.addEventListener("click", () => this.clicked(e))
@@ -13144,234 +13250,234 @@
         }
     },
     Pi;
 (b => {
     class n extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [El]
+            this.extensions = [Cl]
         }
         clicked(y) {
             y.chain().focus().toggleBold().run(), this.activate(y)
         }
     }
     b.BoldAction = n;
     class e extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [zl]
+            this.extensions = [$l]
         }
         clicked(y) {
             y.chain().focus().toggleItalic().run(), this.activate(y)
         }
     }
     b.ItalicAction = e;
     class t extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [ql]
+            this.extensions = [Wl]
         }
         clicked(y) {
             y.chain().focus().toggleStrike().run(), this.activate(y)
         }
     }
     b.StrikeAction = t;
     class r extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [Wl]
+            this.extensions = [Kl]
         }
         clicked(y) {
             y.chain().focus().unsetSuperscript().run(), y.chain().focus().toggleSubscript().run(), this.activate(y)
         }
     }
     b.SubscriptAction = r;
     class i extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [Kl]
+            this.extensions = [Ul]
         }
         clicked(y) {
             y.chain().focus().unsetSubscript().run(), y.chain().focus().toggleSuperscript().run(), this.activate(y)
         }
     }
     b.SuperscriptAction = i;
     class s extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [Gl]
+            this.extensions = [Yl]
         }
         clicked(y) {
             y.chain().focus().toggleUnderline().run(), this.activate(y)
         }
     }
     b.UnderlineAction = s;
     class o extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [Al, Ni]
+            this.extensions = [vl, Ni]
         }
         clicked(y) {
             y.chain().focus().toggleBulletList().run(), this.activate(y)
         }
     }
     b.BulletListAction = o;
     class l extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [wl]
+            this.extensions = [El]
         }
         clicked(y) {
             y.chain().focus().toggleBlockquote().run(), this.activate(y)
         }
     }
     b.BlockquoteAction = l;
     class a extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [Ol]
+            this.extensions = [Nl]
         }
         clicked(y) {
             y.chain().focus().toggleCodeBlock().run(), this.activate(y)
         }
     }
     b.CodeBlockAction = a;
     class c extends K {
         clicked(v) {
             v.chain().focus().setHardBreak().run(), this.activate(v)
         }
     }
     b.HardBreakAction = c;
     class d extends en {
-        constructor(y, w, x) {
-            super(y, w, x, '[richtext-click^="color:"]');
+        constructor(y, M, x) {
+            super(y, M, x, '[richtext-click^="color:"]');
             this.colors = [];
             this.allowedClasses = [];
             if (!(x.nextElementSibling instanceof HTMLUListElement) || x.nextElementSibling.getAttribute("role") !== "menu") throw new Error('Text color requires a sibling element <ul role="menu">\u2026</ul>');
             this.collecColors()
         }
         collecColors() {
             this.dropdownItems.forEach(y => {
-                let w = this.extractColor(y);
-                if (w)
-                    if (/^rgb\(\d{1,3}, \d{1,3}, \d{1,3}\)$/.test(w)) {
+                let M = this.extractColor(y);
+                if (M)
+                    if (/^rgb\(\d{1,3}, \d{1,3}, \d{1,3}\)$/.test(M)) {
                         if (this.allowedClasses.length !== 0) throw new Error(`In element ${y} can not mix class based with style based colors.`);
-                        this.colors.push(w)
-                    } else if (/^-?[_a-zA-Z]+[_a-zA-Z0-9-]*$/.test(w)) this.allowedClasses.push(w);
-                else throw new Error(`${w} is not a valid color.`)
+                        this.colors.push(M)
+                    } else if (/^-?[_a-zA-Z]+[_a-zA-Z0-9-]*$/.test(M)) this.allowedClasses.push(M);
+                else throw new Error(`${M} is not a valid color.`)
             })
         }
         extractColor(y) {
             var x;
-            let w = ((x = y.getAttribute("richtext-click")) == null ? void 0 : x.split(":")) ?? [];
-            if (w.length !== 2) throw new Error(`Element ${y} requires attribute 'richtext-click'.`);
-            return w[1] === "null" ? null : w[1]
+            let M = ((x = y.getAttribute("richtext-click")) == null ? void 0 : x.split(":")) ?? [];
+            if (M.length !== 2) throw new Error(`Element ${y} requires attribute 'richtext-click'.`);
+            return M[1] === "null" ? null : M[1]
         }
         clicked() {}
         activate(y) {
-            let w = !1,
+            let M = !1,
                 x = this.button.querySelector("svg > rect");
             this.dropdownItems.forEach(N => {
                 let V = this.extractColor(N);
                 V && y.isActive({
                     textColor: V
-                }) && (this.allowedClasses.length === 0 ? x == null || x.setAttribute("fill", V) : (x == null || x.classList.forEach(ne => x.classList.remove(ne)), x == null || x.classList.add(V)), w = !0)
-            }), this.button.classList.toggle("active", w), w || (this.allowedClasses.length === 0 ? x == null || x.removeAttribute("fill") : x == null || x.classList.forEach(N => x.classList.remove(N)))
+                }) && (this.allowedClasses.length === 0 ? x == null || x.setAttribute("fill", V) : (x == null || x.classList.forEach(ne => x.classList.remove(ne)), x == null || x.classList.add(V)), M = !0)
+            }), this.button.classList.toggle("active", M), M || (this.allowedClasses.length === 0 ? x == null || x.removeAttribute("fill") : x == null || x.classList.forEach(N => x.classList.remove(N)))
         }
         extendExtensions(y) {
-            let w = !0;
+            let M = !0;
             y.forEach(x => {
                 if (x.name === "textColor") throw new Error("RichtextArea allows only one control element with 'textColor'.")
-            }), y.push(Zl.configure({
+            }), y.push(Ql.configure({
                 allowedClasses: this.allowedClasses
             }))
         }
-        toggleMenu(y, w) {
-            super.toggleMenu(y, w), this.dropdownItems.forEach(x => {
+        toggleMenu(y, M) {
+            super.toggleMenu(y, M), this.dropdownItems.forEach(x => {
                 var V;
                 let N = this.extractColor(x);
                 (V = x.parentElement) == null || V.classList.toggle("active", y.isActive({
                     textColor: N
                 }))
             })
         }
-        toggleItem(y, w) {
+        toggleItem(y, M) {
             let x = y.target instanceof Element ? y.target : null;
             for (; x;) {
                 if (x instanceof HTMLAnchorElement) {
                     let N = this.extractColor(x);
-                    N ? w.chain().focus().setColor(N).run() : w.chain().focus().unsetColor().run(), this.activate(w), this.toggleMenu(w, !1);
+                    N ? M.chain().focus().setColor(N).run() : M.chain().focus().unsetColor().run(), this.activate(M), this.toggleMenu(M, !1);
                     break
                 }
                 x = x.parentElement
             }
         }
     }
     b.TextColorAction = d;
     class u extends K {
-        constructor(y, w, x) {
-            super(y, w, x);
+        constructor(y, M, x) {
+            super(y, M, x);
             this.options = {
                 types: ["heading", "paragraph"]
             };
-            let N = w.split(":");
+            let N = M.split(":");
             this.indent = N[1] ?? ""
         }
         clicked(y) {
             y.isActive({
                 textIndent: this.indent
             }) ? y.chain().focus().unsetTextIndent().run() : y.chain().focus().setTextIndent(this.indent).run(), this.activate(y)
         }
         activate(y) {
             this.button.classList.toggle("active", y.isActive({
                 textIndent: this.indent
             }))
         }
         extendExtensions(y) {
-            y.filter(w => w.name === "textIndent").length || y.push(Yl.configure(this.options))
+            y.filter(M => M.name === "textIndent").length || y.push(Xl.configure(this.options))
         }
     }
     b.TextIndentAction = u;
     class f extends K {
-        constructor(y, w, x) {
-            super(y, w, x);
+        constructor(y, M, x) {
+            super(y, M, x);
             this.options = {
                 types: ["heading", "paragraph"],
                 maxIndentLevel: 5
             };
-            let N = w.split(":");
+            let N = M.split(":");
             this.indent = N[1] ?? ""
         }
         clicked(y) {
             this.indent === "increase" ? y.chain().focus().increaseTextMargin().run() : this.indent === "decrease" ? y.chain().focus().decreaseTextMargin().run() : y.chain().focus().unsetTextMargin().run(), this.activate(y)
         }
         activate(y) {
             this.button.classList.toggle("active", y.isActive({
                 textMargin: this.indent
             }))
         }
         extendExtensions(y) {
-            y.filter(w => w.name === "textMargin").length || y.push(Xl.configure(this.options))
+            y.filter(M => M.name === "textMargin").length || y.push(Zl.configure(this.options))
         }
     }
     b.TextMarginAction = f;
     class h extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [Vl, Ni]
+            this.extensions = [jl, Ni]
         }
         clicked(y) {
             y.chain().focus().toggleOrderedList().run(), this.activate(y)
         }
     }
     b.OrderedListAction = h;
     class p extends K {
         constructor() {
             super(...arguments);
-            this.extensions = [Fl]
+            this.extensions = [zl]
         }
         clicked(y) {
             y.chain().focus().setHorizontalRule().run()
         }
     }
     b.HorizontalRuleAction = p;
     class m extends K {
@@ -13397,149 +13503,149 @@
         }
         clicked(y) {
             y.commands.redo()
         }
     }
     b.RedoAction = k;
     class R extends en {
-        constructor(y, w, x) {
+        constructor(y, M, x) {
             var N;
-            super(y, w, x, '[richtext-click^="heading:"]');
+            super(y, M, x, '[richtext-click^="heading:"]');
             this.levels = [];
             this.dropdownMenu ? this.dropdownItems.forEach(V => this.levels.push(this.extractLevel(V))) : this.levels.push(this.extractLevel(this.button)), this.defaultIcon = (N = this.button.querySelector("svg")) == null ? void 0 : N.cloneNode(!0)
         }
         extractLevel(y) {
             var N;
-            let w = ((N = y.getAttribute("richtext-click")) == null ? void 0 : N.split(":")) ?? [];
-            if (w.length !== 2) throw new Error(`Element ${y} requires attribute 'richtext-click'.`);
-            return parseInt(w[1])
+            let M = ((N = y.getAttribute("richtext-click")) == null ? void 0 : N.split(":")) ?? [];
+            if (M.length !== 2) throw new Error(`Element ${y} requires attribute 'richtext-click'.`);
+            return parseInt(M[1])
         }
         clicked() {}
         activate(y) {
             if (this.dropdownMenu) {
-                let w = !1;
+                let M = !1;
                 this.dropdownItems.forEach(x => {
                     var ne;
                     let N = this.extractLevel(x),
                         V = (ne = x.querySelector("svg")) == null ? void 0 : ne.cloneNode(!0);
                     y.isActive("heading", {
                         level: N
-                    }) && V && (this.button.replaceChildren(V), w = !0)
-                }), this.button.classList.toggle("active", w), w || this.button.replaceChildren(this.defaultIcon)
+                    }) && V && (this.button.replaceChildren(V), M = !0)
+                }), this.button.classList.toggle("active", M), M || this.button.replaceChildren(this.defaultIcon)
             } else {
-                let w = this.extractLevel(this.button);
+                let M = this.extractLevel(this.button);
                 this.button.classList.toggle("active", y.isActive("heading", {
-                    level: w
+                    level: M
                 }))
             }
         }
         extendExtensions(y) {
-            let w = !0;
+            let M = !0;
             y.forEach(x => {
-                x.name === "heading" && (x.options.levels.push(...this.levels), w = !1)
-            }), w && y.push(Il.configure({
+                x.name === "heading" && (x.options.levels.push(...this.levels), M = !1)
+            }), M && y.push(Pl.configure({
                 levels: this.levels
             }))
         }
-        toggleMenu(y, w) {
-            super.toggleMenu(y, w), this.dropdownItems.forEach(x => {
+        toggleMenu(y, M) {
+            super.toggleMenu(y, M), this.dropdownItems.forEach(x => {
                 var V;
                 let N = this.extractLevel(x);
                 (V = x.parentElement) == null || V.classList.toggle("active", y.isActive("heading", {
                     level: N
                 }))
             })
         }
-        toggleItem(y, w) {
+        toggleItem(y, M) {
             var N;
             let x = y.target instanceof Element ? y.target : null;
             for (; x;) {
                 if (x instanceof HTMLButtonElement || x instanceof HTMLAnchorElement) {
                     let V = this.extractLevel(x);
-                    w.chain().focus().setHeading({
+                    M.chain().focus().setHeading({
                         level: V
-                    }).run(), this.activate(w), this.toggleMenu(w, !1);
+                    }).run(), this.activate(M), this.toggleMenu(M, !1);
                     let ne = (N = x.querySelector("svg")) == null ? void 0 : N.cloneNode(!0);
                     ne && this.button.replaceChildren(ne);
                     break
                 }
                 x = x.parentElement
             }
         }
     }
     b.HeadingAction = R;
-    class H extends en {
-        constructor(y, w, x) {
+    class $ extends en {
+        constructor(y, M, x) {
             var N;
-            super(y, w, x, '[richtext-click^="alignment:"]');
+            super(y, M, x, '[richtext-click^="alignment:"]');
             this.options = {
                 types: ["heading", "paragraph"],
                 alignments: [],
                 defaultAlignment: ""
             };
             this.dropdownMenu ? this.dropdownItems.forEach(V => {
                 this.options.alignments.push(this.extractAlignment(V))
             }) : this.options.alignments.push(this.extractAlignment(this.button)), this.defaultIcon = (N = this.button.querySelector("svg")) == null ? void 0 : N.cloneNode(!0)
         }
         extractAlignment(y) {
             var x;
-            let w = ((x = y.getAttribute("richtext-click")) == null ? void 0 : x.split(":")) ?? [];
-            if (w.length !== 2) throw new Error(`Element ${y} requires attribute 'richtext-click'.`);
-            return w[1]
+            let M = ((x = y.getAttribute("richtext-click")) == null ? void 0 : x.split(":")) ?? [];
+            if (M.length !== 2) throw new Error(`Element ${y} requires attribute 'richtext-click'.`);
+            return M[1]
         }
         clicked() {}
         activate(y) {
             if (this.dropdownMenu) {
-                let w = !1;
+                let M = !1;
                 this.dropdownItems.forEach(x => {
                     var ne;
                     let N = this.extractAlignment(x),
                         V = (ne = x.querySelector("svg")) == null ? void 0 : ne.cloneNode(!0);
                     y.isActive({
                         textAlign: N
-                    }) && V && (this.button.replaceChildren(V), w = !0)
-                }), w || this.button.replaceChildren(this.defaultIcon)
+                    }) && V && (this.button.replaceChildren(V), M = !0)
+                }), M || this.button.replaceChildren(this.defaultIcon)
             } else {
-                let w = this.extractAlignment(this.button);
+                let M = this.extractAlignment(this.button);
                 this.button.classList.toggle("active", y.isActive({
-                    textAlign: w
+                    textAlign: M
                 }))
             }
         }
         extendExtensions(y) {
-            let w = !0;
+            let M = !0;
             y.forEach(x => {
-                x.name === "textAlign" && (x.options.alignments.push(...this.options.alignments), w = !1)
-            }), w && y.push(_l.configure(this.options))
+                x.name === "textAlign" && (x.options.alignments.push(...this.options.alignments), M = !1)
+            }), M && y.push(Gl.configure(this.options))
         }
-        toggleMenu(y, w) {
-            super.toggleMenu(y, w), this.dropdownItems.forEach(x => {
+        toggleMenu(y, M) {
+            super.toggleMenu(y, M), this.dropdownItems.forEach(x => {
                 var V;
                 let N = this.extractAlignment(x);
                 (V = x.parentElement) == null || V.classList.toggle("active", y.isActive({
                     textAlign: N
                 }))
             })
         }
-        toggleItem(y, w) {
+        toggleItem(y, M) {
             var N;
             let x = y.target instanceof Element ? y.target : null;
             for (; x;) {
                 if (x instanceof HTMLButtonElement || x instanceof HTMLAnchorElement) {
                     let V = this.extractAlignment(x);
-                    w.chain().focus().setTextAlign(V).run(), this.activate(w), this.toggleMenu(w, !1);
+                    M.chain().focus().setTextAlign(V).run(), this.activate(M), this.toggleMenu(M, !1);
                     let ne = (N = x.querySelector("svg")) == null ? void 0 : N.cloneNode(!0);
                     ne && this.button.replaceChildren(ne);
                     break
                 }
                 x = x.parentElement
             }
         }
     }
-    b.TextAlignAction = H
+    b.TextAlignAction = $
 })(Pi || (Pi = {}));
 var Ri = class extends Vi {
         constructor(t, r, i) {
             super(t);
             this.inputElements = new Array;
             this.textSelectionField = null;
             this.applyAttributes = () => {};
@@ -13570,15 +13676,15 @@
             let t = this;
             return () => [new W({
                 key: new Y(t.extension),
                 props: {
                     handleDoubleClick: (i, s, o) => {
                         if (!(o.target instanceof HTMLElement) || o.button !== 0) return !1;
                         let l = wi(i.state, t.extension);
-                        if ((0, na.default)(l)) return !1;
+                        if ((0, ra.default)(l)) return !1;
                         let a = o.target.pmViewDesc;
                         return a && t.richtext.editor.chain().focus().setTextSelection({
                             from: a.posAtStart,
                             to: a.posAtEnd
                         }).run(), t.openPrefilledDialog(l), !0
                     }
                 }
@@ -13586,15 +13692,15 @@
         }
         async createPlugin() {
             if (!(this.element.nextElementSibling instanceof HTMLScriptElement) || this.element.nextElementSibling.type !== "text/plain") throw new Error(`Element ${this.element} requires a <script type="text/plain">\u2026<\/script>`);
             let t = this.element.nextElementSibling;
             try {
                 let r = t.getAttribute("tiptap-plugin"),
                     i = await fetch(t.src),
-                    s = Ql(await i.text(), {
+                    s = ea(await i.text(), {
                         startRule: "FunctionCode"
                     }),
                     l = new Function("mergeAttributes", "markPasteRule", `return ${s}`)(z, Ce);
                 switch (l.addProseMirrorPlugins = this.addProseMirrorPlugins(), r) {
                     case "mark":
                         return this.applyAttributes = this.applyMarkAttributes, this.revertAttributes = this.revertMarkAttributes, q.create(l);
                     case "node":
@@ -13606,15 +13712,15 @@
                 throw new Error(`Error while parsing <script type="text/plain" tiptap-plugin="${this.extension}"><\/script>: ${r}.`)
             }
         }
         isButtonActive(t, r) {
             var o;
             if (r !== "active") return !1;
             let i = (o = this.richtext.formDialogs.find(l => l.induceButton.name === t[0])) == null ? void 0 : o.induceButton;
-            return i instanceof HTMLButtonElement ? i === document.activeElement : this.closeButtons.find(l => (0, ra.default)(l.name, t[0])) === document.activeElement
+            return i instanceof HTMLButtonElement ? i === document.activeElement : this.closeButtons.find(l => (0, ia.default)(l.name, t[0])) === document.activeElement
         }
         openPrefilledDialog(t) {
             var r;
             if ((r = this.revertButton) == null || r.removeAttribute("hidden"), this.textSelectionField) {
                 let {
                     selection: i,
                     doc: s
@@ -13751,16 +13857,16 @@
                     this.editor = r, this.initialValue = this.getValue(), this.concealTextArea(this.wrapperElement), this.useJson && (this.textAreaElement.innerHTML = this.editor.getHTML()), this.contentUpdate(), this.installEventHandlers(), this.observer.observe(this.textAreaElement, {
                         attributes: !0
                     }), this.isInitialized = !0, t()
                 })
             })
         }
         async createEditor(e, t) {
-            let r = new Array(Nl, jl, Ul, Dl);
-            return this.registerControlActions(r), await this.registerFormDialogs(r), this.registerPlaceholder(r), this.registerCharaterCount(r), new Bn({
+            let r = new Array(Dl, Jl, _l, Il);
+            return this.registerControlActions(r), await this.registerFormDialogs(r), this.registerPlaceholder(r), this.registerCharaterCount(r), new Fn({
                 element: e,
                 extensions: r,
                 content: t,
                 autofocus: !1,
                 editable: !this.textAreaElement.disabled,
                 injectCSS: !1
             })
@@ -13795,23 +13901,23 @@
                 }), Promise.all(r).then(s => {
                     s.forEach(o => e.push(o)), t()
                 })
             })
         }
         registerPlaceholder(e) {
             let t = this.textAreaElement.getAttribute("placeholder");
-            t && e.push(Jl.configure({
+            t && e.push(ql.configure({
                 placeholder: t
             }))
         }
         registerCharaterCount(e) {
             let t = parseInt(this.textAreaElement.getAttribute("maxlength") ?? "");
-            t > 0 && (e.push(vl.configure({
+            t > 0 && (e.push(Ol.configure({
                 limit: t
-            })), this.characterCountTemplate = (0, ta.default)(`\${count}/${t}`), this.charaterCountDiv = document.createElement("div"), this.charaterCountDiv.classList.add("character-count"), this.wrapperElement.insertAdjacentElement("beforeend", this.charaterCountDiv))
+            })), this.characterCountTemplate = (0, na.default)(`\${count}/${t}`), this.charaterCountDiv = document.createElement("div"), this.charaterCountDiv.classList.add("character-count"), this.wrapperElement.insertAdjacentElement("beforeend", this.charaterCountDiv))
         }
         installEventHandlers() {
             this.editor.on("focus", this.focused), this.editor.on("update", this.updated), this.editor.on("blur", this.blurred), this.editor.on("update", this.contentUpdate), this.editor.on("selectionUpdate", this.selectionUpdate);
             let e = this.textAreaElement.form;
             e.addEventListener("reset", this.formResetted), e.addEventListener("submitted", this.formSubmitted), this.registeredActions.forEach(t => t.installEventHandler(this.editor))
         }
         concealTextArea(e) {
@@ -13867,15 +13973,15 @@
             return this.editor.isEmpty ? "" : this.useJson ? this.editor.getJSON() : this.editor.getHTML()
         }
         updateOperability(e) {
             this.formDialogs.forEach(t => t.updateOperability(e))
         }
     },
     ht = Symbol("RichtextArea"),
-    ea = class extends HTMLTextAreaElement {
+    ta = class extends HTMLTextAreaElement {
         constructor() {
             super();
             let e = this.closest(".dj-richtext-wrapper");
             if (!(e instanceof HTMLElement)) throw new Error(`${this} must be a child of '<ANY class="dj-richtext-wrapper">' element.`);
             this[ht] = new Li(e, this)
         }
         connectedCallback() {
@@ -13896,9 +14002,9 @@
         }
         updateOperability(e) {
             this[ht].updateOperability(e)
         }
     };
 ht;
 export {
-    ea as RichTextAreaElement
+    ta as RichTextAreaElement
 };
```

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-3KEXNODE.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-QHDAXJJP.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-65OJRBX6.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-65OJRBX6.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-EQH4AZSI.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-XQYS6DVW.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-FDUUONAQ.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-FDUUONAQ.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-INHB3J7K.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-CRVLB3K3.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,40 +1,40 @@
 import {
     a as Ve
 } from "./chunk-SERXULES.js";
 import {
-    a as it
+    a as rt
 } from "./chunk-FDUUONAQ.js";
 import {
     a as ie
 } from "./chunk-65OJRBX6.js";
 import {
-    a as Re,
-    b as ye,
+    a as $e,
+    b as Se,
     c as x
 } from "./chunk-P2VM2T3G.js";
-var Ke = Re((_e, $e) => {
+var je = $e((_e, Ke) => {
     (function(r, c) {
-        typeof _e == "object" && typeof $e < "u" ? c(_e) : typeof define == "function" && define.amd ? define(["exports"], c) : (r = typeof globalThis < "u" ? globalThis : r || self, c(r.sifter = {}))
+        typeof _e == "object" && typeof Ke < "u" ? c(_e) : typeof define == "function" && define.amd ? define(["exports"], c) : (r = typeof globalThis < "u" ? globalThis : r || self, c(r.sifter = {}))
     })(_e, function(r) {
         "use strict";
         let c = l => (l = l.filter(Boolean), l.length < 2 ? l[0] || "" : o(l) == 1 ? "[" + l.join("") + "]" : "(?:" + l.join("|") + ")"),
             e = l => {
                 if (!n(l)) return l.join("");
                 let a = "",
                     u = 0,
                     d = () => {
                         u > 1 && (a += "{" + u + "}")
                     };
-                return l.forEach((S, m) => {
-                    if (S === l[m - 1]) {
+                return l.forEach((_, v) => {
+                    if (_ === l[v - 1]) {
                         u++;
                         return
                     }
-                    d(), a += S, u = 1
+                    d(), a += _, u = 1
                 }), d(), a
             },
             t = l => {
                 let a = p(l);
                 return c(a)
             },
             n = l => new Set(l).size !== l.length,
@@ -44,20 +44,20 @@
             p = l => Array.from(l);
         let g = l => {
             if (l.length === 1) return [
                 [l]
             ];
             let a = [],
                 u = l.substring(1);
-            return g(u).forEach(function(S) {
-                let m = S.slice(0);
-                m[0] = l.charAt(0) + m[0], a.push(m), m = S.slice(0), m.unshift(l.charAt(0)), a.push(m)
+            return g(u).forEach(function(_) {
+                let v = _.slice(0);
+                v[0] = l.charAt(0) + v[0], a.push(v), v = _.slice(0), v.unshift(l.charAt(0)), a.push(v)
             }), a
         };
-        let v = [
+        let m = [
                 [0, 65535]
             ],
             M = "[\u0300-\u036F\xB7\u02BE\u02BC]",
             w, X, U = 3,
             h = {},
             Y = {
                 "/": "\u2044\u2215",
@@ -107,80 +107,80 @@
             for (let u = 0; u < a.length; u++) {
                 let d = a.substring(u, u + 1);
                 h[d] = l
             }
         }
         let k = new RegExp(Object.keys(h).join("|") + "|" + M, "gu"),
             N = l => {
-                w === void 0 && (w = A(l || v))
+                w === void 0 && (w = A(l || m))
             },
             b = (l, a = "NFKD") => l.normalize(a),
-            V = l => p(l).reduce((a, u) => a + W(u), ""),
+            $ = l => p(l).reduce((a, u) => a + W(u), ""),
             W = l => (l = b(l).toLowerCase().replace(k, a => h[a] || ""), b(l, "NFC"));
 
         function* oe(l) {
             for (let [a, u] of l)
                 for (let d = a; d <= u; d++) {
-                    let S = String.fromCharCode(d),
-                        m = V(S);
-                    m != S.toLowerCase() && (m.length > U || m.length != 0 && (yield {
-                        folded: m,
-                        composed: S,
+                    let _ = String.fromCharCode(d),
+                        v = $(_);
+                    v != _.toLowerCase() && (v.length > U || v.length != 0 && (yield {
+                        folded: v,
+                        composed: _,
                         code_point: d
                     }))
                 }
         }
-        let $ = l => {
+        let V = l => {
                 let a = {},
-                    u = (d, S) => {
-                        let m = a[d] || new Set,
-                            E = new RegExp("^" + t(m) + "$", "iu");
-                        S.match(E) || (m.add(s(S)), a[d] = m)
+                    u = (d, _) => {
+                        let v = a[d] || new Set,
+                            E = new RegExp("^" + t(v) + "$", "iu");
+                        _.match(E) || (v.add(s(_)), a[d] = v)
                     };
                 for (let d of oe(l)) u(d.folded, d.folded), u(d.folded, d.composed);
                 return a
             },
             A = l => {
-                let a = $(l),
+                let a = V(l),
                     u = {},
                     d = [];
-                for (let m in a) {
-                    let E = a[m];
-                    E && (u[m] = t(E)), m.length > 1 && d.push(s(m))
-                }
-                d.sort((m, E) => E.length - m.length);
-                let S = c(d);
-                return X = new RegExp("^" + S, "u"), u
+                for (let v in a) {
+                    let E = a[v];
+                    E && (u[v] = t(E)), v.length > 1 && d.push(s(v))
+                }
+                d.sort((v, E) => E.length - v.length);
+                let _ = c(d);
+                return X = new RegExp("^" + _, "u"), u
             },
             O = (l, a = 1) => {
                 let u = 0;
                 return l = l.map(d => (w[d] && (u += d.length), w[d] || d)), u >= a ? e(l) : ""
             },
             q = (l, a = 1) => (a = Math.max(a, l.length - 1), c(g(l).map(u => O(u, a)))),
             P = (l, a = !0) => {
                 let u = l.length > 1 ? 1 : 0;
                 return c(l.map(d => {
-                    let S = [],
-                        m = a ? d.length() : d.length() - 1;
-                    for (let E = 0; E < m; E++) S.push(q(d.substrs[E] || "", u));
-                    return e(S)
+                    let _ = [],
+                        v = a ? d.length() : d.length() - 1;
+                    for (let E = 0; E < v; E++) _.push(q(d.substrs[E] || "", u));
+                    return e(_)
                 }))
             },
             z = (l, a) => {
                 for (let u of a) {
                     if (u.start != l.start || u.end != l.end || u.substrs.join("") !== l.substrs.join("")) continue;
                     let d = l.parts,
-                        S = E => {
+                        _ = E => {
                             for (let F of d) {
                                 if (F.start === E.start && F.substr === E.substr) return !1;
                                 if (!(E.length == 1 || F.length == 1) && (E.start < F.start && E.end > F.start || F.start < E.start && F.end > E.start)) return !0
                             }
                             return !1
                         };
-                    if (!(u.parts.filter(S).length > 0)) return !0
+                    if (!(u.parts.filter(_).length > 0)) return !0
                 }
                 return !1
             };
         class se {
             constructor() {
                 this.parts = [], this.substrs = [], this.start = 0, this.end = 0
             }
@@ -191,35 +191,35 @@
                 return this.parts[this.parts.length - 1]
             }
             length() {
                 return this.parts.length
             }
             clone(a, u) {
                 let d = new se,
-                    S = JSON.parse(JSON.stringify(this.parts)),
-                    m = S.pop();
-                for (let G of S) d.add(G);
-                let E = u.substr.substring(0, a - m.start),
+                    _ = JSON.parse(JSON.stringify(this.parts)),
+                    v = _.pop();
+                for (let G of _) d.add(G);
+                let E = u.substr.substring(0, a - v.start),
                     F = E.length;
                 return d.add({
-                    start: m.start,
-                    end: m.start + F,
+                    start: v.start,
+                    end: v.start + F,
                     length: F,
                     substr: E
                 }), d
             }
         }
         let f = l => {
-                N(), l = V(l);
+                N(), l = $(l);
                 let a = "",
                     u = [new se];
                 for (let d = 0; d < l.length; d++) {
-                    let m = l.substring(d).match(X),
+                    let v = l.substring(d).match(X),
                         E = l.substring(d, d + 1),
-                        F = m ? m[0] : null,
+                        F = v ? v[0] : null,
                         G = [],
                         C = new Set;
                     for (let I of u) {
                         let H = I.last();
                         if (!H || H.length == 1 || H.end <= d)
                             if (F) {
                                 let J = F.length;
@@ -233,19 +233,19 @@
                                 start: d,
                                 end: d + 1,
                                 length: 1,
                                 substr: E
                             }), C.add("2");
                         else if (F) {
                             let J = I.clone(d, H),
-                                ue = F.length;
+                                de = F.length;
                             J.add({
                                 start: d,
-                                end: d + ue,
-                                length: ue,
+                                end: d + de,
+                                length: de,
                                 substr: F
                             }), G.push(J)
                         } else C.add("3")
                     }
                     if (G.length > 0) {
                         G = G.sort((I, H) => I.length() - H.length());
                         for (let I of G) z(I, u) || u.push(I);
@@ -256,88 +256,88 @@
                         let I = new se,
                             H = u[0];
                         H && I.add(H.last()), u = [I]
                     }
                 }
                 return a += P(u, !0), a
             },
-            _ = (l, a) => {
+            S = (l, a) => {
                 if (l) return l[a]
             },
             T = (l, a) => {
                 if (l) {
                     for (var u, d = a.split(".");
                         (u = d.shift()) && (l = l[u]););
                     return l
                 }
             },
             y = (l, a, u) => {
-                var d, S;
-                return !l || (l = l + "", a.regex == null) || (S = l.search(a.regex), S === -1) ? 0 : (d = a.string.length / l.length, S === 0 && (d += .5), d * u)
+                var d, _;
+                return !l || (l = l + "", a.regex == null) || (_ = l.search(a.regex), _ === -1) ? 0 : (d = a.string.length / l.length, _ === 0 && (d += .5), d * u)
             },
             R = (l, a) => {
                 var u = l[a];
                 if (typeof u == "function") return u;
                 u && !Array.isArray(u) && (l[a] = [u])
             },
             L = (l, a) => {
                 if (Array.isArray(l)) l.forEach(a);
                 else
                     for (var u in l) l.hasOwnProperty(u) && a(l[u], u)
             },
-            K = (l, a) => typeof l == "number" && typeof a == "number" ? l > a ? 1 : l < a ? -1 : 0 : (l = V(l + "").toLowerCase(), a = V(a + "").toLowerCase(), l > a ? 1 : a > l ? -1 : 0);
+            K = (l, a) => typeof l == "number" && typeof a == "number" ? l > a ? 1 : l < a ? -1 : 0 : (l = $(l + "").toLowerCase(), a = $(a + "").toLowerCase(), l > a ? 1 : a > l ? -1 : 0);
         class B {
             constructor(a, u) {
                 this.items = void 0, this.settings = void 0, this.items = a, this.settings = u || {
                     diacritics: !0
                 }
             }
             tokenize(a, u, d) {
                 if (!a || !a.length) return [];
-                let S = [],
-                    m = a.split(/\s+/);
+                let _ = [],
+                    v = a.split(/\s+/);
                 var E;
-                return d && (E = new RegExp("^(" + Object.keys(d).map(s).join("|") + "):(.*)$")), m.forEach(F => {
+                return d && (E = new RegExp("^(" + Object.keys(d).map(s).join("|") + "):(.*)$")), v.forEach(F => {
                     let G, C = null,
                         I = null;
-                    E && (G = F.match(E)) && (C = G[1], F = G[2]), F.length > 0 && (this.settings.diacritics ? I = f(F) || null : I = s(F), I && u && (I = "\\b" + I)), S.push({
+                    E && (G = F.match(E)) && (C = G[1], F = G[2]), F.length > 0 && (this.settings.diacritics ? I = f(F) || null : I = s(F), I && u && (I = "\\b" + I)), _.push({
                         string: F,
                         regex: I ? new RegExp(I, "iu") : null,
                         field: C
                     })
-                }), S
+                }), _
             }
             getScoreFunction(a, u) {
                 var d = this.prepareSearch(a, u);
                 return this._getScoreFunction(d)
             }
             _getScoreFunction(a) {
                 let u = a.tokens,
                     d = u.length;
                 if (!d) return function() {
                     return 0
                 };
-                let S = a.options.fields,
-                    m = a.weights,
-                    E = S.length,
+                let _ = a.options.fields,
+                    v = a.weights,
+                    E = _.length,
                     F = a.getAttrFn;
                 if (!E) return function() {
                     return 1
                 };
                 let G = function() {
                     return E === 1 ? function(C, I) {
-                        let H = S[0].field;
-                        return y(F(I, H), C, m[H] || 1)
+                        let H = _[0].field;
+                        return y(F(I, H), C, v[H] || 1)
                     } : function(C, I) {
                         var H = 0;
                         if (C.field) {
                             let J = F(I, C.field);
                             !C.regex && J ? H += 1 / E : H += y(J, C, 1)
-                        } else L(m, (J, ue) => {
-                            H += y(F(I, ue), C, J)
+                        } else L(v, (J, de) => {
+                            H += y(F(I, de), C, J)
                         });
                         return H / E
                     }
                 }();
                 return d === 1 ? function(C) {
                     return G(u[0], C)
                 } : a.options.conjunction === "and" ? function(C) {
@@ -356,20 +356,20 @@
             }
             getSortFunction(a, u) {
                 var d = this.prepareSearch(a, u);
                 return this._getSortFunction(d)
             }
             _getSortFunction(a) {
                 var u, d = [];
-                let S = this,
-                    m = a.options,
-                    E = !a.query && m.sort_empty ? m.sort_empty : m.sort;
+                let _ = this,
+                    v = a.options,
+                    E = !a.query && v.sort_empty ? v.sort_empty : v.sort;
                 if (typeof E == "function") return E.bind(this);
                 let F = function(I, H) {
-                    return I === "$score" ? H.score : a.getAttrFn(S.items[H.id], I)
+                    return I === "$score" ? H.score : a.getAttrFn(_.items[H.id], I)
                 };
                 if (E)
                     for (let C of E)(a.query || C.field !== "$score") && d.push(C);
                 if (a.query) {
                     u = !0;
                     for (let C of d)
                         if (C.field === "$score") {
@@ -378,109 +378,109 @@
                         } u && d.unshift({
                         field: "$score",
                         direction: "desc"
                     })
                 } else d = d.filter(C => C.field !== "$score");
                 return d.length ? function(C, I) {
                     var H, J;
-                    for (let ue of d)
-                        if (J = ue.field, H = (ue.direction === "desc" ? -1 : 1) * K(F(J, C), F(J, I)), H) return H;
+                    for (let de of d)
+                        if (J = de.field, H = (de.direction === "desc" ? -1 : 1) * K(F(J, C), F(J, I)), H) return H;
                     return 0
                 } : null
             }
             prepareSearch(a, u) {
                 let d = {};
-                var S = Object.assign({}, u);
-                if (R(S, "sort"), R(S, "sort_empty"), S.fields) {
-                    R(S, "fields");
-                    let m = [];
-                    S.fields.forEach(E => {
+                var _ = Object.assign({}, u);
+                if (R(_, "sort"), R(_, "sort_empty"), _.fields) {
+                    R(_, "fields");
+                    let v = [];
+                    _.fields.forEach(E => {
                         typeof E == "string" && (E = {
                             field: E,
                             weight: 1
-                        }), m.push(E), d[E.field] = "weight" in E ? E.weight : 1
-                    }), S.fields = m
+                        }), v.push(E), d[E.field] = "weight" in E ? E.weight : 1
+                    }), _.fields = v
                 }
                 return {
-                    options: S,
+                    options: _,
                     query: a.toLowerCase().trim(),
-                    tokens: this.tokenize(a, S.respect_word_boundaries, d),
+                    tokens: this.tokenize(a, _.respect_word_boundaries, d),
                     total: 0,
                     items: [],
                     weights: d,
-                    getAttrFn: S.nesting ? T : _
+                    getAttrFn: _.nesting ? T : S
                 }
             }
             search(a, u) {
                 var d = this,
-                    S, m;
-                m = this.prepareSearch(a, u), u = m.options, a = m.query;
-                let E = u.score || d._getScoreFunction(m);
+                    _, v;
+                v = this.prepareSearch(a, u), u = v.options, a = v.query;
+                let E = u.score || d._getScoreFunction(v);
                 a.length ? L(d.items, (G, C) => {
-                    S = E(G), (u.filter === !1 || S > 0) && m.items.push({
-                        score: S,
+                    _ = E(G), (u.filter === !1 || _ > 0) && v.items.push({
+                        score: _,
                         id: C
                     })
                 }) : L(d.items, (G, C) => {
-                    m.items.push({
+                    v.items.push({
                         score: 1,
                         id: C
                     })
                 });
-                let F = d._getSortFunction(m);
-                return F && m.items.sort(F), m.total = m.items.length, typeof u.limit == "number" && (m.items = m.items.slice(0, u.limit)), m
+                let F = d._getSortFunction(v);
+                return F && v.items.sort(F), v.total = v.items.length, typeof u.limit == "number" && (v.items = v.items.slice(0, u.limit)), v
             }
         }
-        r.Sifter = B, r.cmp = K, r.getAttr = _, r.getAttrNesting = T, r.getPattern = f, r.iterate = L, r.propToArray = R, r.scoreValue = y, Object.defineProperty(r, "__esModule", {
+        r.Sifter = B, r.cmp = K, r.getAttr = S, r.getAttrNesting = T, r.getPattern = f, r.iterate = L, r.propToArray = R, r.scoreValue = y, Object.defineProperty(r, "__esModule", {
             value: !0
         })
     })
 });
-var Ie = Re((Se, je) => {
+var Ae = $e((Te, De) => {
     (function(r, c) {
-        typeof Se == "object" && typeof je < "u" ? c(Se) : typeof define == "function" && define.amd ? define(["exports"], c) : (r = typeof globalThis < "u" ? globalThis : r || self, c(r.diacritics = {}))
-    })(Se, function(r) {
+        typeof Te == "object" && typeof De < "u" ? c(Te) : typeof define == "function" && define.amd ? define(["exports"], c) : (r = typeof globalThis < "u" ? globalThis : r || self, c(r.diacritics = {}))
+    })(Te, function(r) {
         "use strict";
         let c = f => (f = f.filter(Boolean), f.length < 2 ? f[0] || "" : o(f) == 1 ? "[" + f.join("") + "]" : "(?:" + f.join("|") + ")"),
             e = f => {
                 if (!n(f)) return f.join("");
-                let _ = "",
+                let S = "",
                     T = 0,
                     y = () => {
-                        T > 1 && (_ += "{" + T + "}")
+                        T > 1 && (S += "{" + T + "}")
                     };
                 return f.forEach((R, L) => {
                     if (R === f[L - 1]) {
                         T++;
                         return
                     }
-                    y(), _ += R, T = 1
-                }), y(), _
+                    y(), S += R, T = 1
+                }), y(), S
             },
             t = f => {
-                let _ = p(f);
-                return c(_)
+                let S = p(f);
+                return c(S)
             },
             n = f => new Set(f).size !== f.length,
             s = f => (f + "").replace(/([\$\(\)\*\+\.\?\[\]\^\{\|\}\\])/gu, "\\$1"),
-            o = f => f.reduce((_, T) => Math.max(_, i(T)), 0),
+            o = f => f.reduce((S, T) => Math.max(S, i(T)), 0),
             i = f => p(f).length,
             p = f => Array.from(f),
             g = f => {
                 if (f.length === 1) return [
                     [f]
                 ];
-                let _ = [],
+                let S = [],
                     T = f.substring(1);
                 return g(T).forEach(function(R) {
                     let L = R.slice(0);
-                    L[0] = f.charAt(0) + L[0], _.push(L), L = R.slice(0), L.unshift(f.charAt(0)), _.push(L)
-                }), _
+                    L[0] = f.charAt(0) + L[0], S.push(L), L = R.slice(0), L.unshift(f.charAt(0)), S.push(L)
+                }), S
             },
-            v = [
+            m = [
                 [0, 65535]
             ],
             M = "[\u0300-\u036F\xB7\u02BE\u02BC]";
         r.unicode_map = void 0;
         let w, X = 3,
             U = {},
             h = {
@@ -523,78 +523,78 @@
                 vy: "\uA761",
                 w: "\u2C73",
                 y: "\u01B4\u024F\u1EFF",
                 z: "\u01B6\u0225\u0240\u2C6C\uA763",
                 hv: "\u0195"
             };
         for (let f in h) {
-            let _ = h[f] || "";
-            for (let T = 0; T < _.length; T++) {
-                let y = _.substring(T, T + 1);
+            let S = h[f] || "";
+            for (let T = 0; T < S.length; T++) {
+                let y = S.substring(T, T + 1);
                 U[y] = f
             }
         }
         let Y = new RegExp(Object.keys(U).join("|") + "|" + M, "gu"),
             k = f => {
-                r.unicode_map === void 0 && (r.unicode_map = $(f || v))
+                r.unicode_map === void 0 && (r.unicode_map = V(f || m))
             },
-            N = (f, _ = "NFKD") => f.normalize(_),
-            b = f => p(f).reduce((_, T) => _ + V(T), ""),
-            V = f => (f = N(f).toLowerCase().replace(Y, _ => U[_] || ""), N(f, "NFC"));
+            N = (f, S = "NFKD") => f.normalize(S),
+            b = f => p(f).reduce((S, T) => S + $(T), ""),
+            $ = f => (f = N(f).toLowerCase().replace(Y, S => U[S] || ""), N(f, "NFC"));
 
         function* W(f) {
-            for (let [_, T] of f)
-                for (let y = _; y <= T; y++) {
+            for (let [S, T] of f)
+                for (let y = S; y <= T; y++) {
                     let R = String.fromCharCode(y),
                         L = b(R);
                     L != R.toLowerCase() && (L.length > X || L.length != 0 && (yield {
                         folded: L,
                         composed: R,
                         code_point: y
                     }))
                 }
         }
         let oe = f => {
-                let _ = {},
+                let S = {},
                     T = (y, R) => {
-                        let L = _[y] || new Set,
+                        let L = S[y] || new Set,
                             K = new RegExp("^" + t(L) + "$", "iu");
-                        R.match(K) || (L.add(s(R)), _[y] = L)
+                        R.match(K) || (L.add(s(R)), S[y] = L)
                     };
                 for (let y of W(f)) T(y.folded, y.folded), T(y.folded, y.composed);
-                return _
+                return S
             },
-            $ = f => {
-                let _ = oe(f),
+            V = f => {
+                let S = oe(f),
                     T = {},
                     y = [];
-                for (let L in _) {
-                    let K = _[L];
+                for (let L in S) {
+                    let K = S[L];
                     K && (T[L] = t(K)), L.length > 1 && y.push(s(L))
                 }
                 y.sort((L, K) => K.length - L.length);
                 let R = c(y);
                 return w = new RegExp("^" + R, "u"), T
             },
-            A = (f, _ = 1) => {
+            A = (f, S = 1) => {
                 let T = 0;
-                return f = f.map(y => (r.unicode_map[y] && (T += y.length), r.unicode_map[y] || y)), T >= _ ? e(f) : ""
+                return f = f.map(y => (r.unicode_map[y] && (T += y.length), r.unicode_map[y] || y)), T >= S ? e(f) : ""
             },
-            O = (f, _ = 1) => (_ = Math.max(_, f.length - 1), c(g(f).map(T => A(T, _)))),
-            q = (f, _ = !0) => {
+            O = (f, S = 1) => (S = Math.max(S, f.length - 1), c(g(f).map(T => A(T, S)))),
+            q = (f, S = !0) => {
                 let T = f.length > 1 ? 1 : 0;
                 return c(f.map(y => {
                     let R = [],
-                        L = _ ? y.length() : y.length() - 1;
+                        L = S ? y.length() : y.length() - 1;
                     for (let K = 0; K < L; K++) R.push(O(y.substrs[K] || "", T));
                     return e(R)
                 }))
             },
-            P = (f, _) => {
-                for (let T of _) {
+            P = (f, S) => {
+                for (let T of S) {
                     if (T.start != f.start || T.end != f.end || T.substrs.join("") !== f.substrs.join("")) continue;
                     let y = f.parts,
                         R = K => {
                             for (let B of y) {
                                 if (B.start === K.start && B.substr === K.substr) return !1;
                                 if (!(K.length == 1 || B.length == 1) && (K.start < B.start && K.end > B.start || B.start < K.start && B.end > K.start)) return !0
                             }
@@ -604,139 +604,139 @@
                 }
                 return !1
             };
         class z {
             constructor() {
                 this.parts = [], this.substrs = [], this.start = 0, this.end = 0
             }
-            add(_) {
-                _ && (this.parts.push(_), this.substrs.push(_.substr), this.start = Math.min(_.start, this.start), this.end = Math.max(_.end, this.end))
+            add(S) {
+                S && (this.parts.push(S), this.substrs.push(S.substr), this.start = Math.min(S.start, this.start), this.end = Math.max(S.end, this.end))
             }
             last() {
                 return this.parts[this.parts.length - 1]
             }
             length() {
                 return this.parts.length
             }
-            clone(_, T) {
+            clone(S, T) {
                 let y = new z,
                     R = JSON.parse(JSON.stringify(this.parts)),
                     L = R.pop();
                 for (let l of R) y.add(l);
-                let K = T.substr.substring(0, _ - L.start),
+                let K = T.substr.substring(0, S - L.start),
                     B = K.length;
                 return y.add({
                     start: L.start,
                     end: L.start + B,
                     length: B,
                     substr: K
                 }), y
             }
         }
         let se = f => {
             k(), f = b(f);
-            let _ = "",
+            let S = "",
                 T = [new z];
             for (let y = 0; y < f.length; y++) {
                 let L = f.substring(y).match(w),
                     K = f.substring(y, y + 1),
                     B = L ? L[0] : null,
                     l = [],
                     a = new Set;
                 for (let u of T) {
                     let d = u.last();
                     if (!d || d.length == 1 || d.end <= y)
                         if (B) {
-                            let S = B.length;
+                            let _ = B.length;
                             u.add({
                                 start: y,
-                                end: y + S,
-                                length: S,
+                                end: y + _,
+                                length: _,
                                 substr: B
                             }), a.add("1")
                         } else u.add({
                             start: y,
                             end: y + 1,
                             length: 1,
                             substr: K
                         }), a.add("2");
                     else if (B) {
-                        let S = u.clone(y, d),
-                            m = B.length;
-                        S.add({
+                        let _ = u.clone(y, d),
+                            v = B.length;
+                        _.add({
                             start: y,
-                            end: y + m,
-                            length: m,
+                            end: y + v,
+                            length: v,
                             substr: B
-                        }), l.push(S)
+                        }), l.push(_)
                     } else a.add("3")
                 }
                 if (l.length > 0) {
                     l = l.sort((u, d) => u.length() - d.length());
                     for (let u of l) P(u, T) || T.push(u);
                     continue
                 }
                 if (y > 0 && a.size == 1 && !a.has("3")) {
-                    _ += q(T, !1);
+                    S += q(T, !1);
                     let u = new z,
                         d = T[0];
                     d && u.add(d.last()), T = [u]
                 }
             }
-            return _ += q(T, !0), _
+            return S += q(T, !0), S
         };
-        r._asciifold = V, r.asciifold = b, r.code_points = v, r.escape_regex = s, r.generateMap = $, r.generateSets = oe, r.generator = W, r.getPattern = se, r.initialize = k, r.mapSequence = A, r.normalize = N, r.substringsToPattern = O, Object.defineProperty(r, "__esModule", {
+        r._asciifold = $, r.asciifold = b, r.code_points = m, r.escape_regex = s, r.generateMap = V, r.generateSets = oe, r.generator = W, r.getPattern = se, r.initialize = k, r.mapSequence = A, r.normalize = N, r.substringsToPattern = O, Object.defineProperty(r, "__esModule", {
             value: !0
         })
     })
 });
 
-function xe(r, c) {
+function Le(r, c) {
     r.split(/\s+/).forEach(e => {
         c(e)
     })
 }
-var he = class {
+var ge = class {
     constructor() {
         x(this, "_events");
         this._events = {}
     }
     on(c, e) {
-        xe(c, t => {
+        Le(c, t => {
             let n = this._events[t] || [];
             n.push(e), this._events[t] = n
         })
     }
     off(c, e) {
         var t = arguments.length;
         if (t === 0) {
             this._events = {};
             return
         }
-        xe(c, n => {
+        Le(c, n => {
             if (t === 1) {
                 delete this._events[n];
                 return
             }
             let s = this._events[n];
             s !== void 0 && (s.splice(s.indexOf(e), 1), this._events[n] = s)
         })
     }
     trigger(c, ...e) {
         var t = this;
-        xe(c, n => {
+        Le(c, n => {
             let s = t._events[n];
             s !== void 0 && s.forEach(o => {
                 o.apply(t, e)
             })
         })
     }
 };
 
-function Le(r) {
+function Ie(r) {
     return r.plugins = {}, class extends r {
         constructor() {
             super(...arguments);
             x(this, "plugins", {
                 names: [],
                 settings: {},
                 requested: {},
@@ -774,122 +774,122 @@
                 if (n.requested[e]) throw new Error('Plugin has circular dependency ("' + e + '")');
                 t.loadPlugin(e)
             }
             return n.loaded[e]
         }
     }
 }
-var te = ye(Ke()),
-    Ze = ye(Ie());
-var rt = ye(Ie());
+var te = Se(je()),
+    et = Se(Ae());
+var ot = Se(Ae());
 var le = (r, c) => {
     if (Array.isArray(r)) r.forEach(c);
     else
         for (var e in r) r.hasOwnProperty(e) && c(r[e], e)
 };
 var Z = r => {
         if (r.jquery) return r[0];
         if (r instanceof HTMLElement) return r;
-        if (Ae(r)) {
+        if (Ce(r)) {
             var c = document.createElement("template");
             return c.innerHTML = r.trim(), c.content.firstChild
         }
         return document.querySelector(r)
     },
-    Ae = r => typeof r == "string" && r.indexOf("<") > -1,
-    De = r => r.replace(/['"\\]/g, "\\$&"),
-    Te = (r, c) => {
+    Ce = r => typeof r == "string" && r.indexOf("<") > -1,
+    Ne = r => r.replace(/['"\\]/g, "\\$&"),
+    we = (r, c) => {
         var e = document.createEvent("HTMLEvents");
         e.initEvent(c, !0, !1), r.dispatchEvent(e)
     },
-    ge = (r, c) => {
+    me = (r, c) => {
         Object.assign(r.style, c)
     },
     ee = (r, ...c) => {
-        var e = Ne(c);
-        r = qe(r), r.map(t => {
+        var e = qe(c);
+        r = ze(r), r.map(t => {
             e.map(n => {
                 t.classList.add(n)
             })
         })
     },
     re = (r, ...c) => {
-        var e = Ne(c);
-        r = qe(r), r.map(t => {
+        var e = qe(c);
+        r = ze(r), r.map(t => {
             e.map(n => {
                 t.classList.remove(n)
             })
         })
     },
-    Ne = r => {
+    qe = r => {
         var c = [];
         return le(r, e => {
             typeof e == "string" && (e = e.trim().split(/[\11\12\14\15\40]/)), Array.isArray(e) && (c = c.concat(e))
         }), c.filter(Boolean)
     },
-    qe = r => (Array.isArray(r) || (r = [r]), r),
-    we = (r, c, e) => {
+    ze = r => (Array.isArray(r) || (r = [r]), r),
+    Oe = (r, c, e) => {
         if (!(e && !e.contains(r)))
             for (; r && r.matches;) {
                 if (r.matches(c)) return r;
                 r = r.parentNode
             }
     },
-    Ce = (r, c = 0) => c > 0 ? r[r.length - 1] : r[0],
-    ze = r => Object.keys(r).length === 0,
-    Me = (r, c) => {
+    Me = (r, c = 0) => c > 0 ? r[r.length - 1] : r[0],
+    Ye = r => Object.keys(r).length === 0,
+    Fe = (r, c) => {
         if (!r) return -1;
         c = c || r.nodeName;
         for (var e = 0; r = r.previousElementSibling;) r.matches(c) && e++;
         return e
     },
     D = (r, c) => {
         le(c, (e, t) => {
             e == null ? r.removeAttribute(t) : r.setAttribute(t, "" + e)
         })
     },
-    me = (r, c) => {
+    ve = (r, c) => {
         r.parentNode && r.parentNode.replaceChild(c, r)
     };
-var Ye = (r, c) => {
+var Be = (r, c) => {
         if (c === null) return;
         if (typeof c == "string") {
             if (!c.length) return;
             c = new RegExp(c, "i")
         }
         let e = s => {
                 var o = s.data.match(c);
                 if (o && s.data.length > 0) {
                     var i = document.createElement("span");
                     i.className = "highlight";
                     var p = s.splitText(o.index);
                     p.splitText(o[0].length);
                     var g = p.cloneNode(!0);
-                    return i.appendChild(g), me(p, i), 1
+                    return i.appendChild(g), ve(p, i), 1
                 }
                 return 0
             },
             t = s => {
                 s.nodeType === 1 && s.childNodes && !/(script|style)/i.test(s.tagName) && (s.className !== "highlight" || s.tagName !== "SPAN") && Array.from(s.childNodes).forEach(o => {
                     n(o)
                 })
             },
             n = s => s.nodeType === 3 ? e(s) : (t(s), 0);
         n(r)
     },
-    Be = r => {
+    Ge = r => {
         var c = r.querySelectorAll("span.highlight");
         Array.prototype.forEach.call(c, function(e) {
             var t = e.parentNode;
             t.replaceChild(e.firstChild, e), t.normalize()
         })
     };
-var ot = typeof navigator > "u" ? !1 : /Mac/.test(navigator.userAgent),
-    ve = ot ? "metaKey" : "ctrlKey";
-var Fe = {
+var lt = typeof navigator > "u" ? !1 : /Mac/.test(navigator.userAgent),
+    be = lt ? "metaKey" : "ctrlKey";
+var He = {
     options: [],
     optgroups: [],
     plugins: [],
     delimiter: ",",
     splitOn: null,
     persist: !0,
     diacritics: !0,
@@ -934,71 +934,71 @@
     placeholder: null,
     hidePlaceholder: null,
     shouldLoad: function(r) {
         return r.length > 0
     },
     render: {}
 };
-var ne = r => typeof r > "u" || r === null ? null : be(r),
-    be = r => typeof r == "boolean" ? r ? "1" : "0" : r + "",
-    de = r => (r + "").replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;"),
-    Ge = (r, c) => c > 0 ? setTimeout(r, c) : (r.call(null), null),
-    Qe = (r, c) => {
+var ne = r => typeof r > "u" || r === null ? null : ye(r),
+    ye = r => typeof r == "boolean" ? r ? "1" : "0" : r + "",
+    pe = r => (r + "").replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;"),
+    Qe = (r, c) => c > 0 ? setTimeout(r, c) : (r.call(null), null),
+    Ue = (r, c) => {
         var e;
         return function(t, n) {
             var s = this;
             e && (s.loading = Math.max(s.loading - 1, 0), clearTimeout(e)), e = setTimeout(function() {
                 e = null, s.loadedSearches[t] = !0, r.call(s, t, n)
             }, c)
         }
     },
-    He = (r, c, e) => {
+    ke = (r, c, e) => {
         var t, n = r.trigger,
             s = {};
         r.trigger = function() {
             var o = arguments[0];
             if (c.indexOf(o) !== -1) s[o] = arguments;
             else return n.apply(r, arguments)
         }, e.apply(r, []), r.trigger = n;
         for (t of c) t in s && n.apply(r, s[t])
     },
-    Ue = r => ({
+    Je = r => ({
         start: r.selectionStart || 0,
         length: (r.selectionEnd || 0) - (r.selectionStart || 0)
     }),
     j = (r, c = !1) => {
         r && (r.preventDefault(), c && r.stopPropagation())
     },
     Q = (r, c, e, t) => {
         r.addEventListener(c, e, t)
     },
     ae = (r, c) => {
         if (!c || !c[r]) return !1;
         var e = (c.altKey ? 1 : 0) + (c.ctrlKey ? 1 : 0) + (c.shiftKey ? 1 : 0) + (c.metaKey ? 1 : 0);
         return e === 1
     },
-    Oe = (r, c) => {
+    Ee = (r, c) => {
         let e = r.getAttribute("id");
         return e || (r.setAttribute("id", c), c)
     },
-    ke = r => r.replace(/[\\"']/g, "\\$&"),
+    Pe = r => r.replace(/[\\"']/g, "\\$&"),
     ce = (r, c) => {
         c && r.append(c)
     };
 
-function Ee(r, c) {
-    var e = Object.assign({}, Fe, c),
+function xe(r, c) {
+    var e = Object.assign({}, He, c),
         t = e.dataAttr,
         n = e.labelField,
         s = e.valueField,
         o = e.disabledField,
         i = e.optgroupField,
         p = e.optgroupLabelField,
         g = e.optgroupValueField,
-        v = r.tagName.toLowerCase(),
+        m = r.tagName.toLowerCase(),
         M = r.getAttribute("placeholder") || r.getAttribute("data-placeholder");
     if (!M && !e.allowEmptyOption) {
         let h = r.querySelector('option[value=""]');
         h && (M = h.textContent)
     }
     var w = {
             placeholder: M,
@@ -1008,42 +1008,42 @@
             maxItems: null
         },
         X = () => {
             var h, Y = w.options,
                 k = {},
                 N = 1;
             let b = 0;
-            var V = $ => {
-                    var A = Object.assign({}, $.dataset),
+            var $ = V => {
+                    var A = Object.assign({}, V.dataset),
                         O = t && A[t];
                     return typeof O == "string" && O.length && (A = Object.assign(A, JSON.parse(O))), A
                 },
-                W = ($, A) => {
-                    var O = ne($.value);
+                W = (V, A) => {
+                    var O = ne(V.value);
                     if (O != null && !(!O && !e.allowEmptyOption)) {
                         if (k.hasOwnProperty(O)) {
                             if (A) {
                                 var q = k[O][i];
                                 q ? Array.isArray(q) ? q.push(A) : k[O][i] = [q, A] : k[O][i] = A
                             }
                         } else {
-                            var P = V($);
-                            P[n] = P[n] || $.textContent, P[s] = P[s] || O, P[o] = P[o] || $.disabled, P[i] = P[i] || A, P.$option = $, P.$order = P.$order || ++b, k[O] = P, Y.push(P)
+                            var P = $(V);
+                            P[n] = P[n] || V.textContent, P[s] = P[s] || O, P[o] = P[o] || V.disabled, P[i] = P[i] || A, P.$option = V, P.$order = P.$order || ++b, k[O] = P, Y.push(P)
                         }
-                        $.selected && w.items.push(O)
+                        V.selected && w.items.push(O)
                     }
                 },
-                oe = $ => {
+                oe = V => {
                     var A, O;
-                    O = V($), O[p] = O[p] || $.getAttribute("label") || "", O[g] = O[g] || N++, O[o] = O[o] || $.disabled, O.$order = O.$order || ++b, w.optgroups.push(O), A = O[g], le($.children, q => {
+                    O = $(V), O[p] = O[p] || V.getAttribute("label") || "", O[g] = O[g] || N++, O[o] = O[o] || V.disabled, O.$order = O.$order || ++b, w.optgroups.push(O), A = O[g], le(V.children, q => {
                         W(q, A)
                     })
                 };
-            w.maxItems = r.hasAttribute("multiple") ? null : 1, le(r.children, $ => {
-                h = $.tagName.toLowerCase(), h === "optgroup" ? oe($) : h === "option" && W($)
+            w.maxItems = r.hasAttribute("multiple") ? null : 1, le(r.children, V => {
+                h = V.tagName.toLowerCase(), h === "optgroup" ? oe(V) : h === "option" && W(V)
             })
         },
         U = () => {
             let h = r.getAttribute(t);
             if (h) w.options = JSON.parse(h), le(w.options, k => {
                 w.items.push(k[s])
             });
@@ -1053,18 +1053,18 @@
                 let k = Y.split(e.delimiter);
                 le(k, N => {
                     let b = {};
                     b[n] = N, b[s] = N, w.options.push(b)
                 }), w.items = k
             }
         };
-    return v === "select" ? X() : U(), Object.assign({}, Fe, w, c)
+    return m === "select" ? X() : U(), Object.assign({}, He, w, c)
 }
-var Xe = 0,
-    pe = class extends Le(he) {
+var Ze = 0,
+    fe = class extends Ie(ge) {
         constructor(e, t) {
             super();
             x(this, "control_input");
             x(this, "wrapper");
             x(this, "dropdown");
             x(this, "control");
             x(this, "dropdown_content");
@@ -1099,113 +1099,113 @@
             x(this, "activeOption", null);
             x(this, "activeItems", []);
             x(this, "optgroups", {});
             x(this, "options", {});
             x(this, "userOptions", {});
             x(this, "items", []);
             x(this, "refreshTimeout", null);
-            Xe++;
+            Ze++;
             var n, s = Z(e);
             if (s.tomselect) throw new Error("Tom Select already initialized on this element");
             s.tomselect = this;
             var o = window.getComputedStyle && window.getComputedStyle(s, null);
             n = o.getPropertyValue("direction");
-            let i = Ee(s, t);
-            this.settings = i, this.input = s, this.tabIndex = s.tabIndex || 0, this.is_select_tag = s.tagName.toLowerCase() === "select", this.rtl = /rtl/i.test(n), this.inputId = Oe(s, "tomselect-" + Xe), this.isRequired = s.required, this.sifter = new te.Sifter(this.options, {
+            let i = xe(s, t);
+            this.settings = i, this.input = s, this.tabIndex = s.tabIndex || 0, this.is_select_tag = s.tagName.toLowerCase() === "select", this.rtl = /rtl/i.test(n), this.inputId = Ee(s, "tomselect-" + Ze), this.isRequired = s.required, this.sifter = new te.Sifter(this.options, {
                 diacritics: i.diacritics
             }), i.mode = i.mode || (i.maxItems === 1 ? "single" : "multi"), typeof i.hideSelected != "boolean" && (i.hideSelected = i.mode === "multi"), typeof i.hidePlaceholder != "boolean" && (i.hidePlaceholder = i.mode !== "multi");
             var p = i.createFilter;
             typeof p != "function" && (typeof p == "string" && (p = new RegExp(p)), p instanceof RegExp ? i.createFilter = k => p.test(k) : i.createFilter = k => this.settings.duplicates || !this.options[k]), this.initializePlugins(i.plugins), this.setupCallbacks(), this.setupTemplates();
             let g = Z("<div>"),
-                v = Z("<div>"),
+                m = Z("<div>"),
                 M = this._render("dropdown"),
                 w = Z('<div role="listbox" tabindex="-1">'),
                 X = this.input.getAttribute("class") || "",
                 U = i.mode;
             var h;
-            if (ee(g, i.wrapperClass, X, U), ee(v, i.controlClass), ce(g, v), ee(M, i.dropdownClass, U), i.copyClassesToDropdown && ee(M, X), ee(w, i.dropdownContentClass), ce(M, w), Z(i.dropdownParent || g).appendChild(M), Ae(i.controlInput)) {
+            if (ee(g, i.wrapperClass, X, U), ee(m, i.controlClass), ce(g, m), ee(M, i.dropdownClass, U), i.copyClassesToDropdown && ee(M, X), ee(w, i.dropdownContentClass), ce(M, w), Z(i.dropdownParent || g).appendChild(M), Ce(i.controlInput)) {
                 h = Z(i.controlInput);
                 var Y = ["autocorrect", "autocapitalize", "autocomplete", "spellcheck"];
                 (0, te.iterate)(Y, k => {
                     s.getAttribute(k) && D(h, {
                         [k]: s.getAttribute(k)
                     })
-                }), h.tabIndex = -1, v.appendChild(h), this.focus_node = h
-            } else i.controlInput ? (h = Z(i.controlInput), this.focus_node = h) : (h = Z("<input/>"), this.focus_node = v);
-            this.wrapper = g, this.dropdown = M, this.dropdown_content = w, this.control = v, this.control_input = h, this.setup()
+                }), h.tabIndex = -1, m.appendChild(h), this.focus_node = h
+            } else i.controlInput ? (h = Z(i.controlInput), this.focus_node = h) : (h = Z("<input/>"), this.focus_node = m);
+            this.wrapper = g, this.dropdown = M, this.dropdown_content = w, this.control = m, this.control_input = h, this.setup()
         }
         setup() {
             let e = this,
                 t = e.settings,
                 n = e.control_input,
                 s = e.dropdown,
                 o = e.dropdown_content,
                 i = e.wrapper,
                 p = e.control,
                 g = e.input,
-                v = e.focus_node,
+                m = e.focus_node,
                 M = {
                     passive: !0
                 },
                 w = e.inputId + "-ts-dropdown";
             D(o, {
                 id: w
-            }), D(v, {
+            }), D(m, {
                 role: "combobox",
                 "aria-haspopup": "listbox",
                 "aria-expanded": "false",
                 "aria-controls": w
             });
-            let X = Oe(v, e.inputId + "-ts-control"),
-                U = "label[for='" + De(e.inputId) + "']",
+            let X = Ee(m, e.inputId + "-ts-control"),
+                U = "label[for='" + Ne(e.inputId) + "']",
                 h = document.querySelector(U),
                 Y = e.focus.bind(e);
             if (h) {
                 Q(h, "click", Y), D(h, {
                     for: X
                 });
-                let b = Oe(h, e.inputId + "-ts-label");
-                D(v, {
+                let b = Ee(h, e.inputId + "-ts-label");
+                D(m, {
                     "aria-labelledby": b
                 }), D(o, {
                     "aria-labelledby": b
                 })
             }
             if (i.style.width = g.style.width, e.plugins.names.length) {
                 let b = "plugin-" + e.plugins.names.join(" plugin-");
                 ee([i, s], b)
             }(t.maxItems === null || t.maxItems > 1) && e.is_select_tag && D(g, {
                 multiple: "multiple"
             }), t.placeholder && D(n, {
                 placeholder: t.placeholder
-            }), !t.splitOn && t.delimiter && (t.splitOn = new RegExp("\\s*" + (0, Ze.escape_regex)(t.delimiter) + "+\\s*")), t.load && t.loadThrottle && (t.load = Qe(t.load, t.loadThrottle)), Q(s, "mousemove", () => {
+            }), !t.splitOn && t.delimiter && (t.splitOn = new RegExp("\\s*" + (0, et.escape_regex)(t.delimiter) + "+\\s*")), t.load && t.loadThrottle && (t.load = Ue(t.load, t.loadThrottle)), Q(s, "mousemove", () => {
                 e.ignoreHover = !1
             }), Q(s, "mouseenter", b => {
-                var V = we(b.target, "[data-selectable]", s);
-                V && e.onOptionHover(b, V)
+                var $ = Oe(b.target, "[data-selectable]", s);
+                $ && e.onOptionHover(b, $)
             }, {
                 capture: !0
             }), Q(s, "click", b => {
-                let V = we(b.target, "[data-selectable]");
-                V && (e.onOptionSelect(b, V), j(b, !0))
+                let $ = Oe(b.target, "[data-selectable]");
+                $ && (e.onOptionSelect(b, $), j(b, !0))
             }), Q(p, "click", b => {
-                var V = we(b.target, "[data-ts-item]", p);
-                if (V && e.onItemSelect(b, V)) {
+                var $ = Oe(b.target, "[data-ts-item]", p);
+                if ($ && e.onItemSelect(b, $)) {
                     j(b, !0);
                     return
                 }
                 n.value == "" && (e.onClick(), j(b, !0))
-            }), Q(v, "keydown", b => e.onKeyDown(b)), Q(n, "keypress", b => e.onKeyPress(b)), Q(n, "input", b => e.onInput(b)), Q(v, "blur", b => e.onBlur(b)), Q(v, "focus", b => e.onFocus(b)), Q(n, "paste", b => e.onPaste(b));
+            }), Q(m, "keydown", b => e.onKeyDown(b)), Q(n, "keypress", b => e.onKeyPress(b)), Q(n, "input", b => e.onInput(b)), Q(m, "blur", b => e.onBlur(b)), Q(m, "focus", b => e.onFocus(b)), Q(n, "paste", b => e.onPaste(b));
             let k = b => {
-                    let V = b.composedPath()[0];
-                    if (!i.contains(V) && !s.contains(V)) {
+                    let $ = b.composedPath()[0];
+                    if (!i.contains($) && !s.contains($)) {
                         e.isFocused && e.blur(), e.inputState();
                         return
                     }
-                    V == n && e.isOpen ? b.stopPropagation() : j(b, !0)
+                    $ == n && e.isOpen ? b.stopPropagation() : j(b, !0)
                 },
                 N = () => {
                     e.isOpen && e.positionDropdown()
                 };
             Q(document, "mousedown", k), Q(window, "scroll", N, M), Q(window, "resize", N, M), this._destroy = () => {
                 document.removeEventListener("mousedown", k), window.removeEventListener("scroll", N), window.removeEventListener("resize", N), h && h.removeEventListener("click", Y)
             }, this.revertSettings = {
@@ -1261,30 +1261,30 @@
                 focus: "onFocus",
                 blur: "onBlur"
             };
             for (e in n) t = this.settings[n[e]], t && this.on(e, t)
         }
         sync(e = !0) {
             let t = this,
-                n = e ? Ee(t.input, {
+                n = e ? xe(t.input, {
                     delimiter: t.settings.delimiter
                 }) : t.settings;
             t.setupOptions(n.options, n.optgroups), t.setValue(n.items || [], !0), t.lastQuery = null
         }
         onClick() {
             var e = this;
             if (e.activeItems.length > 0) {
                 e.clearActiveItems(), e.focus();
                 return
             }
             e.isFocused && e.isOpen ? e.blur() : e.focus()
         }
         onMouseDown() {}
         onChange() {
-            Te(this.input, "input"), Te(this.input, "change")
+            we(this.input, "input"), we(this.input, "change")
         }
         onPaste(e) {
             var t = this;
             if (t.isInputHidden || t.isLocked) {
                 j(e);
                 return
             }
@@ -1314,15 +1314,15 @@
             var t = this;
             if (t.ignoreHover = !0, t.isLocked) {
                 e.keyCode !== 9 && j(e);
                 return
             }
             switch (e.keyCode) {
                 case 65:
-                    if (ae(ve, e) && t.control_input.value == "") {
+                    if (ae(be, e) && t.control_input.value == "") {
                         j(e), t.selectAll();
                         return
                     }
                     break;
                 case 27:
                     t.isOpen && (j(e, !0), t.close()), t.clearActiveItems();
                     return;
@@ -1354,25 +1354,25 @@
                     t.settings.selectOnTab && (t.canSelect(t.activeOption) && (t.onOptionSelect(e, t.activeOption), j(e)), t.settings.create && t.createItem() && j(e));
                     return;
                 case 8:
                 case 46:
                     t.deleteSelection(e);
                     return
             }
-            t.isInputHidden && !ae(ve, e) && j(e)
+            t.isInputHidden && !ae(be, e) && j(e)
         }
         onInput(e) {
             if (this.isLocked) return;
             let t = this.inputValue();
             if (this.lastValue !== t) {
                 if (this.lastValue = t, t == "") {
                     this._onInput();
                     return
                 }
-                this.refreshTimeout && clearTimeout(this.refreshTimeout), this.refreshTimeout = Ge(() => {
+                this.refreshTimeout && clearTimeout(this.refreshTimeout), this.refreshTimeout = Qe(() => {
                     this.refreshTimeout = null, this._onInput()
                 }, this.settings.refreshThrottle)
             }
         }
         _onInput() {
             let e = this.lastValue;
             this.settings.shouldLoad.call(this, e) && this.load(e), this.refreshOptions(), this.trigger("type", e)
@@ -1431,40 +1431,40 @@
         preload() {
             var e = this.wrapper.classList;
             e.contains("preloaded") || (e.add("preloaded"), this.load(""))
         }
         setTextboxValue(e = "") {
             var t = this.control_input,
                 n = t.value !== e;
-            n && (t.value = e, Te(t, "update"), this.lastValue = e)
+            n && (t.value = e, we(t, "update"), this.lastValue = e)
         }
         getValue() {
             return this.is_select_tag && this.input.hasAttribute("multiple") ? this.items : this.items.join(this.settings.delimiter)
         }
         setValue(e, t) {
             var n = t ? [] : ["change"];
-            He(this, n, () => {
+            ke(this, n, () => {
                 this.clear(t), this.addItems(e, t)
             })
         }
         setMaxItems(e) {
             e === 0 && (e = null), this.settings.maxItems = e, this.refreshState()
         }
         setActiveItem(e, t) {
             var n = this,
-                s, o, i, p, g, v;
+                s, o, i, p, g, m;
             if (n.settings.mode !== "single") {
                 if (!e) {
                     n.clearActiveItems(), n.isFocused && n.inputState();
                     return
                 }
                 if (s = t && t.type.toLowerCase(), s === "click" && ae("shiftKey", t) && n.activeItems.length) {
-                    for (v = n.getLastActive(), i = Array.prototype.indexOf.call(n.control.children, v), p = Array.prototype.indexOf.call(n.control.children, e), i > p && (g = i, i = p, p = g), o = i; o <= p; o++) e = n.control.children[o], n.activeItems.indexOf(e) === -1 && n.setActiveItemClass(e);
+                    for (m = n.getLastActive(), i = Array.prototype.indexOf.call(n.control.children, m), p = Array.prototype.indexOf.call(n.control.children, e), i > p && (g = i, i = p, p = g), o = i; o <= p; o++) e = n.control.children[o], n.activeItems.indexOf(e) === -1 && n.setActiveItemClass(e);
                     j(t)
-                } else s === "click" && ae(ve, t) || s === "keydown" && ae("shiftKey", t) ? e.classList.contains("active") ? n.removeActiveItem(e) : n.setActiveItemClass(e) : (n.clearActiveItems(), n.setActiveItemClass(e));
+                } else s === "click" && ae(be, t) || s === "keydown" && ae("shiftKey", t) ? e.classList.contains("active") ? n.removeActiveItem(e) : n.setActiveItemClass(e) : (n.clearActiveItems(), n.setActiveItemClass(e));
                 n.inputState(), n.isFocused || n.focus()
             }
         }
         setActiveItemClass(e) {
             let t = this,
                 n = t.control.querySelector(".last-active");
             n && re(n, "last-active"), ee(e, "active last-active"), t.trigger("item_select", e), t.activeItems.indexOf(e) == -1 && t.activeItems.push(e)
@@ -1554,25 +1554,25 @@
                 score: n
             })), s.currentResults = t) : t = Object.assign({}, s.currentResults), s.settings.hideSelected && (t.items = t.items.filter(i => {
                 let p = ne(i.id);
                 return !(p && s.items.indexOf(p) !== -1)
             })), t
         }
         refreshOptions(e = !0) {
-            var t, n, s, o, i, p, g, v, M, w;
+            var t, n, s, o, i, p, g, m, M, w;
             let X = {},
                 U = [];
             var h = this,
                 Y = h.inputValue();
             let k = Y === h.lastQuery || Y == "" && h.lastQuery == null;
             var N = h.search(Y),
                 b = null,
-                V = h.settings.shouldOpen || !1,
+                $ = h.settings.shouldOpen || !1,
                 W = h.dropdown_content;
-            k && (b = h.activeOption, b && (M = b.closest("[data-group]"))), o = N.items.length, typeof h.settings.maxOptions == "number" && (o = Math.min(o, h.settings.maxOptions)), o > 0 && (V = !0);
+            k && (b = h.activeOption, b && (M = b.closest("[data-group]"))), o = N.items.length, typeof h.settings.maxOptions == "number" && (o = Math.min(o, h.settings.maxOptions)), o > 0 && ($ = !0);
             let oe = (A, O) => {
                 let q = X[A];
                 if (q !== void 0) {
                     let z = U[q];
                     if (z !== void 0) return [q, z.fragment]
                 }
                 let P = document.createDocumentFragment();
@@ -1584,26 +1584,26 @@
             };
             for (t = 0; t < o; t++) {
                 let A = N.items[t];
                 if (!A) continue;
                 let O = A.id,
                     q = h.options[O];
                 if (q === void 0) continue;
-                let P = be(O),
+                let P = ye(O),
                     z = h.getOption(P, !0);
                 for (h.settings.hideSelected || z.classList.toggle("selected", h.items.includes(P)), i = q[h.settings.optgroupField] || "", p = Array.isArray(i) ? i : [i], n = 0, s = p && p.length; n < s; n++) {
                     i = p[n];
                     let se = q.$order,
                         f = h.optgroups[i];
                     f === void 0 ? i = "" : se = f.$order;
-                    let [_, T] = oe(i, se);
+                    let [S, T] = oe(i, se);
                     n > 0 && (z = z.cloneNode(!0), D(z, {
                         id: q.$id + "-clone-" + n,
                         "aria-selected": null
-                    }), z.classList.add("ts-cloned"), re(z, "active"), h.activeOption && h.activeOption.dataset.value == O && M && M.dataset.group === i.toString() && (b = z)), T.appendChild(z), i != "" && (X[i] = _)
+                    }), z.classList.add("ts-cloned"), re(z, "active"), h.activeOption && h.activeOption.dataset.value == O && M && M.dataset.group === i.toString() && (b = z)), T.appendChild(z), i != "" && (X[i] = S)
                 }
             }
             h.settings.lockOptgroupOrder && U.sort((A, O) => A.order - O.order), g = document.createDocumentFragment(), (0, te.iterate)(U, A => {
                 let O = A.fragment,
                     q = A.optgroup;
                 if (!O || !O.children.length) return;
                 let P = h.optgroups[q];
@@ -1613,24 +1613,24 @@
                     ce(z, se), ce(z, O);
                     let f = h.render("optgroup", {
                         group: P,
                         options: z
                     });
                     ce(g, f)
                 } else ce(g, O)
-            }), W.innerHTML = "", ce(W, g), h.settings.highlight && (Be(W), N.query.length && N.tokens.length && (0, te.iterate)(N.tokens, A => {
-                Ye(W, A.regex)
+            }), W.innerHTML = "", ce(W, g), h.settings.highlight && (Ge(W), N.query.length && N.tokens.length && (0, te.iterate)(N.tokens, A => {
+                Be(W, A.regex)
             }));
-            var $ = A => {
+            var V = A => {
                 let O = h.render(A, {
                     input: Y
                 });
-                return O && (V = !0, W.insertBefore(O, W.firstChild)), O
+                return O && ($ = !0, W.insertBefore(O, W.firstChild)), O
             };
-            if (h.loading ? $("loading") : h.settings.shouldLoad.call(h, Y) ? N.items.length === 0 && $("no_results") : $("not_loading"), v = h.canCreate(Y), v && (w = $("option_create")), h.hasOptions = N.items.length > 0 || v, V) {
+            if (h.loading ? V("loading") : h.settings.shouldLoad.call(h, Y) ? N.items.length === 0 && V("no_results") : V("not_loading"), m = h.canCreate(Y), m && (w = V("option_create")), h.hasOptions = N.items.length > 0 || m, $) {
                 if (N.items.length > 0) {
                     if (!b && h.settings.mode === "single" && h.items[0] != null && (b = h.getOption(h.items[0])), !W.contains(b)) {
                         let A = 0;
                         w && !h.settings.addPrecedence && (A = 1), b = h.selectable()[A]
                     }
                 } else w && (b = w);
                 e && !h.isOpen && (h.open(), h.scrollToOption(b, "auto")), h.setActiveOption(b)
@@ -1672,28 +1672,28 @@
             var s, o;
             let i = ne(e),
                 p = ne(t[n.settings.valueField]);
             if (i === null) return;
             let g = n.options[i];
             if (g == null) return;
             if (typeof p != "string") throw new Error("Value must be set in option data");
-            let v = n.getOption(i),
+            let m = n.getOption(i),
                 M = n.getItem(i);
-            if (t.$order = t.$order || g.$order, delete n.options[i], n.uncacheValue(p), n.options[p] = t, v) {
-                if (n.dropdown_content.contains(v)) {
+            if (t.$order = t.$order || g.$order, delete n.options[i], n.uncacheValue(p), n.options[p] = t, m) {
+                if (n.dropdown_content.contains(m)) {
                     let w = n._render("option", t);
-                    me(v, w), n.activeOption === v && n.setActiveOption(w)
+                    ve(m, w), n.activeOption === m && n.setActiveOption(w)
                 }
-                v.remove()
+                m.remove()
             }
-            M && (o = n.items.indexOf(i), o !== -1 && n.items.splice(o, 1, p), s = n._render("item", t), M.classList.contains("active") && ee(s, "active"), me(M, s)), n.lastQuery = null
+            M && (o = n.items.indexOf(i), o !== -1 && n.items.splice(o, 1, p), s = n._render("item", t), M.classList.contains("active") && ee(s, "active"), ve(M, s)), n.lastQuery = null
         }
         removeOption(e, t) {
             let n = this;
-            e = be(e), n.uncacheValue(e), delete n.userOptions[e], delete n.options[e], n.lastQuery = null, n.trigger("option_remove", e), n.removeItem(e, t)
+            e = ye(e), n.uncacheValue(e), delete n.userOptions[e], delete n.options[e], n.lastQuery = null, n.trigger("option_remove", e), n.removeItem(e, t)
         }
         clearOptions(e) {
             let t = (e || this.clearFilter).bind(this);
             this.loadedSearches = {}, this.userOptions = {}, this.clearCache();
             let n = {};
             (0, te.iterate)(this.options, (s, o) => {
                 t(s, o) && (n[o] = s)
@@ -1720,67 +1720,67 @@
             for (let i = 0; i < o.length; i++)
                 if (o[i] == e) return t > 0 ? o[i + 1] : o[i - 1];
             return null
         }
         getItem(e) {
             if (typeof e == "object") return e;
             var t = ne(e);
-            return t !== null ? this.control.querySelector(`[data-value="${ke(t)}"]`) : null
+            return t !== null ? this.control.querySelector(`[data-value="${Pe(t)}"]`) : null
         }
         addItems(e, t) {
             var n = this,
                 s = Array.isArray(e) ? e : [e];
             s = s.filter(i => n.items.indexOf(i) === -1);
             let o = s[s.length - 1];
             s.forEach(i => {
                 n.isPending = i !== o, n.addItem(i, t)
             })
         }
         addItem(e, t) {
             var n = t ? [] : ["change", "dropdown_close"];
-            He(this, n, () => {
+            ke(this, n, () => {
                 var s, o;
                 let i = this,
                     p = i.settings.mode,
                     g = ne(e);
                 if (!(g && i.items.indexOf(g) !== -1 && (p === "single" && i.close(), p === "single" || !i.settings.duplicates)) && !(g === null || !i.options.hasOwnProperty(g)) && (p === "single" && i.clear(t), !(p === "multi" && i.isFull()))) {
                     if (s = i._render("item", i.options[g]), i.control.contains(s) && (s = s.cloneNode(!0)), o = i.isFull(), i.items.splice(i.caretPos, 0, g), i.insertAtCaret(s), i.isSetup) {
                         if (!i.isPending && i.settings.hideSelected) {
-                            let v = i.getOption(g),
-                                M = i.getAdjacent(v, 1);
+                            let m = i.getOption(g),
+                                M = i.getAdjacent(m, 1);
                             M && i.setActiveOption(M)
                         }!i.isPending && !i.settings.closeAfterSelect && i.refreshOptions(i.isFocused && p !== "single"), i.settings.closeAfterSelect != !1 && i.isFull() ? i.close() : i.isPending || i.positionDropdown(), i.trigger("item_add", g, s), i.isPending || i.updateOriginalInput({
                             silent: t
                         })
                     }(!i.isPending || !o && i.isFull()) && (i.inputState(), i.refreshState())
                 }
             })
         }
         removeItem(e = null, t) {
             let n = this;
             if (e = n.getItem(e), !e) return;
             var s, o;
             let i = e.dataset.value;
-            s = Me(e), e.remove(), e.classList.contains("active") && (o = n.activeItems.indexOf(e), n.activeItems.splice(o, 1), re(e, "active")), n.items.splice(s, 1), n.lastQuery = null, !n.settings.persist && n.userOptions.hasOwnProperty(i) && n.removeOption(i, t), s < n.caretPos && n.setCaret(n.caretPos - 1), n.updateOriginalInput({
+            s = Fe(e), e.remove(), e.classList.contains("active") && (o = n.activeItems.indexOf(e), n.activeItems.splice(o, 1), re(e, "active")), n.items.splice(s, 1), n.lastQuery = null, !n.settings.persist && n.userOptions.hasOwnProperty(i) && n.removeOption(i, t), s < n.caretPos && n.setCaret(n.caretPos - 1), n.updateOriginalInput({
                 silent: t
             }), n.refreshState(), n.positionDropdown(), n.trigger("item_remove", i, e)
         }
         createItem(e = null, t = () => {}) {
             arguments.length === 3 && (t = arguments[2]), typeof t != "function" && (t = () => {});
             var n = this,
                 s = n.caretPos,
                 o;
             if (e = e || n.inputValue(), !n.canCreate(e)) return t(), !1;
             n.lock();
             var i = !1,
                 p = g => {
                     if (n.unlock(), !g || typeof g != "object") return t();
-                    var v = ne(g[n.settings.valueField]);
-                    if (typeof v != "string") return t();
-                    n.setTextboxValue(), n.addOption(g, !0), n.setCaret(s), n.addItem(v), t(g), i = !0
+                    var m = ne(g[n.settings.valueField]);
+                    if (typeof m != "string") return t();
+                    n.setTextboxValue(), n.addOption(g, !0), n.setCaret(s), n.addItem(m), t(g), i = !0
                 };
             return typeof n.settings.create == "function" ? o = n.settings.create.call(this, e, p) : o = {
                 [n.settings.labelField]: e,
                 [n.settings.valueField]: e
             }, i || p(o), !0
         }
         refreshItems() {
@@ -1790,72 +1790,72 @@
         refreshState() {
             let e = this;
             e.refreshValidityState();
             let t = e.isFull(),
                 n = e.isLocked;
             e.wrapper.classList.toggle("rtl", e.rtl);
             let s = e.wrapper.classList;
-            s.toggle("focus", e.isFocused), s.toggle("disabled", e.isDisabled), s.toggle("readonly", e.isReadOnly), s.toggle("required", e.isRequired), s.toggle("invalid", !e.isValid), s.toggle("locked", n), s.toggle("full", t), s.toggle("input-active", e.isFocused && !e.isInputHidden), s.toggle("dropdown-active", e.isOpen), s.toggle("has-options", ze(e.options)), s.toggle("has-items", e.items.length > 0)
+            s.toggle("focus", e.isFocused), s.toggle("disabled", e.isDisabled), s.toggle("readonly", e.isReadOnly), s.toggle("required", e.isRequired), s.toggle("invalid", !e.isValid), s.toggle("locked", n), s.toggle("full", t), s.toggle("input-active", e.isFocused && !e.isInputHidden), s.toggle("dropdown-active", e.isOpen), s.toggle("has-options", Ye(e.options)), s.toggle("has-items", e.items.length > 0)
         }
         refreshValidityState() {
             var e = this;
             e.input.validity && (e.isValid = e.input.validity.valid, e.isInvalid = !e.isValid)
         }
         isFull() {
             return this.settings.maxItems !== null && this.items.length >= this.settings.maxItems
         }
         updateOriginalInput(e = {}) {
             let t = this;
             var n, s;
             let o = t.input.querySelector('option[value=""]');
             if (t.is_select_tag) {
-                let g = function(v, M, w) {
-                        return v || (v = Z('<option value="' + de(M) + '">' + de(w) + "</option>")), v != o && t.input.append(v), i.push(v), (v != o || p > 0) && (v.selected = !0), v
+                let g = function(m, M, w) {
+                        return m || (m = Z('<option value="' + pe(M) + '">' + pe(w) + "</option>")), m != o && t.input.append(m), i.push(m), (m != o || p > 0) && (m.selected = !0), m
                     },
                     i = [],
                     p = t.input.querySelectorAll("option:checked").length;
-                t.input.querySelectorAll("option:checked").forEach(v => {
-                    v.selected = !1
-                }), t.items.length == 0 && t.settings.mode == "single" ? g(o, "", "") : t.items.forEach(v => {
-                    if (n = t.options[v], s = n[t.settings.labelField] || "", i.includes(n.$option)) {
-                        let M = t.input.querySelector(`option[value="${ke(v)}"]:not(:checked)`);
-                        g(M, v, s)
-                    } else n.$option = g(n.$option, v, s)
+                t.input.querySelectorAll("option:checked").forEach(m => {
+                    m.selected = !1
+                }), t.items.length == 0 && t.settings.mode == "single" ? g(o, "", "") : t.items.forEach(m => {
+                    if (n = t.options[m], s = n[t.settings.labelField] || "", i.includes(n.$option)) {
+                        let M = t.input.querySelector(`option[value="${Pe(m)}"]:not(:checked)`);
+                        g(M, m, s)
+                    } else n.$option = g(n.$option, m, s)
                 })
             } else t.input.value = t.getValue();
             t.isSetup && (e.silent || t.trigger("change", t.getValue()))
         }
         open() {
             var e = this;
             e.isLocked || e.isOpen || e.settings.mode === "multi" && e.isFull() || (e.isOpen = !0, D(e.focus_node, {
                 "aria-expanded": "true"
-            }), e.refreshState(), ge(e.dropdown, {
+            }), e.refreshState(), me(e.dropdown, {
                 visibility: "hidden",
                 display: "block"
-            }), e.positionDropdown(), ge(e.dropdown, {
+            }), e.positionDropdown(), me(e.dropdown, {
                 visibility: "visible",
                 display: "block"
             }), e.focus(), e.trigger("dropdown_open", e.dropdown))
         }
         close(e = !0) {
             var t = this,
                 n = t.isOpen;
             e && (t.setTextboxValue(), t.settings.mode === "single" && t.items.length && t.inputState()), t.isOpen = !1, D(t.focus_node, {
                 "aria-expanded": "false"
-            }), ge(t.dropdown, {
+            }), me(t.dropdown, {
                 display: "none"
             }), t.settings.hideSelected && t.clearActiveOption(), t.refreshState(), n && t.trigger("dropdown_close", t.dropdown)
         }
         positionDropdown() {
             if (this.settings.dropdownParent === "body") {
                 var e = this.control,
                     t = e.getBoundingClientRect(),
                     n = e.offsetHeight + t.top + window.scrollY,
                     s = t.left + window.scrollX;
-                ge(this.dropdown, {
+                me(this.dropdown, {
                     width: t.width + "px",
                     top: n + "px",
                     left: s + "px"
                 })
             }
         }
         clear(e) {
@@ -1871,40 +1871,40 @@
             let t = this,
                 n = t.caretPos,
                 s = t.control;
             s.insertBefore(e, s.children[n] || null), t.setCaret(n + 1)
         }
         deleteSelection(e) {
             var t, n, s, o, i = this;
-            t = e && e.keyCode === 8 ? -1 : 1, n = Ue(i.control_input);
+            t = e && e.keyCode === 8 ? -1 : 1, n = Je(i.control_input);
             let p = [];
-            if (i.activeItems.length) o = Ce(i.activeItems, t), s = Me(o), t > 0 && s++, (0, te.iterate)(i.activeItems, g => p.push(g));
+            if (i.activeItems.length) o = Me(i.activeItems, t), s = Fe(o), t > 0 && s++, (0, te.iterate)(i.activeItems, g => p.push(g));
             else if ((i.isFocused || i.settings.mode === "single") && i.items.length) {
                 let g = i.controlChildren(),
-                    v;
-                t < 0 && n.start === 0 && n.length === 0 ? v = g[i.caretPos - 1] : t > 0 && n.start === i.inputValue().length && (v = g[i.caretPos]), v !== void 0 && p.push(v)
+                    m;
+                t < 0 && n.start === 0 && n.length === 0 ? m = g[i.caretPos - 1] : t > 0 && n.start === i.inputValue().length && (m = g[i.caretPos]), m !== void 0 && p.push(m)
             }
             if (!i.shouldDelete(p, e)) return !1;
             for (j(e, !0), typeof s < "u" && i.setCaret(s); p.length;) i.removeItem(p.pop());
             return i.inputState(), i.positionDropdown(), i.refreshOptions(!1), !0
         }
         shouldDelete(e, t) {
             let n = e.map(s => s.dataset.value);
             return !(!n.length || typeof this.settings.onDelete == "function" && this.settings.onDelete(n, t) === !1)
         }
         advanceSelection(e, t) {
             var n, s, o = this;
-            o.rtl && (e *= -1), !o.inputValue().length && (ae(ve, t) || ae("shiftKey", t) ? (n = o.getLastActive(e), n ? n.classList.contains("active") ? s = o.getAdjacent(n, e, "item") : s = n : e > 0 ? s = o.control_input.nextElementSibling : s = o.control_input.previousElementSibling, s && (s.classList.contains("active") && o.removeActiveItem(n), o.setActiveItemClass(s))) : o.moveCaret(e))
+            o.rtl && (e *= -1), !o.inputValue().length && (ae(be, t) || ae("shiftKey", t) ? (n = o.getLastActive(e), n ? n.classList.contains("active") ? s = o.getAdjacent(n, e, "item") : s = n : e > 0 ? s = o.control_input.nextElementSibling : s = o.control_input.previousElementSibling, s && (s.classList.contains("active") && o.removeActiveItem(n), o.setActiveItemClass(s))) : o.moveCaret(e))
         }
         moveCaret(e) {}
         getLastActive(e) {
             let t = this.control.querySelector(".last-active");
             if (t) return t;
             var n = this.control.querySelectorAll(".active");
-            if (n) return Ce(n, e)
+            if (n) return Me(n, e)
         }
         setCaret(e) {
             this.caretPos = this.items.length
         }
         controlChildren() {
             return Array.from(this.control.querySelectorAll("[data-ts-item]"))
         }
@@ -1933,25 +1933,25 @@
             var e = this,
                 t = e.revertSettings;
             e.trigger("destroy"), e.off(), e.wrapper.remove(), e.dropdown.remove(), e.input.innerHTML = t.innerHTML, e.input.tabIndex = t.tabIndex, re(e.input, "tomselected", "ts-hidden-accessible"), e._destroy(), delete e.input.tomselect
         }
         render(e, t) {
             var n, s;
             let o = this;
-            if (typeof this.settings.render[e] != "function" || (s = o.settings.render[e].call(this, t, de), !s)) return null;
+            if (typeof this.settings.render[e] != "function" || (s = o.settings.render[e].call(this, t, pe), !s)) return null;
             if (s = Z(s), e === "option" || e === "option_create" ? t[o.settings.disabledField] ? D(s, {
                     "aria-disabled": "true"
                 }) : D(s, {
                     "data-selectable": ""
                 }) : e === "optgroup" && (n = t.group[o.settings.optgroupValueField], D(s, {
                     "data-group": n
                 }), t.group[o.settings.disabledField] && D(s, {
                     "data-disabled": ""
                 })), e === "option" || e === "item") {
-                let i = be(t[o.settings.valueField]);
+                let i = ye(t[o.settings.valueField]);
                 D(s, {
                     "data-value": i
                 }), e === "item" ? (ee(s, o.settings.itemClass), D(s, {
                     "data-ts-item": ""
                 })) : (ee(s, o.settings.optionClass), D(s, {
                     role: "option",
                     id: t.$id
@@ -1982,241 +1982,249 @@
             s[t] = function() {
                 var i, p;
                 return e === "after" && (i = o.apply(s, arguments)), p = n.apply(s, arguments), e === "instead" ? p : (e === "before" && (i = o.apply(s, arguments)), i)
             }
         }
     };
 
-function et(r) {
+function tt(r) {
     let c = Object.assign({
         label: "&times;",
         title: "Remove",
         className: "remove",
         append: !0
     }, r);
     var e = this;
     if (c.append) {
-        var t = '<a href="javascript:void(0)" class="' + c.className + '" tabindex="-1" title="' + de(c.title) + '">' + c.label + "</a>";
+        var t = '<a href="javascript:void(0)" class="' + c.className + '" tabindex="-1" title="' + pe(c.title) + '">' + c.label + "</a>";
         e.hook("after", "setupTemplates", () => {
             var n = e.settings.render.item;
             e.settings.render.item = (s, o) => {
                 var i = Z(n.call(e, s, o)),
                     p = Z(t);
                 return i.appendChild(p), Q(p, "mousedown", g => {
                     j(g, !0)
                 }), Q(p, "click", g => {
                     e.isLocked || (j(g, !0), !e.isLocked && e.shouldDelete([i], g) && (e.removeItem(i), e.refreshOptions(!1), e.inputState()))
                 }), i
             }
         })
     }
 }
-var st = ye(it());
-var tt = ".ts-wrapper{position:relative}.ts-wrapper .ts-control{overflow:hidden;box-sizing:border-box;display:flex;flex-wrap:wrap;align-content:center}.ts-wrapper .ts-control>input{flex:1 1 auto;box-sizing:border-box;user-select:auto;box-shadow:none;border:none;padding:0;font-size:inherit;font-weight:inherit;font-style:inherit;font-family:inherit;caret-color:rgba(0,0,0,.15)}.ts-wrapper .ts-control>input::placeholder{opacity:1}.ts-wrapper .ts-control>input::-ms-clear{display:none}.ts-wrapper .ts-control>input:focus{outline:none !important}.ts-wrapper .ts-control>div{flex:0 1 auto;box-sizing:border-box}.ts-wrapper.multi .ts-control{padding:0 6px 3px 10px}.ts-wrapper.multi .ts-control>div{border:1px solid rgba(0,0,0,.15);border-radius:3px;margin:3px 3px 0 0}.ts-wrapper.multi .ts-control>div .remove{text-decoration:none;color:rgba(0,0,0,.15);border-left:1px solid rgba(0,0,0,.15);padding-left:2px;margin-left:2px}.ts-wrapper.multi .ts-control>div .remove:hover{color:inherit}.ts-wrapper.multi.full .ts-control>input{visibility:hidden}.ts-wrapper.multi.has-items:not(.dirty) .ts-control>input::placeholder{opacity:0}.ts-wrapper.focus .ts-control{--dummy-style: none}.ts-wrapper.disabled .ts-control{--dummy-style: none}.ts-wrapper.input-hidden .ts-control>input{opacity:0;position:absolute;left:-10000px}.ts-wrapper:not(.multi).dirty.focus .ts-control .item{display:none}.ts-wrapper .ts-dropdown{position:absolute;top:100%;left:0;width:100%;z-index:10;background-color:#f8f8f8;backdrop-filter:blur(0.5rem);margin:.125rem 0 0 0;border-top:0 none;box-sizing:border-box}.ts-wrapper .ts-dropdown [data-selectable]{cursor:pointer;overflow:hidden}.ts-wrapper .ts-dropdown [data-selectable][aria-selected=true]{background-color:rgba(0,0,0,.05)}.ts-wrapper .ts-dropdown [data-selectable].selected{background-color:#e0ecf4}.ts-wrapper .ts-dropdown [data-selectable] .highlight{background:rgba(255,237,40,.4);border-radius:1px}.ts-wrapper .ts-dropdown .ts-dropdown-content{overflow-y:auto;overflow-x:hidden;overflow-scrolling:touch;scroll-behavior:smooth}.ts-wrapper .ts-dropdown .optgroup .optgroup-header{opacity:.5}.ts-wrapper .ts-dropdown .optgroup .option{margin-left:1em}:host-context([role=group].dj-touched) .ts-wrapper.has-items:not(.input-active) .ts-control{border-color:var(--django-formset-color-valid)}:host-context([role=group].dj-touched) .ts-wrapper.invalid:not(.input-active) .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid.focus .ts-control{opacity:1}";
-pe.define("remove_button", et);
-var Pe = class extends Ve {
-        constructor(e) {
-            super(e);
-            this.extraStyleSheet = new CSSStyleSheet;
-            this.numOptions = 12;
-            this.initialValue = "";
-            this.baseSelector = ".ts-wrapper";
-            this.getValue = () => this.currentValue;
-            this.load = (e, t) => {
-                this.loadOptions(this.buildFetchQuery(0, e), n => {
-                    t(n, this.extractOptGroups(n))
-                })
-            };
-            this.blurred = () => {
-                let e = this.shadowRoot.querySelector(".ts-wrapper");
-                e == null || e.classList.remove("dirty")
-            };
-            this.inputted = e => {
-                let t = e,
-                    n = this.shadowRoot.querySelector(".ts-wrapper");
-                n == null || n.classList.toggle("dirty", t.length > 0)
-            };
-            this.attributesChanged = e => {
-                for (let t of e) t.type === "attributes" && t.attributeName === "disabled" && (this.tomSelect.input.disabled ? this.tomSelect.isDisabled || this.tomSelect.disable() : this.tomSelect.isDisabled && this.tomSelect.enable())
-            };
-            let t = !1;
-            e.hasAttribute("multiple") && (e.removeAttribute("multiple"), t = !0);
-            let n = {
-                ...window.getComputedStyle(e)
+var it = Se(rt());
+var nt = ".ts-wrapper{position:relative}.ts-wrapper .ts-control{overflow:hidden;box-sizing:border-box;display:flex;flex-wrap:wrap;align-content:center}.ts-wrapper .ts-control>input{flex:1 1 auto;box-sizing:border-box;user-select:auto;box-shadow:none;border:none;padding:0;font-size:inherit;font-weight:inherit;font-style:inherit;font-family:inherit;caret-color:rgba(0,0,0,.15)}.ts-wrapper .ts-control>input::placeholder{opacity:1}.ts-wrapper .ts-control>input::-ms-clear{display:none}.ts-wrapper .ts-control>input:focus{outline:none !important}.ts-wrapper .ts-control>div{flex:0 1 auto;box-sizing:border-box}.ts-wrapper.multi .ts-control{padding:0 6px 3px 10px}.ts-wrapper.multi .ts-control>div{border:1px solid rgba(0,0,0,.15);border-radius:3px;margin:3px 3px 0 0}.ts-wrapper.multi .ts-control>div .remove{text-decoration:none;color:rgba(0,0,0,.15);border-left:1px solid rgba(0,0,0,.15);padding-left:2px;margin-left:2px}.ts-wrapper.multi .ts-control>div .remove:hover{color:inherit}.ts-wrapper.multi.full .ts-control>input{visibility:hidden}.ts-wrapper.multi.has-items:not(.dirty) .ts-control>input::placeholder{opacity:0}.ts-wrapper.focus .ts-control{--dummy-style: none}.ts-wrapper.disabled .ts-control{--dummy-style: none}.ts-wrapper.input-hidden .ts-control>input{opacity:0;position:absolute;left:-10000px}.ts-wrapper:not(.multi).dirty.focus .ts-control .item{display:none}.ts-wrapper .ts-dropdown{position:absolute;top:100%;left:0;width:100%;z-index:10;background-color:#f8f8f8;backdrop-filter:blur(0.5rem);margin:.125rem 0 0 0;border-top:0 none;box-sizing:border-box}.ts-wrapper .ts-dropdown [data-selectable]{cursor:pointer;overflow:hidden}.ts-wrapper .ts-dropdown [data-selectable][aria-selected=true]{background-color:rgba(0,0,0,.05)}.ts-wrapper .ts-dropdown [data-selectable].selected{background-color:#e0ecf4}.ts-wrapper .ts-dropdown [data-selectable] .highlight{background:rgba(255,237,40,.4);border-radius:1px}.ts-wrapper .ts-dropdown .ts-dropdown-content{overflow-y:auto;overflow-x:hidden;overflow-scrolling:touch;scroll-behavior:smooth}.ts-wrapper .ts-dropdown .optgroup .optgroup-header{opacity:.5}.ts-wrapper .ts-dropdown .optgroup .option{margin-left:1em}:host-context([role=group].dj-touched) .ts-wrapper.has-items:not(.input-active) .ts-control{border-color:var(--django-formset-color-valid)}:host-context([role=group].dj-touched) .ts-wrapper.invalid:not(.input-active) .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid .ts-control{border-color:var(--django-formset-color-invalid)}:host-context([role=group].dj-submitted) .ts-wrapper.invalid.focus .ts-control{opacity:1}";
+fe.define("remove_button", tt);
+var ue = class ue extends Ve {
+    constructor(e) {
+        super(e);
+        this.numOptions = 12;
+        this.initialValue = "";
+        this.baseSelector = ".ts-wrapper";
+        this.getValue = () => this.currentValue;
+        this.load = (e, t) => {
+            this.loadOptions(this.buildFetchQuery(0, e), n => {
+                t(n, this.extractOptGroups(n))
+            })
+        };
+        this.blurred = () => {
+            let e = this.shadowRoot.querySelector(this.baseSelector);
+            e == null || e.classList.remove("dirty")
+        };
+        this.inputted = e => {
+            let t = e,
+                n = this.shadowRoot.querySelector(this.baseSelector);
+            n == null || n.classList.toggle("dirty", t.length > 0)
+        };
+        this.attributesChanged = e => {
+            for (let t of e) t.type === "attributes" && t.attributeName === "disabled" && (this.tomSelect.input.disabled ? this.tomSelect.isDisabled || this.tomSelect.disable() : this.tomSelect.isDisabled && this.tomSelect.enable())
+        };
+        let t = !1;
+        e.hasAttribute("multiple") && (e.removeAttribute("multiple"), t = !0);
+        let n = {
+            ...window.getComputedStyle(e)
+        };
+        t && e.setAttribute("multiple", "multiple"), this.numOptions = parseInt(e.getAttribute("options") ?? this.numOptions.toString()), this.tomSelect = new fe(e, this.getSettings(e)), this.observer = new MutationObserver(this.attributesChanged), this.observer.observe(e, {
+            attributes: !0
+        }), this.initialValue = this.currentValue, this.shadowRoot = this.wrapInShadowRoot(), ue.styleSheet = ue.styleSheet ?? this.transferStyles(n), e.classList.add("dj-concealed"), this.validateInput(this.initialValue)
+    }
+    getSettings(e) {
+        var s, o, i;
+        let t = {
+                create: !1,
+                valueField: "id",
+                labelField: "label",
+                maxItems: 1,
+                maxOptions: void 0,
+                sortField: [{
+                    field: "$order"
+                }, {
+                    field: "$score"
+                }],
+                lockOptgroupOrder: !0,
+                searchField: ["label"],
+                render: {},
+                plugins: {},
+                onFocus: this.touch,
+                onBlur: this.blurred,
+                onType: this.inputted
+            },
+            n = (s = e.parentElement) == null ? void 0 : s.querySelector("template.select-no-results");
+        if (n && (t.render = {
+                ...t.render,
+                no_results: p => (0, it.default)(n.innerHTML)(p)
+            }), this.isIncomplete && (t.load = this.load), e.hasAttribute("multiple")) {
+            t.maxItems = parseInt(e.getAttribute("max_items") ?? "3");
+            let p = (o = e.parentElement) == null ? void 0 : o.querySelector("template.selectize-remove-item");
+            t.plugins = {
+                ...t.plugins,
+                remove_button: {
+                    title: (p == null ? void 0 : p.innerHTML) ?? "Remove item"
+                }
             };
-            t && e.setAttribute("multiple", "multiple"), this.numOptions = parseInt(e.getAttribute("options") ?? this.numOptions.toString()), this.tomSelect = new pe(e, this.getSettings(e)), this.observer = new MutationObserver(this.attributesChanged), this.observer.observe(e, {
-                attributes: !0
-            }), this.initialValue = this.currentValue, this.shadowRoot = this.wrapInShadowRoot(), this.transferStyles(n), e.classList.add("dj-concealed"), this.validateInput(this.initialValue)
-        }
-        getSettings(e) {
-            var s, o, i;
-            let t = {
-                    create: !1,
-                    valueField: "id",
-                    labelField: "label",
-                    maxItems: 1,
-                    maxOptions: void 0,
-                    sortField: [{
-                        field: "$order"
-                    }, {
-                        field: "$score"
-                    }],
-                    lockOptgroupOrder: !0,
-                    searchField: ["label"],
-                    render: {},
-                    plugins: {},
-                    onFocus: this.touch,
-                    onBlur: this.blurred,
-                    onType: this.inputted
-                },
-                n = (s = e.parentElement) == null ? void 0 : s.querySelector("template.select-no-results");
-            if (n && (t.render = {
-                    ...t.render,
-                    no_results: p => (0, st.default)(n.innerHTML)(p)
-                }), this.isIncomplete && (t.load = this.load), e.hasAttribute("multiple")) {
-                t.maxItems = parseInt(e.getAttribute("max_items") ?? "3");
-                let p = (o = e.parentElement) == null ? void 0 : o.querySelector("template.selectize-remove-item");
-                t.plugins = {
-                    ...t.plugins,
-                    remove_button: {
-                        title: (p == null ? void 0 : p.innerHTML) ?? "Remove item"
-                    }
-                };
-                let g = `${e.getAttribute("id")}_initial`;
-                t.items = JSON.parse(((i = document.getElementById(g)) == null ? void 0 : i.textContent) ?? "[]")
-            }
-            return t
+            let g = `${e.getAttribute("id")}_initial`;
+            t.items = JSON.parse(((i = document.getElementById(g)) == null ? void 0 : i.textContent) ?? "[]")
         }
-        async formResetted(e) {
-            this.getValue = () => this.initialValue, this.tomSelect.setValue(this.initialValue, !0), await this.reloadOptions(), this.getValue = () => this.currentValue
-        }
-        formSubmitted(e) {}
-        async reloadOptions(e) {
-            let t = this.getValue();
-            this.tomSelect.clear(!0), this.fieldGroup.classList.remove("dj-dirty", "dj-touched", "dj-validated"), this.fieldGroup.classList.add("dj-untouched", "dj-pristine");
-            let n = this.fieldGroup.querySelector(".dj-errorlist > .dj-placeholder");
-            n && (n.innerHTML = ""), this.isIncomplete && (this.tomSelect.clearOptions(), this.tomSelect.input.replaceChildren(), await this.loadOptions(this.buildFetchQuery(0), s => {
-                this.tomSelect.addOptions(s)
-            })), this.tomSelect.setValue(t, e)
-        }
-        get currentValue() {
-            let e = this.tomSelect.getValue();
-            return Array.isArray(e) ? [...e] : e
-        }
-        extractOptGroups(e) {
-            let t = new Set;
-            return e.forEach(n => {
-                typeof n.optgroup == "string" && t.add(n.optgroup)
-            }), Array.from(t).map(n => ({
-                label: n,
-                value: n
-            }))
-        }
-        validateInput(e) {
-            let t = this.shadowRoot.querySelector(".ts-wrapper");
-            t == null || t.classList.remove("dirty");
-            let n = this.tomSelect.input;
-            if (this.tomSelect.isRequired && n.setCustomValidity(e ? "" : "Value is missing."), n.multiple)
-                for (let s = 0; s < n.options.length; s++) {
-                    let o = n.options.item(s);
-                    o && (o.selected = e.indexOf(o.value) >= 0)
-                } else this.tomSelect.input.value = e
-        }
-        wrapInShadowRoot() {
-            let e = document.createElement("div");
-            e.classList.add("shadow-wrapper");
-            let t = e.attachShadow({
-                    mode: "open",
-                    delegatesFocus: !0
-                }),
-                n = document.createElement("style");
-            t.appendChild(n).textContent = tt, this.tomSelect.input.insertAdjacentElement("beforebegin", e);
-            let s = this.tomSelect.input.parentElement.removeChild(this.tomSelect.wrapper);
-            return t.appendChild(s), t
-        }
-        transferStyles(e) {
-            this.shadowRoot.host.style.setProperty("display", e.display);
-            let n = this.tomSelect.input,
-                s = window.getComputedStyle(n).getPropertyValue("line-height"),
-                o = n.querySelector("option"),
-                i = this.shadowRoot.styleSheets.item(0),
-                p = Math.min(Math.max(this.numOptions, 8), 25),
-                g = !1;
-            for (let v = 0; i && v < i.cssRules.length; v++) {
-                let M = i.cssRules.item(v),
-                    w = null;
-                switch (M.selectorText) {
-                    case this.baseSelector:
-                        w = ie.extractStyles(n, ["font-family", "font-size", "font-stretch", "font-style", "font-weight", "letter-spacing", "white-space"]), g = !0;
-                        break;
-                    case `${this.baseSelector} .ts-control`:
-                        w = ie.extractStyles(n, ["background-color", "border", "border-radius", "box-shadow", "color", "padding"]).concat(`width: ${e.width}; min-height: ${e.height};`);
-                        break;
-                    case `${this.baseSelector} .ts-control > input`:
-                    case `${this.baseSelector} .ts-control > div`:
-                        o && (w = ie.extractStyles(o, ["padding-left", "padding-right"]));
-                        break;
-                    case `${this.baseSelector} .ts-control > input::placeholder`:
-                        n.classList.add("-placeholder-"), w = ie.extractStyles(n, ["background-color", "color"]), n.classList.remove("-placeholder-");
-                        break;
-                    case `${this.baseSelector}.focus .ts-control`:
-                        n.style.transition = "none", n.classList.add("-focus-"), w = ie.extractStyles(n, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), n.classList.remove("-focus-"), n.style.transition = "";
-                        break;
-                    case `${this.baseSelector}.disabled .ts-control`:
-                        n.classList.add("-disabled-"), w = ie.extractStyles(n, ["background-color", "border", "box-shadow", "color", "opacity", "outline", "transition"]), n.classList.remove("-disabled-");
-                        break;
-                    case `${this.baseSelector} .ts-dropdown`:
-                        w = ie.extractStyles(n, ["border-right", "border-bottom", "border-left", "color"]).concat(parseFloat(s) > 0 ? `line-height: calc(${s} * 1.2);` : "line-height: 1.4em;");
-                        break;
-                    case `${this.baseSelector} .ts-dropdown .ts-dropdown-content`:
-                        parseFloat(s) > 0 ? w = `max-height: calc(${s} * 1.2 * ${p});` : w = `max-height: ${p*1.4}em;`;
-                        break;
-                    case `${this.baseSelector} .ts-dropdown [data-selectable]`:
-                        w = ie.extractStyles(n, ["padding-left"]);
-                        break;
-                    case ':host-context([role="group"].dj-submitted) .ts-wrapper.invalid.focus .ts-control':
-                        n.style.transition = "none", n.classList.add("-focus-", "-invalid-", "is-invalid"), w = ie.extractStyles(n, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), n.classList.remove("-focus-", "-invalid-", "is-invalid"), n.style.transition = "";
-                        break;
-                    default:
-                        break
-                }
-                w && this.extraStyleSheet.insertRule(`${M.selectorText}{${w}}`)
-            }
-            if (!g) throw new Error(`Could not load styles for ${this.baseSelector}`)
-        }
-        initialize() {
-            let e = this.shadowRoot.styleSheets.item(0);
-            for (let t = 0; t < this.extraStyleSheet.cssRules.length; t++) {
-                let n = this.extraStyleSheet.cssRules.item(t);
-                e.insertRule(n.cssText)
+        return t
+    }
+    async formResetted(e) {
+        this.getValue = () => this.initialValue, this.tomSelect.setValue(this.initialValue, !0), await this.reloadOptions(), this.getValue = () => this.currentValue
+    }
+    formSubmitted(e) {}
+    async reloadOptions(e) {
+        let t = this.getValue();
+        this.tomSelect.clear(!0), this.fieldGroup.classList.remove("dj-dirty", "dj-touched", "dj-validated"), this.fieldGroup.classList.add("dj-untouched", "dj-pristine");
+        let n = this.fieldGroup.querySelector(".dj-errorlist > .dj-placeholder");
+        n && (n.innerHTML = ""), this.isIncomplete && (this.tomSelect.clearOptions(), this.tomSelect.input.replaceChildren(), await this.loadOptions(this.buildFetchQuery(0), s => {
+            this.tomSelect.addOptions(s)
+        })), this.tomSelect.setValue(t, e)
+    }
+    get currentValue() {
+        let e = this.tomSelect.getValue();
+        return Array.isArray(e) ? [...e] : e
+    }
+    extractOptGroups(e) {
+        let t = new Set;
+        return e.forEach(n => {
+            typeof n.optgroup == "string" && t.add(n.optgroup)
+        }), Array.from(t).map(n => ({
+            label: n,
+            value: n
+        }))
+    }
+    validateInput(e) {
+        let t = this.shadowRoot.querySelector(this.baseSelector);
+        t == null || t.classList.remove("dirty");
+        let n = this.tomSelect.input;
+        if (this.tomSelect.isRequired && n.setCustomValidity(e ? "" : "Value is missing."), n.multiple)
+            for (let s = 0; s < n.options.length; s++) {
+                let o = n.options.item(s);
+                o && (o.selected = e.indexOf(o.value) >= 0)
+            } else this.tomSelect.input.value = e
+    }
+    wrapInShadowRoot() {
+        let e = document.createElement("div");
+        e.classList.add("shadow-wrapper");
+        let t = e.attachShadow({
+            mode: "open",
+            delegatesFocus: !0
+        });
+        t.adoptedStyleSheets = [new CSSStyleSheet], this.tomSelect.input.insertAdjacentElement("beforebegin", e);
+        let n = this.tomSelect.input.parentElement.removeChild(this.tomSelect.wrapper);
+        return t.appendChild(n), t
+    }
+    transferStyles(e) {
+        this.shadowRoot.host.style.setProperty("display", e.display);
+        let n = new CSSStyleSheet;
+        n.replaceSync(nt);
+        let s = this.tomSelect.input,
+            o = window.getComputedStyle(s).getPropertyValue("line-height"),
+            i = s.querySelector("option"),
+            p = Math.min(Math.max(this.numOptions, 8), 25),
+            g = !1;
+        for (let m = 0; n && m < n.cssRules.length; m++) {
+            let M = n.cssRules.item(m),
+                w = null;
+            switch (M.selectorText.trim()) {
+                case this.baseSelector:
+                    w = ie.extractStyles(s, ["font-family", "font-size", "font-stretch", "font-style", "font-weight", "letter-spacing", "white-space"]), g = !0;
+                    break;
+                case `${this.baseSelector} .ts-control`:
+                    w = ie.extractStyles(s, ["background-color", "border", "border-radius", "box-shadow", "color", "padding"]).concat(`min-height: ${e.height};`);
+                    break;
+                case `${this.baseSelector} .ts-control > input`:
+                case `${this.baseSelector} .ts-control > div`:
+                    i && (w = ie.extractStyles(i, ["padding-left", "padding-right"]));
+                    break;
+                case `${this.baseSelector} .ts-control > input::placeholder`:
+                    s.classList.add("-placeholder-"), w = ie.extractStyles(s, ["background-color", "color"]), s.classList.remove("-placeholder-");
+                    break;
+                case `${this.baseSelector}.focus .ts-control`:
+                    s.style.transition = "none", s.classList.add("-focus-"), w = ie.extractStyles(s, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), s.classList.remove("-focus-"), s.style.transition = "";
+                    break;
+                case `${this.baseSelector}.disabled .ts-control`:
+                    s.classList.add("-disabled-"), w = ie.extractStyles(s, ["background-color", "border", "box-shadow", "color", "opacity", "outline", "transition"]), s.classList.remove("-disabled-");
+                    break;
+                case `${this.baseSelector} .ts-dropdown`:
+                    w = ie.extractStyles(s, ["border-right", "border-bottom", "border-left", "color"]).concat(parseFloat(o) > 0 ? `line-height: calc(${o} * 1.2);` : "line-height: 1.4em;");
+                    break;
+                case `${this.baseSelector} .ts-dropdown .ts-dropdown-content`:
+                    parseFloat(o) > 0 ? w = `max-height: calc(${o} * 1.2 * ${p});` : w = `max-height: ${p*1.4}em;`;
+                    break;
+                case `${this.baseSelector} .ts-dropdown [data-selectable]`:
+                    w = ie.extractStyles(s, ["padding-left"]);
+                    break;
+                case ':host-context([role="group"].dj-submitted) .ts-wrapper.invalid.focus .ts-control':
+                    s.style.transition = "none", s.classList.add("-focus-", "-invalid-", "is-invalid"), w = ie.extractStyles(s, ["background-color", "border", "box-shadow", "color", "outline", "transition"]), s.classList.remove("-focus-", "-invalid-", "is-invalid"), s.style.transition = "";
+                    break;
+                default:
+                    break
             }
-            this.setupFilters(this.tomSelect.input), this.tomSelect.on("change", t => this.validateInput(t))
+            w && n.insertRule(`${M.selectorText}{${w}}`, ++m)
         }
-    },
-    fe = Symbol("DjangoSelectize"),
-    nt = class extends HTMLSelectElement {
+        if (!g) throw new Error(`Could not load styles for ${this.baseSelector}`);
+        return n
+    }
+    initialize() {
+        let e = this.shadowRoot.adoptedStyleSheets[0],
+            t = `${this.baseSelector} .ts-control`;
+        if (!ue.styleSheet) throw new Error("Stylesheet not loaded");
+        for (let o = 0; o < ue.styleSheet.cssRules.length; o++) {
+            let i = ue.styleSheet.cssRules.item(o);
+            e.insertRule(i.cssText)
+        }
+        let n = () => window.getComputedStyle(this.tomSelect.input).getPropertyValue("width"),
+            s = e.insertRule(`${t}{width:${n()};}`);
+        addEventListener("resize", o => {
+            e.deleteRule(s), e.insertRule(`${t}{width:${n()};}`, s)
+        }), this.setupFilters(this.tomSelect.input), this.tomSelect.on("change", o => this.validateInput(o))
+    }
+};
+ue.styleSheet = null;
+var Re = ue,
+    he = Symbol("DjangoSelectize"),
+    st = class extends HTMLSelectElement {
         constructor() {
-            super(), this[fe] = new Pe(this)
+            super(), this[he] = new Re(this)
         }
         connectedCallback() {
-            this[fe].initialize()
+            this[he].initialize()
         }
         get value() {
             var e;
-            let c = (e = this[fe]) == null ? void 0 : e.tomSelect.getValue();
+            let c = (e = this[he]) == null ? void 0 : e.tomSelect.getValue();
             return Array.isArray(c) ? c.join(",") : c
         }
         set value(c) {
             var e, t;
-            this.multiple ? (e = this[fe]) == null || e.tomSelect.setValue(c.split(","), !0) : (t = this[fe]) == null || t.tomSelect.setValue(c, !0)
+            this.multiple ? (e = this[he]) == null || e.tomSelect.setValue(c.split(","), !0) : (t = this[he]) == null || t.tomSelect.setValue(c, !0)
         }
     };
-fe;
+he;
 export {
-    Pe as a, nt as b
+    Re as a, st as b
 };
 /*! Bundled license information:
 
 @orchidjs/sifter/dist/umd/sifter.js:
   (*! sifter.js | https://github.com/orchidjs/sifter.js | Apache License (v2) *)
   (*! @orchidjs/unicode-variants | https://github.com/orchidjs/unicode-variants | Apache License (v2) *)
```

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-N376VWFX.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-NIKVGHIO.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-NOGHTXP6.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-NOGHTXP6.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-P2VM2T3G.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-P2VM2T3G.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-RQ46AVYK.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-RLE6ONWJ.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var pt = ["top", "right", "bottom", "left"],
     ht = ["start", "end"],
-    ct = pt.reduce((t, e) => t.concat(e, e + "-" + ht[0], e + "-" + ht[1]), []),
+    lt = pt.reduce((t, e) => t.concat(e, e + "-" + ht[0], e + "-" + ht[1]), []),
     I = Math.min,
     L = Math.max,
     Q = Math.round,
     Z = Math.floor,
     D = t => ({
         x: t,
         y: t
     }),
-    Vt = {
+    $t = {
         left: "right",
         right: "left",
         bottom: "top",
         top: "bottom"
     },
-    $t = {
+    Vt = {
         start: "end",
         end: "start"
     };
 
-function lt(t, e, o) {
+function ft(t, e, o) {
     return L(t, I(e, o))
 }
 
 function tt(t, e) {
     return typeof t == "function" ? t(e) : t
 }
 
@@ -32,46 +32,46 @@
     return t.split("-")[0]
 }
 
 function M(t) {
     return t.split("-")[1]
 }
 
-function ft(t) {
+function at(t) {
     return t === "x" ? "y" : "x"
 }
 
-function at(t) {
+function ut(t) {
     return t === "y" ? "height" : "width"
 }
 
 function it(t) {
     return ["top", "bottom"].includes(k(t)) ? "y" : "x"
 }
 
-function ut(t) {
-    return ft(it(t))
+function mt(t) {
+    return at(it(t))
 }
 
-function mt(t, e, o) {
+function dt(t, e, o) {
     o === void 0 && (o = !1);
     let n = M(t),
-        i = ut(t),
-        r = at(i),
+        i = mt(t),
+        r = ut(i),
         s = i === "x" ? n === (o ? "end" : "start") ? "right" : "left" : n === "start" ? "bottom" : "top";
     return e.reference[r] > e.floating[r] && (s = J(s)), [s, J(s)]
 }
 
-function xt(t) {
+function wt(t) {
     let e = J(t);
     return [G(t), e, G(e)]
 }
 
 function G(t) {
-    return t.replace(/start|end/g, e => $t[e])
+    return t.replace(/start|end/g, e => Vt[e])
 }
 
 function zt(t, e, o) {
     let n = ["left", "right"],
         i = ["right", "left"],
         r = ["top", "bottom"],
         s = ["bottom", "top"];
@@ -83,22 +83,22 @@
         case "right":
             return e ? r : s;
         default:
             return []
     }
 }
 
-function wt(t, e, o, n) {
+function xt(t, e, o, n) {
     let i = M(t),
         r = zt(k(t), o === "start", n);
     return i && (r = r.map(s => s + "-" + i), e && (r = r.concat(r.map(G)))), r
 }
 
 function J(t) {
-    return t.replace(/left|right|bottom|top/g, e => Vt[e])
+    return t.replace(/left|right|bottom|top/g, e => $t[e])
 }
 
 function _t(t) {
     return {
         top: 0,
         right: 0,
         bottom: 0,
@@ -113,28 +113,37 @@
         right: t,
         bottom: t,
         left: t
     }
 }
 
 function W(t) {
-    return {
-        ...t,
-        top: t.y,
-        left: t.x,
-        right: t.x + t.width,
-        bottom: t.y + t.height
+    let {
+        x: e,
+        y: o,
+        width: n,
+        height: i
+    } = t;
+    return {
+        width: n,
+        height: i,
+        top: o,
+        left: e,
+        right: e + n,
+        bottom: o + i,
+        x: e,
+        y: o
     }
 }
 
 function vt(t, e, o) {
     let {
         reference: n,
         floating: i
-    } = t, r = it(e), s = ut(e), c = at(s), f = k(e), l = r === "y", u = n.x + n.width / 2 - i.width / 2, a = n.y + n.height / 2 - i.height / 2, h = n[c] / 2 - i[c] / 2, m;
+    } = t, r = it(e), s = mt(e), c = ut(s), f = k(e), l = r === "y", u = n.x + n.width / 2 - i.width / 2, a = n.y + n.height / 2 - i.height / 2, h = n[c] / 2 - i[c] / 2, m;
     switch (f) {
         case "top":
             m = {
                 x: u,
                 y: n.y - i.height
             };
             break;
@@ -181,18 +190,18 @@
     } = o, c = r.filter(Boolean), f = await (s.isRTL == null ? void 0 : s.isRTL(e)), l = await s.getElementRects({
         reference: t,
         floating: e,
         strategy: i
     }), {
         x: u,
         y: a
-    } = vt(l, n, f), h = n, m = {}, w = 0;
+    } = vt(l, n, f), h = n, m = {}, x = 0;
     for (let g = 0; g < c.length; g++) {
         let {
-            name: x,
+            name: w,
             fn: d
         } = c[g], {
             x: p,
             y,
             data: b,
             reset: v
         } = await d({
@@ -207,19 +216,19 @@
             elements: {
                 reference: t,
                 floating: e
             }
         });
         u = p ?? u, a = y ?? a, m = {
             ...m,
-            [x]: {
-                ...m[x],
+            [w]: {
+                ...m[w],
                 ...b
             }
-        }, v && w <= 50 && (w++, typeof v == "object" && (v.placement && (h = v.placement), v.rects && (l = v.rects === !0 ? await s.getElementRects({
+        }, v && x <= 50 && (x++, typeof v == "object" && (v.placement && (h = v.placement), v.rects && (l = v.rects === !0 ? await s.getElementRects({
             reference: t,
             floating: e,
             strategy: i
         }) : v.rects), {
             x: u,
             y: a
         } = vt(l, h, f)), g = -1)
@@ -228,15 +237,15 @@
         x: u,
         y: a,
         placement: h,
         strategy: i,
         middlewareData: m
     }
 };
-async function dt(t, e) {
+async function st(t, e) {
     var o;
     e === void 0 && (e = {});
     let {
         x: n,
         y: i,
         platform: r,
         rects: s,
@@ -244,40 +253,41 @@
         strategy: f
     } = t, {
         boundary: l = "clippingAncestors",
         rootBoundary: u = "viewport",
         elementContext: a = "floating",
         altBoundary: h = !1,
         padding: m = 0
-    } = tt(e, t), w = yt(m), x = c[h ? a === "floating" ? "reference" : "floating" : a], d = W(await r.getClippingRect({
-        element: (o = await (r.isElement == null ? void 0 : r.isElement(x))) == null || o ? x : x.contextElement || await (r.getDocumentElement == null ? void 0 : r.getDocumentElement(c.floating)),
+    } = tt(e, t), x = yt(m), w = c[h ? a === "floating" ? "reference" : "floating" : a], d = W(await r.getClippingRect({
+        element: (o = await (r.isElement == null ? void 0 : r.isElement(w))) == null || o ? w : w.contextElement || await (r.getDocumentElement == null ? void 0 : r.getDocumentElement(c.floating)),
         boundary: l,
         rootBoundary: u,
         strategy: f
     })), p = a === "floating" ? {
-        ...s.floating,
         x: n,
-        y: i
+        y: i,
+        width: s.floating.width,
+        height: s.floating.height
     } : s.reference, y = await (r.getOffsetParent == null ? void 0 : r.getOffsetParent(c.floating)), b = await (r.isElement == null ? void 0 : r.isElement(y)) ? await (r.getScale == null ? void 0 : r.getScale(y)) || {
         x: 1,
         y: 1
     } : {
         x: 1,
         y: 1
     }, v = W(r.convertOffsetParentRelativeRectToViewportRelativeRect ? await r.convertOffsetParentRelativeRectToViewportRelativeRect({
         elements: c,
         rect: p,
         offsetParent: y,
         strategy: f
     }) : p);
     return {
-        top: (d.top - v.top + w.top) / b.y,
-        bottom: (v.bottom - d.bottom + w.bottom) / b.y,
-        left: (d.left - v.left + w.left) / b.x,
-        right: (v.right - d.right + w.right) / b.x
+        top: (d.top - v.top + x.top) / b.y,
+        bottom: (v.bottom - d.bottom + x.bottom) / b.y,
+        left: (d.left - v.left + x.left) / b.x,
+        right: (v.right - d.right + x.right) / b.x
     }
 }
 
 function It(t, e, o) {
     return (t ? [...o.filter(i => M(i) === t), ...o.filter(i => M(i) !== t)] : o.filter(i => k(i) === i)).filter(i => t ? M(i) === t || (e ? G(i) !== i : !1) : !0)
 }
 var At = function(t) {
@@ -291,26 +301,26 @@
                     middlewareData: s,
                     placement: c,
                     platform: f,
                     elements: l
                 } = e, {
                     crossAxis: u = !1,
                     alignment: a,
-                    allowedPlacements: h = ct,
+                    allowedPlacements: h = lt,
                     autoAlignment: m = !0,
-                    ...w
-                } = tt(t, e), g = a !== void 0 || h === ct ? It(a || null, m, h) : h, x = await dt(e, w), d = ((o = s.autoPlacement) == null ? void 0 : o.index) || 0, p = g[d];
+                    ...x
+                } = tt(t, e), g = a !== void 0 || h === lt ? It(a || null, m, h) : h, w = await st(e, x), d = ((o = s.autoPlacement) == null ? void 0 : o.index) || 0, p = g[d];
                 if (p == null) return {};
-                let y = mt(p, r, await (f.isRTL == null ? void 0 : f.isRTL(l.floating)));
+                let y = dt(p, r, await (f.isRTL == null ? void 0 : f.isRTL(l.floating)));
                 if (c !== p) return {
                     reset: {
                         placement: g[0]
                     }
                 };
-                let b = [x[k(p)], x[y[0]], x[y[1]]],
+                let b = [w[k(p)], w[y[0]], w[y[1]]],
                     v = [...((n = s.autoPlacement) == null ? void 0 : n.overflows) || [], {
                         placement: p,
                         overflows: b
                     }],
                     E = g[d + 1];
                 if (E) return {
                     data: {
@@ -352,53 +362,53 @@
                     platform: f,
                     elements: l
                 } = e, {
                     mainAxis: u = !0,
                     crossAxis: a = !0,
                     fallbackPlacements: h,
                     fallbackStrategy: m = "bestFit",
-                    fallbackAxisSideDirection: w = "none",
+                    fallbackAxisSideDirection: x = "none",
                     flipAlignment: g = !0,
-                    ...x
+                    ...w
                 } = tt(t, e);
                 if ((o = r.arrow) != null && o.alignmentOffset) return {};
                 let d = k(i),
                     p = k(c) === c,
                     y = await (f.isRTL == null ? void 0 : f.isRTL(l.floating)),
-                    b = h || (p || !g ? [J(c)] : xt(c));
-                !h && w !== "none" && b.push(...wt(c, g, w, y));
+                    b = h || (p || !g ? [J(c)] : wt(c));
+                !h && x !== "none" && b.push(...xt(c, g, x, y));
                 let v = [c, ...b],
-                    E = await dt(e, x),
+                    E = await st(e, w),
                     N = [],
-                    $ = ((n = r.flip) == null ? void 0 : n.overflows) || [];
+                    V = ((n = r.flip) == null ? void 0 : n.overflows) || [];
                 if (u && N.push(E[d]), a) {
-                    let P = mt(i, s, y);
+                    let P = dt(i, s, y);
                     N.push(E[P[0]], E[P[1]])
                 }
-                if ($ = [...$, {
+                if (V = [...V, {
                         placement: i,
                         overflows: N
                     }], !N.every(P => P <= 0)) {
                     var q, O;
                     let P = (((q = r.flip) == null ? void 0 : q.index) || 0) + 1,
                         ot = v[P];
                     if (ot) return {
                         data: {
                             index: P,
-                            overflows: $
+                            overflows: V
                         },
                         reset: {
                             placement: ot
                         }
                     };
-                    let K = (O = $.filter(z => z.overflows[0] <= 0).sort((z, _) => z.overflows[1] - _.overflows[1])[0]) == null ? void 0 : O.placement;
+                    let K = (O = V.filter(z => z.overflows[0] <= 0).sort((z, _) => z.overflows[1] - _.overflows[1])[0]) == null ? void 0 : O.placement;
                     if (!K) switch (m) {
                         case "bestFit": {
                             var F;
-                            let z = (F = $.map(_ => [_.placement, _.overflows.filter(U => U > 0).reduce((U, Ht) => U + Ht, 0)]).sort((_, U) => _[1] - U[1])[0]) == null ? void 0 : F[0];
+                            let z = (F = V.map(_ => [_.placement, _.overflows.filter(U => U > 0).reduce((U, Ht) => U + Ht, 0)]).sort((_, U) => _[1] - U[1])[0]) == null ? void 0 : F[0];
                             z && (K = z);
                             break
                         }
                         case "initialPlacement":
                             K = c;
                             break
                     }
@@ -421,48 +431,48 @@
                 x: o,
                 y: n,
                 placement: i
             } = e, {
                 mainAxis: r = !0,
                 crossAxis: s = !1,
                 limiter: c = {
-                    fn: x => {
+                    fn: w => {
                         let {
                             x: d,
                             y: p
-                        } = x;
+                        } = w;
                         return {
                             x: d,
                             y: p
                         }
                     }
                 },
                 ...f
             } = tt(t, e), l = {
                 x: o,
                 y: n
-            }, u = await dt(e, f), a = it(k(i)), h = ft(a), m = l[h], w = l[a];
+            }, u = await st(e, f), a = it(k(i)), h = at(a), m = l[h], x = l[a];
             if (r) {
-                let x = h === "y" ? "top" : "left",
+                let w = h === "y" ? "top" : "left",
                     d = h === "y" ? "bottom" : "right",
-                    p = m + u[x],
+                    p = m + u[w],
                     y = m - u[d];
-                m = lt(p, m, y)
+                m = ft(p, m, y)
             }
             if (s) {
-                let x = a === "y" ? "top" : "left",
+                let w = a === "y" ? "top" : "left",
                     d = a === "y" ? "bottom" : "right",
-                    p = w + u[x],
-                    y = w - u[d];
-                w = lt(p, w, y)
+                    p = x + u[w],
+                    y = x - u[d];
+                x = ft(p, x, y)
             }
             let g = c.fn({
                 ...e,
                 [h]: m,
-                [a]: w
+                [a]: x
             });
             return {
                 ...g,
                 data: {
                     x: g.x - o,
                     y: g.y - n
                 }
@@ -511,30 +521,30 @@
     return /auto|scroll|overlay|hidden|clip/.test(e + n + o) && !["inline", "contents"].includes(i)
 }
 
 function St(t) {
     return ["table", "td", "th"].includes(B(t))
 }
 
-function st(t) {
-    let e = rt(),
+function rt(t) {
+    let e = ct(),
         o = R(t);
     return o.transform !== "none" || o.perspective !== "none" || (o.containerType ? o.containerType !== "normal" : !1) || !e && (o.backdropFilter ? o.backdropFilter !== "none" : !1) || !e && (o.filter ? o.filter !== "none" : !1) || ["transform", "perspective", "filter"].some(n => (o.willChange || "").includes(n)) || ["paint", "layout", "strict", "content"].some(n => (o.contain || "").includes(n))
 }
 
 function Tt(t) {
     let e = H(t);
     for (; C(e) && !et(e);) {
-        if (st(e)) return e;
+        if (rt(e)) return e;
         e = H(e)
     }
     return null
 }
 
-function rt() {
+function ct() {
     return typeof CSS > "u" || !CSS.supports ? !1 : CSS.supports("-webkit-backdrop-filter", "none")
 }
 
 function et(t) {
     return ["html", "body", "#document"].includes(B(t))
 }
 
@@ -607,47 +617,47 @@
         y: c
     }
 }
 var Yt = D(0);
 
 function Mt(t) {
     let e = A(t);
-    return !rt() || !e.visualViewport ? Yt : {
+    return !ct() || !e.visualViewport ? Yt : {
         x: e.visualViewport.offsetLeft,
         y: e.visualViewport.offsetTop
     }
 }
 
 function jt(t, e, o) {
     return e === void 0 && (e = !1), !o || e && o !== A(t) ? !1 : e
 }
 
-function V(t, e, o, n) {
+function $(t, e, o, n) {
     e === void 0 && (e = !1), o === void 0 && (o = !1);
     let i = t.getBoundingClientRect(),
         r = gt(t),
         s = D(1);
     e && (n ? T(n) && (s = X(n)) : s = X(t));
     let c = jt(r, o, n) ? Mt(r) : D(0),
         f = (i.left + c.x) / s.x,
         l = (i.top + c.y) / s.y,
         u = i.width / s.x,
         a = i.height / s.y;
     if (r) {
         let h = A(r),
             m = n && T(n) ? A(n) : n,
-            w = h,
-            g = w.frameElement;
-        for (; g && n && m !== w;) {
-            let x = X(g),
+            x = h,
+            g = x.frameElement;
+        for (; g && n && m !== x;) {
+            let w = X(g),
                 d = g.getBoundingClientRect(),
                 p = R(g),
-                y = d.left + (g.clientLeft + parseFloat(p.paddingLeft)) * x.x,
-                b = d.top + (g.clientTop + parseFloat(p.paddingTop)) * x.y;
-            f *= x.x, l *= x.y, u *= x.x, a *= x.y, f += y, l += b, w = A(g), g = w.frameElement
+                y = d.left + (g.clientLeft + parseFloat(p.paddingLeft)) * w.x,
+                b = d.top + (g.clientTop + parseFloat(p.paddingTop)) * w.y;
+            f *= w.x, l *= w.y, u *= w.x, a *= w.y, f += y, l += b, x = A(g), g = x.frameElement
         }
     }
     return W({
         width: u,
         height: a,
         x: f,
         y: l
@@ -677,15 +687,15 @@
             scrollLeft: 0,
             scrollTop: 0
         },
         l = D(1),
         u = D(0),
         a = C(n);
     if ((a || !a && !r) && ((B(n) !== "body" || j(s)) && (f = nt(n)), C(n))) {
-        let h = V(n);
+        let h = $(n);
         l = X(n), u.x = h.x + n.clientLeft, u.y = h.y + n.clientTop
     }
     return {
         width: o.width * l.x,
         height: o.height * l.y,
         x: o.x * l.x - f.scrollLeft * l.x + u.x,
         y: o.y * l.y - f.scrollTop * l.y + u.y
@@ -693,15 +703,15 @@
 }
 
 function Kt(t) {
     return Array.from(t.getClientRects())
 }
 
 function Ft(t) {
-    return V(S(t)).left + nt(t).scrollLeft
+    return $(S(t)).left + nt(t).scrollLeft
 }
 
 function Ut(t) {
     let e = S(t),
         o = nt(t),
         n = t.ownerDocument.body,
         i = L(e.scrollWidth, e.clientWidth, n.scrollWidth, n.clientWidth),
@@ -722,27 +732,27 @@
         i = o.visualViewport,
         r = n.clientWidth,
         s = n.clientHeight,
         c = 0,
         f = 0;
     if (i) {
         r = i.width, s = i.height;
-        let l = rt();
+        let l = ct();
         (!l || l && e === "fixed") && (c = i.offsetLeft, f = i.offsetTop)
     }
     return {
         width: r,
         height: s,
         x: c,
         y: f
     }
 }
 
 function Jt(t, e) {
-    let o = V(t, !0, e === "fixed"),
+    let o = $(t, !0, e === "fixed"),
         n = o.top + t.clientTop,
         i = o.left + t.clientLeft,
         r = C(t) ? X(t) : D(1),
         s = t.clientWidth * r.x,
         c = t.clientHeight * r.y,
         f = i * r.x,
         l = n * r.y;
@@ -780,15 +790,15 @@
     if (o) return o;
     let n = Y(t, [], !1).filter(c => T(c) && B(c) !== "body"),
         i = null,
         r = R(t).position === "fixed",
         s = r ? H(t) : t;
     for (; T(s) && !et(s);) {
         let c = R(s),
-            f = st(s);
+            f = rt(s);
         !f && c.position === "fixed" && (i = null), (r ? !f && !i : !f && c.position === "static" && !!i && ["absolute", "fixed"].includes(i.position) || j(s) && !f && Nt(t, s)) ? n = n.filter(u => u !== s) : i = c, s = H(s)
     }
     return e.set(t, n), n
 }
 
 function Zt(t) {
     let {
@@ -819,23 +829,23 @@
     }
 }
 
 function ee(t, e, o) {
     let n = C(e),
         i = S(e),
         r = o === "fixed",
-        s = V(t, !0, r, e),
+        s = $(t, !0, r, e),
         c = {
             scrollLeft: 0,
             scrollTop: 0
         },
         f = D(0);
     if (n || !n && !r)
         if ((B(e) !== "body" || j(i)) && (c = nt(e)), n) {
-            let a = V(e, !0, r, e);
+            let a = $(e, !0, r, e);
             f.x = a.x + e.clientLeft, f.y = a.y + e.clientTop
         } else i && (f.x = Ft(i));
     let l = s.left + c.scrollLeft - f.x,
         u = s.top + c.scrollTop - f.y;
     return {
         x: l,
         y: u,
@@ -849,25 +859,27 @@
 }
 
 function Wt(t, e) {
     let o = A(t);
     if (!C(t) || Bt(t)) return o;
     let n = Dt(t, e);
     for (; n && St(n) && R(n).position === "static";) n = Dt(n, e);
-    return n && (B(n) === "html" || B(n) === "body" && R(n).position === "static" && !st(n)) ? o : n || Tt(t) || o
+    return n && (B(n) === "html" || B(n) === "body" && R(n).position === "static" && !rt(n)) ? o : n || Tt(t) || o
 }
 var ne = async function(t) {
     let e = this.getOffsetParent || Wt,
-        o = this.getDimensions;
+        o = this.getDimensions,
+        n = await o(t.floating);
     return {
         reference: ee(t.reference, await e(t.floating), t.strategy),
         floating: {
             x: 0,
             y: 0,
-            ...await o(t.floating)
+            width: n.width,
+            height: n.height
         }
     }
 };
 
 function oe(t) {
     return R(t).direction === "rtl"
 }
@@ -899,30 +911,30 @@
             left: l,
             top: u,
             width: a,
             height: h
         } = t.getBoundingClientRect();
         if (c || e(), !a || !h) return;
         let m = Z(u),
-            w = Z(i.clientWidth - (l + a)),
+            x = Z(i.clientWidth - (l + a)),
             g = Z(i.clientHeight - (u + h)),
-            x = Z(l),
+            w = Z(l),
             p = {
-                rootMargin: -m + "px " + -w + "px " + -g + "px " + -x + "px",
+                rootMargin: -m + "px " + -x + "px " + -g + "px " + -w + "px",
                 threshold: L(0, I(1, f)) || 1
             },
             y = !0;
 
         function b(v) {
             let E = v[0].intersectionRatio;
             if (E !== f) {
                 if (!y) return s();
                 E ? s(!1, E) : n = setTimeout(() => {
                     s(!1, 1e-7)
-                }, 100)
+                }, 1e3)
             }
             y = !1
         }
         try {
             o = new IntersectionObserver(b, {
                 ...p,
                 root: i.ownerDocument
@@ -931,15 +943,15 @@
             o = new IntersectionObserver(b, p)
         }
         o.observe(t)
     }
     return s(!0), r
 }
 
-function ye(t, e, o, n) {
+function ve(t, e, o, n) {
     n === void 0 && (n = {});
     let {
         ancestorScroll: i = !0,
         ancestorResize: r = !0,
         elementResize: s = typeof ResizeObserver == "function",
         layoutShift: c = typeof IntersectionObserver == "function",
         animationFrame: f = !1
@@ -955,32 +967,32 @@
     s && (m = new ResizeObserver(d => {
         let [p] = d;
         p && p.target === l && m && (m.unobserve(e), cancelAnimationFrame(h), h = requestAnimationFrame(() => {
             var y;
             (y = m) == null || y.observe(e)
         })), o()
     }), l && !f && m.observe(l), m.observe(e));
-    let w, g = f ? V(t) : null;
-    f && x();
+    let x, g = f ? $(t) : null;
+    f && w();
 
-    function x() {
-        let d = V(t);
-        g && (d.x !== g.x || d.y !== g.y || d.width !== g.width || d.height !== g.height) && o(), g = d, w = requestAnimationFrame(x)
+    function w() {
+        let d = $(t);
+        g && (d.x !== g.x || d.y !== g.y || d.width !== g.width || d.height !== g.height) && o(), g = d, x = requestAnimationFrame(w)
     }
     return o(), () => {
         var d;
         u.forEach(p => {
             i && p.removeEventListener("scroll", o), r && p.removeEventListener("resize", o)
-        }), a == null || a(), (d = m) == null || d.disconnect(), m = null, f && cancelAnimationFrame(w)
+        }), a == null || a(), (d = m) == null || d.disconnect(), m = null, f && cancelAnimationFrame(x)
     }
 }
-var ve = At,
-    be = Rt,
-    Ae = Ot;
-var Oe = (t, e, o) => {
+var be = At,
+    Ae = Rt,
+    Oe = Ot;
+var Re = (t, e, o) => {
     let n = new Map,
         i = {
             platform: ie,
             ...o
         },
         r = {
             ...i.platform,
@@ -988,9 +1000,9 @@
         };
     return bt(t, e, {
         ...i,
         platform: r
     })
 };
 export {
-    ye as a, ve as b, be as c, Ae as d, Oe as e
+    ve as a, be as b, Ae as c, Oe as d, Re as e
 };
```

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-SERXULES.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-SERXULES.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/chunk-W5RPWA2M.js` & `django_formset-1.4.1/formset/static/formset/js/chunk-W5RPWA2M.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/static/formset/js/django-formset.js` & `django_formset-1.4.1/formset/static/formset/js/django-formset.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
 import {
     a as er,
     b as tr,
     c as rr,
     d as M,
     e as ot,
     f as lt
-} from "./chunk-EQH4AZSI.js";
+} from "./chunk-XQYS6DVW.js";
 import {
     a as it
 } from "./chunk-FDUUONAQ.js";
 import {
     a as st
 } from "./chunk-65OJRBX6.js";
 import {
@@ -63,29 +63,29 @@
         }(),
         gt = wr.toString,
         se = mt.hasOwnProperty,
         bt = mt.toString,
         Ar = RegExp("^" + gt.call(se).replace(hr, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
         dt = Te.Symbol,
         Tr = Er.splice,
-        Cr = vt(Te, "Map"),
+        Fr = vt(Te, "Map"),
         K = vt(Object, "create"),
         ut = dt ? dt.prototype : void 0,
         ht = ut ? ut.toString : void 0;
 
     function I(n) {
         var e = -1,
             t = n ? n.length : 0;
         for (this.clear(); ++e < t;) {
             var r = n[e];
             this.set(r[0], r[1])
         }
     }
 
-    function Fr() {
+    function Cr() {
         this.__data__ = K ? K(null) : {}
     }
 
     function jr(n) {
         return this.has(n) && delete this.__data__[n]
     }
 
@@ -103,15 +103,15 @@
         return K ? e[n] !== void 0 : se.call(e, n)
     }
 
     function Sr(n, e) {
         var t = this.__data__;
         return t[n] = K && e === void 0 ? ft : e, this
     }
-    I.prototype.clear = Fr;
+    I.prototype.clear = Cr;
     I.prototype.delete = jr;
     I.prototype.get = xr;
     I.prototype.has = Lr;
     I.prototype.set = Sr;
 
     function _(n) {
         var e = -1,
@@ -163,15 +163,15 @@
             this.set(r[0], r[1])
         }
     }
 
     function Ir() {
         this.__data__ = {
             hash: new I,
-            map: new(Cr || _),
+            map: new(Fr || _),
             string: new I
         }
     }
 
     function Or(n) {
         return le(this, n).delete(n)
     }
@@ -209,29 +209,29 @@
         var e = Yr(n) || yr(n) ? Ar : pr;
         return e.test(Qr(n))
     }
 
     function $r(n, e, t, r) {
         if (!ne(n)) return n;
         e = zr(e, n) ? [e] : Gr(e);
-        for (var i = -1, s = e.length, o = s - 1, f = n; f != null && ++i < s;) {
+        for (var i = -1, s = e.length, o = s - 1, u = n; u != null && ++i < s;) {
             var d = Jr(e[i]),
                 c = t;
             if (i != o) {
-                var l = f[d];
-                c = r ? r(l, d, f) : void 0, c === void 0 && (c = ne(l) ? l : Ur(e[i + 1]) ? [] : {})
+                var l = u[d];
+                c = r ? r(l, d, u) : void 0, c === void 0 && (c = ne(l) ? l : Ur(e[i + 1]) ? [] : {})
             }
-            _r(f, d, c), f = f[d]
+            _r(u, d, c), u = u[d]
         }
         return n
     }
 
     function Nr(n) {
         if (typeof n == "string") return n;
-        if (Fe(n)) return ht ? ht.call(n) : "";
+        if (Ce(n)) return ht ? ht.call(n) : "";
         var e = n + "";
         return e == "0" && 1 / n == -pt ? "-0" : e
     }
 
     function Gr(n) {
         return Et(n) ? n : Xr(n)
     }
@@ -249,35 +249,35 @@
     function Ur(n, e) {
         return e = e ?? nr, !!e && (typeof n == "number" || mr.test(n)) && n > -1 && n % 1 == 0 && n < e
     }
 
     function zr(n, e) {
         if (Et(n)) return !1;
         var t = typeof n;
-        return t == "number" || t == "symbol" || t == "boolean" || n == null || Fe(n) ? !0 : cr.test(n) || !ar.test(n) || e != null && n in Object(e)
+        return t == "number" || t == "symbol" || t == "boolean" || n == null || Ce(n) ? !0 : cr.test(n) || !ar.test(n) || e != null && n in Object(e)
     }
 
     function Wr(n) {
         var e = typeof n;
         return e == "string" || e == "number" || e == "symbol" || e == "boolean" ? n !== "__proto__" : n === null
     }
 
     function Kr(n) {
         return !!ct && ct in n
     }
-    var Xr = Ce(function(n) {
+    var Xr = Fe(function(n) {
         n = ei(n);
         var e = [];
         return dr.test(n) && e.push(""), n.replace(ur, function(t, r, i, s) {
             e.push(i ? s.replace(fr, "$1") : r || t)
         }), e
     });
 
     function Jr(n) {
-        if (typeof n == "string" || Fe(n)) return n;
+        if (typeof n == "string" || Ce(n)) return n;
         var e = n + "";
         return e == "0" && 1 / n == -pt ? "-0" : e
     }
 
     function Qr(n) {
         if (n != null) {
             try {
@@ -286,27 +286,27 @@
             try {
                 return n + ""
             } catch {}
         }
         return ""
     }
 
-    function Ce(n, e) {
+    function Fe(n, e) {
         if (typeof n != "function" || e && typeof e != "function") throw new TypeError(ir);
         var t = function() {
             var r = arguments,
                 i = e ? e.apply(this, r) : r[0],
                 s = t.cache;
             if (s.has(i)) return s.get(i);
             var o = n.apply(this, r);
             return t.cache = s.set(i, o), o
         };
-        return t.cache = new(Ce.Cache || O), t
+        return t.cache = new(Fe.Cache || O), t
     }
-    Ce.Cache = O;
+    Fe.Cache = O;
 
     function yt(n, e) {
         return n === e || n !== n && e !== e
     }
     var Et = Array.isArray;
 
     function Yr(n) {
@@ -319,86 +319,86 @@
         return !!n && (e == "object" || e == "function")
     }
 
     function Zr(n) {
         return !!n && typeof n == "object"
     }
 
-    function Fe(n) {
+    function Ce(n) {
         return typeof n == "symbol" || Zr(n) && bt.call(n) == lr
     }
 
     function ei(n) {
         return n == null ? "" : Nr(n)
     }
 
     function ti(n, e, t) {
         return n == null ? n : $r(n, e, t)
     }
     wt.exports = ti
 });
 (function() {
     "use strict";
-    var n = function(u, a) {
-        var h = function(y) {
+    var n = function(h, a) {
+        var f = function(y) {
                 for (var g = 0, v = y.length; g < v; g++) p(y[g])
             },
             p = function(y) {
                 var g = y.target,
                     v = y.attributeName,
                     w = y.oldValue;
                 g.attributeChangedCallback(v, w, g.getAttribute(v))
             };
         return function(m, y) {
             var g = m.constructor.observedAttributes;
-            return g && u(y).then(function() {
-                new a(h).observe(m, {
+            return g && h(y).then(function() {
+                new a(f).observe(m, {
                     attributes: !0,
                     attributeOldValue: !0,
                     attributeFilter: g
                 });
                 for (var v = 0, w = g.length; v < w; v++) m.hasAttribute(g[v]) && p({
                     target: m,
                     attributeName: g[v],
                     oldValue: null
                 })
             }), m
         }
     };
 
-    function e(u, a) {
-        if (u) {
-            if (typeof u == "string") return t(u, a);
-            var h = Object.prototype.toString.call(u).slice(8, -1);
-            if (h === "Object" && u.constructor && (h = u.constructor.name), h === "Map" || h === "Set") return Array.from(u);
-            if (h === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(h)) return t(u, a)
+    function e(h, a) {
+        if (h) {
+            if (typeof h == "string") return t(h, a);
+            var f = Object.prototype.toString.call(h).slice(8, -1);
+            if (f === "Object" && h.constructor && (f = h.constructor.name), f === "Map" || f === "Set") return Array.from(h);
+            if (f === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(f)) return t(h, a)
         }
     }
 
-    function t(u, a) {
-        (a == null || a > u.length) && (a = u.length);
-        for (var h = 0, p = new Array(a); h < a; h++) p[h] = u[h];
+    function t(h, a) {
+        (a == null || a > h.length) && (a = h.length);
+        for (var f = 0, p = new Array(a); f < a; f++) p[f] = h[f];
         return p
     }
 
-    function r(u, a) {
-        var h = typeof Symbol < "u" && u[Symbol.iterator] || u["@@iterator"];
-        if (!h) {
-            if (Array.isArray(u) || (h = e(u)) || a && u && typeof u.length == "number") {
-                h && (u = h);
+    function r(h, a) {
+        var f = typeof Symbol < "u" && h[Symbol.iterator] || h["@@iterator"];
+        if (!f) {
+            if (Array.isArray(h) || (f = e(h)) || a && h && typeof h.length == "number") {
+                f && (h = f);
                 var p = 0,
                     m = function() {};
                 return {
                     s: m,
                     n: function() {
-                        return p >= u.length ? {
+                        return p >= h.length ? {
                             done: !0
                         } : {
                             done: !1,
-                            value: u[p++]
+                            value: h[p++]
                         }
                     },
                     e: function(w) {
                         throw w
                     },
                     f: m
                 }
@@ -407,124 +407,124 @@
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
         }
         var y = !0,
             g = !1,
             v;
         return {
             s: function() {
-                h = h.call(u)
+                f = f.call(h)
             },
             n: function() {
-                var w = h.next();
+                var w = f.next();
                 return y = w.done, w
             },
             e: function(w) {
                 g = !0, v = w
             },
             f: function() {
                 try {
-                    !y && h.return != null && h.return()
+                    !y && f.return != null && f.return()
                 } finally {
                     if (g) throw v
                 }
             }
         }
     }
     var i = !0,
         s = !1,
         o = "querySelectorAll",
-        f = function(a) {
-            var h = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : document,
+        u = function(a) {
+            var f = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : document,
                 p = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : MutationObserver,
                 m = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : ["*"],
-                y = function w(P, H, C, b, E, A) {
-                    var F = r(P),
+                y = function w(P, H, F, b, E, A) {
+                    var C = r(P),
                         q;
                     try {
-                        for (F.s(); !(q = F.n()).done;) {
+                        for (C.s(); !(q = C.n()).done;) {
                             var T = q.value;
-                            (A || o in T) && (E ? C.has(T) || (C.add(T), b.delete(T), a(T, E)) : b.has(T) || (b.add(T), C.delete(T), a(T, E)), A || w(T[o](H), H, C, b, E, i))
+                            (A || o in T) && (E ? F.has(T) || (F.add(T), b.delete(T), a(T, E)) : b.has(T) || (b.add(T), F.delete(T), a(T, E)), A || w(T[o](H), H, F, b, E, i))
                         }
                     } catch (we) {
-                        F.e(we)
+                        C.e(we)
                     } finally {
-                        F.f()
+                        C.f()
                     }
                 },
                 g = new p(function(w) {
                     if (m.length) {
                         var P = m.join(","),
                             H = new Set,
-                            C = new Set,
+                            F = new Set,
                             b = r(w),
                             E;
                         try {
                             for (b.s(); !(E = b.n()).done;) {
                                 var A = E.value,
-                                    F = A.addedNodes,
+                                    C = A.addedNodes,
                                     q = A.removedNodes;
-                                y(q, P, H, C, s, s), y(F, P, H, C, i, s)
+                                y(q, P, H, F, s, s), y(C, P, H, F, i, s)
                             }
                         } catch (T) {
                             b.e(T)
                         } finally {
                             b.f()
                         }
                     }
                 }),
                 v = g.observe;
             return (g.observe = function(w) {
                 return v.call(g, w, {
                     subtree: i,
                     childList: i
                 })
-            })(h), g
+            })(f), g
         },
         d = "querySelectorAll",
         c = self,
         l = c.document,
         k = c.Element,
         G = c.MutationObserver,
         Mt = c.Set,
         Dt = c.WeakMap,
         He = function(a) {
             return d in a
         },
         Ie = [].filter,
-        fe = function(u) {
+        fe = function(h) {
             var a = new Dt,
-                h = function(b) {
+                f = function(b) {
                     for (var E = 0, A = b.length; E < A; E++) a.delete(b[E])
                 },
                 p = function() {
                     for (var b = P.takeRecords(), E = 0, A = b.length; E < A; E++) g(Ie.call(b[E].removedNodes, He), !1), g(Ie.call(b[E].addedNodes, He), !0)
                 },
                 m = function(b) {
                     return b.matches || b.webkitMatchesSelector || b.msMatchesSelector
                 },
                 y = function(b, E) {
                     var A;
                     if (E)
-                        for (var F, q = m(b), T = 0, we = v.length; T < we; T++) q.call(b, F = v[T]) && (a.has(b) || a.set(b, new Mt), A = a.get(b), A.has(F) || (A.add(F), u.handle(b, E, F)));
+                        for (var C, q = m(b), T = 0, we = v.length; T < we; T++) q.call(b, C = v[T]) && (a.has(b) || a.set(b, new Mt), A = a.get(b), A.has(C) || (A.add(C), h.handle(b, E, C)));
                     else a.has(b) && (A = a.get(b), a.delete(b), A.forEach(function(Yt) {
-                        u.handle(b, E, Yt)
+                        h.handle(b, E, Yt)
                     }))
                 },
                 g = function(b) {
-                    for (var E = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0, A = 0, F = b.length; A < F; A++) y(b[A], E)
+                    for (var E = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !0, A = 0, C = b.length; A < C; A++) y(b[A], E)
                 },
-                v = u.query,
-                w = u.root || l,
-                P = f(y, w, G, v),
+                v = h.query,
+                w = h.root || l,
+                P = u(y, w, G, v),
                 H = k.prototype.attachShadow;
-            return H && (k.prototype.attachShadow = function(C) {
-                var b = H.call(this, C);
+            return H && (k.prototype.attachShadow = function(F) {
+                var b = H.call(this, F);
                 return P.observe(b), b
             }), v.length && g(w[d](v)), {
-                drop: h,
+                drop: f,
                 flush: p,
                 observer: P,
                 parse: g
             }
         },
         j = self,
         x = j.document,
@@ -541,122 +541,122 @@
         It = j.Reflect,
         J = X.defineProperty,
         Ot = X.keys,
         Rt = X.getOwnPropertyNames,
         U = X.setPrototypeOf,
         z = !self.customElements,
         $e = function(a) {
-            for (var h = Ot(a), p = [], m = new Re, y = h.length, g = 0; g < y; g++) {
-                p[g] = a[h[g]];
+            for (var f = Ot(a), p = [], m = new Re, y = f.length, g = 0; g < y; g++) {
+                p[g] = a[f[g]];
                 try {
-                    delete a[h[g]]
+                    delete a[f[g]]
                 } catch {
                     m.add(g)
                 }
             }
             return function() {
-                for (var v = 0; v < y; v++) m.has(v) || (a[h[v]] = p[v])
+                for (var v = 0; v < y; v++) m.has(v) || (a[f[v]] = p[v])
             }
         };
     if (z) {
         var pe = function() {
                 var a = this.constructor;
                 if (!me.has(a)) throw new Ve("Illegal constructor");
-                var h = me.get(a);
-                if (Y) return ze(Y, h);
-                var p = Ne.call(x, h);
-                return ze(U(p, a.prototype), h)
+                var f = me.get(a);
+                if (Y) return ze(Y, f);
+                var p = Ne.call(x, f);
+                return ze(U(p, a.prototype), f)
             },
             Ne = x.createElement,
             me = new D,
             Q = new D,
             Ge = new D,
             W = new D,
             Ue = [],
-            qt = function(a, h, p) {
+            qt = function(a, f, p) {
                 var m = Ge.get(p);
-                if (h && !m.isPrototypeOf(a)) {
+                if (f && !m.isPrototypeOf(a)) {
                     var y = $e(a);
                     Y = U(a, m);
                     try {
                         new m.constructor
                     } finally {
                         Y = null, y()
                     }
                 }
-                var g = "".concat(h ? "" : "dis", "connectedCallback");
+                var g = "".concat(f ? "" : "dis", "connectedCallback");
                 g in m && a[g]()
             },
             Bt = fe({
                 query: Ue,
                 handle: qt
             }),
             _t = Bt.parse,
             Y = null,
             ge = function(a) {
                 if (!Q.has(a)) {
-                    var h, p = new Promise(function(m) {
-                        h = m
+                    var f, p = new Promise(function(m) {
+                        f = m
                     });
                     Q.set(a, {
                         $: p,
-                        _: h
+                        _: f
                     })
                 }
                 return Q.get(a).$
             },
             ze = n(ge, Oe);
         self.customElements = {
-            define: function(a, h) {
+            define: function(a, f) {
                 if (W.has(a)) throw new _e('the name "'.concat(a, '" has already been used with this registry'));
-                me.set(h, a), Ge.set(a, h.prototype), W.set(a, h), Ue.push(a), ge(a).then(function() {
+                me.set(f, a), Ge.set(a, f.prototype), W.set(a, f), Ue.push(a), ge(a).then(function() {
                     _t(x.querySelectorAll(a))
-                }), Q.get(a)._(h)
+                }), Q.get(a)._(f)
             },
             get: function(a) {
                 return W.get(a)
             },
             whenDefined: ge
         }, J(pe.prototype = Ht.prototype, "constructor", {
             value: pe
-        }), self.HTMLElement = pe, x.createElement = function(u, a) {
-            var h = a && a.is,
-                p = h ? W.get(h) : W.get(u);
-            return p ? new p : Ne.call(x, u)
+        }), self.HTMLElement = pe, x.createElement = function(h, a) {
+            var f = a && a.is,
+                p = f ? W.get(f) : W.get(h);
+            return p ? new p : Ne.call(x, h)
         }, "isConnected" in Be.prototype || J(Be.prototype, "isConnected", {
             configurable: !0,
             get: function() {
                 return !(this.ownerDocument.compareDocumentPosition(this) & this.DOCUMENT_POSITION_DISCONNECTED)
             }
         })
     } else if (z = !self.customElements.get("extends-br"), z) try {
-        var We = function u() {
-            return self.Reflect.construct(HTMLBRElement, [], u)
+        var We = function h() {
+            return self.Reflect.construct(HTMLBRElement, [], h)
         };
         We.prototype = HTMLLIElement.prototype;
         var Ke = "extends-br";
         self.customElements.define("extends-br", We, {
             extends: "br"
         }), z = x.createElement("br", {
             is: Ke
         }).outerHTML.indexOf(Ke) < 0;
         var Xe = self.customElements,
             Vt = Xe.get,
             $t = Xe.whenDefined;
-        self.customElements.whenDefined = function(u) {
+        self.customElements.whenDefined = function(h) {
             var a = this;
-            return $t.call(this, u).then(function(h) {
-                return h || Vt.call(a, u)
+            return $t.call(this, h).then(function(f) {
+                return f || Vt.call(a, h)
             })
         }
     } catch {}
     if (z) {
         var Je = function(a) {
-                var h = be.get(a);
-                tt(h.querySelectorAll(this), a.isConnected)
+                var f = be.get(a);
+                tt(f.querySelectorAll(this), a.isConnected)
             },
             L = self.customElements,
             Qe = x.createElement,
             Nt = L.define,
             Gt = L.get,
             Ut = L.upgrade,
             zt = It || {
@@ -672,111 +672,111 @@
             Ye = new D,
             te = new D,
             Ze = [],
             re = [],
             et = function(a) {
                 return te.get(a) || Gt.call(L, a)
             },
-            Kt = function(a, h, p) {
+            Kt = function(a, f, p) {
                 var m = Ye.get(p);
-                if (h && !m.isPrototypeOf(a)) {
+                if (f && !m.isPrototypeOf(a)) {
                     var y = $e(a);
                     ie = U(a, m);
                     try {
                         new m.constructor
                     } finally {
                         ie = null, y()
                     }
                 }
-                var g = "".concat(h ? "" : "dis", "connectedCallback");
+                var g = "".concat(f ? "" : "dis", "connectedCallback");
                 g in m && a[g]()
             },
             Xt = fe({
                 query: re,
                 handle: Kt
             }),
             tt = Xt.parse,
             Jt = fe({
                 query: Ze,
-                handle: function(a, h) {
-                    be.has(a) && (h ? ve.add(a) : ve.delete(a), re.length && Je.call(re, a))
+                handle: function(a, f) {
+                    be.has(a) && (f ? ve.add(a) : ve.delete(a), re.length && Je.call(re, a))
                 }
             }),
             Qt = Jt.parse,
             rt = qe.prototype.attachShadow;
-        rt && (qe.prototype.attachShadow = function(u) {
-            var a = rt.call(this, u);
+        rt && (qe.prototype.attachShadow = function(h) {
+            var a = rt.call(this, h);
             return be.set(this, a), a
         });
         var ye = function(a) {
                 if (!ee.has(a)) {
-                    var h, p = new Promise(function(m) {
-                        h = m
+                    var f, p = new Promise(function(m) {
+                        f = m
                     });
                     ee.set(a, {
                         $: p,
-                        _: h
+                        _: f
                     })
                 }
                 return ee.get(a).$
             },
             Ee = n(ye, Oe),
             ie = null;
-        Rt(self).filter(function(u) {
-            return /^HTML.*Element$/.test(u)
-        }).forEach(function(u) {
-            var a = self[u];
+        Rt(self).filter(function(h) {
+            return /^HTML.*Element$/.test(h)
+        }).forEach(function(h) {
+            var a = self[h];
 
-            function h() {
+            function f() {
                 var p = this.constructor;
                 if (!Z.has(p)) throw new Ve("Illegal constructor");
                 var m = Z.get(p),
                     y = m.is,
                     g = m.tag;
                 if (y) {
                     if (ie) return Ee(ie, y);
                     var v = Qe.call(x, g);
                     return v.setAttribute("is", y), Ee(U(v, p.prototype), y)
                 } else return Wt.call(this, a, [], p)
             }
-            J(h.prototype = a.prototype, "constructor", {
-                value: h
-            }), J(self, u, {
-                value: h
+            J(f.prototype = a.prototype, "constructor", {
+                value: f
+            }), J(self, h, {
+                value: f
             })
-        }), x.createElement = function(u, a) {
-            var h = a && a.is;
-            if (h) {
-                var p = te.get(h);
-                if (p && Z.get(p).tag === u) return new p
-            }
-            var m = Qe.call(x, u);
-            return h && m.setAttribute("is", h), m
-        }, L.get = et, L.whenDefined = ye, L.upgrade = function(u) {
-            var a = u.getAttribute("is");
+        }), x.createElement = function(h, a) {
+            var f = a && a.is;
+            if (f) {
+                var p = te.get(f);
+                if (p && Z.get(p).tag === h) return new p
+            }
+            var m = Qe.call(x, h);
+            return f && m.setAttribute("is", f), m
+        }, L.get = et, L.whenDefined = ye, L.upgrade = function(h) {
+            var a = h.getAttribute("is");
             if (a) {
-                var h = te.get(a);
-                if (h) {
-                    Ee(U(u, h.prototype), a);
+                var f = te.get(a);
+                if (f) {
+                    Ee(U(h, f.prototype), a);
                     return
                 }
             }
-            Ut.call(L, u)
-        }, L.define = function(u, a, h) {
-            if (et(u)) throw new _e("'".concat(u, "' has already been defined as a custom element"));
-            var p, m = h && h.extends;
+            Ut.call(L, h)
+        }, L.define = function(h, a, f) {
+            if (et(h)) throw new _e("'".concat(h, "' has already been defined as a custom element"));
+            var p, m = f && f.extends;
             Z.set(a, m ? {
-                is: u,
+                is: h,
                 tag: m
             } : {
                 is: "",
-                tag: u
-            }), m ? (p = "".concat(m, '[is="').concat(u, '"]'), Ye.set(p, a.prototype), te.set(u, a), re.push(p)) : (Nt.apply(L, arguments), Ze.push(p = u)), ye(u).then(function() {
+                tag: h
+            }), m ? (p = "".concat(m, '[is="').concat(h, '"]'), Ye.set(p, a.prototype), te.set(h, a), re.push(p)) : (Nt.apply(L, arguments), Ze.push(p = h)), ye(h).then(function() {
                 m ? (tt(x.querySelectorAll(p)), ve.forEach(Je, [p])) : Qt(x.querySelectorAll(p))
-            }), ee.get(u)._(a)
+            }), ee.get(h)._(a)
         }
     }
 })();
 var $ = B(er()),
     xt = B(At()),
     Pe = B(tr()),
     Lt = B(rr()),
@@ -826,21 +826,21 @@
                 }) : r()
             })
         }
         async uploadFile(e, t) {
             let r = this;
 
             function i(o) {
-                let f = o.lengthComputable ? o.loaded / o.total : 0;
-                r.progressBar && (r.progressBar.style.visibility = "visible", r.progressBar.value = .97 * f)
+                let u = o.lengthComputable ? o.loaded / o.total : 0;
+                r.progressBar && (r.progressBar.style.visibility = "visible", r.progressBar.value = .97 * u)
             }
             let s = new FormData;
-            return s.append("temp_file", e), s.append("image_height", t.toString()), new Promise((o, f) => {
+            return s.append("temp_file", e), s.append("image_height", t.toString()), new Promise((o, u) => {
                 function d() {
-                    r.progressBar && (r.progressBar.value = 1, window.setTimeout(() => r.progressBar.style.visibility = "hidden", 333)), c.status === 200 ? o(c.response) : f(c.response)
+                    r.progressBar && (r.progressBar.value = 1, window.setTimeout(() => r.progressBar.style.visibility = "hidden", 333)), c.status === 200 ? o(c.response) : u(c.response)
                 }
                 let c = new XMLHttpRequest;
                 r.progressBar && (c.addEventListener("loadstart", i), c.upload.addEventListener("progress", i, !1)), c.addEventListener("loadend", d), c.open("POST", this.fieldGroup.form.formset.endpoint, !0);
                 let l = this.fieldGroup.form.formset.CSRFToken;
                 l && c.setRequestHeader("X-CSRFToken", l), c.responseType = "json", c.send(s)
             })
         }
@@ -865,24 +865,24 @@
         inProgress() {
             return !!this.inputElement.files && this.inputElement.files.length > 0 && !this.uploadedFiles.length
         }
         resetToInitial() {
             this.uploadedFiles = this.initialData, this.renderDropbox()
         }
     };
-var Ct = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
+var Ft = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<g class="spinner">
 		<path style="stroke-width:0.729" d="m 12.73285,23.212276 -10e-7,-4.393157 A 0.27932072,0.27932072 0 0 0 12.27476,18.604602 l -2.6367848,2.196577 a 0.27932072,0.27932072 0 0 0 -10e-8,0.429037 l 2.6367859,2.196577 a 0.27932072,0.27932072 0 0 0 0.458089,-0.214517 z" />
 		<path style="stroke-width:0.729" d="m 11.298326,5.191792 -10e-7,-4.39315704 a 0.27932072,0.27932072 0 0 1 0.458086,-0.214519 L 14.393193,2.780699 a 0.27932072,0.27932072 0 0 1 2e-6,0.429033 l -2.636785,2.19658 a 0.27932072,0.27932072 0 0 1 -0.458084,-0.21452 z" />
 		<path style="fill:none;stroke:currentColor;stroke-width:2;stroke-linecap:round;stroke-miterlimit:10;stroke-dashoffset:89.339;stroke-dasharray:none" d="M 12.5,2.9179688 C 12.333705,2.9010187 12.166975,2.8886442 12,2.8808594 6.9635919,2.8807514 2.8807499,6.9635934 2.8808594,12 c 0.00661,2.530252 1.064217,4.944009 2.9199218,6.664062" />
 		<path style="fill:none;stroke:currentColor;stroke-width:2;stroke-linecap:round;stroke-miterlimit:10;stroke-dashoffset:89.339;stroke-dasharray:none" d="m 11.458261,21.082031 c 0.166295,0.01695 0.333025,0.02933 0.5,0.03711 C 16.994669,21.119249 21.077511,17.036407 21.077402,12 21.070802,9.469748 20.013185,7.055991 18.15748,5.335938" />
 	</g>
 </svg>
 `;
-var Ft = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
+var Ct = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<circle class="path circle" fill="none" stroke="currentColor" stroke-width="1.93833" stroke-miterlimit="10" cx="12.000002" cy="12.000002" r="10.030837" />
 	<polyline class="path check" fill="none" stroke="currentColor" stroke-width="12" stroke-linecap="round" stroke-miterlimit="10" points="100.2,40.2 51.5,88.8 29.8,67.5 " transform="matrix(0.18,0,0,0.18,-0.284,0.544)" />
 </svg>
 `;
 var jt = `<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="24" height="24" fill="currentColor">
 	<circle class="path circle" fill="none" stroke="currentColor" stroke-width="1.93833" stroke-miterlimit="10" cx="12.000002" cy="12.000002" r="10.030837" />
 	<line class="path line" fill="none" stroke="currentColor" stroke-width="2.12533" stroke-linecap="round" stroke-miterlimit="10" x1="6.562665" y1="7.1626649" x2="17.437328" y2="16.79755" />
@@ -920,18 +920,18 @@
                     break;
                 default:
                     l.addEventListener("focus", () => this.touch()), l.addEventListener("input", () => this.inputted()), l.addEventListener("blur", () => this.validate()), l.addEventListener("invalid", () => this.showErrorMessage(l));
                     break
             }
             this.fieldElements = Array(0).concat(s);
             let o = l => l instanceof HTMLSelectElement && l.name && l.form === e.element,
-                f = Array.from(t.getElementsByTagName("SELECT")).filter(o).at(0);
-            f instanceof HTMLSelectElement && (f.addEventListener("focus", () => this.touch()), f.addEventListener("change", () => {
+                u = Array.from(t.getElementsByTagName("SELECT")).filter(o).at(0);
+            u instanceof HTMLSelectElement && (u.addEventListener("focus", () => this.touch()), u.addEventListener("change", () => {
                 this.setDirty(), this.clearCustomError(), this.validate()
-            }), f.addEventListener("invalid", () => this.showErrorMessage(f)), this.fieldElements.push(f));
+            }), u.addEventListener("invalid", () => this.showErrorMessage(u)), this.fieldElements.push(u));
             let d = l => l instanceof HTMLTextAreaElement && l.name && l.form === e.element,
                 c = Array.from(t.getElementsByTagName("TEXTAREA")).filter(d).at(0);
             c instanceof HTMLTextAreaElement && (c.addEventListener("focus", () => this.touch()), c.addEventListener("input", () => this.inputted()), c.addEventListener("blur", () => this.validate()), c.addEventListener("invalid", () => this.showErrorMessage(c)), this.fieldElements.push(c)), this.name = this.assertUniqueName(), this.initialDisabled = this.fieldElements.map(l => l.disabled), this.initialRequired = this.fieldElements.map(l => l.required), r ? this.validateCheckboxSelectMultiple() : this.validateBoundField(), this.pristineValue = new je(this.aggregateValue()), this.updateVisibility = this.evalVisibility("df-show", !0) ?? this.evalVisibility("df-hide", !1) ?? function() {}, this.updateDisabled = this.evalDisable(), this.updateRequired = this.evalRequire(), this.untouch(), this.setPristine()
         }
         aggregateValue() {
             var e, t;
             if (this.fieldElements.length === 1) {
@@ -980,16 +980,16 @@
                 return Array.isArray(o) ? o.length !== 0 : !!o
             }
             let i = (s = this.fieldElements[0]) == null ? void 0 : s.getAttribute(e);
             if (typeof i != "string") return null;
             try {
                 let o = new Function(`return ${M(i,{startRule:"OperabilityExpression"})};`);
                 return () => {
-                    let f = t != r(o.call(this));
-                    this.element.hasAttribute("hidden") !== f && (this.fieldElements.forEach((d, c) => d.disabled = f || this.initialDisabled[c]), this.element.toggleAttribute("hidden", f))
+                    let u = t != r(o.call(this));
+                    this.element.hasAttribute("hidden") !== u && (this.fieldElements.forEach((d, c) => d.disabled = u || this.initialDisabled[c]), this.element.toggleAttribute("hidden", u))
                 }
             } catch (o) {
                 throw new Error(`Error while parsing <... df-show/hide="${i}">: ${o}.`)
             }
         }
         evalDisable() {
             var t;
@@ -1133,15 +1133,15 @@
         constructor(e, t, r) {
             this.clickHandler = () => {};
             this.path = Array();
             this.clicked = () => {
                 this.clickHandler()
             };
             var i;
-            this.formset = e, this.element = t, this.initialClass = t.getAttribute("class") ?? "", this.isAutoDisabled = t.hasAttribute("auto-disable"), this.decoratorElement = t.querySelector(".dj-button-decorator"), this.originalDecorator = (i = this.decoratorElement) == null ? void 0 : i.cloneNode(!0), this.spinnerElement = document.createElement("i"), this.spinnerElement.classList.add("dj-icon", "dj-spinner"), this.spinnerElement.innerHTML = Ct, this.okayElement = document.createElement("i"), this.okayElement.classList.add("dj-icon", "dj-okay"), this.okayElement.innerHTML = Ft, this.bummerElement = document.createElement("i"), this.bummerElement.classList.add("dj-icon", "dj-bummer"), this.bummerElement.innerHTML = jt, this.path = r, this.parseActionsQueue(t.getAttribute("df-click")), this.updateVisibility = this.evalVisibility("df-show", !0) ?? this.evalVisibility("df-hide", !1) ?? function() {}, this.updateDisabled = this.evalDisable(), t.addEventListener("click", this.clicked)
+            this.formset = e, this.element = t, this.initialClass = t.getAttribute("class") ?? "", this.isAutoDisabled = t.hasAttribute("auto-disable"), this.decoratorElement = t.querySelector(".dj-button-decorator"), this.originalDecorator = (i = this.decoratorElement) == null ? void 0 : i.cloneNode(!0), this.spinnerElement = document.createElement("i"), this.spinnerElement.classList.add("dj-icon", "dj-spinner"), this.spinnerElement.innerHTML = Ft, this.okayElement = document.createElement("i"), this.okayElement.classList.add("dj-icon", "dj-okay"), this.okayElement.innerHTML = Ct, this.bummerElement = document.createElement("i"), this.bummerElement.classList.add("dj-icon", "dj-bummer"), this.bummerElement.innerHTML = jt, this.path = r, this.parseActionsQueue(t.getAttribute("df-click")), this.updateVisibility = this.evalVisibility("df-show", !0) ?? this.evalVisibility("df-hide", !1) ?? function() {}, this.updateDisabled = this.evalDisable(), t.addEventListener("click", this.clicked)
         }
         evalVisibility(e, t) {
             let r = this.element.getAttribute(e);
             if (r === null) return null;
             try {
                 let i = new Function(`return ${M(r,{startRule:"OperabilityExpression"})}`);
                 return () => {
@@ -1185,15 +1185,15 @@
         proceed(e) {
             return async t => {
                 if (typeof e == "string" && e.length > 0) location.href = e;
                 else if (t instanceof Response && t.status === 200) {
                     let r = await t.clone().json();
                     r.success_url ? location.href = r.success_url : console.warn("Neither a success-, nor a proceed-URL are given.")
                 }
-                return Promise.resolve(t)
+                return new Promise(r => window.setTimeout(() => r(t), 3e3))
             }
         }
         delay(e) {
             return t => new Promise(r => this.timeoutHandler = window.setTimeout(() => {
                 this.timeoutHandler = void 0, r(t)
             }, e))
         }
@@ -1260,47 +1260,61 @@
         activate(e) {
             return t => (this.formset.updateOperability(e), Promise.resolve(t))
         }
         noop() {
             return e => Promise.resolve(e)
         }
         restore() {
-            return () => window.setTimeout(() => this.restoreToInitial())
+            window.setTimeout(() => this.restoreToInitial())
         }
         decorate(e, t) {
             return r => {
                 var i;
                 return (i = this.decoratorElement) == null || i.replaceChildren(e), typeof t != "number" ? Promise.resolve(r) : new Promise(s => this.timeoutHandler = window.setTimeout(() => {
                     this.timeoutHandler = void 0, s(r)
                 }, t))
             }
         }
         setClickHandler(e) {
-            let t = (s, o) => {
-                    for (let [f, d] of s.entries()) o ? o = o.then(d.func.apply(this, d.args)) : o = d.func.apply(this, d.args)();
-                    return o
+            let t = o => {
+                    let u;
+                    for (let d of o.values()) u = (u == null ? void 0 : u.then(d.func.apply(this, d.args))) ?? d.func.apply(this, d.args)();
+                    return u
                 },
-                r = (s, o) => {
-                    for (let [f, d] of s.entries()) f === 0 ? o = o.catch(d.func.apply(this, d.args)) : o = o.then(d.func.apply(this, d.args));
-                    return o
+                r = (o, u) => {
+                    let d;
+                    for (let c of o.values()) d = (d == null ? void 0 : d.then(c.func.apply(this, c.args))) ?? c.func.apply(this, c.args)(u);
+                    return d
                 },
-                i = (s, o) => (s.condition.call(this) ? s.fulfilled instanceof N ? (o = t(s.fulfilled.successChain, o), o && (o = r(s.fulfilled.rejectChain, o), o.finally(this.restore.apply(this)))) : o = i(s.fulfilled, o) : s.otherwise instanceof N ? (o = t(s.otherwise.successChain, o), o && (o = r(s.otherwise.rejectChain, o), o.finally(this.restore.apply(this)))) : o = i(s.otherwise, o), o);
+                i = o => {
+                    var u, d;
+                    (d = (u = t(o.successChain)) == null ? void 0 : u.then(() => {
+                        this.restore.apply(this)
+                    })) == null || d.catch(c => {
+                        var l;
+                        (l = r(o.rejectChain, c)) == null || l.finally(() => {
+                            this.restore.apply(this)
+                        })
+                    })
+                },
+                s = o => {
+                    o.condition.call(this) ? o.fulfilled instanceof N ? i(o.fulfilled) : s(o.fulfilled) : o.otherwise instanceof N ? i(o.otherwise) : s(o.otherwise)
+                };
             this.clickHandler = () => {
-                let s;
-                e instanceof N ? (s = t(e.successChain, s), s && (s = r(e.rejectChain, s), s.finally(this.restore.apply(this)))) : i(e, s)
+                e instanceof N ? i(e) : s(e)
             }
         }
         parseActionsQueue(e) {
             if (!e) return;
             let t = i => {
                     let s = new Array;
                     for (let o of i) {
-                        let f = this[o.funcname];
-                        if (typeof f != "function") throw new Error(`Unknown function '${o.funcname}'.`);
-                        s.push(new ce(f, o.args))
+                        let u = this[o.funcname];
+                        if (typeof u != "function") throw new Error(`Unknown function '${o.funcname}'.`);
+                        s.push(new ce(u, o.args))
                     }
                     return s.length === 0 && s.push(new ce(this.noop, [])), s
                 },
                 r = i => i.condition === !0 ? new N(t(i.fulfilled.successChain), t(i.fulfilled.rejectChain)) : new Le(Function(i.condition), r(i.fulfilled), r(i.otherwise));
             try {
                 let i = M(e, {
                         startRule: "Ternary"
@@ -1384,16 +1398,16 @@
         getDataValue(e) {
             return this.form.getDataValue(e)
         }
         isButtonActive(e, t) {
             let r = e[0] !== "" ? e : (() => {
                     let s = [...this.form.path],
                         o = e.filter(d => d !== ""),
-                        f = e.length - o.length;
-                    return s.splice(s.length - f + 1), s.push(...o), s
+                        u = e.length - o.length;
+                    return s.splice(s.length - u + 1), s.push(...o), s
                 })(),
                 i = this.form.formset.buttons.find(s => (0, Pe.default)(s.path, r));
             return t === "active" && (i == null ? void 0 : i.element) === document.activeElement
         }
     },
     Me = class {
         constructor(e, t) {
@@ -1415,16 +1429,16 @@
             };
             var s, o;
             this.formset = e, this.element = t, this.path = ((s = this.name) == null ? void 0 : s.split(".")) ?? [];
             let r = t.nextSibling;
             this.fieldset = r instanceof HTMLFieldSetElement && r.form === t ? new Se(this, r) : null;
             let i = (o = t.nextElementSibling) == null ? void 0 : o.querySelector(".dj-form-errors > .dj-errorlist > .dj-placeholder");
             if (i && (this.errorList = i.parentElement, this.errorPlaceholder = this.errorList.removeChild(i)), this.isTransient = !!this.element.getAttribute("df-transient"), !this.isTransient) {
-                let f = t.closest("dialog");
-                this.parentDialog = f ? new ke(this, f) : null
+                let u = t.closest("dialog");
+                this.parentDialog = u ? new ke(this, u) : null
             }
             this.element.addEventListener("submit", this.handleSubmit), this.element.addEventListener("reset", this.handleReset)
         }
         aggregateValues() {
             let e = new Map;
             for (let t of this.fieldGroups) e.set(t.name, t.aggregateValue());
             for (let t of this.hiddenInputFields.filter(r => r.type === "hidden")) e.set(t.name, t.value);
@@ -1602,17 +1616,17 @@
                 var i, s;
                 let t = ((i = this.parent) == null ? void 0 : i.children) ?? this.formset.formCollections;
                 this.justAdded ? (this.disconnect(), t.splice(t.indexOf(this), 1), this.repositionSiblings()) : (this.toggleForRemoval(!this.markedForRemoval), this.removeButton.disabled = !this.markedForRemoval), t.forEach(o => o.updateRemoveButtonAttrs()), (((s = this.parent) == null ? void 0 : s.formCollectionTemplate) ?? this.formset.formCollectionTemplate).updateAddButtonAttrs()
             };
             let o = r.getAttribute("sibling-position");
             if (!o) throw new Error("Missing argument 'sibling-position' in <django-form-collection>");
             this.position = this.initialPosition = parseInt(o), this.siblingId = i;
-            let f = r.getAttribute("min-siblings");
-            if (!f) throw new Error("Missing argument 'min-siblings' in <django-form-collection>");
-            this.minSiblings = parseInt(f);
+            let u = r.getAttribute("min-siblings");
+            if (!u) throw new Error("Missing argument 'min-siblings' in <django-form-collection>");
+            this.minSiblings = parseInt(u);
             let d = r.getAttribute("max-siblings");
             d && (this.maxSiblings = parseInt(d));
             let c = r.querySelector(":scope > button.remove-collection");
             if (!c) throw new Error('<django-form-collection> with siblings requires child element <button class="remove-collection">');
             this.removeButton = c, this.removeButton.addEventListener("click", this.removeCollection)
         }
         disconnect() {
@@ -1653,42 +1667,42 @@
                 let t = e.oldDraggableIndex ?? NaN,
                     r = e.newDraggableIndex ?? NaN;
                 if (!isFinite(t) || !isFinite(r) || t === r) return;
                 let i = ((s = this.parent) == null ? void 0 : s.children) ?? this.formset.formCollections;
                 if (i.at(t) instanceof S) {
                     let o = i.splice(t, 1);
                     i.splice(r, 0, ...o), o.at(0).repositionSiblings();
-                    let f = this.prefix === "0" ? 0 : this.prefix.split(".").length;
-                    i.forEach((d, c) => d.repositionForms(f, c)), this.formset.validate()
+                    let u = this.prefix === "0" ? 0 : this.prefix.split(".").length;
+                    i.forEach((d, c) => d.repositionForms(u, c)), this.formset.validate()
                 }
             };
             this.appendFormCollectionSibling = () => {
                 var d;
                 let e = Object.fromEntries(this.baseContext),
                     [t, r] = this.getNextPositionAndSiblingId();
                 e.position = t.toString(), e.siblingId = r.toString(), e.position_1 = "${position}", e.siblingId_1 = "${siblingId}";
                 for (let c = 1; c < 10; ++c) e[`position_${c+1}`] = `\${position_${c}}`, e[`siblingId_${c+1}`] = `\${siblingId_${c}}`;
                 let i = this.renderEmptyCollection(e);
                 this.element.insertAdjacentHTML("beforebegin", i);
                 let s = this.element.previousElementSibling;
                 if (!(s instanceof HTMLElement)) throw new Error("Unable to insert empty <django-form-collection> element.");
                 let o = ((d = this.parent) == null ? void 0 : d.children) ?? this.formset.formCollections,
-                    f = new S(this.formset, s, r, this.parent);
-                o.push(f), this.formset.findForms(s), this.formset.assignFieldsToForms(s), this.formset.assignFormsToCollections(), this.formset.findCollectionErrorsList(), f.markAsFreshAndEmpty(!0), this.formset.validate(), o.forEach(c => c.updateRemoveButtonAttrs()), this.updateAddButtonAttrs()
+                    u = new S(this.formset, s, r, this.parent);
+                o.push(u), this.formset.findForms(s), this.formset.assignFieldsToForms(s), this.formset.assignFormsToCollections(), this.formset.findCollectionErrorsList(), u.markAsFreshAndEmpty(!0), this.formset.validate(), o.forEach(c => c.updateRemoveButtonAttrs()), this.updateAddButtonAttrs()
             };
             var d;
             this.formset = e, this.element = t, this.parent = r;
             let i = t.innerHTML.matchAll(/\$\{([^} ]+)\}/g);
             for (let c of i) this.baseContext.set(c[1], c[0]);
             let s = t.getAttribute("prefix");
             if (!s) throw new Error('<template class="empty-collection" ...> requires attribute "prefix"');
             this.prefix = s, e.pushTemplatePrefix(this.prefix), this.renderEmptyCollection = (0, St.default)(t.innerHTML), (d = t.nextElementSibling) != null && d.matches("button.add-collection") && (this.addButton = t.nextElementSibling, this.addButton.addEventListener("click", this.appendFormCollectionSibling));
             let o = this.element.content.querySelector("django-form-collection"),
-                f = o == null ? void 0 : o.getAttribute("max-siblings");
-            f && (this.maxSiblings = parseInt(f)), t.hasAttribute("sortable") && new nt(t.parentElement, {
+                u = o == null ? void 0 : o.getAttribute("max-siblings");
+            u && (this.maxSiblings = parseInt(u)), t.hasAttribute("sortable") && new nt(t.parentElement, {
                 animation: 150,
                 handle: "django-form-collection[sibling-position]:not(.dj-marked-for-removal) > .collection-drag-handle",
                 draggable: "django-form-collection[sibling-position]",
                 selectedClass: "selected",
                 ghostClass: "dj-ghost-collection",
                 onEnd: this.resortSiblings
             })
@@ -1785,15 +1799,15 @@
                 else if (t instanceof HTMLButtonElement) {
                     if (t.hasAttribute("df-click") && t.form === s.element) {
                         let o = new de(s.formset, t, [...s.path, t.name]);
                         this.buttons.push(o)
                     }
                 } else {
                     let o = t.closest('[role="group"]');
-                    o && !s.fieldGroups.find(f => f.element === o) && s.fieldGroups.push(new xe(s, o))
+                    o && !s.fieldGroups.find(u => u.element === o) && s.fieldGroups.push(new xe(s, o))
                 }
             }
         }
         findForms(e) {
             e = e ?? this.element;
             for (let t of e.getElementsByTagName("FORM")) {
                 let r = new Me(this, t);
@@ -1863,38 +1877,38 @@
 
             function r(s, o) {
                 if (o.length === 1) {
                     Array.isArray(s) ? t && !s.includes(t) && s.push(t) : s[o[0]] = t ?? [];
                     return
                 }
                 if (isNaN(parseInt(o[1]))) {
-                    let f = s[o[0]] ?? {};
-                    r(f, o.slice(1));
+                    let u = s[o[0]] ?? {};
+                    r(u, o.slice(1));
                     let d = parseInt(o[0]);
-                    isNaN(d) ? s[o[0]] = f : s[d] = {
+                    isNaN(d) ? s[o[0]] = u : s[d] = {
                         ...s[d],
-                        ...f
+                        ...u
                     }
                 } else {
                     if (Array.isArray(s)) throw new Error("Invalid form structure: Contains nested arrays.");
-                    let f = s[o[0]] ?? [];
-                    if (!Array.isArray(f)) throw new Error("Invalid form structure: Inner array is missing.");
-                    r(f, o.slice(1)), s[o[0]] = f
+                    let u = s[o[0]] ?? [];
+                    if (!Array.isArray(u)) throw new Error("Invalid form structure: Inner array is missing.");
+                    r(u, o.slice(1)), s[o[0]] = u
                 }
             }
             let i = {};
             for (let s of this.emptyCollectionPrefixes) {
                 let o = ["formset_data", ...s.split(".")];
                 t = (0, $.default)(i, o), r(i, o)
             }
             for (let s of this.forms) {
                 if (!s.name) {
-                    let f = Object.fromEntries(s.aggregateValues());
+                    let u = Object.fromEntries(s.aggregateValues());
                     return Object.assign({}, {
-                        formset_data: f
+                        formset_data: u
                     }, {
                         _extra: e
                     })
                 }
                 if (s.isTransient) continue;
                 let o = s.getAbsPath();
                 t = (0, $.default)(this.data, o), s.markedForRemoval && (t[li] = !0), r(i, o)
@@ -1919,22 +1933,22 @@
                         headers: i,
                         body: JSON.stringify(r),
                         signal: this.abortController.signal
                     });
                     switch (s.status) {
                         case 200:
                             this.clearErrors();
-                            for (let f of this.forms) f.element.dispatchEvent(new Event("submitted"));
+                            for (let u of this.forms) u.element.dispatchEvent(new Event("submitted"));
                             return s;
                         case 422:
                             this.clearErrors();
                             let o = await s.clone().json();
                             return this.reportErrors(o), s;
                         default:
-                            return console.warn(`Unknown response status: ${s.status}`), this.clearErrors(), this.buttons.forEach(f => f.restoreToInitial()), s
+                            return console.warn(`Unknown response status: ${s.status}`), this.clearErrors(), this.buttons.forEach(u => u.restoreToInitial()), s
                     }
                 } catch (i) {
                     this.clearErrors(), this.buttons.forEach(s => s.restoreToInitial()), alert(i)
                 }
             } else {
                 this.clearErrors();
                 for (let r of this.forms) r.reportValidity()
@@ -2005,71 +2019,71 @@
         }
     };
 V;
 window.addEventListener("DOMContentLoaded", n => {
     let e = st.convertPseudoClasses(),
         t = Array();
 
-    function r(o, f, d, c = void 0) {
-        customElements.get(f) instanceof Function ? o() : (window.customElements.define(f, d, c), window.customElements.whenDefined(f).then(() => o()))
+    function r(o, u, d, c = void 0) {
+        customElements.get(u) instanceof Function ? o() : (window.customElements.define(u, d, c), window.customElements.whenDefined(u).then(() => o()))
     }
 
     function i(o) {
         o.querySelector('select[is="django-selectize"]') && t.push(new Promise((d, c) => {
-            import("./DjangoSelectize-YB6QRNYJ.js").then(({
+            import("./DjangoSelectize-JMSV2QXX.js").then(({
                 DjangoSelectizeElement: l
             }) => {
                 r(d, "django-selectize", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector('select[is="django-country-selectize"]') && t.push(new Promise((d, c) => {
-            import("./CountrySelectize-ZVZPUZGO.js").then(({
+            import("./CountrySelectize-6YQ6A6VY.js").then(({
                 CountrySelectizeElement: l
             }) => {
                 r(d, "django-country-selectize", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector("django-sortable-select") ? t.push(new Promise((d, c) => {
-            import("./SortableSelect-7PAIJDN5.js").then(({
+            import("./SortableSelect-27BKOQAW.js").then(({
                 SortableSelectElement: l
             }) => {
-                customElements.get("django-sortable-select") instanceof Function ? d() : window.customElements.define("django-sortable-select", l), import("./DualSelector-ZHU2XXXL.js").then(({
+                customElements.get("django-sortable-select") instanceof Function ? d() : window.customElements.define("django-sortable-select", l), import("./DualSelector-233VL6HH.js").then(({
                     DualSelectorElement: k
                 }) => {
                     customElements.get("django-dual-selector") instanceof Function ? d() : (window.customElements.define("django-dual-selector", k, {
                         extends: "select"
                     }), Promise.all([window.customElements.whenDefined("django-sortable-select"), window.customElements.whenDefined("django-dual-selector")]).then(() => d()))
                 }).catch(k => c(k))
             }).catch(l => c(l))
         })) : o.querySelector('select[is="django-dual-selector"]') && t.push(new Promise((d, c) => {
-            import("./DualSelector-ZHU2XXXL.js").then(({
+            import("./DualSelector-233VL6HH.js").then(({
                 DualSelectorElement: l
             }) => {
                 r(d, "django-dual-selector", l, {
                     extends: "select"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-phone-number"]') && t.push(new Promise((d, c) => {
-            import("./PhoneNumber-IX6JTWS7.js").then(({
+            import("./PhoneNumber-KCJABOET.js").then(({
                 PhoneNumberElement: l
             }) => {
                 r(d, "django-phone-number", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelectorAll('textarea[is="django-richtext"]').forEach(d => {
             t.push(new Promise((c, l) => {
                 let k = () => {
                     d.isInitialized ? c() : d.addEventListener("connected", () => c(), {
                         once: !0
                     })
                 };
-                import("./RichtextArea-VJIDTE2W.js").then(({
+                import("./RichtextArea-QY2VVCDL.js").then(({
                     RichTextAreaElement: G
                 }) => {
                     customElements.get("django-richtext") instanceof Function ? k() : (window.customElements.define("django-richtext", G, {
                         extends: "textarea"
                     }), window.customElements.whenDefined("django-richtext").then(k))
                 }).catch(G => l(G))
             }))
@@ -2078,119 +2092,119 @@
                 DjangoSlugElement: l
             }) => {
                 r(d, "django-slug", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-2OODDTX3.js").then(({
+            import("./DateTime-4XMVQT2P.js").then(({
                 DateFieldElement: l
             }) => {
                 r(d, "django-datefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-JILYT5ID.js").then(({
+            import("./Calendar-SME4CT3M.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-2OODDTX3.js").then(({
+            import("./DateTime-4XMVQT2P.js").then(({
                 DatePickerElement: l
             }) => {
                 r(d, "django-datepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-2OODDTX3.js").then(({
+            import("./DateTime-4XMVQT2P.js").then(({
                 DateTimeFieldElement: l
             }) => {
                 r(d, "django-datetimefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-JILYT5ID.js").then(({
+            import("./Calendar-SME4CT3M.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datetimecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-2OODDTX3.js").then(({
+            import("./DateTime-4XMVQT2P.js").then(({
                 DateTimePickerElement: l
             }) => {
                 r(d, "django-datetimepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-2OODDTX3.js").then(({
+            import("./DateTime-4XMVQT2P.js").then(({
                 DateRangeFieldElement: l
             }) => {
                 r(d, "django-daterangefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-JILYT5ID.js").then(({
+            import("./Calendar-SME4CT3M.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-daterangecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-daterangepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-2OODDTX3.js").then(({
+            import("./DateTime-4XMVQT2P.js").then(({
                 DateRangePickerElement: l
             }) => {
                 r(d, "django-daterangepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangefield"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-2OODDTX3.js").then(({
+            import("./DateTime-4XMVQT2P.js").then(({
                 DateTimeRangeFieldElement: l
             }) => {
                 r(d, "django-datetimerangefield", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangecalendar"]') && t.push(new Promise((d, c) => {
-            import("./Calendar-JILYT5ID.js").then(({
+            import("./Calendar-SME4CT3M.js").then(({
                 DateCalendarElement: l
             }) => {
                 r(d, "django-datetimerangecalendar", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         })), o.querySelector('input[is="django-datetimerangepicker"]') && t.push(new Promise((d, c) => {
-            import("./DateTime-2OODDTX3.js").then(({
+            import("./DateTime-4XMVQT2P.js").then(({
                 DateTimeRangePickerElement: l
             }) => {
                 r(d, "django-datetimerangepicker", l, {
                     extends: "input"
                 })
             }).catch(l => c(l))
         }))
     }
     document.querySelectorAll("template.empty-collection").forEach(o => {
         o instanceof HTMLTemplateElement && o.content instanceof DocumentFragment && i(o.content)
     }), i(document);
     let s = new Set;
     document.querySelectorAll("django-formset [id]").forEach(o => {
-        let f = o.getAttribute("id");
-        if (s.has(f)) throw new Error(`There are at least two elements with attribute id="${f}"`);
-        s.add(f)
+        let u = o.getAttribute("id");
+        if (s.has(u)) throw new Error(`There are at least two elements with attribute id="${u}"`);
+        s.add(u)
     }), Promise.all(t).then(() => {
         window.customElements.define("django-formset", he), window.customElements.whenDefined("django-formset").then(() => {
             e.remove()
         })
     }).catch(o => console.error(`Failed to initialize django-formset: ${o}`))
 });
 /*! Bundled license information:
```

### Comparing `django_formset-1.4/formset/static/formset/tiptap-extensions/footnote.js` & `django_formset-1.4.1/formset/static/formset/tiptap-extensions/footnote.js`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/calendar/hours.html` & `django_formset-1.4.1/formset/templates/calendar/hours.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/calendar/months.html` & `django_formset-1.4.1/formset/templates/calendar/months.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/calendar/weeks.html` & `django_formset-1.4.1/formset/templates/calendar/weeks.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/calendar/years.html` & `django_formset-1.4.1/formset/templates/calendar/years.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/bootstrap/widgets/dual_selector.html` & `django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/bootstrap/widgets/file.html` & `django_formset-1.4.1/formset/templates/formset/bootstrap/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/bulma/widgets/dual_selector.html` & `django_formset-1.4.1/formset/templates/formset/bulma/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/bulma/widgets/file.html` & `django_formset-1.4.1/formset/templates/formset/bulma/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/default/collection.html` & `django_formset-1.4.1/formset/templates/formset/default/collection.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/default/fieldset.html` & `django_formset-1.4.1/formset/templates/formset/default/fieldset.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/default/form_dialog.html` & `django_formset-1.4.1/formset/templates/formset/default/form_dialog.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/default/widgets/dual_selector.html` & `django_formset-1.4.1/formset/templates/formset/default/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/default/widgets/file.html` & `django_formset-1.4.1/formset/templates/formset/default/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/default/widgets/selectize.html` & `django_formset-1.4.1/formset/templates/formset/default/widgets/selectize.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/foundation/widgets/dual_selector.html` & `django_formset-1.4.1/formset/templates/formset/foundation/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/foundation/widgets/file.html` & `django_formset-1.4.1/formset/templates/formset/foundation/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/icons/blockquote.svg` & `django_formset-1.4.1/formset/templates/formset/icons/blockquote.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/icons/calendar-today.svg` & `django_formset-1.4.1/formset/templates/formset/icons/calendar-today.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/icons/footnote.svg` & `django_formset-1.4.1/formset/templates/formset/icons/footnote.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/icons/letters.svg` & `django_formset-1.4.1/formset/templates/formset/icons/letters.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/icons/placeholder.svg` & `django_formset-1.4.1/formset/templates/formset/icons/placeholder.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/icons/questionmark.svg` & `django_formset-1.4.1/formset/templates/formset/icons/questionmark.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/icons/strike.svg` & `django_formset-1.4.1/formset/templates/formset/icons/strike.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/icons/subscript.svg` & `django_formset-1.4.1/formset/templates/formset/icons/subscript.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/icons/unlink.svg` & `django_formset-1.4.1/formset/templates/formset/icons/unlink.svg`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/richtext/align.html` & `django_formset-1.4.1/formset/templates/formset/richtext/align.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/richtext/color.html` & `django_formset-1.4.1/formset/templates/formset/richtext/color.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/richtext/heading.html` & `django_formset-1.4.1/formset/templates/formset/richtext/heading.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/tailwind/widgets/dual_selector.html` & `django_formset-1.4.1/formset/templates/formset/tailwind/widgets/dual_selector.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/tailwind/widgets/file.html` & `django_formset-1.4.1/formset/templates/formset/tailwind/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templates/formset/uikit/widgets/file.html` & `django_formset-1.4.1/formset/templates/formset/uikit/widgets/file.html`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templatetags/formsetify.py` & `django_formset-1.4.1/formset/templatetags/formsetify.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templatetags/phonenumber.py` & `django_formset-1.4.1/formset/templatetags/phonenumber.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/templatetags/richtext.py` & `django_formset-1.4.1/formset/templatetags/richtext.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/upload.py` & `django_formset-1.4.1/formset/upload.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/utils.py` & `django_formset-1.4.1/formset/utils.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/views.py` & `django_formset-1.4.1/formset/views.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/formset/widgets.py` & `django_formset-1.4.1/formset/widgets.py`

 * *Files identical despite different names*

### Comparing `django_formset-1.4/setup.py` & `django_formset-1.4.1/setup.py`

 * *Files identical despite different names*

