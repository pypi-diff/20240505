# Comparing `tmp/rer.solrpush-1.3.3.tar.gz` & `tmp/rer.solrpush-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rer.solrpush-1.3.3.tar", last modified: Wed Nov  8 16:22:56 2023, max compression
+gzip compressed data, was "rer.solrpush-1.4.0.tar", last modified: Sun May  5 06:25:40 2024, max compression
```

## Comparing `rer.solrpush-1.3.3.tar` & `rer.solrpush-1.4.0.tar`

### file list

```diff
@@ -1,170 +1,176 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.518708 rer.solrpush-1.3.3/
--rw-r--r--   0 cekk       (501) staff       (20)     4392 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       67 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      652 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      525 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)    13071 2023-11-08 16:22:56.518786 rer.solrpush-1.3.3/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     7496 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)      171 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/docker-compose.yml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.501164 rer.solrpush-1.3.3/docs/
--rw-r--r--   0 cekk       (501) staff       (20)   213611 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/docs/Solr-Push_Configurazione.jpg
--rw-r--r--   0 cekk       (501) staff       (20)     7885 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       59 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)    32560 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/docs/rer-logo.png
--rw-r--r--   0 cekk       (501) staff       (20)     3432 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/publiccode.yml
--rw-r--r--   0 cekk       (501) staff       (20)      321 2023-11-08 16:22:56.519038 rer.solrpush-1.3.3/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2586 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.496614 rer.solrpush-1.3.3/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.501321 rer.solrpush-1.3.3/src/rer/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.504195 rer.solrpush-1.3.3/src/rer/solrpush/
--rw-r--r--   0 cekk       (501) staff       (20)      130 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.504786 rer.solrpush-1.3.3/src/rer/solrpush/adapters/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/adapters/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      348 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/adapters/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1439 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/adapters/file.py
--rw-r--r--   0 cekk       (501) staff       (20)      706 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/adapters/rss_feed.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.505229 rer.solrpush-1.3.3/src/rer/solrpush/behaviors/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/behaviors/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      458 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/behaviors/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1148 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/behaviors/solr_fields.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.506353 rer.solrpush-1.3.3/src/rer/solrpush/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3421 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     3304 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)     1205 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/elevate_settings.py
--rw-r--r--   0 cekk       (501) staff       (20)    16058 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/maintenance.py
--rw-r--r--   0 cekk       (501) staff       (20)      350 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/query_debug.py
--rw-r--r--   0 cekk       (501) staff       (20)     6247 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/querybuilder.py
--rw-r--r--   0 cekk       (501) staff       (20)     2322 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/scales.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.507193 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.497166 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/dist/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.508911 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/dist/dev/
--rw-r--r--   0 cekk       (501) staff       (20)  2311368 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/dist/dev/main.js
--rw-r--r--   0 cekk       (501) staff       (20)  1783747 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/dist/dev/main.js.map
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.510371 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/dist/prod/
--rw-r--r--   0 cekk       (501) staff       (20)   294024 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/dist/prod/main.js
--rw-r--r--   0 cekk       (501) staff       (20)      159 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/dist/prod/main.js.map
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.510491 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.510602 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/FacetsContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     1025 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/FacetsContainer/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.510710 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/ProgressBar/
--rw-r--r--   0 cekk       (501) staff       (20)      946 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/ProgressBar/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.510823 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     1737 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/index.js
--rw-r--r--   0 cekk       (501) staff       (20)      455 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/index.js
--rw-r--r--   0 cekk       (501) staff       (20)      258 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/package.json
--rw-r--r--   0 cekk       (501) staff       (20)      618 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/styles.css
--rw-r--r--   0 cekk       (501) staff       (20)      174 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/styles.css.map
--rw-r--r--   0 cekk       (501) staff       (20)      431 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/styles.scss
--rw-r--r--   0 cekk       (501) staff       (20)    57992 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/static/yarn.lock
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.511173 rer.solrpush-1.3.3/src/rer/solrpush/browser/templates/
--rw-r--r--   0 cekk       (501) staff       (20)     1822 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/templates/controlpanel_layout.pt
--rw-r--r--   0 cekk       (501) staff       (20)      498 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/templates/query_debug.pt
--rw-r--r--   0 cekk       (501) staff       (20)     1453 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/browser/templates/reindex_solr.pt
--rw-r--r--   0 cekk       (501) staff       (20)     2423 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     4080 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/indexer.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.511825 rer.solrpush-1.3.3/src/rer/solrpush/interfaces/
--rw-r--r--   0 cekk       (501) staff       (20)      282 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/interfaces/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      307 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/interfaces/adapter.py
--rw-r--r--   0 cekk       (501) staff       (20)     3344 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/interfaces/elevate.py
--rw-r--r--   0 cekk       (501) staff       (20)      197 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/interfaces/layer.py
--rw-r--r--   0 cekk       (501) staff       (20)      153 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/interfaces/queueprocessor.py
--rw-r--r--   0 cekk       (501) staff       (20)     6735 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/interfaces/settings.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.512358 rer.solrpush-1.3.3/src/rer/solrpush/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/locales/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.497792 rer.solrpush-1.3.3/src/rer/solrpush/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.512596 rer.solrpush-1.3.3/src/rer/solrpush/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      458 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.mo
--rw-r--r--   0 cekk       (501) staff       (20)    11576 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.497905 rer.solrpush-1.3.3/src/rer/solrpush/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.512839 rer.solrpush-1.3.3/src/rer/solrpush/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     9290 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.mo
--rw-r--r--   0 cekk       (501) staff       (20)    16728 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.po
--rw-r--r--   0 cekk       (501) staff       (20)    11694 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/locales/rer.solrpush.pot
--rw-r--r--   0 cekk       (501) staff       (20)     1528 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      473 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)     6130 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/parser.py
--rw-r--r--   0 cekk       (501) staff       (20)      424 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.498388 rer.solrpush-1.3.3/src/rer/solrpush/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.513590 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      854 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/actions.xml
--rw-r--r--   0 cekk       (501) staff       (20)      162 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      953 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      257 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.513948 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/registry/
--rw-r--r--   0 cekk       (501) staff       (20)      891 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/registry/bundle.xml
--rw-r--r--   0 cekk       (501) staff       (20)     2828 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/registry/criteria.xml
--rw-r--r--   0 cekk       (501) staff       (20)      278 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/registry/settings.xml
--rw-r--r--   0 cekk       (501) staff       (20)      387 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.514059 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/types/
--rw-r--r--   0 cekk       (501) staff       (20)      299 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/types/Document.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.514275 rer.solrpush-1.3.3/src/rer/solrpush/profiles/to_1100/
--rw-r--r--   0 cekk       (501) staff       (20)      232 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/to_1100/componentregistry.xml
--rw-r--r--   0 cekk       (501) staff       (20)       97 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/to_1100/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.514495 rer.solrpush-1.3.3/src/rer/solrpush/profiles/to_1300/
--rw-r--r--   0 cekk       (501) staff       (20)      322 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/to_1300/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      211 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/to_1300/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.514849 rer.solrpush-1.3.3/src/rer/solrpush/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      122 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      536 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      605 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/profiles/uninstall/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.515065 rer.solrpush-1.3.3/src/rer/solrpush/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      216 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.515273 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      200 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.515612 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/elevate_schema/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/elevate_schema/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      344 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/elevate_schema/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      355 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/elevate_schema/get.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.516179 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/solr_search/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/solr_search/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3891 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/solr_search/batch.py
--rw-r--r--   0 cekk       (501) staff       (20)      334 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/solr_search/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      919 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/solr_search/get.py
--rw-r--r--   0 cekk       (501) staff       (20)     3064 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/solr_search/solr_search_handler.py
--rw-r--r--   0 cekk       (501) staff       (20)      610 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     5232 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.517654 rer.solrpush-1.3.3/src/rer/solrpush/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.518120 rer.solrpush-1.3.3/src/rer/solrpush/tests/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     6207 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/docs/example.docx
--rw-r--r--   0 cekk       (501) staff       (20)     8355 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/docs/example.ods
--rw-r--r--   0 cekk       (501) staff       (20)    13430 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/docs/example.pdf
--rw-r--r--   0 cekk       (501) staff       (20)    14135 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/docs/plone_logo.png
--rw-r--r--   0 cekk       (501) staff       (20)     2079 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_behaviors.py
--rw-r--r--   0 cekk       (501) staff       (20)     4328 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_elevate.py
--rw-r--r--   0 cekk       (501) staff       (20)     6398 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_events.py
--rw-r--r--   0 cekk       (501) staff       (20)     3137 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_image_tags.py
--rw-r--r--   0 cekk       (501) staff       (20)     6364 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_maintenance.py
--rw-r--r--   0 cekk       (501) staff       (20)     9366 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_querybuilder.py
--rw-r--r--   0 cekk       (501) staff       (20)     4467 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_restapi_search.py
--rw-r--r--   0 cekk       (501) staff       (20)     5992 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_search.py
--rw-r--r--   0 cekk       (501) staff       (20)     2295 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)    14837 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_solr_interface.py
--rw-r--r--   0 cekk       (501) staff       (20)     3137 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_tika.py
--rw-r--r--   0 cekk       (501) staff       (20)     3700 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/tests/test_vocabularies.py
--rw-r--r--   0 cekk       (501) staff       (20)     2213 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/upgrades.py
--rw-r--r--   0 cekk       (501) staff       (20)     2288 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/upgrades.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.518589 rer.solrpush-1.3.3/src/rer/solrpush/utils/
--rw-r--r--   0 cekk       (501) staff       (20)      345 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/utils/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3813 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/utils/solr_common.py
--rw-r--r--   0 cekk       (501) staff       (20)     8731 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/utils/solr_indexer.py
--rw-r--r--   0 cekk       (501) staff       (20)    10807 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/utils/solr_search.py
--rw-r--r--   0 cekk       (501) staff       (20)     1599 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer/solrpush/vocabularies.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-11-08 16:22:56.502678 rer.solrpush-1.3.3/src/rer.solrpush.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)    13071 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer.solrpush.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     5360 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer.solrpush.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer.solrpush.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      117 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer.solrpush.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer.solrpush.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer.solrpush.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      245 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer.solrpush.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2023-11-08 16:22:56.000000 rer.solrpush-1.3.3/src/rer.solrpush.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.491438 rer.solrpush-1.4.0/
+-rw-r--r--   0 cekk       (501) staff       (20)     4466 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       67 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      652 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      539 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)    13289 2024-05-05 06:25:40.491504 rer.solrpush-1.4.0/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     7496 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       62 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/constraints_plone60.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      157 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/docker-compose.yml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.475254 rer.solrpush-1.4.0/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)   213611 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/docs/Solr-Push_Configurazione.jpg
+-rw-r--r--   0 cekk       (501) staff       (20)       59 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    32560 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/docs/rer-logo.png
+-rw-r--r--   0 cekk       (501) staff       (20)     3432 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/publiccode.yml
+-rw-r--r--   0 cekk       (501) staff       (20)      445 2024-05-05 06:25:40.491887 rer.solrpush-1.4.0/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2747 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.471153 rer.solrpush-1.4.0/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.475422 rer.solrpush-1.4.0/src/rer/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.477764 rer.solrpush-1.4.0/src/rer/solrpush/
+-rw-r--r--   0 cekk       (501) staff       (20)      130 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.478276 rer.solrpush-1.4.0/src/rer/solrpush/adapters/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/adapters/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      353 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/adapters/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1433 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/adapters/file.py
+-rw-r--r--   0 cekk       (501) staff       (20)      705 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/adapters/rss_feed.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.478638 rer.solrpush-1.4.0/src/rer/solrpush/behaviors/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/behaviors/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      497 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/behaviors/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1143 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/behaviors/solr_fields.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.479639 rer.solrpush-1.4.0/src/rer/solrpush/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3598 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3297 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1195 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/elevate_settings.py
+-rw-r--r--   0 cekk       (501) staff       (20)    16305 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/maintenance.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.479771 rer.solrpush-1.4.0/src/rer/solrpush/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)     8883 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/overrides/plone.app.contenttypes.browser.templates.listing.pt
+-rw-r--r--   0 cekk       (501) staff       (20)      350 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/query_debug.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6510 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/querybuilder.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2317 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/scales.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.480553 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.471742 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/dist/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.481889 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/dist/dev/
+-rw-r--r--   0 cekk       (501) staff       (20)  2311368 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/dist/dev/main.js
+-rw-r--r--   0 cekk       (501) staff       (20)  1783747 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/dist/dev/main.js.map
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.483073 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/dist/prod/
+-rw-r--r--   0 cekk       (501) staff       (20)   294024 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/dist/prod/main.js
+-rw-r--r--   0 cekk       (501) staff       (20)      159 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/dist/prod/main.js.map
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.483178 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.483289 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/FacetsContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     1025 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/FacetsContainer/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.483393 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/ProgressBar/
+-rw-r--r--   0 cekk       (501) staff       (20)      946 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/ProgressBar/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.483507 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     1737 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)      455 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)      258 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/package.json
+-rw-r--r--   0 cekk       (501) staff       (20)      618 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/styles.css
+-rw-r--r--   0 cekk       (501) staff       (20)      174 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/styles.css.map
+-rw-r--r--   0 cekk       (501) staff       (20)      431 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/styles.scss
+-rw-r--r--   0 cekk       (501) staff       (20)    57992 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/static/yarn.lock
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.483829 rer.solrpush-1.4.0/src/rer/solrpush/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)     1822 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/templates/controlpanel_layout.pt
+-rw-r--r--   0 cekk       (501) staff       (20)      498 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/templates/query_debug.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1453 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/browser/templates/reindex_solr.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     2425 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     4077 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/indexer.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.484438 rer.solrpush-1.4.0/src/rer/solrpush/interfaces/
+-rw-r--r--   0 cekk       (501) staff       (20)      389 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/interfaces/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      389 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/interfaces/adapter.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3336 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/interfaces/elevate.py
+-rw-r--r--   0 cekk       (501) staff       (20)      372 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/interfaces/layer.py
+-rw-r--r--   0 cekk       (501) staff       (20)      153 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/interfaces/queueprocessor.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6666 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/interfaces/settings.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.484930 rer.solrpush-1.4.0/src/rer/solrpush/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/locales/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.472333 rer.solrpush-1.4.0/src/rer/solrpush/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.485152 rer.solrpush-1.4.0/src/rer/solrpush/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.mo
+-rw-r--r--   0 cekk       (501) staff       (20)    11576 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.472451 rer.solrpush-1.4.0/src/rer/solrpush/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.485364 rer.solrpush-1.4.0/src/rer/solrpush/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     9290 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.mo
+-rw-r--r--   0 cekk       (501) staff       (20)    16728 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.po
+-rw-r--r--   0 cekk       (501) staff       (20)    11694 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/locales/rer.solrpush.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1528 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      473 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)     7068 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/parser.py
+-rw-r--r--   0 cekk       (501) staff       (20)      447 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.472886 rer.solrpush-1.4.0/src/rer/solrpush/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.486008 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      854 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/actions.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      162 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      953 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      257 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.486315 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)      891 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/registry/bundle.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     2828 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/registry/criteria.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      278 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/registry/settings.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      480 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.486420 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/types/
+-rw-r--r--   0 cekk       (501) staff       (20)      299 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/types/Document.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.486630 rer.solrpush-1.4.0/src/rer/solrpush/profiles/to_1100/
+-rw-r--r--   0 cekk       (501) staff       (20)      232 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/to_1100/componentregistry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)       97 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/to_1100/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.486837 rer.solrpush-1.4.0/src/rer/solrpush/profiles/to_1300/
+-rw-r--r--   0 cekk       (501) staff       (20)      322 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/to_1300/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      211 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/to_1300/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.487144 rer.solrpush-1.4.0/src/rer/solrpush/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      122 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      536 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      605 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/profiles/uninstall/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.487427 rer.solrpush-1.4.0/src/rer/solrpush/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      716 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      978 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/controlpanel.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.487736 rer.solrpush-1.4.0/src/rer/solrpush/restapi/deserializer/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/deserializer/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      208 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/deserializer/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      584 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/deserializer/controlpanel.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.487965 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      205 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.488311 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/elevate_schema/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/elevate_schema/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      363 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/elevate_schema/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      355 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/elevate_schema/get.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.488921 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/solr_search/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/solr_search/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3873 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/solr_search/batch.py
+-rw-r--r--   0 cekk       (501) staff       (20)      353 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/solr_search/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      919 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/solr_search/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3065 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/solr_search/solr_search_handler.py
+-rw-r--r--   0 cekk       (501) staff       (20)      610 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5230 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.490352 rer.solrpush-1.4.0/src/rer/solrpush/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.490840 rer.solrpush-1.4.0/src/rer/solrpush/tests/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     6207 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/docs/example.docx
+-rw-r--r--   0 cekk       (501) staff       (20)     8355 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/docs/example.ods
+-rw-r--r--   0 cekk       (501) staff       (20)    13430 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/docs/example.pdf
+-rw-r--r--   0 cekk       (501) staff       (20)    14135 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/docs/plone_logo.png
+-rw-r--r--   0 cekk       (501) staff       (20)     2077 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_behaviors.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4336 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_elevate.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6395 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_events.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3132 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_image_tags.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6358 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_maintenance.py
+-rw-r--r--   0 cekk       (501) staff       (20)     9341 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_querybuilder.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5044 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_restapi_search.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5984 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_search.py
+-rw-r--r--   0 cekk       (501) staff       (20)    14834 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_solr_interface.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3132 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_tika.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3700 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/tests/test_vocabularies.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2214 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2433 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/upgrades.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.491320 rer.solrpush-1.4.0/src/rer/solrpush/utils/
+-rw-r--r--   0 cekk       (501) staff       (20)      345 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/utils/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3832 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/utils/solr_common.py
+-rw-r--r--   0 cekk       (501) staff       (20)     9270 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/utils/solr_indexer.py
+-rw-r--r--   0 cekk       (501) staff       (20)    10943 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/utils/solr_search.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1633 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer/solrpush/vocabularies.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2024-05-05 06:25:40.476476 rer.solrpush-1.4.0/src/rer.solrpush.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)    13289 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer.solrpush.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     5619 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer.solrpush.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer.solrpush.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      117 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer.solrpush.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer.solrpush.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer.solrpush.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      254 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer.solrpush.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2024-05-05 06:25:40.000000 rer.solrpush-1.4.0/src/rer.solrpush.egg-info/top_level.txt
```

### Comparing `rer.solrpush-1.3.3/CHANGES.rst` & `rer.solrpush-1.4.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.4.0 (2024-05-05)
+------------------
+
+- Plone6 compatibility.
+  [cekk]
+
+
 1.3.3 (2023-11-08)
 ------------------
 
 - Fix RSS Feed.
   [cekk]
 
 1.3.2 (2023-11-08)
```

### Comparing `rer.solrpush-1.3.3/DEVELOP.rst` & `rer.solrpush-1.4.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/LICENSE.GPL` & `rer.solrpush-1.4.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/LICENSE.rst` & `rer.solrpush-1.4.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/MANIFEST.in` & `rer.solrpush-1.4.0/MANIFEST.in`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 graft src/rer
 graft docs
 include *.rst
+include *.txt
 include LICENSE.GPL
 include *.yml
 global-exclude *.pyc
 prune config
 prune .github
 exclude .babelrc
 exclude .eslintrc.json
```

### Comparing `rer.solrpush-1.3.3/PKG-INFO` & `rer.solrpush-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: rer.solrpush
-Version: 1.3.3
+Version: 1.4.0
 Summary: Prodotto per Regione Emilia-Romagna relativo all'indicizzazione dei contenuti con solr
 Home-page: https://github.com/collective/rer.solrpush
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.solrpush
 Project-URL: Source, https://github.com/collective/rer.solrpush
 Project-URL: Tracker, https://github.com/collective/rer.solrpush/issues
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: ==2.7
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 ============
 rer.solrpush
 ============
@@ -237,14 +240,21 @@
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
 
+1.4.0 (2024-05-05)
+------------------
+
+- Plone6 compatibility.
+  [cekk]
+
+
 1.3.3 (2023-11-08)
 ------------------
 
 - Fix RSS Feed.
   [cekk]
 
 1.3.2 (2023-11-08)
```

### Comparing `rer.solrpush-1.3.3/README.rst` & `rer.solrpush-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/docs/Solr-Push_Configurazione.jpg` & `rer.solrpush-1.4.0/docs/Solr-Push_Configurazione.jpg`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/docs/rer-logo.png` & `rer.solrpush-1.4.0/docs/rer-logo.png`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/publiccode.yml` & `rer.solrpush-1.4.0/publiccode.yml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/setup.py` & `rer.solrpush-1.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,28 +12,31 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="rer.solrpush",
-    version="1.3.3",
+    version="1.4.0",
     description="Prodotto per Regione Emilia-Romagna relativo all'indicizzazione dei contenuti con solr",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
+        "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.1",
         "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords="Python Plone",
     author="RedTurtle",
     author_email="sviluppoplone@redturtle.it",
     url="https://github.com/collective/rer.solrpush",
@@ -45,22 +48,23 @@
     },
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup"]),
     namespace_packages=["rer"],
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    python_requires="==2.7",
+    python_requires=">=3.7",
     install_requires=[
         "setuptools",
         "collective.z3cform.jsonwidget",
         "plone.api>=1.8.4",
         "pysolr",
         'ftfy==4.4.3;python_version<="2.7"',
         "plone.restapi",
+        "z3c.jbot",
     ],
     extras_require={
         "test": [
             "plone.app.testing",
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/adapters/file.py` & `rer.solrpush-1.4.0/src/rer/solrpush/adapters/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # -*- coding: utf-8 -*-
 from plone import api
 from rer.solrpush.interfaces.adapter import IExtractFileFromTika
 from zope.interface import implementer
 
+
 try:
     from collective.limitfilesizepanel.interfaces import ILimitFileSizePanel
 
     HAS_LFSP = True
 except ImportError:
     HAS_LFSP = False
 
 import logging
 
+
 logger = logging.getLogger(__name__)
 
 
 @implementer(IExtractFileFromTika)
 class FileExtractor(object):
     def __init__(self, context):
         self.context = context
@@ -30,16 +32,15 @@
                 if file_size:
                     max_size = file_size
             except Exception:
                 pass  # we use our default
         return max_size * 1024 * 1024
 
     def get_file_to_index(self):
-        """
-        """
+        """ """
         file_obj = getattr(self.context, "file", None)
         if not file_obj:
             return None
         max_size = self.maxfilesize()
         if file_obj.getSize() > max_size:
             logger.warning(
                 "Maximun file size reached (%s > %s) for %s %s",
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/adapters/rss_feed.py` & `rer.solrpush-1.4.0/src/rer/solrpush/adapters/rss_feed.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from zope.component import adapter
 from zope.interface import implementer
 
 
 @implementer(IFeedItem)
 @adapter(ISolrBrain, IFeed)
 class SOLRFeedItem(BaseItem):
-
     @property
     def link(self):
         return self.context.getURL()
 
     @property
     def title(self):
         return self.context.Title
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/behaviors/solr_fields.py` & `rer.solrpush-1.4.0/src/rer/solrpush/behaviors/solr_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,27 @@
         "categorization", fields=["showinsearch", "searchwords"]
     )
 
     showinsearch = schema.Bool(
         required=False,
         default=True,
         missing_value=True,
-        title=_("label_showinsearch", default=u"Show in search"),
+        title=_("label_showinsearch", default="Show in search"),
         description=_("help_showinsearch", default=""),
     )
 
     searchwords = schema.List(
         required=False,
         default=[],
         missing_value=[],
-        title=_("label_searchwords", default=u"Search words"),
+        title=_("label_searchwords", default="Search words"),
         value_type=schema.TextLine(),
         description=_(
             "help_searchwords",
-            u"Specify words for which this item will show up "
-            u"as the first search result. Multiple words can be "
-            u"specified on new lines.",
+            "Specify words for which this item will show up "
+            "as the first search result. Multiple words can be "
+            "specified on new lines.",
         ),
     )
 
 
 # EOF
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/configure.zcml` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/configure.zcml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:browser="http://namespaces.zope.org/browser"
     xmlns:plone="http://namespaces.plone.org/plone"
-    i18n_domain="rer.solrpush">
+    i18n_domain="rer.solrpush"
+    >
+
+  <!-- Set overrides folder for Just-a-Bunch-Of-Templates product -->
+  <include
+      package="z3c.jbot"
+      file="meta.zcml"
+      />
+  <browser:jbot
+      directory="overrides"
+      layer="rer.solrpush.interfaces.IRerSolrpushLayer"
+      />
 
   <plone:static
+      directory="static"
       name="rer.solrpush"
       type="plone"
-      directory="static"
       />
 
   <!-- controlpanel -->
   <browser:page
       name="solrpush-settings"
       for="Products.CMFPlone.interfaces.IPloneSiteRoot"
       class=".controlpanel.RerSolrpushSettingsView"
@@ -23,89 +34,89 @@
       for="Products.CMFPlone.interfaces.IPloneSiteRoot"
       class=".elevate_settings.ElevateSettingsView"
       permission="rer.solrpush.editElevate"
       layer="rer.solrpush.interfaces.IRerSolrpushLayer"
       />
 
   <browser:page
-    for="Products.CMFCore.interfaces.ISiteRoot"
-    name="reindex-solr"
-    permission="cmf.ManagePortal"
-    class=".maintenance.ReindexSolrView"
-    template="templates/reindex_solr.pt"
-    layer="rer.solrpush.interfaces.IRerSolrpushLayer"
-    />
-    <browser:page
-    for="Products.CMFCore.interfaces.ISiteRoot"
-    name="sync-solr"
-    permission="cmf.ManagePortal"
-    class=".maintenance.SyncSolrView"
-    template="templates/reindex_solr.pt"
-    layer="rer.solrpush.interfaces.IRerSolrpushLayer"
-    />
-
-   <browser:page
-        for="Products.CMFCore.interfaces.ISiteRoot"
-        name="reindex-progress"
-        permission="cmf.ManagePortal"
-        class=".maintenance.ReindexProgressView"
-        layer="rer.solrpush.interfaces.IRerSolrpushLayer"
-    />
-    <browser:page
-        for="Products.CMFCore.interfaces.ISiteRoot"
-        name="do-reindex"
-        permission="cmf.ManagePortal"
-        class=".maintenance.DoReindexView"
-        layer="rer.solrpush.interfaces.IRerSolrpushLayer"
-    />
-    <browser:page
-        for="Products.CMFCore.interfaces.ISiteRoot"
-        name="do-sync"
-        permission="cmf.ManagePortal"
-        class=".maintenance.DoSyncView"
-        layer="rer.solrpush.interfaces.IRerSolrpushLayer"
-    />
-    
-    <browser:page
-          for="Products.CMFCore.interfaces.ISiteRoot"
-          name="reset-solr"
-          permission="cmf.ManagePortal"
-          class=".maintenance.ResetSolr"
-          layer="rer.solrpush.interfaces.IRerSolrpushLayer"
-          />
+      name="reindex-solr"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      class=".maintenance.ReindexSolrView"
+      template="templates/reindex_solr.pt"
+      permission="cmf.ManagePortal"
+      layer="rer.solrpush.interfaces.IRerSolrpushLayer"
+      />
+  <browser:page
+      name="sync-solr"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      class=".maintenance.SyncSolrView"
+      template="templates/reindex_solr.pt"
+      permission="cmf.ManagePortal"
+      layer="rer.solrpush.interfaces.IRerSolrpushLayer"
+      />
 
-    <!-- return scaled image -->
-    <browser:page
+  <browser:page
+      name="reindex-progress"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      class=".maintenance.ReindexProgressView"
+      permission="cmf.ManagePortal"
+      layer="rer.solrpush.interfaces.IRerSolrpushLayer"
+      />
+  <browser:page
+      name="do-reindex"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      class=".maintenance.DoReindexView"
+      permission="cmf.ManagePortal"
+      layer="rer.solrpush.interfaces.IRerSolrpushLayer"
+      />
+  <browser:page
+      name="do-sync"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      class=".maintenance.DoSyncView"
+      permission="cmf.ManagePortal"
+      layer="rer.solrpush.interfaces.IRerSolrpushLayer"
+      />
+
+  <browser:page
+      name="reset-solr"
+      for="Products.CMFCore.interfaces.ISiteRoot"
+      class=".maintenance.ResetSolr"
+      permission="cmf.ManagePortal"
+      layer="rer.solrpush.interfaces.IRerSolrpushLayer"
+      />
+
+  <!-- return scaled image -->
+  <!-- <browser:page
         name="solr-images"
         class=".scales.SolrImages"
         permission="zope2.View"
         for="*"
         layer="rer.solrpush.interfaces.IRerSolrpushLayer"
-        />
+        /> -->
 
-    <!-- CUSTOM COLLECTIONS -->
-    <browser:page
-        name="querybuilderresults"
-        class=".querybuilder.QueryBuilder"
-        permission="zope2.View"
-        for="*"
-        layer="rer.solrpush.interfaces.IRerSolrpushLayer"
-        />
-    <browser:page
-        name="querybuilder_html_results"
-        class=".querybuilder.QueryBuilder"
-        permission="zope2.View"
-        attribute="html_results"
-        for="*"
-        layer="rer.solrpush.interfaces.IRerSolrpushLayer"
-        />
+  <!-- CUSTOM COLLECTIONS -->
+  <browser:page
+      name="querybuilderresults"
+      for="*"
+      class=".querybuilder.QueryBuilder"
+      permission="zope2.View"
+      layer="rer.solrpush.interfaces.IRerSolrpushLayer"
+      />
+  <browser:page
+      name="querybuilder_html_results"
+      for="*"
+      class=".querybuilder.QueryBuilder"
+      attribute="html_results"
+      permission="zope2.View"
+      layer="rer.solrpush.interfaces.IRerSolrpushLayer"
+      />
 
-    <browser:viewlet
-        name="solrpush.querydebug"
-        manager="plone.app.layout.viewlets.interfaces.IBelowContent"
-        class=".query_debug.QueryDebug"
-        permission="cmf.ManagePortal"
-        template="templates/query_debug.pt"
-        layer="rer.solrpush.interfaces.IRerSolrpushLayer"
-        />
+  <browser:viewlet
+      name="solrpush.querydebug"
+      manager="plone.app.layout.viewlets.interfaces.IBelowContent"
+      class=".query_debug.QueryDebug"
+      template="templates/query_debug.pt"
+      permission="cmf.ManagePortal"
+      layer="rer.solrpush.interfaces.IRerSolrpushLayer"
+      />
 
 </configure>
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/controlpanel.py` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/controlpanel.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,43 +11,44 @@
 from z3c.form import button
 from z3c.form import field
 from z3c.form import group
 from z3c.form.interfaces import HIDDEN_MODE
 
 import logging
 
+
 logger = logging.getLogger(__name__)
 
 
 class FormDefault(group.Group):
-    label = _("settings_default_label", default=u"Settings")
+    label = _("settings_default_label", default="Settings")
     fields = field.Fields(IRerSolrpushConf)
 
 
 class FormSearch(group.Group):
-    label = _("settings_search_label", default=u"Search")
+    label = _("settings_search_label", default="Search")
     description = _(
         "settings_search_help",
-        default=u"Use these settings to tweak search results.",
+        default="Use these settings to tweak search results.",
     )
     fields = field.Fields(IRerSolrpushSearchConf)
 
 
 class RerSolrpushEditForm(RegistryEditForm):
     """Nel form del pannello di controllo mettiamo anche le logiche per
     il caricamento
     """
 
     schema = IRerSolrpushSettings
     groups = (FormDefault, FormSearch)
-    label = _(u"Solr Push Configuration")
+    label = _("Solr Push Configuration")
 
     formErrorsMessage = _(
         "settings_form_error",
-        default=u"Sono presenti degli errori, si prega di ricontrollare i dati inseriti",
+        default="Sono presenti degli errori, si prega di ricontrollare i dati inseriti",
     )
 
     def updateFields(self):
         super(RerSolrpushEditForm, self).updateFields()
         for form_group in self.groups:
             if "ready" in form_group.fields:
                 form_group.fields["ready"].mode = HIDDEN_MODE
@@ -55,23 +56,23 @@
     @button.buttonAndHandler(_("Save"), name=None)
     def handleSave(self, action):
         data, errors = self.extractData()
         if errors:
             self.status = self.formErrorsMessage
             return
         self.applyChanges(data)
-        api.portal.show_message(_(u"Changes saved."), request=self.request)
+        api.portal.show_message(_("Changes saved."), request=self.request)
         init_error = init_solr_push()
         if init_error:
             api.portal.show_message(
                 init_error, type="error", request=self.request
             )
         else:
             api.portal.show_message(
-                _(u"Loaded schema.xml from SOLR"), request=self.request
+                _("Loaded schema.xml from SOLR"), request=self.request
             )
         self.request.response.redirect(self.request.getURL())
 
     @button.buttonAndHandler(_("Cancel"), name="cancel")
     def handleCancel(self, action):
         super(RerSolrpushEditForm, self).handleCancel(self, action)
 
@@ -82,15 +83,15 @@
         init_error = init_solr_push()
         if init_error:
             api.portal.show_message(
                 init_error, type="error", request=self.request
             )
         else:
             api.portal.show_message(
-                _(u"Reloaded schema.xml from SOLR"), request=self.request
+                _("Reloaded schema.xml from SOLR"), request=self.request
             )
         self.request.response.redirect(self.request.getURL())
 
 
 class RerSolrpushSettingsView(ControlPanelFormWrapper):
     form = RerSolrpushEditForm
     index = ViewPageTemplateFile("templates/controlpanel_layout.pt")
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/elevate_settings.py` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/elevate_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,25 @@
 from rer.solrpush import _
 from rer.solrpush.interfaces import IElevateSettings
 from rer.solrpush.interfaces.elevate import IElevateRowSchema
 from z3c.form import field
 
 
 class ElevateSettingsEditForm(RegistryEditForm):
-
     schema = IElevateSettings
     label = _(
         "solr_elevate_configuration_label",
-        default=u"Solr Push Elevate Configuration",
+        default="Solr Push Elevate Configuration",
     )
 
     fields = field.Fields(IElevateSettings)
     fields["elevate_schema"].widgetFactory = JSONFieldWidget
 
     def updateWidgets(self):
-        """
-        """
+        """ """
         super(ElevateSettingsEditForm, self).updateWidgets()
         self.widgets["elevate_schema"].schema = IElevateRowSchema
 
 
 class ElevateSettingsView(ControlPanelFormWrapper):
     form = ElevateSettingsEditForm
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/maintenance.py` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/maintenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,40 +41,39 @@
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 def timer(func=time):
-    """ set up a generator returning the elapsed time since the last call """
+    """set up a generator returning the elapsed time since the last call"""
 
     def gen(last=func()):
         while True:
             elapsed = func() - last
             last = func()
             yield "%.3fs" % elapsed
 
     return gen()
 
 
 class SolrMaintenanceBaseForm(form.Form):
-
     # template = ViewPageTemplateFile('templates/reindex_solr.pt')
 
     ignoreContext = True
 
-    @button.buttonAndHandler(_("start_label", default=u"Start"))
+    @button.buttonAndHandler(_("start_label", default="Start"))
     def handleApply(self, action):
         data, errors = self.extractData()
         if errors:
             self.status = self.formErrorsMessage
             return
         self.do_action()
 
-    @button.buttonAndHandler(_("cancel_label", default=u"Cancel"))
+    @button.buttonAndHandler(_("cancel_label", default="Cancel"))
     def handleCancel(self, action):
         msg_label = _("maintenance_cancel_action", default="Action cancelled")
         api.portal.show_message(message=msg_label, request=self.request)
         return self.request.response.redirect(
             "{}/@@solrpush-settings".format(api.portal.get().absolute_url())
         )
 
@@ -104,16 +103,16 @@
 
 class ReindexBaseView(BrowserView):
     @property
     def solr_error_message(self):
         return translate(
             _(
                 "solr_error_connection",
-                default=u"There have been problems connecting to SOLR. "
-                u"Contact site administrator.",
+                default="There have been problems connecting to SOLR. "
+                "Contact site administrator.",
             ),
             context=self.request,
         )
 
     def setupAnnotations(self, items_len, message):
         annotations = IAnnotations(api.portal.get())
         annotations["solr_reindex"] = PersistentDict(
@@ -311,23 +310,30 @@
         indexed = []
         not_indexed = []
         removed = []
         if not disable_progress:
             status = self.setupAnnotations(
                 items_len=len(brains_to_sync), message="Sync contents to SOLR"
             )
+        i = 0
+        tot = len(brains_to_sync)
         for brain in brains_to_sync:
+            i += 1
+            if i % 10 == 0:
+                logger.info(f"Progress: {i}/{tot}")
             if not disable_progress:
                 status["counter"] = status["counter"] + 1
                 commit()
             item = brain.getObject()
             if brain.UID not in solr_items:
                 # missing from solr: try to index it
                 try:
+                    logger.info("send to solr")
                     res = push_to_solr(item)
+                    logger.info("received response from solr")
                     if res:
                         indexed.append(brain.getPath())
                 except SolrError as e:
                     not_indexed.append(
                         {"path": brain.getPath(), "message": e.__str__()}
                     )
                 except Exception as e:
@@ -361,15 +367,15 @@
             "removed": removed,
         }
 
 
 class DoReindexView(ReindexBaseView):
     def __call__(self):
         authenticator = getMultiAdapter(
-            (self.context, self.request), name=u"authenticator"
+            (self.context, self.request), name="authenticator"
         )
         if not authenticator.verify():
             raise Unauthorized
         # disable noisy logging from pysolr
         debug = os.environ.get("DEBUG_SOLR", "").lower() not in ("true", "1")
         if debug:
             pysolr_logger = logging.getLogger("pysolr")
@@ -383,15 +389,15 @@
             pt_logger.setLevel(logging.INFO)
 
 
 class DoSyncView(ReindexBaseView):
     def __call__(self, cron_view=False):
         if not cron_view:
             authenticator = getMultiAdapter(
-                (self.context, self.request), name=u"authenticator"
+                (self.context, self.request), name="authenticator"
             )
             if not authenticator.verify():
                 raise Unauthorized
         # disable noisy logging from pysolr
         if os.environ.get("DEBUG_SOLR", "").lower() not in ("true", "1"):
             pysolr_logger = logging.getLogger("pysolr")
             pt_logger = logging.getLogger("PortalTransforms")
@@ -453,24 +459,22 @@
 
     @property
     def is_active(self):
         return is_solr_active()
 
 
 class ReindexSolrView(ReactView):
-
     label = _("maintenance_reindex_label", default="Reindex SOLR")
     description = _(
         "maintenance_reindex_help",
         default="Get all Plone contents and reindex them on SOLR.",
     )
     action = "do-reindex"
 
 
 class SyncSolrView(ReactView):
-
     label = _("maintenance_sync_label", default="Sync SOLR")
     description = _(
         "maintenance_sync_help",
         default="Remove no more existing contents from SOLR and sync with Plone.",  # noqa
     )
     action = "do-sync"
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/querybuilder.py` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/querybuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from plone.app.querystring import queryparser
 from plone.app.querystring.interfaces import IParsedQueryIndexModifier
 from plone.app.querystring.interfaces import IQueryModifier
 from plone.app.querystring.querybuilder import QueryBuilder as BaseView
 from plone.batching import Batch
 from Products.CMFCore.utils import getToolByName
 from rer.solrpush.parser import SolrResponse
-from rer.solrpush.utils.solr_indexer import get_site_title
 from rer.solrpush.utils import search as solr_search
+from rer.solrpush.utils.solr_indexer import get_site_title
 from zope.component import getUtilitiesFor
 
-
 import logging
 
 
 SORT_ON_MAPPING = {"sortable_title": "Title"}
 
 logger = logging.getLogger(__name__)
 
@@ -39,14 +38,15 @@
         query_modifiers = getUtilitiesFor(IQueryModifier)
         for name, modifier in sorted(query_modifiers, key=itemgetter(0)):
             query = modifier(query)
 
         parsedquery = queryparser.parseFormquery(
             self.context, query, sort_on, sort_order
         )
+
         index_modifiers = getUtilitiesFor(IParsedQueryIndexModifier)
         for name, modifier in index_modifiers:
             if name in parsedquery:
                 new_name, query = modifier(parsedquery[name])
                 parsedquery[name] = query
                 # if a new index name has been returned, we need to replace
                 # the native ones
@@ -77,29 +77,36 @@
             parsedquery["sort_limit"] = limit
 
         if "path" not in parsedquery:
             parsedquery["path"] = {"query": ""}
 
         if isinstance(custom_query, dict) and custom_query:
             # Update the parsed query with an extra query dictionary. This may
-            # override the parsed query. The custom_query is a dictonary of
+            # override the parsed query. The custom_query is a dictionary of
             # index names and their associated query values.
-            parsedquery.update(custom_query)
+            for key in custom_query:
+                if isinstance(parsedquery.get(key), dict) and isinstance(
+                    custom_query.get(key), dict
+                ):
+                    parsedquery[key].update(custom_query[key])
+                    continue
+                parsedquery[key] = custom_query[key]
             empty_query = False
 
         # filter bad term and operator in query
         parsedquery = self.filter_query(parsedquery)
         results = []
 
         # RER.SOLRPUSH PATCH
         search_with_solr = False
         if "searchWithSolr" in parsedquery:
             if parsedquery["searchWithSolr"]["query"]:
                 search_with_solr = True
             del parsedquery["searchWithSolr"]
+
         if not empty_query:
             if search_with_solr:
                 if "SearchableText" in parsedquery:
                     if isinstance(parsedquery["SearchableText"], dict):
                         parsedquery["SearchableText"]["query"] = parsedquery[
                             "SearchableText"
                         ]["query"].rstrip("*")
@@ -112,16 +119,16 @@
                         **self.clean_query_for_solr(query=parsedquery)
                     )
                 )
             else:
                 results = catalog(**parsedquery)
             if (
                 getattr(results, "actual_result_count", False)
-                and limit  # noqa
-                and results.actual_result_count > limit  # noqa
+                and limit
+                and results.actual_result_count > limit
             ):
                 results.actual_result_count = limit
 
         if not brains and not search_with_solr:
             results = IContentListing(results)
         if batch:
             results = Batch(results, b_size, start=b_start)
@@ -133,15 +140,15 @@
         for k, v in query.items():
             if k == "sort_on":
                 fixed_query[k] = SORT_ON_MAPPING.get(v, v)
             elif k == "path":
                 portal_state = api.content.get_view(
                     context=self.context,
                     request=self.request,
-                    name=u"plone_portal_state",
+                    name="plone_portal_state",
                 )
                 root_path = portal_state.navigation_root_path()
                 path = self.extract_value(v)
                 if len(path) == 1 and path[0].rstrip("/") == root_path:
                     if "solr_sites" not in query.keys():
                         filtered_sites.append(get_site_title())
                 else:
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/scales.py` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/scales.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
+from plone import api
 from Products.Five.browser import BrowserView
-from zope.publisher.interfaces import IPublishTraverse
 from zope.interface import implementer
-from plone import api
+from zope.publisher.interfaces import IPublishTraverse
 
 import six
 
 
 class SolrScalesHandler(BrowserView):
     """
     View callable on SolrBrain contents that mimic @@images.
@@ -31,15 +31,15 @@
         if six.PY2:
             title = title.encode("utf-8")
             alt = alt.encode("utf-8")
 
         # needed for cache invalidation
         date = self.context.modified.strftime("%Y%m%d%H%M%S")
 
-        html = '<img src="{url}/@@solr-images/{fieldname}/{scale}?direction={direction}&v={date}" alt="{alt}" title="{title}" loading="{loading}"'.format(
+        html = '<img src="{url}/@@images/{fieldname}/{scale}?direction={direction}&v={date}" alt="{alt}" title="{title}" loading="{loading}"'.format(
             url=self.context.getURL(),
             fieldname=fieldname or "image",
             scale=scale or "thumb",
             alt=alt,
             title=title,
             loading=loading,
             direction=direction,
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/static/dist/dev/main.js` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/static/dist/dev/main.js`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/static/dist/dev/main.js.map` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/static/dist/dev/main.js.map`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/static/dist/prod/main.js` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/static/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/FacetsContainer/index.js` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/FacetsContainer/index.js`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/ProgressBar/index.js` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/ProgressBar/index.js`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/index.js` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/index.js`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/static/styles.css` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/static/styles.css`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/static/yarn.lock` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/static/yarn.lock`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/templates/controlpanel_layout.pt` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/templates/controlpanel_layout.pt`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/browser/templates/reindex_solr.pt` & `rer.solrpush-1.4.0/src/rer/solrpush/browser/templates/reindex_solr.pt`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/configure.zcml` & `rer.solrpush-1.4.0/src/rer/solrpush/configure.zcml`

 * *Files 4% similar despite different names*

```diff
@@ -1,81 +1,88 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
     xmlns:i18n="http://namespaces.zope.org/i18n"
     xmlns:plone="http://namespaces.plone.org/plone"
-    i18n_domain="rer.solrpush">
+    i18n_domain="rer.solrpush"
+    >
 
   <i18n:registerTranslations directory="locales" />
   <include file="permissions.zcml" />
 
   <include package=".adapters" />
   <include package=".behaviors" />
   <include package=".browser" />
   <include package=".restapi" />
-  
+
 
   <include file="upgrades.zcml" />
 
   <genericsetup:registerProfile
       name="default"
       title="RER: Solr push"
-      directory="profiles/default"
       description="Installs the rer.solrpush add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/default"
       post_handler=".setuphandlers.post_install"
       />
 
   <genericsetup:registerProfile
       name="uninstall"
       title="RER: Solr push (uninstall)"
-      directory="profiles/uninstall"
       description="Uninstalls the rer.solrpush add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/uninstall"
       post_handler=".setuphandlers.uninstall"
       />
-  
+
   <genericsetup:registerProfile
       name="to_1100"
       title="RER: Solr push remove persistent utility"
-      directory="profiles/to_1100"
       description=""
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/to_1100"
       />
 
   <genericsetup:registerProfile
       name="to_1300"
       title="RER: Solr push remove unused control panel"
-      directory="profiles/to_1300"
       description=""
       provides="Products.GenericSetup.interfaces.EXTENSION"
+      directory="profiles/to_1300"
       />
-  
+
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="rer.solrpush-hiddenprofiles"
       />
-    
 
-    <!-- vocabularies -->
-    <utility
-        name="rer.solrpush.vocabularies.AvailableSites"
-        component=".vocabularies.AvailableSitesVocabulary"
-    />
-    <utility
-        name="rer.solrpush.vocabularies.AvailableSubjects"
-        component=".vocabularies.AvailableSubjectsVocabulary"
-    />
-    <utility
-        name="rer.solrpush.vocabularies.AvailablePortalTypes"
-        component=".vocabularies.AvailablePortalTypesVocabulary"
-    />
-
-    <!-- indexers -->
-    <utility
-        factory=".indexer.SolrIndexProcessor" 
-        name="solrpush.utility"
-        />
-    <adapter name="path_depth" factory=".indexer.path_depth" />
-    <adapter name="path_parents" factory=".indexer.path_parents" />
+
+  <!-- vocabularies -->
+  <utility
+      name="rer.solrpush.vocabularies.AvailableSites"
+      component=".vocabularies.AvailableSitesVocabulary"
+      />
+  <utility
+      name="rer.solrpush.vocabularies.AvailableSubjects"
+      component=".vocabularies.AvailableSubjectsVocabulary"
+      />
+  <utility
+      name="rer.solrpush.vocabularies.AvailablePortalTypes"
+      component=".vocabularies.AvailablePortalTypesVocabulary"
+      />
+
+  <!-- indexers -->
+  <utility
+      factory=".indexer.SolrIndexProcessor"
+      name="solrpush.utility"
+      />
+  <adapter
+      factory=".indexer.path_depth"
+      name="path_depth"
+      />
+  <adapter
+      factory=".indexer.path_parents"
+      name="path_parents"
+      />
 
 </configure>
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/indexer.py` & `rer.solrpush-1.4.0/src/rer/solrpush/indexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,17 +90,17 @@
                         push_to_solr(data)
                     elif iop == UNINDEX:
                         remove_from_solr(uid)
                 except SolrError:
                     logger.exception("error indexing %s %s", iop, uid)
                     message = _(
                         "content_indexed_error",
-                        default=u"There was a problem indexing or unindexing "
-                        u"this content. Please take note of this address and "
-                        u"contact site administrator.",
+                        default="There was a problem indexing or unindexing "
+                        "this content. Please take note of this address and "
+                        "contact site administrator.",
                     )
                     api.portal.show_message(
                         message=message, request=getRequest(), type="warning"
                     )
             self.queue = []
 
     def abort(self):
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/interfaces/elevate.py` & `rer.solrpush-1.4.0/src/rer/solrpush/interfaces/elevate.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from plone.app.z3cform.widget import RelatedItemsFieldWidget
 from plone.autoform import directives as form
 from plone.supermodel import model
 from rer.solrpush import _
 from z3c.relationfield.schema import RelationChoice
 from z3c.relationfield.schema import RelationList
 from zope import schema
+from zope.globalrequest import getRequest
 from zope.i18n import translate
 from zope.interface import Invalid
 from zope.interface import invariant
-from zope.globalrequest import getRequest
 
 import json
 
 
 class CatalogSource(CatalogSourceBase):
     """
     Without this hack, validation doesn't pass
@@ -22,27 +22,27 @@
 
     def __contains__(self, value):
         return True  # Always contains to allow lazy handling of removed objs
 
 
 class IElevateRowSchema(model.Schema):
     text = schema.List(
-        title=_("elevate_row_schema_text_label", default=u"Text"),
+        title=_("elevate_row_schema_text_label", default="Text"),
         description=_(
             "elevate_row_schema_text_help",
-            default=u"The word that should match in the search.",
+            default="The word that should match in the search.",
         ),
         required=True,
         value_type=schema.TextLine(),
     )
     uid = RelationList(
-        title=_("elevate_row_schema_uid_label", u"Elements"),
+        title=_("elevate_row_schema_uid_label", "Elements"),
         description=_(
             "elevate_row_schema_uid_help",
-            u"Select a list of elements to elevate for that search word.",
+            "Select a list of elements to elevate for that search word.",
         ),
         value_type=RelationChoice(vocabulary="plone.app.vocabularies.Catalog"),
         required=True,
     )
     form.widget(
         "uid",
         RelatedItemsFieldWidget,
@@ -50,18 +50,18 @@
     )
 
 
 class IElevateSettings(model.Schema):
     """ """
 
     elevate_schema = schema.SourceText(
-        title=_(u"elevate_schema_label", default=u"Elevate configuration"),
+        title=_("elevate_schema_label", default="Elevate configuration"),
         description=_(
-            u"elevate_schema_help",
-            default=u"Insert a list of values for elevate.",
+            "elevate_schema_help",
+            default="Insert a list of values for elevate.",
         ),
         required=False,
     )
 
     @invariant
     def elevate_invariant(data):
         schema = json.loads(data.elevate_schema)
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/interfaces/settings.py` & `rer.solrpush-1.4.0/src/rer/solrpush/interfaces/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,180 +15,180 @@
 
     def __contains__(self, value):
         return True  # Always contains to allow lazy handling of removed objs
 
 
 class IElevateRowSchema(model.Schema):
     text = schema.TextLine(
-        title=_("elevate_row_schema_text_label", default=u"Text"),
+        title=_("elevate_row_schema_text_label", default="Text"),
         description=_(
             "elevate_row_schema_text_help",
-            default=u"The word that should match in the search.",
+            default="The word that should match in the search.",
         ),
         required=True,
     )
     uid = schema.List(
-        title=_("elevate_row_schema_uid_label", u"Elements"),
+        title=_("elevate_row_schema_uid_label", "Elements"),
         description=_(
             "elevate_row_schema_uid_help",
-            u"Select a list of elements to elevate for that search word.",
+            "Select a list of elements to elevate for that search word.",
         ),
         value_type=schema.Choice(source=CatalogSource()),
         required=True,
     )
     form.widget("uid", RelatedItemsFieldWidget)
 
 
 class IRerSolrpushConf(model.Schema):
     """"""
 
     active = schema.Bool(
-        title=_(u"Active"),
-        description=_(u"Enable SOLR indexing on this site."),
+        title=_("Active"),
+        description=_("Enable SOLR indexing on this site."),
         required=False,
         default=False,
     )
     search_enabled = schema.Bool(
-        title=_(u"Search enabled"),
+        title=_("Search enabled"),
         description=_(
-            u"Site search will use SOLR as engine instead portal_catalog."
+            "Site search will use SOLR as engine instead portal_catalog."
         ),
         required=False,
         default=True,
     )
     force_commit = schema.Bool(
-        title=_(u"Force commit"),
+        title=_("Force commit"),
         description=_(
-            u"Force commits on CRUD operations. If enabled, each indexing "
-            u"operation to SOLR will be immediately committed and persisted. "
-            u"This means that updates are immediately available on SOLR queries."  # noqa
-            u"If you are using SolrCloud with ZooKeeper, immediate commits "
-            u"will slow down response performances when indexing, so it's "
-            u"better to turn it off. In this case updates will be available "
-            u"when SOLR periodically commit changes."
+            "Force commits on CRUD operations. If enabled, each indexing "
+            "operation to SOLR will be immediately committed and persisted. "
+            "This means that updates are immediately available on SOLR queries."  # noqa
+            "If you are using SolrCloud with ZooKeeper, immediate commits "
+            "will slow down response performances when indexing, so it's "
+            "better to turn it off. In this case updates will be available "
+            "when SOLR periodically commit changes."
         ),
         required=False,
         default=True,
     )
 
     solr_url = schema.TextLine(
-        title=_(u"SOLR url"),
-        description=_(u"The SOLR core to connect to."),
+        title=_("SOLR url"),
+        description=_("The SOLR core to connect to."),
         required=True,
     )
 
     frontend_url = schema.TextLine(
-        title=_(u"Frontend url"),
-        description=_(u"If the website has different URL for frontend users."),
+        title=_("Frontend url"),
+        description=_("If the website has different URL for frontend users."),
         required=False,
     )
 
     enabled_types = schema.List(
-        title=_(u"enabled_types_label", default=u"Enabled portal types"),
+        title=_("enabled_types_label", default="Enabled portal types"),
         description=_(
-            u"enabled_types_help",
-            default=u"Select a list of portal types to index in solr. "
-            u"Empty list means that all portal types will be indexed.",
+            "enabled_types_help",
+            default="Select a list of portal types to index in solr. "
+            "Empty list means that all portal types will be indexed.",
         ),
         required=False,
         default=[],
         missing_value=[],
         value_type=schema.Choice(
             vocabulary="plone.app.vocabularies.PortalTypes"
         ),
     )
 
     index_fields = schema.SourceText(
         title=_(
             "index_fields_label",
-            default=u"List of fields loaded from SOLR that we use for "
-            u"indexing.",
+            default="List of fields loaded from SOLR that we use for "
+            "indexing.",
         ),
         description=_(
-            u"index_fields_help",
-            default=u"We store this list for performance"
-            u" reasons. If the configuration changes, you need to click on"
-            u" Reload button",
+            "index_fields_help",
+            default="We store this list for performance"
+            " reasons. If the configuration changes, you need to click on"
+            " Reload button",
         ),
         required=False,
     )
     # NASCOSTO DAL PANNELLO DI CONTROLLO (vedi: browser/controlpanel.py)
     ready = schema.Bool(
-        title=_(u"Ready"),
-        description=_(u"SOLR push is ready to be used."),
+        title=_("Ready"),
+        description=_("SOLR push is ready to be used."),
         required=False,
         default=False,
     )
 
 
 class IRerSolrpushSearchConf(model.Schema):
     query_debug = schema.Bool(
-        title=_(u"Query debug"),
+        title=_("Query debug"),
         description=_(
-            u"If enabled, when a search to SOLR is performed (for "
-            u"example in Collection), the query will be showed in the page for "
-            u"debug. Only visible to Managers."
+            "If enabled, when a search to SOLR is performed (for "
+            "example in Collection), the query will be showed in the page for "
+            "debug. Only visible to Managers."
         ),
         required=False,
         default=False,
     )
     remote_elevate_schema = schema.TextLine(
-        title=_(u"remote_elevate_label", default=u"Remote elevate"),
+        title=_("remote_elevate_label", default="Remote elevate"),
         description=_(
-            u"remote_elevate_help",
-            default=u'If this field is set and no "site_name" is '
-            u"passed in query, elevate schema is taken from an external "
-            u"source. This is useful if you index several sites and handle "
-            u"elevate configuration in one single site. This should be an url "
-            u'that points to "@elevate-schema" view.'
-            u"For example: http://my-site/@elevate-schema.",
+            "remote_elevate_help",
+            default='If this field is set and no "site_name" is '
+            "passed in query, elevate schema is taken from an external "
+            "source. This is useful if you index several sites and handle "
+            "elevate configuration in one single site. This should be an url "
+            'that points to "@elevate-schema" view.'
+            "For example: http://my-site/@elevate-schema.",
         ),
-        default=u"",
+        default="",
         required=False,
     )
     qf = schema.TextLine(
-        title=_("qf_label", default=u"qf (query fields)"),
+        title=_("qf_label", default="qf (query fields)"),
         description=_(
             "qf_help",
-            default=u"Set a list of fields, each of which is assigned a boost "
-            u"factor to increase or decrease that particular field’s "
-            u"importance in the query. "
-            u"For example: fieldOne^1000.0 fieldTwo fieldThree^10.0",
+            default="Set a list of fields, each of which is assigned a boost "
+            "factor to increase or decrease that particular field’s "
+            "importance in the query. "
+            "For example: fieldOne^1000.0 fieldTwo fieldThree^10.0",
         ),
         required=False,
-        default=u"",
+        default="",
     )
     bq = schema.TextLine(
-        title=_("bq_label", default=u"bq (boost query)"),
+        title=_("bq_label", default="bq (boost query)"),
         description=_(
             "bq_help",
-            default=u"Set a list query clauses that will be added to the main "
-            u"query to influence the score. For example if we want to boost "
-            u'results that have a specific "searchwords" term: '
-            u"searchwords:something^1000",
+            default="Set a list query clauses that will be added to the main "
+            "query to influence the score. For example if we want to boost "
+            'results that have a specific "searchwords" term: '
+            "searchwords:something^1000",
         ),
         required=False,
-        default=u"",
+        default="",
     )
 
     bf = schema.TextLine(
-        title=_("bf_label", default=u"bf (boost functions)"),
+        title=_("bf_label", default="bf (boost functions)"),
         description=_(
             "bf_help",
-            default=u"Set a list of functions (with optional boosts) that "
-            u"will be used to construct FunctionQueries which will be added "
-            u"to the main query as optional clauses that will influence the "
-            u"score. Any function supported natively by Solr can be used, "
-            u"along with a boost value. "
-            u"For example if we want to give less relevance to "
-            u"items deeper in the tree we can set something like this: "
-            u"recip(path_depth,10,100,1)",
+            default="Set a list of functions (with optional boosts) that "
+            "will be used to construct FunctionQueries which will be added "
+            "to the main query as optional clauses that will influence the "
+            "score. Any function supported natively by Solr can be used, "
+            "along with a boost value. "
+            "For example if we want to give less relevance to "
+            "items deeper in the tree we can set something like this: "
+            "recip(path_depth,10,100,1)",
         ),
         required=False,
-        default=u"",
+        default="",
     )
 
 
 class IRerSolrpushSettings(IRerSolrpushConf, IRerSolrpushSearchConf):
     """
     Marker interface for settings
     """
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/locales/README.rst` & `rer.solrpush-1.4.0/src/rer/solrpush/locales/README.rst`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.po` & `rer.solrpush-1.4.0/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.po`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.mo` & `rer.solrpush-1.4.0/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.mo`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.po` & `rer.solrpush-1.4.0/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.po`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/locales/rer.solrpush.pot` & `rer.solrpush-1.4.0/src/rer/solrpush/locales/rer.solrpush.pot`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/locales/update.py` & `rer.solrpush-1.4.0/src/rer/solrpush/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/parser.py` & `rer.solrpush-1.4.0/src/rer/solrpush/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,41 +7,46 @@
 from rer.solrpush.interfaces.adapter import ISolrBrain
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
 from rer.solrpush.utils.solr_indexer import get_index_fields
 from rer.solrpush.utils.solr_indexer import get_site_title
 from zope.globalrequest import getRequest
 from zope.interface import implementer
 
+
 try:
     from ZTUtils.Lazy import Lazy
 except ImportError:
     from Products.ZCatalog.Lazy import Lazy
 
 try:
     from design.plone.theme.interfaces import IDesignPloneThemeLayer
 
     HAS_RER_THEME = True
 except ImportError:
     HAS_RER_THEME = False
 
+import json
 import os
 import six
 
+
 timezone = DateTime().timezone()
 
 
 @implementer(ISolrBrain)
 class Brain(dict):
     """a dictionary with attribute access"""
 
     def __repr__(self):
         return "<SolrBrain for {}>".format(self.getPath())
 
     def __getattr__(self, name):
         """look up attributes in dict"""
+        if name not in self.keys():
+            return None
         marker = []
         value = self.get(name, marker)
         schema = get_index_fields()
         if value is not marker:
             field_schema = schema.get(name, {})
             if field_schema.get("type", "") == "date":
                 # dates are stored in SOLR as UTC
@@ -67,15 +72,15 @@
 
     @property
     def Description(self):
         return self.get("description", "")
 
     def absolute_url(self):
         """convenience alias"""
-        return self.getUrl()
+        return self.getURL()
 
     @property
     def Date(self):
         if self.EffectiveDate().startswith("1969"):
             return self.CreationDate()
         return self.EffectiveDate()
 
@@ -161,14 +166,43 @@
         return mimeicon
 
     def restrictedTraverse(self, name):
         if name == "@@images":
             return SolrScalesHandler(self, getRequest())
         return None
 
+    @property
+    def image_scales(self):
+        scales = json.loads(self.get("image_scales", "{}"))
+        if scales:
+            return scales
+
+        # backward compatibility with < Plone6 indexed contents
+        if not self.get("getIcon", False):
+            return {}
+
+        return {
+            "image": [
+                {
+                    "download": "@@images/image",
+                    "scales": {
+                        "preview": {
+                            "download": "@@images/image/preview",
+                        },
+                        "thumb": {
+                            "download": "@@images/image/thumb",
+                        },
+                        "mini": {
+                            "download": "@@images/image/mini",
+                        },
+                    },
+                }
+            ]
+        }
+
 
 class SolrResults(list):
     """a list of results returned from solr, i.e. sol(a)r flares"""
 
 
 def parseDate(value):
     """use `DateTime` to parse a date, but take care of solr 1.4
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/actions.xml` & `rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/controlpanel.xml` & `rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/controlpanel.xml`

 * *Files 16% similar despite different names*

#### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/controlpanel.xml` & `rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/controlpanel.xml`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
 <object xmlns:i18n="http://xml.zope.org/namespaces/i18n" name="portal_controlpanel" i18n:domain="rer.bandisolr">
-  <configlet title="Configurazione RER SolrPush" action_id="solrpush.configuration" appId="solrpush" category="Products" condition_expr="" url_expr="string:${portal_url}/@@solrpush-settings" icon_expr="" visible="True" i18n:attributes="title">
+  <configlet title="Configurazione RER SolrPush" action_id="SolrPushSettings" appId="SolrPushSettings" category="Products" condition_expr="" url_expr="string:${portal_url}/@@solrpush-settings" icon_expr="" visible="True" i18n:attributes="title">
     <permission>rer.solrpush: Edit Settings</permission>
   </configlet>
-  <configlet title="Configurazione Elevate" action_id="solrpush.elevate" appId="solrpush-elevate" category="Products" condition_expr="" url_expr="string:${portal_url}/@@elevate-settings" icon_expr="" visible="True" i18n:attributes="title">
+  <configlet title="Configurazione Elevate" action_id="SolrPushElevate" appId="SolrPushElevate" category="Products" condition_expr="" url_expr="string:${portal_url}/@@elevate-settings" icon_expr="" visible="True" i18n:attributes="title">
     <permission>rer.solrpush: Edit Elevate</permission>
   </configlet>
 </object>
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/registry/bundle.xml` & `rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/registry/bundle.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/profiles/default/registry/criteria.xml` & `rer.solrpush-1.4.0/src/rer/solrpush/profiles/default/registry/criteria.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/profiles/uninstall/controlpanel.xml` & `rer.solrpush-1.4.0/src/rer/solrpush/profiles/uninstall/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/profiles/uninstall/registry.xml` & `rer.solrpush-1.4.0/src/rer/solrpush/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/solr_search/batch.py` & `rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/solr_search/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,16 +53,15 @@
         qs = self.request["QUERY_STRING"]
         if qs:
             url = "?".join((url, qs))
         return url
 
     @property
     def links(self):
-        """Get a dictionary with batching links.
-        """
+        """Get a dictionary with batching links."""
         # Don't provide batching links if resultset isn't batched
         if self.hits <= self.b_size:
             return None
 
         links = {}
 
         last = self._last_page()
@@ -78,16 +77,15 @@
 
         if prev:
             links["prev"] = self._url_for_batch(prev)
 
         return links
 
     def _url_for_batch(self, pagenumber):
-        """Return a new Batch object for the given pagenumber.
-        """
+        """Return a new Batch object for the given pagenumber."""
         new_start = pagenumber * self.b_size
         return self._url_with_params(params={"b_start": new_start})
 
     def _last_page(self):
         page = self.hits / self.b_size
         if self.hits % self.b_size == 0:
             return page - 1
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/solr_search/get.py` & `rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/solr_search/get.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
+from plone import api
+from plone.restapi.search.handler import SearchHandler
 from plone.restapi.search.utils import unflatten_dotted_dict
 from plone.restapi.services import Service
+from rer.solrpush.interfaces.settings import IRerSolrpushSettings
 from rer.solrpush.restapi.services.solr_search.solr_search_handler import (
     SolrSearchHandler,
 )
-from plone.restapi.search.handler import SearchHandler
-from rer.solrpush.interfaces.settings import IRerSolrpushSettings
-from plone import api
 
 
 class SearchGet(Service):
     def reply(self):
         query = self.request.form.copy()
         query = unflatten_dotted_dict(query)
         handler = SearchHandler
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/restapi/services/solr_search/solr_search_handler.py` & `rer.solrpush-1.4.0/src/rer/solrpush/restapi/services/solr_search/solr_search_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from copy import deepcopy
-from Products.CMFCore.utils import getToolByName
+from plone.restapi.deserializer import boolean_value
 from plone.restapi.search.handler import SearchHandler as BaseHandler
-from rer.solrpush.utils import search as solr_search
+from Products.CMFCore.utils import getToolByName
 from rer.solrpush.restapi.services.solr_search.batch import SolrHypermediaBatch
-from plone.restapi.deserializer import boolean_value
+from rer.solrpush.utils import search as solr_search
+
 
 DEFAULT_METADATA_FIELDS = set(
     ["@id", "@type", "description", "review_state", "title"]
 )
 FIELD_ACCESSORS = {
     "@id": "getURL",
     "@type": "PortalType",
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/setuphandlers.py` & `rer.solrpush-1.4.0/src/rer/solrpush/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/testing.py` & `rer.solrpush-1.4.0/src/rer/solrpush/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import os
 import plone.restapi
 import rer.solrpush
 import six
 import subprocess
 import sys
 
+
 BIN_DIR = os.path.dirname(os.path.realpath(sys.argv[0]))
 
 
 class SolrLayer(Layer):
     """Solr test layer that fires up and shuts down a Solr instance. This
     layer can be used to unit test a Solr configuration without having to
     fire up Plone.
@@ -42,15 +43,15 @@
         solr_port=8983,
         solr_base="/solr/solrpush_test",
     ):
         super(SolrLayer, self).__init__(bases, name, module)
         self.solr_host = solr_host
         self.solr_port = solr_port
         self.solr_base = solr_base
-        self.solr_url = u"http://{0}:{1}{2}".format(
+        self.solr_url = "http://{0}:{1}{2}".format(
             solr_host, solr_port, solr_base
         )
 
     def setUp(self):
         """Start Solr and poll until it is up and running."""
         self.proc = subprocess.call(
             "./solr-start", shell=True, close_fds=True, cwd=BIN_DIR
@@ -92,17 +93,17 @@
     defaultBases = (PLONE_APP_CONTENTTYPES_FIXTURE,)
 
     def __init__(
         self,
         bases=None,
         name="SolrPush Layer",
         module=None,
-        solr_host=u"localhost",
+        solr_host="localhost",
         solr_port=8983,
-        solr_base=u"/solr/solrpush_test",
+        solr_base="/solr/solrpush_test",
     ):
         super(PloneSandboxLayer, self).__init__(bases, name, module)
         self.solr_host = solr_host
         self.solr_port = solr_port
         self.solr_base = solr_base
         # SolrLayer should use the same settings as CollectiveSolrLayer
         self.solr_layer = SolrLayer(
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/docs/example.docx` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/docs/example.docx`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/docs/example.ods` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/docs/example.ods`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/docs/example.pdf` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/docs/example.pdf`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/docs/plone_logo.png` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/docs/plone_logo.png`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_behaviors.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_behaviors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 """Setup tests for this package."""
 from plone import api
 from plone.api.portal import set_registry_record
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
-from rer.solrpush.utils import init_solr_push
-from rer.solrpush.utils import reset_solr
-from rer.solrpush.utils import search
 from rer.solrpush.testing import (
     RER_SOLRPUSH_API_FUNCTIONAL_TESTING,
 )  # noqa: E501
+from rer.solrpush.utils import init_solr_push
+from rer.solrpush.utils import reset_solr
+from rer.solrpush.utils import search
 from transaction import commit
 
 import unittest
 
 
 class TestShowInSearch(unittest.TestCase):
     """Test show in search field behavior."""
@@ -27,15 +27,15 @@
         always empty on setUp.
         """
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record(
             "enabled_types",
-            [u"Document", u"News Item"],
+            ["Document", "News Item"],
             interface=IRerSolrpushSettings,
         )
         init_solr_push()
         self.document = api.content.create(
             container=self.portal, type="Document", title="Document foo"
         )
         api.content.transition(obj=self.document, transition="publish")
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_elevate.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_elevate.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,40 +2,38 @@
 """Setup tests for this package."""
 from plone import api
 from plone.api.portal import set_registry_record
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from rer.solrpush.interfaces import IElevateSettings
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
+from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 from rer.solrpush.utils import init_solr_push
 from rer.solrpush.utils import reset_solr
 from rer.solrpush.utils import search
-from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 from transaction import commit
 
-import unittest
 import json
 import six
+import unittest
 
 
 class TestSolrSearch(unittest.TestCase):
-    """
-    """
+    """ """
 
     layer = RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 
     def setUp(self):
-        """
-        """
+        """ """
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record(
             "enabled_types",
-            [u"Document", u"News Item"],
+            ["Document", "News Item"],
             interface=IRerSolrpushSettings,
         )
 
         init_solr_push()
         commit()
         self.doc1 = api.content.create(
             container=self.portal,
@@ -74,15 +72,15 @@
         api.content.transition(obj=self.published_news, transition="publish")
         api.content.transition(obj=self.event, transition="publish")
         commit()
 
     def tearDown(self):
         set_registry_record("active", True, interface=IRerSolrpushSettings)
         #  reset elevate
-        set_registry_record("elevate_schema", u"", interface=IElevateSettings)
+        set_registry_record("elevate_schema", "", interface=IElevateSettings)
         reset_solr()
         commit()
 
     def test_search_with_elevate(self):
         doc3 = api.content.create(
             container=self.portal, type="Document", title="Third page"
         )
@@ -100,19 +98,21 @@
         self.assertEqual(len(solr_results), 4)
         self.assertEqual(
             solr_results[0],
             {"UID": doc4.UID(), "Title": doc4.Title(), "[elevated]": False},
         )
 
         # now let's set an elevate for third document
-        value = json.dumps([{"text": [u"page"], "uid": [{"UID": doc3.UID()}]}])
+        value = json.dumps([{"text": ["page"], "uid": [{"UID": doc3.UID()}]}])
         if six.PY2:
             value = value.decode("utf-8")
         set_registry_record(
-            "elevate_schema", value, interface=IElevateSettings,
+            "elevate_schema",
+            value,
+            interface=IElevateSettings,
         )
         solr_results = search(
             query={"SearchableText": "page"}, fl=["UID", "Title", "[elevated]"]
         ).docs
         self.assertEqual(len(solr_results), 4)
         self.assertEqual(
             solr_results[0],
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_events.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 """Setup tests for this package."""
 from plone import api
 from plone.api.portal import get_registry_record
 from plone.api.portal import set_registry_record
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
-from rer.solrpush.utils import init_solr_push
 from rer.solrpush.testing import (
     RER_SOLRPUSH_API_FUNCTIONAL_TESTING,
 )  # noqa: E501
+from rer.solrpush.utils import init_solr_push
+from rer.solrpush.utils import reset_solr
 from transaction import commit
 from zope.event import notify
 from zope.lifecycleevent import ObjectModifiedEvent
-from rer.solrpush.utils import reset_solr
 
 import requests
 import unittest
 
+
 try:
     from Products.CMFPlone.utils import get_installer
 except ImportError:
     get_installer = None
 
 
 class TestSOLRPush(unittest.TestCase):
@@ -32,15 +33,15 @@
     def setUp(self):
         """Custom shared utility setup for tests."""
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record(
             "enabled_types",
-            [u"Document", u"File"],
+            ["Document", "File"],
             interface=IRerSolrpushSettings,
         )
 
     def tearDown(self):
         set_registry_record("active", True, interface=IRerSolrpushSettings)
         reset_solr()
 
@@ -77,15 +78,15 @@
     def setUp(self):
         """Custom shared utility setup for tests."""
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record(
             "enabled_types",
-            [u"Document", u"File"],
+            ["Document", "File"],
             interface=IRerSolrpushSettings,
         )
         init_solr_push()
 
     def tearDown(self):
         set_registry_record("active", True, interface=IRerSolrpushSettings)
         reset_solr()
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_image_tags.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_image_tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 """Setup tests for this package."""
 from plone import api
 from plone.api.portal import set_registry_record
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.namedfile.file import NamedFile
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
+from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 from rer.solrpush.utils import init_solr_push
 from rer.solrpush.utils import reset_solr
 from rer.solrpush.utils import search
-from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 from transaction import commit
 
-import unittest
 import os
+import unittest
 
 
 class TestTika(unittest.TestCase):
     """Test solr indexing for files"""
 
     layer = RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         """Custom shared utility setup for tests."""
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record(
-            "enabled_types", [u"File"], interface=IRerSolrpushSettings
+            "enabled_types", ["File"], interface=IRerSolrpushSettings
         )
         init_solr_push()
         commit()
 
     def tearDown(self):
         set_registry_record("active", True, interface=IRerSolrpushSettings)
         reset_solr()
@@ -47,39 +47,39 @@
         file_item = api.content.create(
             container=self.portal, type="File", title=filename, file=item_file
         )
         commit()
         return file_item
 
     def test_index_and_extract_pdf(self):
-        file_item = self.create_file_item(u"example.pdf")
+        file_item = self.create_file_item("example.pdf")
 
         solr_results = search(query={"*": "*"}, fl="UID")
         self.assertEqual(solr_results.hits, 1)
         st_results = search(query={"SearchablesText": "lorem"}, fl="UID")
         self.assertEqual(st_results.hits, 1)
         self.assertEqual(file_item.UID(), st_results.docs[0]["UID"])
 
     def test_index_and_extract_docx(self):
-        file_item = self.create_file_item(u"example.docx")
+        file_item = self.create_file_item("example.docx")
 
         solr_results = search(query={"*": "*"}, fl="UID SearchableText")
         self.assertEqual(solr_results.hits, 1)
         st_results = search(query={"SearchableText": "ipsum"}, fl="UID")
         self.assertEqual(st_results.hits, 1)
         self.assertEqual(file_item.UID(), st_results.docs[0]["UID"])
 
     def test_index_and_extract_ods(self):
-        file_item = self.create_file_item(u"example.ods")
+        file_item = self.create_file_item("example.ods")
 
         solr_results = search(query={"*": "*"}, fl="UID SearchableText")
         self.assertEqual(solr_results.hits, 1)
         st_results = search(query={"SearchableText": "yyy"}, fl="UID")
         self.assertEqual(st_results.hits, 1)
         self.assertEqual(file_item.UID(), st_results.docs[0]["UID"])
 
     def test_indexed_file_has_right_mimetype(self):
-        self.create_file_item(u"example.pdf")
+        self.create_file_item("example.pdf")
 
         solr_results = search(query={"*": "*"}, fl="UID mime_type")
         self.assertEqual(solr_results.hits, 1)
         self.assertEqual(solr_results.docs[0]["mime_type"], "application/pdf")
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_maintenance.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_maintenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 from plone import api
 from plone.api.portal import get_registry_record
 from plone.api.portal import set_registry_record
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.protect.authenticator import createToken
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
-from rer.solrpush.utils import init_solr_push
-from rer.solrpush.utils import reset_solr
-from rer.solrpush.utils import search
 from rer.solrpush.testing import (
     RER_SOLRPUSH_API_FUNCTIONAL_TESTING,
 )  # noqa: E501
+from rer.solrpush.utils import init_solr_push
+from rer.solrpush.utils import reset_solr
+from rer.solrpush.utils import search
 from transaction import commit
 
 import unittest
 
+
 try:
     from Products.CMFPlone.utils import get_installer
 except ImportError:
     get_installer = None
 
 
 class TestMaintenance(unittest.TestCase):
@@ -35,15 +36,15 @@
         always empty on setUp.
         """
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record("active", False, interface=IRerSolrpushSettings)
         set_registry_record(
-            "enabled_types", [u"Document"], interface=IRerSolrpushSettings
+            "enabled_types", ["Document"], interface=IRerSolrpushSettings
         )
         get_registry_record("enabled_types", interface=IRerSolrpushSettings)
         self.published_doc = api.content.create(
             container=self.portal, type="Document", title="Published Document"
         )
         api.content.transition(obj=self.published_doc, transition="publish")
         self.unpublished_doc = api.content.create(
@@ -121,45 +122,45 @@
     def test_maintenance_reindex_with_unwanted_types(self):
         self.reindex_view()
         solr_results = search(query={"*": "*", "b_size": 100000}, fl="UID")
         self.assertEqual(solr_results.hits, 1)
 
         set_registry_record(
             "enabled_types",
-            [u"Document", u"News Item"],
+            ["Document", "News Item"],
             interface=IRerSolrpushSettings,
         )
         api.content.transition(obj=self.news, transition="publish")
         api.content.transition(obj=self.unpublished_doc, transition="publish")
         commit()
         solr_results = search(
             query={"*": "*", "b_size": 100000}, fl="UID,portal_type"
         )
         self.assertEqual(solr_results.hits, 3)
 
         set_registry_record(
-            "enabled_types", [u"Document"], interface=IRerSolrpushSettings
+            "enabled_types", ["Document"], interface=IRerSolrpushSettings
         )
         self.reindex_view()
         solr_results = search(query={"*": "*", "b_size": 100000}, fl="UID")
         # News isn't removed because reindex view only reindex values from
         # Plone
         self.assertEqual(solr_results.hits, 3)
 
     def test_maintenance_sync(self):
         api.content.transition(obj=self.news, transition="publish")
         api.content.transition(obj=self.unpublished_doc, transition="publish")
         set_registry_record(
             "enabled_types",
-            [u"Document", u"News Item"],
+            ["Document", "News Item"],
             interface=IRerSolrpushSettings,
         )
         self.reindex_view()
         solr_results = search(query={"*": "*", "b_size": 100000}, fl="UID")
         self.assertEqual(solr_results.hits, 3)
 
         set_registry_record(
-            "enabled_types", [u"Document"], interface=IRerSolrpushSettings
+            "enabled_types", ["Document"], interface=IRerSolrpushSettings
         )
         self.sync_view()
         solr_results = search(query={"*": "*", "b_size": 100000}, fl="UID")
         self.assertEqual(solr_results.hits, 2)
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_querybuilder.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_querybuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 """Setup tests for this package."""
 from plone import api
 from plone.api.portal import set_registry_record
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.namedfile.file import NamedBlobImage
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
-from rer.solrpush.utils.solr_common import init_solr_push
-from rer.solrpush.utils.solr_common import get_solr_connection
-from rer.solrpush.utils import push_to_solr
 from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
+from rer.solrpush.utils import push_to_solr
+from rer.solrpush.utils.solr_common import get_solr_connection
+from rer.solrpush.utils.solr_common import init_solr_push
 from transaction import commit
 
-import unittest
 import os
+import unittest
 
 
 class TestCollections(unittest.TestCase):
     """Test show in search field behavior."""
 
     layer = RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 
@@ -27,15 +27,15 @@
         always empty on setUp.
         """
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record(
             "enabled_types",
-            [u"Document", u"News Item"],
+            ["Document", "News Item"],
             interface=IRerSolrpushSettings,
         )
         init_solr_push()
         commit()
         # set_registry_record("active", True, interface=IRerSolrpushSettings)
         self.docs = {}
         for i in range(20):
@@ -76,17 +76,17 @@
             api.content.transition(obj=obj, transition="publish")
 
         commit()
 
     def tearDown(self):
         solr = get_solr_connection()
         solr.delete(q="*:*", commit=True)
-        set_registry_record("qf", u"", interface=IRerSolrpushSettings)
-        set_registry_record("bq", u"", interface=IRerSolrpushSettings)
-        set_registry_record("bf", u"", interface=IRerSolrpushSettings)
+        set_registry_record("qf", "", interface=IRerSolrpushSettings)
+        set_registry_record("bq", "", interface=IRerSolrpushSettings)
+        set_registry_record("bf", "", interface=IRerSolrpushSettings)
         commit()
 
     def get_results(
         self,
         query,
         batch=True,
         sort_order="",
@@ -235,38 +235,38 @@
         ]
         results = self.get_results(query=query)
         self.assertEqual(results.sequence_length, 1)
 
         item = results[0]
         self.assertEqual(
             item.restrictedTraverse("@@images").tag(),
-            '<img src="{url}/@@solr-images/image/thumb?direction=thumbnail&v={date}" alt="News with image" title="News with image" loading="lazy">'.format(
+            '<img src="{url}/@@images/image/thumb?direction=thumbnail&v={date}" alt="News with image" title="News with image" loading="lazy">'.format(
                 url=news.absolute_url(),
                 date=news.modified().strftime("%Y%m%d%H%M%S"),
             ),
         )
 
         self.assertEqual(
             item.restrictedTraverse("@@images").tag(
                 alt="alt text", title="custom title"
             ),
-            '<img src="{url}/@@solr-images/image/thumb?direction=thumbnail&v={date}" alt="alt text" title="custom title" loading="lazy">'.format(
+            '<img src="{url}/@@images/image/thumb?direction=thumbnail&v={date}" alt="alt text" title="custom title" loading="lazy">'.format(
                 url=news.absolute_url(),
                 date=news.modified().strftime("%Y%m%d%H%M%S"),
             ),
         )
 
         self.assertEqual(
             item.restrictedTraverse("@@images").tag(css_class="custom-css"),
-            '<img src="{url}/@@solr-images/image/thumb?direction=thumbnail&v={date}" alt="News with image" title="News with image" loading="lazy" class="custom-css">'.format(
+            '<img src="{url}/@@images/image/thumb?direction=thumbnail&v={date}" alt="News with image" title="News with image" loading="lazy" class="custom-css">'.format(
                 url=news.absolute_url(),
                 date=news.modified().strftime("%Y%m%d%H%M%S"),
             ),
         )
 
         self.assertEqual(
             item.restrictedTraverse("@@images").tag(scale="mini"),
-            '<img src="{url}/@@solr-images/image/mini?direction=thumbnail&v={date}" alt="News with image" title="News with image" loading="lazy">'.format(
+            '<img src="{url}/@@images/image/mini?direction=thumbnail&v={date}" alt="News with image" title="News with image" loading="lazy">'.format(
                 url=news.absolute_url(),
                 date=news.modified().strftime("%Y%m%d%H%M%S"),
             ),
         )
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_restapi_search.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_restapi_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 from plone.app.testing import TEST_USER_ID
 from plone.restapi.testing import RelativeSession
 from Products.CMFCore.utils import getToolByName
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
 from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 from rer.solrpush.utils import init_solr_push
 from rer.solrpush.utils import reset_solr
-
 from transaction import commit
+
 import unittest
 
 
 class SearchBandiTest(unittest.TestCase):
-
     layer = RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.portal_url = self.portal.absolute_url()
         self.catalog = getToolByName(self.portal, "portal_catalog")
@@ -33,15 +32,15 @@
         self.api_session.headers.update({"Accept": "application/json"})
         self.api_session.auth = (SITE_OWNER_NAME, SITE_OWNER_PASSWORD)
 
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
         set_registry_record(
             "enabled_types",
-            [u"Document", u"News Item"],
+            ["Document", "News Item"],
             interface=IRerSolrpushSettings,
         )
 
         init_solr_push()
         commit()
 
         self.doc1 = api.content.create(
@@ -91,37 +90,49 @@
             True,
             interface=IRerSolrpushSettings,
         )
         reset_solr()
         commit()
 
     def test_search_works(self):
-
         solr_response = self.api_session.get("/@solr-search")
         plone_response = self.api_session.get("/@search")
         solr_results = solr_response.json()
         plone_results = plone_response.json()
-        self.assertEqual(plone_results[u"items_total"], 6)
-        self.assertEqual(solr_results[u"items_total"], 3)
+        if api.env.plone_version() < "6.0":
+            self.assertEqual(plone_results["items_total"], 6)
+        else:
+            # there is also Plone Site in results
+            self.assertEqual(plone_results["items_total"], 7)
+        self.assertEqual(solr_results["items_total"], 3)
 
     def test_disable_search_will_perform_classic_search(self):
-
         solr_response = self.api_session.get("/@solr-search")
         plone_response = self.api_session.get("/@search")
         solr_results = solr_response.json()
         plone_results = plone_response.json()
-        self.assertEqual(plone_results[u"items_total"], 6)
-        self.assertEqual(solr_results[u"items_total"], 3)
+
+        if api.env.plone_version() < "6.0":
+            self.assertEqual(plone_results["items_total"], 6)
+        else:
+            # there is also Plone Site in results
+            self.assertEqual(plone_results["items_total"], 7)
+        self.assertEqual(solr_results["items_total"], 3)
 
         set_registry_record(
             "search_enabled",
             False,
             interface=IRerSolrpushSettings,
         )
         commit()
 
         solr_response = self.api_session.get("/@solr-search")
         plone_response = self.api_session.get("/@search")
         solr_results = solr_response.json()
         plone_results = plone_response.json()
-        self.assertEqual(plone_results[u"items_total"], 6)
-        self.assertEqual(solr_results[u"items_total"], 6)
+        if api.env.plone_version() < "6.0":
+            self.assertEqual(plone_results["items_total"], 6)
+            self.assertEqual(solr_results["items_total"], 6)
+        else:
+            # there is also Plone Site in results
+            self.assertEqual(plone_results["items_total"], 7)
+            self.assertEqual(solr_results["items_total"], 7)
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_search.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 """Setup tests for this package."""
 from plone import api
 from plone.api.portal import set_registry_record
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
+from rer.solrpush.testing import (
+    RER_SOLRPUSH_API_FUNCTIONAL_TESTING,
+)  # noqa: E501
 from rer.solrpush.utils import init_solr_push
 from rer.solrpush.utils import reset_solr
 from rer.solrpush.utils import search
 from rer.solrpush.utils.solr_search import escape_special_characters
-from rer.solrpush.testing import (
-    RER_SOLRPUSH_API_FUNCTIONAL_TESTING,
-)  # noqa: E501
 from transaction import commit
 
 import unittest
 
 
 class TestSearch(unittest.TestCase):
     """Test show in search field behavior."""
@@ -28,15 +28,15 @@
         always empty on setUp.
         """
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record(
             "enabled_types",
-            [u"Document", u"News Item"],
+            ["Document", "News Item"],
             interface=IRerSolrpushSettings,
         )
         init_solr_push()
         # set_registry_record("active", True, interface=IRerSolrpushSettings)
         self.docs = {}
         for i in range(20):
             searchwords = []
@@ -58,17 +58,17 @@
             )
             # obj.reindexObject(idxs=['Title'])
             api.content.transition(obj=obj, transition="publish")
         commit()
 
     def tearDown(self):
         reset_solr()
-        set_registry_record("qf", u"", interface=IRerSolrpushSettings)
-        set_registry_record("bq", u"", interface=IRerSolrpushSettings)
-        set_registry_record("bf", u"", interface=IRerSolrpushSettings)
+        set_registry_record("qf", "", interface=IRerSolrpushSettings)
+        set_registry_record("bq", "", interface=IRerSolrpushSettings)
+        set_registry_record("bf", "", interface=IRerSolrpushSettings)
         commit()
 
     def test_all_items(self):
         solr_results = search(query={}, fl="UID")
         self.assertEqual(solr_results.hits, len(self.docs))
 
     def test_search_odd(self):
@@ -78,44 +78,44 @@
     def test_search_qf(self):
         solr_results = search(query={"": "odd"}, fl=["UID", "id", "Title"])
         self.assertEqual(solr_results.hits, len(self.docs) / 2)
         self.assertNotEqual(solr_results.docs[0]["id"], "odd")
 
         set_registry_record(
             "qf",
-            u"id^1000.0 SearchableText^1.0",
+            "id^1000.0 SearchableText^1.0",
             interface=IRerSolrpushSettings,
         )
         commit()
         solr_results = search(query={"": "odd"}, fl=["UID", "id", "Title"])
         self.assertEqual(solr_results.hits, len(self.docs) / 2)
         self.assertEqual(solr_results.docs[0]["id"], "odd")
 
     def test_search_qf_for_searchwords(self):
         solr_results = search(query={"": "odd"}, fl=["UID", "id", "Title"])
         self.assertEqual(solr_results.hits, len(self.docs) / 2)
         self.assertNotEqual(solr_results.docs[0]["id"], "odd")
 
         set_registry_record(
             "qf",
-            u"searchwords^1000.0 SearchableText^1.0",
+            "searchwords^1000.0 SearchableText^1.0",
             interface=IRerSolrpushSettings,
         )
         commit()
 
         solr_results = search(query={"": "odd"}, fl=["UID", "id", "Title"])
         self.assertEqual(solr_results.hits, len(self.docs) / 2)
         self.assertEqual(solr_results.docs[0]["id"], "odd")
 
     def test_search_bq(self):
         solr_results = search(query={"": "odd"}, fl=["UID", "id", "Title"])
         self.assertEqual(solr_results.hits, len(self.docs) / 2)
         self.assertNotEqual(solr_results.docs[0]["id"], "odd")
 
-        set_registry_record("bq", u"id:odd", interface=IRerSolrpushSettings)
+        set_registry_record("bq", "id:odd", interface=IRerSolrpushSettings)
         commit()
 
         solr_results = search(query={"": "odd"}, fl=["UID", "id", "Title"])
         self.assertEqual(solr_results.hits, len(self.docs) / 2)
         self.assertEqual(solr_results.docs[0]["id"], "odd")
 
     def test_escape_chars(self):
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_solr_interface.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_solr_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # -*- coding: utf-8 -*-
 """Setup tests for this package."""
 from plone import api
 from plone.api.portal import set_registry_record
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
+from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 from rer.solrpush.utils import init_solr_push
-from rer.solrpush.utils import reset_solr
-from rer.solrpush.utils import search
 from rer.solrpush.utils import push_to_solr
 from rer.solrpush.utils import remove_from_solr
-from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
-import time
+from rer.solrpush.utils import reset_solr
+from rer.solrpush.utils import search
 from transaction import commit
 
+import time
 import unittest
 
 
 class TestSolrIndexActions(unittest.TestCase):
     """Test that rer.solrpush is properly installed."""
 
     layer = RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         """"""
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record(
-            "enabled_types", [u"Document"], interface=IRerSolrpushSettings
+            "enabled_types", ["Document"], interface=IRerSolrpushSettings
         )
         self.published_doc = api.content.create(
             container=self.portal, type="Document", title="Published Document"
         )
         api.content.transition(obj=self.published_doc, transition="publish")
         self.unpublished_doc = api.content.create(
             container=self.portal,
@@ -149,15 +149,15 @@
     def setUp(self):
         """"""
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record(
             "enabled_types",
-            [u"Document", u"News Item"],
+            ["Document", "News Item"],
             interface=IRerSolrpushSettings,
         )
         #  initialize solr push, so solr will be populated automatically
         # on commits
         init_solr_push()
         commit()
         self.doc1 = api.content.create(
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_tika.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_tika.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 """Setup tests for this package."""
 from plone import api
 from plone.api.portal import set_registry_record
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.namedfile.file import NamedFile
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
+from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 from rer.solrpush.utils import init_solr_push
 from rer.solrpush.utils import reset_solr
 from rer.solrpush.utils import search
-from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 from transaction import commit
 
-import unittest
 import os
+import unittest
 
 
 class TestTika(unittest.TestCase):
     """Test solr indexing for files"""
 
     layer = RER_SOLRPUSH_API_FUNCTIONAL_TESTING
 
     def setUp(self):
         """Custom shared utility setup for tests."""
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
         set_registry_record(
-            "enabled_types", [u"File"], interface=IRerSolrpushSettings
+            "enabled_types", ["File"], interface=IRerSolrpushSettings
         )
         init_solr_push()
         commit()
 
     def tearDown(self):
         set_registry_record("active", True, interface=IRerSolrpushSettings)
         reset_solr()
@@ -47,39 +47,39 @@
         file_item = api.content.create(
             container=self.portal, type="File", title=filename, file=item_file
         )
         commit()
         return file_item
 
     def test_index_and_extract_pdf(self):
-        file_item = self.create_file_item(u"example.pdf")
+        file_item = self.create_file_item("example.pdf")
 
         solr_results = search(query={"*": "*"}, fl="UID")
         self.assertEqual(solr_results.hits, 1)
         st_results = search(query={"SearchablesText": "lorem"}, fl="UID")
         self.assertEqual(st_results.hits, 1)
         self.assertEqual(file_item.UID(), st_results.docs[0]["UID"])
 
     def test_index_and_extract_docx(self):
-        file_item = self.create_file_item(u"example.docx")
+        file_item = self.create_file_item("example.docx")
 
         solr_results = search(query={"*": "*"}, fl="UID SearchableText")
         self.assertEqual(solr_results.hits, 1)
         st_results = search(query={"SearchableText": "ipsum"}, fl="UID")
         self.assertEqual(st_results.hits, 1)
         self.assertEqual(file_item.UID(), st_results.docs[0]["UID"])
 
     def test_index_and_extract_ods(self):
-        file_item = self.create_file_item(u"example.ods")
+        file_item = self.create_file_item("example.ods")
 
         solr_results = search(query={"*": "*"}, fl="UID SearchableText")
         self.assertEqual(solr_results.hits, 1)
         st_results = search(query={"SearchableText": "yyy"}, fl="UID")
         self.assertEqual(st_results.hits, 1)
         self.assertEqual(file_item.UID(), st_results.docs[0]["UID"])
 
     def test_indexed_file_has_right_mimetype(self):
-        self.create_file_item(u"example.pdf")
+        self.create_file_item("example.pdf")
 
         solr_results = search(query={"*": "*"}, fl="UID mime_type")
         self.assertEqual(solr_results.hits, 1)
         self.assertEqual(solr_results.docs[0]["mime_type"], "application/pdf")
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/tests/test_vocabularies.py` & `rer.solrpush-1.4.0/src/rer/solrpush/tests/test_vocabularies.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """Setup tests for this package."""
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
-from rer.solrpush.utils.solr_common import init_solr_push
-from rer.solrpush.utils.solr_common import get_solr_connection
-from rer.solrpush.utils import push_to_solr
 from rer.solrpush.testing import RER_SOLRPUSH_API_FUNCTIONAL_TESTING
+from rer.solrpush.utils import push_to_solr
+from rer.solrpush.utils.solr_common import get_solr_connection
+from rer.solrpush.utils.solr_common import init_solr_push
 from transaction import commit
 from zope.component import getUtility
 from zope.schema.interfaces import IVocabularyFactory
 
 import unittest
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/upgrades.py` & `rer.solrpush-1.4.0/src/rer/solrpush/upgrades.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from plone import api
 from plone.app.upgrade.utils import installOrReinstallProduct
 from rer.solrpush.utils.solr_common import init_solr_push
 from rer.solrpush.utils.solr_indexer import push_to_solr
 
 import logging
 
+
 logger = logging.getLogger(__name__)
 
 default_profile = "profile-rer.solrpush:default"
 
 
 def update_profile(context, name):
     setup_tool = api.portal.get_tool(name="portal_setup")
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/upgrades.zcml` & `rer.solrpush-1.4.0/src/rer/solrpush/upgrades.zcml`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 <configure
-  xmlns="http://namespaces.zope.org/zope"
-  xmlns:genericsetup="http://namespaces.zope.org/genericsetup">
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
+    >
 
   <genericsetup:upgradeStep
-    source="1000"
-    destination="1100"
-    title="Remove persistent utility"
-    description=""
-    profile="rer.solrpush:default"
-    handler=".upgrades.to_1100"
-    />
+      title="Remove persistent utility"
+      description=""
+      profile="rer.solrpush:default"
+      source="1000"
+      destination="1100"
+      handler=".upgrades.to_1100"
+      />
 
   <genericsetup:upgradeStep
-    source="1100"
-    destination="1200"
-    title="Added css resource and bundle"
-    description="Styles for controlpanel"
-    profile="rer.solrpush:default"
-    handler=".upgrades.to_1200"
-    />
-  <genericsetup:upgradeStep
-    source="1200"
-    destination="1300"
-    title="Remove unused control panel"
-    description=""
-    profile="rer.solrpush:default"
-    handler=".upgrades.to_1300"
-    />
-  <genericsetup:upgradeStep
-    source="1300"
-    destination="1400"
-    title="Remove unused control panel"
-    description=""
-    profile="rer.solrpush:default"
-    handler=".upgrades.to_1400"
-    />
-  <genericsetup:upgradeStep
-    source="1400"
-    destination="1500"
-    title="Add new field in controlpanel: force_commit"
-    description=""
-    profile="rer.solrpush:default"
-    handler=".upgrades.update_registry"
-    />
-  <genericsetup:upgradeStep
-    source="1500"
-    destination="1600"
-    title="Add new criteria and reindex files"
-    description=""
-    profile="rer.solrpush:default"
-    handler=".upgrades.to_1600"
-    />
-  <genericsetup:upgradeStep
-    source="1600"
-    destination="1700"
-    title="Add new field in controlpanel: query_debug"
-    description=""
-    profile="rer.solrpush:default"
-    handler=".upgrades.update_registry"
-    />  
-  <genericsetup:upgradeStep
-    source="1700"
-    destination="1800"
-    title="Add new criteria: solr_portal_types"
-    description=""
-    profile="rer.solrpush:default"
-    handler=".upgrades.update_registry"
-    />
-  <genericsetup:upgradeStep
-    source="1800"
-    destination="1900"
-    title="Add elevate control panel link in user actions"
-    description=""
-    profile="rer.solrpush:default"
-    handler=".upgrades.update_actions"
-    />
-  <genericsetup:upgradeStep
-    source="1900"
-    destination="2000"
-    title="Add search_enabled setting field"
-    description=""
-    profile="rer.solrpush:default"
-    handler=".upgrades.update_registry"
-    />  
+      title="Added css resource and bundle"
+      description="Styles for controlpanel"
+      profile="rer.solrpush:default"
+      source="1100"
+      destination="1200"
+      handler=".upgrades.to_1200"
+      />
+  <genericsetup:upgradeStep
+      title="Remove unused control panel"
+      description=""
+      profile="rer.solrpush:default"
+      source="1200"
+      destination="1300"
+      handler=".upgrades.to_1300"
+      />
+  <genericsetup:upgradeStep
+      title="Remove unused control panel"
+      description=""
+      profile="rer.solrpush:default"
+      source="1300"
+      destination="1400"
+      handler=".upgrades.to_1400"
+      />
+  <genericsetup:upgradeStep
+      title="Add new field in controlpanel: force_commit"
+      description=""
+      profile="rer.solrpush:default"
+      source="1400"
+      destination="1500"
+      handler=".upgrades.update_registry"
+      />
+  <genericsetup:upgradeStep
+      title="Add new criteria and reindex files"
+      description=""
+      profile="rer.solrpush:default"
+      source="1500"
+      destination="1600"
+      handler=".upgrades.to_1600"
+      />
+  <genericsetup:upgradeStep
+      title="Add new field in controlpanel: query_debug"
+      description=""
+      profile="rer.solrpush:default"
+      source="1600"
+      destination="1700"
+      handler=".upgrades.update_registry"
+      />
+  <genericsetup:upgradeStep
+      title="Add new criteria: solr_portal_types"
+      description=""
+      profile="rer.solrpush:default"
+      source="1700"
+      destination="1800"
+      handler=".upgrades.update_registry"
+      />
+  <genericsetup:upgradeStep
+      title="Add elevate control panel link in user actions"
+      description=""
+      profile="rer.solrpush:default"
+      source="1800"
+      destination="1900"
+      handler=".upgrades.update_actions"
+      />
+  <genericsetup:upgradeStep
+      title="Add search_enabled setting field"
+      description=""
+      profile="rer.solrpush:default"
+      source="1900"
+      destination="2000"
+      handler=".upgrades.update_registry"
+      />
 </configure>
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/utils/solr_common.py` & `rer.solrpush-1.4.0/src/rer/solrpush/utils/solr_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 def should_force_commit():
     return get_setting(field="force_commit") or False
 
 
 def get_index_fields():
     json_str = get_setting(field="index_fields")
-    return json.loads(json_str)
+    return json_str and json.loads(json_str) or {}
 
 
 def extract_fields(nodes):
     fields = {}
     for node in nodes:
         field_name = node.get("name")
         field_type = node.get("type")
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/utils/solr_indexer.py` & `rer.solrpush-1.4.0/src/rer/solrpush/utils/solr_indexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # -*- coding: utf-8 -*-
 from DateTime import DateTime
+from persistent.mapping import PersistentMapping
 from plone import api
 from plone.indexer.interfaces import IIndexableObject
 from plone.registry.interfaces import IRegistry
+from plone.restapi.serializer.converters import json_compatible
 from rer.solrpush import _
 from rer.solrpush.interfaces.adapter import IExtractFileFromTika
-from six.moves import map
-from zope.component import getUtility
-from zope.component import queryMultiAdapter
-from rer.solrpush.utils.solr_common import get_solr_connection
-from rer.solrpush.utils.solr_common import get_setting
 from rer.solrpush.utils.solr_common import get_index_fields
+from rer.solrpush.utils.solr_common import get_setting
+from rer.solrpush.utils.solr_common import get_solr_connection
 from rer.solrpush.utils.solr_common import is_solr_active
 from rer.solrpush.utils.solr_common import should_force_commit
+from six.moves import map
+from zope.component import getUtility
+from zope.component import queryMultiAdapter
 
 import datetime
+import json
 import logging
 import pysolr
 import six
 
 
 if six.PY2:
     from ftfy import fix_text
@@ -136,14 +139,17 @@
         if six.PY2:
             value = fix_py2_strings(value)
         if isinstance(value, DateTime):
             value = parse_date_as_datetime(value)
         else:
             if field_type == "date":
                 value = parse_date_str(value)
+        if isinstance(value, PersistentMapping):
+            # convert dict-like object in json object
+            value = json.dumps(json_compatible(value))
         index_me[field] = value
 
     for field in ADDITIONAL_FIELDS:
         value = getattr(item, field, None)
         if value is not None:
             index_me[field] = value
     portal = api.portal.get()
@@ -161,15 +167,22 @@
     if frontend_url:
         index_me["url"] = item.absolute_url().replace(
             portal.portal_url(), frontend_url
         )
     else:
         index_me["url"] = item.absolute_url()
 
-    has_image = getattr(item.aq_base, "image", None)
+    # backward compatibility with Plone < 6 where there wasn't image_field and image_scales indexers
+    has_image = False
+    if index_me.get("image_field", None) and index_me.get(
+        "image_scales", None
+    ):
+        has_image = True
+    else:
+        has_image = getattr(item.aq_base, "image", None)
     if has_image:
         index_me["getIcon"] = True
 
     return index_me
 
 
 def fix_py2_strings(value):
@@ -271,15 +284,15 @@
             q="UID:{}".format(uid),
             commit=should_force_commit(),
         )
     except (pysolr.SolrError, TypeError) as err:
         logger.error(err)
         message = _(
             "content_remove_error",
-            default=u"There was a problem removing this content from SOLR. "
+            default="There was a problem removing this content from SOLR. "
             " Please contact site administrator.",
         )
         api.portal.show_message(
             message=message, request=portal.REQUEST, type="warning"
         )
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/utils/solr_search.py` & `rer.solrpush-1.4.0/src/rer/solrpush/utils/solr_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
+from DateTime import DateTime
 from plone import api
+from pysolr import safe_urlencode
 from rer.solrpush import _
 from rer.solrpush.interfaces import IElevateSettings
-from zope.i18n import translate
-from rer.solrpush.utils.solr_common import get_solr_connection
-from rer.solrpush.utils.solr_common import get_setting
-from rer.solrpush.utils.solr_common import get_index_fields
 from rer.solrpush.interfaces.settings import IRerSolrpushSettings
+from rer.solrpush.utils.solr_common import get_index_fields
+from rer.solrpush.utils.solr_common import get_setting
+from rer.solrpush.utils.solr_common import get_solr_connection
+from rer.solrpush.utils.solr_common import is_solr_active
 from rer.solrpush.utils.solr_indexer import parse_date_str
-from DateTime import DateTime
-from pysolr import safe_urlencode
 from zope.annotation.interfaces import IAnnotations
 from zope.globalrequest import getRequest
+from zope.i18n import translate
 
-import logging
 import json
+import logging
 import re
 import requests
 import six
 
 
 logger = logging.getLogger(__name__)
 
@@ -272,14 +273,15 @@
     if params:
         params["defType"] = "edismax"
     return params
 
 
 # END HELPER METHODS
 
+
 # LIBRARY METHODS
 def search(
     query,
     fl=None,
     facets=False,
     facet_fields=["Subject", "portal_type"],
     **kwargs
@@ -294,16 +296,18 @@
         Defaults to ["Subject", "portal_type"].
 
     Returns:
         [type]: [description]
     """
     solr = get_solr_connection()
     if not solr:
-        msg = u"Unable to search using solr. Configuration is incomplete."
-        logger.error(msg)
+        msg = "Unable to search using solr. Configuration is incomplete."
+        if is_solr_active():
+            # log it beacuse it's misconfigured
+            logger.error(msg)
         return {
             "error": True,
             "message": translate(
                 _("solr_configuration_error_label", default=msg),
                 context=api.portal.get().REQUEST,
             ),
         }
@@ -320,17 +324,17 @@
     except Exception as e:
         logger.exception(e)
         return {
             "error": True,
             "message": translate(
                 _(
                     "search_error_label",
-                    default=u"Unable to perform a search with SOLR."
-                    u" Please contact the site administrator or wait some"
-                    u" minutes.",
+                    default="Unable to perform a search with SOLR."
+                    " Please contact the site administrator or wait some"
+                    " minutes.",
                 ),
                 context=api.portal.get().REQUEST,
             ),
         }
 
 
 def _set_query_debug(solr, params):
```

### Comparing `rer.solrpush-1.3.3/src/rer/solrpush/vocabularies.py` & `rer.solrpush-1.4.0/src/rer/solrpush/vocabularies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from rer.solrpush.utils import search
 from zope.interface import implementer
 from zope.schema.interfaces import IVocabularyFactory
-from zope.schema.vocabulary import SimpleVocabulary, SimpleTerm
+from zope.schema.vocabulary import SimpleTerm
+from zope.schema.vocabulary import SimpleVocabulary
 
 
 class FacetsVocabulary(object):
     def get_terms(self):
         solr_results = search(
             query={"*": "*", "b_size": 1},
             fl="UID",
```

### Comparing `rer.solrpush-1.3.3/src/rer.solrpush.egg-info/PKG-INFO` & `rer.solrpush-1.4.0/src/rer.solrpush.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: rer.solrpush
-Version: 1.3.3
+Version: 1.4.0
 Summary: Prodotto per Regione Emilia-Romagna relativo all'indicizzazione dei contenuti con solr
 Home-page: https://github.com/collective/rer.solrpush
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.solrpush
 Project-URL: Source, https://github.com/collective/rer.solrpush
 Project-URL: Tracker, https://github.com/collective/rer.solrpush/issues
 Keywords: Python Plone
 Classifier: Environment :: Web Environment
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.1
 Classifier: Framework :: Plone :: 5.2
+Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: ==2.7
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
 ============
 rer.solrpush
 ============
@@ -237,14 +240,21 @@
 - RedTurtle, sviluppoplone@redturtle.it
 
 
 Changelog
 =========
 
 
+1.4.0 (2024-05-05)
+------------------
+
+- Plone6 compatibility.
+  [cekk]
+
+
 1.3.3 (2023-11-08)
 ------------------
 
 - Fix RSS Feed.
   [cekk]
 
 1.3.2 (2023-11-08)
```

### Comparing `rer.solrpush-1.3.3/src/rer.solrpush.egg-info/SOURCES.txt` & `rer.solrpush-1.4.0/src/rer.solrpush.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 DEVELOP.rst
 LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
+constraints_plone60.txt
 docker-compose.yml
 publiccode.yml
 setup.cfg
 setup.py
 docs/Solr-Push_Configurazione.jpg
-docs/conf.py
 docs/index.rst
 docs/rer-logo.png
 src/rer/__init__.py
 src/rer.solrpush.egg-info/PKG-INFO
 src/rer.solrpush.egg-info/SOURCES.txt
 src/rer.solrpush.egg-info/dependency_links.txt
 src/rer.solrpush.egg-info/entry_points.txt
@@ -43,14 +43,15 @@
 src/rer/solrpush/browser/configure.zcml
 src/rer/solrpush/browser/controlpanel.py
 src/rer/solrpush/browser/elevate_settings.py
 src/rer/solrpush/browser/maintenance.py
 src/rer/solrpush/browser/query_debug.py
 src/rer/solrpush/browser/querybuilder.py
 src/rer/solrpush/browser/scales.py
+src/rer/solrpush/browser/overrides/plone.app.contenttypes.browser.templates.listing.pt
 src/rer/solrpush/browser/static/.gitkeep
 src/rer/solrpush/browser/static/package.json
 src/rer/solrpush/browser/static/styles.css
 src/rer/solrpush/browser/static/styles.css.map
 src/rer/solrpush/browser/static/styles.scss
 src/rer/solrpush/browser/static/yarn.lock
 src/rer/solrpush/browser/static/dist/dev/main.js
@@ -94,14 +95,18 @@
 src/rer/solrpush/profiles/to_1300/controlpanel.xml
 src/rer/solrpush/profiles/to_1300/registry.xml
 src/rer/solrpush/profiles/uninstall/browserlayer.xml
 src/rer/solrpush/profiles/uninstall/controlpanel.xml
 src/rer/solrpush/profiles/uninstall/registry.xml
 src/rer/solrpush/restapi/__init__.py
 src/rer/solrpush/restapi/configure.zcml
+src/rer/solrpush/restapi/controlpanel.py
+src/rer/solrpush/restapi/deserializer/__init__.py
+src/rer/solrpush/restapi/deserializer/configure.zcml
+src/rer/solrpush/restapi/deserializer/controlpanel.py
 src/rer/solrpush/restapi/services/__init__.py
 src/rer/solrpush/restapi/services/configure.zcml
 src/rer/solrpush/restapi/services/elevate_schema/__init__.py
 src/rer/solrpush/restapi/services/elevate_schema/configure.zcml
 src/rer/solrpush/restapi/services/elevate_schema/get.py
 src/rer/solrpush/restapi/services/solr_search/__init__.py
 src/rer/solrpush/restapi/services/solr_search/batch.py
@@ -113,15 +118,14 @@
 src/rer/solrpush/tests/test_elevate.py
 src/rer/solrpush/tests/test_events.py
 src/rer/solrpush/tests/test_image_tags.py
 src/rer/solrpush/tests/test_maintenance.py
 src/rer/solrpush/tests/test_querybuilder.py
 src/rer/solrpush/tests/test_restapi_search.py
 src/rer/solrpush/tests/test_search.py
-src/rer/solrpush/tests/test_setup.py
 src/rer/solrpush/tests/test_solr_interface.py
 src/rer/solrpush/tests/test_tika.py
 src/rer/solrpush/tests/test_vocabularies.py
 src/rer/solrpush/tests/docs/example.docx
 src/rer/solrpush/tests/docs/example.ods
 src/rer/solrpush/tests/docs/example.pdf
 src/rer/solrpush/tests/docs/plone_logo.png
```

