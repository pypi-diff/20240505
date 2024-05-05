# Comparing `tmp/betty-0.3.3.tar.gz` & `tmp/betty-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betty-0.3.3.tar", last modified: Thu Apr 11 22:30:12 2024, max compression
+gzip compressed data, was "betty-0.3.4.tar", last modified: Sun May  5 11:20:20 2024, max compression
```

## Comparing `betty-0.3.3.tar` & `betty-0.3.4.tar`

### file list

```diff
@@ -1,300 +1,307 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.238239 betty-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-11 22:29:12.000000 betty-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    43400 2024-04-11 22:30:12.238239 betty-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-11 22:29:12.000000 betty-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-11 22:29:12.000000 betty-0.3.3/betty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.186239 betty-0.3.3/betty/_package/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/_package/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_package/pyinstaller/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/_package/pyinstaller/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_package/pyinstaller/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_package/pyinstaller/hooks/hook-betty.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_package/pyinstaller/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-11 22:29:12.000000 betty-0.3.3/betty/_resizeimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-11 22:29:12.000000 betty-0.3.3/betty/about.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/app/
--rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-11 22:29:12.000000 betty-0.3.3/betty/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/app/extension/
--rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-04-11 22:29:12.000000 betty-0.3.3/betty/app/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-11 22:29:12.000000 betty-0.3.3/betty/app/extension/requirement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 22:29:21.000000 betty-0.3.3/betty/assets/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)    21162 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/betty.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.186239 betty-0.3.3/betty/assets/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/assets/locale/de-DE/
--rw-r--r--   0 runner    (1001) docker     (127)    36368 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/locale/de-DE/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.202239 betty-0.3.3/betty/assets/locale/fr-FR/
--rw-r--r--   0 runner    (1001) docker     (127)    25619 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/locale/fr-FR/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/locale/nl-NL/
--rw-r--r--   0 runner    (1001) docker     (127)    36229 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/locale/nl-NL/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/locale/uk/
--rw-r--r--   0 runner    (1001) docker     (127)    25644 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/locale/uk/betty.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.186239 betty-0.3.3/betty/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/public/localized/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/localized/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/public/static/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/betty-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/betty-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/betty-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)    19708 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/betty-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)   152126 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/betty.ico
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/public/static/robots.txt.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/base.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/assets/templates/entity/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/entity/page-list.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/entity/page.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/head.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/linked-data.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/sitemap-index.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 22:29:12.000000 betty-0.3.3/betty/assets/templates/sitemap.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-11 22:29:12.000000 betty-0.3.3/betty/asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-11 22:29:12.000000 betty-0.3.3/betty/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-11 22:29:12.000000 betty-0.3.3/betty/cache/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-11 22:29:12.000000 betty-0.3.3/betty/cache/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-11 22:29:12.000000 betty-0.3.3/betty/cache/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-11 22:29:12.000000 betty-0.3.3/betty/classtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-04-11 22:29:12.000000 betty-0.3.3/betty/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-11 22:29:12.000000 betty-0.3.3/betty/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    22568 2024-04-11 22:29:12.000000 betty-0.3.3/betty/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-11 22:29:12.000000 betty-0.3.3/betty/contextlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    10802 2024-04-11 22:29:12.000000 betty-0.3.3/betty/deriver.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-11 22:29:12.000000 betty-0.3.3/betty/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-11 22:29:12.000000 betty-0.3.3/betty/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-11 22:29:12.000000 betty-0.3.3/betty/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.206239 betty-0.3.3/betty/extension/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.210239 betty-0.3.3/betty/extension/cotton_candy/
--rw-r--r--   0 runner    (1001) docker     (127)    14934 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/cotton_candy/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.210239 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/accessibility.scss
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/citation.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/entity.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.js
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.scss
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/main.js
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/main.scss
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/meta.scss
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/overlay.scss
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/page.scss
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/permalink.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/person.scss
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.js
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.scss
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/show.js
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/show.scss
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/text.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/variables.scss.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/cotton_candy/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.210239 betty-0.3.3/betty/extension/cotton_candy/assets/public/localized/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/public/localized/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/public/localized/search-index.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.214239 betty-0.3.3/betty/extension/cotton_candy/assets/public/static/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/public/static/betty.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/public/static/search-configuration.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.214239 betty-0.3.3/betty/extension/cotton_candy/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/base.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.218239 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--event.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-extended--application--pdf.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-extended--image.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-extended.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-summary--application--pdf.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-summary--image.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file-summary.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/footer.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.218239 betty-0.3.3/betty/extension/cotton_candy/assets/templates/macro/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/macro/citation.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/media.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/permalink.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/references.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-person.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-place.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/results.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/section-notes.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/show-countable.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/show.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/assets/templates/timeline.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/cotton_candy/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/demo/
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/deriver/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/deriver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/gramps/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/gramps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/gramps/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/gramps/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/http_api_doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/http_api_doc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/http_api_doc/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/http_api_doc/assets/betty.extension.npm._Npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/http_api_doc/assets/betty.extension.npm._Npm/src/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/http_api_doc/assets/betty.extension.npm._Npm/src/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/http_api_doc/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/http_api_doc/assets/public/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/http_api_doc/assets/public/static/api/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/http_api_doc/assets/public/static/api/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/maps/
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/maps/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.190239 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.css
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.js
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.222239 betty-0.3.3/betty/extension/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/nginx/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/assets/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/assets/content_negotiation.lua
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/assets/nginx.conf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/nginx/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/npm/
--rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/npm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/privatizer/
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/privatizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/trees/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/betty/extension/trees/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.css
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.js
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/betty/extension/trees/assets/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/trees/assets/public/localized/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/trees/assets/public/localized/people.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/wikipedia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/betty/extension/wikipedia/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/extension/wikipedia/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-11 22:29:12.000000 betty-0.3.3/betty/extension/wikipedia/assets/templates/wikipedia.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-11 22:29:12.000000 betty-0.3.3/betty/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-11 22:29:12.000000 betty-0.3.3/betty/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-11 22:29:12.000000 betty-0.3.3/betty/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.226239 betty-0.3.3/betty/gramps/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gramps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gramps/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    31162 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gramps/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12727 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    31464 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-11 22:29:12.000000 betty-0.3.3/betty/gui/window.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-11 22:29:12.000000 betty-0.3.3/betty/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-11 22:29:12.000000 betty-0.3.3/betty/importlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-04-11 22:29:12.000000 betty-0.3.3/betty/jinja2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-04-11 22:29:12.000000 betty-0.3.3/betty/jinja2/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-11 22:29:12.000000 betty-0.3.3/betty/jinja2/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-11 22:29:12.000000 betty-0.3.3/betty/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/json/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 22:29:12.000000 betty-0.3.3/betty/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-11 22:29:12.000000 betty-0.3.3/betty/json/linked_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-11 22:29:12.000000 betty-0.3.3/betty/json/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 22:29:12.000000 betty-0.3.3/betty/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    36985 2024-04-11 22:29:12.000000 betty-0.3.3/betty/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-11 22:29:12.000000 betty-0.3.3/betty/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-11 22:29:12.000000 betty-0.3.3/betty/media_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/model/
--rw-r--r--   0 runner    (1001) docker     (127)    35361 2024-04-11 22:29:12.000000 betty-0.3.3/betty/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56370 2024-04-11 22:29:12.000000 betty-0.3.3/betty/model/ancestry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-04-11 22:29:12.000000 betty-0.3.3/betty/model/event_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-11 22:29:12.000000 betty-0.3.3/betty/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-11 22:29:12.000000 betty-0.3.3/betty/os.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-11 22:29:12.000000 betty-0.3.3/betty/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-11 22:29:12.000000 betty-0.3.3/betty/privatizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29182 2024-04-11 22:29:12.000000 betty-0.3.3/betty/project.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:29:12.000000 betty-0.3.3/betty/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-11 22:29:12.000000 betty-0.3.3/betty/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/serde/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serde/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serde/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serde/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serde/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-11 22:29:12.000000 betty-0.3.3/betty/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 22:29:12.000000 betty-0.3.3/betty/sphinx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty/sphinx/extension/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 22:29:12.000000 betty-0.3.3/betty/sphinx/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-11 22:29:12.000000 betty-0.3.3/betty/sphinx/extension/replacements.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 22:29:12.000000 betty-0.3.3/betty/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-11 22:29:12.000000 betty-0.3.3/betty/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-11 22:29:12.000000 betty-0.3.3/betty/url.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-11 22:29:12.000000 betty-0.3.3/betty/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16686 2024-04-11 22:29:12.000000 betty-0.3.3/betty/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/betty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43400 2024-04-11 22:30:11.000000 betty-0.3.3/betty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-04-11 22:30:12.000000 betty-0.3.3/betty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:30:11.000000 betty-0.3.3/betty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 22:30:11.000000 betty-0.3.3/betty.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-11 22:30:11.000000 betty-0.3.3/betty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 22:30:11.000000 betty-0.3.3/betty.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-11 22:29:12.000000 betty-0.3.3/documentation/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/node_modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.194239 betty-0.3.3/node_modules/flatted/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:30:12.230239 betty-0.3.3/node_modules/flatted/python/
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-11 22:29:59.000000 betty-0.3.3/node_modules/flatted/python/flatted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-11 22:29:59.000000 betty-0.3.3/node_modules/flatted/python/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-11 22:29:12.000000 betty-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:30:12.238239 betty-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-11 22:29:12.000000 betty-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.591119 betty-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-05 11:19:09.000000 betty-0.3.4/.browserslistrc
+-rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-05-05 11:19:09.000000 betty-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-05 11:19:09.000000 betty-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43621 2024-05-05 11:20:20.591119 betty-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-05 11:19:09.000000 betty-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.551119 betty-0.3.4/betty/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-05 11:19:09.000000 betty-0.3.4/betty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_npm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.535119 betty-0.3.4/betty/_package/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/_package/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_package/pyinstaller/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/_package/pyinstaller/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_package/pyinstaller/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_package/pyinstaller/hooks/hook-betty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_package/pyinstaller/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-05 11:19:09.000000 betty-0.3.4/betty/_resizeimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-05 11:19:09.000000 betty-0.3.4/betty/about.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    19649 2024-05-05 11:19:09.000000 betty-0.3.4/betty/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/app/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-05 11:19:09.000000 betty-0.3.4/betty/app/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-05 11:19:09.000000 betty-0.3.4/betty/app/extension/requirement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 11:19:20.000000 betty-0.3.4/betty/assets/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)    21029 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/betty.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.535119 betty-0.3.4/betty/assets/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/locale/de-DE/
+-rw-r--r--   0 runner    (1001) docker     (127)    36131 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/locale/de-DE/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/locale/fr-FR/
+-rw-r--r--   0 runner    (1001) docker     (127)    25486 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/locale/fr-FR/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/locale/nl-NL/
+-rw-r--r--   0 runner    (1001) docker     (127)    36020 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/locale/nl-NL/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/locale/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/locale/uk/betty.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.535119 betty-0.3.4/betty/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.555119 betty-0.3.4/betty/assets/public/localized/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/localized/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.559119 betty-0.3.4/betty/assets/public/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/betty-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/betty-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/betty-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19708 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/betty-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)   152126 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/betty.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/public/static/robots.txt.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.559119 betty-0.3.4/betty/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/base.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.559119 betty-0.3.4/betty/assets/templates/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/entity/page-list.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/entity/page.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/head.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/linked-data.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/scripts.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/sitemap-index.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/sitemap.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 11:19:09.000000 betty-0.3.4/betty/assets/templates/stylesheets.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-05 11:19:09.000000 betty-0.3.4/betty/asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.559119 betty-0.3.4/betty/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-05 11:19:09.000000 betty-0.3.4/betty/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-05 11:19:09.000000 betty-0.3.4/betty/cache/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-05 11:19:09.000000 betty-0.3.4/betty/cache/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-05 11:19:09.000000 betty-0.3.4/betty/cache/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-05 11:19:09.000000 betty-0.3.4/betty/classtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-05-05 11:19:09.000000 betty-0.3.4/betty/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-05 11:19:09.000000 betty-0.3.4/betty/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-05-05 11:19:09.000000 betty-0.3.4/betty/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-05 11:19:09.000000 betty-0.3.4/betty/contextlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-05 11:19:09.000000 betty-0.3.4/betty/deriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 11:19:09.000000 betty-0.3.4/betty/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-05 11:19:09.000000 betty-0.3.4/betty/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-05 11:19:09.000000 betty-0.3.4/betty/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.559119 betty-0.3.4/betty/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.563119 betty-0.3.4/betty/extension/cotton_candy/
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/cotton_candy/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/cotton_candy/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.563119 betty-0.3.4/betty/extension/cotton_candy/assets/public/localized/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/public/localized/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/public/localized/search-index.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.563119 betty-0.3.4/betty/extension/cotton_candy/assets/public/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/public/static/betty.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/public/static/search-configuration.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.563119 betty-0.3.4/betty/extension/cotton_candy/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/base.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.571119 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--event.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-extended--application--pdf.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-extended--image.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-extended.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-summary--application--pdf.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-summary--image.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file-summary.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/footer.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.571119 betty-0.3.4/betty/extension/cotton_candy/assets/templates/macro/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/macro/citation.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/map.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/media.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/permalink.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/references.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.571119 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-person.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-place.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/results.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/section-notes.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/show-countable.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/show.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/timeline.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/assets/templates/tree.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/cotton_candy/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/accessibility.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/citation.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/entity.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/file.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/file.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/main.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/main.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/meta.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/overlay.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/page.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/permalink.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/person.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/search.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/search.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/show.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/show.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/text.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/cotton_candy/webpack/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)    17350 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/deriver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/deriver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/gramps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/gramps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/gramps/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/gramps/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/http_api_doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/http_api_doc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/http_api_doc/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/http_api_doc/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/http_api_doc/assets/public/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/http_api_doc/assets/public/static/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/http_api_doc/assets/public/static/api/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/http_api_doc/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/http_api_doc/webpack/main.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/http_api_doc/webpack/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/maps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.575119 betty-0.3.4/betty/extension/maps/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/maps/webpack/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/maps/webpack/main.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/maps/webpack/maps.js
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/maps/webpack/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/nginx/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/assets/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/assets/content_negotiation.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/assets/nginx.conf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/nginx/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/privatizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/privatizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/trees/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/trees/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.539119 betty-0.3.4/betty/extension/trees/assets/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/trees/assets/public/localized/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/assets/public/localized/people.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/trees/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/webpack/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/webpack/main.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/webpack/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/trees/webpack/trees.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.543119 betty-0.3.4/betty/extension/webpack/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/webpack/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/assets/templates/webpack-entry-loader.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9439 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/webpack/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/jinja2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/jinja2/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/webpack/webpack/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/webpack/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/webpack/webpack/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/wikipedia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.543119 betty-0.3.4/betty/extension/wikipedia/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/extension/wikipedia/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-05 11:19:09.000000 betty-0.3.4/betty/extension/wikipedia/assets/templates/wikipedia.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-05 11:19:09.000000 betty-0.3.4/betty/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-05-05 11:19:09.000000 betty-0.3.4/betty/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-05-05 11:19:09.000000 betty-0.3.4/betty/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.579119 betty-0.3.4/betty/gramps/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gramps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gramps/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32472 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gramps/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.583119 betty-0.3.4/betty/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33182 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-05 11:19:09.000000 betty-0.3.4/betty/gui/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-05 11:19:09.000000 betty-0.3.4/betty/hashid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-05 11:19:09.000000 betty-0.3.4/betty/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-05 11:19:09.000000 betty-0.3.4/betty/importlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.583119 betty-0.3.4/betty/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-05 11:19:09.000000 betty-0.3.4/betty/jinja2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17552 2024-05-05 11:19:09.000000 betty-0.3.4/betty/jinja2/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-05 11:19:09.000000 betty-0.3.4/betty/jinja2/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-05 11:19:09.000000 betty-0.3.4/betty/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.583119 betty-0.3.4/betty/json/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-05 11:19:09.000000 betty-0.3.4/betty/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-05 11:19:09.000000 betty-0.3.4/betty/json/linked_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-05 11:19:09.000000 betty-0.3.4/betty/json/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-05 11:19:09.000000 betty-0.3.4/betty/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39939 2024-05-05 11:19:09.000000 betty-0.3.4/betty/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-05 11:19:09.000000 betty-0.3.4/betty/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-05 11:19:09.000000 betty-0.3.4/betty/media_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.583119 betty-0.3.4/betty/model/
+-rw-r--r--   0 runner    (1001) docker     (127)    35924 2024-05-05 11:19:09.000000 betty-0.3.4/betty/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58905 2024-05-05 11:19:09.000000 betty-0.3.4/betty/model/ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-05 11:19:09.000000 betty-0.3.4/betty/model/event_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-05 11:19:09.000000 betty-0.3.4/betty/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-05 11:19:09.000000 betty-0.3.4/betty/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-05 11:19:09.000000 betty-0.3.4/betty/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-05-05 11:19:09.000000 betty-0.3.4/betty/privatizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-05 11:19:09.000000 betty-0.3.4/betty/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 11:19:09.000000 betty-0.3.4/betty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-05 11:19:09.000000 betty-0.3.4/betty/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-05 11:19:09.000000 betty-0.3.4/betty/requirement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.587119 betty-0.3.4/betty/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serde/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serde/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serde/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16180 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serde/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-05-05 11:19:09.000000 betty-0.3.4/betty/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.587119 betty-0.3.4/betty/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 11:19:09.000000 betty-0.3.4/betty/sphinx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.587119 betty-0.3.4/betty/sphinx/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-05 11:19:09.000000 betty-0.3.4/betty/sphinx/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-05 11:19:09.000000 betty-0.3.4/betty/sphinx/extension/replacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-05 11:19:09.000000 betty-0.3.4/betty/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-05 11:19:09.000000 betty-0.3.4/betty/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-05 11:19:09.000000 betty-0.3.4/betty/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-05 11:19:09.000000 betty-0.3.4/betty/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17927 2024-05-05 11:19:09.000000 betty-0.3.4/betty/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.587119 betty-0.3.4/betty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43621 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 11:20:20.000000 betty-0.3.4/betty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 11:20:20.587119 betty-0.3.4/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-05 11:19:09.000000 betty-0.3.4/documentation/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-05 11:19:09.000000 betty-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 11:20:20.591119 betty-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-05 11:19:09.000000 betty-0.3.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-05 11:19:09.000000 betty-0.3.4/tsconfig.json
```

### Comparing `betty-0.3.3/LICENSE.txt` & `betty-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/PKG-INFO` & `betty-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betty
-Version: 0.3.3
+Version: 0.3.4
 Summary: Betty helps you visualize and publish your family history by building interactive genealogy websites out of your Gramps and GECOM family trees
 Author-email: Bart Feenstra <bar@bartfeenstra.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,18 +683,19 @@
 Requires-Dist: pyinstaller>=6.1.0,~=6.1; extra == "pyinstaller"
 Provides-Extra: setuptools
 Requires-Dist: setuptools~=69.0; extra == "setuptools"
 Requires-Dist: twine~=5.0; extra == "setuptools"
 Requires-Dist: wheel>=0.40.0,~=0.40; extra == "setuptools"
 Provides-Extra: test
 Requires-Dist: aioresponses>=0.7.6,~=0.7; extra == "test"
-Requires-Dist: autopep8>=2.0.2,~=2.0; extra == "test"
 Requires-Dist: basedmypy>=2.2.1,~=2.0; extra == "test"
+Requires-Dist: black>=24.4.0,~=24.4; extra == "test"
 Requires-Dist: coverage>=7.2.4,~=7.2; extra == "test"
 Requires-Dist: flake8~=7.0; extra == "test"
+Requires-Dist: flake8-bugbear~=24.4; extra == "test"
 Requires-Dist: html5lib~=1.1; extra == "test"
 Requires-Dist: lxml~=5.0; sys_platform != "win32" and extra == "test"
 Requires-Dist: pip-licenses>=4.3.0,~=4.3; extra == "test"
 Requires-Dist: pydocstyle>=6.3.0,~=6.3; extra == "test"
 Requires-Dist: pytest>=7.3.1,~=7.3; extra == "test"
 Requires-Dist: pytest-aioresponses>=0.2.0,~=0.2; extra == "test"
 Requires-Dist: pytest-asyncio>=0.23.4,~=0.23; extra == "test"
@@ -710,14 +711,15 @@
 Requires-Dist: types-lxml>=2024.3.27; extra == "test"
 Requires-Dist: types-mock>=5.0.0.6,~=5.0; extra == "test"
 Requires-Dist: types-polib>=1.2.0.0,~=1.2; extra == "test"
 Requires-Dist: types-pyinstaller>=6.5.0.20240311,~=6.5; extra == "test"
 Requires-Dist: types-pyyaml>=6.0.6,~=6.0; extra == "test"
 Requires-Dist: types-requests>=2.29.0.0,~=2.29; extra == "test"
 Requires-Dist: types-setuptools~=69.0; extra == "test"
+Requires-Dist: virtualenv~=20.26; extra == "test"
 Requires-Dist: betty[pyinstaller]; extra == "test"
 Requires-Dist: betty[setuptools]; extra == "test"
 Provides-Extra: development
 Requires-Dist: pytest-repeat>=0.9.1,~=0.9; extra == "development"
 Requires-Dist: betty[test]; extra == "development"
 Provides-Extra: ci
 Requires-Dist: codecov>=2.1.12,~=2.1; extra == "ci"
@@ -726,10 +728,14 @@
 # Betty 👵
 
 ![Test status](https://github.com/bartfeenstra/betty/workflows/Test/badge.svg?branch=0.3.x) [![Code coverage](https://codecov.io/gh/bartfeenstra/betty/branch/0.3.x/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/betty) [![PyPI releases](https://badge.fury.io/py/betty.svg)](https://pypi.org/project/betty/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/betty.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/betty/) [![Recent downloads](https://img.shields.io/pypi/dm/betty.svg)](https://pypi.org/project/betty/) [![Follow Betty on Twitter](https://img.shields.io/twitter/follow/Betty_Project.svg?label=Betty_Project&style=flat&logo=twitter&logoColor=4FADFF)](https://twitter.com/Betty_Project)
 
 Betty visualizes and publishes your family history by building interactive, encyclopedia-like genealogy websites out of your
 [Gramps](https://gramps-project.org/) and [GEDCOM](https://en.wikipedia.org/wiki/GEDCOM) family trees.
 
+## View an example site
+
+View a Betty example site at [ancestry.bartfeenstra.com](https://ancestry.bartfeenstra.com).
+
 ## Documentation
 
 View the documentation at [https://betty.readthedocs.io/](https://betty.readthedocs.io/).
```

### Comparing `betty-0.3.3/README.md` & `betty-0.3.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Betty 👵
 
 ![Test status](https://github.com/bartfeenstra/betty/workflows/Test/badge.svg?branch=0.3.x) [![Code coverage](https://codecov.io/gh/bartfeenstra/betty/branch/0.3.x/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/betty) [![PyPI releases](https://badge.fury.io/py/betty.svg)](https://pypi.org/project/betty/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/betty.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/betty/) [![Recent downloads](https://img.shields.io/pypi/dm/betty.svg)](https://pypi.org/project/betty/) [![Follow Betty on Twitter](https://img.shields.io/twitter/follow/Betty_Project.svg?label=Betty_Project&style=flat&logo=twitter&logoColor=4FADFF)](https://twitter.com/Betty_Project)
 
 Betty visualizes and publishes your family history by building interactive, encyclopedia-like genealogy websites out of your
 [Gramps](https://gramps-project.org/) and [GEDCOM](https://en.wikipedia.org/wiki/GEDCOM) family trees.
 
+## View an example site
+
+View a Betty example site at [ancestry.bartfeenstra.com](https://ancestry.bartfeenstra.com).
+
 ## Documentation
 
 View the documentation at [https://betty.readthedocs.io/](https://betty.readthedocs.io/).
```

### Comparing `betty-0.3.3/betty/_package/pyinstaller/main.py` & `betty-0.3.4/betty/_package/pyinstaller/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,10 @@
 async def _main() -> None:
     async with App.new_from_environment() as app:
         async with BettyApplication([sys.argv[0]]).with_app(app) as qapp:
             window = WelcomeWindow(app)
             window.show()
             sys.exit(qapp.exec())
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `betty-0.3.3/betty/_patch.py` & `betty-0.3.4/betty/_patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from asyncio import BaseEventLoop
 from typing import Any
 
 _original_shutdown_default_executor = BaseEventLoop.shutdown_default_executor
 
 
-async def _shutdown_default_executor(loop: BaseEventLoop, *args: Any, **kwargs: Any) -> None:
+async def _shutdown_default_executor(
+    loop: BaseEventLoop, *args: Any, **kwargs: Any
+) -> None:
     try:
         await _original_shutdown_default_executor(loop, *args, **kwargs)
     except RuntimeError as error:
         # Work around a bug in Python 3.12 that will randomly cause a RuntimeError with the
         # following message to be raised.
         if "can't create new thread at interpreter shutdown" not in str(error):
             raise
+
+
 BaseEventLoop.shutdown_default_executor = _shutdown_default_executor  # type: ignore[assignment, method-assign]
```

### Comparing `betty-0.3.3/betty/_resizeimage.py` & `betty-0.3.4/betty/_resizeimage.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 A partial, simplified fork of the abandoned python-resize-image package.
 
 This module exists purely because existing Betty code depended on an abandoned package, and that code has not been
 refactored yet.
 
 New code MUST NOT use this module.
 """
+
 import math
 
 from PIL.Image import Image
 
 
 def resize_crop(image: Image, size: tuple[int, int]) -> Image:
     """
@@ -35,15 +36,15 @@
     """
     img_format = image.format
     img = image.copy()
     img_size = img.size
     ratio = max(size[0] / img_size[0], size[1] / img_size[1])
     new_size = [
         int(math.ceil(img_size[0] * ratio)),
-        int(math.ceil(img_size[1] * ratio))
+        int(math.ceil(img_size[1] * ratio)),
     ]
     img = img.resize((new_size[0], new_size[1]))
     img = resize_crop(img, size)
     img.format = img_format
     return img
```

### Comparing `betty-0.3.3/betty/about.py` & `betty-0.3.4/betty/about.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 import aiofiles
 
 
 async def version() -> str | None:
     """
     Get the current Betty installation's version, if it has any.
     """
-    async with aiofiles.open(Path(__file__).parent / 'assets' / 'VERSION', encoding='utf-8') as f:
+    async with aiofiles.open(
+        Path(__file__).parent / "assets" / "VERSION", encoding="utf-8"
+    ) as f:
         release_version = (await f.read()).strip()
-    if release_version == '0.0.0':
+    if release_version == "0.0.0":
         return None
     return release_version
 
 
 async def version_label() -> str:
     """
     Get the human-readable label for the current Betty installation's version.
     """
-    return await version() or 'development'
+    return await version() or "development"
 
 
 async def is_stable() -> bool:
     """
     Check if the current Betty installation is a stable version.
     """
     return await version() is not None
@@ -41,36 +43,44 @@
     Check if the current Betty installation is an unstable development version.
     """
     return await version() is None
 
 
 def _indent_mapping(items: dict[str, str]) -> str:
     max_indentation = max(map(len, items.keys())) + 4
-    return '\n'.join(map(lambda x: '\n'.join(_indent_mapping_item(x[0], x[1], max_indentation)), items.items()))
+    return "\n".join(
+        map(
+            lambda x: "\n".join(_indent_mapping_item(x[0], x[1], max_indentation)),
+            items.items(),
+        )
+    )
 
 
 def _indent_mapping_item(key: str, value: str, max_indentation: int) -> Iterator[str]:
-    lines = value.split('\n')
+    lines = value.split("\n")
     yield f'{key}{" " * (max_indentation - len(key))}    {lines[0]}'
     for line in lines[1:]:
         yield f'{" " * max_indentation}    {line}'
 
 
 async def report() -> str:
     """
     Produce a human-readable report about the current Betty installation.
 
     :returns: A human-readable string in US English, using monospace indentation.
     """
-    return _indent_mapping({
-        'Betty': await version_label(),
-        'Operating system': platform.platform(),
-        'Python': sys.version,
-        'Python packages': _indent_mapping({
-            x.metadata['Name']: x.version
-            for x
-            in sorted(
-                distributions(),
-                key=lambda x: x.metadata['Name'].lower(),  # type: ignore[no-any-return, unused-ignore]
-            )
-        }),
-    })
+    return _indent_mapping(
+        {
+            "Betty": await version_label(),
+            "Operating system": platform.platform(),
+            "Python": sys.version,
+            "Python packages": _indent_mapping(
+                {
+                    x.metadata["Name"]: x.version
+                    for x in sorted(
+                        distributions(),
+                        key=lambda x: x.metadata["Name"].lower(),  # type: ignore[no-any-return, unused-ignore]
+                    )
+                }
+            ),
+        }
+    )
```

### Comparing `betty-0.3.3/betty/app/__init__.py` & `betty-0.3.4/betty/app/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,47 +6,82 @@
 import weakref
 from collections.abc import AsyncIterator
 from concurrent.futures import Executor, ProcessPoolExecutor
 from contextlib import suppress, asynccontextmanager
 from functools import reduce
 from graphlib import CycleError, TopologicalSorter
 from multiprocessing import get_context
+from os import environ
 from pathlib import Path
 from types import TracebackType
 from typing import TYPE_CHECKING, Mapping, Self, Any, final
 
 import aiohttp
 from aiofiles.tempfile import TemporaryDirectory
 
 from betty import fs
-from betty.app.extension import ListExtensions, Extension, Extensions, build_extension_type_graph, \
-    CyclicDependencyError, ExtensionDispatcher, ConfigurableExtension, discover_extension_types
+from betty.app.extension import (
+    ListExtensions,
+    Extension,
+    Extensions,
+    build_extension_type_graph,
+    CyclicDependencyError,
+    ExtensionDispatcher,
+    ConfigurableExtension,
+)
 from betty.asyncio import wait_to_thread
 from betty.cache import Cache, FileCache
 from betty.cache.file import BinaryFileCache, PickledFileCache
 from betty.config import Configurable, FileBasedConfiguration
 from betty.dispatch import Dispatcher
 from betty.fs import FileSystem, CACHE_DIRECTORY_PATH
 from betty.locale import LocalizerRepository, get_data, DEFAULT_LOCALE, Localizer, Str
 from betty.model import Entity, EntityTypeProvider
-from betty.model.event_type import EventType, EventTypeProvider, Birth, Baptism, Adoption, Death, Funeral, Cremation, \
-    Burial, Will, Engagement, Marriage, MarriageAnnouncement, Divorce, DivorceAnnouncement, Residence, Immigration, \
-    Emigration, Occupation, Retirement, Correspondence, Confirmation
+from betty.model.event_type import (
+    EventType,
+    EventTypeProvider,
+    Birth,
+    Baptism,
+    Adoption,
+    Death,
+    Funeral,
+    Cremation,
+    Burial,
+    Will,
+    Engagement,
+    Marriage,
+    MarriageAnnouncement,
+    Divorce,
+    DivorceAnnouncement,
+    Residence,
+    Immigration,
+    Emigration,
+    Occupation,
+    Retirement,
+    Correspondence,
+    Confirmation,
+)
 from betty.project import Project
 from betty.render import Renderer, SequentialRenderer
 from betty.serde.dump import minimize, void_none, Dump, VoidableDump
-from betty.serde.load import AssertionFailed, Fields, Assertions, OptionalField, Asserter
+from betty.serde.load import (
+    AssertionFailed,
+    Fields,
+    Assertions,
+    OptionalField,
+    Asserter,
+)
 from betty.warnings import deprecate
 
 if TYPE_CHECKING:
     from betty.jinja2 import Environment
     from betty.serve import Server
     from betty.url import StaticUrlGenerator, LocalizedUrlGenerator
 
-CONFIGURATION_DIRECTORY_PATH = fs.HOME_DIRECTORY_PATH / 'configuration'
+CONFIGURATION_DIRECTORY_PATH = fs.HOME_DIRECTORY_PATH / "configuration"
 
 
 class _AppExtensions(ListExtensions):
     def __init__(self):
         super().__init__([])
 
     def _update(self, extensions: list[list[Extension]]) -> None:
@@ -58,25 +93,25 @@
         self,
         configuration_directory_path: Path | None = None,
         *,
         locale: str | None = None,
     ):
         if configuration_directory_path is None:
             deprecate(
-                f'Initializing {type(self)} without a configuration directory path is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x.',
+                f"Initializing {type(self)} without a configuration directory path is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x.",
                 stacklevel=2,
             )
             configuration_directory_path = CONFIGURATION_DIRECTORY_PATH
         super().__init__()
         self._configuration_directory_path = configuration_directory_path
         self._locale: str | None = locale
 
     @property
     def configuration_file_path(self) -> Path:
-        return self._configuration_directory_path / 'app.json'
+        return self._configuration_directory_path / "app.json"
 
     @configuration_file_path.setter
     def configuration_file_path(self, __) -> None:
         pass
 
     @configuration_file_path.deleter
     def configuration_file_path(self) -> None:
@@ -87,46 +122,49 @@
         return self._locale
 
     @locale.setter
     def locale(self, locale: str) -> None:
         try:
             get_data(locale)
         except ValueError:
-            raise AssertionFailed(Str._(
-                '"{locale}" is not a valid IETF BCP 47 language tag.',
-                locale=locale,
-            ))
+            raise AssertionFailed(
+                Str._(
+                    '"{locale}" is not a valid IETF BCP 47 language tag.',
+                    locale=locale,
+                )
+            )
         self._locale = locale
         self._dispatch_change()
 
     def update(self, other: Self) -> None:
         self._locale = other._locale
         self._dispatch_change()
 
     @classmethod
     def load(
-            cls,
-            dump: Dump,
-            configuration: Self | None = None,
+        cls,
+        dump: Dump,
+        configuration: Self | None = None,
     ) -> Self:
         if configuration is None:
             configuration = cls()
         asserter = Asserter()
-        asserter.assert_record(Fields(
-            OptionalField(
-                'locale',
-                Assertions(asserter.assert_str()) | asserter.assert_setattr(configuration, 'locale')),
-        ),
+        asserter.assert_record(
+            Fields(
+                OptionalField(
+                    "locale",
+                    Assertions(asserter.assert_str())
+                    | asserter.assert_setattr(configuration, "locale"),
+                ),
+            ),
         )(dump)
         return configuration
 
     def dump(self) -> VoidableDump:
-        return minimize({
-            'locale': void_none(self.locale)
-        }, True)
+        return minimize({"locale": void_none(self.locale)}, True)
 
 
 class _BackwardsCompatiblePickledFileCache(PickledFileCache[Any], FileCache):
     """
     Provide a Backwards Compatible cache.
 
     .. deprecated:: 0.3.3
@@ -146,20 +184,20 @@
         project: Project | None = None,
         cache_directory_path: Path | None = None,
     ):
         super().__init__()
         self._started = False
         if configuration is None:
             deprecate(
-                f'Initializing {type(self)} without `configuration` is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x.',
+                f"Initializing {type(self)} without `configuration` is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x.",
                 stacklevel=2,
             )
         if cache_directory_path is None:
             deprecate(
-                f'Initializing {type(self)} without `cache_directory_path` is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x.',
+                f"Initializing {type(self)} without `cache_directory_path` is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x.",
                 stacklevel=2,
             )
         self._configuration = configuration or AppConfiguration()
         self._configuration.on_change(self._on_locale_change)
         self._assets: FileSystem | None = None
         self._extensions = _AppExtensions()
         self._extensions_initialized = False
@@ -175,30 +213,34 @@
         self._entity_types: set[type[Entity]] | None = None
         self._event_types: set[type[EventType]] | None = None
         self._url_generator: LocalizedUrlGenerator | None = None
         self._static_url_generator: StaticUrlGenerator | None = None
         self._jinja2_environment: Environment | None = None
         self._renderer: Renderer | None = None
         self._http_client: aiohttp.ClientSession | None = None
-        self._cache_directory_path = CACHE_DIRECTORY_PATH if cache_directory_path is None else cache_directory_path
+        self._cache_directory_path = (
+            CACHE_DIRECTORY_PATH
+            if cache_directory_path is None
+            else cache_directory_path
+        )
         self._cache: Cache[Any] & FileCache | None = None
         self._binary_file_cache: BinaryFileCache | None = None
         self._process_pool: Executor | None = None
 
     @classmethod
     @asynccontextmanager
     async def new_from_environment(
         cls,
         *,
         project: Project | None = None,
     ) -> AsyncIterator[Self]:
         yield cls(
             AppConfiguration(CONFIGURATION_DIRECTORY_PATH),
             project,
-            CACHE_DIRECTORY_PATH,
+            Path(environ.get("BETTY_CACHE_DIRECTORY", CACHE_DIRECTORY_PATH)),
         )
 
     @classmethod
     @asynccontextmanager
     async def new_from_app(
         cls,
         app: App,
@@ -228,98 +270,123 @@
                 cache_directory_path=Path(cache_directory_path_str),
             )
 
     async def __aenter__(self) -> Self:
         await self.start()
         return self
 
-    async def __aexit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
         await self.stop()
 
     async def start(self) -> None:
         if self._started:
-            raise RuntimeError('This app has started already.')
+            raise RuntimeError("This app has started already.")
         self._started = True
 
     async def stop(self) -> None:
         del self.http_client
         self._started = False
 
     def __del__(self) -> None:
         if self._started:
-            raise RuntimeError(f'{self} was started, but never stopped.')
+            raise RuntimeError(f"{self} was started, but never stopped.")
 
     def _on_locale_change(self) -> None:
         del self.localizer
         del self.localizers
 
     @property
     def project(self) -> Project:
         return self._project
 
     def discover_extension_types(self) -> set[type[Extension]]:
-        return {*discover_extension_types(), *map(type, self._extensions.flatten())}
+        from betty.app import extension
+
+        return {
+            *extension.discover_extension_types(),
+            *map(type, self._extensions.flatten()),
+        }
 
     @property
     def extensions(self) -> Extensions:
         if not self._extensions_initialized:
             self._extensions_initialized = True
             self._update_extensions()
 
         return self._extensions
 
     def _update_extensions(self) -> None:
         extension_types_enabled_in_configuration = set()
-        for app_extension_configuration in self.project.configuration.extensions.values():
+        for (
+            app_extension_configuration
+        ) in self.project.configuration.extensions.values():
             if app_extension_configuration.enabled:
                 app_extension_configuration.extension_type.enable_requirement().assert_met()
-                extension_types_enabled_in_configuration.add(app_extension_configuration.extension_type)
+                extension_types_enabled_in_configuration.add(
+                    app_extension_configuration.extension_type
+                )
 
         extension_types_sorter = TopologicalSorter(
             build_extension_type_graph(extension_types_enabled_in_configuration)
         )
         try:
             extension_types_sorter.prepare()
         except CycleError:
-            raise CyclicDependencyError([
-                app_extension_configuration.extension_type
-                for app_extension_configuration
-                in self.project.configuration.extensions.values()
-            ])
+            raise CyclicDependencyError(
+                [
+                    app_extension_configuration.extension_type
+                    for app_extension_configuration in self.project.configuration.extensions.values()
+                ]
+            )
 
         extensions = []
         while extension_types_sorter.is_active():
             extension_types_batch = extension_types_sorter.get_ready()
             extensions_batch = []
             for extension_type in extension_types_batch:
-                if issubclass(extension_type, ConfigurableExtension) and extension_type in self.project.configuration.extensions:
-                    extension: Extension = extension_type(self, configuration=self.project.configuration.extensions[extension_type].extension_configuration)
+                if (
+                    issubclass(extension_type, ConfigurableExtension)
+                    and extension_type in self.project.configuration.extensions
+                ):
+                    extension: Extension = extension_type(
+                        self,
+                        configuration=self.project.configuration.extensions[
+                            extension_type
+                        ].extension_configuration,
+                    )
                 else:
                     extension = extension_type(self)
                 extensions_batch.append(extension)
                 extension_types_sorter.done(extension_type)
-            extensions.append(sorted(extensions_batch, key=lambda extension: extension.name()))
+            extensions.append(
+                sorted(extensions_batch, key=lambda extension: extension.name())
+            )
         self._extensions._update(extensions)
         del self.assets
         del self.localizers
         del self.localizer
         del self.jinja2_environment
         del self.renderer
         del self.entity_types
         del self.event_types
 
     @property
     def assets(self) -> FileSystem:
         if self._assets is None:
             assets = FileSystem()
-            assets.prepend(fs.ASSETS_DIRECTORY_PATH, 'utf-8')
+            assets.prepend(fs.ASSETS_DIRECTORY_PATH, "utf-8")
             for extension in self.extensions.flatten():
                 extension_assets_directory_path = extension.assets_directory_path()
                 if extension_assets_directory_path is not None:
-                    assets.prepend(extension_assets_directory_path, 'utf-8')
+                    assets.prepend(extension_assets_directory_path, "utf-8")
             assets.prepend(self.project.configuration.assets_directory_path)
             self._assets = assets
         return self._assets
 
     @assets.deleter
     def assets(self) -> None:
         self._assets = None
@@ -340,24 +407,30 @@
         return self._url_generator
 
     @property
     def static_url_generator(self) -> StaticUrlGenerator:
         from betty.url import StaticPathUrlGenerator
 
         if self._static_url_generator is None:
-            self._static_url_generator = StaticPathUrlGenerator(self.project.configuration)
+            self._static_url_generator = StaticPathUrlGenerator(
+                self.project.configuration
+            )
         return self._static_url_generator
 
     @property
     def localizer(self) -> Localizer:
         """
         Get the application's localizer.
         """
         if self._localizer is None:
-            self._localizer = wait_to_thread(self.localizers.get_negotiated(self.configuration.locale or DEFAULT_LOCALE))
+            self._localizer = wait_to_thread(
+                self.localizers.get_negotiated(
+                    self.configuration.locale or DEFAULT_LOCALE
+                )
+            )
         return self._localizer
 
     @localizer.deleter
     def localizer(self) -> None:
         self._localizer = None
         del self.cache
         del self.binary_file_cache
@@ -372,61 +445,86 @@
     def localizers(self) -> None:
         self._localizers = None
 
     @property
     def jinja2_environment(self) -> Environment:
         if not self._jinja2_environment:
             from betty.jinja2 import Environment
+
             self._jinja2_environment = Environment(self)
 
         return self._jinja2_environment
 
     @jinja2_environment.deleter
     def jinja2_environment(self) -> None:
         self._jinja2_environment = None
 
     @property
     def renderer(self) -> Renderer:
         if not self._renderer:
             from betty.jinja2 import Jinja2Renderer
 
-            self._renderer = SequentialRenderer([
-                Jinja2Renderer(self.jinja2_environment, self.project.configuration),
-            ])
+            self._renderer = SequentialRenderer(
+                [
+                    Jinja2Renderer(self.jinja2_environment, self.project.configuration),
+                ]
+            )
 
         return self._renderer
 
     @renderer.deleter
     def renderer(self) -> None:
         self._renderer = None
 
     @property
     def http_client(self) -> aiohttp.ClientSession:
         if not self._http_client:
             self._http_client = aiohttp.ClientSession(
                 connector=aiohttp.TCPConnector(limit_per_host=5),
                 headers={
-                    'User-Agent': f'Betty (https://github.com/bartfeenstra/betty) on behalf of {self._project.configuration.base_url}{self._project.configuration.root_path}',
+                    "User-Agent": f"Betty (https://github.com/bartfeenstra/betty) on behalf of {self._project.configuration.base_url}{self._project.configuration.root_path}",
                 },
             )
-            weakref.finalize(self, lambda: None if self._http_client is None else wait_to_thread(self._http_client.close()))
+            weakref.finalize(
+                self,
+                lambda: (
+                    None
+                    if self._http_client is None
+                    else wait_to_thread(self._http_client.close())
+                ),
+            )
         return self._http_client
 
     @http_client.deleter
     def http_client(self) -> None:
         if self._http_client is not None:
             wait_to_thread(self._http_client.close())
             self._http_client = None
 
     @property
     def entity_types(self) -> set[type[Entity]]:
         if self._entity_types is None:
-            from betty.model.ancestry import Citation, Enclosure, Event, File, Note, Person, PersonName, Presence, Place, Source
+            from betty.model.ancestry import (
+                Citation,
+                Enclosure,
+                Event,
+                File,
+                Note,
+                Person,
+                PersonName,
+                Presence,
+                Place,
+                Source,
+            )
 
-            self._entity_types = reduce(operator.or_, wait_to_thread(self.dispatcher.dispatch(EntityTypeProvider)()), set()) | {
+            self._entity_types = reduce(
+                operator.or_,
+                wait_to_thread(self.dispatcher.dispatch(EntityTypeProvider)()),
+                set(),
+            ) | {
                 Citation,
                 Enclosure,
                 Event,
                 File,
                 Note,
                 Person,
                 PersonName,
@@ -439,15 +537,17 @@
     @entity_types.deleter
     def entity_types(self) -> None:
         self._entity_types = None
 
     @property
     def event_types(self) -> set[type[EventType]]:
         if self._event_types is None:
-            self._event_types = set(wait_to_thread(self.dispatcher.dispatch(EventTypeProvider)())) | {
+            self._event_types = set(
+                wait_to_thread(self.dispatcher.dispatch(EventTypeProvider)())
+            ) | {
                 Birth,
                 Baptism,
                 Adoption,
                 Death,
                 Funeral,
                 Cremation,
                 Burial,
@@ -474,47 +574,50 @@
     @property
     def servers(self) -> Mapping[str, Server]:
         from betty import serve
         from betty.extension.demo import DemoServer
 
         return {
             server.name(): server
-            for server
-            in [
+            for server in [
                 *(
                     server
                     for extension in self.extensions.flatten()
                     if isinstance(extension, serve.ServerProvider)
                     for server in extension.servers
                 ),
                 serve.BuiltinAppServer(self),
                 DemoServer(app=self),
             ]
         }
 
     @property
     def cache(self) -> Cache[Any] & FileCache:
         if self._cache is None:
-            self._cache = _BackwardsCompatiblePickledFileCache(self.localizer, self._cache_directory_path)
+            self._cache = _BackwardsCompatiblePickledFileCache(
+                self.localizer, self._cache_directory_path
+            )
         return self._cache
 
     @cache.deleter
     def cache(self) -> None:
         self._cache = None
 
     @property
     def binary_file_cache(self) -> BinaryFileCache:
         if self._binary_file_cache is None:
-            self._binary_file_cache = BinaryFileCache(self.localizer, self._cache_directory_path)
+            self._binary_file_cache = BinaryFileCache(
+                self.localizer, self._cache_directory_path
+            )
         return self._binary_file_cache
 
     @binary_file_cache.deleter
     def binary_file_cache(self) -> None:
         self._binary_file_cache = None
 
     @property
     def process_pool(self) -> Executor:
         if self._process_pool is None:
             # Avoid `fork` so as not to start worker processes with unneeded resources.
             # Settle for `spawn` so all environments use the same start method.
-            self._process_pool = ProcessPoolExecutor(mp_context=get_context('spawn'))
+            self._process_pool = ProcessPoolExecutor(mp_context=get_context("spawn"))
         return self._process_pool
```

### Comparing `betty-0.3.3/betty/app/extension/__init__.py` & `betty-0.3.4/betty/app/extension/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 """Provide Betty's extension API."""
+
 from __future__ import annotations
 
 import functools
 from collections import defaultdict
 from importlib.metadata import entry_points, EntryPoint
 from pathlib import Path
-from typing import Any, TypeVar, Iterable, TYPE_CHECKING, Generic, \
-    Iterator, Sequence, Self
+from typing import (
+    Any,
+    TypeVar,
+    Iterable,
+    TYPE_CHECKING,
+    Generic,
+    Iterator,
+    Sequence,
+    Self,
+)
 
-from betty.app.extension.requirement import Requirement, AllRequirements
+from betty.requirement import Requirement, AllRequirements
 from betty.asyncio import gather
 from betty.config import ConfigurationT, Configurable
 from betty.dispatch import Dispatcher, TargetedDispatcher
 from betty.importlib import import_any
 from betty.locale import Str
 
 if TYPE_CHECKING:
@@ -29,30 +38,36 @@
 
 class ExtensionTypeImportError(ExtensionTypeError, ImportError):
     """
     Raised when an alleged extension type cannot be imported.
     """
 
     def __init__(self, extension_type_name: str):
-        super().__init__(f'Cannot find and import an extension with name "{extension_type_name}".')
+        super().__init__(
+            f'Cannot find and import an extension with name "{extension_type_name}".'
+        )
 
 
 class ExtensionTypeInvalidError(ExtensionTypeError, ImportError):
     """
     Raised for types that are not valid extension types.
     """
 
     def __init__(self, extension_type: type):
-        super().__init__(f'{extension_type.__module__}.{extension_type.__name__} is not an extension type class. Extension types must extend {Extension.__module__}.{Extension.__name__}.')
+        super().__init__(
+            f"{extension_type.__module__}.{extension_type.__name__} is not an extension type class. Extension types must extend {Extension.__module__}.{Extension.__name__}."
+        )
 
 
 class CyclicDependencyError(ExtensionError, RuntimeError):
     def __init__(self, extension_types: Iterable[type[Extension]]):
-        extension_names = ', '.join([extension.name() for extension in extension_types])
-        super().__init__(f'The following extensions have cyclic dependencies: {extension_names}')
+        extension_names = ", ".join([extension.name() for extension in extension_types])
+        super().__init__(
+            f"The following extensions have cyclic dependencies: {extension_names}"
+        )
 
 
 class Dependencies(AllRequirements):
     def __init__(self, dependent_type: type[Extension]):
         dependency_requirements = []
         for dependency_type in dependent_type.depends_on():
             try:
@@ -66,20 +81,22 @@
 
     @classmethod
     def for_dependent(cls, dependent_type: type[Extension]) -> Self:
         return cls(dependent_type)
 
     def summary(self) -> Str:
         return Str._(
-            '{dependent_label} requires {dependency_labels}.',
+            "{dependent_label} requires {dependency_labels}.",
             dependent_label=format_extension_type(self._dependent_type),
             dependency_labels=Str.call(
-                lambda localizer: ', '.join(
+                lambda localizer: ", ".join(
                     map(
-                        lambda extension_type: format_extension_type(extension_type).localize(localizer),
+                        lambda extension_type: format_extension_type(
+                            extension_type
+                        ).localize(localizer),
                         self._dependent_type.depends_on(),
                     ),
                 ),
             ),
         )
 
 
@@ -87,35 +104,38 @@
     def __init__(self, dependency: Extension, dependents: Sequence[Extension]):
         super().__init__()
         self._dependency = dependency
         self._dependents = dependents
 
     def summary(self) -> Str:
         return Str._(
-            '{dependency_label} is required by {dependency_labels}.',
+            "{dependency_label} is required by {dependency_labels}.",
             dependency_label=format_extension_type(type(self._dependency)),
-            dependent_labels=Str.call(lambda localizer: ', '.join([
-                format_extension_type(type(dependent)).localize(localizer)
-                for dependent
-                in self._dependents
-            ])),
+            dependent_labels=Str.call(
+                lambda localizer: ", ".join(
+                    [
+                        format_extension_type(type(dependent)).localize(localizer)
+                        for dependent in self._dependents
+                    ]
+                )
+            ),
         )
 
     def is_met(self) -> bool:
         # This class is never instantiated unless there is at least one enabled dependent, which means this requirement
         # is always met.
         return True
 
     @classmethod
     def for_dependency(cls, dependency: Extension) -> Self:
         dependents = [
             dependency.app.extensions[extension_type]
-            for extension_type
-            in discover_extension_types()
-            if dependency.__class__ in extension_type.depends_on() and extension_type in dependency.app.extensions
+            for extension_type in discover_extension_types()
+            if dependency.__class__ in extension_type.depends_on()
+            and extension_type in dependency.app.extensions
         ]
         return cls(dependency, dependents)
 
 
 class Extension:
     """
     Integrate optional functionality with the Betty app.
@@ -124,15 +144,15 @@
     def __init__(self, app: App, *args: Any, **kwargs: Any):
         assert type(self) is not Extension
         super().__init__(*args, **kwargs)
         self._app = app
 
     @classmethod
     def name(cls) -> str:
-        return '%s.%s' % (cls.__module__, cls.__name__)
+        return "%s.%s" % (cls.__module__, cls.__name__)
 
     @classmethod
     def depends_on(cls) -> set[type[Extension]]:
         return set()
 
     @classmethod
     def comes_after(cls) -> set[type[Extension]]:
@@ -169,15 +189,15 @@
         return None
 
     @property
     def app(self) -> App:
         return self._app
 
 
-ExtensionT = TypeVar('ExtensionT', bound=Extension)
+ExtensionT = TypeVar("ExtensionT", bound=Extension)
 
 
 class UserFacingExtension(Extension):
     @classmethod
     def label(cls) -> Str:
         raise NotImplementedError(repr(cls))
 
@@ -187,19 +207,23 @@
 
 
 class Theme(UserFacingExtension):
     pass
 
 
 @functools.singledispatch
-def get_extension_type(extension_type_definition: str | type[Extension] | Extension) -> type[Extension]:
+def get_extension_type(
+    extension_type_definition: str | type[Extension] | Extension,
+) -> type[Extension]:
     """
     Get the extension type for an extension, extension type, or extension type name.
     """
-    raise ExtensionTypeError(f'Cannot get the extension type for "{extension_type_definition}".')
+    raise ExtensionTypeError(
+        f'Cannot get the extension type for "{extension_type_definition}".'
+    )
 
 
 @get_extension_type.register(str)
 def get_extension_type_by_name(extension_type_name: str) -> type[Extension]:
     """
     Get the extension type for an extension type name.
     """
@@ -229,20 +253,26 @@
 
 
 def format_extension_type(extension_type: type[Extension]) -> Str:
     """
     Format an extension type to a human-readable label.
     """
     if issubclass(extension_type, UserFacingExtension):
-        return Str.call(lambda localizer: f'{extension_type.label().localize(localizer)} ({extension_type.name()})')
+        return Str.call(
+            lambda localizer: f"{extension_type.label().localize(localizer)} ({extension_type.name()})"
+        )
     return Str.plain(extension_type.name())
 
 
-class ConfigurableExtension(Extension, Generic[ConfigurationT], Configurable[ConfigurationT]):
-    def __init__(self, *args: Any, configuration: ConfigurationT | None = None, **kwargs: Any):
+class ConfigurableExtension(
+    Extension, Generic[ConfigurationT], Configurable[ConfigurationT]
+):
+    def __init__(
+        self, *args: Any, configuration: ConfigurationT | None = None, **kwargs: Any
+    ):
         assert type(self) is not ConfigurableExtension
         super().__init__(*args, **kwargs)
         self._configuration = configuration or self.default_configuration()
 
     @classmethod
     def default_configuration(cls) -> ConfigurationT:
         raise NotImplementedError(repr(cls))
@@ -297,38 +327,47 @@
 
 
 class ExtensionDispatcher(Dispatcher):
     def __init__(self, extensions: Extensions):
         self._extensions = extensions
 
     def dispatch(self, target_type: type[Any]) -> TargetedDispatcher:
-        target_method_names = [method_name for method_name in dir(target_type) if not method_name.startswith('_')]
+        target_method_names = [
+            method_name
+            for method_name in dir(target_type)
+            if not method_name.startswith("_")
+        ]
         if len(target_method_names) != 1:
-            raise ValueError(f"A dispatch's target type must have a single method to dispatch to, but {target_type} has {len(target_method_names)}.")
+            raise ValueError(
+                f"A dispatch's target type must have a single method to dispatch to, but {target_type} has {len(target_method_names)}."
+            )
         target_method_name = target_method_names[0]
 
         async def _dispatch(*args: Any, **kwargs: Any) -> list[Any]:
             return [
                 result
-                for target_extension_batch
-                in self._extensions
-                for result
-                in await gather(*(
-                    getattr(target_extension, target_method_name)(*args, **kwargs)
-                    for target_extension in target_extension_batch
-                    if isinstance(target_extension, target_type)
-                ))
+                for target_extension_batch in self._extensions
+                for result in await gather(
+                    *(
+                        getattr(target_extension, target_method_name)(*args, **kwargs)
+                        for target_extension in target_extension_batch
+                        if isinstance(target_extension, target_type)
+                    )
+                )
             ]
+
         return _dispatch
 
 
 ExtensionTypeGraph = dict[type[Extension], set[type[Extension]]]
 
 
-def build_extension_type_graph(extension_types: Iterable[type[Extension]]) -> ExtensionTypeGraph:
+def build_extension_type_graph(
+    extension_types: Iterable[type[Extension]],
+) -> ExtensionTypeGraph:
     """
     Build a dependency graph of the given extension types.
     """
     extension_types_graph: ExtensionTypeGraph = defaultdict(set)
     # Add dependencies to the extension graph.
     for extension_type in extension_types:
         _extend_extension_type_graph(extension_types_graph, extension_type)
@@ -340,15 +379,17 @@
         for after in extension_type.comes_after():
             if after in extension_types_graph:
                 extension_types_graph[extension_type].add(after)
 
     return extension_types_graph
 
 
-def _extend_extension_type_graph(graph: ExtensionTypeGraph, extension_type: type[Extension]) -> None:
+def _extend_extension_type_graph(
+    graph: ExtensionTypeGraph, extension_type: type[Extension]
+) -> None:
     dependencies = extension_type.depends_on()
     # Ensure each extension type appears in the graph, even if they're isolated.
     graph.setdefault(extension_type, set())
     for dependency in dependencies:
         seen_dependency = dependency in graph
         graph[extension_type].add(dependency)
         if not seen_dependency:
@@ -357,10 +398,12 @@
 
 def discover_extension_types() -> set[type[Extension]]:
     """
     Gather the available extension types.
     """
     betty_entry_points: Sequence[EntryPoint]
     betty_entry_points = entry_points(  # type: ignore[assignment, unused-ignore]
-        group='betty.extensions',  # type: ignore[call-arg, unused-ignore]
+        group="betty.extensions",  # type: ignore[call-arg, unused-ignore]
     )
-    return {import_any(betty_entry_point.value) for betty_entry_point in betty_entry_points}
+    return {
+        import_any(betty_entry_point.value) for betty_entry_point in betty_entry_points
+    }
```

### Comparing `betty-0.3.3/betty/app/extension/requirement.py` & `betty-0.3.4/betty/requirement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide an API that lets code express arbitrary requirements.
 """
+
 from __future__ import annotations
 
 from textwrap import indent
 from typing import cast, Any, Self
 
 from betty.error import UserFacingError
 from betty.locale import Str, Localizable, Localizer
@@ -26,15 +27,15 @@
         return None
 
     def localize(self, localizer: Localizer) -> str:
         string = self.summary().localize(localizer)
         details = self.details()
         if details is not None:
             string += f'\n{"-" * len(string)}'
-            string += f'\n{details.localize(localizer)}'
+            string += f"\n{details.localize(localizer)}"
         return string
 
     def reduce(self) -> Requirement | None:
         """
         Remove unnecessary components of this requirement.
 
         - Collections can flatten unnecessary hierarchies.
@@ -56,15 +57,17 @@
     def requirement(self) -> Requirement:
         return self._requirement
 
 
 class RequirementCollection(Requirement):
     def __init__(self, *requirements: Requirement | None):
         super().__init__()
-        self._requirements: list[Requirement] = [requirement for requirement in requirements if requirement]
+        self._requirements: list[Requirement] = [
+            requirement for requirement in requirements if requirement
+        ]
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, type(self)):
             return False
         return self._requirements == other._requirements
 
     def __add__(self, other: Any) -> Self:
@@ -81,43 +84,45 @@
 
     def reduce(self) -> Requirement | None:
         reduced_requirements = []
         for requirement in self._requirements:
             reduced_requirement = requirement.reduce()
             if reduced_requirement:
                 if type(reduced_requirement) is type(self):
-                    reduced_requirements.extend(cast(RequirementCollection, reduced_requirement)._requirements)
+                    reduced_requirements.extend(
+                        cast(RequirementCollection, reduced_requirement)._requirements
+                    )
                 else:
                     reduced_requirements.append(reduced_requirement)
         if len(reduced_requirements) == 1:
             return reduced_requirements[0]
         if reduced_requirements:
             return type(self)(*reduced_requirements)
         return None
 
 
 class AnyRequirement(RequirementCollection):
     def __init__(self, *requirements: Requirement | None):
         super().__init__(*requirements)
-        self._summary = Str._('One or more of these requirements must be met')
+        self._summary = Str._("One or more of these requirements must be met")
 
     def is_met(self) -> bool:
         for requirement in self._requirements:
             if requirement.is_met():
                 return True
         return False
 
     def summary(self) -> Str:
         return self._summary
 
 
 class AllRequirements(RequirementCollection):
     def __init__(self, *requirements: Requirement | None):
         super().__init__(*requirements)
-        self._summary = Str._('All of these requirements must be met')
+        self._summary = Str._("All of these requirements must be met")
 
     def is_met(self) -> bool:
         for requirement in self._requirements:
             if not requirement.is_met():
                 return False
         return True
```

### Comparing `betty-0.3.3/betty/assets/betty.pot` & `betty-0.3.4/betty/assets/betty.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: Betty VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-03-27 23:37+0000\n"
+"POT-Creation-Date: 2024-04-30 22:56+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.14.0\n"
@@ -185,24 +185,15 @@
 
 msgid "Betty project configuration ({supported_formats})"
 msgstr ""
 
 msgid "Birth"
 msgstr ""
 
-msgid "Built the Cotton Candy front-end assets."
-msgstr ""
-
-msgid "Built the HTTP API documentation."
-msgstr ""
-
-msgid "Built the interactive family trees."
-msgstr ""
-
-msgid "Built the interactive maps."
+msgid "Built the Webpack front-end assets."
 msgstr ""
 
 msgid "Burial"
 msgstr ""
 
 msgid "Cancel"
 msgstr ""
@@ -586,18 +577,18 @@
 
 msgid "Place"
 msgstr ""
 
 msgid "Places"
 msgstr ""
 
-msgid "Pre-built assets"
+msgid "Pre-built Webpack front-end assets are available"
 msgstr ""
 
-msgid "Pre-built assets are unavailable for {extension_names}."
+msgid "Pre-built Webpack front-end assets are unavailable"
 msgstr ""
 
 msgid "Presence"
 msgstr ""
 
 msgid "Presence of {person} at {event}"
 msgstr ""
```

### Comparing `betty-0.3.3/betty/assets/locale/de-DE/betty.po` & `betty-0.3.4/betty/assets/locale/de-DE/betty.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Betty project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Betty VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-03-27 23:37+0000\n"
+"POT-Creation-Date: 2024-04-30 22:56+0100\n"
 "PO-Revision-Date: 2024-02-08 13:24+0000\n"
 "Last-Translator: Bart Feenstra <bart@bartfeenstra.com>\n"
 "Language: de\n"
 "Language-Team: rainerthi@gmail.com\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -275,25 +275,16 @@
 
 msgid "Betty project configuration ({supported_formats})"
 msgstr "Betty-Projektkonfiguration ({supported_formats})"
 
 msgid "Birth"
 msgstr "Geburt"
 
-msgid "Built the Cotton Candy front-end assets."
-msgstr "Cotton Candy front-end assets erstellt."
-
-msgid "Built the HTTP API documentation."
-msgstr "Die HTTP-API-Dokumentation wurde erstellt."
-
-msgid "Built the interactive family trees."
-msgstr "Die interaktiven Stammbäume sind erstellt."
-
-msgid "Built the interactive maps."
-msgstr "Die interaktiven Karten wurden erstellt."
+msgid "Built the Webpack front-end assets."
+msgstr "Webpack front-end assets erstellt."
 
 msgid "Burial"
 msgstr "Beerdigung"
 
 msgid "Cancel"
 msgstr "Abbrechen"
 
@@ -756,19 +747,19 @@
 
 msgid "Place"
 msgstr "Ort"
 
 msgid "Places"
 msgstr "Orte"
 
-msgid "Pre-built assets"
-msgstr "Vorgefertigte Objekte"
+msgid "Pre-built Webpack front-end assets are available"
+msgstr "Vorgefertigte Webpack front-end assets sind verfügbar"
 
-msgid "Pre-built assets are unavailable for {extension_names}."
-msgstr "Vorgefertigte Objekte für {extension_names} sind nicht verfügbar."
+msgid "Pre-built Webpack front-end assets are unavailable"
+msgstr "Vorgefertigte Webpack front-end assets sind nicht verfügbar"
 
 msgid "Presence"
 msgstr "Anwesenheit"
 
 msgid "Presence of {person} at {event}"
 msgstr "Anwesenheit von {person} zum {event}"
```

### Comparing `betty-0.3.3/betty/assets/locale/fr-FR/betty.po` & `betty-0.3.4/betty/assets/locale/fr-FR/betty.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2019.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-03-27 23:37+0000\n"
+"POT-Creation-Date: 2024-04-30 22:56+0100\n"
 "PO-Revision-Date: 2024-02-08 13:24+0000\n"
 "Last-Translator: Bart Feenstra <bart@bartfeenstra.com>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -229,24 +229,15 @@
 
 msgid "Betty project configuration ({supported_formats})"
 msgstr ""
 
 msgid "Birth"
 msgstr "Naissance"
 
-msgid "Built the Cotton Candy front-end assets."
-msgstr ""
-
-msgid "Built the HTTP API documentation."
-msgstr ""
-
-msgid "Built the interactive family trees."
-msgstr ""
-
-msgid "Built the interactive maps."
+msgid "Built the Webpack front-end assets."
 msgstr ""
 
 msgid "Burial"
 msgstr "Enterrement"
 
 msgid "Cancel"
 msgstr ""
@@ -670,18 +661,18 @@
 
 msgid "Place"
 msgstr "Lieu"
 
 msgid "Places"
 msgstr "Lieux"
 
-msgid "Pre-built assets"
+msgid "Pre-built Webpack front-end assets are available"
 msgstr ""
 
-msgid "Pre-built assets are unavailable for {extension_names}."
+msgid "Pre-built Webpack front-end assets are unavailable"
 msgstr ""
 
 msgid "Presence"
 msgstr ""
 
 msgid "Presence of {person} at {event}"
 msgstr ""
```

### Comparing `betty-0.3.3/betty/assets/locale/nl-NL/betty.po` & `betty-0.3.4/betty/assets/locale/nl-NL/betty.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2019.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-03-27 23:37+0000\n"
+"POT-Creation-Date: 2024-04-30 22:56+0100\n"
 "PO-Revision-Date: 2024-02-11 15:31+0000\n"
 "Last-Translator: Bart Feenstra <bart@bartfeenstra.com>\n"
 "Language: nl\n"
 "Language-Team: nl <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -272,25 +272,16 @@
 
 msgid "Betty project configuration ({supported_formats})"
 msgstr "Betty-projectconfiguratie ({supported_formats})"
 
 msgid "Birth"
 msgstr "Geboorte"
 
-msgid "Built the Cotton Candy front-end assets."
-msgstr "De Cotton Candy front-endassets gegenereerd."
-
-msgid "Built the HTTP API documentation."
-msgstr "HTTP API-documentatie gegenereerd."
-
-msgid "Built the interactive family trees."
-msgstr "De interactieve stambomen gegenereerd."
-
-msgid "Built the interactive maps."
-msgstr "De interactieve kaarten gegenereerd."
+msgid "Built the Webpack front-end assets."
+msgstr "De Webpack front-end assets gebouwd."
 
 msgid "Burial"
 msgstr "Begravenis"
 
 msgid "Cancel"
 msgstr "Annuleren"
 
@@ -751,19 +742,19 @@
 
 msgid "Place"
 msgstr "Plaats"
 
 msgid "Places"
 msgstr "Plaatsen"
 
-msgid "Pre-built assets"
-msgstr "Kant-en-klare assets"
+msgid "Pre-built Webpack front-end assets are available"
+msgstr "Vooraf gebouwde Webpack front-end assets zijn beschikbaar."
 
-msgid "Pre-built assets are unavailable for {extension_names}."
-msgstr "Kant-en-klare assets zijn beschikbaar voor {extension_names}."
+msgid "Pre-built Webpack front-end assets are unavailable"
+msgstr "Vooraf gebouwde Webpack front-end assets zijn niet beschikbaar."
 
 msgid "Presence"
 msgstr "Aanwezigheid"
 
 msgid "Presence of {person} at {event}"
 msgstr "Aanwezigheid van {person} bij {event}"
```

### Comparing `betty-0.3.3/betty/assets/locale/uk/betty.po` & `betty-0.3.4/betty/assets/locale/uk/betty.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Betty project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Betty VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-03-27 23:37+0000\n"
+"POT-Creation-Date: 2024-04-30 22:56+0100\n"
 "PO-Revision-Date: 2024-02-08 13:08+0000\n"
 "Last-Translator: Rainer Thieringer <rainerthi@gmail.com>\n"
 "Language: uk\n"
 "Language-Team: uk <LL@li.org>\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
@@ -229,24 +229,15 @@
 
 msgid "Betty project configuration ({supported_formats})"
 msgstr ""
 
 msgid "Birth"
 msgstr "Народження"
 
-msgid "Built the Cotton Candy front-end assets."
-msgstr ""
-
-msgid "Built the HTTP API documentation."
-msgstr ""
-
-msgid "Built the interactive family trees."
-msgstr ""
-
-msgid "Built the interactive maps."
+msgid "Built the Webpack front-end assets."
 msgstr ""
 
 msgid "Burial"
 msgstr "Поховання"
 
 msgid "Cancel"
 msgstr ""
@@ -670,18 +661,18 @@
 
 msgid "Place"
 msgstr "Місце"
 
 msgid "Places"
 msgstr "Місця"
 
-msgid "Pre-built assets"
+msgid "Pre-built Webpack front-end assets are available"
 msgstr ""
 
-msgid "Pre-built assets are unavailable for {extension_names}."
+msgid "Pre-built Webpack front-end assets are unavailable"
 msgstr ""
 
 msgid "Presence"
 msgstr ""
 
 msgid "Presence of {person} at {event}"
 msgstr ""
```

### Comparing `betty-0.3.3/betty/assets/public/static/betty-16x16.png` & `betty-0.3.4/betty/assets/public/static/betty-16x16.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/assets/public/static/betty-192x192.png` & `betty-0.3.4/betty/assets/public/static/betty-192x192.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/assets/public/static/betty-32x32.png` & `betty-0.3.4/betty/assets/public/static/betty-32x32.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/assets/public/static/betty-512x512.png` & `betty-0.3.4/betty/assets/public/static/betty-512x512.png`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/assets/public/static/betty.ico` & `betty-0.3.4/betty/assets/public/static/betty.ico`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/assets/templates/head.html.j2` & `betty-0.3.4/betty/assets/templates/head.html.j2`

 * *Files 4% similar despite different names*

```diff
@@ -37,13 +37,7 @@
         </script>
     {% endif %}
     {% if page_resource is entity and page_resource is not has_generated_entity_id %}
         <link rel="alternate" href="{{ page_resource | url(media_type='application/json') }}" hreflang="und" type="application/json">
     {% endif %}
 {% endif %}
 <link rel="icon" href="{{ '/betty.ico' | static_url }}">
-{% for css_path in public_css_paths %}
-    <link rel="stylesheet" href="{{ css_path }}">
-{% endfor %}
-{% for js_path in public_js_paths %}
-    <script src="{{ js_path }}" defer></script>
-{% endfor %}
```

#### html2text {}

```diff
@@ -7,10 +7,7 @@
 {% endif %} {% endif %} {% endfor %} {% endif %}
 {% for project_locale in app.project.configuration.locales %} {% if
 project_locale != localizer.locale %}
 {% endif %} {% endfor %} {% if page_resource is linked_data_dumpable %}
 {% endif %} {% if page_resource is entity and page_resource is not
 has_generated_entity_id %}
 {% endif %} {% endif %}
-{% for css_path in public_css_paths %}
-{% endfor %} {% for js_path in public_js_paths %}
-{% endfor %}
```

### Comparing `betty-0.3.3/betty/asyncio.py` & `betty-0.3.4/betty/asyncio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 """
 Provide asynchronous programming utilities.
 """
+
 from __future__ import annotations
 
 from asyncio import TaskGroup, get_running_loop, run
 from functools import wraps
 from threading import Thread
-from typing import Callable, Awaitable, TypeVar, Generic, cast, ParamSpec, Coroutine, Any
+from typing import (
+    Callable,
+    Awaitable,
+    TypeVar,
+    Generic,
+    cast,
+    ParamSpec,
+    Coroutine,
+    Any,
+)
 
 from betty.warnings import deprecated
 
-P = ParamSpec('P')
-T = TypeVar('T')
+P = ParamSpec("P")
+T = TypeVar("T")
 
 
 async def gather(*coroutines: Coroutine[Any, None, T]) -> tuple[T, ...]:
     """
     Gather multiple coroutines.
 
     This is like Python's own ``asyncio.gather``, but with improved error handling.
     """
     tasks = []
     async with TaskGroup() as task_group:
         for coroutine in coroutines:
             tasks.append(task_group.create_task(coroutine))
-    return tuple(
-        task.result()
-        for task
-        in tasks
-    )
+    return tuple(task.result() for task in tasks)
 
 
-@deprecated('This function is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x. Instead, use `betty.asyncio.wait_to_thread()` or `asyncio.run()`.')
+@deprecated(
+    "This function is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x. Instead, use `betty.asyncio.wait_to_thread()` or `asyncio.run()`."
+)
 def wait(f: Awaitable[T]) -> T:
     """
     Wait for an awaitable, either in a new event loop or another thread.
     """
     try:
         loop = get_running_loop()
     except RuntimeError:
@@ -54,22 +62,26 @@
     """
     synced = _WaiterThread(f)
     synced.start()
     synced.join()
     return synced.return_value
 
 
-@deprecated('This function is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x. Instead, use `betty.asyncio.wait_to_thread()` or `asyncio.run()`.')
+@deprecated(
+    "This function is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x. Instead, use `betty.asyncio.wait_to_thread()` or `asyncio.run()`."
+)
 def sync(f: Callable[P, Awaitable[T]]) -> Callable[P, T]:
     """
     Decorate an asynchronous callable to become synchronous.
     """
+
     @wraps(f)
     def _synced(*args: P.args, **kwargs: P.kwargs) -> T:
         return wait(f(*args, **kwargs))
+
     return _synced
 
 
 class _WaiterThread(Thread, Generic[T]):
     def __init__(self, awaitable: Awaitable[T]):
         super().__init__()
         self._awaitable = awaitable
@@ -84,9 +96,11 @@
 
     def run(self) -> None:
         run(self._run())
 
     async def _run(self) -> None:
         try:
             self._return_value = await self._awaitable
-        except BaseException as e:
+        except BaseException as e:  # noqa: B036
+            # Store the exception, so it can be reraised when the calling thread
+            # gets self.return_value.
             self._e = e
```

### Comparing `betty-0.3.3/betty/cache/__init__.py` & `betty-0.3.4/betty/cache/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Provide the Cache API.
 """
+
 from __future__ import annotations
 
 from collections.abc import Awaitable, Callable
 from pathlib import Path
 from typing import Self, Generic, TypeAlias, AsyncContextManager, overload, Literal
 
 import typing_extensions
 from typing_extensions import TypeVar
 
-CacheItemValueT = TypeVar('CacheItemValueT')
-CacheItemValueCoT = TypeVar('CacheItemValueCoT', covariant=True)
-CacheItemValueContraT = TypeVar('CacheItemValueContraT', contravariant=True)
+CacheItemValueT = TypeVar("CacheItemValueT")
+CacheItemValueCoT = TypeVar("CacheItemValueCoT", covariant=True)
+CacheItemValueContraT = TypeVar("CacheItemValueContraT", contravariant=True)
 
 
 class CacheItem(Generic[CacheItemValueCoT]):
     @property
     def modified(self) -> int | float:
         """
         Get the time this cache item was last modified, in seconds.
@@ -42,35 +43,60 @@
 
     def with_scope(self, scope: str) -> Self:
         """
         Return a new nested cache with the given scope.
         """
         raise NotImplementedError
 
-    def get(self, cache_item_id: str) -> AsyncContextManager[CacheItem[CacheItemValueContraT] | None]:
+    def get(
+        self, cache_item_id: str
+    ) -> AsyncContextManager[CacheItem[CacheItemValueContraT] | None]:
         """
         Get the cache item with the given ID.
         """
         raise NotImplementedError
 
-    async def set(self, cache_item_id: str, value: CacheItemValueContraT, *, modified: int | float | None = None) -> None:
+    async def set(
+        self,
+        cache_item_id: str,
+        value: CacheItemValueContraT,
+        *,
+        modified: int | float | None = None,
+    ) -> None:
         """
         Add or update a cache item.
         """
         raise NotImplementedError
 
     @overload
-    def getset(self, cache_item_id: str) -> AsyncContextManager[tuple[CacheItem[CacheItemValueContraT] | None, CacheItemValueSetter[CacheItemValueContraT]]]:
+    def getset(self, cache_item_id: str) -> AsyncContextManager[
+        tuple[
+            CacheItem[CacheItemValueContraT] | None,
+            CacheItemValueSetter[CacheItemValueContraT],
+        ]
+    ]:
         pass
 
     @overload
-    def getset(self, cache_item_id: str, *, wait: Literal[False] = False) -> AsyncContextManager[tuple[CacheItem[CacheItemValueContraT] | None, CacheItemValueSetter[CacheItemValueContraT] | None]]:
+    def getset(
+        self, cache_item_id: str, *, wait: Literal[False] = False
+    ) -> AsyncContextManager[
+        tuple[
+            CacheItem[CacheItemValueContraT] | None,
+            CacheItemValueSetter[CacheItemValueContraT] | None,
+        ]
+    ]:
         pass
 
-    def getset(self, cache_item_id: str, *, wait: bool = True) -> AsyncContextManager[tuple[CacheItem[CacheItemValueContraT] | None, CacheItemValueSetter[CacheItemValueContraT] | None]]:
+    def getset(self, cache_item_id: str, *, wait: bool = True) -> AsyncContextManager[
+        tuple[
+            CacheItem[CacheItemValueContraT] | None,
+            CacheItemValueSetter[CacheItemValueContraT] | None,
+        ]
+    ]:
         """
         Get the cache item with the given ID, and provide a setter to add or update it within the same atomic operation.
 
         If ``wait`` is ``False`` and no lock can be acquired, return ``None, None``.
         Otherwise return:
         0. A cache item if one could be found, or else ``None``.
         1. An asynchronous setter that takes the cache item's value as its only argument.
@@ -86,15 +112,17 @@
     async def clear(self) -> None:
         """
         Clear all items from the cache.
         """
         raise NotImplementedError
 
 
-@typing_extensions.deprecated(f"This class is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x. It exists only for App.cache's backwards compatibility. Use {Cache} instead.")
+@typing_extensions.deprecated(
+    f"This class is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x. It exists only for App.cache's backwards compatibility. Use {Cache} instead."
+)
 class FileCache:
     @property
     def path(self) -> Path:  # type: ignore[empty-body]
         pass
 
     async def clear(self) -> None:
         pass
```

### Comparing `betty-0.3.3/betty/cache/_base.py` & `betty-0.3.4/betty/cache/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import logging
 from collections import defaultdict
 from collections.abc import Sequence, MutableMapping, AsyncIterator
 from contextlib import asynccontextmanager
 from datetime import datetime
 from typing import Generic, Self, overload, AsyncContextManager, Literal
 
-from betty.cache import CacheItemValueCoT, Cache, CacheItem, CacheItemValueContraT, CacheItemValueSetter
+from betty.cache import (
+    CacheItemValueCoT,
+    Cache,
+    CacheItem,
+    CacheItemValueContraT,
+    CacheItemValueSetter,
+)
 from betty.concurrent import _Lock, AsynchronizedLock, MultiLock
 from betty.locale import Localizer
 
 
 class _StaticCacheItem(CacheItem[CacheItemValueCoT], Generic[CacheItemValueCoT]):
-    __slots__ = '_value', '_modified'
+    __slots__ = "_value", "_modified"
 
     def __init__(
         self,
         value: CacheItemValueCoT,
         modified: int | float | None = None,
     ):
         self._value = value
@@ -35,15 +41,17 @@
         localizer: Localizer,
         *,
         scopes: Sequence[str] | None = None,
     ):
         self._localizer = localizer
         self._scopes = scopes or ()
         self._scoped_caches: dict[str, Self] = {}
-        self._locks: MutableMapping[str, _Lock] = defaultdict(AsynchronizedLock.threading)
+        self._locks: MutableMapping[str, _Lock] = defaultdict(
+            AsynchronizedLock.threading
+        )
         self._locks_lock = AsynchronizedLock.threading()
 
     async def _lock(self, cache_item_id: str) -> _Lock:
         async with self._locks_lock:
             return self._locks[cache_item_id]
 
     def with_scope(self, scope: str) -> Self:
@@ -53,43 +61,76 @@
             self._scoped_caches[scope] = self._with_scope(scope)
             return self._scoped_caches[scope]
 
     def _with_scope(self, scope: str) -> Self:
         raise NotImplementedError
 
     @asynccontextmanager
-    async def get(self, cache_item_id: str) -> AsyncIterator[CacheItem[CacheItemValueContraT] | None]:
+    async def get(
+        self, cache_item_id: str
+    ) -> AsyncIterator[CacheItem[CacheItemValueContraT] | None]:
         async with await self._lock(cache_item_id):
             yield await self._get(cache_item_id)
 
     async def _get(self, cache_item_id: str) -> CacheItem[CacheItemValueContraT] | None:
         raise NotImplementedError
 
-    async def set(self, cache_item_id: str, value: CacheItemValueContraT, *, modified: int | float | None = None) -> None:
+    async def set(
+        self,
+        cache_item_id: str,
+        value: CacheItemValueContraT,
+        *,
+        modified: int | float | None = None,
+    ) -> None:
         async with await self._lock(cache_item_id):
             await self._set(cache_item_id, value, modified=modified)
 
-    async def _set(self, cache_item_id: str, value: CacheItemValueContraT, *, modified: int | float | None = None) -> None:
+    async def _set(
+        self,
+        cache_item_id: str,
+        value: CacheItemValueContraT,
+        *,
+        modified: int | float | None = None,
+    ) -> None:
         raise NotImplementedError
 
     @overload
-    def getset(self, cache_item_id: str) -> AsyncContextManager[tuple[CacheItem[CacheItemValueContraT] | None, CacheItemValueSetter[CacheItemValueContraT]]]:
+    def getset(self, cache_item_id: str) -> AsyncContextManager[
+        tuple[
+            CacheItem[CacheItemValueContraT] | None,
+            CacheItemValueSetter[CacheItemValueContraT],
+        ]
+    ]:
         pass
 
     @overload
-    def getset(self, cache_item_id: str, *, wait: Literal[False] = False) -> AsyncContextManager[tuple[CacheItem[CacheItemValueContraT] | None, CacheItemValueSetter[CacheItemValueContraT] | None]]:
+    def getset(
+        self, cache_item_id: str, *, wait: Literal[False] = False
+    ) -> AsyncContextManager[
+        tuple[
+            CacheItem[CacheItemValueContraT] | None,
+            CacheItemValueSetter[CacheItemValueContraT] | None,
+        ]
+    ]:
         pass
 
     @asynccontextmanager  # type: ignore[misc]
-    async def getset(self, cache_item_id: str, *, wait: bool = True) -> AsyncIterator[tuple[CacheItem[CacheItemValueContraT] | None, CacheItemValueSetter[CacheItemValueContraT] | None]]:
+    async def getset(self, cache_item_id: str, *, wait: bool = True) -> AsyncIterator[
+        tuple[
+            CacheItem[CacheItemValueContraT] | None,
+            CacheItemValueSetter[CacheItemValueContraT] | None,
+        ]
+    ]:
         lock = await self._lock(cache_item_id)
         if await lock.acquire(wait=wait):
             try:
+
                 async def _setter(value: CacheItemValueContraT) -> None:
                     await self._set(cache_item_id, value)
+
                 yield await self._get(cache_item_id), _setter
                 return
             finally:
                 lock.release()
         yield None, None
 
     async def delete(self, cache_item_id: str) -> None:
@@ -100,13 +141,17 @@
         raise NotImplementedError
 
     async def clear(self) -> None:
         async with MultiLock(self._locks_lock, *self._locks.values()):
             await self._clear()
         logger = logging.getLogger(__name__)
         if self._scopes:
-            logger.info(self._localizer._('"{scope}" cache cleared.').format(scope='.'.join(self._scopes)))
+            logger.info(
+                self._localizer._('"{scope}" cache cleared.').format(
+                    scope=".".join(self._scopes)
+                )
+            )
         else:
-            logger.info(self._localizer._('All caches cleared.'))
+            logger.info(self._localizer._("All caches cleared."))
 
     async def _clear(self) -> None:
         raise NotImplementedError
```

### Comparing `betty-0.3.3/betty/cache/file.py` & `betty-0.3.4/betty/cache/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 """
 Provide caching that persists cache items to files.
 """
+
 from __future__ import annotations
 
 import asyncio
 import shutil
-from base64 import b64encode
 from collections.abc import Sequence
 from contextlib import suppress
 from os import utime
 from pathlib import Path
 from pickle import dumps, loads
 from typing import Generic, Self
 
 import aiofiles
 from aiofiles.ospath import getmtime
 
 from betty.cache import CacheItem, CacheItemValueContraT, CacheItemValueCoT
 from betty.cache._base import _CommonCacheBase
+from betty.hashid import hashid
 from betty.locale import Localizer
 
 
 class _FileCacheItem(CacheItem[CacheItemValueCoT], Generic[CacheItemValueCoT]):
-    __slots__ = '_modified', '_path'
+    __slots__ = "_modified", "_path"
 
     def __init__(
         self,
         modified: int | float,
         path: Path,
     ):
         self._modified = modified
         self._path = path
 
     @property
     def modified(self) -> int | float:
         return self._modified
 
     async def value(self) -> CacheItemValueCoT:
-        async with aiofiles.open(self._path, 'rb') as f:
+        async with aiofiles.open(self._path, "rb") as f:
             value_bytes = await f.read()
         return await self._load_value(value_bytes)
 
     async def _load_value(self, value_bytes: bytes) -> CacheItemValueCoT:
         raise NotImplementedError
 
 
-class _PickledFileCacheItem(_FileCacheItem[CacheItemValueCoT], Generic[CacheItemValueCoT]):
+class _PickledFileCacheItem(
+    _FileCacheItem[CacheItemValueCoT], Generic[CacheItemValueCoT]
+):
     async def _load_value(self, value_bytes: bytes) -> CacheItemValueCoT:
         return loads(value_bytes)  # type: ignore[no-any-return]
 
 
 class _BinaryFileCacheItem(_FileCacheItem[bytes]):
     async def _load_value(self, value_bytes: bytes) -> bytes:
         return value_bytes
 
 
-class _FileCache(_CommonCacheBase[CacheItemValueContraT], Generic[CacheItemValueContraT]):
+class _FileCache(
+    _CommonCacheBase[CacheItemValueContraT], Generic[CacheItemValueContraT]
+):
     """
     Provide a cache that persists cache items on a file system.
     """
 
     _cache_item_cls: type[_FileCacheItem[CacheItemValueContraT]]
 
     def __init__(
@@ -69,43 +74,56 @@
         *,
         scopes: Sequence[str] | None = None,
     ):
         super().__init__(localizer, scopes=scopes)
         self._root_path = cache_directory_path
 
     def _with_scope(self, scope: str) -> Self:
-        return type(self)(self._localizer, self._root_path, scopes=(*self._scopes, scope))
+        return type(self)(
+            self._localizer, self._root_path, scopes=(*self._scopes, scope)
+        )
 
     def _cache_item_file_path(self, cache_item_id: str) -> Path:
-        return self._path / b64encode(cache_item_id.encode('utf-8')).decode('utf-8')
+        return self._path / hashid(cache_item_id)
 
     def _dump_value(self, value: CacheItemValueContraT) -> bytes:
         raise NotImplementedError
 
     async def _get(self, cache_item_id: str) -> CacheItem[CacheItemValueContraT] | None:
         try:
             cache_item_file_path = self._cache_item_file_path(cache_item_id)
             return self._cache_item_cls(
                 await getmtime(cache_item_file_path),
                 cache_item_file_path,
             )
         except OSError:
             return None
 
-    async def _set(self, cache_item_id: str, value: CacheItemValueContraT, *, modified: int | float | None = None) -> None:
+    async def _set(
+        self,
+        cache_item_id: str,
+        value: CacheItemValueContraT,
+        *,
+        modified: int | float | None = None,
+    ) -> None:
         value = self._dump_value(value)
         cache_item_file_path = self._cache_item_file_path(cache_item_id)
         try:
             await self._write(cache_item_file_path, value, modified)
         except FileNotFoundError:
             await aiofiles.os.makedirs(cache_item_file_path.parent, exist_ok=True)
             await self._write(cache_item_file_path, value, modified)
 
-    async def _write(self, cache_item_file_path: Path, value: bytes, modified: int | float | None = None) -> None:
-        async with aiofiles.open(cache_item_file_path, 'wb') as f:
+    async def _write(
+        self,
+        cache_item_file_path: Path,
+        value: bytes,
+        modified: int | float | None = None,
+    ) -> None:
+        async with aiofiles.open(cache_item_file_path, "wb") as f:
             await f.write(value)
         if modified is not None:
             await asyncio.to_thread(utime, cache_item_file_path, (modified, modified))
 
     async def _delete(self, cache_item_id: str) -> None:
         with suppress(FileNotFoundError):
             await aiofiles.os.remove(self._cache_item_file_path(cache_item_id))
@@ -115,15 +133,17 @@
             await asyncio.to_thread(shutil.rmtree, self._path)
 
     @property
     def _path(self) -> Path:
         return self._root_path.joinpath(*self._scopes)
 
 
-class PickledFileCache(_FileCache[CacheItemValueContraT], Generic[CacheItemValueContraT]):
+class PickledFileCache(
+    _FileCache[CacheItemValueContraT], Generic[CacheItemValueContraT]
+):
     """
     Provide a cache that pickles values and persists them to files.
     """
 
     _cache_item_cls = _PickledFileCacheItem
 
     def _dump_value(self, value: CacheItemValueContraT) -> bytes:
```

### Comparing `betty-0.3.3/betty/cache/memory.py` & `betty-0.3.4/betty/cache/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """
 Provide caching that stores cache items in volatile memory.
 """
+
 from __future__ import annotations
 
 from collections.abc import MutableMapping, Sequence
 from typing import TypeAlias, Generic, Self, cast
 
 from betty.cache import CacheItem, CacheItemValueContraT
 from betty.cache._base import _CommonCacheBase, _StaticCacheItem
 from betty.locale import Localizer
 
-_MemoryCacheStore: TypeAlias = MutableMapping[str, 'CacheItem[CacheItemValueContraT] | None | _MemoryCacheStore[CacheItemValueContraT]']
+_MemoryCacheStore: TypeAlias = MutableMapping[
+    str,
+    "CacheItem[CacheItemValueContraT] | None | _MemoryCacheStore[CacheItemValueContraT]",
+]
 
 
-class MemoryCache(_CommonCacheBase[CacheItemValueContraT], Generic[CacheItemValueContraT]):
+class MemoryCache(
+    _CommonCacheBase[CacheItemValueContraT], Generic[CacheItemValueContraT]
+):
     """
     Provide a cache that stores cache items in volatile memory.
     """
 
     def __init__(
         self,
         localizer: Localizer,
@@ -28,24 +34,33 @@
         super().__init__(localizer, scopes=scopes)
         self._store: _MemoryCacheStore[CacheItemValueContraT] = _store or {}
 
     def _with_scope(self, scope: str) -> Self:
         return type(self)(
             self._localizer,
             scopes=(*self._scopes, scope),
-            _store=cast('_MemoryCacheStore[CacheItemValueContraT]', self._store.setdefault(scope, {})),
+            _store=cast(
+                "_MemoryCacheStore[CacheItemValueContraT]",
+                self._store.setdefault(scope, {}),
+            ),
         )
 
     async def _get(self, cache_item_id: str) -> CacheItem[CacheItemValueContraT] | None:
         cache_item = self._store.get(cache_item_id, None)
         if isinstance(cache_item, CacheItem):
             return cache_item
         return None
 
-    async def _set(self, cache_item_id: str, value: CacheItemValueContraT, *, modified: int | float | None = None) -> None:
+    async def _set(
+        self,
+        cache_item_id: str,
+        value: CacheItemValueContraT,
+        *,
+        modified: int | float | None = None,
+    ) -> None:
         self._store[cache_item_id] = _StaticCacheItem(value, modified)
 
     async def _delete(self, cache_item_id: str) -> None:
         self._store.pop(cache_item_id, None)
 
     async def _clear(self) -> None:
         self._store.clear()
```

### Comparing `betty-0.3.3/betty/cli.py` & `betty-0.3.4/betty/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide the Command Line Interface.
 """
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import sys
 from contextlib import suppress, contextmanager
 from functools import wraps
@@ -25,16 +26,16 @@
 from betty.gui.app import WelcomeWindow
 from betty.gui.project import ProjectWindow
 from betty.locale import update_translations, init_translation, Str
 from betty.logging import CliHandler
 from betty.serde.load import AssertionFailed
 from betty.serve import AppServer
 
-T = TypeVar('T')
-P = ParamSpec('P')
+T = TypeVar("T")
+P = ParamSpec("P")
 
 
 class CommandProvider:
     @property
     def commands(self) -> dict[str, Command]:
         raise NotImplementedError(repr(self))
 
@@ -43,17 +44,17 @@
 def catch_exceptions() -> Iterator[None]:
     """
     Catch and log all exceptions.
     """
     try:
         yield
     except KeyboardInterrupt:
-        print('Quitting...')
+        print("Quitting...")
         sys.exit(0)
-    except BaseException as e:
+    except BaseException as e:  # noqa: B036
         logger = logging.getLogger(__name__)
         if isinstance(e, UserFacingError):
             logger.error(str(e))
         else:
             logger.exception(e)
         sys.exit(1)
 
@@ -64,21 +65,23 @@
 ) -> Callable[P, None]:
     @wraps(f)
     @catch_exceptions()
     def _command(*args: P.args, **kwargs: P.kwargs) -> None:
         if is_app_command:
             # We must get the current Click context from the main thread.
             # Once that is done, we can wait for the async commands to complete, which MAY be done in a thread.
-            app = get_current_context().obj['app']
+            app = get_current_context().obj["app"]
 
             async def _app_command():
                 async with app:
                     await f(app, *args, **kwargs)
+
             return wait_to_thread(_app_command())
         return wait_to_thread(f(*args, **kwargs))
+
     return _command
 
 
 def global_command(f: Callable[P, Awaitable[None]]) -> Callable[P, None]:
     """
     Decorate a command to be global.
     """
@@ -103,177 +106,188 @@
 
 async def __init_ctx_app(
     ctx: Context,
     configuration_file_path: str | None = None,
 ) -> None:
     ctx.ensure_object(dict)
 
-    if 'initialized' in ctx.obj:
+    if "initialized" in ctx.obj:
         return
-    ctx.obj['initialized'] = True
+    ctx.obj["initialized"] = True
 
     logging.getLogger().addHandler(CliHandler())
     logger = logging.getLogger(__name__)
 
     app = ctx.with_resource(  # type: ignore[attr-defined]
         SynchronizedContextManager(App.new_from_environment())
     )
-    ctx.obj['commands'] = {
-        'docs': _docs,
-        'clear-caches': _clear_caches,
-        'demo': _demo,
-        'gui': _gui,
+    ctx.obj["commands"] = {
+        "docs": _docs,
+        "clear-caches": _clear_caches,
+        "demo": _demo,
+        "gui": _gui,
     }
     if wait_to_thread(about.is_development()):
-        ctx.obj['commands']['init-translation'] = _init_translation
-        ctx.obj['commands']['update-translations'] = _update_translations
-    ctx.obj['app'] = app
+        ctx.obj["commands"]["init-translation"] = _init_translation
+        ctx.obj["commands"]["update-translations"] = _update_translations
+    ctx.obj["app"] = app
 
     if configuration_file_path is None:
         try_configuration_file_paths = [
-            Path.cwd() / f'betty{extension}'
-            for extension
-            in {'.json', '.yaml', '.yml'}
+            Path.cwd() / f"betty{extension}" for extension in {".json", ".yaml", ".yml"}
         ]
     else:
         try_configuration_file_paths = [Path.cwd() / configuration_file_path]
 
     async with app:
         for try_configuration_file_path in try_configuration_file_paths:
             try:
                 await app.project.configuration.read(try_configuration_file_path)
             except FileNotFoundError:
                 continue
             else:
-                ctx.obj['commands']['generate'] = _generate
-                ctx.obj['commands']['serve'] = _serve
+                ctx.obj["commands"]["generate"] = _generate
+                ctx.obj["commands"]["serve"] = _serve
                 for extension in app.extensions.flatten():
                     if isinstance(extension, CommandProvider):
                         for command_name, command in extension.commands.items():
-                            ctx.obj['commands'][command_name] = command
-                logger.info(app.localizer._('Loaded the configuration from {configuration_file_path}.').format(
-                    configuration_file_path=str(try_configuration_file_path)),
+                            ctx.obj["commands"][command_name] = command
+                logger.info(
+                    app.localizer._(
+                        "Loaded the configuration from {configuration_file_path}."
+                    ).format(configuration_file_path=str(try_configuration_file_path)),
                 )
                 return
 
         if configuration_file_path is not None:
-            raise AssertionFailed(Str._(
-                'Configuration file "{configuration_file_path}" does not exist.',
-                configuration_file_path=configuration_file_path,
-            ))
+            raise AssertionFailed(
+                Str._(
+                    'Configuration file "{configuration_file_path}" does not exist.',
+                    configuration_file_path=configuration_file_path,
+                )
+            )
 
 
 def _build_init_ctx_verbosity(
     betty_logger_level: int,
     root_logger_level: int | None = None,
 ) -> Callable[[Context, Option | Parameter | None, bool], None]:
     def _init_ctx_verbosity(
         ctx: Context,
         __: Option | Parameter | None = None,
         is_verbose: bool = False,
     ) -> None:
         if is_verbose:
-            for logger_name, logger_level in (('betty', betty_logger_level), (None, root_logger_level)):
+            for logger_name, logger_level in (
+                ("betty", betty_logger_level),
+                (None, root_logger_level),
+            ):
                 logger = logging.getLogger(logger_name)
-                if logger_level is not None and logger.getEffectiveLevel() > logger_level:
+                if (
+                    logger_level is not None
+                    and logger.getEffectiveLevel() > logger_level
+                ):
                     logger.setLevel(logger_level)
+
     return _init_ctx_verbosity
 
 
 class _BettyCommands(click.MultiCommand):
     @catch_exceptions()
     def list_commands(self, ctx: Context) -> list[str]:
         _init_ctx_app(ctx)
-        return list(ctx.obj['commands'].keys())
+        return list(ctx.obj["commands"].keys())
 
     @catch_exceptions()
     def get_command(self, ctx: Context, cmd_name: str) -> Command | None:
         _init_ctx_app(ctx)
         with suppress(KeyError):
-            return cast(Command, ctx.obj['commands'][cmd_name])
+            return cast(Command, ctx.obj["commands"][cmd_name])
         return None
 
 
 @click.command(
     cls=_BettyCommands,
     # Set an empty help text so Click does not automatically use the function's docstring.
-    help='',
+    help="",
 )
 @click.option(
-    '--configuration',
-    '-c',
-    'app',
+    "--configuration",
+    "-c",
+    "app",
     is_eager=True,
-    help='The path to a Betty project configuration file. Defaults to betty.json|yaml|yml in the current working directory. This will make additional commands available.',
+    help="The path to a Betty project configuration file. Defaults to betty.json|yaml|yml in the current working directory. This will make additional commands available.",
     callback=_init_ctx_app,
 )
 @click.option(
-    '-v',
-    '--verbose',
+    "-v",
+    "--verbose",
     is_eager=True,
     default=False,
     is_flag=True,
-    help='Show verbose output, including informative log messages.',
+    help="Show verbose output, including informative log messages.",
     callback=_build_init_ctx_verbosity(logging.INFO),
 )
 @click.option(
-    '-vv',
-    '--more-verbose',
-    'more_verbose',
+    "-vv",
+    "--more-verbose",
+    "more_verbose",
     is_eager=True,
     default=False,
     is_flag=True,
-    help='Show more verbose output, including debug log messages.',
+    help="Show more verbose output, including debug log messages.",
     callback=_build_init_ctx_verbosity(logging.DEBUG),
 )
 @click.option(
-    '-vvv',
-    '--most-verbose',
-    'most_verbose',
+    "-vvv",
+    "--most-verbose",
+    "most_verbose",
     is_eager=True,
     default=False,
     is_flag=True,
-    help='Show most verbose output, including all log messages.',
+    help="Show most verbose output, including all log messages.",
     callback=_build_init_ctx_verbosity(logging.NOTSET, logging.NOTSET),
 )
 @click.version_option(
     wait_to_thread(about.version_label()),
     message=wait_to_thread(about.report()),
-    prog_name='Betty',
+    prog_name="Betty",
 )
 def main(app: App, verbose: bool, more_verbose: bool, most_verbose: bool) -> None:
     """
     Launch Betty's Command-Line Interface.
     """
     pass
 
 
-@click.command(help='Clear all caches.')
+@click.command(help="Clear all caches.")
 @app_command
 async def _clear_caches(app: App) -> None:
     await app.cache.clear()
 
 
-@click.command(help='Explore a demonstration site.')
+@click.command(help="Explore a demonstration site.")
 @app_command
 async def _demo(app: App) -> None:
     async with demo.DemoServer(app=app) as server:
         await server.show()
         while True:
             await asyncio.sleep(999)
 
 
 @click.command(help="Open Betty's graphical user interface (GUI).")
 @click.option(
-    '--configuration',
-    '-c',
-    'configuration_file_path',
+    "--configuration",
+    "-c",
+    "configuration_file_path",
     is_eager=True,
-    help='The path to a Betty project configuration file. Defaults to betty.json|yaml|yml in the current working directory.',
-    callback=lambda _, __, configuration_file_path: Path(configuration_file_path) if configuration_file_path else None,
+    help="The path to a Betty project configuration file. Defaults to betty.json|yaml|yml in the current working directory.",
+    callback=lambda _, __, configuration_file_path: (
+        Path(configuration_file_path) if configuration_file_path else None
+    ),
 )
 @global_command
 async def _gui(configuration_file_path: Path | None) -> None:
     async with App.new_from_environment() as app:
         async with BettyApplication([sys.argv[0]]).with_app(app) as qapp:
             window: QMainWindow
             if configuration_file_path is None:
@@ -281,31 +295,31 @@
             else:
                 await app.project.configuration.read(configuration_file_path)
                 window = ProjectWindow(app)
             window.show()
             sys.exit(qapp.exec())
 
 
-@click.command(help='Generate a static site.')
+@click.command(help="Generate a static site.")
 @app_command
 async def _generate(app: App) -> None:
     await load.load(app)
     await generate.generate(app)
 
 
-@click.command(help='Serve a generated site.')
+@click.command(help="Serve a generated site.")
 @app_command
 async def _serve(app: App) -> None:
     async with AppServer.get(app) as server:
         await server.show()
         while True:
             await asyncio.sleep(999)
 
 
-@click.command(help='View the documentation.')
+@click.command(help="View the documentation.")
 @global_command
 async def _docs():
     async with App.new_from_environment() as app:
         async with app:
             server = documentation.DocumentationServer(
                 app.binary_file_cache.path,
                 localizer=app.localizer,
@@ -313,17 +327,24 @@
             async with server:
                 await server.show()
                 while True:
                     await asyncio.sleep(999)
 
 
 if wait_to_thread(about.is_development()):
-    @click.command(short_help='Initialize a new translation', help='Initialize a new translation.\n\nThis is available only when developing Betty.')
-    @click.argument('locale')
+
+    @click.command(
+        short_help="Initialize a new translation",
+        help="Initialize a new translation.\n\nThis is available only when developing Betty.",
+    )
+    @click.argument("locale")
     @global_command
     async def _init_translation(locale: str) -> None:
         await init_translation(locale)
 
-    @click.command(short_help='Update all existing translations', help='Update all existing translations.\n\nThis is available only when developing Betty.')
+    @click.command(
+        short_help="Update all existing translations",
+        help="Update all existing translations.\n\nThis is available only when developing Betty.",
+    )
     @global_command
     async def _update_translations() -> None:
         await update_translations()
```

### Comparing `betty-0.3.3/betty/concurrent.py` & `betty-0.3.4/betty/concurrent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide utilities for concurrent programming.
 """
+
 import asyncio
 import threading
 import time
 from asyncio import sleep
 from math import floor
 from threading import Lock
 from types import TracebackType
@@ -17,15 +18,20 @@
     """
     Provide an asynchronous lock.
     """
 
     async def __aenter__(self):
         await self.acquire()
 
-    async def __aexit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
         self.release()
 
     async def acquire(self, *, wait: bool = True) -> bool:
         raise NotImplementedError
 
     def release(self) -> None:
         raise NotImplementedError
@@ -46,15 +52,15 @@
 
 
 class AsynchronizedLock(_Lock):
     """
     Make a sychronous (blocking) lock asynchronous (non-blocking).
     """
 
-    __slots__ = '_lock'
+    __slots__ = "_lock"
 
     def __init__(self, lock: Lock):
         self._lock = lock
 
     async def acquire(self, *, wait: bool = True) -> bool:
         return await asynchronize_acquire(self._lock, wait=wait)
 
@@ -67,15 +73,15 @@
 
 
 class MultiLock(_Lock):
     """
     Provide a lock that only acquires if all of the given locks can be acquired.
     """
 
-    __slots__ = '_locked', '_locks'
+    __slots__ = "_locked", "_locks"
 
     def __init__(self, *locks: _Lock):
         self._locks = locks
         self._locked = False
 
     async def acquire(self, *, wait: bool = True) -> bool:
         acquisitions = await gather(*(lock.acquire(wait=wait) for lock in self._locks))
@@ -125,15 +131,20 @@
         if possibly_available > 0:
             self._available = min(possibly_available, self._maximum)
             self._last_add = now
 
     async def __aenter__(self) -> None:
         await self.wait()
 
-    async def __aexit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
         return
 
     async def wait(self) -> None:
         async with self._lock:
             while self._available < 1:
                 self._add_tokens()
                 if self._available < 1:
```

### Comparing `betty-0.3.3/betty/config.py` & `betty-0.3.4/betty/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,76 @@
 """
 Provide the Configuration API.
 """
+
 from __future__ import annotations
 
 import inspect
 import weakref
 from _weakref import ReferenceType
 from collections import OrderedDict
 from collections.abc import Callable
 from contextlib import suppress, chdir
 from pathlib import Path
 from reprlib import recursive_repr
 from tempfile import TemporaryDirectory
-from typing import Generic, Iterable, Iterator, SupportsIndex, Hashable, \
-    MutableSequence, MutableMapping, TypeVar, Any, Sequence, overload, cast, Self, TypeAlias
+from typing import (
+    Generic,
+    Iterable,
+    Iterator,
+    SupportsIndex,
+    Hashable,
+    MutableSequence,
+    MutableMapping,
+    TypeVar,
+    Any,
+    Sequence,
+    overload,
+    cast,
+    Self,
+    TypeAlias,
+)
 
 import aiofiles
 from aiofiles.os import makedirs
 
 from betty.asyncio import wait_to_thread
 from betty.classtools import repr_instance
 from betty.functools import slice_to_range
 from betty.locale import Str
 from betty.serde.dump import Dumpable, Dump, minimize, VoidableDump, Void
 from betty.serde.error import SerdeErrorCollection
 from betty.serde.format import FormatRepository
 from betty.serde.load import Asserter, Assertion, Assertions
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 _ConfigurationListener: TypeAlias = Callable[[], None]
-ConfigurationListener: TypeAlias = 'Configuration | _ConfigurationListener'
+ConfigurationListener: TypeAlias = "Configuration | _ConfigurationListener"
 
 
 class Configuration(Dumpable):
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self._asserter = Asserter()
-        self._on_change_listeners: MutableSequence[ReferenceType[_ConfigurationListener]] = []
+        self._on_change_listeners: MutableSequence[
+            ReferenceType[_ConfigurationListener]
+        ] = []
 
     def _dispatch_change(self) -> None:
         for listener_reference in self._on_change_listeners:
             listener = listener_reference()
             if listener is None:
                 continue
             listener()
 
-    def _prepare_listener(self, listener: ConfigurationListener) -> ReferenceType[_ConfigurationListener]:
+    def _prepare_listener(
+        self, listener: ConfigurationListener
+    ) -> ReferenceType[_ConfigurationListener]:
         if isinstance(listener, Configuration):
             listener = listener._dispatch_change
         if inspect.ismethod(listener):  # type: ignore[redundant-expr]
             return weakref.WeakMethod(listener)
         return weakref.ref(listener)
 
     def on_change(self, listener: ConfigurationListener) -> None:
@@ -71,22 +90,27 @@
     ) -> Self:
         """
         Load dumped configuration into a new configuration instance.
         """
         raise NotImplementedError(repr(cls))
 
     @classmethod
-    def assert_load(cls: type[ConfigurationT], configuration: ConfigurationT | None = None) -> Assertion[Dump, ConfigurationT]:
+    def assert_load(
+        cls: type[ConfigurationT], configuration: ConfigurationT | None = None
+    ) -> Assertion[Dump, ConfigurationT]:
         def _assert_load(dump: Dump) -> ConfigurationT:
             return cls.load(dump, configuration)
-        _assert_load.__qualname__ = f'{_assert_load.__qualname__} for {cls.__module__}.{cls.__qualname__}.load'
+
+        _assert_load.__qualname__ = (
+            f"{_assert_load.__qualname__} for {cls.__module__}.{cls.__qualname__}.load"
+        )
         return _assert_load
 
 
-ConfigurationT = TypeVar('ConfigurationT', bound=Configuration)
+ConfigurationT = TypeVar("ConfigurationT", bound=Configuration)
 
 
 class FileBasedConfiguration(Configuration):
     def __init__(self):
         super().__init__()
         self._configuration_directory: TemporaryDirectory | None = None  # type: ignore[type-arg]
         self._configuration_file_path: Path | None = None
@@ -116,15 +140,15 @@
 
     async def _write(self, configuration_file_path: Path) -> None:
         # Change the working directory to allow absolute paths to be turned relative to the configuration file's directory
         # path.
         formats = FormatRepository()
         dump = formats.format_for(configuration_file_path.suffix[1:]).dump(self.dump())
         try:
-            async with aiofiles.open(configuration_file_path, mode='w') as f:
+            async with aiofiles.open(configuration_file_path, mode="w") as f:
                 await f.write(dump)
         except FileNotFoundError:
             await makedirs(configuration_file_path.parent)
             await self.write()
         self._configuration_file_path = configuration_file_path
 
     async def read(self, configuration_file_path: Path | None = None) -> None:
@@ -134,57 +158,78 @@
         formats = FormatRepository()
         with SerdeErrorCollection().assert_valid() as errors:
             # Change the working directory to allow relative paths to be resolved against the configuration file's directory
             # path.
             with chdir(self.configuration_file_path.parent):
                 async with aiofiles.open(self.configuration_file_path) as f:
                     read_configuration = await f.read()
-                with errors.catch(Str.plain(
-                    'in {configuration_file_path}',
-                    configuration_file_path=str(self.configuration_file_path.resolve()),
-                )):
+                with errors.catch(
+                    Str.plain(
+                        "in {configuration_file_path}",
+                        configuration_file_path=str(
+                            self.configuration_file_path.resolve()
+                        ),
+                    )
+                ):
                     loaded_configuration = self.load(
-                        formats.format_for(self.configuration_file_path.suffix[1:]).load(read_configuration),
+                        formats.format_for(
+                            self.configuration_file_path.suffix[1:]
+                        ).load(read_configuration),
                         self,
                     )
         self.update(loaded_configuration)
 
     def __del__(self) -> None:
-        if hasattr(self, '_configuration_directory') and self._configuration_directory is not None:
+        if (
+            hasattr(self, "_configuration_directory")
+            and self._configuration_directory is not None
+        ):
             self._configuration_directory.cleanup()
 
     @property
     def configuration_file_path(self) -> Path:
         if self._configuration_file_path is None:
             if self._configuration_directory is None:
                 self._configuration_directory = TemporaryDirectory()
-            wait_to_thread(self._write(Path(self._configuration_directory.name) / f'{type(self).__name__}.json'))
+            wait_to_thread(
+                self._write(
+                    Path(self._configuration_directory.name)
+                    / f"{type(self).__name__}.json"
+                )
+            )
         return cast(Path, self._configuration_file_path)
 
     @configuration_file_path.setter
     def configuration_file_path(self, configuration_file_path: Path) -> None:
         if configuration_file_path == self._configuration_file_path:
             return
         formats = FormatRepository()
         formats.format_for(configuration_file_path.suffix[1:])
         self._configuration_file_path = configuration_file_path
 
     @configuration_file_path.deleter
     def configuration_file_path(self) -> None:
         if self._autowrite:
-            raise RuntimeError('Cannot remove the configuration file path while autowrite is enabled.')
+            raise RuntimeError(
+                "Cannot remove the configuration file path while autowrite is enabled."
+            )
         self._configuration_file_path = None
 
 
 ConfigurationKey: TypeAlias = SupportsIndex | Hashable | type[Any]
-ConfigurationKeyT = TypeVar('ConfigurationKeyT', bound=ConfigurationKey)
+ConfigurationKeyT = TypeVar("ConfigurationKeyT", bound=ConfigurationKey)
 
 
-class ConfigurationCollection(Configuration, Generic[ConfigurationKeyT, ConfigurationT]):
-    _configurations: MutableSequence[ConfigurationT] | MutableMapping[ConfigurationKeyT, ConfigurationT]
+class ConfigurationCollection(
+    Configuration, Generic[ConfigurationKeyT, ConfigurationT]
+):
+    _configurations: (
+        MutableSequence[ConfigurationT]
+        | MutableMapping[ConfigurationKeyT, ConfigurationT]
+    )
 
     def __init__(
         self,
         configurations: Iterable[ConfigurationT] | None = None,
     ):
         super().__init__()
         if configurations is not None:
@@ -263,15 +308,17 @@
             yield self.to_key(index)
 
     @classmethod
     def _item_type(cls) -> type[ConfigurationT]:
         raise NotImplementedError(repr(cls))
 
     @classmethod
-    def _create_default_item(cls, configuration_key: ConfigurationKeyT) -> ConfigurationT:
+    def _create_default_item(
+        cls, configuration_key: ConfigurationKeyT
+    ) -> ConfigurationT:
         raise NotImplementedError(repr(cls))
 
     def keys(self) -> Iterator[ConfigurationKeyT]:
         raise NotImplementedError(repr(self))
 
     def values(self) -> Iterator[ConfigurationT]:
         raise NotImplementedError(repr(self))
@@ -294,15 +341,17 @@
     def move_to_end(self, *configuration_keys: ConfigurationKeyT) -> None:
         raise NotImplementedError(repr(self))
 
     def move_towards_end(self, *configuration_keys: ConfigurationKeyT) -> None:
         raise NotImplementedError(repr(self))
 
 
-class ConfigurationSequence(ConfigurationCollection[int, ConfigurationT], Generic[ConfigurationT]):
+class ConfigurationSequence(
+    ConfigurationCollection[int, ConfigurationT], Generic[ConfigurationT]
+):
     def __init__(
         self,
         configurations: Iterable[ConfigurationT] | None = None,
     ):
         self._configurations: MutableSequence[ConfigurationT] = []
         super().__init__(configurations)
 
@@ -316,15 +365,17 @@
     def __getitem__(self, configuration_key: int) -> ConfigurationT:
         pass
 
     @overload
     def __getitem__(self, configuration_key: slice) -> Sequence[ConfigurationT]:
         pass
 
-    def __getitem__(self, configuration_key: int | slice) -> ConfigurationT | Sequence[ConfigurationT]:
+    def __getitem__(
+        self, configuration_key: int | slice
+    ) -> ConfigurationT | Sequence[ConfigurationT]:
         return self._configurations[configuration_key]
 
     def __iter__(self) -> Iterator[ConfigurationT]:
         return (configuration for configuration in self._configurations)
 
     def keys(self) -> Iterator[int]:
         return iter(range(0, len(self._configurations)))
@@ -333,32 +384,35 @@
         yield from self._configurations
 
     def update(self, other: Self) -> None:
         raise NotImplementedError(repr(self))
 
     @classmethod
     def load(
-            cls,
-            dump: Dump,
-            configuration: Self | None = None,
+        cls,
+        dump: Dump,
+        configuration: Self | None = None,
     ) -> Self:
         if configuration is None:
             configuration = cls()
         else:
             configuration._clear_without_dispatch()
         asserter = Asserter()
         with SerdeErrorCollection().assert_valid():
-            configuration.append(*asserter.assert_sequence(Assertions(cls._item_type().assert_load()))(dump))
+            configuration.append(
+                *asserter.assert_sequence(Assertions(cls._item_type().assert_load()))(
+                    dump
+                )
+            )
         return configuration
 
     def dump(self) -> VoidableDump:
-        return minimize([
-            configuration.dump()
-            for configuration in self._configurations
-        ])
+        return minimize(
+            [configuration.dump() for configuration in self._configurations]
+        )
 
     def prepend(self, *configurations: ConfigurationT) -> None:
         for configuration in configurations:
             self._on_add(configuration)
             self._configurations.insert(0, configuration)
         self._dispatch_change()
 
@@ -375,18 +429,17 @@
         self._dispatch_change()
 
     def move_to_beginning(self, *configuration_keys: int) -> None:
         self.move_to_end(
             *configuration_keys,
             *[
                 index
-                for index
-                in range(0, len(self._configurations))
+                for index in range(0, len(self._configurations))
                 if index not in configuration_keys
-            ]
+            ],
         )
 
     def move_towards_beginning(self, *configuration_keys: int) -> None:
         for index in configuration_keys:
             self._configurations.insert(index - 1, self._configurations.pop(index))
         self._dispatch_change()
 
@@ -399,20 +452,25 @@
 
     def move_towards_end(self, *configuration_keys: int) -> None:
         for index in reversed(configuration_keys):
             self._configurations.insert(index + 1, self._configurations.pop(index))
         self._dispatch_change()
 
 
-class ConfigurationMapping(ConfigurationCollection[ConfigurationKeyT, ConfigurationT], Generic[ConfigurationKeyT, ConfigurationT]):
+class ConfigurationMapping(
+    ConfigurationCollection[ConfigurationKeyT, ConfigurationT],
+    Generic[ConfigurationKeyT, ConfigurationT],
+):
     def __init__(
         self,
         configurations: Iterable[ConfigurationT] | None = None,
     ):
-        self._configurations: OrderedDict[ConfigurationKeyT, ConfigurationT] = OrderedDict()
+        self._configurations: OrderedDict[ConfigurationKeyT, ConfigurationT] = (
+            OrderedDict()
+        )
         super().__init__(configurations)
 
     def _minimize_item_dump(self) -> bool:
         return False
 
     def to_index(self, configuration_key: ConfigurationKeyT) -> int:
         return list(self._configurations.keys()).index(configuration_key)
@@ -440,60 +498,49 @@
         yield from self._configurations.values()
 
     def update(self, other: Self) -> None:
         self.replace(*other.values())
 
     def replace(self, *values: ConfigurationT) -> None:
         self_keys = list(self.keys())
-        other = {
-            self._get_key(value): value
-            for value in values
-        }
+        other = {self._get_key(value): value for value in values}
         other_values = list(values)
         other_keys = list(map(self._get_key, other_values))
 
         # Update items that are kept.
         for key in self_keys:
             if key in other_keys:
                 self[key].update(other[key])
 
         # Add items that are new.
-        self._append_without_trigger(*(
-            other[key]
-            for key
-            in other_keys
-            if key not in self_keys
-        ))
+        self._append_without_trigger(
+            *(other[key] for key in other_keys if key not in self_keys)
+        )
 
         # Remove items that should no longer be present.
-        self._remove_without_dispatch(*(
-            key
-            for key
-            in self_keys
-            if key not in other_keys
-        ))
+        self._remove_without_dispatch(
+            *(key for key in self_keys if key not in other_keys)
+        )
 
         # Ensure everything is in the correct order. This will also trigger reactors.
         self.move_to_beginning(*other_keys)
 
     @classmethod
     def load(
-            cls,
-            dump: Dump,
-            configuration: Self | None = None,
+        cls,
+        dump: Dump,
+        configuration: Self | None = None,
     ) -> Self:
         if configuration is None:
             configuration = cls()
         asserter = Asserter()
         dict_dump = asserter.assert_dict()(dump)
-        mapping = asserter.assert_mapping(Assertions(cls._item_type().load))({
-            key: cls._load_key(value, key)
-            for key, value
-            in dict_dump.items()
-        })
+        mapping = asserter.assert_mapping(Assertions(cls._item_type().load))(
+            {key: cls._load_key(value, key) for key, value in dict_dump.items()}
+        )
         configuration.replace(*mapping.values())
         return configuration
 
     def dump(self) -> VoidableDump:
         dump = {}
         for configuration_item in self._configurations.values():
             item_dump = configuration_item.dump()
@@ -518,53 +565,62 @@
             configuration.on_change(self)
         self._move_to_end_without_trigger(*map(self._get_key, configurations))
 
     def append(self, *configurations: ConfigurationT) -> None:
         self._append_without_trigger(*configurations)
         self._dispatch_change()
 
-    def _insert_without_trigger(self, index: int, *configurations: ConfigurationT) -> None:
+    def _insert_without_trigger(
+        self, index: int, *configurations: ConfigurationT
+    ) -> None:
         current_configuration_keys = list(self._keys_without_scope())
         self._append_without_trigger(*configurations)
         self._move_to_end_without_trigger(
             *current_configuration_keys[0:index],
             *map(self._get_key, configurations),
-            *current_configuration_keys[index:]
+            *current_configuration_keys[index:],
         )
 
     def insert(self, index: int, *configurations: ConfigurationT) -> None:
         self._insert_without_trigger(index, *configurations)
         self._dispatch_change()
 
     def move_to_beginning(self, *configuration_keys: ConfigurationKeyT) -> None:
         for configuration_key in reversed(configuration_keys):
             self._configurations.move_to_end(configuration_key, False)
         self._dispatch_change()
 
     def move_towards_beginning(self, *configuration_keys: ConfigurationKeyT) -> None:
         self._move_by_offset(-1, *configuration_keys)
 
-    def _move_to_end_without_trigger(self, *configuration_keys: ConfigurationKeyT) -> None:
+    def _move_to_end_without_trigger(
+        self, *configuration_keys: ConfigurationKeyT
+    ) -> None:
         for configuration_key in configuration_keys:
             self._configurations.move_to_end(configuration_key)
 
     def move_to_end(self, *configuration_keys: ConfigurationKeyT) -> None:
         self._move_to_end_without_trigger(*configuration_keys)
         self._dispatch_change()
 
     def move_towards_end(self, *configuration_keys: ConfigurationKeyT) -> None:
         self._move_by_offset(1, *configuration_keys)
 
-    def _move_by_offset(self, offset: int, *configuration_keys: ConfigurationKeyT) -> None:
+    def _move_by_offset(
+        self, offset: int, *configuration_keys: ConfigurationKeyT
+    ) -> None:
         current_configuration_keys = list(self._keys_without_scope())
         indices = list(self.to_indices(*configuration_keys))
         if offset > 0:
             indices.reverse()
         for index in indices:
-            self._insert_without_trigger(index + offset, self._configurations.pop(current_configuration_keys[index]))
+            self._insert_without_trigger(
+                index + offset,
+                self._configurations.pop(current_configuration_keys[index]),
+            )
         self._dispatch_change()
 
     def _get_key(self, configuration: ConfigurationT) -> ConfigurationKeyT:
         raise NotImplementedError(repr(self))
 
     @classmethod
     def _load_key(
@@ -582,10 +638,12 @@
     _configuration: ConfigurationT
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
 
     @property
     def configuration(self) -> ConfigurationT:
-        if not hasattr(self, '_configuration'):
-            raise RuntimeError(f'{self} has no configuration. {type(self)}.__init__() must ensure it is set.')
+        if not hasattr(self, "_configuration"):
+            raise RuntimeError(
+                f"{self} has no configuration. {type(self)}.__init__() must ensure it is set."
+            )
         return self._configuration
```

### Comparing `betty-0.3.3/betty/deriver.py` & `betty-0.3.4/betty/deriver.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 
 import logging
 from enum import Enum
 from typing import Iterable, cast
 
 from betty.locale import DateRange, Date, Localizer
 from betty.model.ancestry import Person, Presence, Event, Subject, Ancestry
-from betty.model.event_type import DerivableEventType, CreatableDerivableEventType, EventType
+from betty.model.event_type import (
+    DerivableEventType,
+    CreatableDerivableEventType,
+    EventType,
+)
 
 
 class Derivation(Enum):
     NONE = 1
     CREATE = 2
     UPDATE = 3
 
@@ -40,32 +44,54 @@
             created_derivations = 0
             updated_derivations = 0
             for person in self._ancestry[Person]:
                 created, updated = self._derive_person(person, derivable_event_type)
                 created_derivations += created
                 updated_derivations += updated
             if updated_derivations > 0:
-                logger.info(self._localizer._('Updated {updated_derivations} {event_type} events based on existing information.').format(
-                    updated_derivations=str(updated_derivations),
-                    event_type=derivable_event_type.label().localize(self._localizer),
-                ))
+                logger.info(
+                    self._localizer._(
+                        "Updated {updated_derivations} {event_type} events based on existing information."
+                    ).format(
+                        updated_derivations=str(updated_derivations),
+                        event_type=derivable_event_type.label().localize(
+                            self._localizer
+                        ),
+                    )
+                )
             if created_derivations > 0:
-                logger.info(self._localizer._('Created {created_derivations} additional {event_type} events based on existing information.').format(
-                    created_derivations=str(created_derivations),
-                    event_type=derivable_event_type.label().localize(self._localizer),
-                ))
-
-    def _derive_person(self, person: Person, derivable_event_type: type[DerivableEventType]) -> tuple[int, int]:
+                logger.info(
+                    self._localizer._(
+                        "Created {created_derivations} additional {event_type} events based on existing information."
+                    ).format(
+                        created_derivations=str(created_derivations),
+                        event_type=derivable_event_type.label().localize(
+                            self._localizer
+                        ),
+                    )
+                )
+
+    def _derive_person(
+        self, person: Person, derivable_event_type: type[DerivableEventType]
+    ) -> tuple[int, int]:
         # Gather any existing events that could be derived, or create a new derived event if needed.
-        derivable_events: list[tuple[Event, Derivation]] = list(map(lambda event: (event, Derivation.UPDATE), _get_derivable_events(person, derivable_event_type)))
+        derivable_events: list[tuple[Event, Derivation]] = list(
+            map(
+                lambda event: (event, Derivation.UPDATE),
+                _get_derivable_events(person, derivable_event_type),
+            )
+        )
         if not derivable_events:
-            if list(filter(
-                lambda presence: presence.event is not None and issubclass(presence.event.event_type, derivable_event_type),
-                person.presences,
-            )):
+            if list(
+                filter(
+                    lambda presence: presence.event is not None
+                    and issubclass(presence.event.event_type, derivable_event_type),
+                    person.presences,
+                )
+            ):
                 return 0, 0
             if issubclass(
                 derivable_event_type,
                 CreatableDerivableEventType,
             ) and derivable_event_type.may_create(
                 person,
                 self._lifetime_threshold,
@@ -91,18 +117,22 @@
         for derivable_event, derivation in derivable_events:
             dates_derived = False
             # We know _get_derivable_events() only returns events without a date or a with a date range, but Python
             # does not let us express that in a(n intersection) type, so we must instead cast here.
             derivable_date = cast(DateRange | None, derivable_event.date)
 
             if derivable_date is None or derivable_date.end is None:
-                dates_derived = dates_derived or _ComesBeforeDateDeriver.derive(person, derivable_event, comes_before_event_types)
+                dates_derived = dates_derived or _ComesBeforeDateDeriver.derive(
+                    person, derivable_event, comes_before_event_types
+                )
 
             if derivable_date is None or derivable_date.start is None:
-                dates_derived = dates_derived or _ComesAfterDateDeriver.derive(person, derivable_event, comes_after_event_types)
+                dates_derived = dates_derived or _ComesAfterDateDeriver.derive(
+                    person, derivable_event, comes_after_event_types
+                )
 
             if dates_derived:
                 self._ancestry.add(derivable_event)
                 if derivation is Derivation.CREATE:
                     created_derivations += 1
                     presence = Presence(person, Subject(), derivable_event)
                     self._ancestry.add(presence)
@@ -110,38 +140,52 @@
                     updated_derivations += 1
 
         return created_derivations, updated_derivations
 
 
 class _DateDeriver:
     @classmethod
-    def derive(cls, person: Person, derivable_event: Event, reference_event_types: set[type[EventType]]) -> bool:
+    def derive(
+        cls,
+        person: Person,
+        derivable_event: Event,
+        reference_event_types: set[type[EventType]],
+    ) -> bool:
         assert issubclass(derivable_event.event_type, DerivableEventType)
 
         if not reference_event_types:
             return False
 
-        reference_events = _get_reference_events(person, reference_event_types, derivable_event.event_type)
+        reference_events = _get_reference_events(
+            person, reference_event_types, derivable_event.event_type
+        )
         reference_events_dates: Iterable[tuple[Event, Date]] = filter(
-            lambda x: x[1].comparable,
-            cls._get_events_dates(reference_events)
+            lambda x: x[1].comparable, cls._get_events_dates(reference_events)
         )
         if derivable_event.date is not None:
-            reference_events_dates = filter(lambda x: cls._compare(cast(DateRange, derivable_event.date), x[1]), reference_events_dates)
+            reference_events_dates = filter(
+                lambda x: cls._compare(cast(DateRange, derivable_event.date), x[1]),
+                reference_events_dates,
+            )
         sorted_reference_events_dates = cls._sort(reference_events_dates)
         try:
             reference_event, reference_date = sorted_reference_events_dates[0]
         except IndexError:
             return False
 
         if derivable_event.date is None:
             derivable_event.date = DateRange()
         cls._set(
             cast(DateRange, derivable_event.date),
-            Date(reference_date.year, reference_date.month, reference_date.day, fuzzy=reference_date.fuzzy),
+            Date(
+                reference_date.year,
+                reference_date.month,
+                reference_date.day,
+                fuzzy=reference_date.fuzzy,
+            ),
         )
         derivable_event.citations.add(*reference_event.citations)
 
         return True
 
     @classmethod
     def _get_events_dates(cls, events: Iterable[Event]) -> Iterable[tuple[Event, Date]]:
@@ -157,15 +201,17 @@
         raise NotImplementedError(repr(cls))
 
     @classmethod
     def _compare(cls, derivable_date: DateRange, reference_date: Date) -> bool:
         raise NotImplementedError(repr(cls))
 
     @classmethod
-    def _sort(cls, events_dates: Iterable[tuple[Event, Date]]) -> list[tuple[Event, Date]]:
+    def _sort(
+        cls, events_dates: Iterable[tuple[Event, Date]]
+    ) -> list[tuple[Event, Date]]:
         raise NotImplementedError(repr(cls))
 
     @classmethod
     def _set(cls, derivable_date: DateRange, derived_date: Date) -> None:
         raise NotImplementedError(repr(cls))
 
 
@@ -178,15 +224,17 @@
             yield date.end
 
     @classmethod
     def _compare(cls, derivable_date: DateRange, reference_date: Date) -> bool:
         return derivable_date < reference_date
 
     @classmethod
-    def _sort(cls, events_dates: Iterable[tuple[Event, Date]]) -> list[tuple[Event, Date]]:
+    def _sort(
+        cls, events_dates: Iterable[tuple[Event, Date]]
+    ) -> list[tuple[Event, Date]]:
         return sorted(events_dates, key=lambda x: x[1])
 
     @classmethod
     def _set(cls, derivable_date: DateRange, derived_date: Date) -> None:
         derivable_date.end = derived_date
         derivable_date.end_is_boundary = True
 
@@ -200,38 +248,46 @@
             yield date.end
 
     @classmethod
     def _compare(cls, derivable_date: DateRange, reference_date: Date) -> bool:
         return derivable_date > reference_date
 
     @classmethod
-    def _sort(cls, events_dates: Iterable[tuple[Event, Date]]) -> list[tuple[Event, Date]]:
+    def _sort(
+        cls, events_dates: Iterable[tuple[Event, Date]]
+    ) -> list[tuple[Event, Date]]:
         return sorted(events_dates, key=lambda x: x[1], reverse=True)
 
     @classmethod
     def _set(cls, derivable_date: DateRange, derived_date: Date) -> None:
         derivable_date.start = derived_date
         derivable_date.start_is_boundary = True
 
 
-def _get_derivable_events(person: Person, derivable_event_type: type[EventType]) -> Iterable[Event]:
+def _get_derivable_events(
+    person: Person, derivable_event_type: type[EventType]
+) -> Iterable[Event]:
     for presence in person.presences:
         event = presence.event
 
         if event is None:
             continue
 
         # Ignore events of the wrong type.
         if not issubclass(event.event_type, derivable_event_type):
             continue
 
         # Ignore events with enough date information that nothing more can be derived.
         if isinstance(event.date, Date):
             continue
-        if isinstance(event.date, DateRange) and (not event.event_type.comes_after() or event.date.start is not None) and (not event.event_type.comes_before() or event.date.end is not None):
+        if (
+            isinstance(event.date, DateRange)
+            and (not event.event_type.comes_after() or event.date.start is not None)
+            and (not event.event_type.comes_before() or event.date.end is not None)
+        ):
             continue
 
         yield event
 
 
 def _get_reference_events(
     person: Person,
```

### Comparing `betty-0.3.3/betty/documentation.py` & `betty-0.3.4/betty/documentation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide the Documentation API.
 """
+
 import asyncio
 import logging
 import shutil
 from contextlib import suppress, AsyncExitStack
 from pathlib import Path
 from subprocess import CalledProcessError
 from tempfile import TemporaryDirectory
@@ -15,53 +16,57 @@
 from betty.fs import ROOT_DIRECTORY_PATH
 from betty.locale import Str, Localizer
 from betty.serve import Server, NoPublicUrlBecauseServerNotStartedError
 from betty.subprocess import run_process
 
 
 async def _build_cache(cache_directory_path: Path) -> Path:
-    cache_directory_path /= 'docs'
+    cache_directory_path /= "docs"
     if not cache_directory_path.exists():
         await _build(cache_directory_path)
     return cache_directory_path
 
 
 async def _build(output_directory_path: Path) -> None:
     with suppress(FileExistsError):
         await makedirs(output_directory_path)
     with TemporaryDirectory() as working_directory_path_str:
         working_directory_path = Path(working_directory_path_str)
         # sphinx-apidoc must output to the documentation directory, but because we do not want
         # to 'pollute' that with generated files that must not be committed, do our work in a
         # temporary directory and copy the documentation source files there.
-        source_directory_path = working_directory_path / 'source'
-        await asyncio.to_thread(shutil.copytree, ROOT_DIRECTORY_PATH / 'documentation', source_directory_path)
+        source_directory_path = working_directory_path / "source"
+        await asyncio.to_thread(
+            shutil.copytree,
+            ROOT_DIRECTORY_PATH / "documentation",
+            source_directory_path,
+        )
         try:
 
             await run_process(
                 [
-                    'sphinx-apidoc',
-                    '--force',
-                    '--separate',
-                    '-d',
-                    '999',
-                    '-o',
+                    "sphinx-apidoc",
+                    "--force",
+                    "--separate",
+                    "-d",
+                    "999",
+                    "-o",
                     str(source_directory_path),
-                    str(ROOT_DIRECTORY_PATH / 'betty'),
-                    str(ROOT_DIRECTORY_PATH / 'betty' / 'tests'),
+                    str(ROOT_DIRECTORY_PATH / "betty"),
+                    str(ROOT_DIRECTORY_PATH / "betty" / "tests"),
                 ],
                 cwd=working_directory_path,
             )
             await run_process(
                 [
-                    'sphinx-build',
-                    '-j',
-                    'auto',
-                    '-b',
-                    'dirhtml',
+                    "sphinx-build",
+                    "-j",
+                    "auto",
+                    "-b",
+                    "dirhtml",
                     str(source_directory_path),
                     str(output_directory_path),
                 ],
                 cwd=working_directory_path,
             )
         except CalledProcessError as e:
             if e.stderr is not None:
@@ -79,25 +84,27 @@
         super().__init__(localizer)
         self._cache_directory_path = cache_directory_path
         self._server: Server | None = None
         self._exit_stack = AsyncExitStack()
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Betty documentation')
+        return Str._("Betty documentation")
 
     @property
     def public_url(self) -> str:
         if self._server is not None:
             return self._server.public_url
         raise NoPublicUrlBecauseServerNotStartedError()
 
     async def start(self) -> None:
         await super().start()
         www_directory_path = await _build_cache(self._cache_directory_path)
-        self._server = serve.BuiltinServer(www_directory_path, localizer=self._localizer)
+        self._server = serve.BuiltinServer(
+            www_directory_path, localizer=self._localizer
+        )
         await self._exit_stack.enter_async_context(self._server)
         await self.assert_available()
 
     async def stop(self) -> None:
         await self._exit_stack.aclose()
         await super().stop()
```

### Comparing `betty-0.3.3/betty/error.py` & `betty-0.3.4/betty/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Provide error handling utilities.
 """
+
 import traceback
 from typing import TypeVar, Self
 
 from betty.locale import Localizable, DEFAULT_LOCALIZER, Localizer
 
-BaseExceptionT = TypeVar('BaseExceptionT', bound=BaseException)
+BaseExceptionT = TypeVar("BaseExceptionT", bound=BaseException)
 
 
 def serialize(error: BaseExceptionT) -> BaseExceptionT:
     """
     Serialize an exception.
 
     This replaces the exception's traceback object with the traceback formatted as a string.
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/__init__.py` & `betty-0.3.4/betty/extension/cotton_candy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,82 @@
 """
 Provide Betty's default theme.
 """
+
 from __future__ import annotations
 
-import asyncio
-import logging
 import re
 from collections import defaultdict
 from collections.abc import Sequence, AsyncIterable
 from pathlib import Path
-from shutil import copy2
 from typing import Any, Callable, Iterable, Self, cast
 
 from PyQt6.QtWidgets import QWidget
-from aiofiles.os import makedirs
 from jinja2 import pass_context
 from jinja2.runtime import Context
 
 from betty.app.extension import ConfigurableExtension, Extension, Theme
 from betty.config import Configuration
 from betty.extension.cotton_candy.search import Index
-from betty.extension.npm import _Npm, _NpmBuilder, npm
+from betty.extension.webpack import Webpack, WebpackEntrypointProvider
 from betty.functools import walk
-from betty.generate import Generator, GenerationContext
 from betty.gui import GuiBuilder
-from betty.jinja2 import Jinja2Provider, context_app, context_localizer, context_job_context
+from betty.html import CssProvider
+from betty.jinja2 import (
+    Jinja2Provider,
+    context_app,
+    context_localizer,
+    context_job_context,
+)
 from betty.locale import Date, Str, Datey
 from betty.model import Entity, UserFacingEntity, GeneratedEntityId
 from betty.model.ancestry import Event, Person, Presence, is_public, Subject
 from betty.model.event_type import StartOfLifeEventType, EndOfLifeEventType
 from betty.project import EntityReferenceSequence, EntityReference
 from betty.serde.dump import minimize, Dump, VoidableDump
-from betty.serde.load import AssertionFailed, Fields, Assertions, OptionalField, Asserter
+from betty.serde.load import (
+    AssertionFailed,
+    Fields,
+    Assertions,
+    OptionalField,
+    Asserter,
+)
 
 
 class _ColorConfiguration(Configuration):
-    _HEX_PATTERN = re.compile(r'^#[a-zA-Z0-9]{6}$')
+    _HEX_PATTERN = re.compile(r"^#[a-zA-Z0-9]{6}$")
 
     def __init__(self, hex_value: str):
         super().__init__()
         self._hex: str
         self.hex = hex_value
 
     def _validate_hex(self, hex_value: str) -> str:
         if not self._HEX_PATTERN.match(hex_value):
-            raise AssertionFailed(Str._(
-                '"{hex_value}" is not a valid hexadecimal color, such as #ffc0cb.',
-                hex_value=hex_value,
-            ))
+            raise AssertionFailed(
+                Str._(
+                    '"{hex_value}" is not a valid hexadecimal color, such as #ffc0cb.',
+                    hex_value=hex_value,
+                )
+            )
         return hex_value
 
     @property
     def hex(self) -> str:
         return self._hex
 
     @hex.setter
     def hex(self, hex_value: str) -> None:
         if not self._HEX_PATTERN.match(hex_value):
-            raise AssertionFailed(Str._(
-                '"{hex_value}" is not a valid hexadecimal color, such as #ffc0cb.',
-                hex_value=hex_value,
-            ))
+            raise AssertionFailed(
+                Str._(
+                    '"{hex_value}" is not a valid hexadecimal color, such as #ffc0cb.',
+                    hex_value=hex_value,
+                )
+            )
         self._hex = hex_value
         self._dispatch_change()
 
     def update(self, other: Self) -> None:
         self.hex = other.hex
 
     @classmethod
@@ -82,30 +94,34 @@
         return configuration
 
     def dump(self) -> VoidableDump:
         return self._hex
 
 
 class CottonCandyConfiguration(Configuration):
-    DEFAULT_PRIMARY_INACTIVE_COLOR = '#ffc0cb'
-    DEFAULT_PRIMARY_ACTIVE_COLOR = '#ff69b4'
-    DEFAULT_LINK_INACTIVE_COLOR = '#149988'
-    DEFAULT_LINK_ACTIVE_COLOR = '#2a615a'
+    DEFAULT_PRIMARY_INACTIVE_COLOR = "#ffc0cb"
+    DEFAULT_PRIMARY_ACTIVE_COLOR = "#ff69b4"
+    DEFAULT_LINK_INACTIVE_COLOR = "#149988"
+    DEFAULT_LINK_ACTIVE_COLOR = "#2a615a"
 
     def __init__(
         self,
         *,
-        featured_entities: Sequence[EntityReference[UserFacingEntity & Entity]] | None = None,
+        featured_entities: (
+            Sequence[EntityReference[UserFacingEntity & Entity]] | None
+        ) = None,
         primary_inactive_color: str = DEFAULT_PRIMARY_INACTIVE_COLOR,
         primary_active_color: str = DEFAULT_PRIMARY_ACTIVE_COLOR,
         link_inactive_color: str = DEFAULT_LINK_INACTIVE_COLOR,
         link_active_color: str = DEFAULT_LINK_ACTIVE_COLOR,
     ):
         super().__init__()
-        self._featured_entities = EntityReferenceSequence['UserFacingEntity & Entity'](featured_entities or ())
+        self._featured_entities = EntityReferenceSequence["UserFacingEntity & Entity"](
+            featured_entities or ()
+        )
         self._featured_entities.on_change(self)
         self._primary_inactive_color = _ColorConfiguration(primary_inactive_color)
         self._primary_inactive_color.on_change(self)
         self._primary_active_color = _ColorConfiguration(primary_active_color)
         self._primary_active_color.on_change(self)
         self._link_inactive_color = _ColorConfiguration(link_inactive_color)
         self._link_inactive_color.on_change(self)
@@ -137,60 +153,122 @@
         cls,
         dump: Dump,
         configuration: Self | None = None,
     ) -> Self:
         if configuration is None:
             configuration = cls()
         asserter = Asserter()
-        asserter.assert_record(Fields(
-            OptionalField(
-                'featured_entities',
-                Assertions(configuration._featured_entities.assert_load(configuration._featured_entities)),
-            ),
-            OptionalField(
-                'primary_inactive_color',
-                Assertions(configuration._primary_inactive_color.assert_load(configuration._primary_inactive_color)),
-            ),
-            OptionalField(
-                'primary_active_color',
-                Assertions(configuration._primary_active_color.assert_load(configuration._primary_active_color)),
-            ),
-            OptionalField(
-                'link_inactive_color',
-                Assertions(configuration._link_inactive_color.assert_load(configuration._link_inactive_color)),
-            ),
-            OptionalField(
-                'link_active_color',
-                Assertions(configuration._link_active_color.assert_load(configuration._link_active_color)),
-            ),
-        ))(dump)
+        asserter.assert_record(
+            Fields(
+                OptionalField(
+                    "featured_entities",
+                    Assertions(
+                        configuration._featured_entities.assert_load(
+                            configuration._featured_entities
+                        )
+                    ),
+                ),
+                OptionalField(
+                    "primary_inactive_color",
+                    Assertions(
+                        configuration._primary_inactive_color.assert_load(
+                            configuration._primary_inactive_color
+                        )
+                    ),
+                ),
+                OptionalField(
+                    "primary_active_color",
+                    Assertions(
+                        configuration._primary_active_color.assert_load(
+                            configuration._primary_active_color
+                        )
+                    ),
+                ),
+                OptionalField(
+                    "link_inactive_color",
+                    Assertions(
+                        configuration._link_inactive_color.assert_load(
+                            configuration._link_inactive_color
+                        )
+                    ),
+                ),
+                OptionalField(
+                    "link_active_color",
+                    Assertions(
+                        configuration._link_active_color.assert_load(
+                            configuration._link_active_color
+                        )
+                    ),
+                ),
+            )
+        )(dump)
         return configuration
 
     def dump(self) -> VoidableDump:
-        return minimize({
-            'featured_entities': self.featured_entities.dump(),
-            'primary_inactive_color': self._primary_inactive_color.dump(),
-            'primary_active_color': self._primary_active_color.dump(),
-            'link_inactive_color': self._link_inactive_color.dump(),
-            'link_active_color': self._link_active_color.dump(),
-        })
+        return minimize(
+            {
+                "featured_entities": self.featured_entities.dump(),
+                "primary_inactive_color": self._primary_inactive_color.dump(),
+                "primary_active_color": self._primary_active_color.dump(),
+                "link_inactive_color": self._link_inactive_color.dump(),
+                "link_active_color": self._link_active_color.dump(),
+            }
+        )
+
 
+class CottonCandy(
+    Theme,
+    CssProvider,
+    ConfigurableExtension[CottonCandyConfiguration],
+    GuiBuilder,
+    Jinja2Provider,
+    WebpackEntrypointProvider,
+):
+    @classmethod
+    def name(cls) -> str:
+        return "betty.extension.CottonCandy"
 
-class _CottonCandy(Theme, ConfigurableExtension[CottonCandyConfiguration], Generator, GuiBuilder, _NpmBuilder, Jinja2Provider):
     @classmethod
     def depends_on(cls) -> set[type[Extension]]:
-        return {_Npm}
+        return {Webpack}
+
+    @classmethod
+    def comes_after(cls) -> set[type[Extension]]:
+        from betty.extension import Maps, Trees
+
+        return {Maps, Trees}
+
+    @classmethod
+    def assets_directory_path(cls) -> Path:
+        return Path(__file__).parent / "assets"
 
     @classmethod
-    def assets_directory_path(cls) -> Path | None:
-        return Path(__file__).parent / 'assets'
+    def webpack_entrypoint_directory_path(cls) -> Path:
+        return Path(__file__).parent / "webpack"
+
+    def webpack_entrypoint_cache_keys(self) -> Sequence[str]:
+        return (
+            self._app.project.configuration.root_path,
+            self._configuration.primary_inactive_color.hex,
+            self._configuration.primary_active_color.hex,
+            self._configuration.link_inactive_color.hex,
+            self._configuration.link_active_color.hex,
+        )
+
+    @property
+    def public_css_paths(self) -> list[str]:
+        return [
+            self.app.static_url_generator.generate(
+                "css/betty.extension.CottonCandy.css"
+            ),
+        ]
 
     @classmethod
     def label(cls) -> Str:
-        return Str.plain('Cotton Candy')
+        return Str.plain("Cotton Candy")
 
     @classmethod
     def default_configuration(cls) -> CottonCandyConfiguration:
         return CottonCandyConfiguration()
 
     @classmethod
     def description(cls) -> Str:
@@ -200,43 +278,26 @@
         from betty.extension.cotton_candy.gui import _CottonCandyGuiWidget
 
         return _CottonCandyGuiWidget(self._app)
 
     @property
     def globals(self) -> dict[str, Any]:
         return {
-            'search_index': _global_search_index,
+            "search_index": _global_search_index,
         }
 
     @property
     def filters(self) -> dict[str, Callable[..., Any]]:
         return {
-            'person_timeline_events': lambda person: person_timeline_events(
-                person,
-                self.app.project.configuration.lifetime_threshold
+            "person_timeline_events": lambda person: person_timeline_events(
+                person, self.app.project.configuration.lifetime_threshold
             ),
-            'person_descendant_families': person_descendant_families,
+            "person_descendant_families": person_descendant_families,
         }
 
-    async def npm_build(self, working_directory_path: Path, assets_directory_path: Path) -> None:
-        await self.app.extensions[_Npm].install(type(self), working_directory_path)
-        await npm(('run', 'webpack'), cwd=working_directory_path)
-        await self._copy_npm_build(working_directory_path / 'webpack-build', assets_directory_path)
-        logging.getLogger(__name__).info(self._app.localizer._('Built the Cotton Candy front-end assets.'))
-
-    async def _copy_npm_build(self, source_directory_path: Path, destination_directory_path: Path) -> None:
-        await makedirs(destination_directory_path, exist_ok=True)
-        await asyncio.to_thread(copy2, source_directory_path / 'cotton_candy.css', destination_directory_path / 'cotton_candy.css')
-        await asyncio.to_thread(copy2, source_directory_path / 'cotton_candy.js', destination_directory_path / 'cotton_candy.js')
-
-    async def generate(self, job_context: GenerationContext) -> None:
-        assets_directory_path = await self.app.extensions[_Npm].ensure_assets(self)
-        await makedirs(self.app.project.configuration.www_directory_path, exist_ok=True)
-        await self._copy_npm_build(assets_directory_path, self.app.project.configuration.www_directory_path)
-
 
 @pass_context
 async def _global_search_index(context: Context) -> AsyncIterable[dict[str, str]]:
     return Index(
         context_app(context),
         context_job_context(context),
         context_localizer(context),
@@ -263,15 +324,17 @@
     for event in _person_timeline_events(person, lifetime_threshold):
         if event in seen:
             continue
         seen.append(event)
         yield event
 
 
-def person_descendant_families(person: Person) -> Iterable[tuple[Sequence[Person], Sequence[Person]]]:
+def person_descendant_families(
+    person: Person,
+) -> Iterable[tuple[Sequence[Person], Sequence[Person]]]:
     """
     Gather a person's families they are a parent in.
     """
     parents = {}
     children = defaultdict(set)
     for child in person.children:
         family = tuple(sorted(map(lambda parent: parent.id, child.parents)))
@@ -342,39 +405,46 @@
             end_date_reference.year + lifetime_threshold,
             end_date_reference.month,
             end_date_reference.day,
             end_date_reference.fuzzy,
         )
 
     if start_date is None or end_date is None:
-        reference_dates = list(sorted(
-            cast(Datey, cast(Event, presence.event).date)
-            for presence
-            in person.presences
-            if _is_person_timeline_presence(presence)
-        ))
+        reference_dates = list(
+            sorted(
+                cast(Datey, cast(Event, presence.event).date)
+                for presence in person.presences
+                if _is_person_timeline_presence(presence)
+            )
+        )
         if reference_dates:
             if not start_date:
                 start_date = reference_dates[0]
             if not end_date:
                 end_date = reference_dates[-1]
 
     if start_date is not None and end_date is not None:
-        associated_people = filter(is_public, (
-            # All ancestors.
-            *walk(person, 'parents'),
-            # All descendants.
-            *walk(person, 'children'),
-            # All siblings.
-            *person.siblings,
-        ))
+        associated_people = filter(
+            is_public,
+            (
+                # All ancestors.
+                *walk(person, "parents"),
+                # All descendants.
+                *walk(person, "children"),
+                # All siblings.
+                *person.siblings,
+            ),
+        )
         for associated_person in associated_people:
             # For associated events, we are only interested in people's start- or end-of-life events.
             for associated_presence in associated_person.presences:
-                if not associated_presence.event or not issubclass(associated_presence.event.event_type, (StartOfLifeEventType, EndOfLifeEventType)):
+                if not associated_presence.event or not issubclass(
+                    associated_presence.event.event_type,
+                    (StartOfLifeEventType, EndOfLifeEventType),
+                ):
                     continue
                 if isinstance(associated_presence.event.id, GeneratedEntityId):
                     continue
                 if not isinstance(associated_presence.role, Subject):
                     continue
                 if not _is_person_timeline_presence(associated_presence):
                     continue
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/citation.scss` & `betty-0.3.4/betty/extension/cotton_candy/webpack/citation.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/entity.scss` & `betty-0.3.4/betty/extension/cotton_candy/webpack/entity.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.js` & `betty-0.3.4/betty/extension/cotton_candy/webpack/file.ts`

 * *Files 20% similar despite different names*

```diff
@@ -4,112 +4,115 @@
 00000030: 7374 205f 5052 4556 494f 5553 5f46 494c  st _PREVIOUS_FIL
 00000040: 455f 4b45 5953 203d 205b 2741 7272 6f77  E_KEYS = ['Arrow
 00000050: 4c65 6674 275d 0a63 6f6e 7374 205f 4e45  Left'].const _NE
 00000060: 5854 5f46 494c 455f 4b45 5953 203d 205b  XT_FILE_KEYS = [
 00000070: 2741 7272 6f77 5269 6768 7427 5d0a 0a6c  'ArrowRight']..l
 00000080: 6574 205f 706f 7369 7469 6f6e 5820 3d20  et _positionX = 
 00000090: 6e75 6c6c 0a6c 6574 205f 706f 7369 7469  null.let _positi
-000000a0: 6f6e 5920 3d20 6e75 6c6c 0a0a 6675 6e63  onY = null..func
-000000b0: 7469 6f6e 205f 696e 6974 6961 6c69 7a65  tion _initialize
-000000c0: 4669 6c65 7320 2829 207b 0a20 205f 696e  Files () {.  _in
-000000d0: 6974 6961 6c69 7a65 4669 6c65 4578 7465  itializeFileExte
-000000e0: 6e64 6564 4f70 656e 2829 0a20 205f 696e  ndedOpen().  _in
-000000f0: 6974 6961 6c69 7a65 4669 6c65 4578 7465  itializeFileExte
-00000100: 6e64 6564 436c 6f73 6528 290a 2020 5f69  ndedClose().  _i
-00000110: 6e69 7469 616c 697a 6546 696c 6545 7874  nitializeFileExt
-00000120: 656e 6465 644b 6579 5072 6573 7365 7328  endedKeyPresses(
-00000130: 290a 7d0a 0a66 756e 6374 696f 6e20 5f69  ).}..function _i
-00000140: 6e69 7469 616c 697a 6546 696c 6545 7874  nitializeFileExt
-00000150: 656e 6465 644f 7065 6e20 2829 207b 0a20  endedOpen () {. 
-00000160: 2063 6f6e 7374 206c 696e 6b73 203d 2064   const links = d
-00000170: 6f63 756d 656e 742e 6765 7445 6c65 6d65  ocument.getEleme
-00000180: 6e74 7342 7943 6c61 7373 4e61 6d65 2827  ntsByClassName('
-00000190: 6669 6c65 2d65 7874 656e 6465 642d 6f70  file-extended-op
-000001a0: 656e 2729 0a20 2066 6f72 2028 6c65 7420  en').  for (let 
-000001b0: 6920 3d20 303b 2069 203c 206c 696e 6b73  i = 0; i < links
-000001c0: 2e6c 656e 6774 683b 2069 2b2b 2920 7b0a  .length; i++) {.
-000001d0: 2020 2020 636f 6e73 7420 6c69 6e6b 203d      const link =
-000001e0: 206c 696e 6b73 5b69 5d0a 2020 2020 6c69   links[i].    li
-000001f0: 6e6b 2e61 6464 4576 656e 744c 6973 7465  nk.addEventListe
-00000200: 6e65 7228 2763 6c69 636b 272c 205f 6f70  ner('click', _op
-00000210: 656e 4578 7465 6e64 6564 290a 2020 7d0a  enExtended).  }.
-00000220: 7d0a 0a66 756e 6374 696f 6e20 5f6f 7065  }..function _ope
-00000230: 6e45 7874 656e 6465 6420 2829 207b 0a20  nExtended () {. 
-00000240: 205f 706f 7369 7469 6f6e 5820 3d20 7769   _positionX = wi
-00000250: 6e64 6f77 2e73 6372 6f6c 6c58 0a20 205f  ndow.scrollX.  _
-00000260: 706f 7369 7469 6f6e 5920 3d20 7769 6e64  positionY = wind
-00000270: 6f77 2e73 6372 6f6c 6c59 0a7d 0a0a 6675  ow.scrollY.}..fu
-00000280: 6e63 7469 6f6e 205f 696e 6974 6961 6c69  nction _initiali
-00000290: 7a65 4669 6c65 4578 7465 6e64 6564 436c  zeFileExtendedCl
-000002a0: 6f73 6520 2829 207b 0a20 2063 6f6e 7374  ose () {.  const
-000002b0: 206c 696e 6b73 203d 2064 6f63 756d 656e   links = documen
-000002c0: 742e 6765 7445 6c65 6d65 6e74 7342 7943  t.getElementsByC
-000002d0: 6c61 7373 4e61 6d65 2827 6669 6c65 2d65  lassName('file-e
-000002e0: 7874 656e 6465 642d 636c 6f73 6527 290a  xtended-close').
-000002f0: 2020 666f 7220 286c 6574 2069 203d 2030    for (let i = 0
-00000300: 3b20 6920 3c20 6c69 6e6b 732e 6c65 6e67  ; i < links.leng
-00000310: 7468 3b20 692b 2b29 207b 0a20 2020 2063  th; i++) {.    c
-00000320: 6f6e 7374 206c 696e 6b20 3d20 6c69 6e6b  onst link = link
-00000330: 735b 695d 0a20 2020 206c 696e 6b2e 6164  s[i].    link.ad
-00000340: 6445 7665 6e74 4c69 7374 656e 6572 2827  dEventListener('
-00000350: 636c 6963 6b27 2c20 5f63 6c6f 7365 4578  click', _closeEx
-00000360: 7465 6e64 6564 290a 2020 7d0a 7d0a 0a66  tended).  }.}..f
-00000370: 756e 6374 696f 6e20 5f63 6c6f 7365 4578  unction _closeEx
-00000380: 7465 6e64 6564 2028 6529 207b 0a20 2077  tended (e) {.  w
-00000390: 696e 646f 772e 6c6f 6361 7469 6f6e 203d  indow.location =
-000003a0: 2027 2327 0a20 2077 696e 646f 772e 7363   '#'.  window.sc
-000003b0: 726f 6c6c 546f 287b 0a20 2020 206c 6566  rollTo({.    lef
-000003c0: 743a 205f 706f 7369 7469 6f6e 582c 0a20  t: _positionX,. 
-000003d0: 2020 2074 6f70 3a20 5f70 6f73 6974 696f     top: _positio
-000003e0: 6e59 0a20 207d 290a 2020 5f70 6f73 6974  nY.  }).  _posit
-000003f0: 696f 6e58 203d 206e 756c 6c0a 2020 5f70  ionX = null.  _p
-00000400: 6f73 6974 696f 6e59 203d 206e 756c 6c0a  ositionY = null.
-00000410: 2020 652e 7072 6576 656e 7444 6566 6175    e.preventDefau
-00000420: 6c74 2829 0a7d 0a0a 6675 6e63 7469 6f6e  lt().}..function
-00000430: 205f 696e 6974 6961 6c69 7a65 4669 6c65   _initializeFile
-00000440: 4578 7465 6e64 6564 4b65 7950 7265 7373  ExtendedKeyPress
-00000450: 6573 2028 2920 7b0a 2020 646f 6375 6d65  es () {.  docume
-00000460: 6e74 2e61 6464 4576 656e 744c 6973 7465  nt.addEventListe
-00000470: 6e65 7228 276b 6579 646f 776e 272c 2066  ner('keydown', f
-00000480: 756e 6374 696f 6e20 2865 2920 7b0a 2020  unction (e) {.  
-00000490: 2020 6966 2028 5f43 4c4f 5345 5f4b 4559    if (_CLOSE_KEY
-000004a0: 532e 696e 6465 784f 6628 652e 6b65 7929  S.indexOf(e.key)
-000004b0: 2021 3d3d 202d 3129 207b 0a20 2020 2020   !== -1) {.     
-000004c0: 2063 6f6e 7374 2063 6c6f 7365 203d 2064   const close = d
-000004d0: 6f63 756d 656e 742e 7175 6572 7953 656c  ocument.querySel
-000004e0: 6563 746f 7228 272e 6669 6c65 2d65 7874  ector('.file-ext
-000004f0: 656e 6465 643a 7461 7267 6574 202e 6669  ended:target .fi
-00000500: 6c65 2d65 7874 656e 6465 642d 636c 6f73  le-extended-clos
-00000510: 6520 6127 290a 2020 2020 2020 6966 2028  e a').      if (
-00000520: 636c 6f73 6529 207b 0a20 2020 2020 2020  close) {.       
-00000530: 2063 6c6f 7365 2e63 6c69 636b 2829 0a20   close.click(). 
-00000540: 2020 2020 207d 0a20 2020 207d 2065 6c73       }.    } els
-00000550: 6520 6966 2028 5f50 5245 5649 4f55 535f  e if (_PREVIOUS_
-00000560: 4649 4c45 5f4b 4559 532e 696e 6465 784f  FILE_KEYS.indexO
-00000570: 6628 652e 6b65 7929 2021 3d3d 202d 3129  f(e.key) !== -1)
-00000580: 207b 0a20 2020 2020 2063 6f6e 7374 2070   {.      const p
-00000590: 7265 7669 6f75 7320 3d20 646f 6375 6d65  revious = docume
-000005a0: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
-000005b0: 2827 2e66 696c 652d 6578 7465 6e64 6564  ('.file-extended
-000005c0: 3a74 6172 6765 7420 2e66 696c 652d 6578  :target .file-ex
-000005d0: 7465 6e64 6564 2d70 7265 7669 6f75 7320  tended-previous 
-000005e0: 6127 290a 2020 2020 2020 6966 2028 7072  a').      if (pr
-000005f0: 6576 696f 7573 2920 7b0a 2020 2020 2020  evious) {.      
-00000600: 2020 7072 6576 696f 7573 2e63 6c69 636b    previous.click
-00000610: 2829 0a20 2020 2020 207d 0a20 2020 207d  ().      }.    }
-00000620: 2065 6c73 6520 6966 2028 5f4e 4558 545f   else if (_NEXT_
-00000630: 4649 4c45 5f4b 4559 532e 696e 6465 784f  FILE_KEYS.indexO
-00000640: 6628 652e 6b65 7929 2021 3d3d 202d 3129  f(e.key) !== -1)
-00000650: 207b 0a20 2020 2020 2063 6f6e 7374 206e   {.      const n
-00000660: 6578 7420 3d20 646f 6375 6d65 6e74 2e71  ext = document.q
-00000670: 7565 7279 5365 6c65 6374 6f72 2827 2e66  uerySelector('.f
-00000680: 696c 652d 6578 7465 6e64 6564 3a74 6172  ile-extended:tar
-00000690: 6765 7420 2e66 696c 652d 6578 7465 6e64  get .file-extend
-000006a0: 6564 2d6e 6578 7420 6127 290a 2020 2020  ed-next a').    
-000006b0: 2020 6966 2028 6e65 7874 2920 7b0a 2020    if (next) {.  
-000006c0: 2020 2020 2020 6e65 7874 2e63 6c69 636b        next.click
-000006d0: 2829 0a20 2020 2020 207d 0a20 2020 207d  ().      }.    }
-000006e0: 0a20 207d 290a 7d0a 0a64 6f63 756d 656e  .  }).}..documen
-000006f0: 742e 6164 6445 7665 6e74 4c69 7374 656e  t.addEventListen
-00000700: 6572 2827 444f 4d43 6f6e 7465 6e74 4c6f  er('DOMContentLo
-00000710: 6164 6564 272c 205f 696e 6974 6961 6c69  aded', _initiali
-00000720: 7a65 4669 6c65 7329 0a                   zeFiles).
+000000a0: 6f6e 5920 3d20 6e75 6c6c 0a0a 6173 796e  onY = null..asyn
+000000b0: 6320 6675 6e63 7469 6f6e 2069 6e69 7469  c function initi
+000000c0: 616c 697a 6546 696c 6573 2028 2920 3a50  alizeFiles () :P
+000000d0: 726f 6d69 7365 3c76 6f69 643e 207b 202f  romise<void> { /
+000000e0: 2f20 6573 6c69 6e74 2d64 6973 6162 6c65  / eslint-disable
+000000f0: 2d6c 696e 6520 4074 7970 6573 6372 6970  -line @typescrip
+00000100: 742d 6573 6c69 6e74 2f72 6571 7569 7265  t-eslint/require
+00000110: 2d61 7761 6974 0a20 205f 696e 6974 6961  -await.  _initia
+00000120: 6c69 7a65 4669 6c65 4578 7465 6e64 6564  lizeFileExtended
+00000130: 4f70 656e 2829 0a20 205f 696e 6974 6961  Open().  _initia
+00000140: 6c69 7a65 4669 6c65 4578 7465 6e64 6564  lizeFileExtended
+00000150: 436c 6f73 6528 290a 2020 5f69 6e69 7469  Close().  _initi
+00000160: 616c 697a 6546 696c 6545 7874 656e 6465  alizeFileExtende
+00000170: 644b 6579 5072 6573 7365 7328 290a 7d0a  dKeyPresses().}.
+00000180: 0a66 756e 6374 696f 6e20 5f69 6e69 7469  .function _initi
+00000190: 616c 697a 6546 696c 6545 7874 656e 6465  alizeFileExtende
+000001a0: 644f 7065 6e20 2829 203a 766f 6964 207b  dOpen () :void {
+000001b0: 0a20 2063 6f6e 7374 206c 696e 6b73 203d  .  const links =
+000001c0: 2064 6f63 756d 656e 742e 6765 7445 6c65   document.getEle
+000001d0: 6d65 6e74 7342 7943 6c61 7373 4e61 6d65  mentsByClassName
+000001e0: 2827 6669 6c65 2d65 7874 656e 6465 642d  ('file-extended-
+000001f0: 6f70 656e 2729 0a20 2066 6f72 2028 636f  open').  for (co
+00000200: 6e73 7420 6c69 6e6b 206f 6620 6c69 6e6b  nst link of link
+00000210: 7329 207b 0a20 2020 2028 6c69 6e6b 2061  s) {.    (link a
+00000220: 7320 456c 656d 656e 7429 2e61 6464 4576  s Element).addEv
+00000230: 656e 744c 6973 7465 6e65 7228 2763 6c69  entListener('cli
+00000240: 636b 272c 205f 6f70 656e 4578 7465 6e64  ck', _openExtend
+00000250: 6564 290a 2020 7d0a 7d0a 0a66 756e 6374  ed).  }.}..funct
+00000260: 696f 6e20 5f6f 7065 6e45 7874 656e 6465  ion _openExtende
+00000270: 6420 2829 203a 766f 6964 207b 0a20 205f  d () :void {.  _
+00000280: 706f 7369 7469 6f6e 5820 3d20 7769 6e64  positionX = wind
+00000290: 6f77 2e73 6372 6f6c 6c58 0a20 205f 706f  ow.scrollX.  _po
+000002a0: 7369 7469 6f6e 5920 3d20 7769 6e64 6f77  sitionY = window
+000002b0: 2e73 6372 6f6c 6c59 0a7d 0a0a 6675 6e63  .scrollY.}..func
+000002c0: 7469 6f6e 205f 696e 6974 6961 6c69 7a65  tion _initialize
+000002d0: 4669 6c65 4578 7465 6e64 6564 436c 6f73  FileExtendedClos
+000002e0: 6520 2829 203a 766f 6964 207b 0a20 2063  e () :void {.  c
+000002f0: 6f6e 7374 206c 696e 6b73 203d 2064 6f63  onst links = doc
+00000300: 756d 656e 742e 6765 7445 6c65 6d65 6e74  ument.getElement
+00000310: 7342 7943 6c61 7373 4e61 6d65 2827 6669  sByClassName('fi
+00000320: 6c65 2d65 7874 656e 6465 642d 636c 6f73  le-extended-clos
+00000330: 6527 290a 2020 666f 7220 2863 6f6e 7374  e').  for (const
+00000340: 206c 696e 6b20 6f66 206c 696e 6b73 2920   link of links) 
+00000350: 7b0a 2020 2020 286c 696e 6b20 6173 2045  {.    (link as E
+00000360: 6c65 6d65 6e74 292e 6164 6445 7665 6e74  lement).addEvent
+00000370: 4c69 7374 656e 6572 2827 636c 6963 6b27  Listener('click'
+00000380: 2c20 5f63 6c6f 7365 4578 7465 6e64 6564  , _closeExtended
+00000390: 290a 2020 7d0a 7d0a 0a66 756e 6374 696f  ).  }.}..functio
+000003a0: 6e20 5f63 6c6f 7365 4578 7465 6e64 6564  n _closeExtended
+000003b0: 2028 653a 2045 7665 6e74 2920 3a76 6f69   (e: Event) :voi
+000003c0: 6420 7b0a 2020 7769 6e64 6f77 2e6c 6f63  d {.  window.loc
+000003d0: 6174 696f 6e20 3d20 2723 270a 2020 7769  ation = '#'.  wi
+000003e0: 6e64 6f77 2e73 6372 6f6c 6c54 6f28 7b0a  ndow.scrollTo({.
+000003f0: 2020 2020 6c65 6674 3a20 5f70 6f73 6974      left: _posit
+00000400: 696f 6e58 2c0a 2020 2020 746f 703a 205f  ionX,.    top: _
+00000410: 706f 7369 7469 6f6e 590a 2020 7d29 0a20  positionY.  }). 
+00000420: 205f 706f 7369 7469 6f6e 5820 3d20 6e75   _positionX = nu
+00000430: 6c6c 0a20 205f 706f 7369 7469 6f6e 5920  ll.  _positionY 
+00000440: 3d20 6e75 6c6c 0a20 2065 2e70 7265 7665  = null.  e.preve
+00000450: 6e74 4465 6661 756c 7428 290a 7d0a 0a66  ntDefault().}..f
+00000460: 756e 6374 696f 6e20 5f69 6e69 7469 616c  unction _initial
+00000470: 697a 6546 696c 6545 7874 656e 6465 644b  izeFileExtendedK
+00000480: 6579 5072 6573 7365 7320 2829 203a 766f  eyPresses () :vo
+00000490: 6964 207b 0a20 2064 6f63 756d 656e 742e  id {.  document.
+000004a0: 6164 6445 7665 6e74 4c69 7374 656e 6572  addEventListener
+000004b0: 2827 6b65 7964 6f77 6e27 2c20 6675 6e63  ('keydown', func
+000004c0: 7469 6f6e 2028 6529 207b 0a20 2020 2069  tion (e) {.    i
+000004d0: 6620 285f 434c 4f53 455f 4b45 5953 2e69  f (_CLOSE_KEYS.i
+000004e0: 6e63 6c75 6465 7328 652e 6b65 7929 2920  ncludes(e.key)) 
+000004f0: 7b0a 2020 2020 2020 636f 6e73 7420 636c  {.      const cl
+00000500: 6f73 6520 3d20 646f 6375 6d65 6e74 2e71  ose = document.q
+00000510: 7565 7279 5365 6c65 6374 6f72 3c48 544d  uerySelector<HTM
+00000520: 4c45 6c65 6d65 6e74 3e28 272e 6669 6c65  LElement>('.file
+00000530: 2d65 7874 656e 6465 643a 7461 7267 6574  -extended:target
+00000540: 202e 6669 6c65 2d65 7874 656e 6465 642d   .file-extended-
+00000550: 636c 6f73 6520 6127 290a 2020 2020 2020  close a').      
+00000560: 6966 2028 636c 6f73 6529 207b 0a20 2020  if (close) {.   
+00000570: 2020 2020 2063 6c6f 7365 2e63 6c69 636b       close.click
+00000580: 2829 0a20 2020 2020 207d 0a20 2020 207d  ().      }.    }
+00000590: 2065 6c73 6520 6966 2028 5f50 5245 5649   else if (_PREVI
+000005a0: 4f55 535f 4649 4c45 5f4b 4559 532e 696e  OUS_FILE_KEYS.in
+000005b0: 636c 7564 6573 2865 2e6b 6579 2929 207b  cludes(e.key)) {
+000005c0: 0a20 2020 2020 2063 6f6e 7374 2070 7265  .      const pre
+000005d0: 7669 6f75 7320 3d20 646f 6375 6d65 6e74  vious = document
+000005e0: 2e71 7565 7279 5365 6c65 6374 6f72 3c48  .querySelector<H
+000005f0: 544d 4c45 6c65 6d65 6e74 3e28 272e 6669  TMLElement>('.fi
+00000600: 6c65 2d65 7874 656e 6465 643a 7461 7267  le-extended:targ
+00000610: 6574 202e 6669 6c65 2d65 7874 656e 6465  et .file-extende
+00000620: 642d 7072 6576 696f 7573 2061 2729 0a20  d-previous a'). 
+00000630: 2020 2020 2069 6620 2870 7265 7669 6f75       if (previou
+00000640: 7329 207b 0a20 2020 2020 2020 2070 7265  s) {.        pre
+00000650: 7669 6f75 732e 636c 6963 6b28 290a 2020  vious.click().  
+00000660: 2020 2020 7d0a 2020 2020 7d20 656c 7365      }.    } else
+00000670: 2069 6620 285f 4e45 5854 5f46 494c 455f   if (_NEXT_FILE_
+00000680: 4b45 5953 2e69 6e63 6c75 6465 7328 652e  KEYS.includes(e.
+00000690: 6b65 7929 2920 7b0a 2020 2020 2020 636f  key)) {.      co
+000006a0: 6e73 7420 6e65 7874 203d 2064 6f63 756d  nst next = docum
+000006b0: 656e 742e 7175 6572 7953 656c 6563 746f  ent.querySelecto
+000006c0: 723c 4854 4d4c 456c 656d 656e 743e 2827  r<HTMLElement>('
+000006d0: 2e66 696c 652d 6578 7465 6e64 6564 3a74  .file-extended:t
+000006e0: 6172 6765 7420 2e66 696c 652d 6578 7465  arget .file-exte
+000006f0: 6e64 6564 2d6e 6578 7420 6127 290a 2020  nded-next a').  
+00000700: 2020 2020 6966 2028 6e65 7874 2920 7b0a      if (next) {.
+00000710: 2020 2020 2020 2020 6e65 7874 2e63 6c69          next.cli
+00000720: 636b 2829 0a20 2020 2020 207d 0a20 2020  ck().      }.   
+00000730: 207d 0a20 207d 290a 7d0a 0a65 7870 6f72   }.  }).}..expor
+00000740: 7420 7b0a 2020 696e 6974 6961 6c69 7a65  t {.  initialize
+00000750: 4669 6c65 732c 0a7d 0a                   Files,.}.
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.scss` & `betty-0.3.4/betty/extension/cotton_candy/webpack/file.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/overlay.scss` & `betty-0.3.4/betty/extension/cotton_candy/webpack/overlay.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/page.scss` & `betty-0.3.4/betty/extension/cotton_candy/webpack/page.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/person.scss` & `betty-0.3.4/betty/extension/cotton_candy/webpack/person.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.scss` & `betty-0.3.4/betty/extension/cotton_candy/webpack/search.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/text.scss` & `betty-0.3.4/betty/extension/cotton_candy/webpack/text.scss`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/variables.scss.j2` & `betty-0.3.4/betty/extension/cotton_candy/webpack/variables.scss`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-$primary-inactive-color: {{ app.extensions['betty.extension.CottonCandy'].configuration.primary_inactive_color.hex }};
-$primary-active-color: {{ app.extensions['betty.extension.CottonCandy'].configuration.primary_active_color.hex }};
-$link-inactive-color: {{ app.extensions['betty.extension.CottonCandy'].configuration.link_inactive_color.hex }};
-$link-active-color: {{ app.extensions['betty.extension.CottonCandy'].configuration.link_active_color.hex }};
-$betty-32-32-png-url: url('{{ "/betty-32x32.png" | static_url }}');
+$primary-inactive-color: #ffc0cb;
+$primary-active-color: #ff69b4;
+$link-inactive-color: #149988;
+$link-active-color: #2a615a;
+$betty-32-32-png-url: url('/betty-32x32.png');
 $language-svg-url: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="512" height="512" viewBox="0 0 512 512" fill="%23777777"><title>ionicons-v5-l</title><path d="M478.33,433.6l-90-218a22,22,0,0,0-40.67,0l-90,218a22,22,0,1,0,40.67,16.79L316.66,406H419.33l18.33,44.39A22,22,0,0,0,458,464a22,22,0,0,0,20.32-30.4ZM334.83,362,368,281.65,401.17,362Z"/><path d="M267.84,342.92a22,22,0,0,0-4.89-30.7c-.2-.15-15-11.13-36.49-34.73,39.65-53.68,62.11-114.75,71.27-143.49H330a22,22,0,0,0,0-44H214V70a22,22,0,0,0-44,0V90H54a22,22,0,0,0,0,44H251.25c-9.52,26.95-27.05,69.5-53.79,108.36-31.41-41.68-43.08-68.65-43.17-68.87a22,22,0,0,0-40.58,17c.58,1.38,14.55,34.23,52.86,83.93.92,1.19,1.83,2.35,2.74,3.51-39.24,44.35-77.74,71.86-93.85,80.74a22,22,0,1,0,21.07,38.63c2.16-1.18,48.6-26.89,101.63-85.59,22.52,24.08,38,35.44,38.93,36.1a22,22,0,0,0,30.75-4.9Z"/></svg>');
 $menu-svg-url: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="512" height="512" viewBox="0 0 512 512" fill="%23777777"><title>ionicons-v5-j</title><path d="M64,384H448V341.33H64Zm0-106.67H448V234.67H64ZM64,128v42.67H448V128Z"/></svg>');
 $close-svg-url: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="512" height="512" viewBox="0 0 512 512" fill="%23777777"><title>ionicons-v5-m</title><path d="M289.94,256l95-95A24,24,0,0,0,351,127l-95,95-95-95A24,24,0,0,0,127,161l95,95-95,95A24,24,0,1,0,161,385l95-95,95,95A24,24,0,0,0,385,351Z"/></svg>');
-$search-svg-url: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="512" height="512" viewBox="0 0 512 512" fill="%23ffffff"><title>ionicons-v5-f</title><path d="M456.69,421.39,362.6,327.3a173.81,173.81,0,0,0,34.84-104.58C397.44,126.38,319.06,48,222.72,48S48,126.38,48,222.72s78.38,174.72,174.72,174.72A173.81,173.81,0,0,0,327.3,362.6l94.09,94.09a25,25,0,0,0,35.3-35.3ZM97.92,222.72a124.8,124.8,0,1,1,124.8,124.8A124.95,124.95,0,0,1,97.92,222.72Z"/></svg>');
+$search-svg-url: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="512" height="512" viewBox="0 0 512 512" fill="%23ffffff"><title>ionicons-v5-f</title><path d="M456.69,421.39,362.6,327.3a173.81,173.81,0,0,0,34.84-104.58C397.44,126.38,319.06,48,222.72,48S48,126.38,48,222.72s78.38,174.72,174.72,174.72A173.81,173.81,0,0,0,327.3,362.6l94.09,94.09a25,25,0,0,0,35.3-35.3ZM97.92,222.72a124.8,124.8,0,1,1,124.8,124.8A124.95,124.95,0,0,1,97.92,222.72Z"/></svg>');
```

#### html2text {}

```diff
@@ -1,14 +1,7 @@
-$primary-inactive-color: {{ app.extensions
-['betty.extension.CottonCandy'].configuration.primary_inactive_color.hex }};
-$primary-active-color: {{ app.extensions
-['betty.extension.CottonCandy'].configuration.primary_active_color.hex }};
-$link-inactive-color: {{ app.extensions
-['betty.extension.CottonCandy'].configuration.link_inactive_color.hex }};
-$link-active-color: {{ app.extensions
-['betty.extension.CottonCandy'].configuration.link_active_color.hex }}; $betty-
-32-32-png-url: url('{{ "/betty-32x32.png" | static_url }}'); $language-svg-url:
-url('data:image/svg+xml;utf8,
+$primary-inactive-color: #ffc0cb; $primary-active-color: #ff69b4; $link-
+inactive-color: #149988; $link-active-color: #2a615a; $betty-32-32-png-url: url
+('/betty-32x32.png'); $language-svg-url: url('data:image/svg+xml;utf8,
 '); $menu-svg-url: url('data:image/svg+xml;utf8,
 '); $close-svg-url: url('data:image/svg+xml;utf8,
 '); $search-svg-url: url('data:image/svg+xml;utf8,
 ');
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/public/localized/index.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/public/localized/index.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/public/static/betty.webmanifest` & `betty-0.3.4/betty/extension/cotton_candy/assets/public/static/betty.webmanifest`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/base.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/base.html.j2`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 <!doctype html>
 <html lang="{{ localizer.locale }}"
       prefix="foaf: http://xmlns.com/foaf/0.1/ og: http://ogp.me/ns# rel: http://purl.org/vocab/relationship/">
 <head>
     {% include 'head.html.j2' %}
     <link rel="manifest" href="{{ '/betty.webmanifest' | static_url }}">
-    <link rel="stylesheet" href="{{ '/cotton_candy.css' | static_url }}">
-    <script src="{{ '/cotton_candy.js' | static_url }}" defer></script>
 </head>
 <body>
 <script>
     document.body.classList.add('with-js');
 </script>
 <div id="page">
     <nav id="nav-primary">
@@ -114,9 +112,13 @@
         {% include 'references.html.j2' %}
     </div>
     <footer>
         {% include 'footer.html.j2' %}
     </footer>
 </div>
 {% include 'linked-data.html.j2' %}
+{% include 'stylesheets.html.j2' %}
+{% do 'betty.extension.CottonCandy' | webpack_entrypoint_js %}
+{% include 'webpack-entry-loader.html.j2' %}
+{% include 'scripts.html.j2' %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -53,8 +53,10 @@
       endif %}>{{ link.label }}
  {% if link.description is not none %}
 {{ link.description }}
 {% endif %}
 {% endfor %}
 {% endif %} {% endif %} {% include 'references.html.j2' %}
 {% include 'footer.html.j2' %}
-{% include 'linked-data.html.j2' %}
+{% include 'linked-data.html.j2' %} {% include 'stylesheets.html.j2' %} {% do
+'betty.extension.CottonCandy' | webpack_entrypoint_js %} {% include 'webpack-
+entry-loader.html.j2' %} {% include 'scripts.html.j2' %}
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/featured.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% import 'macro/citation.html.j2' as citation_macros %}
+{% import 'macro/citation.html.j2' as citation_macros with context %}
 {% set person_name = person_name | default(entity) %}
 {% set embedded = embedded | default(False) %}
 {% set person_context = entity_contexts['Person'] %}
 {% set label_as_link = not embedded and person_context != person_name.person and person_name is not has_generated_entity_id and person_name is public %}
 {% if label_as_link -%}
     <a href="{{ person_name | url }}">
 {%- endif %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-{% import 'macro/citation.html.j2' as citation_macros %} {% set person_name =
-person_name | default(entity) %} {% set embedded = embedded | default(False) %}
-{% set person_context = entity_contexts['Person'] %} {% set label_as_link = not
-embedded and person_context != person_name.person and person_name is not
-has_generated_entity_id and person_name is public %} {% if label_as_link -%}
-_{_%_-_ _e_n_d_i_f_ _%_}_ _{_%_ _i_f_ _p_e_r_s_o_n___n_a_m_e_._p_r_i_v_a_t_e_ _-_%_}_ _{_%_ _t_r_a_n_s_ _%_}_p_r_i_v_a_t_e_{_%_ _e_n_d_t_r_a_n_s_ _%_}_ _{_%_-
-_e_l_s_e_ _-_%_}_ _{_%_-_ _i_f_ _p_e_r_s_o_n___n_a_m_e_._i_n_d_i_v_i_d_u_a_l_ _i_s_ _n_o_t_ _n_o_n_e_ _-_%_}_ _{
+{% import 'macro/citation.html.j2' as citation_macros with context %} {% set
+person_name = person_name | default(entity) %} {% set embedded = embedded |
+default(False) %} {% set person_context = entity_contexts['Person'] %} {% set
+label_as_link = not embedded and person_context != person_name.person and
+person_name is not has_generated_entity_id and person_name is public %} {% if
+label_as_link -%} _{_%_-_ _e_n_d_i_f_ _%_}_ _{_%_ _i_f_ _p_e_r_s_o_n___n_a_m_e_._p_r_i_v_a_t_e_ _-_%_}_ _{_%_ _t_r_a_n_s_ _%_}_p_r_i_v_a_t_e
+_{_%_ _e_n_d_t_r_a_n_s_ _%_}_ _{_%_-_ _e_l_s_e_ _-_%_}_ _{_%_-_ _i_f_ _p_e_r_s_o_n___n_a_m_e_._i_n_d_i_v_i_d_u_a_l_ _i_s_ _n_o_t_ _n_o_n_e_ _-_%_}_ _{
 _{_ _p_e_r_s_o_n___n_a_m_e_._i_n_d_i_v_i_d_u_a_l_ _}_}_ _{_%_-_ _e_l_s_e_ _-_%_}_ _â__¦_ _{_%_-_ _e_n_d_i_f_ _-_%_}_ _{_%_-_ _i_f
 _p_e_r_s_o_n___n_a_m_e_._a_f_f_i_l_i_a_t_i_o_n_ _i_s_ _n_o_t_ _n_o_n_e_ _%_}_ _{_{_ _p_e_r_s_o_n___n_a_m_e_._a_f_f_i_l_i_a_t_i_o_n_ _}_}_ _{_%_-_ _e_n_d_i_f
 _-_%_}_ _{_%_-_ _e_n_d_i_f_ _-_%_}_ _{_%_-_ _i_f_ _l_a_b_e_l___a_s___l_i_n_k_ _-_%_}_ {%- endif -%} {%- if not embedded
 and person_name is public -%} {{ citation_macros.cite(person_name.citations) }}
 {%- endif -%}
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--event.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/list--place.html.j2`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% set place_context = entity_contexts['Place'] %}
 {% set featured = featured | default(True) %}
 {% set places = places | default(entities) | select('public') | list | sort_localizeds(localized_attribute='names', sort_attribute='name') | list %}
 <div class="places{% if 'betty.extension.Maps' in app.extensions %} with-map{% endif %}">
     {% if 'betty.extension.Maps' in app.extensions and places | rejectattr('coordinates', 'none') | list | length > 0 %}
-        <div class="{% if featured %}featured {% endif %}map"></div>
+        {% include 'map.html.j2' %}
     {% endif %}
     <ul class="entities{% if hide_list | default(false) %} visually-hidden{% endif %}{% if map_hides_list | default(false) %} js-visually-hidden{% endif %}">
         {% for place in places %}
             <li class="{{ loop.cycle('odd', 'even') }}" data-betty-place="{{ place | url(media_type='application/json') }}">
                 {% include 'entity/label--place.html.j2' %}
                 {% include 'entity/meta--place.html.j2' %}
             </li>
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--person.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/meta--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--citation.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--event.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--file.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--person.html.j2`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                             {% endwith %}
                         {% endif %}
                     </div>
                 {% endfor %}
             {% endif %}
         </section>
 
-        <div class="featured tree" data-betty-person-id="{{ person.id }}" data-betty-people="{{ 'people.json' | url }}"></div>
+        {% include 'tree.html.j2' %}
     {% endif %}
 
     {% with events=person | person_timeline_events %}
         {% include 'timeline.html.j2' %}
     {% endwith %}
 
     {% with files = person.associated_files %}
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--place.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page--source.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/entity/page-list--source.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- import 'macro/citation.html.j2' as citation_macros -%}
+{%- import 'macro/citation.html.j2' as citation_macros with context -%}
 {%- set embedded = embedded | default(False) -%}
 {%- set citation_context = entity_contexts['Citation'] -%}
 {%- set place_context = entity_contexts['Place'] -%}
 {%- set formatted_date = '' -%}
 {%- if event.date -%}
     {%- set formatted_date = event.date | format_datey -%}
 {%- endif -%}
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/file.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/file.html.j2`

 * *Files 8% similar despite different names*

```diff
@@ -16,32 +16,32 @@
     {% do extended_media_type_paths.append('file-extended--' ~ file.media_type.type ~ '.html.j2') %}
     {% do extended_media_type_paths.append('file-extended--' ~ file.media_type.type ~ '--' ~ file.media_type.subtypes | join('---') ~ '.html.j2') %}
     {% if file.media_type.suffix %}
         {% do extended_media_type_paths.append('file-extended--' ~ file.media_type.type ~ '--' ~ file.media_type.subtypes | join('---') ~ '----' ~ file.media_type.suffix ~ '.html.j2') %}
     {% endif %}
 {% endif %}
 
-{% set file_id_base64 = file.id | base64 %}
-<div class="file" id="file-{{ file_id_base64 }}">
-    <a href="#file-extended-{{ file_id_base64 }}" class="file-extended-open file-summary">
+{% set file_hashid = file.id | hashid %}
+<div class="file" id="file-{{ file_hashid }}">
+    <a href="#file-extended-{{ file_hashid }}" class="file-extended-open file-summary">
         <div class="file-summary">
             {% include summary_media_type_paths | reverse | list %}
         </div>
     </a>
-    <div id="file-extended-{{ file_id_base64 }}" class="file-extended">
+    <div id="file-extended-{{ file_hashid }}" class="file-extended">
         <ul class="file-controls">
             <li><a href="{{ file | file | static_url }}" title="View original in full">⇔</a></li>
             <li><a href="{{ file | file | static_url }}" download="{{ file.path.name }}" title="Download this file">⇓</a></li>
             <li><a href="{{ file | url }}" title="More details">ℹ</a></li>
-            <li class="file-extended-close"><a href="#file-{{ file_id_base64 }}" title="Close this file">×</a></li>
+            <li class="file-extended-close"><a href="#file-{{ file_hashid }}" title="Close this file">×</a></li>
             {% if previous_file is defined %}
-                <li class="file-nav file-extended-previous"><a href="#file-extended-{{ previous_file.id | base64 }}" title="{{ previous_file.description }}">←</a></li>
+                <li class="file-nav file-extended-previous"><a href="#file-extended-{{ previous_file.id | hashid }}" title="{{ previous_file.description }}">←</a></li>
             {% endif %}
             {% if next_file is defined %}
-                <li class="file-nav file-extended-next"><a href="#file-extended-{{ next_file.id | base64 }}" title="{{ next_file.description }}">→</a></li>
+                <li class="file-nav file-extended-next"><a href="#file-extended-{{ next_file.id | hashid }}" title="{{ next_file.description }}">→</a></li>
             {% endif %}
         </ul>
         <div class="file-content">
             {% include extended_media_type_paths | reverse | list %}
         </div>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 '.html.j2') %} {% endif %} {% do extended_media_type_paths.append('file-
 extended--' ~ file.media_type.type ~ '.html.j2') %} {% do
 extended_media_type_paths.append('file-extended--' ~ file.media_type.type ~ '--
 ' ~ file.media_type.subtypes | join('---') ~ '.html.j2') %} {% if
 file.media_type.suffix %} {% do extended_media_type_paths.append('file-
 extended--' ~ file.media_type.type ~ '--' ~ file.media_type.subtypes | join('--
 -') ~ '----' ~ file.media_type.suffix ~ '.html.j2') %} {% endif %} {% endif %}
-{% set file_id_base64 = file.id | base64 %}
+{% set file_hashid = file.id | hashid %}
 _{_%_ _i_n_c_l_u_d_e_ _s_u_m_m_a_r_y___m_e_d_i_a___t_y_p_e___p_a_t_h_s_ _|_ _r_e_v_e_r_s_e_ _|_ _l_i_s_t_ _%_}
     * _â__
     * _â__
     * _â__¹
     * _Ã_
     * {% if previous_file is defined %}
     * _â__
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/references.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/references.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-file.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2` & `betty-0.3.4/betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/cotton_candy/gui.py` & `betty-0.3.4/betty/extension/cotton_candy/gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,101 @@
 """
 Provide Cotton Candy's Graphical User Interface.
 """
+
 from __future__ import annotations
 
 from typing import Any
 
 from PyQt6.QtCore import QRect
 from PyQt6.QtGui import QPainter, QBrush, QColor, QPaintEvent
-from PyQt6.QtWidgets import QVBoxLayout, QLabel, QPushButton, QColorDialog, QHBoxLayout, QFormLayout, QWidget
+from PyQt6.QtWidgets import (
+    QVBoxLayout,
+    QLabel,
+    QPushButton,
+    QColorDialog,
+    QHBoxLayout,
+    QFormLayout,
+    QWidget,
+)
 
 from betty.app import App
-from betty.extension import CottonCandy
+from betty.extension import CottonCandy, Webpack
 from betty.extension.cotton_candy import _ColorConfiguration, CottonCandyConfiguration
 from betty.gui.locale import LocalizedObject
 from betty.gui.model import EntityReferenceSequenceCollector
+from betty.gui.text import Caption
 from betty.locale import Str, Localizable
 
 
 class _ColorConfigurationSwatch(LocalizedObject, QWidget):
     def __init__(self, app: App, color: _ColorConfiguration, *args: Any, **kwargs: Any):
         super().__init__(app, *args, **kwargs)
         self._color = color
         self._color.on_change(self.repaint)
         self.setFixedHeight(24)
         self.setFixedWidth(24)
+        self._swatch = QRect(self.rect())
 
     def paintEvent(self, a0: QPaintEvent | None) -> None:
         painter = QPainter(self)
-        swatch = QRect(self.rect())
-        painter.fillRect(swatch, QBrush(QColor.fromString(self._color.hex)))
-        painter.drawRect(swatch)
+        painter.fillRect(self._swatch, QBrush(QColor.fromString(self._color.hex)))
+        painter.drawRect(self._swatch)
 
 
 class _ColorConfigurationWidget(LocalizedObject, QWidget):
-    def __init__(self, app: App, color: _ColorConfiguration, color_default: str, *args: Any, **kwargs: Any):
+    def __init__(
+        self,
+        app: App,
+        color: _ColorConfiguration,
+        color_default: str,
+        *args: Any,
+        **kwargs: Any,
+    ):
         super().__init__(app, *args, **kwargs)
         self._color = color
         self._color_default = color_default
         self._layout = QHBoxLayout()
         self.setLayout(self._layout)
 
         self._label = QLabel()
         self._layout.addWidget(self._label)
         self._swatch = _ColorConfigurationSwatch(app, self._color)
         self._layout.addWidget(self._swatch)
         self._configure = QPushButton()
         self._layout.addWidget(self._configure)
 
         def _configure() -> None:
-            qcolor = QColorDialog.getColor(
-                initial=QColor.fromString(self._color.hex)
-            )
+            qcolor = QColorDialog.getColor(initial=QColor.fromString(self._color.hex))
             if qcolor.isValid():
                 self._color.hex = qcolor.name()
+
         self._configure.clicked.connect(_configure)
         self._reset = QPushButton()
         self._layout.addWidget(self._reset)
 
         def _reset() -> None:
             self._color.hex = self._color_default
 
         self._reset.clicked.connect(_reset)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._configure.setText(self._app.localizer._('Configure'))
-        self._reset.setText(self._app.localizer._('Reset'))
+        self._configure.setText(self._app.localizer._("Configure"))
+        self._reset.setText(self._app.localizer._("Reset"))
 
 
 class _ColorConfigurationsWidget(LocalizedObject, QWidget):
-    def __init__(self, app: App, colors: list[tuple[_ColorConfiguration, Localizable, str]], *args: Any, **kwargs: Any):
+    def __init__(
+        self,
+        app: App,
+        colors: list[tuple[_ColorConfiguration, Localizable, str]],
+        *args: Any,
+        **kwargs: Any,
+    ):
         super().__init__(app, *args, **kwargs)
         self._colors = colors
         self._color_configurations = []
         self._color_labels = []
         self._layout = QFormLayout()
         self.setLayout(self._layout)
 
@@ -94,40 +116,54 @@
     def __init__(self, app: App, *args: Any, **kwargs: Any):
         super().__init__(app, *args, **kwargs)
         self._app = app
 
         self._layout = QVBoxLayout()
         self.setLayout(self._layout)
 
-        self._color_configurations_widget = _ColorConfigurationsWidget(app, [
-            (
-                app.extensions[CottonCandy].configuration.primary_inactive_color,
-                Str._('Primary color (inactive)'),
-                CottonCandyConfiguration.DEFAULT_PRIMARY_INACTIVE_COLOR,
-            ),
-            (
-                app.extensions[CottonCandy].configuration.primary_active_color,
-                Str._('Primary color (active)'),
-                CottonCandyConfiguration.DEFAULT_PRIMARY_ACTIVE_COLOR,
-            ),
-            (
-                app.extensions[CottonCandy].configuration.link_inactive_color,
-                Str._('Link color (inactive)'),
-                CottonCandyConfiguration.DEFAULT_LINK_INACTIVE_COLOR,
-            ),
-            (
-                app.extensions[CottonCandy].configuration.link_active_color,
-                Str._('Link color (active)'),
-                CottonCandyConfiguration.DEFAULT_LINK_ACTIVE_COLOR,
-            ),
-        ])
+        self._color_configurations_widget = _ColorConfigurationsWidget(
+            app,
+            [
+                (
+                    app.extensions[CottonCandy].configuration.primary_inactive_color,
+                    Str._("Primary color (inactive)"),
+                    CottonCandyConfiguration.DEFAULT_PRIMARY_INACTIVE_COLOR,
+                ),
+                (
+                    app.extensions[CottonCandy].configuration.primary_active_color,
+                    Str._("Primary color (active)"),
+                    CottonCandyConfiguration.DEFAULT_PRIMARY_ACTIVE_COLOR,
+                ),
+                (
+                    app.extensions[CottonCandy].configuration.link_inactive_color,
+                    Str._("Link color (inactive)"),
+                    CottonCandyConfiguration.DEFAULT_LINK_INACTIVE_COLOR,
+                ),
+                (
+                    app.extensions[CottonCandy].configuration.link_active_color,
+                    Str._("Link color (active)"),
+                    CottonCandyConfiguration.DEFAULT_LINK_ACTIVE_COLOR,
+                ),
+            ],
+        )
         self._layout.addWidget(self._color_configurations_widget)
+        self._color_configurations_widget_caption = Caption()
+        self._layout.addWidget(self._color_configurations_widget_caption)
+        if not self._app.extensions[Webpack].build_requirement().is_met():
+            self._color_configurations_widget.setDisabled(True)
+            self._color_configurations_widget_caption.setText(
+                self._app.extensions[Webpack]
+                .build_requirement()
+                .localize(self._app.localizer)
+            )
 
         self._featured_entities_label = QLabel()
         self._layout.addWidget(self._featured_entities_label)
-        self._featured_entities_entity_references_collector = EntityReferenceSequenceCollector(
-            self._app,
-            self._app.extensions[CottonCandy].configuration.featured_entities,
-            Str._('Featured entities'),
-            Str._("These entities are featured on your site's front page."),
+        self._featured_entities_entity_references_collector = (
+            EntityReferenceSequenceCollector(
+                self._app,
+                self._app.extensions[CottonCandy].configuration.featured_entities,
+                Str._("Featured entities"),
+                Str._("These entities are featured on your site's front page."),
+            )
         )
         self._layout.addWidget(self._featured_entities_entity_references_collector)
```

### Comparing `betty-0.3.3/betty/extension/cotton_candy/search.py` & `betty-0.3.4/betty/extension/cotton_candy/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide Cotton Candy's search functionality.
 """
+
 from __future__ import annotations
 
 from collections.abc import AsyncIterable
 from typing import Any
 
 from betty.app import App
 from betty.locale import Localizer
@@ -49,52 +50,56 @@
         for file in self._app.project.ancestry[File]:
             entry = await self._build_file(file)
             if entry is not None:
                 yield entry
 
     async def _render_entity(self, entity: Entity) -> str:
         entity_type_name = get_entity_type_name(entity)
-        return await self._app.jinja2_environment.select_template([
-            f'search/result-{camel_case_to_snake_case(entity_type_name)}.html.j2',
-            'search/result.html.j2',
-        ]).render_async({
-            'job_context': self._job_context,
-            'localizer': self._localizer,
-            'entity': entity,
-        })
+        return await self._app.jinja2_environment.select_template(
+            [
+                f"search/result-{camel_case_to_snake_case(entity_type_name)}.html.j2",
+                "search/result.html.j2",
+            ]
+        ).render_async(
+            {
+                "job_context": self._job_context,
+                "localizer": self._localizer,
+                "entity": entity,
+            }
+        )
 
     async def _build_person(self, person: Person) -> dict[Any, Any] | None:
         if person.private:
             return None
 
         names = []
         for name in person.names:
             if name.individual is not None:
                 names.append(name.individual.lower())
             if name.affiliation is not None:
                 names.append(name.affiliation.lower())
         if not names:
             return None
         return {
-            'text': ' '.join(names),
-            'result': await self._render_entity(person),
+            "text": " ".join(names),
+            "result": await self._render_entity(person),
         }
 
     async def _build_place(self, place: Place) -> dict[Any, Any] | None:
         if place.private:
             return None
 
         return {
-            'text': ' '.join(map(lambda x: x.name.lower(), place.names)),
-            'result': await self._render_entity(place),
+            "text": " ".join(map(lambda x: x.name.lower(), place.names)),
+            "result": await self._render_entity(place),
         }
 
     async def _build_file(self, file: File) -> dict[Any, Any] | None:
         if file.private:
             return None
 
         if not file.description:
             return None
         return {
-            'text': file.description.lower(),
-            'result': await self._render_entity(file),
+            "text": file.description.lower(),
+            "result": await self._render_entity(file),
         }
```

### Comparing `betty-0.3.3/betty/extension/demo/__init__.py` & `betty-0.3.4/betty/extension/demo/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,50 @@
 """Provide demonstration site functionality."""
+
 from __future__ import annotations
 
 from contextlib import AsyncExitStack
 
 from betty import load, generate, serve
 from betty.app import App
 from betty.app.extension import Extension
 from betty.extension.cotton_candy import CottonCandyConfiguration
 from betty.load import Loader
 from betty.locale import Date, DateRange, Str, DEFAULT_LOCALIZER
 from betty.model import Entity
-from betty.model.ancestry import Place, PlaceName, Person, Presence, Subject, PersonName, Link, Source, Citation, Event, \
-    Enclosure, Note
+from betty.model.ancestry import (
+    Place,
+    PlaceName,
+    Person,
+    Presence,
+    Subject,
+    PersonName,
+    Link,
+    Source,
+    Citation,
+    Event,
+    Enclosure,
+    Note,
+)
 from betty.model.event_type import Marriage, Birth, Death
-from betty.project import LocaleConfiguration, ExtensionConfiguration, EntityReference, Project
+from betty.project import (
+    LocaleConfiguration,
+    ExtensionConfiguration,
+    EntityReference,
+    Project,
+)
 from betty.serve import Server, NoPublicUrlBecauseServerNotStartedError
 from betty.warnings import deprecate
 
 
-class _Demo(Extension, Loader):
+class Demo(Extension, Loader):
+    @classmethod
+    def name(cls) -> str:
+        return "betty.extension.Demo"
+
     @classmethod
     def depends_on(cls) -> set[type[Extension]]:
         from betty.extension import CottonCandy, HttpApiDoc, Maps, Trees, Wikipedia
 
         return {CottonCandy, HttpApiDoc, Maps, Trees, Wikipedia}
 
     def _load(self, *entities: Entity) -> None:
@@ -31,381 +53,424 @@
     @classmethod
     def project(cls) -> Project:
         from betty.extension import CottonCandy, Demo
 
         project = Project()
         project.configuration.name = cls.name()
         project.configuration.extensions.append(ExtensionConfiguration(Demo))
-        project.configuration.extensions.append(ExtensionConfiguration(
-            CottonCandy,
-            extension_configuration=CottonCandyConfiguration(
-                featured_entities=[
-                    EntityReference(Place, 'betty-demo-amsterdam'),
-                    EntityReference(Person, 'betty-demo-liberta-lankester'),
-                    EntityReference(Place, 'betty-demo-netherlands'),
-                ],
-            ),
-        ))
+        project.configuration.extensions.append(
+            ExtensionConfiguration(
+                CottonCandy,
+                extension_configuration=CottonCandyConfiguration(
+                    featured_entities=[
+                        EntityReference(Place, "betty-demo-amsterdam"),
+                        EntityReference(Person, "betty-demo-liberta-lankester"),
+                        EntityReference(Place, "betty-demo-netherlands"),
+                    ],
+                ),
+            )
+        )
         # Include all of the translations Betty ships with.
         project.configuration.locales.replace(
             LocaleConfiguration(
-                'en-US',
-                alias='en',
+                "en-US",
+                alias="en",
             ),
             LocaleConfiguration(
-                'nl-NL',
-                alias='nl',
+                "nl-NL",
+                alias="nl",
             ),
             LocaleConfiguration(
-                'fr-FR',
-                alias='fr',
+                "fr-FR",
+                alias="fr",
             ),
             LocaleConfiguration(
-                'uk',
-                alias='uk',
+                "uk",
+                alias="uk",
             ),
             LocaleConfiguration(
-                'de-DE',
-                alias='de',
+                "de-DE",
+                alias="de",
             ),
         )
         return project
 
     async def load(self) -> None:
         netherlands = Place(
-            id='betty-demo-netherlands',
+            id="betty-demo-netherlands",
             names=[
-                PlaceName(name='Netherlands'),
+                PlaceName(name="Netherlands"),
                 PlaceName(
-                    name='Nederland',
-                    locale='nl',
+                    name="Nederland",
+                    locale="nl",
                 ),
                 PlaceName(
-                    name='Нідерланди',
-                    locale='uk',
+                    name="Нідерланди",
+                    locale="uk",
                 ),
                 PlaceName(
-                    name='Pays-Bas',
-                    locale='fr',
+                    name="Pays-Bas",
+                    locale="fr",
                 ),
             ],
-            links=[Link('https://en.wikipedia.org/wiki/Netherlands')],
+            links=[Link("https://en.wikipedia.org/wiki/Netherlands")],
         )
         self._load(netherlands)
 
         north_holland = Place(
-            id='betty-demo-north-holland',
+            id="betty-demo-north-holland",
             names=[
-                PlaceName(name='North Holland'),
+                PlaceName(name="North Holland"),
                 PlaceName(
-                    name='Noord-Holland',
-                    locale='nl',
+                    name="Noord-Holland",
+                    locale="nl",
                 ),
                 PlaceName(
-                    name='Північна Голландія',
-                    locale='uk',
+                    name="Північна Голландія",
+                    locale="uk",
                 ),
                 PlaceName(
-                    name='Hollande-Septentrionale',
-                    locale='fr',
+                    name="Hollande-Septentrionale",
+                    locale="fr",
                 ),
             ],
-            links=[Link('https://en.wikipedia.org/wiki/North_Holland')],
+            links=[Link("https://en.wikipedia.org/wiki/North_Holland")],
         )
         self._load(Enclosure(encloses=north_holland, enclosed_by=netherlands))
         self._load(north_holland)
 
-        amsterdam_note = Note("""
+        amsterdam_note = Note(
+            """
 Did you know that while Amsterdam is the country's official capital, The Hague is the Netherlands' administrative center and seat of government?
-        """)
+        """
+        )
 
         amsterdam = Place(
-            id='betty-demo-amsterdam',
+            id="betty-demo-amsterdam",
             names=[
-                PlaceName(name='Amsterdam'),
+                PlaceName(name="Amsterdam"),
                 PlaceName(
-                    name='Амстерда́м',
-                    locale='uk',
+                    name="Амстерда́м",
+                    locale="uk",
                 ),
             ],
-            links=[Link('https://nl.wikipedia.org/wiki/Amsterdam')],
+            links=[Link("https://nl.wikipedia.org/wiki/Amsterdam")],
             notes=[amsterdam_note],
         )
         self._load(Enclosure(encloses=amsterdam, enclosed_by=north_holland))
         self._load(amsterdam)
 
         ilpendam = Place(
-            id='betty-demo-ilpendam',
+            id="betty-demo-ilpendam",
             names=[
-                PlaceName(name='Ilpendam'),
+                PlaceName(name="Ilpendam"),
                 PlaceName(
-                    name='Илпендам',
-                    locale='uk',
+                    name="Илпендам",
+                    locale="uk",
                 ),
             ],
-            links=[Link('https://nl.wikipedia.org/wiki/Ilpendam')],
+            links=[Link("https://nl.wikipedia.org/wiki/Ilpendam")],
         )
         self._load(Enclosure(encloses=ilpendam, enclosed_by=north_holland))
         self._load(ilpendam)
 
         personal_accounts = Source(
-            id='betty-demo-personal-accounts',
-            name='Personal accounts',
+            id="betty-demo-personal-accounts",
+            name="Personal accounts",
         )
         self._load(personal_accounts)
 
         cite_first_person_account = Citation(
-            id='betty-demo-first-person-account',
+            id="betty-demo-first-person-account",
             source=personal_accounts,
         )
         self._load(cite_first_person_account)
 
         bevolkingsregister_amsterdam = Source(
-            id='betty-demo-bevolkingsregister-amsterdam',
-            name='Bevolkingsregister Amsterdam',
-            author='Gemeente Amsterdam',
-            publisher='Gemeente Amsterdam',
+            id="betty-demo-bevolkingsregister-amsterdam",
+            name="Bevolkingsregister Amsterdam",
+            author="Gemeente Amsterdam",
+            publisher="Gemeente Amsterdam",
         )
         self._load(bevolkingsregister_amsterdam)
 
-        david_marinus_lankester = Person(id='betty-demo-david-marinus-lankester')
+        david_marinus_lankester = Person(id="betty-demo-david-marinus-lankester")
         self._load(
             PersonName(
                 person=david_marinus_lankester,
-                individual='David Marinus',
-                affiliation='Lankester',
+                individual="David Marinus",
+                affiliation="Lankester",
             ),
             david_marinus_lankester,
         )
 
-        geertruida_van_ling = Person(id='betty-demo-geertruida-van-ling')
+        geertruida_van_ling = Person(id="betty-demo-geertruida-van-ling")
         self._load(
             PersonName(
                 person=geertruida_van_ling,
-                individual='Geertruida',
-                affiliation='Van Ling',
+                individual="Geertruida",
+                affiliation="Van Ling",
             ),
             geertruida_van_ling,
         )
 
         marriage_of_dirk_jacobus_lankester_and_jannigje_palsen = Event(
-            id='betty-demo-marriage-of-dirk-jacobus-lankester-and-jannigje-palsen',
+            id="betty-demo-marriage-of-dirk-jacobus-lankester-and-jannigje-palsen",
             event_type=Marriage,
             date=Date(1922, 7, 4),
             place=ilpendam,
         )
         self._load(marriage_of_dirk_jacobus_lankester_and_jannigje_palsen)
 
         birth_of_dirk_jacobus_lankester = Event(
-            id='betty-demo-birth-of-dirk-jacobus-lankester',
+            id="betty-demo-birth-of-dirk-jacobus-lankester",
             event_type=Birth,
             date=Date(1897, 8, 25),
             place=amsterdam,
         )
         self._load(birth_of_dirk_jacobus_lankester)
 
         death_of_dirk_jacobus_lankester = Event(
-            id='betty-demo-death-of-dirk-jacobus-lankester',
+            id="betty-demo-death-of-dirk-jacobus-lankester",
             event_type=Death,
             date=Date(1986, 8, 18),
             place=amsterdam,
         )
         self._load(death_of_dirk_jacobus_lankester)
 
         dirk_jacobus_lankester = Person(
-            id='betty-demo-dirk-jacobus-lankester',
-            parents=(david_marinus_lankester, geertruida_van_ling)
+            id="betty-demo-dirk-jacobus-lankester",
+            parents=(david_marinus_lankester, geertruida_van_ling),
         )
         self._load(
             PersonName(
                 person=dirk_jacobus_lankester,
-                individual='Dirk Jacobus',
-                affiliation='Lankester',
+                individual="Dirk Jacobus",
+                affiliation="Lankester",
+            ),
+            Presence(
+                dirk_jacobus_lankester, Subject(), birth_of_dirk_jacobus_lankester
+            ),
+            Presence(
+                dirk_jacobus_lankester, Subject(), death_of_dirk_jacobus_lankester
+            ),
+            Presence(
+                dirk_jacobus_lankester,
+                Subject(),
+                marriage_of_dirk_jacobus_lankester_and_jannigje_palsen,
             ),
-            Presence(dirk_jacobus_lankester, Subject(), birth_of_dirk_jacobus_lankester),
-            Presence(dirk_jacobus_lankester, Subject(), death_of_dirk_jacobus_lankester),
-            Presence(dirk_jacobus_lankester, Subject(), marriage_of_dirk_jacobus_lankester_and_jannigje_palsen),
         )
         self._load(dirk_jacobus_lankester)
 
         birth_of_marinus_david_lankester = Event(
-            id='betty-demo-birth-of-marinus-david',
+            id="betty-demo-birth-of-marinus-david",
             event_type=Birth,
-            date=DateRange(Date(1874, 1, 15), Date(1874, 3, 21), start_is_boundary=True, end_is_boundary=True),
+            date=DateRange(
+                Date(1874, 1, 15),
+                Date(1874, 3, 21),
+                start_is_boundary=True,
+                end_is_boundary=True,
+            ),
             place=amsterdam,
         )
         self._load(birth_of_marinus_david_lankester)
 
         death_of_marinus_david_lankester = Event(
-            id='betty-demo-death-of-marinus-david',
+            id="betty-demo-death-of-marinus-david",
             event_type=Death,
             date=Date(1971),
             place=amsterdam,
         )
         self._load(death_of_marinus_david_lankester)
 
         marinus_david_lankester = Person(
-            id='betty-demo-marinus-david-lankester',
+            id="betty-demo-marinus-david-lankester",
             parents=(david_marinus_lankester, geertruida_van_ling),
         )
         self._load(
             PersonName(
                 person=marinus_david_lankester,
-                individual='Marinus David',
-                affiliation='Lankester',
+                individual="Marinus David",
+                affiliation="Lankester",
+            ),
+            Presence(
+                marinus_david_lankester, Subject(), birth_of_marinus_david_lankester
+            ),
+            Presence(
+                marinus_david_lankester, Subject(), death_of_marinus_david_lankester
             ),
-            Presence(marinus_david_lankester, Subject(), birth_of_marinus_david_lankester),
-            Presence(marinus_david_lankester, Subject(), death_of_marinus_david_lankester),
         )
         self._load(marinus_david_lankester)
 
         birth_of_jacoba_gesina_lankester = Event(
-            id='betty-demo-birth-of-jacoba-gesina',
+            id="betty-demo-birth-of-jacoba-gesina",
             event_type=Birth,
             date=Date(1900, 3, 14),
             place=amsterdam,
         )
         self._load(birth_of_jacoba_gesina_lankester)
 
         jacoba_gesina_lankester = Person(
-            id='betty-demo-jacoba-gesina-lankester',
+            id="betty-demo-jacoba-gesina-lankester",
             parents=(david_marinus_lankester, geertruida_van_ling),
         )
         self._load(
             PersonName(
                 person=jacoba_gesina_lankester,
-                individual='Jacoba Gesina',
-                affiliation='Lankester',
+                individual="Jacoba Gesina",
+                affiliation="Lankester",
+            ),
+            Presence(
+                jacoba_gesina_lankester, Subject(), birth_of_jacoba_gesina_lankester
             ),
-            Presence(jacoba_gesina_lankester, Subject(), birth_of_jacoba_gesina_lankester),
         )
         self._load(jacoba_gesina_lankester)
 
-        jannigje_palsen = Person(id='betty-demo-jannigje-palsen')
+        jannigje_palsen = Person(id="betty-demo-jannigje-palsen")
         self._load(
             PersonName(
                 person=jannigje_palsen,
-                individual='Jannigje',
-                affiliation='Palsen',
+                individual="Jannigje",
+                affiliation="Palsen",
+            ),
+            Presence(
+                jannigje_palsen,
+                Subject(),
+                marriage_of_dirk_jacobus_lankester_and_jannigje_palsen,
             ),
-            Presence(jannigje_palsen, Subject(), marriage_of_dirk_jacobus_lankester_and_jannigje_palsen),
             jannigje_palsen,
         )
 
         marriage_of_johan_de_boer_and_liberta_lankester = Event(
-            id='betty-demo-marriage-of-johan-de-boer-and-liberta-lankester',
+            id="betty-demo-marriage-of-johan-de-boer-and-liberta-lankester",
             event_type=Marriage,
             date=Date(1953, 6, 19),
             place=amsterdam,
         )
         self._load(marriage_of_johan_de_boer_and_liberta_lankester)
 
         cite_birth_of_liberta_lankester_from_bevolkingsregister_amsterdam = Citation(
-            id='betty-demo-birth-of-liberta-lankester-from-bevolkingsregister-amsterdam',
+            id="betty-demo-birth-of-liberta-lankester-from-bevolkingsregister-amsterdam",
             source=bevolkingsregister_amsterdam,
-            location=Str.plain('Amsterdam'),
+            location=Str.plain("Amsterdam"),
         )
         self._load(cite_birth_of_liberta_lankester_from_bevolkingsregister_amsterdam)
 
         birth_of_liberta_lankester = Event(
-            id='betty-demo-birth-of-liberta-lankester',
+            id="betty-demo-birth-of-liberta-lankester",
             event_type=Birth,
             date=Date(1929, 12, 22),
             place=amsterdam,
-            citations=[cite_birth_of_liberta_lankester_from_bevolkingsregister_amsterdam],
+            citations=[
+                cite_birth_of_liberta_lankester_from_bevolkingsregister_amsterdam
+            ],
         )
         self._load(birth_of_liberta_lankester)
 
         death_of_liberta_lankester = Event(
-            id='betty-demo-death-of-liberta-lankester',
+            id="betty-demo-death-of-liberta-lankester",
             event_type=Death,
             date=Date(2015, 1, 17),
             place=amsterdam,
             citations=[cite_first_person_account],
         )
         self._load(death_of_liberta_lankester)
 
-        liberta_lankester_note = Note("""
+        liberta_lankester_note = Note(
+            """
 Did you know that Liberta "Betty" Lankester is Betty's namesake?
-        """)
+        """
+        )
 
         liberta_lankester = Person(
-            id='betty-demo-liberta-lankester',
+            id="betty-demo-liberta-lankester",
             parents=(dirk_jacobus_lankester, jannigje_palsen),
             notes=[liberta_lankester_note],
         )
         self._load(
             PersonName(
                 person=liberta_lankester,
-                individual='Liberta',
-                affiliation='Lankester',
+                individual="Liberta",
+                affiliation="Lankester",
             ),
             PersonName(
                 person=liberta_lankester,
-                individual='Betty',
+                individual="Betty",
             ),
             Presence(liberta_lankester, Subject(), birth_of_liberta_lankester),
             Presence(liberta_lankester, Subject(), death_of_liberta_lankester),
-            Presence(liberta_lankester, Subject(), marriage_of_johan_de_boer_and_liberta_lankester),
+            Presence(
+                liberta_lankester,
+                Subject(),
+                marriage_of_johan_de_boer_and_liberta_lankester,
+            ),
         )
         self._load(liberta_lankester)
 
         birth_of_johan_de_boer = Event(
-            id='betty-demo-birth-of-johan-de-boer',
+            id="betty-demo-birth-of-johan-de-boer",
             event_type=Birth,
             date=Date(1930, 6, 20),
             place=amsterdam,
         )
         self._load(birth_of_johan_de_boer)
 
         death_of_johan_de_boer = Event(
-            id='betty-demo-death-of-johan-de-boer',
+            id="betty-demo-death-of-johan-de-boer",
             event_type=Death,
             date=Date(1999, 3, 10),
             place=amsterdam,
             citations=[cite_first_person_account],
         )
         self._load(death_of_johan_de_boer)
 
-        johan_de_boer = Person(id='betty-demo-johan-de-boer')
+        johan_de_boer = Person(id="betty-demo-johan-de-boer")
         self._load(
             PersonName(
                 person=johan_de_boer,
-                individual='Johan',
-                affiliation='De Boer',
+                individual="Johan",
+                affiliation="De Boer",
             ),
             PersonName(
                 person=johan_de_boer,
-                individual='Hans',
+                individual="Hans",
             ),
             Presence(johan_de_boer, Subject(), birth_of_johan_de_boer),
             Presence(johan_de_boer, Subject(), death_of_johan_de_boer),
-            Presence(johan_de_boer, Subject(), marriage_of_johan_de_boer_and_liberta_lankester),
+            Presence(
+                johan_de_boer,
+                Subject(),
+                marriage_of_johan_de_boer_and_liberta_lankester,
+            ),
             johan_de_boer,
         )
 
         parent_of_bart_feenstra_child_of_liberta_lankester = Person(
-            id='betty-demo-parent-of-bart-feenstra-child-of-liberta-lankester',
+            id="betty-demo-parent-of-bart-feenstra-child-of-liberta-lankester",
             parents=(johan_de_boer, liberta_lankester),
         )
-        self._load(PersonName(
-            person=parent_of_bart_feenstra_child_of_liberta_lankester,
-            individual='Bart\'s parent',
-        ))
+        self._load(
+            PersonName(
+                person=parent_of_bart_feenstra_child_of_liberta_lankester,
+                individual="Bart's parent",
+            )
+        )
         self._load(parent_of_bart_feenstra_child_of_liberta_lankester)
 
         bart_feenstra = Person(
-            id='betty-demo-bart-feenstra',
+            id="betty-demo-bart-feenstra",
             parents=(parent_of_bart_feenstra_child_of_liberta_lankester,),
         )
-        self._load(PersonName(
-            person=bart_feenstra,
-            individual='Bart',
-            affiliation='Feenstra',
-        ))
+        self._load(
+            PersonName(
+                person=bart_feenstra,
+                individual="Bart",
+                affiliation="Feenstra",
+            )
+        )
         self._load(bart_feenstra)
 
 
 class DemoServer(Server):
     def __init__(
         self,
         *,
@@ -413,21 +478,21 @@
     ):
         super().__init__(localizer=DEFAULT_LOCALIZER)
         self._app = app
         self._server: Server | None = None
         self._exit_stack = AsyncExitStack()
         if app is None:
             deprecate(
-                f'Initializing {type(self)} with a project ID is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, set {type(self)}.configuration.name.',
+                f"Initializing {type(self)} with a project ID is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, set {type(self)}.configuration.name.",
                 stacklevel=2,
             )
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Demo')
+        return Str._("Demo")
 
     @property
     def public_url(self) -> str:
         if self._server is not None:
             return self._server.public_url
         raise NoPublicUrlBecauseServerNotStartedError()
 
@@ -442,15 +507,17 @@
             )
         else:
             isolated_app_factory = App.new_from_app(
                 self._app,
                 project=project,
             )
         try:
-            isolated_app = await self._exit_stack.enter_async_context(isolated_app_factory)
+            isolated_app = await self._exit_stack.enter_async_context(
+                isolated_app_factory
+            )
             await self._exit_stack.enter_async_context(isolated_app)
             self._localizer = isolated_app.localizer
             await load.load(isolated_app)
             self._server = serve.BuiltinAppServer(isolated_app)
             await self._exit_stack.enter_async_context(self._server)
             isolated_app.project.configuration.base_url = self._server.public_url
             await generate.generate(isolated_app)
```

### Comparing `betty-0.3.3/betty/extension/deriver/__init__.py` & `betty-0.3.4/betty/extension/deriver/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 """Expand an ancestry by deriving additional data from existing data."""
+
 from __future__ import annotations
 
 from logging import getLogger
 
 from betty.app.extension import Extension, UserFacingExtension
-from betty.deriver import Deriver
+from betty.deriver import Deriver as DeriverApi
 from betty.load import PostLoader
 from betty.locale import Str
 from betty.model.event_type import DerivableEventType
 
 
-class _Deriver(UserFacingExtension, PostLoader):
+class Deriver(UserFacingExtension, PostLoader):
+    @classmethod
+    def name(cls) -> str:
+        return "betty.extension.Deriver"
+
     async def post_load(self) -> None:
         logger = getLogger(__name__)
-        logger.info(self._app.localizer._('Deriving...'))
+        logger.info(self._app.localizer._("Deriving..."))
 
-        deriver = Deriver(
+        deriver = DeriverApi(
             self.app.project.ancestry,
             self.app.project.configuration.lifetime_threshold,
             {
                 event_type
-                for event_type
-                in self.app.event_types
+                for event_type in self.app.event_types
                 if issubclass(event_type, DerivableEventType)
             },
             localizer=self._app.localizer,
         )
         await deriver.derive()
 
     @classmethod
     def comes_before(cls) -> set[type[Extension]]:
         from betty.extension import Privatizer
 
         return {Privatizer}
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Deriver')
+        return Str._("Deriver")
 
     @classmethod
     def description(cls) -> Str:
-        return Str._('Create events such as births and deaths by deriving their details from existing information.')
+        return Str._(
+            "Create events such as births and deaths by deriving their details from existing information."
+        )
```

### Comparing `betty-0.3.3/betty/extension/gramps/__init__.py` & `betty-0.3.4/betty/extension/gramps/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Integrate Betty with `Gramps <https://gramps-project.org>`_."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from betty.app.extension import ConfigurableExtension, UserFacingExtension
 from betty.gramps.loader import GrampsLoader
 from betty.locale import Str
@@ -11,15 +12,21 @@
     from betty.extension.gramps.gui import _GrampsGuiWidget
 
 from betty.extension.gramps.config import GrampsConfiguration
 from betty.gui import GuiBuilder
 from betty.load import Loader
 
 
-class _Gramps(ConfigurableExtension[GrampsConfiguration], UserFacingExtension, Loader, GuiBuilder):
+class Gramps(
+    ConfigurableExtension[GrampsConfiguration], UserFacingExtension, Loader, GuiBuilder
+):
+    @classmethod
+    def name(cls) -> str:
+        return "betty.extension.Gramps"
+
     @classmethod
     def default_configuration(cls) -> GrampsConfiguration:
         return GrampsConfiguration()
 
     async def load(self) -> None:
         for family_tree in self.configuration.family_trees:
             file_path = family_tree.file_path
@@ -27,17 +34,19 @@
                 await GrampsLoader(
                     self._app.project,
                     localizer=self._app.localizer,
                 ).load_file(file_path)
 
     @classmethod
     def label(cls) -> Str:
-        return Str.plain('Gramps')
+        return Str.plain("Gramps")
 
     @classmethod
     def description(cls) -> Str:
-        return Str._('Load <a href="https://gramps-project.org/">Gramps</a> family trees.')
+        return Str._(
+            'Load <a href="https://gramps-project.org/">Gramps</a> family trees.'
+        )
 
     def gui_build(self) -> _GrampsGuiWidget:
         from betty.extension.gramps.gui import _GrampsGuiWidget
 
         return _GrampsGuiWidget(self._app)
```

### Comparing `betty-0.3.3/betty/extension/gramps/config.py` & `betty-0.3.4/betty/extension/gramps/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide configuration for the :py:class:`betty.extension.Gramps` extension.
 """
+
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Iterable, Any, Self
 
 from betty.config import Configuration, ConfigurationSequence
 from betty.serde.dump import minimize, Dump, VoidableDump
@@ -31,32 +32,35 @@
 
     @file_path.setter
     def file_path(self, file_path: Path | None) -> None:
         self._file_path = file_path
 
     @classmethod
     def load(
-            cls,
-            dump: Dump,
-            configuration: Self | None = None,
+        cls,
+        dump: Dump,
+        configuration: Self | None = None,
     ) -> Self:
         if configuration is None:
             configuration = cls()
         asserter = Asserter()
-        asserter.assert_record(Fields(
-            RequiredField(
-                'file',
-                Assertions(asserter.assert_path()) | asserter.assert_setattr(configuration, 'file_path'),
-            ),
-        ))(dump)
+        asserter.assert_record(
+            Fields(
+                RequiredField(
+                    "file",
+                    Assertions(asserter.assert_path())
+                    | asserter.assert_setattr(configuration, "file_path"),
+                ),
+            )
+        )(dump)
         return configuration
 
     def dump(self) -> VoidableDump:
         return {
-            'file': str(self.file_path),
+            "file": str(self.file_path),
         }
 
 
 class FamilyTreeConfigurationSequence(ConfigurationSequence[FamilyTreeConfiguration]):
     def update(self, other: Self) -> None:
         self._clear_without_dispatch()
         self.append(*other)
@@ -85,26 +89,35 @@
         return self._family_trees
 
     def update(self, other: Self) -> None:
         self._family_trees.update(other._family_trees)
 
     @classmethod
     def load(
-            cls,
-            dump: Dump,
-            configuration: Self | None = None,
+        cls,
+        dump: Dump,
+        configuration: Self | None = None,
     ) -> Self:
         if configuration is None:
             configuration = cls()
         asserter = Asserter()
-        asserter.assert_record(Fields(
-            OptionalField(
-                'family_trees',
-                Assertions(configuration._family_trees.assert_load(configuration.family_trees)),
-            ),
-        ))(dump)
+        asserter.assert_record(
+            Fields(
+                OptionalField(
+                    "family_trees",
+                    Assertions(
+                        configuration._family_trees.assert_load(
+                            configuration.family_trees
+                        )
+                    ),
+                ),
+            )
+        )(dump)
         return configuration
 
     def dump(self) -> VoidableDump:
-        return minimize({
-            'family_trees': self.family_trees.dump(),
-        }, True)
+        return minimize(
+            {
+                "family_trees": self.family_trees.dump(),
+            },
+            True,
+        )
```

### Comparing `betty-0.3.3/betty/extension/gramps/gui.py` & `betty-0.3.4/betty/extension/gramps/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 """
 Provide Gramps's Graphical User Interface.
 """
+
 from __future__ import annotations
 
 from contextlib import suppress
 from pathlib import Path
 from typing import Any
 
 from PyQt6.QtCore import Qt, QObject
-from PyQt6.QtWidgets import QWidget, QFormLayout, QPushButton, QFileDialog, QLineEdit, QHBoxLayout, QVBoxLayout, \
-    QGridLayout, QLabel
+from PyQt6.QtWidgets import (
+    QWidget,
+    QFormLayout,
+    QPushButton,
+    QFileDialog,
+    QLineEdit,
+    QHBoxLayout,
+    QVBoxLayout,
+    QGridLayout,
+    QLabel,
+)
 
 from betty.app import App
 from betty.extension import Gramps
 from betty.extension.gramps.config import FamilyTreeConfiguration
 from betty.gui import mark_valid, mark_invalid
 from betty.gui.error import ExceptionCatcher
 from betty.gui.locale import LocalizedObject
@@ -31,15 +41,17 @@
         self.setLayout(self._layout)
 
         self._family_trees_widget: QWidget
         self._family_trees_layout: QGridLayout
         self._family_trees_remove_buttons: list[QPushButton]
 
         self._build_family_trees()
-        self._app.extensions[Gramps].configuration.family_trees.on_change(self._build_family_trees)
+        self._app.extensions[Gramps].configuration.family_trees.on_change(
+            self._build_family_trees
+        )
 
         self._add_family_tree_button = QPushButton()
         self._add_family_tree_button.released.connect(self._add_family_tree)
         self._layout.addWidget(self._add_family_tree_button, 1)
 
     def _build_family_trees(self) -> None:
         with suppress(AttributeError):
@@ -47,28 +59,40 @@
             self._family_trees_widget.setParent(None)
         self._family_trees_widget = QWidget()
         self._family_trees_layout = QGridLayout()
         self._family_trees_remove_buttons = []
         self._family_trees_widget.setLayout(self._family_trees_layout)
         self._layout.addWidget(self._family_trees_widget)
 
-        for i, family_tree in enumerate(self._app.extensions[Gramps].configuration.family_trees):
-            def _remove_family_tree() -> None:
-                del self._app.extensions[Gramps].configuration.family_trees[i]
-            self._family_trees_layout.addWidget(Text(str(family_tree.file_path)), i, 0)
-            self._family_trees_remove_buttons.insert(i, QPushButton())
-            self._family_trees_remove_buttons[i].released.connect(_remove_family_tree)
-            self._family_trees_layout.addWidget(self._family_trees_remove_buttons[i], i, 1)
-        self._layout.insertWidget(0, self._family_trees_widget, alignment=Qt.AlignmentFlag.AlignTop)
+        for index, family_tree in enumerate(
+            self._app.extensions[Gramps].configuration.family_trees
+        ):
+            self._build_family_tree(family_tree, index)
+        self._layout.insertWidget(
+            0, self._family_trees_widget, alignment=Qt.AlignmentFlag.AlignTop
+        )
+
+    def _build_family_tree(
+        self, family_tree: FamilyTreeConfiguration, index: int
+    ) -> None:
+        def _remove_family_tree() -> None:
+            del self._app.extensions[Gramps].configuration.family_trees[index]
+
+        self._family_trees_layout.addWidget(Text(str(family_tree.file_path)), index, 0)
+        self._family_trees_remove_buttons.insert(index, QPushButton())
+        self._family_trees_remove_buttons[index].released.connect(_remove_family_tree)
+        self._family_trees_layout.addWidget(
+            self._family_trees_remove_buttons[index], index, 1
+        )
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._add_family_tree_button.setText(self._app.localizer._('Add a family tree'))
+        self._add_family_tree_button.setText(self._app.localizer._("Add a family tree"))
         for button in self._family_trees_remove_buttons:
-            button.setText(self._app.localizer._('Remove'))
+            button.setText(self._app.localizer._("Remove"))
 
     def _add_family_tree(self) -> None:
         window = _AddFamilyTreeWindow(self._app, parent=self)
         window.show()
 
 
 class _GrampsGuiWidget(LocalizedObject, QWidget):
@@ -108,52 +132,57 @@
             try:
                 self._family_tree.file_path = Path(file_path)
                 mark_valid(self._file_path)
                 self._save_and_close.setDisabled(False)
             except SerdeError as e:
                 mark_invalid(self._file_path, str(e))
                 self._save_and_close.setDisabled(True)
+
         self._file_path = QLineEdit()
         self._file_path.textChanged.connect(_update_configuration_file_path)
         file_path_layout = QHBoxLayout()
         file_path_layout.addWidget(self._file_path)
 
         def find_family_tree_file_path() -> None:
             with ExceptionCatcher(self):
                 found_family_tree_file_path, __ = QFileDialog.getOpenFileName(
                     self._widget,
-                    self._app.localizer._('Load the family tree from...'),
+                    self._app.localizer._("Load the family tree from..."),
                     directory=self._file_path.text(),
                 )
-                if '' != found_family_tree_file_path:
+                if "" != found_family_tree_file_path:
                     self._file_path.setText(found_family_tree_file_path)
-        self._file_path_find = QPushButton('...')
+
+        self._file_path_find = QPushButton("...")
         self._file_path_find.released.connect(find_family_tree_file_path)
         file_path_layout.addWidget(self._file_path_find)
         self._file_path_label = QLabel()
         self._layout.addRow(self._file_path_label, file_path_layout)
 
         buttons_layout = QHBoxLayout()
         self._layout.addRow(buttons_layout)
 
         def save_and_close_family_tree() -> None:
             with ExceptionCatcher(self):
-                self._app.extensions[Gramps].configuration.family_trees.append(self._family_tree)
+                self._app.extensions[Gramps].configuration.family_trees.append(
+                    self._family_tree
+                )
                 self.close()
+
         self._save_and_close = QPushButton()
         self._save_and_close.setDisabled(True)
         self._save_and_close.released.connect(save_and_close_family_tree)
         buttons_layout.addWidget(self._save_and_close)
 
         self._cancel = QPushButton()
         self._cancel.released.connect(self.close)
         buttons_layout.addWidget(self._cancel)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._file_path_label.setText(self._app.localizer._('File path'))
-        self._save_and_close.setText(self._app.localizer._('Save and close'))
-        self._cancel.setText(self._app.localizer._('Cancel'))
+        self._file_path_label.setText(self._app.localizer._("File path"))
+        self._save_and_close.setText(self._app.localizer._("Save and close"))
+        self._cancel.setText(self._app.localizer._("Cancel"))
 
     @property
     def window_title(self) -> Localizable:
-        return Str._('Add a family tree')
+        return Str._("Add a family tree")
```

### Comparing `betty-0.3.3/betty/extension/http_api_doc/assets/public/static/api/index.html.j2` & `betty-0.3.4/betty/extension/http_api_doc/assets/public/static/api/index.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -10,10 +10,10 @@
             margin: 0;
             padding: 0;
         }
     </style>
 </head>
 <body>
 <redoc spec-url='{{ '/api/index.json' | static_url }}'></redoc>
-<script src="/http-api-doc.js"></script>
+<script src="/js/http-api-doc.js"></script>
 </body>
 </html>
```

### Comparing `betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.js` & `betty-0.3.4/betty/extension/maps/webpack/maps.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,36 @@
 'use strict'
 
-import mapsStyle from './maps.css' // eslint-disable-line no-unused-vars
+import './main.css'
 
 import * as L from 'leaflet'
-import leafletStyle from 'leaflet/dist/leaflet.css' // eslint-disable-line no-unused-vars
+import 'leaflet/dist/leaflet.css'
 import leafletMarkerIconImage from 'leaflet/dist/images/marker-icon.png'
 import leafletMarkerIcon2xImage from 'leaflet/dist/images/marker-icon-2x.png'
 import leafletMarkerShadowImage from 'leaflet/dist/images/marker-shadow.png'
 import {
     GestureHandling
 } from 'leaflet-gesture-handling'
 import 'leaflet.markercluster/dist/leaflet.markercluster.js'
-import 'leaflet.markercluster/dist/MarkerCluster.css' // eslint-disable-line no-unused-vars
-import 'leaflet.markercluster/dist/MarkerCluster.Default.css' // eslint-disable-line no-unused-vars
+import 'leaflet.markercluster/dist/MarkerCluster.css'
+import 'leaflet.markercluster/dist/MarkerCluster.Default.css'
 import 'leaflet.fullscreen/Control.FullScreen.js'
-import 'leaflet.fullscreen/Control.FullScreen.css' // eslint-disable-line no-unused-vars
-import 'leaflet-gesture-handling/dist/leaflet-gesture-handling.css' // eslint-disable-line no-unused-vars
+import 'leaflet.fullscreen/Control.FullScreen.css'
+import 'leaflet-gesture-handling/dist/leaflet-gesture-handling.css'
 
 L.Map.addInitHook('addHandler', 'gestureHandling', GestureHandling)
 
 let mapCount = 0
 
-function initializePlaceLists() {
+async function initializePlaceLists() {
     const placeLists = document.getElementsByClassName('places')
-    for (const placeList of placeLists) {
-        initializePlaceList(placeList)
-    }
+    await Promise.allSettled(Array.from(placeLists).map(placeList => initializePlaceList(placeList)))
 }
 
-function initializePlaceList(placeList) {
+async function initializePlaceList(placeList) {
     const mapArea = placeList.getElementsByClassName('map')[0]
     mapArea.id = (++mapCount).toString()
 
     const map = L.map(mapArea.id, {
         gestureHandling: true,
         fullscreenControl: true,
         fullscreenControlOptions: {
@@ -46,37 +44,35 @@
     }).addTo(map)
 
     // Build place markers.
     const markerGroup = L.markerClusterGroup({
         showCoverageOnHover: false
     })
     map.addLayer(markerGroup)
-    Promise.all(Array.from(placeList.querySelectorAll('[data-betty-place]')).map((placeDatum) => {
-            return fetch(placeDatum.dataset.bettyPlace)
-                .then((response) => response.json())
-                .then((place) => {
-                    if (!place.coordinates) {
-                        return
-                    }
-                    const marker = L.marker([place.coordinates.latitude, place.coordinates.longitude], {
-                        icon: new BettyIcon()
-                    })
-                    marker.bindPopup(placeDatum.innerHTML)
-                    markerGroup.addLayer(marker)
-                })
-        }))
-        .then(() => {
-            map.fitBounds(markerGroup.getBounds(), {
-                maxZoom: 9
-            })
+    await Promise.all(Array.from(placeList.querySelectorAll('[data-betty-place]')).map(async (placeDatum) => {
+        const response = await fetch(placeDatum.dataset.bettyPlace)
+        const place = await response.json()
+        if (!place.coordinates) {
+            return
+        }
+        const marker = L.marker([place.coordinates.latitude, place.coordinates.longitude], {
+            icon: new BettyIcon()
         })
+        marker.bindPopup(placeDatum.innerHTML)
+        markerGroup.addLayer(marker)
+    }))
+    map.fitBounds(markerGroup.getBounds(), {
+        maxZoom: 9
+    })
 }
 
 const BettyIcon = L.Icon.Default.extend({
     options: {
         iconUrl: leafletMarkerIconImage,
         iconRetinaUrl: leafletMarkerIcon2xImage,
         shadowUrl: leafletMarkerShadowImage
     }
 })
 
-document.addEventListener('DOMContentLoaded', initializePlaceLists)
+export {
+    initializePlaceLists,
+}
```

### Comparing `betty-0.3.3/betty/extension/maps/assets/betty.extension.npm._Npm/src/package.json` & `betty-0.3.4/betty/extension/webpack/webpack/package.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5375%*

 * *Differences: {"'dependencies'": "{'@babel/preset-typescript': '^7.24.1', 'copy-webpack-plugin': '^12.0.2', "*

 * *                   "'css-minimizer-webpack-plugin': '^6.0.0', 'file-loader': '^6.2.0', "*

 * *                   "'postcss-loader': '^8.0.0', 'resolve-url-loader': '^5.0.0', 'sass': '^1.56.1', "*

 * *                   "'sass-loader': '^14.0.0', 'style-loader': '^4.0.0', 'terser-webpack-plugin': "*

 * *                   "'^5.3.10', 'typescript': '^5.4.5', delete: ['leaflet', "*

 * *                   "'leaflet.markercluster', 'leaf […]*

```diff
@@ -1,24 +1,31 @@
 {
     "dependencies": {
         "@babel/core": "^7.19.6",
         "@babel/preset-env": "^7.19.4",
+        "@babel/preset-typescript": "^7.24.1",
         "babel-loader": "^9.1.0",
         "clean-webpack-plugin": "^4.0.0",
+        "copy-webpack-plugin": "^12.0.2",
         "core-js": "^3.26.0",
         "css-loader": "^7.1.0",
-        "leaflet": "^1.9.2",
-        "leaflet-gesture-handling": "^1.2.2",
-        "leaflet.fullscreen": "^3.0.0",
-        "leaflet.markercluster": "^1.5.3",
+        "css-minimizer-webpack-plugin": "^6.0.0",
+        "file-loader": "^6.2.0",
         "mini-css-extract-plugin": "^2.6.1",
+        "postcss-loader": "^8.0.0",
+        "resolve-url-loader": "^5.0.0",
+        "sass": "^1.56.1",
+        "sass-loader": "^14.0.0",
+        "style-loader": "^4.0.0",
+        "terser-webpack-plugin": "^5.3.10",
+        "typescript": "^5.4.5",
         "webpack": "^5.74.0",
         "webpack-cli": "^5.1.4"
     },
     "engines": {
         "node": ">= 16"
     },
-    "main": "maps.js",
     "scripts": {
         "webpack": "webpack --config webpack.config.js"
-    }
+    },
+    "type": "module"
 }
```

### Comparing `betty-0.3.3/betty/extension/nginx/__init__.py` & `betty-0.3.4/betty/extension/nginx/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 """Integrate Betty with `nginx <https://nginx.org/>`_."""
+
 from collections.abc import Sequence
 from pathlib import Path
 from typing import Any, Self
 
-from PyQt6.QtWidgets import QFormLayout, QButtonGroup, QRadioButton, QWidget, QHBoxLayout, QLineEdit, \
-    QFileDialog, QPushButton
+from PyQt6.QtWidgets import (
+    QFormLayout,
+    QButtonGroup,
+    QRadioButton,
+    QWidget,
+    QHBoxLayout,
+    QLineEdit,
+    QFileDialog,
+    QPushButton,
+)
 
 from betty.app import App
 from betty.app.extension import ConfigurableExtension
 from betty.config import Configuration
-from betty.extension.nginx.artifact import generate_configuration_file, generate_dockerfile_file
+from betty.extension.nginx.artifact import (
+    generate_configuration_file,
+    generate_dockerfile_file,
+)
 from betty.generate import Generator, GenerationContext
 from betty.gui import GuiBuilder
 from betty.gui.error import ExceptionCatcher
 from betty.locale import Str
 from betty.serde.dump import Dump, VoidableDump, minimize, Void, VoidableDictDump
 from betty.serde.load import Asserter, Fields, OptionalField, Assertions
 from betty.serve import ServerProvider, Server
@@ -58,42 +70,58 @@
         cls,
         dump: Dump,
         configuration: Self | None = None,
     ) -> Self:
         if configuration is None:
             configuration = cls()
         asserter = Asserter()
-        asserter.assert_record(Fields(
-            OptionalField(
-                'https',
-                Assertions(asserter.assert_or(asserter.assert_bool(), asserter.assert_none())) | asserter.assert_setattr(configuration, 'https'),
-            ),
-            OptionalField(
-                'www_directory_path',
-                Assertions(asserter.assert_str()) | asserter.assert_setattr(configuration, 'www_directory_path'),
-            ),
-        ))(dump)
+        asserter.assert_record(
+            Fields(
+                OptionalField(
+                    "https",
+                    Assertions(
+                        asserter.assert_or(
+                            asserter.assert_bool(), asserter.assert_none()
+                        )
+                    )
+                    | asserter.assert_setattr(configuration, "https"),
+                ),
+                OptionalField(
+                    "www_directory_path",
+                    Assertions(asserter.assert_str())
+                    | asserter.assert_setattr(configuration, "www_directory_path"),
+                ),
+            )
+        )(dump)
         return configuration
 
     def dump(self) -> VoidableDump:
         dump: VoidableDictDump[VoidableDump] = {
-            'https': self.https,
-            'www_directory_path': Void if self.www_directory_path is None else str(self.www_directory_path),
+            "https": self.https,
+            "www_directory_path": (
+                Void
+                if self.www_directory_path is None
+                else str(self.www_directory_path)
+            ),
         }
         return minimize(dump, True)
 
 
-class _Nginx(ConfigurableExtension[NginxConfiguration], Generator, ServerProvider, GuiBuilder):
+class Nginx(
+    ConfigurableExtension[NginxConfiguration], Generator, ServerProvider, GuiBuilder
+):
     @classmethod
     def label(cls) -> Str:
-        return Str.plain('Nginx')
+        return Str.plain("Nginx")
 
     @classmethod
     def description(cls) -> Str:
-        return Str._('Generate <a href="">nginx</a> configuration for your site, as well as a <code>Dockerfile</code> to build a <a href="https://www.docker.com/">Docker</a> container around it.')
+        return Str._(
+            'Generate <a href="">nginx</a> configuration for your site, as well as a <code>Dockerfile</code> to build a <a href="https://www.docker.com/">Docker</a> container around it.'
+        )
 
     @classmethod
     def default_configuration(cls) -> NginxConfiguration:
         return NginxConfiguration()
 
     @property
     def servers(self) -> Sequence[Server]:
@@ -105,78 +133,105 @@
 
     async def generate(self, job_context: GenerationContext) -> None:
         await generate_configuration_file(self._app)
         await generate_dockerfile_file(self._app)
 
     @classmethod
     def assets_directory_path(cls) -> Path | None:
-        return Path(__file__).parent / 'assets'
+        return Path(__file__).parent / "assets"
 
     @property
     def https(self) -> bool:
         if self._configuration.https is None:
-            return self._app.project.configuration.base_url.startswith('https')
+            return self._app.project.configuration.base_url.startswith("https")
         return self._configuration.https
 
     @property
     def www_directory_path(self) -> str:
-        return self._configuration.www_directory_path or str(self._app.project.configuration.www_directory_path)
+        return self._configuration.www_directory_path or str(
+            self._app.project.configuration.www_directory_path
+        )
 
     def gui_build(self) -> QWidget:
         return _NginxGuiWidget(self._app, self._configuration)
 
 
 class _NginxGuiWidget(QWidget):
-    def __init__(self, app: App, configuration: NginxConfiguration, *args: Any, **kwargs: Any):
+    def __init__(
+        self, app: App, configuration: NginxConfiguration, *args: Any, **kwargs: Any
+    ):
         super().__init__(*args, **kwargs)
         self._app = app
         self._configuration = configuration
         layout = QFormLayout()
 
         self.setLayout(layout)
 
         https_button_group = QButtonGroup()
 
         def _update_configuration_https_base_url(checked: bool) -> None:
             if checked:
                 self._configuration.https = None
-        self._nginx_https_base_url = QRadioButton("Use HTTPS and HTTP/2 if the site's URL starts with https://")
+
+        self._nginx_https_base_url = QRadioButton(
+            "Use HTTPS and HTTP/2 if the site's URL starts with https://"
+        )
         self._nginx_https_base_url.setChecked(self._configuration.https is None)
         self._nginx_https_base_url.toggled.connect(_update_configuration_https_base_url)
         layout.addRow(self._nginx_https_base_url)
         https_button_group.addButton(self._nginx_https_base_url)
 
         def _update_configuration_https_https(checked: bool) -> None:
             if checked:
                 self._configuration.https = True
-        self._nginx_https_https = QRadioButton('Use HTTPS and HTTP/2')
+
+        self._nginx_https_https = QRadioButton("Use HTTPS and HTTP/2")
         self._nginx_https_https.setChecked(self._configuration.https is True)
         self._nginx_https_https.toggled.connect(_update_configuration_https_https)
         layout.addRow(self._nginx_https_https)
         https_button_group.addButton(self._nginx_https_https)
 
         def _update_configuration_https_http(checked: bool) -> None:
             if checked:
                 self._configuration.https = False
-        self._nginx_https_http = QRadioButton('Use HTTP')
+
+        self._nginx_https_http = QRadioButton("Use HTTP")
         self._nginx_https_http.setChecked(self._configuration.https is False)
         self._nginx_https_http.toggled.connect(_update_configuration_https_http)
         layout.addRow(self._nginx_https_http)
         https_button_group.addButton(self._nginx_https_http)
 
         def _update_configuration_www_directory_path(www_directory_path: str) -> None:
-            self._configuration.www_directory_path = None if www_directory_path == '' or www_directory_path == str(self._app.project.configuration.www_directory_path) else www_directory_path
+            self._configuration.www_directory_path = (
+                None
+                if www_directory_path == ""
+                or www_directory_path
+                == str(self._app.project.configuration.www_directory_path)
+                else www_directory_path
+            )
+
         self._nginx_www_directory_path = QLineEdit()
-        self._nginx_www_directory_path.setText(str(self._configuration.www_directory_path) if self._configuration.www_directory_path is not None else str(self._app.project.configuration.www_directory_path))
-        self._nginx_www_directory_path.textChanged.connect(_update_configuration_www_directory_path)
+        self._nginx_www_directory_path.setText(
+            str(self._configuration.www_directory_path)
+            if self._configuration.www_directory_path is not None
+            else str(self._app.project.configuration.www_directory_path)
+        )
+        self._nginx_www_directory_path.textChanged.connect(
+            _update_configuration_www_directory_path
+        )
         www_directory_path_layout = QHBoxLayout()
         www_directory_path_layout.addWidget(self._nginx_www_directory_path)
 
         def find_www_directory_path() -> None:
             with ExceptionCatcher(self):
-                found_www_directory_path = QFileDialog.getExistingDirectory(self, 'Serve your site from...', directory=self._nginx_www_directory_path.text())
-                if '' != found_www_directory_path:
+                found_www_directory_path = QFileDialog.getExistingDirectory(
+                    self,
+                    "Serve your site from...",
+                    directory=self._nginx_www_directory_path.text(),
+                )
+                if "" != found_www_directory_path:
                     self._nginx_www_directory_path.setText(found_www_directory_path)
-        self._nginx_www_directory_path_find = QPushButton('...')
+
+        self._nginx_www_directory_path_find = QPushButton("...")
         self._nginx_www_directory_path_find.released.connect(find_www_directory_path)
         www_directory_path_layout.addWidget(self._nginx_www_directory_path_find)
-        layout.addRow('WWW directory', www_directory_path_layout)
+        layout.addRow("WWW directory", www_directory_path_layout)
```

### Comparing `betty-0.3.3/betty/extension/nginx/artifact.py` & `betty-0.3.4/betty/extension/nginx/artifact.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Build nginx and Docker artifacts, such as configuration files.
 """
+
 import asyncio
 from pathlib import Path
 from shutil import copyfile
 from urllib.parse import urlparse
 
 import aiofiles
 from aiofiles.os import makedirs
@@ -22,31 +23,52 @@
 ) -> None:
     """
     Generate an ``nginx.conf`` file to the given destination path.
     """
     from betty.extension import Nginx
 
     data = {
-        'server_name': urlparse(app.project.configuration.base_url).netloc,
-        'www_directory_path': www_directory_path or app.extensions[Nginx].www_directory_path,
-        'https': https or app.extensions[Nginx].https,
+        "server_name": urlparse(app.project.configuration.base_url).netloc,
+        "www_directory_path": www_directory_path
+        or app.extensions[Nginx].www_directory_path,
+        "https": https or app.extensions[Nginx].https,
     }
     if destination_file_path is None:
-        destination_file_path = app.project.configuration.output_directory_path / 'nginx' / 'nginx.conf'
+        destination_file_path = (
+            app.project.configuration.output_directory_path / "nginx" / "nginx.conf"
+        )
     root_path = rootname(Path(__file__))
-    configuration_file_template_name = '/'.join((Path(__file__).parent / 'assets' / 'nginx.conf.j2').relative_to(root_path).parts)
-    template = FileSystemLoader(root_path).load(app.jinja2_environment, configuration_file_template_name, app.jinja2_environment.globals)
+    configuration_file_template_name = "/".join(
+        (Path(__file__).parent / "assets" / "nginx.conf.j2")
+        .relative_to(root_path)
+        .parts
+    )
+    template = FileSystemLoader(root_path).load(
+        app.jinja2_environment,
+        configuration_file_template_name,
+        app.jinja2_environment.globals,
+    )
     await makedirs(destination_file_path.parent, exist_ok=True)
     configuration_file_contents = await template.render_async(data)
-    async with aiofiles.open(destination_file_path, 'w', encoding='utf-8') as f:
+    async with aiofiles.open(destination_file_path, "w", encoding="utf-8") as f:
         await f.write(configuration_file_contents)
 
 
-async def generate_dockerfile_file(app: App, destination_file_path: Path | None = None) -> None:
+async def generate_dockerfile_file(
+    app: App, destination_file_path: Path | None = None
+) -> None:
     """
     Generate a ``Dockerfile`` to the given destination path.
     """
     if destination_file_path is None:
-        destination_file_path = app.project.configuration.output_directory_path / 'nginx' / 'Dockerfile'
+        destination_file_path = (
+            app.project.configuration.output_directory_path / "nginx" / "Dockerfile"
+        )
     await makedirs(destination_file_path.parent, exist_ok=True)
-    await asyncio.to_thread(copyfile, Path(__file__).parent / 'assets' / 'Dockerfile', destination_file_path)
-    await asyncio.to_thread(copyfile, Path(__file__).parent / 'assets' / 'content_negotiation.lua', destination_file_path.parent / 'content_negotiation.lua')
+    await asyncio.to_thread(
+        copyfile, Path(__file__).parent / "assets" / "Dockerfile", destination_file_path
+    )
+    await asyncio.to_thread(
+        copyfile,
+        Path(__file__).parent / "assets" / "content_negotiation.lua",
+        destination_file_path.parent / "content_negotiation.lua",
+    )
```

### Comparing `betty-0.3.3/betty/extension/nginx/assets/content_negotiation.lua` & `betty-0.3.4/betty/extension/nginx/assets/content_negotiation.lua`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/nginx/assets/nginx.conf.j2` & `betty-0.3.4/betty/extension/nginx/assets/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/nginx/docker.py` & `betty-0.3.4/betty/extension/nginx/docker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 """
 Integrate Betty with Docker.
 """
+
 import asyncio
 from pathlib import Path
 from types import TracebackType
 
 import docker
 from docker.models.containers import Container as DockerContainer
 
 
 class Container:
-    _IMAGE_TAG = 'betty-serve'
+    _IMAGE_TAG = "betty-serve"
 
-    def __init__(self, www_directory_path: Path, docker_directory_path: Path, nginx_configuration_file_path: Path):
+    def __init__(
+        self,
+        www_directory_path: Path,
+        docker_directory_path: Path,
+        nginx_configuration_file_path: Path,
+    ):
         self._docker_directory_path = docker_directory_path
         self._nginx_configuration_file_path = nginx_configuration_file_path
         self._www_directory_path = www_directory_path
         self._client = docker.from_env()
         self.__container: DockerContainer | None = None
 
     async def __aenter__(self) -> None:
         await self.start()
 
-    async def __aexit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
         await self.stop()
 
     async def start(self) -> None:
         await asyncio.to_thread(self._start)
 
     def _start(self) -> None:
-        self._client.images.build(path=str(self._docker_directory_path), tag=self._IMAGE_TAG)
+        self._client.images.build(
+            path=str(self._docker_directory_path), tag=self._IMAGE_TAG
+        )
         self._container.start()
-        self._container.exec_run(['nginx', '-s', 'reload'])
+        self._container.exec_run(["nginx", "-s", "reload"])
 
     async def stop(self) -> None:
         await asyncio.to_thread(self._stop)
 
     def _stop(self) -> None:
         if self._container is not None:
             self._container.stop()
@@ -45,21 +58,23 @@
         if self.__container is None:
             self.__container = self._client.containers.create(
                 self._IMAGE_TAG,
                 auto_remove=True,
                 detach=True,
                 volumes={
                     self._nginx_configuration_file_path: {
-                        'bind': '/etc/nginx/conf.d/betty.conf',
-                        'mode': 'ro',
+                        "bind": "/etc/nginx/conf.d/betty.conf",
+                        "mode": "ro",
                     },
                     self._www_directory_path: {
-                        'bind': '/var/www/betty',
-                        'mode': 'ro',
+                        "bind": "/var/www/betty",
+                        "mode": "ro",
                     },
                 },
             )
         return self.__container
 
     @property
     def ip(self) -> DockerContainer:
-        return self._client.api.inspect_container(self._container.id)['NetworkSettings']['Networks']['bridge']['IPAddress']
+        return self._client.api.inspect_container(self._container.id)[
+            "NetworkSettings"
+        ]["Networks"]["bridge"]["IPAddress"]
```

### Comparing `betty-0.3.3/betty/extension/nginx/serve.py` & `betty-0.3.4/betty/extension/nginx/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """
 Integrate the nginx extension with Betty's Serve API.
 """
+
 import logging
 from contextlib import AsyncExitStack
 from pathlib import Path
 
 import docker
 from aiofiles.tempfile import TemporaryDirectory
 from docker.errors import DockerException
 
 from betty.app import App
-from betty.extension.nginx.artifact import generate_dockerfile_file, generate_configuration_file
+from betty.extension.nginx.artifact import (
+    generate_dockerfile_file,
+    generate_configuration_file,
+)
 from betty.extension.nginx.docker import Container
 from betty.project import Project
 from betty.serve import NoPublicUrlBecauseServerNotStartedError, Server
 
 
 class DockerizedNginxServer(Server):
     def __init__(self, app: App) -> None:
@@ -23,39 +27,45 @@
         self._exit_stack = AsyncExitStack()
         self._container: Container | None = None
 
     async def start(self) -> None:
         from betty.extension import Nginx
 
         await super().start()
-        logging.getLogger(__name__).info('Starting a Dockerized nginx web server...')
+        logging.getLogger(__name__).info("Starting a Dockerized nginx web server...")
 
-        output_directory_path_str = await self._exit_stack.enter_async_context(TemporaryDirectory())
+        output_directory_path_str = await self._exit_stack.enter_async_context(
+            TemporaryDirectory()
+        )
 
         isolated_project = Project(ancestry=self._app.project.ancestry)
         isolated_project.configuration.autowrite = False
-        isolated_project.configuration.configuration_file_path = self._app.project.configuration.configuration_file_path
+        isolated_project.configuration.configuration_file_path = (
+            self._app.project.configuration.configuration_file_path
+        )
         isolated_project.configuration.update(self._app.project.configuration)
         isolated_project.configuration.debug = True
 
-        isolated_app = await self._exit_stack.enter_async_context(App.new_from_app(self._app, project=isolated_project))
+        isolated_app = await self._exit_stack.enter_async_context(
+            App.new_from_app(self._app, project=isolated_project)
+        )
         await self._exit_stack.enter_async_context(isolated_app)
         isolated_app.configuration.update(self._app.configuration)
         # Work around https://github.com/bartfeenstra/betty/issues/1056.
         isolated_app.extensions[Nginx].configuration.https = False
 
-        nginx_configuration_file_path = Path(output_directory_path_str) / 'nginx.conf'
+        nginx_configuration_file_path = Path(output_directory_path_str) / "nginx.conf"
         docker_directory_path = Path(output_directory_path_str)
-        dockerfile_file_path = docker_directory_path / 'Dockerfile'
+        dockerfile_file_path = docker_directory_path / "Dockerfile"
 
         await generate_configuration_file(
             isolated_app,
             destination_file_path=nginx_configuration_file_path,
             https=False,
-            www_directory_path='/var/www/betty',
+            www_directory_path="/var/www/betty",
         )
         await generate_dockerfile_file(
             isolated_app,
             destination_file_path=dockerfile_file_path,
         )
         self._container = Container(
             isolated_app.project.configuration.www_directory_path,
@@ -67,15 +77,15 @@
 
     async def stop(self) -> None:
         await self._exit_stack.aclose()
 
     @property
     def public_url(self) -> str:
         if self._container is not None:
-            return 'http://%s' % self._container.ip
+            return "http://%s" % self._container.ip
         raise NoPublicUrlBecauseServerNotStartedError()
 
     @classmethod
     def is_available(cls) -> bool:
         try:
             docker.from_env().info()
             return True
```

### Comparing `betty-0.3.3/betty/extension/privatizer/__init__.py` & `betty-0.3.4/betty/extension/privatizer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,77 @@
 """Privatize people and associated data by determining if they are likely to be alive."""
+
 from __future__ import annotations
 
 from collections import defaultdict
 from logging import getLogger
 
 from betty.app.extension import UserFacingExtension
 from betty.load import PostLoader
 from betty.locale import Str
 from betty.model import Entity
 from betty.model.ancestry import Person, HasPrivacy
 from betty.privatizer import Privatizer as PrivatizerApi
 
 
-class _Privatizer(UserFacingExtension, PostLoader):
+class Privatizer(UserFacingExtension, PostLoader):
+    @classmethod
+    def name(cls) -> str:
+        return "betty.extension.Privatizer"
+
     async def post_load(self) -> None:
         self.privatize()
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Privatizer')
+        return Str._("Privatizer")
 
     @classmethod
     def description(cls) -> Str:
-        return Str._('Determine if people can be proven to have died. If not, mark them and their associated entities private.')
+        return Str._(
+            "Determine if people can be proven to have died. If not, mark them and their associated entities private."
+        )
 
     def privatize(self) -> None:
         logger = getLogger(__name__)
-        logger.info(self._app.localizer._('Privatizing...'))
+        logger.info(self._app.localizer._("Privatizing..."))
 
         privatizer = PrivatizerApi(
             self._app.project.configuration.lifetime_threshold,
             localizer=self._app.localizer,
         )
 
         newly_privatized: dict[type[HasPrivacy & Entity], int] = defaultdict(lambda: 0)
         entities: list[HasPrivacy & Entity] = []
         for entity in self._app.project.ancestry:
             if isinstance(entity, HasPrivacy):
                 entities.append(entity)
                 if entity.private:
-                    newly_privatized[
-                        entity.type  # type: ignore[index]
-                    ] -= 1
+                    newly_privatized[entity.type] -= 1  # type: ignore[index]
 
         for entity in entities:
             privatizer.privatize(entity)
 
         for entity in entities:
             if entity.private:
                 newly_privatized[entity.type] += 1  # type: ignore[index]
 
         if newly_privatized[Person] > 0:
-            logger.info(self._app.localizer._('Privatized {count} people because they are likely still alive.').format(
-                count=str(newly_privatized[Person]),
-            ))
+            logger.info(
+                self._app.localizer._(
+                    "Privatized {count} people because they are likely still alive."
+                ).format(
+                    count=str(newly_privatized[Person]),
+                )
+            )
         for entity_type in set(newly_privatized) - {Person}:
             if newly_privatized[entity_type] > 0:
-                logger.info(self._app.localizer._('Privatized {count} {entity_type}, because they are associated with private information.').format(
-                    count=str(newly_privatized[entity_type]),
-                    entity_type=entity_type.entity_type_label_plural().localize(self._app.localizer),
-                ))
+                logger.info(
+                    self._app.localizer._(
+                        "Privatized {count} {entity_type}, because they are associated with private information."
+                    ).format(
+                        count=str(newly_privatized[entity_type]),
+                        entity_type=entity_type.entity_type_label_plural().localize(
+                            self._app.localizer
+                        ),
+                    )
+                )
```

### Comparing `betty-0.3.3/betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.js` & `betty-0.3.4/betty/extension/trees/webpack/trees.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,90 +1,86 @@
 'use strict'
 
-import treesStyle from './trees.css' // eslint-disable-line no-unused-vars
+import './main.css'
 
 import cytoscape from 'cytoscape'
 import dagre from 'cytoscape-dagre'
 
 cytoscape.use(dagre)
 
-function initializeAncestryTrees() {
+async function initializeAncestryTrees() {
     const trees = document.getElementsByClassName('tree')
-    for (const tree of trees) {
-        initializeAncestryTree(tree, tree.dataset.bettyPersonId)
-    }
+    await Promise.allSettled(Array.from(trees).map(tree => initializeAncestryTree(tree, tree.dataset.bettyPersonId)))
 }
 
-function initializeAncestryTree(tree, personId) {
-    fetch(tree.dataset.bettyPeople)
-        .then((response) => response.json())
-        .then((people) => {
-            const elements = {
-                nodes: [],
-                edges: []
-            }
-            const person = people[personId]
-            personToNode(person, elements.nodes)
-            parentsToElements(person, elements, people)
-            childrenToElements(person, elements, people)
-            const cy = cytoscape({
-                container: document.getElementsByClassName('tree')[0],
-                layout: {
-                    name: 'dagre'
-                },
-                wheelSensitivity: 0.25,
-                style: [{
-                    selector: 'node',
-                    style: {
-                        content: 'data(label)',
-                        shape: 'round-rectangle',
-                        'text-valign': 'center',
-                        'text-halign': 'center',
-                        'background-color': '#eee',
-                        width: 'label',
-                        height: 'label',
-                        padding: '9px'
-                    }
-                }, {
-                    selector: 'node.public',
-                    style: {
-                        color: '#149988'
-                    }
-                }, {
-                    selector: 'node.public.hover',
-                    style: {
-                        color: '#2a615a'
-                    }
-                }, {
-                    selector: 'edge',
-                    style: {
-                        'curve-style': 'taxi',
-                        'taxi-direction': 'downward',
-                        width: 4,
-                        'target-arrow-shape': 'triangle',
-                        'line-color': '#777',
-                        'target-arrow-color': '#777'
-                    }
-                }],
-                elements
-            })
-            cy.zoom({
-                level: 1,
-                position: cy.getElementById(personId).position()
-            })
-            cy.on('mouseover', 'node.public', (event) => {
-                event.target.addClass('hover')
-            })
-            cy.on('mouseout', 'node.public', (event) => {
-                event.target.removeClass('hover')
-            })
-            cy.on('tap', 'node.public', (event) => {
-                window.location = event.target.data().url
-            })
-        })
+async function initializeAncestryTree(tree, personId) {
+    const response = await fetch(tree.dataset.bettyPeople)
+    const people = await response.json()
+    const elements = {
+        nodes: [],
+        edges: []
+    }
+    const person = people[personId]
+    personToNode(person, elements.nodes)
+    parentsToElements(person, elements, people)
+    childrenToElements(person, elements, people)
+    const cy = cytoscape({
+        container: document.getElementsByClassName('tree')[0],
+        layout: {
+            name: 'dagre'
+        },
+        wheelSensitivity: 0.25,
+        style: [{
+            selector: 'node',
+            style: {
+                content: 'data(label)',
+                shape: 'round-rectangle',
+                'text-valign': 'center',
+                'text-halign': 'center',
+                'background-color': '#eee',
+                width: 'label',
+                height: 'label',
+                padding: '9px'
+            }
+        }, {
+            selector: 'node.public',
+            style: {
+                color: '#149988'
+            }
+        }, {
+            selector: 'node.public.hover',
+            style: {
+                color: '#2a615a'
+            }
+        }, {
+            selector: 'edge',
+            style: {
+                'curve-style': 'taxi',
+                'taxi-direction': 'downward',
+                width: 4,
+                'target-arrow-shape': 'triangle',
+                'line-color': '#777',
+                'target-arrow-color': '#777'
+            }
+        }],
+        elements
+    })
+    cy.zoom({
+        level: 1,
+        position: cy.getElementById(personId).position()
+    })
+    cy.on('mouseover', 'node.public', (event) => {
+        event.target.addClass('hover')
+    })
+    cy.on('mouseout', 'node.public', (event) => {
+        event.target.removeClass('hover')
+    })
+    cy.on('tap', 'node.public', (event) => {
+        window.location = event.target.data().url
+    })
 }
 
 function personToNode(person, nodes) {
     nodes.push({
         data: {
             id: person.id,
             label: person.label,
@@ -121,8 +117,10 @@
             }
         })
         personToNode(child, elements.nodes)
         childrenToElements(child, elements, people)
     }
 }
 
-document.addEventListener('DOMContentLoaded', initializeAncestryTrees)
+export {
+    initializeAncestryTrees,
+}
```

### Comparing `betty-0.3.3/betty/extension/trees/assets/public/localized/people.json.j2` & `betty-0.3.4/betty/extension/trees/assets/public/localized/people.json.j2`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty/extension/wikipedia/__init__.py` & `betty-0.3.4/betty/extension/wikipedia/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Integrate Betty with `Wikipedia <https://wikipedia.org>`_."""
+
 from __future__ import annotations
 
 import logging
 from pathlib import Path
 from typing import Callable, Iterable, Any
 
 from jinja2 import pass_context
@@ -14,15 +15,19 @@
 from betty.jinja2 import Jinja2Provider, context_localizer
 from betty.load import PostLoader
 from betty.locale import negotiate_locale, Str
 from betty.model.ancestry import Link
 from betty.wikipedia import Summary, _parse_url, NotAPageError, RetrievalError
 
 
-class _Wikipedia(UserFacingExtension, Jinja2Provider, PostLoader):
+class Wikipedia(UserFacingExtension, Jinja2Provider, PostLoader):
+    @classmethod
+    def name(cls) -> str:
+        return "betty.extension.Wikipedia"
+
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.__retriever: wikipedia._Retriever | None = None
         self.__populator: wikipedia._Populator | None = None
 
     async def post_load(self) -> None:
         populator = wikipedia._Populator(self.app, self._retriever)
@@ -41,29 +46,32 @@
     @_retriever.deleter
     def _retriever(self) -> None:
         self.__retriever = None
 
     @property
     def filters(self) -> dict[str, Callable[..., Any]]:
         return {
-            'wikipedia': self._filter_wikipedia_links,
+            "wikipedia": self._filter_wikipedia_links,
         }
 
     @pass_context
-    async def _filter_wikipedia_links(self, context: Context, links: Iterable[Link]) -> Iterable[Summary]:
+    async def _filter_wikipedia_links(
+        self, context: Context, links: Iterable[Link]
+    ) -> Iterable[Summary]:
         return filter(
             None,
-            await gather(*(
-                self._filter_wikipedia_link(
-                    context_localizer(context).locale,
-                    link,
+            await gather(
+                *(
+                    self._filter_wikipedia_link(
+                        context_localizer(context).locale,
+                        link,
+                    )
+                    for link in links
                 )
-                for link
-                in links
-            )),
+            ),
         )
 
     async def _filter_wikipedia_link(self, locale: str, link: Link) -> Summary | None:
         try:
             page_language, page_name = _parse_url(link.url)
         except NotAPageError:
             return None
@@ -74,21 +82,23 @@
         except RetrievalError as error:
             logger = logging.getLogger(__name__)
             logger.warning(str(error))
             return None
 
     @classmethod
     def assets_directory_path(cls) -> Path | None:
-        return Path(__file__).parent / 'assets'
+        return Path(__file__).parent / "assets"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Wikipedia')
+        return Str._("Wikipedia")
 
     @classmethod
     def description(cls) -> Str:
-        return Str._("""
+        return Str._(
+            """
 Display <a href="https://www.wikipedia.org/">Wikipedia</a> summaries for resources with external links. In your custom <a href="https://jinja2docs.readthedocs.io/en/stable/">Jinja2</a> templates, use the following: <pre><code>
 {{% with resource=resource_with_links %}}
     {{% include 'wikipedia.html.j2' %}}
 {{% endwith %}}
-</code></pre>""")
+</code></pre>"""
+        )
```

### Comparing `betty-0.3.3/betty/fs.py` & `betty-0.3.4/betty/fs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide file system utilities.
 """
+
 from __future__ import annotations
 
 import asyncio
 import hashlib
 import os
 from collections import deque
 from contextlib import suppress
@@ -15,25 +16,29 @@
 from typing import AsyncIterable, AsyncContextManager, Sequence
 
 import aiofiles
 from aiofiles.os import makedirs
 from aiofiles.threadpool.text import AsyncTextIOWrapper
 
 from betty import _ROOT_DIRECTORY_PATH
+from betty.warnings import deprecated
 
 ROOT_DIRECTORY_PATH = _ROOT_DIRECTORY_PATH
 
 
-ASSETS_DIRECTORY_PATH = ROOT_DIRECTORY_PATH / 'betty' / 'assets'
+ASSETS_DIRECTORY_PATH = ROOT_DIRECTORY_PATH / "betty" / "assets"
+
+
+PREBUILT_ASSETS_DIRECTORY_PATH = ROOT_DIRECTORY_PATH / "prebuild"
 
 
-HOME_DIRECTORY_PATH = Path.home() / '.betty'
+HOME_DIRECTORY_PATH = Path.home() / ".betty"
 
 
-CACHE_DIRECTORY_PATH = HOME_DIRECTORY_PATH / 'cache'
+CACHE_DIRECTORY_PATH = HOME_DIRECTORY_PATH / "cache"
 """
 Define the path to the cache directory.
 
 .. deprecated:: 0.3.3
    This constant is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x.
    Instead, use :py:class:`betty.cache.file.BinaryFileCache`.
 """
@@ -44,39 +49,51 @@
     Recursively iterate over any files found in a directory.
     """
     for dir_path, _, filenames in os.walk(str(path)):
         for filename in filenames:
             yield Path(dir_path) / filename
 
 
+@deprecated(
+    "This function is deprecated as of Betty 0.3.4, and will be removed in Betty 0.4.x. Instead, use `betty.hashid.hashid_file_meta()`."
+)
 def hashfile(path: Path) -> str:
     """
     Get a hash for a file.
 
     This function relies on the file path and last modified time for uniqueness.
     File contents are ignored.
     """
-    return hashlib.md5(':'.join([str(getmtime(path)), str(path)]).encode('utf-8')).hexdigest()
+    return hashlib.md5(
+        ":".join([str(getmtime(path)), str(path)]).encode("utf-8")
+    ).hexdigest()
 
 
 class _Open:
     def __init__(self, fs: FileSystem, file_paths: tuple[Path, ...]):
         self._fs = fs
         self._file_paths = file_paths
         self._file: AsyncContextManager[AsyncTextIOWrapper] | None = None
 
     async def __aenter__(self) -> AsyncTextIOWrapper:
         for file_path in map(Path, self._file_paths):
             for fs_path, fs_encoding in self._fs._paths:
                 with suppress(FileNotFoundError):
-                    self._file = aiofiles.open(fs_path / file_path, encoding=fs_encoding)
+                    self._file = aiofiles.open(
+                        fs_path / file_path, encoding=fs_encoding
+                    )
                     return await self._file.__aenter__()
         raise FileNotFoundError
 
-    async def __aexit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
         if self._file is not None:
             await self._file.__aexit__(None, None, None)
 
 
 class FileSystem:
     def __init__(self, *paths: tuple[Path, str | None]):
         self._paths = deque(paths)
@@ -99,19 +116,25 @@
 
     async def copy2(self, source_path: Path, destination_path: Path) -> Path:
         for fs_path, _ in self._paths:
             with suppress(FileNotFoundError):
                 await asyncio.to_thread(copy2, fs_path / source_path, destination_path)
                 return destination_path
         tried_paths = [str(fs_path / source_path) for fs_path, _ in self._paths]
-        raise FileNotFoundError('Could not find any of %s.' % ', '.join(tried_paths))
+        raise FileNotFoundError("Could not find any of %s." % ", ".join(tried_paths))
 
-    async def copytree(self, source_path: Path, destination_path: Path) -> AsyncIterable[Path]:
+    async def copytree(
+        self, source_path: Path, destination_path: Path
+    ) -> AsyncIterable[Path]:
         file_destination_paths = set()
         for fs_path, _ in self._paths:
             async for file_source_path in iterfiles(fs_path / source_path):
-                file_destination_path = destination_path / file_source_path.relative_to(fs_path / source_path)
+                file_destination_path = destination_path / file_source_path.relative_to(
+                    fs_path / source_path
+                )
                 if file_destination_path not in file_destination_paths:
                     file_destination_paths.add(file_destination_path)
                     await makedirs(file_destination_path.parent, exist_ok=True)
-                    await asyncio.to_thread(copy2, file_source_path, file_destination_path)
+                    await asyncio.to_thread(
+                        copy2, file_source_path, file_destination_path
+                    )
                     yield file_destination_path
```

### Comparing `betty-0.3.3/betty/functools.py` & `betty-0.3.4/betty/functools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 """
 Provide functional programming utilities.
 """
+
 from __future__ import annotations
 
 from asyncio import sleep
 from inspect import isawaitable
 from time import time
-from typing import Any, Iterable, Sized, TypeVar, Callable, Iterator, Generic, cast, ParamSpec, Awaitable
+from typing import (
+    Any,
+    Iterable,
+    Sized,
+    TypeVar,
+    Callable,
+    Iterator,
+    Generic,
+    cast,
+    ParamSpec,
+    Awaitable,
+)
 
-T = TypeVar('T')
-U = TypeVar('U')
+T = TypeVar("T")
+U = TypeVar("U")
 
 
 def walk(item: Any, attribute_name: str) -> Iterable[Any]:
     """
     Walk over a graph of objects by following a single attribute.
     """
     child = getattr(item, attribute_name)
@@ -21,20 +33,20 @@
     # If the child has the requested attribute, yield it,
     if hasattr(child, attribute_name):
         yield child
         yield from walk(child, attribute_name)
 
     # Otherwise loop over the children and yield their attributes.
     try:
-        child = iter(child)
+        child_children = iter(child)
     except TypeError:
         return
-    for child in child:
-        yield child
-        yield from walk(child, attribute_name)
+    for child_child in child_children:
+        yield child_child
+        yield from walk(child_child, attribute_name)
 
 
 def slice_to_range(indices: slice, iterable: Sized) -> Iterable[int]:
     """
     Apply a slice to an iterable, and return the corresponding range.
     """
     length = len(iterable)
@@ -72,32 +84,36 @@
         return cast(T, self._value)
 
     def map(self, f: Callable[[T], U]) -> _Result[U]:
         if self._error:
             return cast(_Result[U], self)
         try:
             return _Result(f(self.value))
-        except BaseException as e:
+        except Exception as e:
             return _Result(None, e)
 
 
-def filter_suppress(raising_filter: Callable[[T], Any], exception_type: type[BaseException], items: Iterable[T]) -> Iterator[T]:
+def filter_suppress(
+    raising_filter: Callable[[T], Any],
+    exception_type: type[BaseException],
+    items: Iterable[T],
+) -> Iterator[T]:
     """
     Filter values, skipping those for which the application of `raising_filter` raises errors.
     """
     for item in items:
         try:
             raising_filter(item)
             yield item
         except exception_type:
             continue
 
 
-_DoFReturnT = TypeVar('_DoFReturnT')
-_DoFP = ParamSpec('_DoFP')
+_DoFReturnT = TypeVar("_DoFReturnT")
+_DoFP = ParamSpec("_DoFP")
 
 
 class Do(Generic[_DoFP, _DoFReturnT]):
     def __init__(
         self,
         f: Callable[_DoFP, _DoFReturnT | Awaitable[_DoFReturnT]],
         *args: _DoFP.args,
@@ -124,17 +140,21 @@
                 else:
                     f_result = f_result_or_coroutine
                 for condition in conditions:
                     condition_result_or_coroutine = condition(f_result)
                     if isawaitable(condition_result_or_coroutine):
                         condition_result = await condition_result_or_coroutine
                     else:
-                        condition_result = cast(None | bool, condition_result_or_coroutine)
+                        condition_result = cast(
+                            None | bool, condition_result_or_coroutine
+                        )
                     if condition_result is False:
-                        raise RuntimeError(f'Condition {condition} was not met for {f_result}.')
+                        raise RuntimeError(
+                            f"Condition {condition} was not met for {f_result}."
+                        )
             except BaseException:
                 if retries == 0:
                     raise
                 if time() - start_time > timeout:
                     raise
                 await sleep(interval)
             else:
```

### Comparing `betty-0.3.3/betty/generate.py` & `betty-0.3.4/betty/generate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide the Generation API.
 """
+
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import os
 import shutil
@@ -20,23 +21,34 @@
 from aiofiles.threadpool.text import AsyncTextIOWrapper
 
 from betty.app import App
 from betty.job import Context
 from betty.json.linked_data import LinkedDataDumpable
 from betty.json.schema import Schema
 from betty.locale import get_display_name
-from betty.model import get_entity_type_name, UserFacingEntity, Entity, GeneratedEntityId
+from betty.model import (
+    get_entity_type_name,
+    UserFacingEntity,
+    Entity,
+    GeneratedEntityId,
+)
 from betty.model.ancestry import is_public
 from betty.openapi import Specification
 from betty.serde.dump import DictDump, Dump
-from betty.string import camel_case_to_kebab_case, camel_case_to_snake_case, upper_camel_case_to_lower_camel_case
+from betty.string import (
+    camel_case_to_kebab_case,
+    camel_case_to_snake_case,
+    upper_camel_case_to_lower_camel_case,
+)
 from betty.warnings import deprecated
 
 
-@deprecated('This function is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, use `logging.logging.getLogger(__name__)`.')
+@deprecated(
+    "This function is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, use `logging.logging.getLogger(__name__)`."
+)
 def getLogger() -> logging.Logger:
     """
     Get the site generation logger.
     """
     return logging.getLogger(__name__)
 
 
@@ -58,68 +70,89 @@
 async def generate(app: App) -> None:
     """
     Generate a new site.
     """
     logger = logging.getLogger(__name__)
     job_context = GenerationContext(app)
 
-    logger.info(app.localizer._('Generating your site to {output_directory}.').format(output_directory=app.project.configuration.output_directory_path))
+    logger.info(
+        app.localizer._("Generating your site to {output_directory}.").format(
+            output_directory=app.project.configuration.output_directory_path
+        )
+    )
     with suppress(FileNotFoundError):
-        await asyncio.to_thread(shutil.rmtree, app.project.configuration.output_directory_path)
+        await asyncio.to_thread(
+            shutil.rmtree, app.project.configuration.output_directory_path
+        )
     await makedirs(app.project.configuration.output_directory_path, exist_ok=True)
 
     # The static public assets may be overridden depending on the number of locales rendered, so ensure they are
     # generated before anything else.
     await _generate_static_public(app, job_context)
 
     jobs = [job async for job in _run_jobs(app, job_context)]
     log_job = create_task(_log_jobs_forever(app, jobs))
     for completed_job in as_completed(jobs):
         await completed_job
     log_job.cancel()
     await _log_jobs(app, jobs)
 
     os.chmod(app.project.configuration.output_directory_path, 0o755)
-    for directory_path_str, subdirectory_names, file_names in os.walk(app.project.configuration.output_directory_path):
+    for directory_path_str, subdirectory_names, file_names in os.walk(
+        app.project.configuration.output_directory_path
+    ):
         directory_path = Path(directory_path_str)
         for subdirectory_name in subdirectory_names:
             os.chmod(directory_path / subdirectory_name, 0o755)
         for file_name in file_names:
             os.chmod(directory_path / file_name, 0o644)
 
 
 async def _log_jobs(app: App, jobs: Sequence[Task[None]]) -> None:
     total_job_count = len(jobs)
     completed_job_count = len([job for job in jobs if job.done()])
-    logging.getLogger(__name__).info(app.localizer._(
-        'Generated {completed_job_count} out of {total_job_count} items ({completed_job_percentage}%).').format(
-        completed_job_count=completed_job_count,
-        total_job_count=total_job_count,
-        completed_job_percentage=floor(completed_job_count / (total_job_count / 100)),
-    ))
+    logging.getLogger(__name__).info(
+        app.localizer._(
+            "Generated {completed_job_count} out of {total_job_count} items ({completed_job_percentage}%)."
+        ).format(
+            completed_job_count=completed_job_count,
+            total_job_count=total_job_count,
+            completed_job_percentage=floor(
+                completed_job_count / (total_job_count / 100)
+            ),
+        )
+    )
 
 
 async def _log_jobs_forever(app: App, jobs: Sequence[Task[None]]) -> None:
     with suppress(CancelledError):
         while True:
             await _log_jobs(app, jobs)
             await sleep(5)
 
 
-_JobP = ParamSpec('_JobP')
+_JobP = ParamSpec("_JobP")
 
 
-def _run_job(semaphore: Semaphore, f: Callable[_JobP, Awaitable[None]], *args: _JobP.args, **kwargs: _JobP.kwargs) -> Task[None]:
+def _run_job(
+    semaphore: Semaphore,
+    f: Callable[_JobP, Awaitable[None]],
+    *args: _JobP.args,
+    **kwargs: _JobP.kwargs,
+) -> Task[None]:
     async def _job():
         async with semaphore:
             await f(*args, **kwargs)
+
     return create_task(_job())
 
 
-async def _run_jobs(app: App, job_context: GenerationContext) -> AsyncIterator[Task[None]]:
+async def _run_jobs(
+    app: App, job_context: GenerationContext
+) -> AsyncIterator[Task[None]]:
     semaphore = Semaphore(512)
     yield _run_job(semaphore, _generate_dispatch, job_context)
     yield _run_job(semaphore, _generate_sitemap, job_context)
     yield _run_job(semaphore, _generate_json_schema, job_context)
     yield _run_job(semaphore, _generate_openapi, job_context)
 
     locales = app.project.configuration.locales
@@ -128,147 +161,193 @@
         yield _run_job(semaphore, _generate_public, job_context, locale)
 
     for entity_type in app.entity_types:
         if not issubclass(entity_type, UserFacingEntity):
             continue
         if app.project.configuration.entity_types[entity_type].generate_html_list:
             for locale in locales:
-                yield _run_job(semaphore, _generate_entity_type_list_html, job_context, locale, entity_type)
-        yield _run_job(semaphore, _generate_entity_type_list_json, job_context, entity_type)
+                yield _run_job(
+                    semaphore,
+                    _generate_entity_type_list_html,
+                    job_context,
+                    locale,
+                    entity_type,
+                )
+        yield _run_job(
+            semaphore, _generate_entity_type_list_json, job_context, entity_type
+        )
         for entity in app.project.ancestry[entity_type]:
             if isinstance(entity.id, GeneratedEntityId):
                 continue
 
-            yield _run_job(semaphore, _generate_entity_json, job_context, entity_type, entity.id)
+            yield _run_job(
+                semaphore, _generate_entity_json, job_context, entity_type, entity.id
+            )
             if is_public(entity):
                 for locale in locales:
-                    yield _run_job(semaphore, _generate_entity_html, job_context, locale, entity_type, entity.id)
+                    yield _run_job(
+                        semaphore,
+                        _generate_entity_html,
+                        job_context,
+                        locale,
+                        entity_type,
+                        entity.id,
+                    )
 
 
 async def create_file(path: Path) -> AsyncContextManager[AsyncTextIOWrapper]:
     """
     Create the file for a resource.
     """
     await makedirs(path.parent, exist_ok=True)
-    return cast(AsyncContextManager[AsyncTextIOWrapper], aiofiles.open(path, 'w', encoding='utf-8'))
+    return cast(
+        AsyncContextManager[AsyncTextIOWrapper],
+        aiofiles.open(path, "w", encoding="utf-8"),
+    )
 
 
 async def create_html_resource(path: Path) -> AsyncContextManager[AsyncTextIOWrapper]:
     """
     Create the file for an HTML resource.
     """
-    return await create_file(path / 'index.html')
+    return await create_file(path / "index.html")
 
 
 async def create_json_resource(path: Path) -> AsyncContextManager[AsyncTextIOWrapper]:
     """
     Create the file for a JSON resource.
     """
-    return await create_file(path / 'index.json')
+    return await create_file(path / "index.json")
 
 
 async def _generate_dispatch(
     job_context: GenerationContext,
 ) -> None:
     app = job_context.app
-    await app.dispatcher.dispatch(Generator)(job_context),
+    await app.dispatcher.dispatch(Generator)(job_context)
 
 
 async def _generate_public(
     job_context: GenerationContext,
     locale: str,
 ) -> None:
     app = job_context.app
     locale_label = get_display_name(locale, app.localizer.locale)
-    logging.getLogger(__name__).debug(app.localizer._('Generating localized public files in {locale}...').format(
-        locale=locale_label,
-    ))
-    async for file_path in app.assets.copytree(Path('public') / 'localized', app.project.configuration.localize_www_directory_path(locale)):
+    logging.getLogger(__name__).debug(
+        app.localizer._("Generating localized public files in {locale}...").format(
+            locale=locale_label,
+        )
+    )
+    async for file_path in app.assets.copytree(
+        Path("public") / "localized",
+        app.project.configuration.localize_www_directory_path(locale),
+    ):
         await app.renderer.render_file(
             file_path,
             job_context=job_context,
-            localizer=app.localizers[locale],
+            localizer=await app.localizers.get(locale),
         )
 
 
 async def _generate_static_public(
     app: App,
     job_context: Context,
 ) -> None:
-    logging.getLogger(__name__).info(app.localizer._('Generating static public files...'))
-    async for file_path in app.assets.copytree(Path('public') / 'static', app.project.configuration.www_directory_path):
+    logging.getLogger(__name__).info(
+        app.localizer._("Generating static public files...")
+    )
+    async for file_path in app.assets.copytree(
+        Path("public") / "static", app.project.configuration.www_directory_path
+    ):
         await app.renderer.render_file(
             file_path,
             job_context=job_context,
         )
 
 
 async def _generate_entity_type_list_html(
     job_context: GenerationContext,
     locale: str,
     entity_type: type[Entity],
 ) -> None:
     app = job_context.app
     entity_type_name_fs = camel_case_to_kebab_case(get_entity_type_name(entity_type))
-    entity_type_path = app.project.configuration.localize_www_directory_path(locale) / entity_type_name_fs
-    template = app.jinja2_environment.select_template([
-        f'entity/page-list--{entity_type_name_fs}.html.j2',
-        'entity/page-list.html.j2',
-    ])
+    entity_type_path = (
+        app.project.configuration.localize_www_directory_path(locale)
+        / entity_type_name_fs
+    )
+    template = app.jinja2_environment.select_template(
+        [
+            f"entity/page-list--{entity_type_name_fs}.html.j2",
+            "entity/page-list.html.j2",
+        ]
+    )
     rendered_html = await template.render_async(
         job_context=job_context,
-        localizer=app.localizers[locale],
-        page_resource=f'/{entity_type_name_fs}/index.html',
+        localizer=await app.localizers.get(locale),
+        page_resource=f"/{entity_type_name_fs}/index.html",
         entity_type=entity_type,
         entities=app.project.ancestry[entity_type],
     )
     async with await create_html_resource(entity_type_path) as f:
         await f.write(rendered_html)
 
 
 async def _generate_entity_type_list_json(
     job_context: GenerationContext,
     entity_type: type[Entity & LinkedDataDumpable],
 ) -> None:
     app = job_context.app
     entity_type_name = get_entity_type_name(entity_type)
     entity_type_name_fs = camel_case_to_kebab_case(get_entity_type_name(entity_type))
-    entity_type_path = app.project.configuration.www_directory_path / entity_type_name_fs
+    entity_type_path = (
+        app.project.configuration.www_directory_path / entity_type_name_fs
+    )
     data: DictDump[Dump] = {
-        '$schema': app.static_url_generator.generate(f'schema.json#/definitions/response/{upper_camel_case_to_lower_camel_case(entity_type_name)}Collection', absolute=True),
-        'collection': []
+        "$schema": app.static_url_generator.generate(
+            f"schema.json#/definitions/response/{upper_camel_case_to_lower_camel_case(entity_type_name)}Collection",
+            absolute=True,
+        ),
+        "collection": [],
     }
     for entity in app.project.ancestry[entity_type]:
-        cast(list[str], data['collection']).append(
+        cast(list[str], data["collection"]).append(
             app.url_generator.generate(
                 entity,
-                'application/json',
+                "application/json",
                 absolute=True,
-            ))
+            )
+        )
     rendered_json = json.dumps(data)
     async with await create_json_resource(entity_type_path) as f:
         await f.write(rendered_json)
 
 
 async def _generate_entity_html(
     job_context: GenerationContext,
     locale: str,
     entity_type: type[Entity],
     entity_id: str,
 ) -> None:
     app = job_context.app
     entity = app.project.ancestry[entity_type][entity_id]
     entity_type_name_fs = camel_case_to_kebab_case(get_entity_type_name(entity))
-    entity_path = app.project.configuration.localize_www_directory_path(locale) / entity_type_name_fs / entity.id
-    rendered_html = await app.jinja2_environment.select_template([
-        f'entity/page--{entity_type_name_fs}.html.j2',
-        'entity/page.html.j2',
-    ]).render_async(
+    entity_path = (
+        app.project.configuration.localize_www_directory_path(locale)
+        / entity_type_name_fs
+        / entity.id
+    )
+    rendered_html = await app.jinja2_environment.select_template(
+        [
+            f"entity/page--{entity_type_name_fs}.html.j2",
+            "entity/page.html.j2",
+        ]
+    ).render_async(
         job_context=job_context,
-        localizer=app.localizers[locale],
+        localizer=await app.localizers.get(locale),
         page_resource=entity,
         entity_type=entity.type,
         entity=entity,
     )
     async with await create_html_resource(entity_path) as f:
         await f.write(rendered_html)
 
@@ -276,86 +355,108 @@
 async def _generate_entity_json(
     job_context: GenerationContext,
     entity_type: type[Entity & LinkedDataDumpable],
     entity_id: str,
 ) -> None:
     app = job_context.app
     entity_type_name_fs = camel_case_to_kebab_case(get_entity_type_name(entity_type))
-    entity_path = app.project.configuration.www_directory_path / entity_type_name_fs / entity_id
-    entity = cast('Entity & LinkedDataDumpable', app.project.ancestry[entity_type][entity_id])
+    entity_path = (
+        app.project.configuration.www_directory_path / entity_type_name_fs / entity_id
+    )
+    entity = cast(
+        "Entity & LinkedDataDumpable", app.project.ancestry[entity_type][entity_id]
+    )
     rendered_json = json.dumps(await entity.dump_linked_data(app))
     async with await create_json_resource(entity_path) as f:
         await f.write(rendered_json)
 
 
 async def _generate_sitemap(
     job_context: GenerationContext,
 ) -> None:
     app = job_context.app
-    sitemap_template = app.jinja2_environment.get_template('sitemap.xml.j2')
+    sitemap_template = app.jinja2_environment.get_template("sitemap.xml.j2")
     sitemaps = []
     sitemap: list[str] = []
     sitemap_length = 0
     sitemaps.append(sitemap)
     for locale in app.project.configuration.locales:
         for entity in app.project.ancestry:
             if isinstance(entity.id, GeneratedEntityId):
                 continue
             if not isinstance(entity, UserFacingEntity):
                 continue
 
-            sitemap.append(app.url_generator.generate(
-                entity,
-                absolute=True,
-                locale=locale,
-                media_type='text/html',
-            ))
+            sitemap.append(
+                app.url_generator.generate(
+                    entity,
+                    absolute=True,
+                    locale=locale,
+                    media_type="text/html",
+                )
+            )
             sitemap_length += 1
 
             if sitemap_length == 50_000:
                 sitemap = []
                 sitemap_length = 0
                 sitemaps.append(sitemap)
 
     sitemaps_urls = []
     for index, sitemap in enumerate(sitemaps):
-        sitemaps_urls.append(app.static_url_generator.generate(
-            f'sitemap-{index}.xml',
-            absolute=True,
-        ))
-        rendered_sitemap = await sitemap_template.render_async({
-            'urls': sitemap,
-        })
-        async with aiofiles.open(app.project.configuration.www_directory_path / f'sitemap-{index}.xml', 'w') as f:
+        sitemaps_urls.append(
+            app.static_url_generator.generate(
+                f"sitemap-{index}.xml",
+                absolute=True,
+            )
+        )
+        rendered_sitemap = await sitemap_template.render_async(
+            {
+                "urls": sitemap,
+            }
+        )
+        async with aiofiles.open(
+            app.project.configuration.www_directory_path / f"sitemap-{index}.xml", "w"
+        ) as f:
             await f.write(rendered_sitemap)
 
-    rendered_sitemap_index = await app.jinja2_environment.get_template('sitemap-index.xml.j2').render_async({
-        'sitemaps_urls': sitemaps_urls,
-    })
-    async with aiofiles.open(app.project.configuration.www_directory_path / 'sitemap.xml', 'w') as f:
+    rendered_sitemap_index = await app.jinja2_environment.get_template(
+        "sitemap-index.xml.j2"
+    ).render_async(
+        {
+            "sitemaps_urls": sitemaps_urls,
+        }
+    )
+    async with aiofiles.open(
+        app.project.configuration.www_directory_path / "sitemap.xml", "w"
+    ) as f:
         await f.write(rendered_sitemap_index)
 
 
 async def _generate_json_schema(
     job_context: GenerationContext,
 ) -> None:
     app = job_context.app
-    logging.getLogger(__name__).debug(app.localizer._('Generating JSON Schema...'))
+    logging.getLogger(__name__).debug(app.localizer._("Generating JSON Schema..."))
     schema = Schema(app)
     rendered_json = json.dumps(await schema.build())
-    async with await create_file(app.project.configuration.www_directory_path / 'schema.json') as f:
+    async with await create_file(
+        app.project.configuration.www_directory_path / "schema.json"
+    ) as f:
         await f.write(rendered_json)
 
 
 async def _generate_openapi(
     job_context: GenerationContext,
 ) -> None:
     app = job_context.app
-    logging.getLogger(__name__).debug(app.localizer._('Generating OpenAPI specification...'))
-    api_directory_path = app.project.configuration.www_directory_path / 'api'
+    logging.getLogger(__name__).debug(
+        app.localizer._("Generating OpenAPI specification...")
+    )
+    api_directory_path = app.project.configuration.www_directory_path / "api"
     rendered_json = json.dumps(await Specification(app).build())
     async with await create_json_resource(api_directory_path) as f:
         await f.write(rendered_json)
 
 
 def _get_entity_type_jinja2_name(entity_type_name: str) -> str:
-    return camel_case_to_snake_case(entity_type_name).replace('.', '__')
+    return camel_case_to_snake_case(entity_type_name).replace(".", "__")
```

### Comparing `betty-0.3.3/betty/gramps/loader.py` & `betty-0.3.4/betty/gramps/loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide an API to load `Gramps <https://gramps-project.org>`_ family trees into Betty ancestries.
 """
+
 from __future__ import annotations
 
 import gzip
 import re
 import tarfile
 from collections import defaultdict
 from contextlib import suppress
@@ -17,20 +18,67 @@
 from aiofiles.tempfile import TemporaryDirectory
 from geopy import Point
 
 from betty.gramps.error import GrampsError
 from betty.locale import DateRange, Datey, Date, Str, Localizer
 from betty.media_type import MediaType
 from betty.model import Entity, EntityGraphBuilder, AliasedEntity, AliasableEntity
-from betty.model.ancestry import Ancestry, Note, File, Source, Citation, Place, Event, Person, PersonName, Subject, \
-    Witness, Beneficiary, Attendee, Presence, PlaceName, Enclosure, HasLinks, Link, HasFiles, HasCitations, \
-    HasPrivacy, Speaker, Celebrant, Organizer, HasNotes
-from betty.model.event_type import Birth, Baptism, Adoption, Cremation, Death, Funeral, Burial, Will, Engagement, \
-    Marriage, MarriageAnnouncement, Divorce, DivorceAnnouncement, Residence, Immigration, Emigration, Occupation, \
-    Retirement, Correspondence, Confirmation, Missing, UnknownEventType, EventType, Conference
+from betty.model.ancestry import (
+    Ancestry,
+    Note,
+    File,
+    Source,
+    Citation,
+    Place,
+    Event,
+    Person,
+    PersonName,
+    Subject,
+    Witness,
+    Beneficiary,
+    Attendee,
+    Presence,
+    PlaceName,
+    Enclosure,
+    HasLinks,
+    Link,
+    HasFiles,
+    HasCitations,
+    HasPrivacy,
+    Speaker,
+    Celebrant,
+    Organizer,
+    HasNotes,
+)
+from betty.model.event_type import (
+    Birth,
+    Baptism,
+    Adoption,
+    Cremation,
+    Death,
+    Funeral,
+    Burial,
+    Will,
+    Engagement,
+    Marriage,
+    MarriageAnnouncement,
+    Divorce,
+    DivorceAnnouncement,
+    Residence,
+    Immigration,
+    Emigration,
+    Occupation,
+    Retirement,
+    Correspondence,
+    Confirmation,
+    Missing,
+    UnknownEventType,
+    EventType,
+    Conference,
+)
 from betty.path import rootname
 from betty.project import Project
 from betty.warnings import deprecate
 
 
 class GrampsLoadFileError(GrampsError, RuntimeError):
     pass
@@ -50,15 +98,15 @@
         project_or_ancestry: Project | Ancestry,
         *,
         localizer: Localizer,
     ):
         super().__init__()
         if isinstance(project_or_ancestry, Ancestry):
             deprecate(
-                f'Initializing {type(self)} with {Ancestry} is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, provide {Project}.',
+                f"Initializing {type(self)} with {Ancestry} is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, provide {Project}.",
                 stacklevel=2,
             )
             self._ancestry = project_or_ancestry
             self._project = None
         else:
             self._ancestry = project_or_ancestry.ancestry
             self._project = project_or_ancestry
@@ -68,47 +116,53 @@
         self._gramps_tree_directory_path: Path | None = None
         self._loaded = False
         self._localizer = localizer
 
     async def load_file(self, file_path: Path) -> None:
         file_path = file_path.resolve()
         logger = getLogger(__name__)
-        logger.info(self._localizer._('Loading "{file_path}"...').format(
-            file_path=str(file_path),
-        ))
+        logger.info(
+            self._localizer._('Loading "{file_path}"...').format(
+                file_path=str(file_path),
+            )
+        )
 
         with suppress(GrampsLoadFileError):
             await self.load_gpkg(file_path)
             return
 
         with suppress(GrampsLoadFileError):
             await self.load_gramps(file_path)
             return
 
         try:
             async with aiofiles.open(file_path) as f:
                 xml = await f.read()
         except FileNotFoundError:
-            raise GrampsFileNotFoundError(Str._(
-                'Could not find the file "{file_path}".',
-                file_path=str(file_path),
-            )) from None
+            raise GrampsFileNotFoundError(
+                Str._(
+                    'Could not find the file "{file_path}".',
+                    file_path=str(file_path),
+                )
+            ) from None
         with suppress(GrampsLoadFileError):
             await self.load_xml(xml, Path(file_path.anchor))
             return
 
-        raise GrampsLoadFileError(Str._(
-            'Could not load "{file_path}" as a *.gpkg, a *.gramps, or an *.xml family tree.',
-            file_path=str(file_path),
-        ))
+        raise GrampsLoadFileError(
+            Str._(
+                'Could not load "{file_path}" as a *.gpkg, a *.gramps, or an *.xml family tree.',
+                file_path=str(file_path),
+            )
+        )
 
     async def load_gramps(self, gramps_path: Path) -> None:
         gramps_path = gramps_path.resolve()
         try:
-            with gzip.open(gramps_path, mode='r') as f:
+            with gzip.open(gramps_path, mode="r") as f:
                 xml: str = f.read()  # type: ignore[assignment]
             await self.load_xml(
                 xml,
                 rootname(gramps_path),
             )
         except OSError as e:
             raise GrampsLoadFileError(Str.plain(e))
@@ -118,281 +172,309 @@
         try:
             tar_file: IO[bytes] = gzip.open(gpkg_path)  # type: ignore[assignment]
             try:
                 async with TemporaryDirectory() as cache_directory_path_str:
                     tarfile.open(
                         fileobj=tar_file,
                     ).extractall(cache_directory_path_str)
-                    await self.load_gramps(Path(cache_directory_path_str) / 'data.gramps')
+                    await self.load_gramps(
+                        Path(cache_directory_path_str) / "data.gramps"
+                    )
             except tarfile.ReadError:
-                raise GrampsLoadFileError(Str._(
-                    'Could not extract {file_path} as a tar (*.tar) file after extracting the outer gzip (*.gz) file.',
-                    file_path=str(gpkg_path),
-                ))
+                raise GrampsLoadFileError(
+                    Str._(
+                        "Could not extract {file_path} as a tar (*.tar) file after extracting the outer gzip (*.gz) file.",
+                        file_path=str(gpkg_path),
+                    )
+                )
         except OSError:
-            raise GrampsLoadFileError(Str._(
-                'Could not extract {file_path} as a gzip (*.gz) file.',
-                file_path=str(gpkg_path),
-            ))
+            raise GrampsLoadFileError(
+                Str._(
+                    "Could not extract {file_path} as a gzip (*.gz) file.",
+                    file_path=str(gpkg_path),
+                )
+            )
 
     async def load_xml(self, xml: str | Path, gramps_tree_directory_path: Path) -> None:
         if isinstance(xml, Path):
             async with aiofiles.open(xml) as f:
                 xml = await f.read()
         try:
-            tree = ElementTree.ElementTree(ElementTree.fromstring(
-                xml,
-            ))
+            tree = ElementTree.ElementTree(
+                ElementTree.fromstring(
+                    xml,
+                )
+            )
         except ElementTree.ParseError as e:
             raise GrampsLoadFileError(Str.plain(e))
         await self.load_tree(tree, gramps_tree_directory_path)
 
-    async def load_tree(self, tree: ElementTree.ElementTree, gramps_tree_directory_path: Path) -> None:
+    async def load_tree(
+        self, tree: ElementTree.ElementTree, gramps_tree_directory_path: Path
+    ) -> None:
         if self._loaded:
-            raise RuntimeError('This loader has been used up.')
+            raise RuntimeError("This loader has been used up.")
 
         self._loaded = True
         self._tree = tree
         self._gramps_tree_directory_path = gramps_tree_directory_path.resolve()
 
         logger = getLogger(__name__)
 
         database = self._tree.getroot()
 
         self._load_notes(database)
         # @todo Localize all log messages
-        logger.info(f'Loaded {self._added_entity_counts[Note]} notes.')
+        logger.info(f"Loaded {self._added_entity_counts[Note]} notes.")
         self._load_objects(database, self._gramps_tree_directory_path)
-        logger.info(f'Loaded {self._added_entity_counts[File]} files.')
+        logger.info(f"Loaded {self._added_entity_counts[File]} files.")
 
         self._load_repositories(database)
         repository_count = self._added_entity_counts[Source]
-        logger.info(f'Loaded {repository_count} repositories as sources.')
+        logger.info(f"Loaded {repository_count} repositories as sources.")
 
         self._load_sources(database)
-        logger.info(f'Loaded {self._added_entity_counts[Source] - repository_count} sources.')
+        logger.info(
+            f"Loaded {self._added_entity_counts[Source] - repository_count} sources."
+        )
 
         self._load_citations(database)
-        logger.info(f'Loaded {self._added_entity_counts[Citation]} citations.')
+        logger.info(f"Loaded {self._added_entity_counts[Citation]} citations.")
 
         self._load_places(database)
-        logger.info(f'Loaded {self._added_entity_counts[Place]} places.')
+        logger.info(f"Loaded {self._added_entity_counts[Place]} places.")
 
         self._load_events(database)
-        logger.info(f'Loaded {self._added_entity_counts[Event]} events.')
+        logger.info(f"Loaded {self._added_entity_counts[Event]} events.")
 
         self._load_people(database)
-        logger.info(f'Loaded {self._added_entity_counts[Person]} people.')
+        logger.info(f"Loaded {self._added_entity_counts[Person]} people.")
 
         self._load_families(database)
 
         self._ancestry.add_unchecked_graph(*self._ancestry_builder.build())
 
     def add_entity(self, entity: AliasableEntity[Entity]) -> None:
         self._ancestry_builder.add_entity(entity)
         self._added_entity_counts[entity.type] += 1
 
     def add_association(self, *args: Any, **kwargs: Any) -> None:
         self._ancestry_builder.add_association(*args, **kwargs)
 
     _NS = {
-        'ns': 'http://gramps-project.org/xml/1.7.1/',
+        "ns": "http://gramps-project.org/xml/1.7.1/",
     }
 
-    def _xpath(self, element: ElementTree.Element, selector: str) -> list[ElementTree.Element]:
+    def _xpath(
+        self, element: ElementTree.Element, selector: str
+    ) -> list[ElementTree.Element]:
         return element.findall(selector, namespaces=self._NS)
 
-    def _xpath1(self, element: ElementTree.Element, selector: str) -> ElementTree.Element:
+    def _xpath1(
+        self, element: ElementTree.Element, selector: str
+    ) -> ElementTree.Element:
         found_element = element.find(selector, namespaces=self._NS)
         if found_element is None:
-            raise XPathError(Str.plain(
-                'Cannot find an element "{selector}" within {element}.',
-                selector=selector,
-                element=str(element),
-            ))
+            raise XPathError(
+                Str.plain(
+                    'Cannot find an element "{selector}" within {element}.',
+                    selector=selector,
+                    element=str(element),
+                )
+            )
         return found_element
 
-    _DATE_PATTERN = re.compile(r'^.{4}((-.{2})?-.{2})?$')
-    _DATE_PART_PATTERN = re.compile(r'^\d+$')
+    _DATE_PATTERN = re.compile(r"^.{4}((-.{2})?-.{2})?$")
+    _DATE_PART_PATTERN = re.compile(r"^\d+$")
 
     def _load_date(self, element: ElementTree.Element) -> Datey | None:
         with suppress(XPathError):
-            dateval_element = self._xpath1(element, './ns:dateval')
-            if dateval_element.get('cformat') is None:
-                dateval_type = dateval_element.get('type')
+            dateval_element = self._xpath1(element, "./ns:dateval")
+            if dateval_element.get("cformat") is None:
+                dateval_type = dateval_element.get("type")
                 if dateval_type is None:
-                    return self._load_dateval(dateval_element, 'val')
+                    return self._load_dateval(dateval_element, "val")
                 dateval_type = str(dateval_type)
-                if dateval_type == 'about':
-                    date = self._load_dateval(dateval_element, 'val')
+                if dateval_type == "about":
+                    date = self._load_dateval(dateval_element, "val")
                     if date is None:
                         return None
                     date.fuzzy = True
                     return date
-                if dateval_type == 'before':
+                if dateval_type == "before":
                     return DateRange(
                         None,
-                        self._load_dateval(dateval_element, 'val'),
+                        self._load_dateval(dateval_element, "val"),
                         end_is_boundary=True,
                     )
-                if dateval_type == 'after':
+                if dateval_type == "after":
                     return DateRange(
-                        self._load_dateval(dateval_element, 'val'),
+                        self._load_dateval(dateval_element, "val"),
                         start_is_boundary=True,
                     )
         with suppress(XPathError):
-            datespan_element = self._xpath1(element, './ns:datespan')
-            if datespan_element.get('cformat') is None:
+            datespan_element = self._xpath1(element, "./ns:datespan")
+            if datespan_element.get("cformat") is None:
                 return DateRange(
-                    self._load_dateval(datespan_element, 'start'),
-                    self._load_dateval(datespan_element, 'stop'),
+                    self._load_dateval(datespan_element, "start"),
+                    self._load_dateval(datespan_element, "stop"),
                 )
         with suppress(XPathError):
-            daterange_element = self._xpath1(element, './ns:daterange')
-            if daterange_element.get('cformat') is None:
+            daterange_element = self._xpath1(element, "./ns:daterange")
+            if daterange_element.get("cformat") is None:
                 return DateRange(
-                    self._load_dateval(daterange_element, 'start'),
-                    self._load_dateval(daterange_element, 'stop'),
+                    self._load_dateval(daterange_element, "start"),
+                    self._load_dateval(daterange_element, "stop"),
                     start_is_boundary=True,
                     end_is_boundary=True,
                 )
         return None
 
-    def _load_dateval(self, element: ElementTree.Element, value_attribute_name: str) -> Date | None:
+    def _load_dateval(
+        self, element: ElementTree.Element, value_attribute_name: str
+    ) -> Date | None:
         dateval = str(element.get(value_attribute_name))
         if self._DATE_PATTERN.fullmatch(dateval):
             date_parts: tuple[int | None, int | None, int | None] = tuple(  # type: ignore[assignment]
-                int(part)
-                if self._DATE_PART_PATTERN.fullmatch(part) and int(part) > 0
-                else None
-                for part
-                in dateval.split('-')
+                (
+                    int(part)
+                    if self._DATE_PART_PATTERN.fullmatch(part) and int(part) > 0
+                    else None
+                )
+                for part in dateval.split("-")
             )
             date = Date(*date_parts)
-            dateval_quality = element.get('quality')
-            if dateval_quality == 'estimated':
+            dateval_quality = element.get("quality")
+            if dateval_quality == "estimated":
                 date.fuzzy = True
             return date
         return None
 
     def _load_notes(self, database: ElementTree.Element) -> None:
-        for element in self._xpath(database, './ns:notes/ns:note'):
+        for element in self._xpath(database, "./ns:notes/ns:note"):
             self._load_note(element)
 
     def _load_note(self, element: ElementTree.Element) -> None:
-        note_handle = element.get('handle')
-        note_id = element.get('id')
+        note_handle = element.get("handle")
+        note_id = element.get("id")
         assert note_id is not None
-        text_element = self._xpath1(element, './ns:text')
+        text_element = self._xpath1(element, "./ns:text")
         assert text_element is not None
         text = str(text_element.text)
         note = Note(
             id=note_id,
             text=text,
         )
-        if element.get('priv') == '1':
+        if element.get("priv") == "1":
             note.private = True
         self.add_entity(AliasedEntity(note, note_handle))
 
-    def _load_noteref(self, owner: AliasableEntity[HasNotes & Entity], element: ElementTree.Element) -> None:
-        note_handles = self._load_handles('noteref', element)
+    def _load_noteref(
+        self, owner: AliasableEntity[HasNotes & Entity], element: ElementTree.Element
+    ) -> None:
+        note_handles = self._load_handles("noteref", element)
         for note_handle in note_handles:
-            self.add_association(owner.type, owner.id, 'notes', Note, note_handle)
+            self.add_association(owner.type, owner.id, "notes", Note, note_handle)
 
-    def _load_objects(self, database: ElementTree.Element, gramps_tree_directory_path: Path) -> None:
-        for element in self._xpath(database, './ns:objects/ns:object'):
+    def _load_objects(
+        self, database: ElementTree.Element, gramps_tree_directory_path: Path
+    ) -> None:
+        for element in self._xpath(database, "./ns:objects/ns:object"):
             self._load_object(element, gramps_tree_directory_path)
 
-    def _load_object(self, element: ElementTree.Element, gramps_tree_directory_path: Path) -> None:
-        file_handle = element.get('handle')
-        file_id = element.get('id')
-        file_element = self._xpath1(element, './ns:file')
-        src = file_element.get('src')
+    def _load_object(
+        self, element: ElementTree.Element, gramps_tree_directory_path: Path
+    ) -> None:
+        file_handle = element.get("handle")
+        file_id = element.get("id")
+        file_element = self._xpath1(element, "./ns:file")
+        src = file_element.get("src")
         assert src is not None
         file_path = gramps_tree_directory_path / src
         file = File(
             id=file_id,
             path=file_path,
         )
-        mime = file_element.get('mime')
+        mime = file_element.get("mime")
         assert mime is not None
         file.media_type = MediaType(mime)
-        description = file_element.get('description')
+        description = file_element.get("description")
         if description:
             file.description = description
-        if element.get('priv') == '1':
+        if element.get("priv") == "1":
             file.private = True
         aliased_file = AliasedEntity(file, file_handle)
 
-        self._load_attributes(file, element, 'attribute')
+        self._load_attributes(file, element, "attribute")
 
         self.add_entity(
             aliased_file,  # type: ignore[arg-type]
         )
-        for citation_handle in self._load_handles('citationref', element):
-            self.add_association(File, file_handle, 'citations', Citation, citation_handle)
+        for citation_handle in self._load_handles("citationref", element):
+            self.add_association(
+                File, file_handle, "citations", Citation, citation_handle
+            )
         self._load_noteref(
             aliased_file,  # type: ignore[arg-type]
             element,
         )
 
     def _load_people(self, database: ElementTree.Element) -> None:
-        for element in self._xpath(database, './ns:people/ns:person'):
+        for element in self._xpath(database, "./ns:people/ns:person"):
             self._load_person(element)
 
     def _load_person(self, element: ElementTree.Element) -> None:
-        person_handle = element.get('handle')
+        person_handle = element.get("handle")
         assert person_handle is not None
-        person = Person(id=element.get('id'))
+        person = Person(id=element.get("id"))
 
-        name_elements = sorted(self._xpath(element, './ns:name'), key=lambda x: x.get('alt') == '1')
+        name_elements = sorted(
+            self._xpath(element, "./ns:name"), key=lambda x: x.get("alt") == "1"
+        )
         person_names = []
         for name_element in name_elements:
-            is_alternative = name_element.get('alt') == '1'
+            is_alternative = name_element.get("alt") == "1"
             try:
-                individual_name = self._xpath1(name_element, './ns:first').text
+                individual_name = self._xpath1(name_element, "./ns:first").text
             except XPathError:
                 individual_name = None
             surname_elements = [
                 surname_element
-                for surname_element
-                in self._xpath(
-                    name_element,
-                    './ns:surname'
-                )
+                for surname_element in self._xpath(name_element, "./ns:surname")
                 if surname_element.text is not None
             ]
             if surname_elements:
                 for surname_element in surname_elements:
                     if not is_alternative:
-                        is_alternative = surname_element.get('prim') == '0'
+                        is_alternative = surname_element.get("prim") == "0"
                     affiliation_name = surname_element.text
-                    surname_prefix = surname_element.get('prefix')
+                    surname_prefix = surname_element.get("prefix")
                     if surname_prefix is not None:
-                        affiliation_name = '%s %s' % (
-                            surname_prefix, affiliation_name)
+                        affiliation_name = "%s %s" % (surname_prefix, affiliation_name)
                     person_name = PersonName(
                         individual=individual_name,
                         affiliation=affiliation_name,
                     )
                     self._load_citationref(person_name, name_element)
                     person_names.append((person_name, is_alternative))
             elif individual_name is not None:
                 person_name = PersonName(individual=individual_name)
                 self._load_citationref(person_name, name_element)
                 person_names.append((person_name, is_alternative))
         for person_name, _ in sorted(person_names, key=lambda x: x[1]):
             self.add_entity(person_name)
-            self.add_association(Person, person_handle, 'names', PersonName, person_name.id)
+            self.add_association(
+                Person, person_handle, "names", PersonName, person_name.id
+            )
 
         self._load_eventrefs(person_handle, element)
-        if element.get('priv') == '1':
+        if element.get("priv") == "1":
             person.private = True
 
-        self._load_attributes(person, element, 'attribute')
+        self._load_attributes(person, element, "attribute")
 
         aliased_person = AliasedEntity(person, person_handle)
         self._load_citationref(
             aliased_person,  # type: ignore[arg-type]
             element,
         )
         self._load_objref(
@@ -405,104 +487,110 @@
         )
         self._load_urls(person, element)
         self.add_entity(
             aliased_person,  # type: ignore[arg-type]
         )
 
     def _load_families(self, database: ElementTree.Element) -> None:
-        for element in self._xpath(database, './ns:families/ns:family'):
+        for element in self._xpath(database, "./ns:families/ns:family"):
             self._load_family(element)
 
     def _load_family(self, element: ElementTree.Element) -> None:
         parent_handles = []
 
         # Load the father.
-        father_handle = self._load_handle('father', element)
+        father_handle = self._load_handle("father", element)
         if father_handle is not None:
             self._load_eventrefs(father_handle, element)
             parent_handles.append(father_handle)
 
         # Load the mother.
-        mother_handle = self._load_handle('mother', element)
+        mother_handle = self._load_handle("mother", element)
         if mother_handle is not None:
             self._load_eventrefs(mother_handle, element)
             parent_handles.append(mother_handle)
 
         # Load the children.
-        child_handles = self._load_handles('childref', element)
+        child_handles = self._load_handles("childref", element)
         for child_handle in child_handles:
             for parent_handle in parent_handles:
-                self.add_association(Person, child_handle, 'parents', Person, parent_handle)
+                self.add_association(
+                    Person, child_handle, "parents", Person, parent_handle
+                )
 
     def _load_eventrefs(self, person_id: str, element: ElementTree.Element) -> None:
-        eventrefs = self._xpath(element, './ns:eventref')
+        eventrefs = self._xpath(element, "./ns:eventref")
         for eventref in eventrefs:
             self._load_eventref(person_id, eventref)
 
     _PRESENCE_ROLE_MAP = {
-        'Primary': Subject(),
-        'Family': Subject(),
-        'Witness': Witness(),
-        'Beneficiary': Beneficiary(),
-        'Speaker': Speaker(),
-        'Celebrant': Celebrant(),
-        'Organizer': Organizer(),
-        'Attendee': Attendee(),
-        'Unknown': Attendee(),
+        "Primary": Subject(),
+        "Family": Subject(),
+        "Witness": Witness(),
+        "Beneficiary": Beneficiary(),
+        "Speaker": Speaker(),
+        "Celebrant": Celebrant(),
+        "Organizer": Organizer(),
+        "Attendee": Attendee(),
+        "Unknown": Attendee(),
     }
 
     def _load_eventref(self, person_id: str, eventref: ElementTree.Element) -> None:
-        event_handle = eventref.get('hlink')
+        event_handle = eventref.get("hlink")
         assert event_handle is not None
-        gramps_presence_role = cast(str, eventref.get('role'))
+        gramps_presence_role = cast(str, eventref.get("role"))
 
         try:
             role = self._PRESENCE_ROLE_MAP[gramps_presence_role]
         except KeyError:
             role = Attendee()
-            getLogger(__name__).warning(self._localizer._(
-                'Betty is unfamiliar with person "{person_id}"\'s Gramps presence role of "{gramps_presence_role}" for the event with Gramps handle "{event_handle}". The role was imported, but set to "{betty_presence_role}".',
-            ).format(
-                person_id=person_id,
-                event_handle=event_handle,
-                gramps_presence_role=gramps_presence_role,
-                betty_presence_role=role.label,
-            ))
+            getLogger(__name__).warning(
+                self._localizer._(
+                    'Betty is unfamiliar with person "{person_id}"\'s Gramps presence role of "{gramps_presence_role}" for the event with Gramps handle "{event_handle}". The role was imported, but set to "{betty_presence_role}".',
+                ).format(
+                    person_id=person_id,
+                    event_handle=event_handle,
+                    gramps_presence_role=gramps_presence_role,
+                    betty_presence_role=role.label,
+                )
+            )
 
         presence = Presence(None, role, None)
-        if eventref.get('priv') == '1':
+        if eventref.get("priv") == "1":
             presence.private = True
 
-        self._load_attributes(presence, eventref, 'attribute')
+        self._load_attributes(presence, eventref, "attribute")
 
         self.add_entity(presence)
-        self.add_association(Presence, presence.id, 'person', Person, person_id)
-        self.add_association(Presence, presence.id, 'event', Event, event_handle)
+        self.add_association(Presence, presence.id, "person", Person, person_id)
+        self.add_association(Presence, presence.id, "event", Event, event_handle)
 
     def _load_places(self, database: ElementTree.Element) -> None:
-        for element in self._xpath(database, './ns:places/ns:placeobj'):
+        for element in self._xpath(database, "./ns:places/ns:placeobj"):
             self._load_place(element)
 
     def _load_place(self, element: ElementTree.Element) -> None:
-        place_handle = element.get('handle')
+        place_handle = element.get("handle")
         names = []
-        for name_element in self._xpath(element, './ns:pname'):
+        for name_element in self._xpath(element, "./ns:pname"):
             # The Gramps language is a single ISO language code, which is a valid BCP 47 locale.
-            language = name_element.get('lang')
+            language = name_element.get("lang")
             date = self._load_date(name_element)
-            name = name_element.get('value')
+            name = name_element.get("value")
             assert name is not None
-            names.append(PlaceName(
-                name=name,
-                locale=language,
-                date=date,
-            ))
+            names.append(
+                PlaceName(
+                    name=name,
+                    locale=language,
+                    date=date,
+                )
+            )
 
         place = Place(
-            id=element.get('id'),
+            id=element.get("id"),
             names=names,
         )
 
         coordinates = self._load_coordinates(element)
         if coordinates:
             place.coordinates = coordinates
 
@@ -515,102 +603,116 @@
             element,
         )
 
         self.add_entity(
             aliased_place,  # type: ignore[arg-type]
         )
 
-        for enclosed_by_handle in self._load_handles('placeref', element):
-            aliased_enclosure = AliasedEntity(Enclosure(encloses=None, enclosed_by=None))
+        for enclosed_by_handle in self._load_handles("placeref", element):
+            aliased_enclosure = AliasedEntity(
+                Enclosure(encloses=None, enclosed_by=None)
+            )
             self.add_entity(
                 aliased_enclosure,  # type: ignore[arg-type]
             )
-            self.add_association(Enclosure, aliased_enclosure.id, 'encloses', Place, place_handle)
-            self.add_association(Enclosure, aliased_enclosure.id, 'enclosed_by', Place, enclosed_by_handle)
+            self.add_association(
+                Enclosure, aliased_enclosure.id, "encloses", Place, place_handle
+            )
+            self.add_association(
+                Enclosure,
+                aliased_enclosure.id,
+                "enclosed_by",
+                Place,
+                enclosed_by_handle,
+            )
 
     def _load_coordinates(self, element: ElementTree.Element) -> Point | None:
         with suppress(XPathError):
-            coord_element = self._xpath1(element, './ns:coord')
+            coord_element = self._xpath1(element, "./ns:coord")
 
             coordinates = f'{coord_element.get("lat")}; {coord_element.get("long")}'
             try:
                 return Point.from_string(coordinates)
             except ValueError:
-                getLogger(__name__).warning(self._localizer._(
-                    'Cannot load coordinates "{coordinates}", because they are in an unknown format.',
-                ).format(
-                    coordinates=coordinates,
-                ))
+                getLogger(__name__).warning(
+                    self._localizer._(
+                        'Cannot load coordinates "{coordinates}", because they are in an unknown format.',
+                    ).format(
+                        coordinates=coordinates,
+                    )
+                )
         return None
 
     def _load_events(self, database: ElementTree.Element) -> None:
-        for element in self._xpath(database, './ns:events/ns:event'):
+        for element in self._xpath(database, "./ns:events/ns:event"):
             self._load_event(element)
 
     _EVENT_TYPE_MAP = {
-        'Birth': Birth,
-        'Baptism': Baptism,
-        'Adopted': Adoption,
-        'Cremation': Cremation,
-        'Death': Death,
-        'Funeral': Funeral,
-        'Burial': Burial,
-        'Will': Will,
-        'Engagement': Engagement,
-        'Marriage': Marriage,
-        'Marriage Banns': MarriageAnnouncement,
-        'Divorce': Divorce,
-        'Divorce Filing': DivorceAnnouncement,
-        'Residence': Residence,
-        'Immigration': Immigration,
-        'Emigration': Emigration,
-        'Occupation': Occupation,
-        'Retirement': Retirement,
-        'Correspondence': Correspondence,
-        'Confirmation': Confirmation,
-        'Missing': Missing,
-        'Conference': Conference,
+        "Birth": Birth,
+        "Baptism": Baptism,
+        "Adopted": Adoption,
+        "Cremation": Cremation,
+        "Death": Death,
+        "Funeral": Funeral,
+        "Burial": Burial,
+        "Will": Will,
+        "Engagement": Engagement,
+        "Marriage": Marriage,
+        "Marriage Banns": MarriageAnnouncement,
+        "Divorce": Divorce,
+        "Divorce Filing": DivorceAnnouncement,
+        "Residence": Residence,
+        "Immigration": Immigration,
+        "Emigration": Emigration,
+        "Occupation": Occupation,
+        "Retirement": Retirement,
+        "Correspondence": Correspondence,
+        "Confirmation": Confirmation,
+        "Missing": Missing,
+        "Conference": Conference,
     }
 
     def _load_event(self, element: ElementTree.Element) -> None:
-        event_handle = element.get('handle')
-        event_id = element.get('id')
+        event_handle = element.get("handle")
+        event_id = element.get("id")
         assert event_id is not None
-        gramps_type = self._xpath1(element, './ns:type').text
+        gramps_type = self._xpath1(element, "./ns:type").text
         assert gramps_type is not None
 
         try:
             event_type: type[EventType] = self._EVENT_TYPE_MAP[gramps_type]
         except KeyError:
             event_type = UnknownEventType
-            getLogger(__name__).warning(self._localizer._(
-                'Betty is unfamiliar with Gramps event "{event_id}"\'s type of "{gramps_event_type}". The event was imported, but its type was set to "{betty_event_type}".',
-            ).format(
-                event_id=event_id,
-                gramps_event_type=gramps_type,
-                betty_event_type=event_type.label().localize(self._localizer),
-            ))
+            getLogger(__name__).warning(
+                self._localizer._(
+                    'Betty is unfamiliar with Gramps event "{event_id}"\'s type of "{gramps_event_type}". The event was imported, but its type was set to "{betty_event_type}".',
+                ).format(
+                    event_id=event_id,
+                    gramps_event_type=gramps_type,
+                    betty_event_type=event_type.label().localize(self._localizer),
+                )
+            )
 
         event = Event(
             id=event_id,
             event_type=event_type,
         )
 
         event.date = self._load_date(element)
 
         # Load the event place.
-        place_handle = self._load_handle('place', element)
+        place_handle = self._load_handle("place", element)
         if place_handle is not None:
-            self.add_association(Event, event_handle, 'place', Place, place_handle)
+            self.add_association(Event, event_handle, "place", Place, place_handle)
 
         # Load the description.
         with suppress(XPathError):
-            event.description = self._xpath1(element, './ns:description').text
+            event.description = self._xpath1(element, "./ns:description").text
 
-        if element.get('priv') == '1':
+        if element.get("priv") == "1":
             event.private = True
 
         aliased_event = AliasedEntity(event, event_handle)
         self._load_objref(
             aliased_event,  # type: ignore[arg-type]
             element,
         )
@@ -619,74 +721,76 @@
             element,
         )
         self._load_noteref(
             aliased_event,  # type: ignore[arg-type]
             element,
         )
 
-        self._load_attributes(event, element, 'attribute')
+        self._load_attributes(event, element, "attribute")
 
         self.add_entity(
             aliased_event,  # type: ignore[arg-type]
         )
 
     def _load_repositories(self, database: ElementTree.Element) -> None:
-        for element in self._xpath(database, './ns:repositories/ns:repository'):
+        for element in self._xpath(database, "./ns:repositories/ns:repository"):
             self._load_repository(element)
 
     def _load_repository(self, element: ElementTree.Element) -> None:
-        repository_source_handle = element.get('handle')
+        repository_source_handle = element.get("handle")
 
         source = Source(
-            id=element.get('id'),
-            name=self._xpath1(element, './ns:rname').text,
+            id=element.get("id"),
+            name=self._xpath1(element, "./ns:rname").text,
         )
 
         self._load_urls(source, element)
         aliased_source = AliasedEntity(source, repository_source_handle)
         self._load_noteref(
             aliased_source,  # type: ignore[arg-type]
             element,
         )
         self.add_entity(
             aliased_source,  # type: ignore[arg-type]
         )
 
     def _load_sources(self, database: ElementTree.Element) -> None:
-        for element in self._xpath(database, './ns:sources/ns:source'):
+        for element in self._xpath(database, "./ns:sources/ns:source"):
             self._load_source(element)
 
     def _load_source(self, element: ElementTree.Element) -> None:
-        source_handle = element.get('handle')
+        source_handle = element.get("handle")
         try:
-            source_name = self._xpath1(element, './ns:stitle').text
+            source_name = self._xpath1(element, "./ns:stitle").text
         except XPathError:
             source_name = None
 
         source = Source(
-            id=element.get('id'),
+            id=element.get("id"),
             name=source_name,
         )
 
-        repository_source_handle = self._load_handle('reporef', element)
+        repository_source_handle = self._load_handle("reporef", element)
         if repository_source_handle is not None:
-            self.add_association(Source, source_handle, 'contained_by', Source, repository_source_handle)
+            self.add_association(
+                Source, source_handle, "contained_by", Source, repository_source_handle
+            )
 
         # Load the author.
         with suppress(XPathError):
-            source.author = self._xpath1(element, './ns:sauthor').text
+            source.author = self._xpath1(element, "./ns:sauthor").text
 
         # Load the publication info.
         with suppress(XPathError):
-            source.publisher = self._xpath1(element, './ns:spubinfo').text
+            source.publisher = self._xpath1(element, "./ns:spubinfo").text
 
-        if element.get('priv') == '1':
+        if element.get("priv") == "1":
             source.private = True
 
-        self._load_attributes(source, element, 'srcattribute')
+        self._load_attributes(source, element, "srcattribute")
 
         aliased_source = AliasedEntity(source, source_handle)
         self._load_objref(
             aliased_source,  # type: ignore[arg-type]
             element,
         )
         self._load_noteref(
@@ -694,95 +798,117 @@
             element,
         )
         self.add_entity(
             aliased_source,  # type: ignore[arg-type]
         )
 
     def _load_citations(self, database: ElementTree.Element) -> None:
-        for element in self._xpath(database, './ns:citations/ns:citation'):
+        for element in self._xpath(database, "./ns:citations/ns:citation"):
             self._load_citation(element)
 
     def _load_citation(self, element: ElementTree.Element) -> None:
-        citation_handle = element.get('handle')
-        source_handle = self._xpath1(element, './ns:sourceref').get('hlink')
+        citation_handle = element.get("handle")
+        source_handle = self._xpath1(element, "./ns:sourceref").get("hlink")
 
-        citation = Citation(id=element.get('id'))
-        self.add_association(Citation, citation_handle, 'source', Source, source_handle)
+        citation = Citation(id=element.get("id"))
+        self.add_association(Citation, citation_handle, "source", Source, source_handle)
 
         citation.date = self._load_date(element)
-        if element.get('priv') == '1':
+        if element.get("priv") == "1":
             citation.private = True
 
         with suppress(XPathError):
-            citation.location = Str.plain(self._xpath1(element, './ns:page').text)
+            citation.location = Str.plain(self._xpath1(element, "./ns:page").text)
 
         aliased_citation = AliasedEntity(citation, citation_handle)
         self._load_objref(
             aliased_citation,  # type: ignore[arg-type]
             element,
         )
 
-        self._load_attributes(citation, element, 'srcattribute')
+        self._load_attributes(citation, element, "srcattribute")
 
         self.add_entity(
             aliased_citation,  # type: ignore[arg-type]
         )
 
-    def _load_citationref(self, owner: AliasableEntity[HasCitations & Entity], element: ElementTree.Element) -> None:
-        for citation_handle in self._load_handles('citationref', element):
-            self.add_association(owner.type, owner.id, 'citations', Citation, citation_handle)
-
-    def _load_handles(self, handle_type: str, element: ElementTree.Element) -> Iterable[str]:
-        for citation_handle_element in self._xpath(element, f'./ns:{handle_type}'):
-            hlink = citation_handle_element.get('hlink')
+    def _load_citationref(
+        self,
+        owner: AliasableEntity[HasCitations & Entity],
+        element: ElementTree.Element,
+    ) -> None:
+        for citation_handle in self._load_handles("citationref", element):
+            self.add_association(
+                owner.type, owner.id, "citations", Citation, citation_handle
+            )
+
+    def _load_handles(
+        self, handle_type: str, element: ElementTree.Element
+    ) -> Iterable[str]:
+        for citation_handle_element in self._xpath(element, f"./ns:{handle_type}"):
+            hlink = citation_handle_element.get("hlink")
             if hlink:
                 yield hlink
 
-    def _load_handle(self, handle_type: str, element: ElementTree.Element) -> str | None:
-        for citation_handle_element in self._xpath(element, f'./ns:{handle_type}'):
-            return citation_handle_element.get('hlink')
+    def _load_handle(
+        self, handle_type: str, element: ElementTree.Element
+    ) -> str | None:
+        for citation_handle_element in self._xpath(element, f"./ns:{handle_type}"):
+            return citation_handle_element.get("hlink")
         return None
 
-    def _load_objref(self, owner: AliasableEntity[HasFiles & Entity], element: ElementTree.Element) -> None:
-        file_handles = self._load_handles('objref', element)
+    def _load_objref(
+        self, owner: AliasableEntity[HasFiles & Entity], element: ElementTree.Element
+    ) -> None:
+        file_handles = self._load_handles("objref", element)
         for file_handle in file_handles:
-            self.add_association(owner.type, owner.id, 'files', File, file_handle)
+            self.add_association(owner.type, owner.id, "files", File, file_handle)
 
     def _load_urls(self, owner: HasLinks, element: ElementTree.Element) -> None:
-        url_elements = self._xpath(element, './ns:url')
+        url_elements = self._xpath(element, "./ns:url")
         for url_element in url_elements:
-            link = Link(str(url_element.get('href')))
-            link.relationship = 'external'
-            link.label = url_element.get('description')
+            link = Link(str(url_element.get("href")))
+            link.relationship = "external"
+            link.label = url_element.get("description")
             owner.links.append(link)
 
-    def _load_attribute_privacy(self, entity: HasPrivacy & Entity, element: ElementTree.Element, tag: str) -> None:
-        privacy_value = self._load_attribute('privacy', element, tag)
+    def _load_attribute_privacy(
+        self, entity: HasPrivacy & Entity, element: ElementTree.Element, tag: str
+    ) -> None:
+        privacy_value = self._load_attribute("privacy", element, tag)
         if privacy_value is None:
             return
-        if privacy_value == 'private':
+        if privacy_value == "private":
             entity.private = True
             return
-        if privacy_value == 'public':
+        if privacy_value == "public":
             entity.public = True
             return
-        getLogger(__name__).warning(self._localizer._(
-            'The betty:privacy Gramps attribute must have a value of "public" or "private", but "{privacy_value}" was given for {entity_type} {entity_id} ({entity_label}), which was ignored.',
-        ).format(
-            privacy_value=privacy_value,
-            entity_type=entity.entity_type_label().localize(self._localizer),
-            entity_id=entity.id,
-            entity_label=entity.label.localize(self._localizer),
-        ))
+        getLogger(__name__).warning(
+            self._localizer._(
+                'The betty:privacy Gramps attribute must have a value of "public" or "private", but "{privacy_value}" was given for {entity_type} {entity_id} ({entity_label}), which was ignored.',
+            ).format(
+                privacy_value=privacy_value,
+                entity_type=entity.entity_type_label().localize(self._localizer),
+                entity_id=entity.id,
+                entity_label=entity.label.localize(self._localizer),
+            )
+        )
 
-    def _load_attribute(self, name: str, element: ElementTree.Element, tag: str) -> str | None:
-        prefixes = ['betty']
+    def _load_attribute(
+        self, name: str, element: ElementTree.Element, tag: str
+    ) -> str | None:
+        prefixes = ["betty"]
         if self._project is not None and self._project.configuration.name is not None:
-            prefixes.insert(0, f'betty-{self._project.configuration.name}')
+            prefixes.insert(0, f"betty-{self._project.configuration.name}")
         for prefix in prefixes:
             with suppress(XPathError):
-                return self._xpath1(element, f'./ns:{tag}[@type="{prefix}:{name}"]').get('value')
+                return self._xpath1(
+                    element, f'./ns:{tag}[@type="{prefix}:{name}"]'
+                ).get("value")
         return None
 
-    def _load_attributes(self, entity: Entity, element: ElementTree.Element, tag: str) -> None:
+    def _load_attributes(
+        self, entity: Entity, element: ElementTree.Element, tag: str
+    ) -> None:
         if isinstance(entity, HasPrivacy):
             self._load_attribute_privacy(entity, element, tag)
```

### Comparing `betty-0.3.3/betty/gui/__init__.py` & `betty-0.3.4/betty/gui/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provide the Graphical User Interface (GUI) for Betty Desktop."""
+
 from __future__ import annotations
 
 import pickle
 from collections.abc import AsyncIterator
 from contextlib import asynccontextmanager
 from typing import Any, TypeVar, Self
 
@@ -11,74 +12,73 @@
 from PyQt6.QtWidgets import QApplication, QWidget
 
 from betty.app import App
 from betty.gui.error import ExceptionError, _UnexpectedExceptionError
 from betty.locale import Str
 from betty.serde.format import FormatRepository
 
-QWidgetT = TypeVar('QWidgetT', bound=QWidget)
+QWidgetT = TypeVar("QWidgetT", bound=QWidget)
 
 
 def get_configuration_file_filter() -> Str:
     """
     Get the Qt file filter for project configuration files.
     """
     formats = FormatRepository()
     return Str._(
-        'Betty project configuration ({supported_formats})',
-        supported_formats=' '.join(
-            f'*.{extension}'
-            for format
-            in formats.formats
+        "Betty project configuration ({supported_formats})",
+        supported_formats=" ".join(
+            f"*.{extension}"
+            for format in formats.formats
             for extension in format.extensions
         ),
     )
 
 
 class GuiBuilder:
     def gui_build(self) -> QWidget:
         raise NotImplementedError(repr(self))
 
 
 def mark_valid(widget: QWidget) -> None:
     """
     Mark a widget as currently containing valid input.
     """
-    widget.setProperty('invalid', 'false')
+    widget.setProperty("invalid", "false")
     widget.setStyle(widget.style())
-    widget.setToolTip('')
+    widget.setToolTip("")
 
 
 def mark_invalid(widget: QWidget, reason: str) -> None:
     """
     Mark a widget as currently containing invalid input.
     """
-    widget.setProperty('invalid', 'true')
+    widget.setProperty("invalid", "true")
     widget.setStyle(widget.style())
     widget.setToolTip(reason)
 
 
 class BettyApplication(QApplication):
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self._app: App | None = None
-        self.setApplicationName('Betty')
+        self.setApplicationName("Betty")
         self.setStyleSheet(self._stylesheet())
 
     def _is_dark_mode(self) -> bool:
         palette = self.palette()
         window_lightness = palette.color(QPalette.ColorRole.Window).lightness()
         window_text_lightness = palette.color(QPalette.ColorRole.WindowText).lightness()
         return window_lightness < window_text_lightness
 
     def _stylesheet(self) -> str:
         if self._is_dark_mode():
-            caption_color = '#eeeeee'
+            caption_color = "#eeeeee"
         else:
-            caption_color = '#333333'
+            caption_color = "#333333"
         return f"""
             Caption {{
                 color: {caption_color};
                 font-size: 14px;
                 margin-bottom: 0.3em;
             }}
 
@@ -142,15 +142,21 @@
         self,
         error_type: type[Exception],
         pickled_error_message: bytes,
         parent: QObject,
         close_parent: bool,
     ) -> None:
         error_message = pickle.loads(pickled_error_message)
-        window = ExceptionError(self.app, error_message, error_type, parent=parent, close_parent=close_parent)
+        window = ExceptionError(
+            self.app,
+            error_message,
+            error_type,
+            parent=parent,
+            close_parent=close_parent,
+        )
         window.show()
 
     @pyqtSlot(
         type,
         str,
         str,
         QObject,
@@ -160,29 +166,36 @@
         self,
         error_type: type[Exception],
         error_message: str,
         error_traceback: str,
         parent: QObject,
         close_parent: bool,
     ) -> None:
-        window = _UnexpectedExceptionError(self.app, error_type, error_message, error_traceback, parent=parent, close_parent=close_parent)
+        window = _UnexpectedExceptionError(
+            self.app,
+            error_type,
+            error_message,
+            error_traceback,
+            parent=parent,
+            close_parent=close_parent,
+        )
         window.show()
 
     @classmethod
     def instance(cls) -> Self:
         qapp = QCoreApplication.instance()
         assert isinstance(qapp, cls)
         return qapp
 
     @asynccontextmanager
     async def with_app(self, app: App) -> AsyncIterator[Self]:
         if self._app is not None:
-            raise RuntimeError(f'This {type(self)} already has an {App}.')
+            raise RuntimeError(f"This {type(self)} already has an {App}.")
         self._app = app
         yield self
         self._app = None
 
     @property
     def app(self) -> App:
         if self._app is None:
-            raise RuntimeError(f'This {type(self)} does not have an {App} yet.')
+            raise RuntimeError(f"This {type(self)} does not have an {App} yet.")
         return self._app
```

### Comparing `betty-0.3.3/betty/gui/app.py` & `betty-0.3.4/betty/gui/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 """
 Provide the desktop application/Graphical User Interface.
 """
+
 import webbrowser
 from datetime import datetime
 from os import path
 from pathlib import Path
 from urllib.parse import urlencode
 
 from PyQt6.QtCore import Qt, QCoreApplication, QObject
 from PyQt6.QtGui import QIcon, QAction
-from PyQt6.QtWidgets import QFormLayout, QWidget, QVBoxLayout, QHBoxLayout, QFileDialog, QPushButton
+from PyQt6.QtWidgets import (
+    QFormLayout,
+    QWidget,
+    QVBoxLayout,
+    QHBoxLayout,
+    QFileDialog,
+    QPushButton,
+)
 
 from betty import about
 from betty.about import report
 from betty.app import App
 from betty.asyncio import wait_to_thread
 from betty.gui import get_configuration_file_filter
 from betty.gui.error import ExceptionCatcher
@@ -28,32 +36,42 @@
 class BettyPrimaryWindow(BettyMainWindow):
     def __init__(
         self,
         app: App,
         /,
     ):
         super().__init__(app)
-        self.setWindowIcon(QIcon(path.join(path.dirname(__file__), 'assets', 'public', 'static', 'betty-512x512.png')))
+        self.setWindowIcon(
+            QIcon(
+                path.join(
+                    path.dirname(__file__),
+                    "assets",
+                    "public",
+                    "static",
+                    "betty-512x512.png",
+                )
+            )
+        )
 
         menu_bar = self.menuBar()
         assert menu_bar is not None
 
-        betty_menu = menu_bar.addMenu('&Betty')
+        betty_menu = menu_bar.addMenu("&Betty")
         assert betty_menu is not None
         self.betty_menu = betty_menu
 
         self.new_project_action = QAction(self)
-        self.new_project_action.setShortcut('Ctrl+N')
+        self.new_project_action.setShortcut("Ctrl+N")
         self.new_project_action.triggered.connect(
             lambda _: self.new_project(),
         )
         betty_menu.addAction(self.new_project_action)
 
         self.open_project_action = QAction(self)
-        self.open_project_action.setShortcut('Ctrl+O')
+        self.open_project_action.setShortcut("Ctrl+O")
         self.open_project_action.triggered.connect(
             lambda _: self.open_project(),
         )
         betty_menu.addAction(self.open_project_action)
 
         self._demo_action = QAction(self)
         self._demo_action.triggered.connect(
@@ -70,19 +88,19 @@
         self.clear_caches_action = QAction(self)
         self.clear_caches_action.triggered.connect(
             lambda _: self.clear_caches(),
         )
         betty_menu.addAction(self.clear_caches_action)
 
         self.exit_action = QAction(self)
-        self.exit_action.setShortcut('Ctrl+Q')
+        self.exit_action.setShortcut("Ctrl+Q")
         self.exit_action.triggered.connect(QCoreApplication.quit)
         betty_menu.addAction(self.exit_action)
 
-        help_menu = menu_bar.addMenu('')
+        help_menu = menu_bar.addMenu("")
         assert help_menu is not None
         self.help_menu = help_menu
 
         self.report_bug_action = QAction(self)
         self.report_bug_action.triggered.connect(
             lambda _: self.report_bug(),
         )
@@ -104,61 +122,75 @@
         self.about_action.triggered.connect(
             lambda _: self._about_betty(),
         )
         help_menu.addAction(self.about_action)
 
     @property
     def window_title(self) -> Localizable:
-        return Str.plain('Betty')
+        return Str.plain("Betty")
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self.new_project_action.setText(self._app.localizer._('New project...'))
-        self.open_project_action.setText(self._app.localizer._('Open project...'))
-        self._demo_action.setText(self._app.localizer._('View demo site...'))
-        self.open_application_configuration_action.setText(self._app.localizer._('Settings...'))
-        self.clear_caches_action.setText(self._app.localizer._('Clear all caches'))
-        self.exit_action.setText(self._app.localizer._('Exit'))
-        self.help_menu.setTitle('&' + self._app.localizer._('Help'))
-        self.report_bug_action.setText(self._app.localizer._('Report a bug'))
-        self.request_feature_action.setText(self._app.localizer._('Request a new feature'))
-        self._docs_action.setText(self._app.localizer._('View documentation'))
-        self.about_action.setText(self._app.localizer._('About Betty'))
+        self.new_project_action.setText(self._app.localizer._("New project..."))
+        self.open_project_action.setText(self._app.localizer._("Open project..."))
+        self._demo_action.setText(self._app.localizer._("View demo site..."))
+        self.open_application_configuration_action.setText(
+            self._app.localizer._("Settings...")
+        )
+        self.clear_caches_action.setText(self._app.localizer._("Clear all caches"))
+        self.exit_action.setText(self._app.localizer._("Exit"))
+        self.help_menu.setTitle("&" + self._app.localizer._("Help"))
+        self.report_bug_action.setText(self._app.localizer._("Report a bug"))
+        self.request_feature_action.setText(
+            self._app.localizer._("Request a new feature")
+        )
+        self._docs_action.setText(self._app.localizer._("View documentation"))
+        self.about_action.setText(self._app.localizer._("About Betty"))
 
     def report_bug(self) -> None:
         with ExceptionCatcher(self):
-            body = f'''
+            body = f"""
 ## Summary
 
 ## Steps to reproduce
 
 ## Expected behavior
 
 ## System report
 ```
 {report()}
 ```
-'''.strip()
-            webbrowser.open_new_tab('https://github.com/bartfeenstra/betty/issues/new?' + urlencode({
-                'body': body,
-                'labels': 'bug',
-            }))
+""".strip()
+            webbrowser.open_new_tab(
+                "https://github.com/bartfeenstra/betty/issues/new?"
+                + urlencode(
+                    {
+                        "body": body,
+                        "labels": "bug",
+                    }
+                )
+            )
 
     def request_feature(self) -> None:
         with ExceptionCatcher(self):
-            body = '''
+            body = """
 ## Summary
 
 ## Expected behavior
 
-'''.strip()
-            webbrowser.open_new_tab('https://github.com/bartfeenstra/betty/issues/new?' + urlencode({
-                'body': body,
-                'labels': 'enhancement',
-            }))
+""".strip()
+            webbrowser.open_new_tab(
+                "https://github.com/bartfeenstra/betty/issues/new?"
+                + urlencode(
+                    {
+                        "body": body,
+                        "labels": "enhancement",
+                    }
+                )
+            )
 
     def _docs(self) -> None:
         with ExceptionCatcher(self):
             serve_window = ServeDocsWindow(self._app, parent=self)
             serve_window.show()
 
     def _about_betty(self) -> None:
@@ -168,33 +200,35 @@
 
     def open_project(self) -> None:
         with ExceptionCatcher(self):
             from betty.gui.project import ProjectWindow
 
             configuration_file_path_str, __ = QFileDialog.getOpenFileName(
                 self,
-                self._app.localizer._('Open your project from...'),
-                '',
+                self._app.localizer._("Open your project from..."),
+                "",
                 get_configuration_file_filter().localize(self._app.localizer),
             )
             if not configuration_file_path_str:
                 return
-            wait_to_thread(self._app.project.configuration.read(Path(configuration_file_path_str)))
+            wait_to_thread(
+                self._app.project.configuration.read(Path(configuration_file_path_str))
+            )
             project_window = ProjectWindow(self._app)
             project_window.show()
             self.close()
 
     def new_project(self) -> None:
         with ExceptionCatcher(self):
             from betty.gui.project import ProjectWindow
 
             configuration_file_path_str, __ = QFileDialog.getSaveFileName(
                 self,
-                self._app.localizer._('Save your new project to...'),
-                '',
+                self._app.localizer._("Save your new project to..."),
+                "",
                 get_configuration_file_filter().localize(self._app.localizer),
             )
             if not configuration_file_path_str:
                 return
             configuration = ProjectConfiguration()
             wait_to_thread(configuration.write(Path(configuration_file_path_str)))
             project_window = ProjectWindow(self._app)
@@ -282,24 +316,36 @@
 
         self.demo_button = _WelcomeAction(self)
         self.demo_button.released.connect(self._demo)
         central_layout.addWidget(self.demo_button)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._welcome.setText(self._app.localizer._('Welcome to Betty'))
-        self._welcome_caption.setText(self._app.localizer._('Betty helps you visualize and publish your family history by building interactive genealogy websites out of your <a href="{gramps_url}">Gramps</a> and <a href="{gedcom_url}">GEDCOM</a> family trees.').format(
-            gramps_url='https://gramps-project.org/',
-            gedcom_url='https://en.wikipedia.org/wiki/GEDCOM',
-        ))
-        self._project_instruction.setText(self._app.localizer._('Work on a new or existing site of your own'))
-        self.open_project_button.setText(self._app.localizer._('Open an existing project'))
-        self.new_project_button.setText(self._app.localizer._('Create a new project'))
-        self._demo_instruction.setText(self._app.localizer._('View a demonstration of what a Betty site looks like'))
-        self.demo_button.setText(self._app.localizer._('View a demo site'))
+        self._welcome.setText(self._app.localizer._("Welcome to Betty"))
+        self._welcome_caption.setText(
+            self._app.localizer._(
+                'Betty helps you visualize and publish your family history by building interactive genealogy websites out of your <a href="{gramps_url}">Gramps</a> and <a href="{gedcom_url}">GEDCOM</a> family trees.'
+            ).format(
+                gramps_url="https://gramps-project.org/",
+                gedcom_url="https://en.wikipedia.org/wiki/GEDCOM",
+            )
+        )
+        self._project_instruction.setText(
+            self._app.localizer._("Work on a new or existing site of your own")
+        )
+        self.open_project_button.setText(
+            self._app.localizer._("Open an existing project")
+        )
+        self.new_project_button.setText(self._app.localizer._("Create a new project"))
+        self._demo_instruction.setText(
+            self._app.localizer._(
+                "View a demonstration of what a Betty site looks like"
+            )
+        )
+        self.demo_button.setText(self._app.localizer._("View a demo site"))
 
 
 class _AboutBettyWindow(BettyMainWindow):
     window_width = 500
     window_height = 100
 
     def __init__(
@@ -311,27 +357,38 @@
         super().__init__(app, parent=parent)
         self._label = Text()
         self._label.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.setCentralWidget(self._label)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._label.setText(''.join(map(lambda x: '<p>%s</p>' % x, [
-            self._app.localizer._('Version: {version}').format(
-                version=wait_to_thread(about.version_label()),
-            ),
-            self._app.localizer._('Copyright 2019-{year} Bart Feenstra & contributors. Betty is made available to you under the <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GNU General Public License, Version 3</a> (GPLv3).').format(
-                year=datetime.now().year,
-            ),
-            self._app.localizer._('Follow Betty on <a href="https://twitter.com/Betty_Project">Twitter</a> and <a href="https://github.com/bartfeenstra/betty">Github</a>.'),
-        ])))
+        self._label.setText(
+            "".join(
+                map(
+                    lambda x: "<p>%s</p>" % x,
+                    [
+                        self._app.localizer._("Version: {version}").format(
+                            version=wait_to_thread(about.version_label()),
+                        ),
+                        self._app.localizer._(
+                            'Copyright 2019-{year} Bart Feenstra & contributors. Betty is made available to you under the <a href="https://www.gnu.org/licenses/gpl-3.0.en.html">GNU General Public License, Version 3</a> (GPLv3).'
+                        ).format(
+                            year=datetime.now().year,
+                        ),
+                        self._app.localizer._(
+                            'Follow Betty on <a href="https://twitter.com/Betty_Project">Twitter</a> and <a href="https://github.com/bartfeenstra/betty">Github</a>.'
+                        ),
+                    ],
+                )
+            )
+        )
 
     @property
     def window_title(self) -> Localizable:
-        return Str._('About Betty')
+        return Str._("About Betty")
 
 
 class ApplicationConfiguration(BettyMainWindow):
     window_width = 400
     window_height = 150
 
     def __init__(
@@ -342,14 +399,16 @@
     ):
         super().__init__(app, parent=parent)
 
         self._form = QFormLayout()
         form_widget = QWidget()
         form_widget.setLayout(self._form)
         self.setCentralWidget(form_widget)
-        self._locale_collector = TranslationsLocaleCollector(self._app, set(self._app.localizers.locales))
+        self._locale_collector = TranslationsLocaleCollector(
+            self._app, set(self._app.localizers.locales)
+        )
         for row in self._locale_collector.rows:
             self._form.addRow(*row)
 
     @property
     def window_title(self) -> Localizable:
-        return Str._('Configuration')
+        return Str._("Configuration")
```

### Comparing `betty-0.3.3/betty/gui/error.py` & `betty-0.3.4/betty/gui/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,93 +1,113 @@
 """
 Provide error handling for the Graphical User Interface.
 """
+
 from __future__ import annotations
 
 import pickle
 from asyncio import CancelledError
 from logging import getLogger
 from traceback import format_exception
 from types import TracebackType
 from typing import TypeVar, Generic, ParamSpec
 
 from PyQt6.QtCore import QMetaObject, Qt, Q_ARG, QObject
 from PyQt6.QtGui import QCloseEvent
-from PyQt6.QtWidgets import QWidget, QVBoxLayout, QHBoxLayout, QPushButton, QScrollArea, QFrame
+from PyQt6.QtWidgets import (
+    QWidget,
+    QVBoxLayout,
+    QHBoxLayout,
+    QPushButton,
+    QScrollArea,
+    QFrame,
+)
 
 from betty.app import App
 from betty.error import UserFacingError
 from betty.gui.text import Code, Text
 from betty.gui.window import BettyMainWindow
 from betty.locale import Str, Localizable
 
-T = TypeVar('T')
-P = ParamSpec('P')
+T = TypeVar("T")
+P = ParamSpec("P")
 
-BaseExceptionT = TypeVar('BaseExceptionT', bound=BaseException)
+BaseExceptionT = TypeVar("BaseExceptionT", bound=BaseException)
 
 
 class ExceptionCatcher(Generic[P, T]):
     """
     Catch any exception and show an error window instead.
     """
 
-    _SUPPRESS_EXCEPTION_TYPES = (
-        CancelledError,
-    )
+    _SUPPRESS_EXCEPTION_TYPES = (CancelledError,)
 
     def __init__(
         self,
         parent: QObject,
         *,
         close_parent: bool = False,
     ):
         self._parent = parent
         self._close_parent = close_parent
 
     def __enter__(self) -> None:
         pass
 
-    def __exit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> bool | None:
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         return self._catch(exc_type, exc_val)
 
     async def __aenter__(self) -> None:
         pass
 
-    async def __aexit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> bool | None:
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         return self._catch(exc_type, exc_val)
 
-    def _catch(self, exception_type: type[BaseExceptionT] | None, exception: BaseExceptionT | None) -> bool | None:
+    def _catch(
+        self,
+        exception_type: type[BaseExceptionT] | None,
+        exception: BaseExceptionT | None,
+    ) -> bool | None:
         from betty.gui import BettyApplication
 
         if exception_type is None or exception is None:
             return None
 
         if isinstance(exception, self._SUPPRESS_EXCEPTION_TYPES):
             return None
 
         if isinstance(exception, UserFacingError):
             QMetaObject.invokeMethod(
                 BettyApplication.instance(),
-                '_show_user_facing_error',
+                "_show_user_facing_error",
                 Qt.ConnectionType.QueuedConnection,
                 Q_ARG(type, exception_type),
                 Q_ARG(bytes, pickle.dumps(exception)),
                 Q_ARG(QObject, self._parent),
                 Q_ARG(bool, self._close_parent),
             )
         else:
             getLogger(__name__).exception(exception)
             QMetaObject.invokeMethod(
                 BettyApplication.instance(),
-                '_show_unexpected_exception',
+                "_show_unexpected_exception",
                 Qt.ConnectionType.QueuedConnection,
                 Q_ARG(type, exception_type),
                 Q_ARG(str, str(exception)),
-                Q_ARG(str, ''.join(format_exception(exception))),
+                Q_ARG(str, "".join(format_exception(exception))),
                 Q_ARG(QObject, self._parent),
                 Q_ARG(bool, self._close_parent),
             )
         return True
 
 
 class Error(BettyMainWindow):
@@ -101,15 +121,15 @@
         *,
         parent: QObject,
         close_parent: bool = False,
     ):
         super().__init__(app, parent=parent)
         self._message_localizable = message
         if close_parent and not isinstance(parent, QWidget):
-            raise ValueError('If `close_parent` is true, `parent` must be `QWidget`.')
+            raise ValueError("If `close_parent` is true, `parent` must be `QWidget`.")
         self._close_parent = close_parent
         self.setWindowModality(Qt.WindowModality.WindowModal)
 
         central_widget = QWidget()
         self._central_layout = QVBoxLayout()
         central_widget.setLayout(self._central_layout)
         self.setCentralWidget(central_widget)
@@ -122,30 +142,30 @@
 
         self._dismiss = QPushButton()
         self._dismiss.released.connect(self.close)
         self._controls.addWidget(self._dismiss)
 
     @property
     def window_title(self) -> Localizable:
-        return Str.plain('{error} - Betty', error=Str._('Error'))
+        return Str.plain("{error} - Betty", error=Str._("Error"))
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
         self._message.setText(self._message_localizable.localize(self._app.localizer))
-        self._dismiss.setText(self._app.localizer._('Close'))
+        self._dismiss.setText(self._app.localizer._("Close"))
 
     def closeEvent(self, a0: QCloseEvent | None) -> None:
         if self._close_parent:
             parent = self.parent()
             if isinstance(parent, QWidget):
                 parent.close()
         super().closeEvent(a0)
 
 
-ErrorT = TypeVar('ErrorT', bound=Error)
+ErrorT = TypeVar("ErrorT", bound=Error)
 
 
 class ExceptionError(Error):
     def __init__(
         self,
         app: App,
         message: Localizable,
@@ -154,15 +174,15 @@
         parent: QObject,
         close_parent: bool = False,
     ):
         super().__init__(app, message, parent=parent, close_parent=close_parent)
         self.error_type = error_type
 
 
-ExceptionErrorT = TypeVar('ExceptionErrorT', bound=ExceptionError)
+ExceptionErrorT = TypeVar("ExceptionErrorT", bound=ExceptionError)
 
 
 class _UnexpectedExceptionError(ExceptionError):
     def __init__(
         self,
         app: App,
         error_type: type[Exception],
@@ -172,23 +192,25 @@
         parent: QObject,
         close_parent: bool = False,
     ):
         super().__init__(
             app,
             Str._(
                 'An unexpected error occurred and Betty could not complete the task. Please <a href="{report_url}">report this problem</a> and include the following details, so the team behind Betty can address it.',
-                report_url='https://github.com/bartfeenstra/betty/issues',
+                report_url="https://github.com/bartfeenstra/betty/issues",
             ),
             error_type,
             parent=parent,
             close_parent=close_parent,
         )
 
         if error_message:
             self._exception_message = Code(error_message)
             self._central_layout.addWidget(self._exception_message)
 
         self._exception_details = QScrollArea()
         self._exception_details.setFrameShape(QFrame.Shape.NoFrame)
-        self._exception_details.setWidget(Code(error_traceback + error_traceback + error_traceback + error_traceback))
+        self._exception_details.setWidget(
+            Code(error_traceback + error_traceback + error_traceback + error_traceback)
+        )
         self._exception_details.setWidgetResizable(True)
         self._central_layout.addWidget(self._exception_details)
```

### Comparing `betty-0.3.3/betty/gui/locale.py` & `betty-0.3.4/betty/gui/locale.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide locale management for the Graphical User Interface.
 """
+
 from __future__ import annotations
 
 from typing import Any
 
 from PyQt6 import QtGui
 from PyQt6.QtWidgets import QComboBox, QLabel, QWidget
 
@@ -36,28 +37,33 @@
         super().__init__(app)
         self._allowed_locales = allowed_locales
 
         allowed_locale_names: list[tuple[str, str]] = []
         for allowed_locale in allowed_locales:
             locale_name = get_display_name(allowed_locale)
             if locale_name is not None:
-                allowed_locale_names.append((
-                    allowed_locale,
-                    locale_name,
-                ))
+                allowed_locale_names.append(
+                    (
+                        allowed_locale,
+                        locale_name,
+                    )
+                )
         allowed_locale_names = sorted(allowed_locale_names, key=lambda x: x[1])
 
         def _update_configuration_locale() -> None:
             self._app.configuration.locale = self._configuration_locale.currentData()
+
         self._configuration_locale = QComboBox()
         for i, (locale, locale_name) in enumerate(allowed_locale_names):
             self._configuration_locale.addItem(locale_name, locale)
             if locale == self._app.configuration.locale:
                 self._configuration_locale.setCurrentIndex(i)
-        self._configuration_locale.currentIndexChanged.connect(_update_configuration_locale)
+        self._configuration_locale.currentIndexChanged.connect(
+            _update_configuration_locale
+        )
         self._configuration_locale_label = QLabel()
         self._configuration_locale_caption = Caption()
 
         self._set_translatables()
         self._app.configuration.on_change(self._set_translatables)
 
     @property
@@ -71,28 +77,46 @@
             [self._configuration_locale_caption],
         ]
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
         localizer = self._app.localizer
         localizers = self._app.localizers
-        self._configuration_locale_label.setText(localizer._('Locale'))
+        self._configuration_locale_label.setText(localizer._("Locale"))
         locale = self.locale.currentData()
         if locale:
             translations_locale = negotiate_locale(
                 locale,
                 list(localizers.locales),
             )
             if translations_locale is None:
-                self._configuration_locale_caption.setText(localizer._('There are no translations for {locale_name}.').format(
-                    locale_name=get_display_name(locale, localizer.locale),
-                ))
+                self._configuration_locale_caption.setText(
+                    localizer._("There are no translations for {locale_name}.").format(
+                        locale_name=get_display_name(locale, localizer.locale),
+                    )
+                )
             else:
-                negotiated_locale_translations_coverage = wait_to_thread(localizers.coverage(translations_locale))
+                negotiated_locale_translations_coverage = wait_to_thread(
+                    localizers.coverage(translations_locale)
+                )
                 if negotiated_locale_translations_coverage[1] == 0:
                     negotiated_locale_translations_coverage_percentage = 0
                 else:
-                    negotiated_locale_translations_coverage_percentage = round(100 / (negotiated_locale_translations_coverage[1] / negotiated_locale_translations_coverage[0]))
-                self._configuration_locale_caption.setText(localizer._('The translations for {locale_name} are {coverage_percentage}%% complete.').format(
-                    locale_name=get_display_name(translations_locale, localizer.locale),
-                    coverage_percentage=round(negotiated_locale_translations_coverage_percentage)
-                ))
+                    negotiated_locale_translations_coverage_percentage = round(
+                        100
+                        / (
+                            negotiated_locale_translations_coverage[1]
+                            / negotiated_locale_translations_coverage[0]
+                        )
+                    )
+                self._configuration_locale_caption.setText(
+                    localizer._(
+                        "The translations for {locale_name} are {coverage_percentage}%% complete."
+                    ).format(
+                        locale_name=get_display_name(
+                            translations_locale, localizer.locale
+                        ),
+                        coverage_percentage=round(
+                            negotiated_locale_translations_coverage_percentage
+                        ),
+                    )
+                )
```

### Comparing `betty-0.3.3/betty/gui/logging.py` & `betty-0.3.4/betty/gui/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide logging for the Graphical User Interface.
 """
+
 import logging
 
 from PyQt6.QtCore import QObject, pyqtSignal, Qt
 from PyQt6.QtWidgets import QWidget, QVBoxLayout
 
 from betty.gui.text import Text
 
@@ -19,15 +20,15 @@
         logging.NOTSET,
     ]
 
     _formatter = logging.Formatter()
 
     def __init__(self, record: logging.LogRecord):
         super().__init__(self._formatter.format(record))
-        self.setProperty('level', self._normalize_level(record.levelno))
+        self.setProperty("level", self._normalize_level(record.levelno))
 
     def _normalize_level(self, record_level: int) -> int:
         for level in self._LEVELS:
             if record_level >= level:
                 return level
         return logging.NOTSET
```

### Comparing `betty-0.3.3/betty/gui/model.py` & `betty-0.3.4/betty/gui/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 """
 Provide entity management widgets for the Graphical User Interface.
 """
+
 from __future__ import annotations
 
 from typing import Callable, cast, Iterator
 
-from PyQt6.QtWidgets import QFormLayout, QLabel, QComboBox, QLineEdit, QWidget, QPushButton, QVBoxLayout, QHBoxLayout
+from PyQt6.QtWidgets import (
+    QFormLayout,
+    QLabel,
+    QComboBox,
+    QLineEdit,
+    QWidget,
+    QPushButton,
+    QVBoxLayout,
+    QHBoxLayout,
+)
 
 from betty.app import App
 from betty.gui.locale import LocalizedObject
 from betty.locale import Localizable
 from betty.model import UserFacingEntity, Entity
 from betty.project import EntityReference, EntityReferenceSequence
 
@@ -29,46 +39,68 @@
 
         self._layout = QFormLayout()
         self.setLayout(self._layout)
 
         if self._entity_reference.entity_type_is_constrained:
             self._entity_type_label = QLabel()
         else:
+
             def _update_entity_type() -> None:
                 self._entity_reference.entity_type = self._entity_type.currentData()
+
             self._entity_type = QComboBox()
             self._entity_type.currentIndexChanged.connect(_update_entity_type)
-            entity_types = enumerate(sorted(cast(Iterator[type['UserFacingEntity & Entity']], filter(
-                lambda entity_type: issubclass(entity_type, UserFacingEntity),
-                self._app.entity_types,
-            )), key=lambda entity_type: entity_type.entity_type_label().localize(self._app.localizer)))
+            entity_types = enumerate(
+                sorted(
+                    cast(
+                        Iterator[type["UserFacingEntity & Entity"]],
+                        filter(
+                            lambda entity_type: issubclass(
+                                entity_type, UserFacingEntity
+                            ),
+                            self._app.entity_types,
+                        ),
+                    ),
+                    key=lambda entity_type: entity_type.entity_type_label().localize(
+                        self._app.localizer
+                    ),
+                )
+            )
             for i, entity_type in entity_types:
-                self._entity_type.addItem(entity_type.entity_type_label().localize(self._app.localizer), entity_type)
+                self._entity_type.addItem(
+                    entity_type.entity_type_label().localize(self._app.localizer),
+                    entity_type,
+                )
                 if entity_type == self._entity_reference.entity_type:
                     self._entity_type.setCurrentIndex(i)
             self._entity_type_label = QLabel()
             self._layout.addRow(self._entity_type_label, self._entity_type)
 
         def _update_entity_id() -> None:
             self._entity_reference.entity_id = self._entity_id.text()
+
         self._entity_id = QLineEdit()
         self._entity_id.textChanged.connect(_update_entity_id)
         self._entity_id_label = QLabel()
         self._layout.addRow(self._entity_id_label, self._entity_id)
 
         self._set_translatables()
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
         if self._entity_reference.entity_type:
-            self._entity_id_label.setText(self._app.localizer._('{entity_type_label} ID').format(
-                entity_type_label=self._entity_reference.entity_type.entity_type_label().localize(self._app.localizer),
-            ))
+            self._entity_id_label.setText(
+                self._app.localizer._("{entity_type_label} ID").format(
+                    entity_type_label=self._entity_reference.entity_type.entity_type_label().localize(
+                        self._app.localizer
+                    ),
+                )
+            )
         else:
-            self._entity_id_label.setText(self._app.localizer._('Entity ID'))
+            self._entity_id_label.setText(self._app.localizer._("Entity ID"))
 
 
 class EntityReferenceSequenceCollector(LocalizedObject, QWidget):
     def __init__(
         self,
         app: App,
         entity_references: EntityReferenceSequence[UserFacingEntity & Entity],
@@ -77,28 +109,29 @@
     ):
         super().__init__(app)
         self._entity_references = entity_references
         self._label_text = label_text
         self._caption_text = caption_text
         self._entity_reference_collectors: list[EntityReferenceCollector] = [
             EntityReferenceCollector(self._app, entity_reference)
-            for entity_reference
-            in entity_references
+            for entity_reference in entity_references
         ]
 
         self._layout = QVBoxLayout()
         self.setLayout(self._layout)
 
         if label_text:
             self._label = QLabel()
             self._layout.addWidget(self._label)
 
         self._entity_reference_collectors_widget = QWidget()
         self._entity_reference_collectors_layout = QVBoxLayout()
-        self._entity_reference_collectors_widget.setLayout(self._entity_reference_collectors_layout)
+        self._entity_reference_collectors_widget.setLayout(
+            self._entity_reference_collectors_layout
+        )
         self._layout.addWidget(self._entity_reference_collectors_widget)
 
         self._entity_reference_collection_widgets: list[QWidget] = []
         self._entity_reference_remove_buttons: list[QPushButton] = []
 
         if caption_text:
             self._caption = QLabel()
@@ -109,24 +142,28 @@
         self._layout.addWidget(self._add_entity_reference_button)
 
         self._build_entity_references_collection()
 
         self._set_translatables()
 
     def _add_entity_reference(self) -> None:
-        entity_reference = EntityReference['UserFacingEntity & Entity']()
+        entity_reference = EntityReference["UserFacingEntity & Entity"]()
         self._entity_references.append(entity_reference)
-        self._build_entity_reference_collection(len(self._entity_references) - 1, entity_reference)
+        self._build_entity_reference_collection(
+            len(self._entity_references) - 1, entity_reference
+        )
         self._set_translatables()
 
     def _remove_entity_reference(self, i: int) -> None:
         del self._entity_references[i]
         del self._entity_reference_collectors[i]
         del self._entity_reference_remove_buttons[i]
-        self._entity_reference_collectors_layout.removeWidget(self._entity_reference_collection_widgets[i])
+        self._entity_reference_collectors_layout.removeWidget(
+            self._entity_reference_collection_widgets[i]
+        )
         del self._entity_reference_collection_widgets[i]
 
     def _build_entity_references_collection(self) -> None:
         for i, entity_reference in enumerate(self._entity_references):
             self._build_entity_reference_collection(i, entity_reference)
 
     def _build_entity_reference_collection(
@@ -136,25 +173,31 @@
     ) -> None:
         widget = QWidget()
         layout = QHBoxLayout()
         widget.setLayout(layout)
         self._entity_reference_collection_widgets.insert(i, widget)
         self._entity_reference_collectors_layout.insertWidget(i, widget)
 
-        entity_reference_collector = EntityReferenceCollector(self._app, entity_reference)
+        entity_reference_collector = EntityReferenceCollector(
+            self._app, entity_reference
+        )
         self._entity_reference_collectors.append(entity_reference_collector)
         layout.addWidget(entity_reference_collector)
 
         entity_reference_remove_button = QPushButton()
         self._entity_reference_remove_buttons.insert(i, entity_reference_remove_button)
-        entity_reference_remove_button.released.connect(lambda: self._remove_entity_reference(i))
+        entity_reference_remove_button.released.connect(
+            lambda: self._remove_entity_reference(i)
+        )
         layout.addWidget(entity_reference_remove_button)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
         if self._label_text:
             self._label.setText(self._label_text.localize(self._app.localizer))
         if self._caption_text:
             self._caption.setText(self._caption_text.localize(self._app.localizer))
-        self._add_entity_reference_button.setText(self._app.localizer._('Add an entity'))
+        self._add_entity_reference_button.setText(
+            self._app.localizer._("Add an entity")
+        )
         for entity_reference_remove_button in self._entity_reference_remove_buttons:
-            entity_reference_remove_button.setText(self._app.localizer._('Remove'))
+            entity_reference_remove_button.setText(self._app.localizer._("Remove"))
```

### Comparing `betty-0.3.3/betty/gui/project.py` & `betty-0.3.4/betty/gui/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,56 @@
 """
 Provide project administration for the Graphical User Interface.
 """
+
 from __future__ import annotations
 
 import asyncio
 import copy
 import re
 from asyncio import Task, CancelledError
 from contextlib import suppress
 from logging import getLogger
 from pathlib import Path
 from urllib.parse import urlparse
 
 from PyQt6.QtCore import Qt, QThread, QObject
 from PyQt6.QtGui import QAction, QCloseEvent
-from PyQt6.QtWidgets import QFileDialog, QPushButton, QWidget, QVBoxLayout, QHBoxLayout, QMenu, QStackedLayout, \
-    QGridLayout, QCheckBox, QFormLayout, QLabel, QLineEdit, QButtonGroup, QRadioButton, QFrame, QScrollArea, QSizePolicy
+from PyQt6.QtWidgets import (
+    QFileDialog,
+    QPushButton,
+    QWidget,
+    QVBoxLayout,
+    QHBoxLayout,
+    QMenu,
+    QStackedLayout,
+    QGridLayout,
+    QCheckBox,
+    QFormLayout,
+    QLabel,
+    QLineEdit,
+    QButtonGroup,
+    QRadioButton,
+    QFrame,
+    QScrollArea,
+    QSizePolicy,
+)
 from babel import Locale
 from babel.localedata import locale_identifiers
 
 from betty import load, generate
 from betty.app import App
 from betty.app.extension import UserFacingExtension
 from betty.asyncio import wait_to_thread
-from betty.gui import get_configuration_file_filter, GuiBuilder, mark_invalid, mark_valid
+from betty.gui import (
+    get_configuration_file_filter,
+    GuiBuilder,
+    mark_invalid,
+    mark_valid,
+)
 from betty.gui.app import BettyPrimaryWindow
 from betty.gui.error import ExceptionCatcher
 from betty.gui.locale import LocalizedObject
 from betty.gui.locale import TranslationsLocaleCollector
 from betty.gui.logging import LogRecordViewerHandler, LogRecordViewer
 from betty.gui.serve import ServeProjectWindow
 from betty.gui.text import Text, Caption
@@ -38,17 +61,19 @@
 from betty.serde.load import AssertionFailed
 
 
 class _PaneButton(QPushButton):
     def __init__(self, pane_name: str, project_window: ProjectWindow):
         super().__init__()
         self.setFlat(True)
-        self.setProperty('pane-selector', 'true')
+        self.setProperty("pane-selector", "true")
         self.setCursor(Qt.CursorShape.PointingHandCursor)
-        self.setSizePolicy(QSizePolicy.Policy.MinimumExpanding, QSizePolicy.Policy.Fixed)
+        self.setSizePolicy(
+            QSizePolicy.Policy.MinimumExpanding, QSizePolicy.Policy.Fixed
+        )
         self._project_window = project_window
         self.released.connect(lambda: self._project_window._navigate_to_pane(pane_name))
 
 
 class _GenerateHtmlListForm(LocalizedObject, QWidget):
     def __init__(self, app: App):
         super().__init__(app)
@@ -58,48 +83,60 @@
         self._form.addRow(self._form_label)
         self._checkboxes_form = QFormLayout()
         self._form.addRow(self._checkboxes_form)
         self._checkboxes: dict[type[UserFacingEntity & Entity], QCheckBox] = {}
         self._update()
 
     def _update(self) -> None:
-        entity_types = list(sorted(
-            [
-                entity_type
-                for entity_type
-                in self._app.entity_types
-                if issubclass(entity_type, UserFacingEntity)
-            ],
-            key=lambda x: x.entity_type_label_plural().localize(self._app.localizer),
-        ))
+        entity_types = list(
+            sorted(
+                [
+                    entity_type
+                    for entity_type in self._app.entity_types
+                    if issubclass(entity_type, UserFacingEntity)
+                ],
+                key=lambda x: x.entity_type_label_plural().localize(
+                    self._app.localizer
+                ),
+            )
+        )
         for entity_type in self._checkboxes.keys():
             if entity_type not in entity_types:
                 self._form.removeWidget(self._checkboxes[entity_type])
                 del self._checkboxes[entity_type]
         for row_i, entity_type in enumerate(entity_types):
             self._update_for_entity_type(entity_type, row_i)
 
-    def _update_for_entity_type(self, entity_type: type[UserFacingEntity & Entity], row_i: int) -> None:
+    def _update_for_entity_type(
+        self, entity_type: type[UserFacingEntity & Entity], row_i: int
+    ) -> None:
         if entity_type in self._checkboxes:
             self._checkboxes_form.insertRow(row_i, self._checkboxes[entity_type])
             return
 
         def _update(generate_html_list: bool) -> None:
-            self._app.project.configuration.entity_types[entity_type].generate_html_list = generate_html_list
+            self._app.project.configuration.entity_types[
+                entity_type
+            ].generate_html_list = generate_html_list
+
         self._checkboxes[entity_type] = QCheckBox()
-        self._checkboxes[entity_type].setChecked(self._app.project.configuration.entity_types[entity_type].generate_html_list)
+        self._checkboxes[entity_type].setChecked(
+            self._app.project.configuration.entity_types[entity_type].generate_html_list
+        )
         self._checkboxes[entity_type].toggled.connect(_update)
         self._update_for_entity_type(entity_type, row_i)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._form_label.setText(self._app.localizer._('Generate entity listing pages'))
+        self._form_label.setText(self._app.localizer._("Generate entity listing pages"))
         for entity_type in self._app.entity_types:
             if issubclass(entity_type, UserFacingEntity):
-                self._checkboxes[entity_type].setText(entity_type.entity_type_label_plural().localize(self._app.localizer))
+                self._checkboxes[entity_type].setText(
+                    entity_type.entity_type_label_plural().localize(self._app.localizer)
+                )
 
 
 class _GeneralPane(LocalizedObject, QWidget):
     def __init__(self, app: App):
         super().__init__(app)
 
         self._form = QFormLayout()
@@ -113,168 +150,218 @@
         self._build_clean_urls()
         self._generate_html_list_form = _GenerateHtmlListForm(app)
         self._form.addRow(self._generate_html_list_form)
 
     def _build_name(self) -> None:
         def _update_configuration_name(name: str) -> None:
             self._app.project.configuration.name = name
+
         self._configuration_name = QLineEdit()
         self._configuration_name.setText(self._app.project.configuration.name)
         self._configuration_name.textChanged.connect(_update_configuration_name)
         self._configuration_name_label = QLabel()
         self._form.addRow(self._configuration_name_label, self._configuration_name)
         self._configuration_name_caption = Caption()
         self._form.addRow(self._configuration_name_caption)
 
     def _build_title(self) -> None:
         def _update_configuration_title(title: str) -> None:
             self._app.project.configuration.title = title
+
         self._configuration_title = QLineEdit()
         self._configuration_title.setText(self._app.project.configuration.title)
         self._configuration_title.textChanged.connect(_update_configuration_title)
         self._configuration_title_label = QLabel()
         self._form.addRow(self._configuration_title_label, self._configuration_title)
 
     def _build_author(self) -> None:
         def _update_configuration_author(author: str) -> None:
             self._app.project.configuration.author = author
+
         self._configuration_author = QLineEdit()
         self._configuration_author.setText(str(self._app.project.configuration.author))
         self._configuration_author.textChanged.connect(_update_configuration_author)
         self._configuration_author_label = QLabel()
         self._form.addRow(self._configuration_author_label, self._configuration_author)
 
     def _build_url(self) -> None:
         def _update_configuration_url(url: str) -> None:
             url_parts = urlparse(url)
-            base_url = '%s://%s' % (url_parts.scheme, url_parts.netloc)
+            base_url = "%s://%s" % (url_parts.scheme, url_parts.netloc)
             root_path = url_parts.path
             configuration = copy.copy(self._app.project.configuration)
             try:
                 configuration.base_url = base_url
                 configuration.root_path = root_path
             except AssertionFailed as e:
                 mark_invalid(self._configuration_url, str(e))
                 return
             self._app.project.configuration.base_url = base_url
             self._app.project.configuration.root_path = root_path
             mark_valid(self._configuration_url)
+
         self._configuration_url = QLineEdit()
-        self._configuration_url.setText(self._app.project.configuration.base_url + self._app.project.configuration.root_path)
+        self._configuration_url.setText(
+            self._app.project.configuration.base_url
+            + self._app.project.configuration.root_path
+        )
         self._configuration_url.textChanged.connect(_update_configuration_url)
         self._configuration_url_label = QLabel()
         self._form.addRow(self._configuration_url_label, self._configuration_url)
 
     def _build_lifetime_threshold(self) -> None:
-        def _update_configuration_lifetime_threshold(lifetime_threshold_value: str) -> None:
-            if re.fullmatch(r'^\d+$', lifetime_threshold_value) is None:
-                mark_invalid(self._configuration_url, self._app.localizer._('The lifetime threshold must consist of digits only.'))
+        def _update_configuration_lifetime_threshold(
+            lifetime_threshold_value: str,
+        ) -> None:
+            if re.fullmatch(r"^\d+$", lifetime_threshold_value) is None:
+                mark_invalid(
+                    self._configuration_url,
+                    self._app.localizer._(
+                        "The lifetime threshold must consist of digits only."
+                    ),
+                )
                 return
             lifetime_threshold = int(lifetime_threshold_value)
             try:
                 self._app.project.configuration.lifetime_threshold = lifetime_threshold
                 mark_valid(self._configuration_lifetime_threshold)
             except AssertionFailed as e:
                 mark_invalid(self._configuration_lifetime_threshold, str(e))
+
         self._configuration_lifetime_threshold = QLineEdit()
         self._configuration_lifetime_threshold.setFixedWidth(32)
-        self._configuration_lifetime_threshold.setText(str(self._app.project.configuration.lifetime_threshold))
-        self._configuration_lifetime_threshold.textChanged.connect(_update_configuration_lifetime_threshold)
+        self._configuration_lifetime_threshold.setText(
+            str(self._app.project.configuration.lifetime_threshold)
+        )
+        self._configuration_lifetime_threshold.textChanged.connect(
+            _update_configuration_lifetime_threshold
+        )
         self._configuration_lifetime_threshold_label = QLabel()
-        self._form.addRow(self._configuration_lifetime_threshold_label, self._configuration_lifetime_threshold)
+        self._form.addRow(
+            self._configuration_lifetime_threshold_label,
+            self._configuration_lifetime_threshold,
+        )
         self._configuration_lifetime_threshold_caption = Caption()
         self._form.addRow(self._configuration_lifetime_threshold_caption)
 
     def _build_mode(self) -> None:
         def _update_configuration_debug(mode: bool) -> None:
             self._app.project.configuration.debug = mode
+
         self._development_debug = QCheckBox()
         self._development_debug.setChecked(self._app.project.configuration.debug)
         self._development_debug.toggled.connect(_update_configuration_debug)
         self._form.addRow(self._development_debug)
         self._development_debug_caption = Caption()
         self._form.addRow(self._development_debug_caption)
 
     def _build_clean_urls(self) -> None:
         def _update_configuration_clean_urls(clean_urls: bool) -> None:
             self._app.project.configuration.clean_urls = clean_urls
+
         self._clean_urls = QCheckBox()
         self._clean_urls.setChecked(self._app.project.configuration.clean_urls)
         self._clean_urls.toggled.connect(_update_configuration_clean_urls)
         self._form.addRow(self._clean_urls)
         self._clean_urls_caption = Caption()
         self._form.addRow(self._clean_urls_caption)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._configuration_name_label.setText(self._app.localizer._('Name'))
-        self._configuration_name_caption.setText(self._app.localizer._("The project's machine name."))
-        self._configuration_author_label.setText(self._app.localizer._('Author'))
-        self._configuration_url_label.setText(self._app.localizer._('URL'))
-        self._configuration_title_label.setText(self._app.localizer._('Title'))
-        self._configuration_lifetime_threshold_label.setText(self._app.localizer._('Lifetime threshold'))
-        self._configuration_lifetime_threshold_caption.setText(self._app.localizer._('The age at which people are presumed dead.'))
-        self._development_debug.setText(self._app.localizer._('Debugging mode'))
-        self._development_debug_caption.setText(self._app.localizer._('Output more detailed logs and disable optimizations that make debugging harder.'))
-        self._clean_urls.setText(self._app.localizer._('Clean URLs'))
-        self._clean_urls_caption.setText(self._app.localizer._('URLs look like <code>/path</code> instead of <code>/path/index.html</code>. This requires a web server that supports it.'))
+        self._configuration_name_label.setText(self._app.localizer._("Name"))
+        self._configuration_name_caption.setText(
+            self._app.localizer._("The project's machine name.")
+        )
+        self._configuration_author_label.setText(self._app.localizer._("Author"))
+        self._configuration_url_label.setText(self._app.localizer._("URL"))
+        self._configuration_title_label.setText(self._app.localizer._("Title"))
+        self._configuration_lifetime_threshold_label.setText(
+            self._app.localizer._("Lifetime threshold")
+        )
+        self._configuration_lifetime_threshold_caption.setText(
+            self._app.localizer._("The age at which people are presumed dead.")
+        )
+        self._development_debug.setText(self._app.localizer._("Debugging mode"))
+        self._development_debug_caption.setText(
+            self._app.localizer._(
+                "Output more detailed logs and disable optimizations that make debugging harder."
+            )
+        )
+        self._clean_urls.setText(self._app.localizer._("Clean URLs"))
+        self._clean_urls_caption.setText(
+            self._app.localizer._(
+                "URLs look like <code>/path</code> instead of <code>/path/index.html</code>. This requires a web server that supports it."
+            )
+        )
 
 
 class _LocalesConfigurationWidget(LocalizedObject, QWidget):
     def __init__(self, app: App):
         super().__init__(app)
 
         self._layout = QGridLayout()
         self.setLayout(self._layout)
         self._remove_buttons: dict[str, QPushButton | None] = {}
         self._default_buttons: dict[str, QRadioButton] = {}
         self._default_locale_button_group = QButtonGroup()
 
-        self._layout.addWidget(Text('Default locale'))
+        self._layout.addWidget(Text("Default locale"))
 
         locales_data: list[tuple[str, str]] = []
         for locale in self._app.project.configuration.locales:
             locale_name = get_display_name(locale)
             if locale_name is None:
                 continue
             locales_data.append((locale, locale_name))
-        for locale_index, (locale, locale_name) in enumerate(sorted(
+        for locale_index, (locale, _locale_name) in enumerate(
+            sorted(
                 locales_data,
                 key=lambda locale_data: locale_data[1],
-        )):
+            )
+        ):
             self._build_locale_configuration(locale, locale_index + 1)
 
     def _build_locale_configuration(self, locale: str, row_index: int) -> None:
         self._default_buttons[locale] = QRadioButton()
-        self._default_buttons[locale].setChecked(locale == self._app.project.configuration.locales.default.locale)
+        self._default_buttons[locale].setChecked(
+            locale == self._app.project.configuration.locales.default.locale
+        )
 
         def _update_locales_configuration_default() -> None:
             self._app.project.configuration.locales.default = locale  # type: ignore[assignment]
-        self._default_buttons[locale].clicked.connect(_update_locales_configuration_default)
+
+        self._default_buttons[locale].clicked.connect(
+            _update_locales_configuration_default
+        )
         self._default_locale_button_group.addButton(self._default_buttons[locale])
         self._layout.addWidget(self._default_buttons[locale], row_index, 0)
 
         # Allow this locale configuration to be removed only if there are others, and if it is not default one.
-        if len(self._app.project.configuration.locales) > 1 and locale != self._app.project.configuration.locales.default.locale:
+        if (
+            len(self._app.project.configuration.locales) > 1
+            and locale != self._app.project.configuration.locales.default.locale
+        ):
+
             def _remove_locale() -> None:
                 del self._app.project.configuration.locales[locale]
+
             remove_button = QPushButton()
             remove_button.released.connect(_remove_locale)
             self._layout.addWidget(remove_button, row_index, 1)
             self._remove_buttons[locale] = remove_button
         else:
             self._remove_buttons[locale] = None
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
         for locale, button in self._default_buttons.items():
             button.setText(get_display_name(locale, self._app.localizer.locale))
         for button in self._remove_buttons.values():
             if button is not None:
-                button.setText(self._app.localizer._('Remove'))
+                button.setText(self._app.localizer._("Remove"))
 
 
 class _LocalizationPane(LocalizedObject, QWidget):
     def __init__(self, app: App):
         super().__init__(app)
 
         self._layout = QVBoxLayout()
@@ -284,28 +371,30 @@
         self._add_locale_button.released.connect(self._add_locale)
         self._layout.addWidget(self._add_locale_button, 1)
 
         self._layout.addStretch()
 
         self._locales_configuration_widget: _LocalesConfigurationWidget
         self._build_locales_configuration()
-        self._app.project.configuration.locales.on_change(self._build_locales_configuration)
+        self._app.project.configuration.locales.on_change(
+            self._build_locales_configuration
+        )
 
     def _build_locales_configuration(self) -> None:
         with suppress(AttributeError):
             self._layout.removeWidget(self._locales_configuration_widget)
             self._locales_configuration_widget.close()
             self._locales_configuration_widget.setParent(None)
             del self._locales_configuration_widget
         self._locales_configuration_widget = _LocalesConfigurationWidget(self._app)
         self._layout.insertWidget(0, self._locales_configuration_widget)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._add_locale_button.setText(self._app.localizer._('Add a locale'))
+        self._add_locale_button.setText(self._app.localizer._("Add a locale"))
 
     def _add_locale(self) -> None:
         window = _AddLocaleWindow(self._app, parent=self)
         window.show()
 
 
 class _AddLocaleWindow(BettyMainWindow):
@@ -325,60 +414,63 @@
         self._widget.setLayout(self._layout)
         self.setCentralWidget(self._widget)
 
         self._locale_collector = TranslationsLocaleCollector(
             self._app,
             {
                 to_locale(Locale.parse(babel_identifier))
-                for babel_identifier
-                in locale_identifiers()
+                for babel_identifier in locale_identifiers()
             },
         )
         for row in self._locale_collector.rows:
             self._layout.addRow(*row)
 
         self._alias = QLineEdit()
         self._alias_label = QLabel()
         self._layout.addRow(self._alias_label, self._alias)
         self._alias_caption = Caption()
         self._layout.addRow(self._alias_caption)
 
         buttons_layout = QHBoxLayout()
         self._layout.addRow(buttons_layout)
 
-        self._save_and_close = QPushButton(self._app.localizer._('Save and close'))
+        self._save_and_close = QPushButton(self._app.localizer._("Save and close"))
         self._save_and_close.released.connect(self._save_and_close_locale)
         buttons_layout.addWidget(self._save_and_close)
 
-        self._cancel = QPushButton(self._app.localizer._('Cancel'))
-        self._cancel.released.connect(
-            lambda _: self.close()
-        )
+        self._cancel = QPushButton(self._app.localizer._("Cancel"))
+        self._cancel.released.connect(lambda _: self.close())
         buttons_layout.addWidget(self._cancel)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._alias_label.setText(self._app.localizer._('Alias'))
-        self._alias_caption.setText(self._app.localizer._('An optional alias is used instead of the locale code to identify this locale, such as in URLs. If US English is the only English language variant on your site, you may want to alias its language code from <code>en-US</code> to <code>en</code>, for instance.'))
+        self._alias_label.setText(self._app.localizer._("Alias"))
+        self._alias_caption.setText(
+            self._app.localizer._(
+                "An optional alias is used instead of the locale code to identify this locale, such as in URLs. If US English is the only English language variant on your site, you may want to alias its language code from <code>en-US</code> to <code>en</code>, for instance."
+            )
+        )
 
     @property
     def window_title(self) -> Localizable:
-        return Str._('Add a locale')
+        return Str._("Add a locale")
 
     def _save_and_close_locale(self) -> None:
         with ExceptionCatcher(self):
             locale = self._locale_collector.locale.currentData()
             alias: str | None = self._alias.text().strip()
-            if alias == '':
+            if alias == "":
                 alias = None
             try:
-                self._app.project.configuration.locales.append(LocaleConfiguration(
-                    locale,
-                    alias=alias,
-                ))
+                self._app.project.configuration.locales.append(
+                    LocaleConfiguration(
+                        locale,
+                        alias=alias,
+                    )
+                )
             except AssertionFailed as e:
                 mark_invalid(self._alias, str(e))
                 return
             self.close()
 
 
 class _ExtensionPane(LocalizedObject, QWidget):
@@ -392,66 +484,82 @@
 
         enable_layout = QFormLayout()
         layout.addLayout(enable_layout)
 
         self._extension_description = Text()
         enable_layout.addRow(self._extension_description)
 
+        self._extension_gui: QWidget | None = None
+
         def _update_enabled(enabled: bool) -> None:
             with ExceptionCatcher(self):
                 if enabled:
                     self._app.project.configuration.extensions.enable(extension_type)
                     extension = self._app.extensions[extension_type]
                     if isinstance(extension, GuiBuilder):
-                        layout.addWidget(extension.gui_build())
+                        self._extension_gui = extension.gui_build()
+                        layout.addWidget(self._extension_gui)
                 else:
                     self._app.project.configuration.extensions.disable(extension_type)
-                    extension_gui_item = layout.itemAt(1)
-                    if extension_gui_item is not None:
-                        extension_gui_widget = extension_gui_item.widget()
-                        assert extension_gui_widget is not None
-                        layout.removeWidget(extension_gui_widget)
-                        extension_gui_widget.close()
-                        extension_gui_widget.setParent(None)
-                        del extension_gui_widget
+                    if self._extension_gui is not None:
+                        layout.removeWidget(self._extension_gui)
+                        self._extension_gui.close()
+                        self._extension_gui.setParent(None)
+                        self._extension_gui.deleteLater()
+                        self._extension_gui = None
 
         self._extension_enabled = QCheckBox()
         self._extension_enabled_caption = Caption()
         self._set_extension_status()
         self._extension_enabled.toggled.connect(_update_enabled)
         enable_layout.addRow(self._extension_enabled)
         enable_layout.addRow(self._extension_enabled_caption)
 
         if extension_type in self._app.extensions:
             extension = self._app.extensions[extension_type]
             if isinstance(extension, GuiBuilder):
-                layout.addWidget(extension.gui_build())
+                self._extension_gui = extension.gui_build()
+                layout.addWidget(self._extension_gui)
 
     def _set_extension_status(self) -> None:
         self._extension_enabled.setDisabled(False)
-        self._extension_enabled_caption.setText('')
+        self._extension_enabled_caption.setText("")
         if self._extension_type in self._app.extensions:
             self._extension_enabled.setChecked(True)
-            disable_requirement = self._app.extensions[self._extension_type].disable_requirement()
+            disable_requirement = self._app.extensions[
+                self._extension_type
+            ].disable_requirement()
             if not disable_requirement.is_met():
                 self._extension_enabled.setDisabled(True)
-                self._extension_enabled_caption.setText(str(disable_requirement.reduce()))
+                reduced_disable_requirement = disable_requirement.reduce()
+                if reduced_disable_requirement is not None:
+                    self._extension_enabled_caption.setText(
+                        reduced_disable_requirement.localize(self._app.localizer)
+                    )
         else:
             self._extension_enabled.setChecked(False)
             enable_requirement = self._extension_type.enable_requirement()
             if not enable_requirement.is_met():
                 self._extension_enabled.setDisabled(True)
-                self._extension_enabled_caption.setText(str(enable_requirement.reduce()))
+                reduced_enable_requirement = enable_requirement.reduce()
+                if reduced_enable_requirement is not None:
+                    self._extension_enabled_caption.setText(
+                        reduced_enable_requirement.localize(self._app.localizer)
+                    )
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._extension_description.setText(self._extension_type.description().localize(self._app.localizer))
-        self._extension_enabled.setText(self._app.localizer._('Enable {extension}').format(
-            extension=self._extension_type.label().localize(self._app.localizer),
-        ))
+        self._extension_description.setText(
+            self._extension_type.description().localize(self._app.localizer)
+        )
+        self._extension_enabled.setText(
+            self._app.localizer._("Enable {extension}").format(
+                extension=self._extension_type.label().localize(self._app.localizer),
+            )
+        )
 
 
 class ProjectWindow(BettyPrimaryWindow):
     def __init__(
         self,
         app: App,
     ):
@@ -463,15 +571,17 @@
         self.setCentralWidget(central_widget)
 
         self._pane_selectors_container_widget = QWidget()
         self._pane_selectors_container_widget.setFixedWidth(225)
 
         self._pane_selectors_container = QScrollArea()
         self._pane_selectors_container.setFrameShape(QFrame.Shape.NoFrame)
-        self._pane_selectors_container.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
+        self._pane_selectors_container.setHorizontalScrollBarPolicy(
+            Qt.ScrollBarPolicy.ScrollBarAlwaysOff
+        )
         self._pane_selectors_container.setWidget(self._pane_selectors_container_widget)
         self._pane_selectors_container.setWidgetResizable(True)
         self._pane_selectors_container.setFixedWidth(225)
         central_layout.addWidget(self._pane_selectors_container)
 
         self._pane_selectors_layout = QVBoxLayout()
         self._pane_selectors_layout.setContentsMargins(0, 0, 25, 0)
@@ -493,46 +603,55 @@
         self._panes_layout = QStackedLayout()
         central_layout.addLayout(self._panes_layout, 999999999)
 
         self._panes: dict[str, QWidget] = {}
         self._pane_containers: dict[str, QWidget] = {}
         self._pane_selectors: dict[str, QPushButton] = {}
 
-        self._add_pane('general', _GeneralPane(self._app))
-        self._builtin_pane_selectors_layout.addWidget(self._pane_selectors['general'])
-        self._navigate_to_pane('general')
-        self._add_pane('localization', _LocalizationPane(self._app))
-        self._builtin_pane_selectors_layout.addWidget(self._pane_selectors['localization'])
-        self._extension_types = [extension_type for extension_type in self._app.discover_extension_types() if issubclass(extension_type, UserFacingExtension)]
+        self._add_pane("general", _GeneralPane(self._app))
+        self._builtin_pane_selectors_layout.addWidget(self._pane_selectors["general"])
+        self._navigate_to_pane("general")
+        self._add_pane("localization", _LocalizationPane(self._app))
+        self._builtin_pane_selectors_layout.addWidget(
+            self._pane_selectors["localization"]
+        )
+        self._extension_types = [
+            extension_type
+            for extension_type in self._app.discover_extension_types()
+            if issubclass(extension_type, UserFacingExtension)
+        ]
         for extension_type in self._extension_types:
-            self._add_pane(f'extension-{extension_type.name()}', _ExtensionPane(self._app, extension_type))
+            self._add_pane(
+                f"extension-{extension_type.name()}",
+                _ExtensionPane(self._app, extension_type),
+            )
 
         menu_bar = self.menuBar()
         assert menu_bar is not None
 
         self.project_menu = QMenu()
         menu_bar.addMenu(self.project_menu)
         menu_bar.insertMenu(self.help_menu.menuAction(), self.project_menu)
 
         self.save_project_as_action = QAction(self)
-        self.save_project_as_action.setShortcut('Ctrl+Shift+S')
+        self.save_project_as_action.setShortcut("Ctrl+Shift+S")
         self.save_project_as_action.triggered.connect(
             lambda _: self._save_project_as(),
         )
         self.project_menu.addAction(self.save_project_as_action)
 
         self.generate_action = QAction(self)
-        self.generate_action.setShortcut('Ctrl+G')
+        self.generate_action.setShortcut("Ctrl+G")
         self.generate_action.triggered.connect(
             lambda _: self._generate(),
         )
         self.project_menu.addAction(self.generate_action)
 
         self.serve_action = QAction(self)
-        self.serve_action.setShortcut('Ctrl+Alt+S')
+        self.serve_action.setShortcut("Ctrl+Alt+S")
         self.serve_action.triggered.connect(
             lambda _: self._serve(),
         )
         self.project_menu.addAction(self.serve_action)
 
     def _add_pane(self, pane_name: str, pane: QWidget) -> None:
         pane_container = QScrollArea()
@@ -558,45 +677,56 @@
 
     def close(self) -> bool:
         self._app.project.configuration.autowrite = False
         return super().close()
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self.project_menu.setTitle('&' + self._app.localizer._('Project'))
-        self.save_project_as_action.setText(self._app.localizer._('Save this project as...'))
-        self.generate_action.setText(self._app.localizer._('Generate site'))
-        self.serve_action.setText(self._app.localizer._('Serve site'))
-        self._pane_selectors['general'].setText(self._app.localizer._('General'))
-        self._pane_selectors['localization'].setText(self._app.localizer._('Localization'))
+        self.project_menu.setTitle("&" + self._app.localizer._("Project"))
+        self.save_project_as_action.setText(
+            self._app.localizer._("Save this project as...")
+        )
+        self.generate_action.setText(self._app.localizer._("Generate site"))
+        self.serve_action.setText(self._app.localizer._("Serve site"))
+        self._pane_selectors["general"].setText(self._app.localizer._("General"))
+        self._pane_selectors["localization"].setText(
+            self._app.localizer._("Localization")
+        )
 
         # Sort extension pane selector buttons by their human-readable label.
         extension_pane_selector_labels = [
             (extension_type, extension_type.label().localize(self._app.localizer))
-            for extension_type
-            in self._extension_types
+            for extension_type in self._extension_types
         ]
-        for extension_type, extension_label in sorted(extension_pane_selector_labels, key=lambda x: x[1]):
-            extension_pane_name = f'extension-{extension_type.name()}'
-            self._pane_selectors[extension_pane_name].setText(extension_type.label().localize(self._app.localizer))
-            self._extension_pane_selectors_layout.addWidget(self._pane_selectors[extension_pane_name])
+        for extension_type, _extension_label in sorted(
+            extension_pane_selector_labels, key=lambda x: x[1]
+        ):
+            extension_pane_name = f"extension-{extension_type.name()}"
+            self._pane_selectors[extension_pane_name].setText(
+                extension_type.label().localize(self._app.localizer)
+            )
+            self._extension_pane_selectors_layout.addWidget(
+                self._pane_selectors[extension_pane_name]
+            )
 
     @property
     def window_title(self) -> Localizable:
         return Str.plain(self._app.project.configuration.title)
 
     def _save_project_as(self) -> None:
         with ExceptionCatcher(self):
             configuration_file_path_str, __ = QFileDialog.getSaveFileName(
                 self,
-                self._app.localizer._('Save your project to...'),
-                '',
+                self._app.localizer._("Save your project to..."),
+                "",
                 get_configuration_file_filter().localize(self._app.localizer),
             )
-            wait_to_thread(self._app.project.configuration.write(Path(configuration_file_path_str)))
+            wait_to_thread(
+                self._app.project.configuration.write(Path(configuration_file_path_str))
+            )
 
     def _generate(self) -> None:
         with ExceptionCatcher(self):
             generate_window = _GenerateWindow(self._app, parent=self)
             generate_window.show()
 
     def _serve(self) -> None:
@@ -674,15 +804,15 @@
 
         self._thread = _GenerateThread(self._app.project, self)
         self._thread.finished.connect(self._finish_generate)
         self._thread.start()
 
     @property
     def window_title(self) -> Localizable:
-        return Str._('Generating your site...')
+        return Str._("Generating your site...")
 
     def _serve(self) -> None:
         with ExceptionCatcher(self):
             serve_window = ServeProjectWindow(self._app, parent=self.parent())
             serve_window.show()
 
     def closeEvent(self, a0: QCloseEvent | None) -> None:
@@ -696,10 +826,10 @@
         self._finalize()
 
     def _finalize(self) -> None:
         getLogger(__name__).removeHandler(self._logging_handler)
 
     def _set_translatables(self) -> None:
         super()._set_translatables()
-        self._cancel_button.setText(self._app.localizer._('Cancel'))
-        self._cancel_button.setText(self._app.localizer._('Cancel'))
-        self._serve_button.setText(self._app.localizer._('View site'))
+        self._cancel_button.setText(self._app.localizer._("Cancel"))
+        self._cancel_button.setText(self._app.localizer._("Cancel"))
+        self._serve_button.setText(self._app.localizer._("View site"))
```

### Comparing `betty-0.3.3/betty/gui/serve.py` & `betty-0.3.4/betty/gui/serve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Integrate Betty's Graphical User Interface with the Serve API.
 """
+
 from __future__ import annotations
 
 import asyncio
 from typing import Any
 
 from PyQt6.QtCore import Qt, QThread, pyqtSignal, QObject
 from PyQt6.QtWidgets import QVBoxLayout, QWidget, QPushButton
@@ -20,15 +21,22 @@
 from betty.project import Project
 from betty.serve import Server, AppServer
 
 
 class _ServeThread(QThread):
     server_started = pyqtSignal()
 
-    def __init__(self, project: Project, server: Server, serve_window: _ServeWindow, *args: Any, **kwargs: Any):
+    def __init__(
+        self,
+        project: Project,
+        server: Server,
+        serve_window: _ServeWindow,
+        *args: Any,
+        **kwargs: Any,
+    ):
         super().__init__(*args, **kwargs)
         self._project = project
         self._server = server
         self._serve_window = serve_window
         self._app: App | None = None
 
     @property
@@ -64,25 +72,25 @@
         self.__thread: _ServeThread | None = None
 
         self._central_layout = QVBoxLayout()
         central_widget = QWidget()
         central_widget.setLayout(self._central_layout)
         self.setCentralWidget(central_widget)
 
-        self._loading_instruction = Text(self._app.localizer._('Loading...'))
+        self._loading_instruction = Text(self._app.localizer._("Loading..."))
         self._loading_instruction.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self._central_layout.addWidget(self._loading_instruction)
 
     def _server(self) -> Server:
         raise NotImplementedError(repr(self))
 
     @property
     def _thread(self) -> _ServeThread:
         if self.__thread is None:
-            raise RuntimeError('This window has not been shown yet.')
+            raise RuntimeError("This window has not been shown yet.")
         return self.__thread
 
     def _build_instruction(self) -> str:
         raise NotImplementedError(repr(self))
 
     def _server_started(self) -> None:
         # The server may have been stopped before this method was called.
@@ -91,19 +99,21 @@
 
         self._loading_instruction.close()
 
         instance_instruction = Text(self._build_instruction())
         instance_instruction.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self._central_layout.addWidget(instance_instruction)
 
-        general_instruction = Text(self._app.localizer._('Keep this window open to keep the site running.'))
+        general_instruction = Text(
+            self._app.localizer._("Keep this window open to keep the site running.")
+        )
         general_instruction.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self._central_layout.addWidget(general_instruction)
 
-        stop_server_button = QPushButton(self._app.localizer._('Stop the site'), self)
+        stop_server_button = QPushButton(self._app.localizer._("Stop the site"), self)
         stop_server_button.released.connect(
             self.close,
         )
         self._central_layout.addWidget(stop_server_button)
 
     def show(self) -> None:
         super().show()
@@ -129,44 +139,50 @@
 
 class ServeProjectWindow(_ServeWindow):
     def _server(self) -> Server:
         return AppServer.get(self._app)
 
     @property
     def window_title(self) -> Localizable:
-        return Str._('Serving your site...')
+        return Str._("Serving your site...")
 
     def _build_instruction(self) -> str:
-        return self._app.localizer._('You can now view your site at <a href="{url}">{url}</a>.').format(
+        return self._app.localizer._(
+            'You can now view your site at <a href="{url}">{url}</a>.'
+        ).format(
             url=self._thread.server.public_url,
         )
 
 
 class ServeDemoWindow(_ServeWindow):
     def _server(self) -> Server:
         return demo.DemoServer(app=self._app)
 
     def _build_instruction(self) -> str:
-        return self._app.localizer._('You can now view a Betty demonstration site at <a href="{url}">{url}</a>.').format(
+        return self._app.localizer._(
+            'You can now view a Betty demonstration site at <a href="{url}">{url}</a>.'
+        ).format(
             url=self._thread.server.public_url,
         )
 
     @property
     def window_title(self) -> Localizable:
-        return Str._('Serving the Betty demo...')
+        return Str._("Serving the Betty demo...")
 
 
 class ServeDocsWindow(_ServeWindow):
     def _server(self) -> Server:
         return documentation.DocumentationServer(
             self._app.binary_file_cache.path,
             localizer=self._app.localizer,
         )
 
     def _build_instruction(self) -> str:
-        return self._app.localizer._('You can now view the documentation at <a href="{url}">{url}</a>.').format(
+        return self._app.localizer._(
+            'You can now view the documentation at <a href="{url}">{url}</a>.'
+        ).format(
             url=self._thread.server.public_url,
         )
 
     @property
     def window_title(self) -> Localizable:
-        return Str._('Serving the Betty documentation...')
+        return Str._("Serving the Betty documentation...")
```

### Comparing `betty-0.3.3/betty/gui/text.py` & `betty-0.3.4/betty/gui/text.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,20 @@
 class Text(QLabel):
     def __init__(self, text: str | None = None):
         super().__init__()
         if text:
             self.setText(text)
         self.setTextFormat(Qt.TextFormat.RichText)
         self.setWordWrap(True)
-        self.setTextInteractionFlags(Qt.TextInteractionFlag.LinksAccessibleByKeyboard | Qt.TextInteractionFlag.LinksAccessibleByMouse | Qt.TextInteractionFlag.TextSelectableByKeyboard | Qt.TextInteractionFlag.TextSelectableByMouse)
+        self.setTextInteractionFlags(
+            Qt.TextInteractionFlag.LinksAccessibleByKeyboard
+            | Qt.TextInteractionFlag.LinksAccessibleByMouse
+            | Qt.TextInteractionFlag.TextSelectableByKeyboard
+            | Qt.TextInteractionFlag.TextSelectableByMouse
+        )
         self.setOpenExternalLinks(True)
 
 
 class Caption(Text):
     def __init__(self, text: str | None = None):
         super().__init__(text)
         font = QFont()
@@ -28,8 +33,8 @@
 class Code(Text):
     def __init__(self, text: str | None = None):
         super().__init__(text)
         font = QFont()
         self.setFont(font)
 
     def setText(self, a0: str | None) -> None:
-        super().setText(f'<pre>{a0}</pre>' if a0 else a0)
+        super().setText(f"<pre>{a0}</pre>" if a0 else a0)
```

### Comparing `betty-0.3.3/betty/gui/window.py` & `betty-0.3.4/betty/gui/window.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Manage windows.
 """
+
 from __future__ import annotations
 
 from os import path
 
 from PyQt6.QtCore import QObject
 from PyQt6.QtGui import QIcon
 from PyQt6.QtWidgets import QApplication, QMainWindow
@@ -22,20 +23,39 @@
         self,
         app: App,
         *,
         parent: QObject | None = None,
     ):
         super().__init__(app, parent)
         self.resize(self.window_width, self.window_height)
-        self.setWindowIcon(QIcon(path.join(path.dirname(__file__), 'assets', 'public', 'static', 'betty-512x512.png')))
+        self.setWindowIcon(
+            QIcon(
+                path.join(
+                    path.dirname(__file__),
+                    "assets",
+                    "public",
+                    "static",
+                    "betty-512x512.png",
+                )
+            )
+        )
         geometry = self.frameGeometry()
         screen = QApplication.primaryScreen()
         assert screen is not None
         geometry.moveCenter(screen.availableGeometry().center())
         self.move(geometry.topLeft())
 
     def _set_translatables(self) -> None:
-        self.setWindowTitle(f'{self.window_title.localize(self._app.localizer)} - Betty')
+        self.setWindowTitle(
+            f"{self.window_title.localize(self._app.localizer)} - Betty"
+        )
 
     @property
     def window_title(self) -> Localizable:
         raise NotImplementedError(repr(self))
+
+    def close(self) -> bool:
+        for child in self.children():
+            if isinstance(child, QMainWindow):
+                child.close()
+                child.deleteLater()
+        return super().close()
```

### Comparing `betty-0.3.3/betty/jinja2/__init__.py` & `betty-0.3.4/betty/jinja2/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,75 @@
 """
 Provide rendering utilities using `Jinja2 <https://jinja.palletsprojects.com>`_.
 """
+
 from __future__ import annotations
 
 import datetime
 from collections import defaultdict
+from collections.abc import MutableMapping, Iterator, Sequence
 from pathlib import Path
 from threading import Lock
-from typing import Callable, Any, cast, \
-    Mapping, TypeVar
+from typing import Callable, Any, cast, TypeVar
 
 import aiofiles
 from aiofiles import os as aiofiles_os
-from jinja2 import Environment as Jinja2Environment, select_autoescape, FileSystemLoader, pass_context, \
-    Template as Jinja2Template
-from jinja2.runtime import StrictUndefined, Context, DebugUndefined, new_context
+from jinja2 import (
+    Environment as Jinja2Environment,
+    select_autoescape,
+    FileSystemLoader,
+    pass_context,
+)
+from jinja2.runtime import StrictUndefined, Context, DebugUndefined
 
 from betty.app import App
+from betty.app.extension import Extension
 from betty.html import CssProvider, JsProvider
 from betty.jinja2.filter import FILTERS
 from betty.jinja2.test import TESTS
 from betty.job import Context as JobContext
-from betty.locale import Date, Localizer, \
-    DEFAULT_LOCALIZER
+from betty.locale import Date, Localizer, DEFAULT_LOCALIZER
 from betty.model import Entity, get_entity_type
 from betty.model.ancestry import Citation
 from betty.project import ProjectConfiguration
 from betty.render import Renderer
 from betty.serde.dump import Dumpable, DictDump, VoidableDump, Void, Dump
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 def context_app(context: Context) -> App:
     """
     Get the current app from the Jinja2 context.
     """
     return cast(Environment, context.environment).app
 
 
 def context_job_context(context: Context) -> JobContext | None:
     """
     Get the current job context from the Jinja2 context.
     """
-    job_context = context.resolve_or_missing('job_context')
+    job_context = context.resolve_or_missing("job_context")
     return job_context if isinstance(job_context, JobContext) else None
 
 
 def context_localizer(context: Context) -> Localizer:
     """
     Get the current localizer from the Jinja2 context.
     """
-    localizer = context.resolve_or_missing('localizer')
+    localizer = context.resolve_or_missing("localizer")
     if isinstance(localizer, Localizer):
         return localizer
-    raise RuntimeError('No `localizer` context variable exists in this Jinja2 template.')
+    raise RuntimeError(
+        "No `localizer` context variable exists in this Jinja2 template."
+    )
 
 
 class _Citer:
-    __slots__ = '_lock', '_cited'
+    __slots__ = "_lock", "_cited"
 
     def __init__(self):
         self._lock = Lock()
         self._cited: list[Citation] = []
 
     def __iter__(self) -> enumerate[Citation]:
         return enumerate(self._cited, 1)
@@ -80,51 +87,52 @@
 class _Breadcrumb(Dumpable):
     def __init__(self, label: str, url: str):
         self._label = label
         self._url = url
 
     def dump(self) -> DictDump[Dump]:
         return {
-            '@type': 'ListItem',
-            'name': self._label,
-            'item': self._url,
+            "@type": "ListItem",
+            "name": self._label,
+            "item": self._url,
         }
 
 
 class _Breadcrumbs(Dumpable):
     def __init__(self):
         self._breadcrumbs: list[_Breadcrumb] = []
 
     def append(self, label: str, url: str) -> None:
         self._breadcrumbs.append(_Breadcrumb(label, url))
 
     def dump(self) -> VoidableDump:
         if not self._breadcrumbs:
             return Void
         return {
-            '@context': 'https://schema.org',
-            '@type': 'BreadcrumbList',
-            'itemListElement': [
+            "@context": "https://schema.org",
+            "@type": "BreadcrumbList",
+            "itemListElement": [
                 {
-                    'position': position,
+                    "position": position,
                     **breadcrumb.dump(),
                 }
-                for position, breadcrumb
-                in enumerate(self._breadcrumbs, 1)
+                for position, breadcrumb in enumerate(self._breadcrumbs, 1)
             ],
         }
 
 
 class EntityContexts:
     def __init__(self, *entities: Entity) -> None:
         self._contexts: dict[type[Entity], Entity | None] = defaultdict(lambda: None)
         for entity in entities:
             self._contexts[entity.type] = entity
 
-    def __getitem__(self, entity_type_or_type_name: type[Entity] | str) -> Entity | None:
+    def __getitem__(
+        self, entity_type_or_type_name: type[Entity] | str
+    ) -> Entity | None:
         if isinstance(entity_type_or_type_name, str):
             entity_type = get_entity_type(entity_type_or_type_name)
         else:
             entity_type = entity_type_or_type_name
         return self._contexts[entity_type]
 
     def __call__(self, *entities: Entity) -> EntityContexts:
@@ -143,161 +151,196 @@
     def filters(self) -> dict[str, Callable[..., Any]]:
         return {}
 
     @property
     def tests(self) -> dict[str, Callable[..., bool]]:
         return {}
 
-
-class Template(Jinja2Template):
-    environment: Environment
-
-    def new_context(
-        self,
-        vars: dict[str, Any] | None = None,
-        shared: bool = False,
-        locals: Mapping[str, Any] | None = None,
-    ) -> Context:
-        return new_context(
-            self.environment,
-            self.name,
-            self.blocks,
-            vars,
-            shared,
-            {
-                'citer': _Citer(),
-                'breadcrumbs': _Breadcrumbs(),
-                **self.globals,
-            },
-            locals,
-        )
+    def new_context_vars(self) -> dict[str, Any]:
+        return {}
 
 
 class Environment(Jinja2Environment):
-    template_class = Template
     globals: dict[str, Any]
     filters: dict[str, Callable[..., Any]]
     tests: dict[str, Callable[..., bool]]
 
     def __init__(self, app: App):
-        template_directory_paths = [str(path / 'templates') for path, _ in app.assets.paths]
+        template_directory_paths = [
+            str(path / "templates") for path, _ in app.assets.paths
+        ]
         super().__init__(
             loader=FileSystemLoader(template_directory_paths),
             auto_reload=app.project.configuration.debug,
             enable_async=True,
-            undefined=DebugUndefined if app.project.configuration.debug else StrictUndefined,
-            autoescape=select_autoescape(['html.j2']),
+            undefined=(
+                DebugUndefined if app.project.configuration.debug else StrictUndefined
+            ),
+            autoescape=select_autoescape(["html.j2"]),
             trim_blocks=True,
             lstrip_blocks=True,
             extensions=[
-                'jinja2.ext.do',
-                'jinja2.ext.i18n',
+                "jinja2.ext.do",
+                "jinja2.ext.i18n",
             ],
         )
 
+        self._context_class: type[Context] | None = None
         self.app = app
 
         if app.project.configuration.debug:
-            self.add_extension('jinja2.ext.debug')
+            self.add_extension("jinja2.ext.debug")
 
         self._init_i18n()
         self._init_globals()
         self.filters.update(FILTERS)
         self.tests.update(TESTS)
         self._init_extensions()
 
     def _init_i18n(self) -> None:
         self.install_gettext_callables(  # type: ignore[attr-defined]
             gettext=self._gettext,
             ngettext=self._ngettext,
             pgettext=self._pgettext,
             npgettext=self._npgettext,
         )
-        self.policies['ext.i18n.trimmed'] = True
+        self.policies["ext.i18n.trimmed"] = True
+
+    @property
+    def context_class(self) -> type[Context]:  # type: ignore[override]
+        if self._context_class is None:
+            jinja2_providers: Sequence[Jinja2Provider & Extension] = [
+                extension
+                for extension in self.app.extensions.flatten()
+                if isinstance(extension, Jinja2Provider)
+            ]
+
+            class _Context(Context):
+                def __init__(
+                    self,
+                    environment: Environment,
+                    parent: dict[str, Any],
+                    name: str | None,
+                    blocks: dict[str, Callable[[Context], Iterator[str]]],
+                    globals: MutableMapping[str, Any] | None = None,
+                ):
+                    if "citer" not in parent:
+                        parent["citer"] = _Citer()
+                    if "breadcrumbs" not in parent:
+                        parent["breadcrumbs"] = _Breadcrumbs()
+                    for jinja2_provider in jinja2_providers:
+                        for key, value in jinja2_provider.new_context_vars().items():
+                            if key not in parent:
+                                parent[key] = value
+                    super().__init__(
+                        environment,
+                        parent,
+                        name,
+                        blocks,
+                        globals,
+                    )
+
+            self._context_class = _Context
+
+        return self._context_class
 
     @pass_context
     def _gettext(self, context: Context, message: str) -> str:
         return context_localizer(context).gettext(message)
 
     @pass_context
-    def _ngettext(self, context: Context, message_singular: str, message_plural: str, n: int) -> str:
+    def _ngettext(
+        self, context: Context, message_singular: str, message_plural: str, n: int
+    ) -> str:
         return context_localizer(context).ngettext(message_singular, message_plural, n)
 
     @pass_context
     def _pgettext(self, context: Context, gettext_context: str, message: str) -> str:
         return context_localizer(context).pgettext(gettext_context, message)
 
     @pass_context
-    def _npgettext(self, context: Context, gettext_context: str, message_singular: str, message_plural: str, n: int) -> str:
-        return context_localizer(context).npgettext(gettext_context, message_singular, message_plural, n)
+    def _npgettext(
+        self,
+        context: Context,
+        gettext_context: str,
+        message_singular: str,
+        message_plural: str,
+        n: int,
+    ) -> str:
+        return context_localizer(context).npgettext(
+            gettext_context, message_singular, message_plural, n
+        )
 
     def _init_globals(self) -> None:
-        self.globals['app'] = self.app
+        self.globals["app"] = self.app
         today = datetime.date.today()
-        self.globals['today'] = Date(today.year, today.month, today.day)
+        self.globals["today"] = Date(today.year, today.month, today.day)
         # Ideally we would use the Dispatcher for this. However, it is asynchronous only.
-        self.globals['public_css_paths'] = [
+        self.globals["public_css_paths"] = [
             path
             for extension in self.app.extensions.flatten()
             if isinstance(extension, CssProvider)
             for path in extension.public_css_paths
         ]
-        self.globals['public_js_paths'] = [
+        self.globals["public_js_paths"] = [
             path
             for extension in self.app.extensions.flatten()
             if isinstance(extension, JsProvider)
             for path in extension.public_js_paths
         ]
-        self.globals['entity_contexts'] = EntityContexts()
-        self.globals['localizer'] = DEFAULT_LOCALIZER
+        self.globals["entity_contexts"] = EntityContexts()
+        self.globals["localizer"] = DEFAULT_LOCALIZER
 
     def _init_extensions(self) -> None:
         for extension in self.app.extensions.flatten():
             if isinstance(extension, Jinja2Provider):
                 self.globals.update(extension.globals)
                 self.filters.update(extension.filters)
                 self.tests.update(extension.tests)
 
 
-Template.environment_class = Environment
-
-
 class Jinja2Renderer(Renderer):
     def __init__(self, environment: Environment, configuration: ProjectConfiguration):
         self._environment = environment
         self._configuration = configuration
 
     @property
     def file_extensions(self) -> set[str]:
-        return {'.j2'}
+        return {".j2"}
 
     async def render_file(
         self,
         file_path: Path,
         *,
         job_context: JobContext | None = None,
         localizer: Localizer | None = None,
     ) -> Path:
         destination_file_path = file_path.parent / file_path.stem
         data: dict[str, Any] = {}
         if job_context is not None:
-            data['job_context'] = job_context
+            data["job_context"] = job_context
         if localizer is not None:
-            data['localizer'] = localizer
+            data["localizer"] = localizer
         try:
-            relative_file_destination_path = destination_file_path.relative_to(self._configuration.www_directory_path)
+            relative_file_destination_path = destination_file_path.relative_to(
+                self._configuration.www_directory_path
+            )
         except ValueError:
             pass
         else:
-            resource = '/'.join(relative_file_destination_path.parts)
+            resource = "/".join(relative_file_destination_path.parts)
             if self._configuration.locales.multilingual:
-                resource_parts = resource.lstrip('/').split('/')
-                if resource_parts[0] in map(lambda x: x.alias, self._configuration.locales.values()):
-                    resource = '/'.join(resource_parts[1:])
-            data['page_resource'] = resource
+                resource_parts = resource.lstrip("/").split("/")
+                if resource_parts[0] in map(
+                    lambda x: x.alias, self._configuration.locales.values()
+                ):
+                    resource = "/".join(resource_parts[1:])
+            data["page_resource"] = resource
         async with aiofiles.open(file_path) as f:
             template_source = await f.read()
-        rendered = await self._environment.from_string(template_source, self._environment.globals).render_async(data)
-        async with aiofiles.open(destination_file_path, 'w', encoding='utf-8') as f:
+        rendered = await self._environment.from_string(
+            template_source, self._environment.globals
+        ).render_async(data)
+        async with aiofiles.open(destination_file_path, "w", encoding="utf-8") as f:
             await f.write(rendered)
         await aiofiles_os.remove(file_path)
         return destination_file_path
```

### Comparing `betty-0.3.3/betty/jinja2/filter.py` & `betty-0.3.4/betty/jinja2/filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide Betty's default Jinja2 filters.
 """
+
 from __future__ import annotations
 
 import json as stdjson
 import re
 import warnings
 from asyncio import get_running_loop, run
 from base64 import b64encode
@@ -17,35 +18,47 @@
 
 import aiofiles
 from PIL import Image
 from PIL.Image import DecompressionBombWarning
 from aiofiles.os import makedirs
 from geopy import units
 from geopy.format import DEGREES_FORMAT
-from jinja2 import pass_context, \
-    pass_eval_context
+from jinja2 import pass_context, pass_eval_context
 from jinja2.async_utils import auto_aiter, auto_await
 from jinja2.filters import prepare_map, make_attrgetter
 from jinja2.nodes import EvalContext
 from jinja2.runtime import Context, Macro
 from markupsafe import Markup, escape
 from pdf2image.pdf2image import convert_from_path
 
 from betty import _resizeimage
-from betty.fs import hashfile
 from betty.functools import walk
-from betty.locale import negotiate_localizeds, Localized, Datey, negotiate_locale, Localey, get_data, Localizable
+from betty.hashid import hashid_file_meta, hashid
+from betty.locale import (
+    negotiate_localizeds,
+    Localized,
+    Datey,
+    negotiate_locale,
+    Localey,
+    get_data,
+    Localizable,
+)
 from betty.media_type import MediaType
 from betty.model import get_entity_type_name
 from betty.model.ancestry import File, Dated
 from betty.os import link_or_copy
 from betty.serde.dump import minimize, none_void, void_none
-from betty.string import camel_case_to_snake_case, camel_case_to_kebab_case, upper_camel_case_to_lower_camel_case
+from betty.string import (
+    camel_case_to_snake_case,
+    camel_case_to_kebab_case,
+    upper_camel_case_to_lower_camel_case,
+)
+from betty.warnings import deprecated
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 @pass_context
 def filter_url(
     context: Context,
     resource: Any,
     media_type: str | None = None,
@@ -56,15 +69,15 @@
     """
     Generate a localized URL for a localizable resource.
     """
     from betty.jinja2 import context_app, context_localizer
 
     return context_app(context).url_generator.generate(
         resource,
-        media_type or 'text/html',
+        media_type or "text/html",
         *args,
         locale=locale or context_localizer(context).locale,  # type: ignore[misc]
         **kwargs,
     )
 
 
 @pass_context
@@ -129,44 +142,46 @@
 def filter_walk(value: Any, attribute_name: str) -> Iterable[Any]:
     """
     Walk over a data structure.
     """
     return walk(value, attribute_name)
 
 
-_paragraph_re = re.compile(r'(?:\r\n|\r|\n){2,}')
+_paragraph_re = re.compile(r"(?:\r\n|\r|\n){2,}")
 
 
 @pass_eval_context
 def filter_paragraphs(eval_ctx: EvalContext, text: str) -> str | Markup:
     """
     Convert newlines to <p> and <br> tags.
 
     Taken from http://jinja.pocoo.org/docs/2.10/api/#custom-filters.
     """
-    result = u'\n\n'.join(u'<p>%s</p>' % p.replace('\n', Markup('<br>\n'))
-                          for p in _paragraph_re.split(escape(text)))
+    result = "\n\n".join(
+        "<p>%s</p>" % p.replace("\n", Markup("<br>\n"))
+        for p in _paragraph_re.split(escape(text))
+    )
     if eval_ctx.autoescape:
         result = Markup(result)
     return result
 
 
 def filter_format_degrees(degrees: int) -> str:
     """
     Format geographic coordinates.
     """
     arcminutes = units.arcminutes(degrees=degrees - int(degrees))
     arcseconds = units.arcseconds(arcminutes=arcminutes - int(arcminutes))
     format_dict = dict(
-        deg='°',
+        deg="°",
         arcmin="'",
         arcsec='"',
         degrees=degrees,
         minutes=round(abs(arcminutes)),
-        seconds=round(abs(arcseconds))
+        seconds=round(abs(arcseconds)),
     )
     return DEGREES_FORMAT % format_dict  # type: ignore[no-any-return]
 
 
 async def filter_unique(value: Iterable[T]) -> AsyncIterator[T]:
     """
     Iterate over an iterable of values and only yield those values that have not been yielded before.
@@ -175,15 +190,17 @@
     async for value in auto_aiter(value):
         if value not in seen:
             yield value
             seen.append(value)
 
 
 @pass_context
-async def filter_map(context: Context, values: Iterable[Any], *args: Any, **kwargs: Any) -> Any:
+async def filter_map(
+    context: Context, values: Iterable[Any], *args: Any, **kwargs: Any
+) -> Any:
     """
     Map an iterable's values.
 
     This mimics Jinja2's built-in map filter, but allows macros as callbacks.
     """
     if len(args) > 0 and isinstance(args[0], Macro):
         func: Macro | Callable[[Any], bool] = args[0]
@@ -203,26 +220,35 @@
     from betty.jinja2 import context_app, context_job_context
 
     app = context_app(context)
     job_context = context_job_context(context)
 
     execute_filter = True
     if job_context:
-        job_cache_item_id = f'filter_file:{file.id}'
-        async with job_context.cache.getset(job_cache_item_id, wait=False) as (cache_item, setter):
+        job_cache_item_id = f"filter_file:{file.id}"
+        async with job_context.cache.getset(job_cache_item_id, wait=False) as (
+            cache_item,
+            setter,
+        ):
             if cache_item is None and setter is not None:
                 await setter(None)
             else:
                 execute_filter = False
     if execute_filter:
-        file_destination_path = app.project.configuration.www_directory_path / 'file' / file.id / 'file' / file.path.name
+        file_destination_path = (
+            app.project.configuration.www_directory_path
+            / "file"
+            / file.id
+            / "file"
+            / file.path.name
+        )
         await makedirs(file_destination_path.parent, exist_ok=True)
         await link_or_copy(file.path, file_destination_path)
 
-    return f'/file/{quote(file.id)}/file/{quote(file.path.name)}'
+    return f"/file/{quote(file.id)}/file/{quote(file.path.name)}"
 
 
 @pass_context
 async def filter_image(
     context: Context,
     file: File,
     width: int | None = None,
@@ -232,116 +258,128 @@
     Preprocess an image file for use in a page.
 
     :return: The public path to the preprocessed file. This can be embedded in a web page.
     """
     from betty.jinja2 import context_app, context_job_context
 
     # Treat SVGs as regular files.
-    if file.media_type and file.media_type.type == 'image' and 'svg+xml' == file.media_type.subtype:
+    if (
+        file.media_type
+        and file.media_type.type == "image"
+        and "svg+xml" == file.media_type.subtype
+    ):
         return await filter_file(context, file)
 
     app = context_app(context)
     job_context = context_job_context(context)
 
-    destination_name = f'{file.id}-'
+    destination_name = f"{file.id}-"
     if height and width:
-        destination_name += f'{width}x{height}'
+        destination_name += f"{width}x{height}"
     elif height:
-        destination_name += f'-x{height}'
+        destination_name += f"-x{height}"
     elif width:
-        destination_name += f'{width}x-'
+        destination_name += f"{width}x-"
     else:
-        raise ValueError('At least the width or height must be given.')
+        raise ValueError("At least the width or height must be given.")
 
-    file_directory_path = app.project.configuration.www_directory_path / 'file'
+    file_directory_path = app.project.configuration.www_directory_path / "file"
 
     if file.media_type:
-        if file.media_type.type == 'image':
+        if file.media_type.type == "image":
             image_loader = _load_image_image
             destination_name += file.path.suffix
-        elif file.media_type.type == 'application' and file.media_type.subtype == 'pdf':
+        elif file.media_type.type == "application" and file.media_type.subtype == "pdf":
             image_loader = _load_image_application_pdf
-            destination_name += '.' + 'jpg'
+            destination_name += "." + "jpg"
         else:
-            raise ValueError(f'Cannot convert a file of media type "{file.media_type}" to an image.')
+            raise ValueError(
+                f'Cannot convert a file of media type "{file.media_type}" to an image.'
+            )
     else:
-        raise ValueError('Cannot convert a file without a media type to an image.')
+        raise ValueError("Cannot convert a file without a media type to an image.")
 
-    cache_item_id = f'{hashfile(file.path)}:{"" if width is None else width}:{"" if height is None else height}'
+    cache_item_id = f'{await hashid_file_meta(file.path)}:{"" if width is None else width}:{"" if height is None else height}'
     execute_filter = True
     if job_context:
-        async with job_context.cache.with_scope('filter_image').getset(cache_item_id, wait=False) as (cache_item, setter):
+        async with job_context.cache.with_scope("filter_image").getset(
+            cache_item_id, wait=False
+        ) as (cache_item, setter):
             if cache_item is None and setter is not None:
                 await setter(True)
             else:
                 execute_filter = False
     if execute_filter:
         loop = get_running_loop()
         await loop.run_in_executor(
             app.process_pool,
             _execute_filter_image,
             image_loader,
             file.path,
             file.media_type,
-            app.binary_file_cache.with_scope('image').cache_item_file_path(cache_item_id),
+            app.binary_file_cache.with_scope("image").cache_item_file_path(
+                cache_item_id
+            ),
             file_directory_path,
             destination_name,
             width,
             height,
         )
-    destination_public_path = f'/file/{quote(destination_name)}'
+    destination_public_path = f"/file/{quote(destination_name)}"
 
     return destination_public_path
 
 
 async def _load_image_image(
     file_path: Path,
     media_type: MediaType,
 ) -> Image.Image:
     # We want to read the image asynchronously and prevent Pillow from keeping too many file
     # descriptors open simultaneously, so we read the image ourselves and store the contents
     # in a synchronous file object.
-    async with aiofiles.open(file_path, 'rb') as f:
+    async with aiofiles.open(file_path, "rb") as f:
         image_f = BytesIO(await f.read())
     # Ignore warnings about decompression bombs, because we know where the files come from.
-    with warnings.catch_warnings(action='ignore', category=DecompressionBombWarning):
+    with warnings.catch_warnings(action="ignore", category=DecompressionBombWarning):
         image = Image.open(image_f, formats=[media_type.subtype])
     return image
 
 
 async def _load_image_application_pdf(
     file_path: Path,
     media_type: MediaType,
 ) -> Image.Image:
     # Ignore warnings about decompression bombs, because we know where the files come from.
-    with warnings.catch_warnings(action='ignore', category=DecompressionBombWarning):
-        image = convert_from_path(file_path, fmt='jpeg')[0]
+    with warnings.catch_warnings(action="ignore", category=DecompressionBombWarning):
+        image = convert_from_path(file_path, fmt="jpeg")[0]
     return image
 
 
 def _execute_filter_image(
     image_loader: Callable[[Path, MediaType], Awaitable[Image.Image]],
     file_path: Path,
     media_type: MediaType,
     cache_item_file_path: Path,
     destination_directory_path: Path,
     destination_name: str,
     width: int | None,
     height: int | None,
 ) -> None:
-    run(__execute_filter_image(
-        image_loader,
-        file_path,
-        media_type,
-        cache_item_file_path,
-        destination_directory_path,
-        destination_name,
-        width,
-        height,
-    ))
+    run(
+        __execute_filter_image(
+            image_loader,
+            file_path,
+            media_type,
+            cache_item_file_path,
+            destination_directory_path,
+            destination_name,
+            width,
+            height,
+        )
+    )
 
 
 async def __execute_filter_image(
     image_loader: Callable[[Path, MediaType], Awaitable[Image.Image]],
     file_path: Path,
     media_type: MediaType,
     cache_item_file_path: Path,
@@ -379,117 +417,180 @@
 ) -> Image.Image:
     if width is not None and height is not None:
         return _resizeimage.resize_cover(image, (width, height))
     if width is not None:
         return _resizeimage.resize_width(image, width)
     if height is not None:
         return _resizeimage.resize_height(image, height)
-    raise ValueError('Width and height cannot both be None.')
+    raise ValueError("Width and height cannot both be None.")
 
 
 @pass_context
-def filter_negotiate_localizeds(context: Context, localizeds: Iterable[Localized]) -> Localized | None:
+def filter_negotiate_localizeds(
+    context: Context, localizeds: Iterable[Localized]
+) -> Localized | None:
     """
     Try to find an object whose locale matches the context's current locale.
     """
     from betty.jinja2 import context_localizer
 
     return negotiate_localizeds(context_localizer(context).locale, list(localizeds))
 
 
 @pass_context
-def filter_sort_localizeds(context: Context, localizeds: Iterable[Localized], localized_attribute: str, sort_attribute: str) -> Iterable[Localized]:
+def filter_sort_localizeds(
+    context: Context,
+    localizeds: Iterable[Localized],
+    localized_attribute: str,
+    sort_attribute: str,
+) -> Iterable[Localized]:
     """
     Sort localized objects.
     """
     from betty.jinja2 import context_localizer
 
-    get_localized_attr = make_attrgetter(
-        context.environment, localized_attribute)
+    get_localized_attr = make_attrgetter(context.environment, localized_attribute)
     get_sort_attr = make_attrgetter(context.environment, sort_attribute)
 
     def _get_sort_key(x: Localized) -> Any:
-        return get_sort_attr(negotiate_localizeds(context_localizer(context).locale, get_localized_attr(x)))
+        return get_sort_attr(
+            negotiate_localizeds(
+                context_localizer(context).locale, get_localized_attr(x)
+            )
+        )
 
     return sorted(localizeds, key=_get_sort_key)
 
 
 @pass_context
-def filter_select_localizeds(context: Context, localizeds: Iterable[Localized], include_unspecified: bool = False) -> Iterable[Localized]:
+def filter_select_localizeds(
+    context: Context, localizeds: Iterable[Localized], include_unspecified: bool = False
+) -> Iterable[Localized]:
     """
     Select all objects whose locale matches the context's current locale.
 
     :param include_unspecified: If True, the return value includes all objects that do not have a locale specified.
     """
     from betty.jinja2 import context_localizer
 
     for localized in localizeds:
-        if include_unspecified and localized.locale in {None, 'mis', 'mul', 'und', 'zxx'}:
+        if include_unspecified and localized.locale in {
+            None,
+            "mis",
+            "mul",
+            "und",
+            "zxx",
+        }:
             yield localized
-        if localized.locale is not None and negotiate_locale(context_localizer(context).locale, [localized.locale]) is not None:
+        if (
+            localized.locale is not None
+            and negotiate_locale(context_localizer(context).locale, [localized.locale])
+            is not None
+        ):
             yield localized
 
 
 @pass_context
-def filter_negotiate_dateds(context: Context, dateds: Iterable[Dated], date: Datey | None) -> Dated | None:
+def filter_negotiate_dateds(
+    context: Context, dateds: Iterable[Dated], date: Datey | None
+) -> Dated | None:
     """
     Try to find an object whose date falls in the given date.
 
     :param date: A date to select by. If None, then today's date is used.
     """
     with suppress(StopIteration):
         return next(filter_select_dateds(context, dateds, date))
     return None
 
 
 @pass_context
-def filter_select_dateds(context: Context, dateds: Iterable[Dated], date: Datey | None) -> Iterator[Dated]:
+def filter_select_dateds(
+    context: Context, dateds: Iterable[Dated], date: Datey | None
+) -> Iterator[Dated]:
     """
     Select all objects whose date falls in the given date.
 
     :param date: A date to select by. If None, then today's date is used.
     """
     if date is None:
-        date = context.resolve_or_missing('today')
+        date = context.resolve_or_missing("today")
     return filter(
-        lambda dated: dated.date is None or dated.date.comparable and dated.date in date,
+        lambda dated: dated.date is None
+        or dated.date.comparable
+        and dated.date in date,
         dateds,
     )
 
 
+@deprecated(
+    "This function is deprecated as of Betty 0.3.4, and will be removed in Betty 0.4.x. Instead, use the `hashid` filter."
+)
 def filter_base64(input: str) -> str:
     """
     Base-64-encode a string.
     """
-    return b64encode(input.encode('utf-8')).decode('utf-8')
+    return b64encode(input.encode("utf-8")).decode("utf-8")
+
+
+def filter_hashid(input: str) -> str:
+    """
+    Create a hash ID.
+    """
+    return hashid(input)
+
+
+@pass_context
+def filter_public_css(context: Context, public_path: str) -> None:
+    """
+    Add a CSS file to the current page.
+    """
+    public_css_paths = context.resolve_or_missing("public_css_paths")
+    if public_path in public_css_paths:
+        return
+    public_css_paths.append(public_path)
+
+
+@pass_context
+def filter_public_js(context: Context, public_path: str) -> None:
+    """
+    Add a JavaScript file to the current page.
+    """
+    public_js_paths = context.resolve_or_missing("public_js_paths")
+    if public_path in public_js_paths:
+        return
+    public_js_paths.append(public_path)
 
 
 FILTERS = {
-    'base64': filter_base64,
-    'camel_case_to_kebab_case': camel_case_to_kebab_case,
-    'camel_case_to_snake_case': camel_case_to_snake_case,
-    'entity_type_name': get_entity_type_name,
-    'file': filter_file,
-    'flatten': filter_flatten,
-    'format_datey': filter_format_datey,
-    'format_degrees': filter_format_degrees,
-    'image': filter_image,
-    'json': filter_json,
-    'locale_get_data': get_data,
-    'localize': filter_localize,
-    'map': filter_map,
-    'minimize': minimize,
-    'negotiate_dateds': filter_negotiate_dateds,
-    'negotiate_localizeds': filter_negotiate_localizeds,
-    'none_void': none_void,
-    'paragraphs': filter_paragraphs,
-    'select_dateds': filter_select_dateds,
-    'select_localizeds': filter_select_localizeds,
-    'static_url': filter_static_url,
-    'sort_localizeds': filter_sort_localizeds,
-    'str': str,
-    'unique': filter_unique,
-    'upper_camel_case_to_lower_camel_case': upper_camel_case_to_lower_camel_case,
-    'url': filter_url,
-    'void_none': void_none,
-    'walk': filter_walk,
+    "base64": filter_base64,
+    "camel_case_to_kebab_case": camel_case_to_kebab_case,
+    "camel_case_to_snake_case": camel_case_to_snake_case,
+    "entity_type_name": get_entity_type_name,
+    "file": filter_file,
+    "flatten": filter_flatten,
+    "format_datey": filter_format_datey,
+    "format_degrees": filter_format_degrees,
+    "hashid": filter_hashid,
+    "image": filter_image,
+    "json": filter_json,
+    "locale_get_data": get_data,
+    "localize": filter_localize,
+    "map": filter_map,
+    "minimize": minimize,
+    "negotiate_dateds": filter_negotiate_dateds,
+    "negotiate_localizeds": filter_negotiate_localizeds,
+    "none_void": none_void,
+    "paragraphs": filter_paragraphs,
+    "select_dateds": filter_select_dateds,
+    "select_localizeds": filter_select_localizeds,
+    "static_url": filter_static_url,
+    "sort_localizeds": filter_sort_localizeds,
+    "str": str,
+    "unique": filter_unique,
+    "upper_camel_case_to_lower_camel_case": upper_camel_case_to_lower_camel_case,
+    "url": filter_url,
+    "void_none": void_none,
+    "walk": filter_walk,
+    "public_css": filter_public_css,
+    "public_js": filter_public_js,
 }
```

### Comparing `betty-0.3.3/betty/jinja2/test.py` & `betty-0.3.4/betty/jinja2/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 """
 Provide Betty's default Jinja2 tests.
 """
+
 from __future__ import annotations
 
 from typing import Any, TypeVar
 
 from betty.json.linked_data import LinkedDataDumpable
 from betty.locale import DateRange
 from betty.model import Entity, GeneratedEntityId, UserFacingEntity, get_entity_type
-from betty.model.ancestry import HasLinks, HasFiles, Subject, Witness, is_private, is_public, Event
+from betty.model.ancestry import (
+    HasLinks,
+    HasFiles,
+    Subject,
+    Witness,
+    is_private,
+    is_public,
+    Event,
+)
 from betty.model.event_type import StartOfLifeEventType, EndOfLifeEventType
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 def test_linked_data_dumpable(value: Any) -> bool:
     """
     Test if a value can be dumped to Linked Data.
     """
     return isinstance(value, LinkedDataDumpable)
@@ -95,21 +104,21 @@
     """
     Test if an event is an end-of-life event.
     """
     return issubclass(event.event_type, EndOfLifeEventType)
 
 
 TESTS = {
-    'date_range': test_date_range,
-    'end_of_life_event': test_end_of_life_event,
-    'entity': test_entity,
-    'has_files': test_has_files,
-    'has_generated_entity_id': test_has_generated_entity_id,
-    'has_links': test_has_links,
-    'linked_data_dumpable': test_linked_data_dumpable,
-    'private': is_private,
-    'public': is_public,
-    'start_of_life_event': test_start_of_life_event,
-    'subject_role': test_subject_role,
-    'user_facing_entity': test_user_facing_entity,
-    'witness_role': test_witness_role,
+    "date_range": test_date_range,
+    "end_of_life_event": test_end_of_life_event,
+    "entity": test_entity,
+    "has_files": test_has_files,
+    "has_generated_entity_id": test_has_generated_entity_id,
+    "has_links": test_has_links,
+    "linked_data_dumpable": test_linked_data_dumpable,
+    "private": is_private,
+    "public": is_public,
+    "start_of_life_event": test_start_of_life_event,
+    "subject_role": test_subject_role,
+    "user_facing_entity": test_user_facing_entity,
+    "witness_role": test_witness_role,
 }
```

### Comparing `betty-0.3.3/betty/job.py` & `betty-0.3.4/betty/job.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 class Context:
     def __init__(self, localizer: Localizer | None = None):
         self._cache: Cache[Any] = MemoryCache(localizer or DEFAULT_LOCALIZER)
         self._claims_lock = threading.Lock()
         self._claimed_job_ids: set[str] = set()
 
-    @deprecated('This method is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x. Use `Context.cache` instead.')
+    @deprecated(
+        "This method is deprecated as of Betty 0.3.3, and will be removed in Betty 0.4.x. Use `Context.cache` instead."
+    )
     def claim(self, job_id: str) -> bool:
         with self._claims_lock:
             if job_id in self._claimed_job_ids:
                 return False
             self._claimed_job_ids.add(job_id)
         return True
```

### Comparing `betty-0.3.3/betty/json/linked_data.py` & `betty-0.3.4/betty/json/linked_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide `JSON-LD <https://json-ld.org/>`_ utilities.
 """
+
 from __future__ import annotations
 
 from collections.abc import Sequence
 from typing import TYPE_CHECKING
 
 from betty.serde.dump import DictDump, Dump, dump_default
 
@@ -28,42 +29,44 @@
         return {}
 
 
 def dump_context(dump: DictDump[Dump], **contexts: str | Sequence[str]) -> None:
     """
     Add one or more contexts to a dump.
     """
-    context_dump = dump_default(dump, '@context', dict)
+    context_dump = dump_default(dump, "@context", dict)
     for key, schema_org in contexts.items():
-        context_dump[key] = f'https://schema.org/{schema_org}'
+        context_dump[key] = f"https://schema.org/{schema_org}"
 
 
 async def dump_link(dump: DictDump[Dump], app: App, *links: Link) -> None:
     """
     Add one or more links to a dump.
     """
-    link_dump = dump_default(dump, 'links', list)
+    link_dump = dump_default(dump, "links", list)
     for link in links:
         link_dump.append(await link.dump_linked_data(app))
 
 
 def ref_json_ld(root_schema: DictDump[Dump]) -> DictDump[Dump]:
     """
     Reference the JSON-LD schema.
     """
-    definitions = dump_default(root_schema, 'definitions', dict)
-    if 'jsonLd' not in definitions:
-        definitions['jsonLd'] = {
-            'description': 'A JSON-LD annotation.',
+    definitions = dump_default(root_schema, "definitions", dict)
+    if "jsonLd" not in definitions:
+        definitions["jsonLd"] = {
+            "description": "A JSON-LD annotation.",
         }
     return {
-        '$ref': '#/definitions/jsonLd',
+        "$ref": "#/definitions/jsonLd",
     }
 
 
-def add_json_ld(schema: DictDump[Dump], root_schema: DictDump[Dump] | None = None) -> None:
+def add_json_ld(
+    schema: DictDump[Dump], root_schema: DictDump[Dump] | None = None
+) -> None:
     """
     Allow JSON-LD properties to be added to a schema.
     """
-    schema['patternProperties'] = {
-        '^@': ref_json_ld(root_schema or schema),
+    schema["patternProperties"] = {
+        "^@": ref_json_ld(root_schema or schema),
     }
```

### Comparing `betty-0.3.3/betty/json/schema.py` & `betty-0.3.4/betty/json/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,134 +1,149 @@
 """
 Provide JSON utilities.
 """
+
 from __future__ import annotations
 
 from typing import Any, TypeVar, TYPE_CHECKING, cast
 
 from jsonschema.validators import Draft202012Validator
 from referencing import Resource, Registry
 
 from betty.serde.dump import DictDump, Dump, dump_default
 from betty.string import upper_camel_case_to_lower_camel_case
 
 if TYPE_CHECKING:
     from betty.app import App
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class Schema:
     def __init__(self, app: App):
         self._app = app
 
     async def build(self) -> DictDump[Dump]:
         from betty.model import get_entity_type_name
 
         schema: DictDump[Dump] = {
-            '$schema': 'https://json-schema.org/draft/2020-12/schema',
-            '$id': self._app.static_url_generator.generate('schema.json', absolute=True),
+            "$schema": "https://json-schema.org/draft/2020-12/schema",
+            "$id": self._app.static_url_generator.generate(
+                "schema.json", absolute=True
+            ),
         }
 
-        definitions = dump_default(schema, 'definitions', dict)
-        entity_definitions = dump_default(definitions, 'entity', dict)
-        response_definitions = dump_default(definitions, 'response', dict)
+        definitions = dump_default(schema, "definitions", dict)
+        entity_definitions = dump_default(definitions, "entity", dict)
+        response_definitions = dump_default(definitions, "response", dict)
 
         # Add entity schemas.
         for entity_type in self._app.entity_types:
-            entity_type_schema_name = upper_camel_case_to_lower_camel_case(get_entity_type_name(entity_type))
+            entity_type_schema_name = upper_camel_case_to_lower_camel_case(
+                get_entity_type_name(entity_type)
+            )
             entity_type_schema = await entity_type.linked_data_schema(self._app)
-            entity_type_schema_definitions = cast(DictDump[Dump], entity_type_schema.pop('definitions', {}))
-            for definition_name, definition_schema in entity_type_schema_definitions.items():
+            entity_type_schema_definitions = cast(
+                DictDump[Dump], entity_type_schema.pop("definitions", {})
+            )
+            for (
+                definition_name,
+                definition_schema,
+            ) in entity_type_schema_definitions.items():
                 if definition_name not in definitions:
                     definitions[definition_name] = definition_schema
             entity_definitions[entity_type_schema_name] = entity_type_schema
-            entity_definitions[f'{entity_type_schema_name}Collection'] = {
-                'type': 'array',
-                'items': {
-                    'type': 'string',
-                    'format': 'uri',
+            entity_definitions[f"{entity_type_schema_name}Collection"] = {
+                "type": "array",
+                "items": {
+                    "type": "string",
+                    "format": "uri",
                 },
             }
-            response_definitions[f'{entity_type_schema_name}Collection'] = {
-                'type': 'object',
-                'properties': {
-                    'collection': {
-                        '$ref': f'#/definitions/entity/{entity_type_schema_name}Collection',
+            response_definitions[f"{entity_type_schema_name}Collection"] = {
+                "type": "object",
+                "properties": {
+                    "collection": {
+                        "$ref": f"#/definitions/entity/{entity_type_schema_name}Collection",
                     },
                 },
             }
 
         # Add the HTTP error response.
-        response_definitions['error'] = {
-            'type': 'object',
-            'properties': {
-                '$schema': ref_json_schema(schema),
-                'message': {
-                    'type': 'string',
+        response_definitions["error"] = {
+            "type": "object",
+            "properties": {
+                "$schema": ref_json_schema(schema),
+                "message": {
+                    "type": "string",
                 },
             },
-            'required': [
-                '$schema',
-                'message',
+            "required": [
+                "$schema",
+                "message",
             ],
-            'additionalProperties': False,
+            "additionalProperties": False,
         }
 
         return schema
 
     async def validate(self, data: Any) -> None:
         """
         Validate JSON against the Betty JSON schema.
         """
         schema = Resource.from_contents(await self.build())
         schema_registry = schema @ Registry()  # type: ignore[operator, var-annotated]
         validator = Draft202012Validator(
             {
-                '$ref': data['$schema'],
+                "$ref": data["$schema"],
             },
             registry=schema_registry,
         )
         validator.validate(data)
 
 
-def add_property(schema: DictDump[Dump], property_name: str, property_schema: DictDump[Dump], property_required: bool = True) -> None:
+def add_property(
+    schema: DictDump[Dump],
+    property_name: str,
+    property_schema: DictDump[Dump],
+    property_required: bool = True,
+) -> None:
     """
     Add a property to an object schema.
     """
-    schema_properties = dump_default(schema, 'properties', dict)
+    schema_properties = dump_default(schema, "properties", dict)
     schema_properties[property_name] = property_schema
     if property_required:
-        schema_required = dump_default(schema, 'required', list)
+        schema_required = dump_default(schema, "required", list)
         schema_required.append(property_name)
 
 
 def ref_locale(root_schema: DictDump[Dump]) -> DictDump[Dump]:
     """
     Reference the locale schema.
     """
-    definitions = dump_default(root_schema, 'definitions', dict)
-    if 'locale' not in definitions:
-        definitions['locale'] = {
-            'type': 'string',
-            'description': 'A BCP 47 locale identifier (https://www.ietf.org/rfc/bcp/bcp47.txt).',
+    definitions = dump_default(root_schema, "definitions", dict)
+    if "locale" not in definitions:
+        definitions["locale"] = {
+            "type": "string",
+            "description": "A BCP 47 locale identifier (https://www.ietf.org/rfc/bcp/bcp47.txt).",
         }
     return {
-        '$ref': '#/definitions/locale',
+        "$ref": "#/definitions/locale",
     }
 
 
 def ref_json_schema(root_schema: DictDump[Dump]) -> DictDump[Dump]:
     """
     Reference the JSON Schema schema.
     """
-    definitions = dump_default(root_schema, 'definitions', dict)
-    if 'schema' not in definitions:
-        definitions['schema'] = {
-            'type': 'string',
-            'format': 'uri',
-            'description': 'A JSON Schema URI.',
+    definitions = dump_default(root_schema, "definitions", dict)
+    if "schema" not in definitions:
+        definitions["schema"] = {
+            "type": "string",
+            "format": "uri",
+            "description": "A JSON Schema URI.",
         }
     return {
-        '$ref': '#/definitions/schema',
+        "$ref": "#/definitions/schema",
     }
```

### Comparing `betty-0.3.3/betty/load.py` & `betty-0.3.4/betty/load.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Provide the Ancestry loading API.
 """
+
 import logging
 
 from betty.app import App
 from betty.warnings import deprecated
 
 
-@deprecated('This function is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, use `logging.getLogger()`.')
+@deprecated(
+    "This function is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, use `logging.getLogger()`."
+)
 def getLogger() -> logging.Logger:
     """
     Get the ancestry loading logger.
     """
     return logging.getLogger(__name__)
```

### Comparing `betty-0.3.3/betty/locale.py` & `betty-0.3.4/betty/locale.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 """
 Provide the Locale API.
 """
+
 from __future__ import annotations
 
-import asyncio
 import calendar
 import datetime
 import gettext
 import glob
 import logging
 import operator
-import threading
+from asyncio import to_thread
 from collections import defaultdict
 from collections.abc import AsyncIterator
-from contextlib import suppress, redirect_stdout, chdir
+from contextlib import suppress, redirect_stdout, redirect_stderr
 from functools import total_ordering
 from io import StringIO
 from pathlib import Path
-from typing import Any, Iterator, Sequence, Mapping, Callable, TypeAlias, cast, TYPE_CHECKING
+from typing import (
+    Any,
+    Iterator,
+    Sequence,
+    Mapping,
+    Callable,
+    TypeAlias,
+    cast,
+    TYPE_CHECKING,
+)
 from warnings import warn
 
 import aiofiles
 import babel
 from aiofiles.os import makedirs
 from aiofiles.ospath import exists
 from babel import dates, Locale
 from babel.messages.frontend import CommandLineInterface
 from langcodes import Language
 from polib import pofile
 
 from betty import fs
 from betty.asyncio import wait_to_thread
-from betty.fs import hashfile, FileSystem, ROOT_DIRECTORY_PATH
+from betty.concurrent import _Lock, AsynchronizedLock
+from betty.fs import FileSystem, ROOT_DIRECTORY_PATH
+from betty.hashid import hashid_file_meta
 from betty.json.linked_data import LinkedDataDumpable, dump_context, add_json_ld
 from betty.json.schema import ref_locale, add_property
 from betty.serde.dump import DictDump, Dump, dump_default
+from betty.warnings import deprecated
 
 if TYPE_CHECKING:
     from betty.app import App
 
 
-DEFAULT_LOCALE = 'en-US'
+DEFAULT_LOCALE = "en-US"
 
-_LOCALE_DIRECTORY_PATH = fs.ASSETS_DIRECTORY_PATH / 'locale'
+_LOCALE_DIRECTORY_PATH = fs.ASSETS_DIRECTORY_PATH / "locale"
 
 
 class LocaleNotFoundError(RuntimeError):
     def __init__(self, locale: str) -> None:
         super().__init__(f'Cannot find locale "{locale}"')
         self.locale = locale
 
@@ -54,36 +66,34 @@
 def to_babel_identifier(locale: Localey) -> str:
     """
     Convert a locale or locale metadata to a Babel locale identifier.
     """
     if isinstance(locale, Locale):
         return str(locale)
     language_data = Language.get(locale)
-    return '_'.join(
+    return "_".join(
         part
-        for part
-        in [
+        for part in [
             language_data.language,
             language_data.script,
             language_data.territory,
         ]
         if part
     )
 
 
 def to_locale(locale: Localey) -> str:
     """
     Ensure that a locale or locale metadata is a locale.
     """
     if isinstance(locale, str):
         return locale
-    return '-'.join(
+    return "-".join(
         part
-        for part
-        in [
+        for part in [
             locale.language,
             locale.script,
             locale.territory,
         ]
         if part
     )
 
@@ -95,19 +105,21 @@
     """
     Get locale metadata.
     """
     if isinstance(locale, Locale):
         return locale
     try:
         return Locale.parse(to_babel_identifier(locale))
-    except BaseException as e:
+    except Exception as e:
         raise LocaleNotFoundError(locale) from e
 
 
-def get_display_name(locale: Localey, display_locale: Localey | None = None) -> str | None:
+def get_display_name(
+    locale: Localey, display_locale: Localey | None = None
+) -> str | None:
     """
     Return a locale's human-readable display name.
     """
     locale_data = get_data(locale)
     return locale_data.get_display_name(
         get_data(display_locale) if display_locale else locale_data
     )
@@ -124,36 +136,36 @@
     ):
         super().__init__(*args, **kwargs)
         self.locale = locale
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
         if self.locale is not None:
-            dump['locale'] = self.locale
+            dump["locale"] = self.locale
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        properties = dump_default(schema, 'properties', dict)
-        properties['locale'] = ref_locale(schema)
+        properties = dump_default(schema, "properties", dict)
+        properties["locale"] = ref_locale(schema)
         return schema
 
 
 class IncompleteDateError(ValueError):
     pass
 
 
 def _dump_date_iso8601(date: Date) -> str | None:
     if not date.complete:
         return None
     assert date.year
     assert date.month
     assert date.day
-    return f'{date.year:04d}-{date.month:02d}-{date.day:02d}'
+    return f"{date.year:04d}-{date.month:02d}-{date.day:02d}"
 
 
 class Date(LinkedDataDumpable):
     year: int | None
     month: int | None
     day: int | None
     fuzzy: bool
@@ -167,15 +179,21 @@
     ):
         self.year = year
         self.month = month
         self.day = day
         self.fuzzy = fuzzy
 
     def __repr__(self) -> str:
-        return '<%s.%s(%s, %s, %s)>' % (self.__class__.__module__, self.__class__.__name__, self.year, self.month, self.day)
+        return "<%s.%s(%s, %s, %s)>" % (
+            self.__class__.__module__,
+            self.__class__.__name__,
+            self.year,
+            self.month,
+            self.day,
+        )
 
     @property
     def comparable(self) -> bool:
         return self.year is not None
 
     @property
     def complete(self) -> bool:
@@ -183,29 +201,33 @@
 
     @property
     def parts(self) -> tuple[int | None, int | None, int | None]:
         return self.year, self.month, self.day
 
     def to_range(self) -> DateRange:
         if not self.comparable:
-            raise ValueError('Cannot convert non-comparable date %s to a date range.' % self)
+            raise ValueError(
+                "Cannot convert non-comparable date %s to a date range." % self
+            )
         if self.month is None:
             month_start = 1
             month_end = 12
         else:
             month_start = month_end = self.month
         if self.day is None:
             day_start = 1
             day_end = calendar.monthrange(
                 self.year,  # type: ignore[arg-type]
                 month_end,
             )[1]
         else:
             day_start = day_end = self.day
-        return DateRange(Date(self.year, month_start, day_start), Date(self.year, month_end, day_end))
+        return DateRange(
+            Date(self.year, month_start, day_start), Date(self.year, month_end, day_end)
+        )
 
     def _compare(self, other: Any, comparator: Callable[[Any, Any], bool]) -> bool:
         if not isinstance(other, Date):
             return NotImplemented
         selfish = self
         if not selfish.comparable or not other.comparable:
             return NotImplemented
@@ -218,15 +240,17 @@
         return comparator(selfish, other)
 
     def __contains__(self, other: Any) -> bool:
         if isinstance(other, Date):
             return self == other
         if isinstance(other, DateRange):
             return self in other
-        raise TypeError('Expected to check a %s, but a %s was given' % (type(Datey), type(other)))
+        raise TypeError(
+            "Expected to check a %s, but a %s was given" % (type(Datey), type(other))
+        )
 
     def __lt__(self, other: Any) -> bool:
         return self._compare(other, operator.lt)
 
     def __le__(self, other: Any) -> bool:
         return self._compare(other, operator.le)
 
@@ -237,67 +261,68 @@
 
     def __ge__(self, other: Any) -> bool:
         return self._compare(other, operator.ge)
 
     def __gt__(self, other: Any) -> bool:
         return self._compare(other, operator.gt)
 
-    async def dump_linked_data(self, app: App, schemas_org: list[str] | None = None) -> DictDump[Dump]:
+    async def dump_linked_data(
+        self, app: App, schemas_org: list[str] | None = None
+    ) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
         if self.year:
-            dump['year'] = self.year
+            dump["year"] = self.year
         if self.month:
-            dump['month'] = self.month
+            dump["month"] = self.month
         if self.day:
-            dump['day'] = self.day
+            dump["day"] = self.day
         if self.comparable:
-            dump['iso8601'] = _dump_date_iso8601(self)
+            dump["iso8601"] = _dump_date_iso8601(self)
         return dump
 
     async def datey_dump_linked_data(
         self,
         dump: DictDump[Dump],
         start_schema_org: str,
         end_schema_org: str,
     ) -> None:
         if self.comparable:
             dump_context(dump, iso8601=(start_schema_org, end_schema_org))
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        schema['type'] = 'object'
-        schema['additionalProperties'] = False
+        schema["type"] = "object"
+        schema["additionalProperties"] = False
         add_json_ld(schema)
-        add_property(schema, 'year', {
-            'type': 'number'
-        }, False)
-        add_property(schema, 'month', {
-            'type': 'number'
-        }, False)
-        add_property(schema, 'day', {
-            'type': 'number'
-        }, False)
-        add_property(schema, 'iso8601', {
-            'type': 'string',
-            'pattern': '^\\d\\d\\d\\d-\\d\\d-\\d\\d$',
-            'description': 'An ISO 8601 date.'
-        }, False)
+        add_property(schema, "year", {"type": "number"}, False)
+        add_property(schema, "month", {"type": "number"}, False)
+        add_property(schema, "day", {"type": "number"}, False)
+        add_property(
+            schema,
+            "iso8601",
+            {
+                "type": "string",
+                "pattern": "^\\d\\d\\d\\d-\\d\\d-\\d\\d$",
+                "description": "An ISO 8601 date.",
+            },
+            False,
+        )
         return schema
 
 
 async def ref_date(root_schema: DictDump[Dump], app: App) -> DictDump[Dump]:
     """
     Reference the Date schema.
     """
-    definitions = dump_default(root_schema, 'definitions', dict)
-    if 'date' not in definitions:
-        definitions['date'] = await Date.linked_data_schema(app)
+    definitions = dump_default(root_schema, "definitions", dict)
+    if "date" not in definitions:
+        definitions["date"] = await Date.linked_data_schema(app)
     return {
-        '$ref': '#/definitions/date',
+        "$ref": "#/definitions/date",
     }
 
 
 @total_ordering
 class DateRange(LinkedDataDumpable):
     start: Date | None
     start_is_boundary: bool
@@ -313,19 +338,31 @@
     ):
         self.start = start
         self.start_is_boundary = start_is_boundary
         self.end = end
         self.end_is_boundary = end_is_boundary
 
     def __repr__(self) -> str:
-        return '%s.%s(%s, %s, start_is_boundary=%s, end_is_boundary=%s)' % (self.__class__.__module__, self.__class__.__name__, repr(self.start), repr(self.end), repr(self.start_is_boundary), repr(self.end_is_boundary))
+        return "%s.%s(%s, %s, start_is_boundary=%s, end_is_boundary=%s)" % (
+            self.__class__.__module__,
+            self.__class__.__name__,
+            repr(self.start),
+            repr(self.end),
+            repr(self.start_is_boundary),
+            repr(self.end_is_boundary),
+        )
 
     @property
     def comparable(self) -> bool:
-        return self.start is not None and self.start.comparable or self.end is not None and self.end.comparable
+        return (
+            self.start is not None
+            and self.start.comparable
+            or self.end is not None
+            and self.end.comparable
+        )
 
     def __contains__(self, other: Any) -> bool:
         if not self.comparable:
             return False
 
         if isinstance(other, Date):
             others = [other]
@@ -334,18 +371,23 @@
                 return False
             others = []
             if other.start is not None and other.start.comparable:
                 others.append(other.start)
             if other.end is not None and other.end.comparable:
                 others.append(other.end)
         else:
-            raise TypeError('Expected to check a %s, but a %s was given' % (type(Datey), type(other)))
+            raise TypeError(
+                "Expected to check a %s, but a %s was given"
+                % (type(Datey), type(other))
+            )
 
         if self.start is not None and self.end is not None:
-            if isinstance(other, DateRange) and (other.start is None or other.end is None):
+            if isinstance(other, DateRange) and (
+                other.start is None or other.end is None
+            ):
                 if other.start is None:
                     return self.start <= other.end or self.end <= other.end
                 if other.end is None:
                     return self.start >= other.start or self.end >= other.start
             for another in others:
                 if self.start <= another <= self.end:
                     return True
@@ -376,69 +418,159 @@
         self,
         app: App,
         start_schema_org: str | None = None,
         end_schema_org: str | None = None,
     ) -> DictDump[Dump]:
         dump: DictDump[Dump] = {}
         if self.start:
-            dump['start'] = await self.start.dump_linked_data(
+            dump["start"] = await self.start.dump_linked_data(
                 app,
                 [start_schema_org] if start_schema_org else None,
             )
         if self.end:
-            dump['end'] = await self.end.dump_linked_data(
+            dump["end"] = await self.end.dump_linked_data(
                 app,
                 [end_schema_org] if end_schema_org else None,
             )
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        schema['type'] = 'object'
-        schema['additionalProperties'] = False
-        add_property(schema, 'start', await ref_date(schema, app), False)
-        add_property(schema, 'end', await ref_date(schema, app), False)
+        schema["type"] = "object"
+        schema["additionalProperties"] = False
+        add_property(schema, "start", await ref_date(schema, app), False)
+        add_property(schema, "end", await ref_date(schema, app), False)
         return schema
 
     async def datey_dump_linked_data(
         self,
         dump: DictDump[Dump],
         start_schema_org: str,
         end_schema_org: str,
     ) -> None:
         if self.start and self.start.comparable:
-            start = dump_default(dump, 'start', dict)
+            start = dump_default(dump, "start", dict)
             dump_context(start, iso8601=start_schema_org)
         if self.end and self.end.comparable:
-            end = dump_default(dump, 'end', dict)
+            end = dump_default(dump, "end", dict)
             dump_context(end, iso8601=end_schema_org)
 
     def _get_comparable_date(self, date: Date | None) -> Date | None:
         if date and date.comparable:
             return date
         return None
 
     _LT_DATE_RANGE_COMPARATORS = {
-        (True, True, True, True): lambda self_start, self_end, other_start, other_end: self_start < other_start,
-        (True, True, True, False): lambda self_start, self_end, other_start, other_end: self_start <= other_start,
-        (True, True, False, True): lambda self_start, self_end, other_start, other_end: self_start < other_end or self_end <= other_end,
-        (True, True, False, False): lambda self_start, self_end, other_start, other_end: NotImplemented,
-        (True, False, True, True): lambda self_start, self_end, other_start, other_end: self_start < other_start,
-        (True, False, True, False): lambda self_start, self_end, other_start, other_end: self_start < other_start,
-        (True, False, False, True): lambda self_start, self_end, other_start, other_end: self_start < other_end,
-        (True, False, False, False): lambda self_start, self_end, other_start, other_end: NotImplemented,
-        (False, True, True, True): lambda self_start, self_end, other_start, other_end: self_end <= other_start,
-        (False, True, True, False): lambda self_start, self_end, other_start, other_end: self_end <= other_start,
-        (False, True, False, True): lambda self_start, self_end, other_start, other_end: self_end < other_end,
-        (False, True, False, False): lambda self_start, self_end, other_start, other_end: NotImplemented,
-        (False, False, True, True): lambda self_start, self_end, other_start, other_end: NotImplemented,
-        (False, False, True, False): lambda self_start, self_end, other_start, other_end: NotImplemented,
-        (False, False, False, True): lambda self_start, self_end, other_start, other_end: NotImplemented,
-        (False, False, False, False): lambda self_start, self_end, other_start, other_end: NotImplemented,
+        (
+            True,
+            True,
+            True,
+            True,
+        ): lambda self_start, self_end, other_start, other_end: self_start
+        < other_start,
+        (
+            True,
+            True,
+            True,
+            False,
+        ): lambda self_start, self_end, other_start, other_end: self_start
+        <= other_start,
+        (
+            True,
+            True,
+            False,
+            True,
+        ): lambda self_start, self_end, other_start, other_end: self_start
+        < other_end
+        or self_end <= other_end,
+        (
+            True,
+            True,
+            False,
+            False,
+        ): lambda self_start, self_end, other_start, other_end: NotImplemented,
+        (
+            True,
+            False,
+            True,
+            True,
+        ): lambda self_start, self_end, other_start, other_end: self_start
+        < other_start,
+        (
+            True,
+            False,
+            True,
+            False,
+        ): lambda self_start, self_end, other_start, other_end: self_start
+        < other_start,
+        (
+            True,
+            False,
+            False,
+            True,
+        ): lambda self_start, self_end, other_start, other_end: self_start
+        < other_end,
+        (
+            True,
+            False,
+            False,
+            False,
+        ): lambda self_start, self_end, other_start, other_end: NotImplemented,
+        (
+            False,
+            True,
+            True,
+            True,
+        ): lambda self_start, self_end, other_start, other_end: self_end
+        <= other_start,
+        (
+            False,
+            True,
+            True,
+            False,
+        ): lambda self_start, self_end, other_start, other_end: self_end
+        <= other_start,
+        (
+            False,
+            True,
+            False,
+            True,
+        ): lambda self_start, self_end, other_start, other_end: self_end
+        < other_end,
+        (
+            False,
+            True,
+            False,
+            False,
+        ): lambda self_start, self_end, other_start, other_end: NotImplemented,
+        (
+            False,
+            False,
+            True,
+            True,
+        ): lambda self_start, self_end, other_start, other_end: NotImplemented,
+        (
+            False,
+            False,
+            True,
+            False,
+        ): lambda self_start, self_end, other_start, other_end: NotImplemented,
+        (
+            False,
+            False,
+            False,
+            True,
+        ): lambda self_start, self_end, other_start, other_end: NotImplemented,
+        (
+            False,
+            False,
+            False,
+            False,
+        ): lambda self_start, self_end, other_start, other_end: NotImplemented,
     }
 
     _LT_DATE_COMPARATORS = {
         (True, True): lambda self_start, self_end, other: self_start < other,
         (True, False): lambda self_start, self_end, other: self_start < other,
         (False, True): lambda self_start, self_end, other: self_end <= other,
         (False, False): lambda self_start, self_end, other: NotImplemented,
@@ -453,64 +585,73 @@
         signature = (
             self_start is not None,
             self_end is not None,
         )
         if isinstance(other, DateRange):
             other_start = self._get_comparable_date(other.start)
             other_end = self._get_comparable_date(other.end)
-            return self._LT_DATE_RANGE_COMPARATORS[(
-                *signature,
-                other_start is not None,
-                other_end is not None,
-            )](self_start, self_end, other_start, other_end)
+            return self._LT_DATE_RANGE_COMPARATORS[
+                (
+                    *signature,
+                    other_start is not None,
+                    other_end is not None,
+                )
+            ](self_start, self_end, other_start, other_end)
         else:
             return self._LT_DATE_COMPARATORS[signature](self_start, self_end, other)
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Date):
             return False
 
         if not isinstance(other, DateRange):
             return NotImplemented
-        return (self.start, self.end, self.start_is_boundary, self.end_is_boundary) == (other.start, other.end, other.start_is_boundary, other.end_is_boundary)
+        return (self.start, self.end, self.start_is_boundary, self.end_is_boundary) == (
+            other.start,
+            other.end,
+            other.start_is_boundary,
+            other.end_is_boundary,
+        )
 
 
 async def ref_date_range(root_schema: DictDump[Dump], app: App) -> DictDump[Dump]:
     """
     Reference the DateRange schema.
     """
-    definitions = dump_default(root_schema, 'definitions', dict)
-    if 'dateRange' not in definitions:
-        definitions['dateRange'] = await DateRange.linked_data_schema(app)
+    definitions = dump_default(root_schema, "definitions", dict)
+    if "dateRange" not in definitions:
+        definitions["dateRange"] = await DateRange.linked_data_schema(app)
     return {
-        '$ref': '#/definitions/dateRange',
+        "$ref": "#/definitions/dateRange",
     }
 
 
 async def ref_datey(root_schema: DictDump[Dump], app: App) -> DictDump[Dump]:
     """
     Reference the Datey schema.
     """
-    definitions = dump_default(root_schema, 'definitions', dict)
-    if 'datey' not in definitions:
-        definitions['datey'] = {
-            'oneOf': [
+    definitions = dump_default(root_schema, "definitions", dict)
+    if "datey" not in definitions:
+        definitions["datey"] = {
+            "oneOf": [
                 await ref_date(root_schema, app),
                 await ref_date_range(root_schema, app),
             ]
         }
     return {
-        '$ref': '#/definitions/datey',
+        "$ref": "#/definitions/datey",
     }
 
 
 Datey: TypeAlias = Date | DateRange
 DatePartsFormatters: TypeAlias = Mapping[tuple[bool, bool, bool], str]
 DateFormatters: TypeAlias = Mapping[tuple[bool | None], str]
-DateRangeFormatters: TypeAlias = Mapping[tuple[bool | None, bool | None, bool | None, bool | None], str]
+DateRangeFormatters: TypeAlias = Mapping[
+    tuple[bool | None, bool | None, bool | None, bool | None], str
+]
 
 
 class Localizer:
     def __init__(self, locale: str, translations: gettext.NullTranslations):
         self._locale = locale
         self._locale_data = get_data(locale)
         self._translations = translations
@@ -530,66 +671,102 @@
 
     def ngettext(self, message_singular: str, message_plural: str, n: int) -> str:
         return self._translations.ngettext(message_singular, message_plural, n)
 
     def pgettext(self, context: str, message: str) -> str:
         return self._translations.pgettext(context, message)
 
-    def npgettext(self, context: str, message_singular: str, message_plural: str, n: int) -> str:
-        return self._translations.npgettext(context, message_singular, message_plural, n)
+    def npgettext(
+        self, context: str, message_singular: str, message_plural: str, n: int
+    ) -> str:
+        return self._translations.npgettext(
+            context, message_singular, message_plural, n
+        )
 
     @property
     def _date_parts_formatters(self) -> DatePartsFormatters:
         if self.__date_parts_formatters is None:
             self.__date_parts_formatters = {
-                (True, True, True): self._('MMMM d, y'),
-                (True, True, False): self._('MMMM, y'),
-                (True, False, False): self._('y'),
-                (False, True, True): self._('MMMM d'),
-                (False, True, False): self._('MMMM'),
+                (True, True, True): self._("MMMM d, y"),
+                (True, True, False): self._("MMMM, y"),
+                (True, False, False): self._("y"),
+                (False, True, True): self._("MMMM d"),
+                (False, True, False): self._("MMMM"),
             }
         return self.__date_parts_formatters
 
     @property
     def _date_formatters(self) -> DateFormatters:
         if self.__date_formatters is None:
             self.__date_formatters = {
-                (True,): self._('around {date}'),
-                (False,): self._('{date}'),
+                (True,): self._("around {date}"),
+                (False,): self._("{date}"),
             }
         return self.__date_formatters
 
     @property
     def _date_range_formatters(self) -> DateRangeFormatters:
         if self.__date_range_formatters is None:
             self.__date_range_formatters = {
-                (False, False, False, False): self._('from {start_date} until {end_date}'),
-                (False, False, False, True): self._('from {start_date} until sometime before {end_date}'),
-                (False, False, True, False): self._('from {start_date} until around {end_date}'),
-                (False, False, True, True): self._('from {start_date} until sometime before around {end_date}'),
-                (False, True, False, False): self._('from sometime after {start_date} until {end_date}'),
-                (False, True, False, True): self._('sometime between {start_date} and {end_date}'),
-                (False, True, True, False): self._('from sometime after {start_date} until around {end_date}'),
-                (False, True, True, True): self._('sometime between {start_date} and around {end_date}'),
-                (True, False, False, False): self._('from around {start_date} until {end_date}'),
-                (True, False, False, True): self._('from around {start_date} until sometime before {end_date}'),
-                (True, False, True, False): self._('from around {start_date} until around {end_date}'),
-                (True, False, True, True): self._('from around {start_date} until sometime before around {end_date}'),
-                (True, True, False, False): self._('from sometime after around {start_date} until {end_date}'),
-                (True, True, False, True): self._('sometime between around {start_date} and {end_date}'),
-                (True, True, True, False): self._('from sometime after around {start_date} until around {end_date}'),
-                (True, True, True, True): self._('sometime between around {start_date} and around {end_date}'),
-                (False, False, None, None): self._('from {start_date}'),
-                (False, True, None, None): self._('sometime after {start_date}'),
-                (True, False, None, None): self._('from around {start_date}'),
-                (True, True, None, None): self._('sometime after around {start_date}'),
-                (None, None, False, False): self._('until {end_date}'),
-                (None, None, False, True): self. _('sometime before {end_date}'),
-                (None, None, True, False): self._('until around {end_date}'),
-                (None, None, True, True): self._('sometime before around {end_date}'),
+                (False, False, False, False): self._(
+                    "from {start_date} until {end_date}"
+                ),
+                (False, False, False, True): self._(
+                    "from {start_date} until sometime before {end_date}"
+                ),
+                (False, False, True, False): self._(
+                    "from {start_date} until around {end_date}"
+                ),
+                (False, False, True, True): self._(
+                    "from {start_date} until sometime before around {end_date}"
+                ),
+                (False, True, False, False): self._(
+                    "from sometime after {start_date} until {end_date}"
+                ),
+                (False, True, False, True): self._(
+                    "sometime between {start_date} and {end_date}"
+                ),
+                (False, True, True, False): self._(
+                    "from sometime after {start_date} until around {end_date}"
+                ),
+                (False, True, True, True): self._(
+                    "sometime between {start_date} and around {end_date}"
+                ),
+                (True, False, False, False): self._(
+                    "from around {start_date} until {end_date}"
+                ),
+                (True, False, False, True): self._(
+                    "from around {start_date} until sometime before {end_date}"
+                ),
+                (True, False, True, False): self._(
+                    "from around {start_date} until around {end_date}"
+                ),
+                (True, False, True, True): self._(
+                    "from around {start_date} until sometime before around {end_date}"
+                ),
+                (True, True, False, False): self._(
+                    "from sometime after around {start_date} until {end_date}"
+                ),
+                (True, True, False, True): self._(
+                    "sometime between around {start_date} and {end_date}"
+                ),
+                (True, True, True, False): self._(
+                    "from sometime after around {start_date} until around {end_date}"
+                ),
+                (True, True, True, True): self._(
+                    "sometime between around {start_date} and around {end_date}"
+                ),
+                (False, False, None, None): self._("from {start_date}"),
+                (False, True, None, None): self._("sometime after {start_date}"),
+                (True, False, None, None): self._("from around {start_date}"),
+                (True, True, None, None): self._("sometime after around {start_date}"),
+                (None, None, False, False): self._("until {end_date}"),
+                (None, None, False, True): self._("sometime before {end_date}"),
+                (None, None, True, False): self._("until around {end_date}"),
+                (None, None, True, True): self._("sometime before around {end_date}"),
             }
         return self.__date_range_formatters
 
     def format_datey(self, date: Datey) -> str:
         """
         Format a datey value into a human-readable string.
         """
@@ -599,162 +776,186 @@
 
     def format_date(self, date: Date) -> str:
         try:
             return self._date_formatters[(date.fuzzy,)].format(
                 date=self._format_date_parts(date),
             )
         except IncompleteDateError:
-            return self._('unknown date')
+            return self._("unknown date")
 
     def _format_date_parts(self, date: Date | None) -> str:
         if date is None:
-            raise IncompleteDateError('This date is None.')
+            raise IncompleteDateError("This date is None.")
         try:
-            date_parts_format = self._date_parts_formatters[tuple(
-                map(lambda x: x is not None, date.parts),  # type: ignore[index]
-            )]
+            date_parts_format = self._date_parts_formatters[
+                tuple(
+                    map(lambda x: x is not None, date.parts),  # type: ignore[index]
+                )
+            ]
         except KeyError:
-            raise IncompleteDateError('This date does not have enough parts to be rendered.')
+            raise IncompleteDateError(
+                "This date does not have enough parts to be rendered."
+            )
         parts = map(lambda x: 1 if x is None else x, date.parts)
-        return dates.format_date(datetime.date(*parts), date_parts_format, self._locale_data)
+        return dates.format_date(
+            datetime.date(*parts), date_parts_format, self._locale_data
+        )
 
     def format_date_range(self, date_range: DateRange) -> str:
-        formatter_configuration: tuple[bool | None, bool | None, bool | None, bool | None] = (None, None, None, None)
+        formatter_configuration: tuple[
+            bool | None, bool | None, bool | None, bool | None
+        ] = (None, None, None, None)
         formatter_arguments = {}
 
         with suppress(IncompleteDateError):
-            formatter_arguments['start_date'] = self._format_date_parts(date_range.start)
+            formatter_arguments["start_date"] = self._format_date_parts(
+                date_range.start
+            )
             formatter_configuration = (
                 None if date_range.start is None else date_range.start.fuzzy,
                 date_range.start_is_boundary,
                 formatter_configuration[2],
                 formatter_configuration[3],
             )
 
         with suppress(IncompleteDateError):
-            formatter_arguments['end_date'] = self._format_date_parts(date_range.end)
+            formatter_arguments["end_date"] = self._format_date_parts(date_range.end)
             formatter_configuration = (
                 formatter_configuration[0],
                 formatter_configuration[1],
                 None if date_range.end is None else date_range.end.fuzzy,
                 date_range.end_is_boundary,
             )
 
         if not formatter_arguments:
-            raise IncompleteDateError('This date range does not have enough parts to be rendered.')
+            raise IncompleteDateError(
+                "This date range does not have enough parts to be rendered."
+            )
 
-        return self._date_range_formatters[formatter_configuration].format(**formatter_arguments)
+        return self._date_range_formatters[formatter_configuration].format(
+            **formatter_arguments
+        )
 
 
 DEFAULT_LOCALIZER = Localizer(DEFAULT_LOCALE, gettext.NullTranslations())
 
 
 class LocalizerRepository:
     def __init__(self, assets: FileSystem):
         self._assets = assets
         self._localizers: dict[str, Localizer] = {}
-        self._locks: dict[str, threading.Lock] = defaultdict(threading.Lock)
+        self._locks: Mapping[str, _Lock] = defaultdict(AsynchronizedLock.threading)
+        self._locales: set[str] | None = None
 
     @property
     def locales(self) -> Iterator[str]:
-        yield DEFAULT_LOCALE
-        for assets_directory_path, __ in reversed(self._assets.paths):
-            for po_file_path in glob.glob(str(assets_directory_path / 'locale' / '*' / 'betty.po')):
-                yield Path(po_file_path).parent.name
+        if self._locales is None:
+            self._locales = set()
+            self._locales.add(DEFAULT_LOCALE)
+            for assets_directory_path, __ in reversed(self._assets.paths):
+                for po_file_path in glob.glob(
+                    str(assets_directory_path / "locale" / "*" / "betty.po")
+                ):
+                    self._locales.add(Path(po_file_path).parent.name)
+        yield from self._locales
 
     async def get(self, locale: Localey) -> Localizer:
         locale = to_locale(locale)
-        try:
-            return self._localizers[locale]
-        except KeyError:
-            return await self._build_translation(locale)
+        async with self._locks[locale]:
+            try:
+                return self._localizers[locale]
+            except KeyError:
+                return await self._build_translation(locale)
 
+    @deprecated(
+        "This method is deprecated as of Betty 0.3.4, and will be removed in Betty 0.4.x. Instead, use `LocalizerRepository.get()`."
+    )
     def __getitem__(self, locale: Localey) -> Localizer:
-        locale = to_locale(locale)
-        try:
-            return self._localizers[locale]
-        except KeyError:
-            return wait_to_thread(self._build_translation(locale))
+        return wait_to_thread(self.get(locale))
 
     async def get_negotiated(self, *preferred_locales: str) -> Localizer:
         preferred_locales = (*preferred_locales, DEFAULT_LOCALE)
         negotiated_locale = negotiate_locale(
             preferred_locales,
-            [
-                str(get_data(locale))
-                for locale
-                in self.locales
-            ],
+            [str(get_data(locale)) for locale in self.locales],
         )
         return await self.get(negotiated_locale or DEFAULT_LOCALE)
 
     async def _build_translation(self, locale: str) -> Localizer:
         translations = gettext.NullTranslations()
         for assets_directory_path, __ in reversed(self._assets.paths):
-            opened_translations = await asyncio.to_thread(self._open_translations, locale, assets_directory_path)
+            opened_translations = await self._open_translations(
+                locale, assets_directory_path
+            )
             if opened_translations:
                 opened_translations.add_fallback(translations)
                 translations = opened_translations
         self._localizers[locale] = Localizer(locale, translations)
         return self._localizers[locale]
 
-    def _open_translations(self, locale: str, assets_directory_path: Path) -> gettext.GNUTranslations | None:
-        po_file_path = assets_directory_path / 'locale' / locale / 'betty.po'
+    async def _open_translations(
+        self, locale: str, assets_directory_path: Path
+    ) -> gettext.GNUTranslations | None:
+        po_file_path = assets_directory_path / "locale" / locale / "betty.po"
         try:
-            translation_version = hashfile(po_file_path)
+            translation_version = await hashid_file_meta(po_file_path)
         except FileNotFoundError:
             return None
-        cache_directory_path = fs.CACHE_DIRECTORY_PATH / 'locale' / translation_version
-        mo_file_path = cache_directory_path / 'betty.mo'
-
-        with self._locks[locale]:
-            with suppress(FileNotFoundError):
-                with open(mo_file_path, 'rb') as f:
-                    return gettext.GNUTranslations(f)
-
-            cache_directory_path.mkdir(exist_ok=True, parents=True)
+        cache_directory_path = fs.CACHE_DIRECTORY_PATH / "locale" / translation_version
+        mo_file_path = cache_directory_path / "betty.mo"
 
-            with redirect_stdout(StringIO()):
-                CommandLineInterface().run([
-                    '',
-                    'compile',
-                    '-i',
-                    str(po_file_path),
-                    '-o',
-                    str(mo_file_path),
-                    '-l',
-                    str(get_data(locale)),
-                    '-D',
-                    'betty',
-                ])
-        with open(mo_file_path, 'rb') as f:
+        with suppress(FileNotFoundError):
+            with open(mo_file_path, "rb") as f:
+                return gettext.GNUTranslations(f)
+
+        cache_directory_path.mkdir(exist_ok=True, parents=True)
+
+        await run_babel(
+            "",
+            "compile",
+            "-i",
+            str(po_file_path),
+            "-o",
+            str(mo_file_path),
+            "-l",
+            str(get_data(locale)),
+            "-D",
+            "betty",
+        )
+        with open(mo_file_path, "rb") as f:
             return gettext.GNUTranslations(f)
 
     async def coverage(self, locale: Localey) -> tuple[int, int]:
-        translatables = {translatable async for translatable in self._get_translatables()}
+        translatables = {
+            translatable async for translatable in self._get_translatables()
+        }
         locale = to_locale(locale)
         if locale == DEFAULT_LOCALE:
             return len(translatables), len(translatables)
-        translations = {translation async for translation in self._get_translations(locale)}
+        translations = {
+            translation async for translation in self._get_translations(locale)
+        }
         return len(translations), len(translatables)
 
     async def _get_translatables(self) -> AsyncIterator[str]:
         for assets_directory_path, __ in self._assets.paths:
             with suppress(FileNotFoundError):
-                async with aiofiles.open(assets_directory_path / 'betty.pot') as pot_data_f:
+                async with aiofiles.open(
+                    assets_directory_path / "betty.pot"
+                ) as pot_data_f:
                     pot_data = await pot_data_f.read()
                     for entry in pofile(pot_data):
                         yield entry.msgid_with_context
 
     async def _get_translations(self, locale: str) -> AsyncIterator[str]:
         for assets_directory_path, __ in reversed(self._assets.paths):
             with suppress(FileNotFoundError):
                 async with aiofiles.open(
-                    assets_directory_path / 'locale' / locale / 'betty.po',
-                    encoding='utf-8',
+                    assets_directory_path / "locale" / locale / "betty.po",
+                    encoding="utf-8",
                 ) as p_data_f:
                     po_data = await p_data_f.read()
                     for entry in pofile(po_data):
                         if entry.translated():
                             yield entry.msgid_with_context
 
 
@@ -768,19 +969,20 @@
             f'{type(self)} ("{localized}") SHOULD NOT be cast to a string. Instead, call {type(self)}.localize() to ensure it is always formatted in the desired locale.',
             stacklevel=2,
         )
         return localized
 
 
 class Str(Localizable):
-    def _localize_format_kwargs(self, localizer: Localizer, **format_kwargs: str | Localizable) -> dict[str, str]:
+    def _localize_format_kwargs(
+        self, localizer: Localizer, **format_kwargs: str | Localizable
+    ) -> dict[str, str]:
         return {
             key: value.localize(localizer) if isinstance(value, Localizable) else value
-            for key, value
-            in format_kwargs.items()
+            for key, value in format_kwargs.items()
         }
 
     @classmethod
     def plain(cls, plain: Any, **format_kwargs: str | Localizable) -> Str:
         return _PlainStr(str(plain), **format_kwargs)
 
     @classmethod
@@ -789,185 +991,234 @@
 
     @classmethod
     def _(cls, message: str, **format_kwargs: str | Localizable) -> Str:
         return cls.gettext(message, **format_kwargs)
 
     @classmethod
     def gettext(cls, message: str, **format_kwargs: str | Localizable) -> Str:
-        return _GettextStr('gettext', message, **format_kwargs)
+        return _GettextStr("gettext", message, **format_kwargs)
 
     @classmethod
-    def ngettext(cls, message_singular: str, message_plural: str, n: int, **format_kwargs: str | Localizable) -> Str:
-        return _GettextStr('ngettext', message_singular, message_plural, n, **format_kwargs)
+    def ngettext(
+        cls,
+        message_singular: str,
+        message_plural: str,
+        n: int,
+        **format_kwargs: str | Localizable,
+    ) -> Str:
+        return _GettextStr(
+            "ngettext", message_singular, message_plural, n, **format_kwargs
+        )
 
     @classmethod
-    def pgettext(cls, context: str, message: str, **format_kwargs: str | Localizable) -> Str:
-        return _GettextStr('pgettext', context, message, **format_kwargs)
+    def pgettext(
+        cls, context: str, message: str, **format_kwargs: str | Localizable
+    ) -> Str:
+        return _GettextStr("pgettext", context, message, **format_kwargs)
 
     @classmethod
-    def npgettext(cls, context: str, message_singular: str, message_plural: str, n: int, **format_kwargs: str | Localizable) -> Str:
-        return _GettextStr('npgettext', context, message_singular, message_plural, n, **format_kwargs)
+    def npgettext(
+        cls,
+        context: str,
+        message_singular: str,
+        message_plural: str,
+        n: int,
+        **format_kwargs: str | Localizable,
+    ) -> Str:
+        return _GettextStr(
+            "npgettext", context, message_singular, message_plural, n, **format_kwargs
+        )
 
 
 class _PlainStr(Str):
     def __init__(self, plain: str, **format_kwargs: str | Localizable):
         self._plain = plain
         self._format_kwargs = format_kwargs
 
     def localize(self, localizer: Localizer) -> str:
-        return self._plain.format(**self._localize_format_kwargs(localizer, **self._format_kwargs))
+        return self._plain.format(
+            **self._localize_format_kwargs(localizer, **self._format_kwargs)
+        )
 
 
 class _CallStr(Str):
     def __init__(self, call: Callable[[Localizer], str]):
         self._call = call
 
     def localize(self, localizer: Localizer) -> str:
         return self._call(localizer)
 
 
 class _GettextStr(Str):
-    def __init__(self, gettext_method_name: str, *gettext_args: Any, **format_kwargs: str | Localizable) -> None:
+    def __init__(
+        self,
+        gettext_method_name: str,
+        *gettext_args: Any,
+        **format_kwargs: str | Localizable,
+    ) -> None:
         self._gettext_method_name = gettext_method_name
         self._gettext_args = gettext_args
         self._format_kwargs = format_kwargs
 
     def localize(self, localizer: Localizer) -> str:
-        return cast(str, getattr(localizer, self._gettext_method_name)(*self._gettext_args)).format(**self._localize_format_kwargs(localizer, **self._format_kwargs))
+        return cast(
+            str, getattr(localizer, self._gettext_method_name)(*self._gettext_args)
+        ).format(**self._localize_format_kwargs(localizer, **self._format_kwargs))
 
 
-def negotiate_locale(preferred_locales: Localey | Sequence[Localey], available_locales: Sequence[Localey]) -> Locale | None:
+def negotiate_locale(
+    preferred_locales: Localey | Sequence[Localey], available_locales: Sequence[Localey]
+) -> Locale | None:
     """
     Negotiate the preferred locale from a sequence.
     """
     if isinstance(preferred_locales, (str, Locale)):
         preferred_locales = [preferred_locales]
     return _negotiate_locale(
-        [
-            to_babel_identifier(locale)
-            for locale
-            in preferred_locales
-        ],
-        {
-            to_babel_identifier(locale)
-            for locale
-            in available_locales
-        },
+        [to_babel_identifier(locale) for locale in preferred_locales],
+        {to_babel_identifier(locale) for locale in available_locales},
         False,
     )
 
 
-def _negotiate_locale(preferred_locale_babel_identifiers: Sequence[str], available_locale_babel_identifiers: set[str], root: bool) -> Locale | None:
-    negotiated_locale = babel.negotiate_locale(preferred_locale_babel_identifiers, available_locale_babel_identifiers)
+def _negotiate_locale(
+    preferred_locale_babel_identifiers: Sequence[str],
+    available_locale_babel_identifiers: set[str],
+    root: bool,
+) -> Locale | None:
+    negotiated_locale = babel.negotiate_locale(
+        preferred_locale_babel_identifiers, available_locale_babel_identifiers
+    )
     if negotiated_locale is not None:
         return Locale.parse(negotiated_locale)
     if not root:
         return _negotiate_locale(
             [
-                babel_identifier.split('_')[0] if '_' in babel_identifier else babel_identifier
-                for babel_identifier
-                in preferred_locale_babel_identifiers
+                (
+                    babel_identifier.split("_")[0]
+                    if "_" in babel_identifier
+                    else babel_identifier
+                )
+                for babel_identifier in preferred_locale_babel_identifiers
             ],
             available_locale_babel_identifiers,
             True,
         )
     return None
 
 
-def negotiate_localizeds(preferred_locales: Localey | Sequence[Localey], localizeds: Sequence[Localized]) -> Localized | None:
+def negotiate_localizeds(
+    preferred_locales: Localey | Sequence[Localey], localizeds: Sequence[Localized]
+) -> Localized | None:
     """
     Negotiate the preferred localized value from a sequence.
     """
     negotiated_locale_data = negotiate_locale(
         preferred_locales,
-        [
-            localized.locale
-            for localized
-            in localizeds
-            if localized.locale is not None
-        ],
+        [localized.locale for localized in localizeds if localized.locale is not None],
     )
     if negotiated_locale_data is not None:
         negotiated_locale = to_locale(negotiated_locale_data)
         for localized in localizeds:
             if localized.locale == negotiated_locale:
                 return localized
     for localized in localizeds:
         if localized.locale is None:
             return localized
     with suppress(IndexError):
         return localizeds[0]
     return None
 
 
+def _run_babel(*args: str) -> None:
+    with redirect_stderr(StringIO()):
+        CommandLineInterface().run(list(args))
+
+
+async def run_babel(*args: str) -> None:
+    """
+    Run a Babel Command Line Interface (CLI) command.
+    """
+    await to_thread(_run_babel, *args)
+
+
 async def init_translation(locale: str) -> None:
     """
     Initialize a new translation.
     """
-    po_file_path = _LOCALE_DIRECTORY_PATH / locale / 'betty.po'
+    po_file_path = _LOCALE_DIRECTORY_PATH / locale / "betty.po"
     with redirect_stdout(StringIO()):
         if await exists(po_file_path):
-            logging.getLogger(__name__).info(f'Translations for {locale} already exist at {po_file_path}.')
+            logging.getLogger(__name__).info(
+                f"Translations for {locale} already exist at {po_file_path}."
+            )
             return
 
         locale_data = get_data(locale)
-        CommandLineInterface().run([
-            '',
-            'init',
-            '--no-wrap',
-            '-i',
-            str(fs.ASSETS_DIRECTORY_PATH / 'betty.pot'),
-            '-o',
+        await run_babel(
+            "",
+            "init",
+            "--no-wrap",
+            "-i",
+            str(fs.ASSETS_DIRECTORY_PATH / "betty.pot"),
+            "-o",
             str(po_file_path),
-            '-l',
+            "-l",
             str(locale_data),
-            '-D',
-            'betty',
-        ])
-        logging.getLogger(__name__).info(f'Translations for {locale} initialized at {po_file_path}.')
+            "-D",
+            "betty",
+        )
+        logging.getLogger(__name__).info(
+            f"Translations for {locale} initialized at {po_file_path}."
+        )
 
 
-async def update_translations(_output_assets_directory_path: Path = fs.ASSETS_DIRECTORY_PATH) -> None:
+async def update_translations(
+    _output_assets_directory_path: Path = fs.ASSETS_DIRECTORY_PATH,
+) -> None:
     """
     Update all existing translations based on changes in translatable strings.
     """
-    source_paths = glob.glob('betty/*')
+    source_paths = glob.glob("betty/*")
     # Remove the tests directory from the extraction,
     # or we'll be seeing some unusual additions to the translations.
-    source_paths.remove(str(Path('betty') / 'tests'))
-    pot_file_path = _output_assets_directory_path / 'betty.pot'
-    with redirect_stdout(StringIO()):
-        with chdir(ROOT_DIRECTORY_PATH):
-            CommandLineInterface().run([
-                '',
-                'extract',
-                '--no-location',
-                '--no-wrap',
-                '--sort-output',
-                '-F',
-                'babel.ini',
-                '-o',
-                str(pot_file_path),
-                '--project',
-                'Betty',
-                '--copyright-holder',
-                'Bart Feenstra & contributors',
-                *source_paths,
-            ])
-            for po_file_path_str in glob.glob('betty/assets/locale/*/betty.po'):
-                po_file_path = (_output_assets_directory_path / (ROOT_DIRECTORY_PATH / po_file_path_str).relative_to(fs.ASSETS_DIRECTORY_PATH)).resolve()
-                await makedirs(po_file_path.parent, exist_ok=True)
-                po_file_path.touch()
-                locale = po_file_path.parent.name
-                locale_data = get_data(locale)
-                CommandLineInterface().run([
-                    '',
-                    'update',
-                    '-i',
-                    str(pot_file_path),
-                    '-o',
-                    str(po_file_path),
-                    '-l',
-                    str(locale_data),
-                    '-D',
-                    'betty',
-                ])
+    source_paths.remove(str(Path("betty") / "tests"))
+    pot_file_path = _output_assets_directory_path / "betty.pot"
+    await run_babel(
+        "",
+        "extract",
+        "--no-location",
+        "--no-wrap",
+        "--sort-output",
+        "-F",
+        "babel.ini",
+        "-o",
+        str(pot_file_path),
+        "--project",
+        "Betty",
+        "--copyright-holder",
+        "Bart Feenstra & contributors",
+        *(str(ROOT_DIRECTORY_PATH / source_path) for source_path in source_paths),
+    )
+    for po_file_path_str in glob.glob("betty/assets/locale/*/betty.po"):
+        po_file_path = (
+            _output_assets_directory_path
+            / (ROOT_DIRECTORY_PATH / po_file_path_str).relative_to(
+                fs.ASSETS_DIRECTORY_PATH
+            )
+        ).resolve()
+        await makedirs(po_file_path.parent, exist_ok=True)
+        po_file_path.touch()
+        locale = po_file_path.parent.name
+        locale_data = get_data(locale)
+        await run_babel(
+            "",
+            "update",
+            "-i",
+            str(pot_file_path),
+            "-o",
+            str(po_file_path),
+            "-l",
+            str(locale_data),
+            "-D",
+            "betty",
+        )
```

### Comparing `betty-0.3.3/betty/logging.py` & `betty-0.3.4/betty/logging.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 """
 Provide logging utilities.
 """
+
 import sys
-from logging import CRITICAL, ERROR, WARNING, INFO, DEBUG, NOTSET, StreamHandler, LogRecord
+from logging import (
+    CRITICAL,
+    ERROR,
+    WARNING,
+    INFO,
+    DEBUG,
+    NOTSET,
+    StreamHandler,
+    LogRecord,
+)
 
 
 class CliHandler(
     StreamHandler,  # type: ignore[type-arg]
 ):
     COLOR_LEVELS = {
         CRITICAL: 91,
@@ -24,8 +34,8 @@
         s = StreamHandler.format(self, record)
         for level, color in self.COLOR_LEVELS.items():
             if record.levelno >= level:
                 return self._color(s, color)
         return self._color(s, self.COLOR_LEVELS[NOTSET])
 
     def _color(self, s: str, color: int) -> str:
-        return '\033[%dm%s\033[0m' % (color, s)
+        return "\033[%dm%s\033[0m" % (color, s)
```

### Comparing `betty-0.3.3/betty/media_type.py` & `betty-0.3.4/betty/media_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 """
 Provide `media type <https://en.wikipedia.org/wiki/Media_type>`_ handling utilities.
 """
+
 from __future__ import annotations
 
 from email.message import EmailMessage
 from typing import Any
 
 
 class InvalidMediaType(ValueError):
     pass
 
 
 class MediaType:
     def __init__(self, media_type: str):
         self._str = media_type
         message = EmailMessage()
-        message['Content-Type'] = media_type
+        message["Content-Type"] = media_type
         type_part = message.get_content_type()
         # EmailMessage.get_content_type() always returns a type, and will fall back to alternatives if the header is
         # invalid.
         if not media_type.startswith(type_part):
             raise InvalidMediaType(f'"{media_type}" is not a valid media type.')
-        self._parameters: dict[str, str] = dict(message['Content-Type'].params)
-        self._type, self._subtype = type_part.split('/')
+        self._parameters: dict[str, str] = dict(message["Content-Type"].params)
+        self._type, self._subtype = type_part.split("/")
         if not self._subtype:
-            raise InvalidMediaType('The subtype must not be empty.')
+            raise InvalidMediaType("The subtype must not be empty.")
 
     @property
     def type(self) -> str:
         return self._type
 
     @property
     def subtype(self) -> str:
         return self._subtype
 
     @property
     def subtypes(self) -> list[str]:
-        return self._subtype.split('+')[0].split('.')
+        return self._subtype.split("+")[0].split(".")
 
     @property
     def suffix(self) -> str | None:
-        if '+' not in self._subtype:
+        if "+" not in self._subtype:
             return None
 
-        return self._subtype.split('+')[-1]
+        return self._subtype.split("+")[-1]
 
     @property
     def parameters(self) -> dict[str, str]:
         return self._parameters
 
     def __str__(self) -> str:
         return self._str
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, MediaType):
             return NotImplemented
-        return (self.type, self.subtype, self.parameters) == (other.type, other.subtype, other.parameters)
+        return (self.type, self.subtype, self.parameters) == (
+            other.type,
+            other.subtype,
+            other.parameters,
+        )
```

### Comparing `betty-0.3.3/betty/model/__init__.py` & `betty-0.3.4/betty/model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,42 @@
 
 import builtins
 import functools
 import weakref
 from collections import defaultdict
 from contextlib import contextmanager
 from reprlib import recursive_repr
-from typing import TypeVar, Generic, Iterable, Any, overload, cast, Iterator, Callable, Self, TypeAlias, TYPE_CHECKING
+from typing import (
+    TypeVar,
+    Generic,
+    Iterable,
+    Any,
+    overload,
+    cast,
+    Iterator,
+    Callable,
+    Self,
+    TypeAlias,
+    TYPE_CHECKING,
+)
 from uuid import uuid4
 
 from betty.classtools import repr_instance
 from betty.importlib import import_any, fully_qualified_type_name
 from betty.json.linked_data import LinkedDataDumpable, add_json_ld
 from betty.json.schema import ref_json_schema
 from betty.locale import Str
 from betty.serde.dump import DictDump, Dump
 from betty.string import camel_case_to_kebab_case, upper_camel_case_to_lower_camel_case
 
 if TYPE_CHECKING:
     from betty.app import App
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class GeneratedEntityId(str):
     """
     Generate a unique entity ID.
 
     Entities must have IDs for identification. However, not all entities can be provided with an ID that exists in the
@@ -74,51 +86,51 @@
     @property
     def ancestry_id(self) -> tuple[builtins.type[Self], str]:
         return self.type, self.id
 
     @property
     def label(self) -> Str:
         return Str._(
-            '{entity_type} {entity_id}',
+            "{entity_type} {entity_id}",
             entity_type=self.entity_type_label(),
             entity_id=self.id,
         )
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
 
         entity_type_name = get_entity_type_name(self.type)
-        dump['$schema'] = app.static_url_generator.generate(
-            f'schema.json#/definitions/entity/{upper_camel_case_to_lower_camel_case(entity_type_name)}',
+        dump["$schema"] = app.static_url_generator.generate(
+            f"schema.json#/definitions/entity/{upper_camel_case_to_lower_camel_case(entity_type_name)}",
             absolute=True,
         )
 
         if not isinstance(self.id, GeneratedEntityId):
-            dump['@id'] = app.static_url_generator.generate(
-                f'/{camel_case_to_kebab_case(entity_type_name)}/{self.id}/index.json',
+            dump["@id"] = app.static_url_generator.generate(
+                f"/{camel_case_to_kebab_case(entity_type_name)}/{self.id}/index.json",
                 absolute=True,
             )
-            dump['id'] = self.id
+            dump["id"] = self.id
 
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        schema['type'] = 'object'
-        schema['properties'] = {
-            '$schema': ref_json_schema(schema),
-            'id': {
-                'type': 'string',
+        schema["type"] = "object"
+        schema["properties"] = {
+            "$schema": ref_json_schema(schema),
+            "id": {
+                "type": "string",
             },
         }
-        schema['required'] = [
-            '$schema',
+        schema["required"] = [
+            "$schema",
         ]
-        schema['additionalProperties'] = False
+        schema["additionalProperties"] = False
         add_json_ld(schema)
         return schema
 
 
 AncestryEntityId: TypeAlias = tuple[type[Entity], str]
 
 
@@ -127,71 +139,75 @@
 
 
 class EntityTypeProvider:
     async def entity_types(self) -> set[type[Entity]]:
         raise NotImplementedError(repr(self))
 
 
-EntityT = TypeVar('EntityT', bound=Entity)
-EntityU = TypeVar('EntityU', bound=Entity)
-TargetT = TypeVar('TargetT')
-OwnerT = TypeVar('OwnerT')
-AssociateT = TypeVar('AssociateT')
-AssociateU = TypeVar('AssociateU')
-LeftAssociateT = TypeVar('LeftAssociateT')
-RightAssociateT = TypeVar('RightAssociateT')
+EntityT = TypeVar("EntityT", bound=Entity)
+EntityU = TypeVar("EntityU", bound=Entity)
+TargetT = TypeVar("TargetT")
+OwnerT = TypeVar("OwnerT")
+AssociateT = TypeVar("AssociateT")
+AssociateU = TypeVar("AssociateU")
+LeftAssociateT = TypeVar("LeftAssociateT")
+RightAssociateT = TypeVar("RightAssociateT")
 
 
 def get_entity_type_name(entity_type_definition: type[Entity] | Entity) -> str:
     """
     Get the entity type name for an entity or entity type.
     """
     if isinstance(entity_type_definition, Entity):
         entity_type = entity_type_definition.type
     else:
         entity_type = entity_type_definition
 
-    if entity_type.__module__.startswith('betty.model.ancestry'):
+    if entity_type.__module__.startswith("betty.model.ancestry"):
         return entity_type.__name__
-    return f'{entity_type.__module__}.{entity_type.__name__}'
+    return f"{entity_type.__module__}.{entity_type.__name__}"
 
 
 def get_entity_type(entity_type_name: str) -> type[Entity]:
     """
     Get the entity type for an entity type name.
     """
     try:
         return import_any(entity_type_name)  # type: ignore[no-any-return]
     except ImportError:
         try:
-            return import_any(f'betty.model.ancestry.{entity_type_name}')  # type: ignore[no-any-return]
+            return import_any(f"betty.model.ancestry.{entity_type_name}")  # type: ignore[no-any-return]
         except ImportError:
             raise EntityTypeImportError(entity_type_name) from None
 
 
 class EntityTypeError(ValueError):
     pass
 
 
 class EntityTypeImportError(EntityTypeError, ImportError):
     """
     Raised when an alleged entity type cannot be imported.
     """
 
     def __init__(self, entity_type_name: str):
-        super().__init__(f'Cannot find and import an entity with name "{entity_type_name}".')
+        super().__init__(
+            f'Cannot find and import an entity with name "{entity_type_name}".'
+        )
 
 
 class EntityTypeInvalidError(EntityTypeError, ImportError):
     """
     Raised for types that are not valid entity types.
     """
 
     def __init__(self, entity_type: type):
-        super().__init__(f'{entity_type.__module__}.{entity_type.__name__} is not an entity type class. Entity types must extend {Entity.__module__}.{Entity.__name__} directly.')
+        super().__init__(
+            f"{entity_type.__module__}.{entity_type.__name__} is not an entity type class. Entity types must extend {Entity.__module__}.{Entity.__name__} directly."
+        )
 
 
 class EntityCollection(Generic[TargetT]):
     __slots__ = ()
 
     def __init__(self):
         super().__init__()
@@ -209,20 +225,15 @@
     def add(self, *entities: TargetT & Entity) -> None:
         raise NotImplementedError(repr(self))
 
     def remove(self, *entities: TargetT & Entity) -> None:
         raise NotImplementedError(repr(self))
 
     def replace(self, *entities: TargetT & Entity) -> None:
-        self.remove(*(
-            entity
-            for entity
-            in self
-            if entity not in entities
-        ))
+        self.remove(*(entity for entity in self if entity not in entities))
         self.add(*entities)
 
     def clear(self) -> None:
         raise NotImplementedError(repr(self))
 
     def __iter__(self) -> Iterator[TargetT & Entity]:
         raise NotImplementedError(repr(self))
@@ -234,15 +245,17 @@
     def __getitem__(self, index: int) -> TargetT & Entity:
         pass
 
     @overload
     def __getitem__(self, indices: slice) -> list[TargetT & Entity]:
         pass
 
-    def __getitem__(self, key: int | slice) -> TargetT & Entity | list[TargetT & Entity]:
+    def __getitem__(
+        self, key: int | slice
+    ) -> TargetT & Entity | list[TargetT & Entity]:
         raise NotImplementedError(repr(self))
 
     def __delitem__(self, key: TargetT & Entity) -> None:
         raise NotImplementedError(repr(self))
 
     def __contains__(self, value: Any) -> bool:
         raise NotImplementedError(repr(self))
@@ -258,36 +271,38 @@
         seen = []
         for entity in entities:
             if entity not in self and entity not in seen:
                 yield entity
                 seen.append(entity)
 
 
-EntityCollectionT = TypeVar('EntityCollectionT', bound=EntityCollection[EntityT])
+EntityCollectionT = TypeVar("EntityCollectionT", bound=EntityCollection[EntityT])
 
 
 class _EntityTypeAssociation(Generic[OwnerT, AssociateT]):
     def __init__(
         self,
         owner_type: type[OwnerT],
         owner_attr_name: str,
         associate_type_name: str,
     ):
         self._owner_type = owner_type
         self._owner_attr_name = owner_attr_name
-        self._owner_private_attr_name = f'_{owner_attr_name}'
+        self._owner_private_attr_name = f"_{owner_attr_name}"
         self._associate_type_name = associate_type_name
         self._associate_type: type[AssociateT] | None = None
 
     def __hash__(self) -> int:
-        return hash((
-            self._owner_type,
-            self._owner_attr_name,
-            self._associate_type_name,
-        ))
+        return hash(
+            (
+                self._owner_type,
+                self._owner_attr_name,
+                self._associate_type_name,
+            )
+        )
 
     def __repr__(self) -> str:
         return repr_instance(
             self,
             owner_type=self._owner_type,
             owner_attr_name=self._owner_attr_name,
             associate_type_name=self._associate_type_name,
@@ -314,14 +329,15 @@
 
         original_init = self._owner_type.__init__
 
         @functools.wraps(original_init)
         def _init(owner: OwnerT & Entity, *args: Any, **kwargs: Any) -> None:
             self.initialize(owner)
             original_init(owner, *args, **kwargs)
+
         self._owner_type.__init__ = _init  # type: ignore[assignment, method-assign]
 
     def initialize(self, owner: OwnerT & Entity) -> None:
         raise NotImplementedError(repr(self))
 
     def finalize(self, owner: OwnerT & Entity) -> None:
         self.delete(owner)
@@ -329,19 +345,23 @@
 
     def delete(self, owner: OwnerT & Entity) -> None:
         raise NotImplementedError(repr(self))
 
     def associate(self, owner: OwnerT & Entity, associate: AssociateT & Entity) -> None:
         raise NotImplementedError(repr(self))
 
-    def disassociate(self, owner: OwnerT & Entity, associate: AssociateT & Entity) -> None:
+    def disassociate(
+        self, owner: OwnerT & Entity, associate: AssociateT & Entity
+    ) -> None:
         raise NotImplementedError(repr(self))
 
 
-class BidirectionalEntityTypeAssociation(Generic[OwnerT, AssociateT], _EntityTypeAssociation[OwnerT, AssociateT]):
+class BidirectionalEntityTypeAssociation(
+    Generic[OwnerT, AssociateT], _EntityTypeAssociation[OwnerT, AssociateT]
+):
     def __init__(
         self,
         owner_type: type[OwnerT],
         owner_attr_name: str,
         associate_type_name: str,
         associate_attr_name: str,
     ):
@@ -349,20 +369,22 @@
             owner_type,
             owner_attr_name,
             associate_type_name,
         )
         self._associate_attr_name = associate_attr_name
 
     def __hash__(self) -> int:
-        return hash((
-            self._owner_type,
-            self._owner_attr_name,
-            self._associate_type_name,
-            self._associate_attr_name,
-        ))
+        return hash(
+            (
+                self._owner_type,
+                self._owner_attr_name,
+                self._associate_type_name,
+                self._associate_attr_name,
+            )
+        )
 
     def __repr__(self) -> str:
         return repr_instance(
             self,
             owner_type=self._owner_type,
             owner_attr_name=self._owner_attr_name,
             associate_type_name=self._associate_type_name,
@@ -370,20 +392,24 @@
         )
 
     @property
     def associate_attr_name(self) -> str:
         return self._associate_attr_name
 
     def inverse(self) -> BidirectionalEntityTypeAssociation[AssociateT, OwnerT]:
-        association = EntityTypeAssociationRegistry.get_association(self.associate_type, self.associate_attr_name)
+        association = EntityTypeAssociationRegistry.get_association(
+            self.associate_type, self.associate_attr_name
+        )
         assert isinstance(association, BidirectionalEntityTypeAssociation)
         return association
 
 
-class ToOneEntityTypeAssociation(Generic[OwnerT, AssociateT], _EntityTypeAssociation[OwnerT, AssociateT]):
+class ToOneEntityTypeAssociation(
+    Generic[OwnerT, AssociateT], _EntityTypeAssociation[OwnerT, AssociateT]
+):
     def register(self) -> None:
         super().register()
         setattr(
             self.owner_type,
             self.owner_attr_name,
             property(
                 self.get,
@@ -394,63 +420,78 @@
 
     def initialize(self, owner: OwnerT & Entity) -> None:
         setattr(owner, self._owner_private_attr_name, None)
 
     def get(self, owner: OwnerT & Entity) -> AssociateT & Entity | None:
         return getattr(owner, self._owner_private_attr_name)  # type: ignore[no-any-return]
 
-    def set(self, owner: OwnerT & Entity, associate: AssociateT & Entity | None) -> None:
+    def set(
+        self, owner: OwnerT & Entity, associate: AssociateT & Entity | None
+    ) -> None:
         setattr(owner, self._owner_private_attr_name, associate)
 
     def delete(self, owner: OwnerT & Entity) -> None:
         self.set(owner, None)
 
     def associate(self, owner: OwnerT & Entity, associate: AssociateT & Entity) -> None:
         self.set(owner, associate)
 
-    def disassociate(self, owner: OwnerT & Entity, associate: AssociateT & Entity) -> None:
+    def disassociate(
+        self, owner: OwnerT & Entity, associate: AssociateT & Entity
+    ) -> None:
         if associate == self.get(owner):
             self.delete(owner)
 
 
-class ToManyEntityTypeAssociation(Generic[OwnerT, AssociateT], _EntityTypeAssociation[OwnerT, AssociateT]):
+class ToManyEntityTypeAssociation(
+    Generic[OwnerT, AssociateT], _EntityTypeAssociation[OwnerT, AssociateT]
+):
     def register(self) -> None:
         super().register()
         setattr(
             self.owner_type,
             self.owner_attr_name,
             property(
                 self.get,
                 self.set,
                 self.delete,
             ),
         )
 
     def get(self, owner: OwnerT & Entity) -> EntityCollection[AssociateT & Entity]:
-        return cast(EntityCollection['AssociateT & Entity'], getattr(owner, self._owner_private_attr_name))
+        return cast(
+            EntityCollection["AssociateT & Entity"],
+            getattr(owner, self._owner_private_attr_name),
+        )
 
-    def set(self, owner: OwnerT & Entity, entities: Iterable[AssociateT & Entity]) -> None:
+    def set(
+        self, owner: OwnerT & Entity, entities: Iterable[AssociateT & Entity]
+    ) -> None:
         self.get(owner).replace(*entities)
 
     def delete(self, owner: OwnerT & Entity) -> None:
         self.get(owner).clear()
 
     def associate(self, owner: OwnerT & Entity, associate: AssociateT & Entity) -> None:
         self.get(owner).add(associate)
 
-    def disassociate(self, owner: OwnerT & Entity, associate: AssociateT & Entity) -> None:
+    def disassociate(
+        self, owner: OwnerT & Entity, associate: AssociateT & Entity
+    ) -> None:
         self.get(owner).remove(associate)
 
 
 class BidirectionalToOneEntityTypeAssociation(
     Generic[OwnerT, AssociateT],
     ToOneEntityTypeAssociation[OwnerT, AssociateT],
-    BidirectionalEntityTypeAssociation[OwnerT, AssociateT]
+    BidirectionalEntityTypeAssociation[OwnerT, AssociateT],
 ):
-    def set(self, owner: OwnerT & Entity, associate: AssociateT & Entity | None) -> None:
+    def set(
+        self, owner: OwnerT & Entity, associate: AssociateT & Entity | None
+    ) -> None:
         previous_associate = self.get(owner)
         if previous_associate == associate:
             return
         super().set(owner, associate)
         if previous_associate is not None:
             self.inverse().disassociate(previous_associate, owner)
         if associate is not None:
@@ -465,211 +506,251 @@
     def initialize(self, owner: OwnerT & Entity) -> None:
         setattr(
             owner,
             self._owner_private_attr_name,
             _BidirectionalAssociateCollection(
                 owner,
                 self,
-            )
+            ),
         )
 
 
-class ToOne(Generic[OwnerT, AssociateT], ToOneEntityTypeAssociation[OwnerT, AssociateT]):
+class ToOne(
+    Generic[OwnerT, AssociateT], ToOneEntityTypeAssociation[OwnerT, AssociateT]
+):
     pass
 
 
-class OneToOne(Generic[OwnerT, AssociateT], BidirectionalToOneEntityTypeAssociation[OwnerT, AssociateT]):
+class OneToOne(
+    Generic[OwnerT, AssociateT],
+    BidirectionalToOneEntityTypeAssociation[OwnerT, AssociateT],
+):
     pass
 
 
-class ManyToOne(Generic[OwnerT, AssociateT], BidirectionalToOneEntityTypeAssociation[OwnerT, AssociateT]):
+class ManyToOne(
+    Generic[OwnerT, AssociateT],
+    BidirectionalToOneEntityTypeAssociation[OwnerT, AssociateT],
+):
     pass
 
 
-class ToMany(Generic[OwnerT, AssociateT], ToManyEntityTypeAssociation[OwnerT, AssociateT]):
+class ToMany(
+    Generic[OwnerT, AssociateT], ToManyEntityTypeAssociation[OwnerT, AssociateT]
+):
     def initialize(self, owner: OwnerT & Entity) -> None:
         setattr(
             owner,
             self._owner_private_attr_name,
-            SingleTypeEntityCollection[AssociateT](self.associate_type)
+            SingleTypeEntityCollection[AssociateT](self.associate_type),
         )
 
 
-class OneToMany(Generic[OwnerT, AssociateT], BidirectionalToManyEntityTypeAssociation[OwnerT, AssociateT]):
+class OneToMany(
+    Generic[OwnerT, AssociateT],
+    BidirectionalToManyEntityTypeAssociation[OwnerT, AssociateT],
+):
     pass
 
 
-class ManyToMany(Generic[OwnerT, AssociateT], BidirectionalToManyEntityTypeAssociation[OwnerT, AssociateT]):
+class ManyToMany(
+    Generic[OwnerT, AssociateT],
+    BidirectionalToManyEntityTypeAssociation[OwnerT, AssociateT],
+):
     pass
 
 
-ToAny: TypeAlias = ToOneEntityTypeAssociation[OwnerT, AssociateT] | ToManyEntityTypeAssociation[OwnerT, AssociateT]
+ToAny: TypeAlias = (
+    ToOneEntityTypeAssociation[OwnerT, AssociateT]
+    | ToManyEntityTypeAssociation[OwnerT, AssociateT]
+)
 
 
 def to_one(
     owner_attr_name: str,
     associate_type_name: str,
 ) -> Callable[[type[OwnerT]], type[OwnerT]]:
     """
     Add a unidirectional to-one association to an entity or entity mixin.
     """
+
     def _decorator(owner_type: type[OwnerT]) -> type[OwnerT]:
         ToOne(
             owner_type,
             owner_attr_name,
             associate_type_name,
         ).register()
         return owner_type
+
     return _decorator
 
 
 def one_to_one(
     owner_attr_name: str,
     associate_type_name: str,
     associate_attr_name: str,
 ) -> Callable[[type[OwnerT]], type[OwnerT]]:
     """
     Add a bidirectional one-to-one association to an entity or entity mixin.
     """
+
     def _decorator(owner_type: type[OwnerT]) -> type[OwnerT]:
         OneToOne(
             owner_type,
             owner_attr_name,
             associate_type_name,
             associate_attr_name,
         ).register()
         return owner_type
+
     return _decorator
 
 
 def many_to_one(
     owner_attr_name: str,
     associate_type_name: str,
     associate_attr_name: str,
 ) -> Callable[[type[OwnerT]], type[OwnerT]]:
     """
     Add a bidirectional many-to-one association to an entity or entity mixin.
     """
+
     def _decorator(owner_type: type[OwnerT]) -> type[OwnerT]:
         ManyToOne(
             owner_type,
             owner_attr_name,
             associate_type_name,
             associate_attr_name,
         ).register()
         return owner_type
+
     return _decorator
 
 
 def to_many(
     owner_attr_name: str,
     associate_type_name: str,
 ) -> Callable[[type[OwnerT]], type[OwnerT]]:
     """
     Add a unidirectional to-many association to an entity or entity mixin.
     """
+
     def _decorator(owner_type: type[OwnerT]) -> type[OwnerT]:
         ToMany(
             owner_type,
             owner_attr_name,
             associate_type_name,
         ).register()
         return owner_type
+
     return _decorator
 
 
 def one_to_many(
     owner_attr_name: str,
     associate_type_name: str,
     associate_attr_name: str,
 ) -> Callable[[type[OwnerT]], type[OwnerT]]:
     """
     Add a bidirectional one-to-many association to an entity or entity mixin.
     """
+
     def _decorator(owner_type: type[OwnerT]) -> type[OwnerT]:
         OneToMany(
             owner_type,
             owner_attr_name,
             associate_type_name,
             associate_attr_name,
         ).register()
         return owner_type
+
     return _decorator
 
 
 def many_to_many(
     owner_attr_name: str,
     associate_type_name: str,
     associate_attr_name: str,
 ) -> Callable[[type[OwnerT]], type[OwnerT]]:
     """
     Add a bidirectional many-to-many association to an entity or entity mixin.
     """
+
     def _decorator(owner_type: type[OwnerT]) -> type[OwnerT]:
         ManyToMany(
             owner_type,
             owner_attr_name,
             associate_type_name,
             associate_attr_name,
         ).register()
         return owner_type
+
     return _decorator
 
 
 def many_to_one_to_many(
     left_associate_type_name: str,
     left_associate_attr_name: str,
     left_owner_attr_name: str,
     right_owner_attr_name: str,
     right_associate_type_name: str,
     right_associate_attr_name: str,
 ) -> Callable[[type[OwnerT]], type[OwnerT]]:
     """
     Add a bidirectional many-to-one-to-many association to an entity or entity mixin.
     """
+
     def _decorator(owner_type: type[OwnerT]) -> type[OwnerT]:
         ManyToOne(
             owner_type,
             left_owner_attr_name,
             left_associate_type_name,
             left_associate_attr_name,
         ).register()
         ManyToOne(
             owner_type,
             right_owner_attr_name,
             right_associate_type_name,
             right_associate_attr_name,
         ).register()
         return owner_type
+
     return _decorator
 
 
 class EntityTypeAssociationRegistry:
     _associations = set[ToAny[Any, Any]]()
 
     @classmethod
     def get_all_associations(cls, owner: type | object) -> set[ToAny[Any, Any]]:
         owner_type = owner if isinstance(owner, type) else type(owner)
         return {
             association
-            for association
-            in cls._associations
+            for association in cls._associations
             if association.owner_type in owner_type.__mro__
         }
 
     @classmethod
-    def get_association(cls, owner: type[OwnerT] | OwnerT & Entity, owner_attr_name: str) -> ToAny[OwnerT, Any]:
+    def get_association(
+        cls, owner: type[OwnerT] | OwnerT & Entity, owner_attr_name: str
+    ) -> ToAny[OwnerT, Any]:
         for association in cls.get_all_associations(owner):
             if association.owner_attr_name == owner_attr_name:
                 return association
-        raise ValueError(f'No association exists for {fully_qualified_type_name(owner if isinstance(owner, type) else owner.__class__)}.{owner_attr_name}.')
+        raise ValueError(
+            f"No association exists for {fully_qualified_type_name(owner if isinstance(owner, type) else owner.__class__)}.{owner_attr_name}."
+        )
 
     @classmethod
-    def get_associates(cls, owner: EntityT, association: ToAny[EntityT, AssociateT]) -> Iterable[AssociateT]:
-        associates: AssociateT | None | Iterable[AssociateT] = getattr(owner, f'_{association.owner_attr_name}')
+    def get_associates(
+        cls, owner: EntityT, association: ToAny[EntityT, AssociateT]
+    ) -> Iterable[AssociateT]:
+        associates: AssociateT | None | Iterable[AssociateT] = getattr(
+            owner, f"_{association.owner_attr_name}"
+        )
         if isinstance(association, ToOneEntityTypeAssociation):
             if associates is None:
                 return
             yield cast(AssociateT, associates)
             return
         yield from cast(Iterable[AssociateT], associates)
 
@@ -687,15 +768,15 @@
     def finalize(cls, *owners: Entity) -> None:
         for owner in owners:
             for association in cls.get_all_associations(owner):
                 association.finalize(owner)
 
 
 class SingleTypeEntityCollection(Generic[TargetT], EntityCollection[TargetT]):
-    __slots__ = '_entities', '_target_type'
+    __slots__ = "_entities", "_target_type"
 
     def __init__(
         self,
         target_type: type[TargetT],
     ):
         super().__init__()
         self._entities: list[TargetT & Entity] = []
@@ -736,15 +817,17 @@
     def __getitem__(self, indices: slice) -> list[TargetT & Entity]:
         pass
 
     @overload
     def __getitem__(self, entity_id: str) -> TargetT & Entity:
         pass
 
-    def __getitem__(self, key: int | slice | str) -> TargetT & Entity | list[TargetT & Entity]:
+    def __getitem__(
+        self, key: int | slice | str
+    ) -> TargetT & Entity | list[TargetT & Entity]:
         if isinstance(key, int):
             return self._getitem_by_index(key)
         if isinstance(key, slice):
             return self._getitem_by_indices(key)
         return self._getitem_by_entity_id(key)
 
     def _getitem_by_index(self, index: int) -> TargetT & Entity:
@@ -753,35 +836,37 @@
     def _getitem_by_indices(self, indices: slice) -> list[TargetT & Entity]:
         return self.view[indices]
 
     def _getitem_by_entity_id(self, entity_id: str) -> TargetT & Entity:
         for entity in self._entities:
             if entity_id == entity.id:
                 return entity
-        raise KeyError(f'Cannot find a {self._target_type} entity with ID "{entity_id}".')
+        raise KeyError(
+            f'Cannot find a {self._target_type} entity with ID "{entity_id}".'
+        )
 
     def __delitem__(self, key: str | TargetT & Entity) -> None:
         if isinstance(key, self._target_type):
-            return self._delitem_by_entity(cast('TargetT & Entity', key))
+            return self._delitem_by_entity(cast("TargetT & Entity", key))
         if isinstance(key, str):
             return self._delitem_by_entity_id(key)
-        raise TypeError(f'Cannot find entities by {repr(key)}.')
+        raise TypeError(f"Cannot find entities by {repr(key)}.")
 
     def _delitem_by_entity(self, entity: TargetT & Entity) -> None:
         self.remove(entity)
 
     def _delitem_by_entity_id(self, entity_id: str) -> None:
         for entity in self._entities:
             if entity_id == entity.id:
                 self.remove(entity)
                 return
 
     def __contains__(self, value: Any) -> bool:
         if isinstance(value, self._target_type):
-            return self._contains_by_entity(cast('TargetT & Entity', value))
+            return self._contains_by_entity(cast("TargetT & Entity", value))
         if isinstance(value, str):
             return self._contains_by_entity_id(value)
         return False
 
     def _contains_by_entity(self, other_entity: TargetT & Entity) -> bool:
         for entity in self._entities:
             if other_entity is entity:
@@ -791,72 +876,91 @@
     def _contains_by_entity_id(self, entity_id: str) -> bool:
         for entity in self._entities:
             if entity.id == entity_id:
                 return True
         return False
 
 
-SingleTypeEntityCollectionT = TypeVar('SingleTypeEntityCollectionT', bound=SingleTypeEntityCollection[AssociateT])
+SingleTypeEntityCollectionT = TypeVar(
+    "SingleTypeEntityCollectionT", bound=SingleTypeEntityCollection[AssociateT]
+)
 
 
 class MultipleTypesEntityCollection(Generic[TargetT], EntityCollection[TargetT]):
-    __slots__ = '_collections'
+    __slots__ = "_collections"
 
     def __init__(self):
         super().__init__()
         self._collections: dict[type[Entity], SingleTypeEntityCollection[Entity]] = {}
 
     @recursive_repr()
     def __repr__(self) -> str:
         return repr_instance(
             self,
-            entity_types=', '.join(map(get_entity_type_name, self._collections.keys())),
+            entity_types=", ".join(map(get_entity_type_name, self._collections.keys())),
             length=len(self),
         )
 
-    def _get_collection(self, entity_type: type[EntityT]) -> SingleTypeEntityCollection[EntityT]:
-        assert issubclass(entity_type, Entity), f'{entity_type} is not an entity type.'
+    def _get_collection(
+        self, entity_type: type[EntityT]
+    ) -> SingleTypeEntityCollection[EntityT]:
+        assert issubclass(entity_type, Entity), f"{entity_type} is not an entity type."
         try:
-            return cast(SingleTypeEntityCollection[EntityT], self._collections[entity_type])
+            return cast(
+                SingleTypeEntityCollection[EntityT], self._collections[entity_type]
+            )
         except KeyError:
             self._collections[entity_type] = SingleTypeEntityCollection(entity_type)
-            return cast(SingleTypeEntityCollection[EntityT], self._collections[entity_type])
+            return cast(
+                SingleTypeEntityCollection[EntityT], self._collections[entity_type]
+            )
 
     @overload
     def __getitem__(self, index: int) -> TargetT & Entity:
         pass
 
     @overload
     def __getitem__(self, indices: slice) -> list[TargetT & Entity]:
         pass
 
     @overload
     def __getitem__(self, entity_type_name: str) -> SingleTypeEntityCollection[Entity]:
         pass
 
     @overload
-    def __getitem__(self, entity_type: type[EntityT]) -> SingleTypeEntityCollection[EntityT]:
+    def __getitem__(
+        self, entity_type: type[EntityT]
+    ) -> SingleTypeEntityCollection[EntityT]:
         pass
 
     def __getitem__(
         self,
         key: int | slice | str | type[EntityT],
-    ) -> TargetT & Entity | SingleTypeEntityCollection[Entity] | SingleTypeEntityCollection[EntityT] | list[TargetT & Entity]:
+    ) -> (
+        TargetT & Entity
+        | SingleTypeEntityCollection[Entity]
+        | SingleTypeEntityCollection[EntityT]
+        | list[TargetT & Entity]
+    ):
         if isinstance(key, int):
             return self._getitem_by_index(key)
         if isinstance(key, slice):
             return self._getitem_by_indices(key)
         if isinstance(key, str):
             return self._getitem_by_entity_type_name(key)
         return self._getitem_by_entity_type(key)
 
-    def _getitem_by_entity_type(self, entity_type: type[EntityT]) -> SingleTypeEntityCollection[EntityT]:
+    def _getitem_by_entity_type(
+        self, entity_type: type[EntityT]
+    ) -> SingleTypeEntityCollection[EntityT]:
         return self._get_collection(entity_type)
 
-    def _getitem_by_entity_type_name(self, entity_type_name: str) -> SingleTypeEntityCollection[Entity]:
+    def _getitem_by_entity_type_name(
+        self, entity_type_name: str
+    ) -> SingleTypeEntityCollection[Entity]:
         return self._get_collection(
             get_entity_type(entity_type_name),
         )
 
     def _getitem_by_index(self, index: int) -> TargetT & Entity:
         return self.view[index]
 
@@ -887,15 +991,15 @@
         self._delitem_by_type(
             get_entity_type(entity_type_name),  # type: ignore[arg-type]
         )
 
     def __iter__(self) -> Iterator[TargetT & Entity]:
         for collection in self._collections.values():
             for entity in collection:
-                yield cast('TargetT & Entity', entity)
+                yield cast("TargetT & Entity", entity)
 
     def __len__(self) -> int:
         return sum(map(len, self._collections.values()))
 
     def __contains__(self, value: Any) -> bool:
         if isinstance(value, Entity):
             return self._contains_by_entity(value)
@@ -925,31 +1029,35 @@
         removed_entities = (*self,)
         for collection in self._collections.values():
             collection.clear()
         if removed_entities:
             self._on_remove(*removed_entities)
 
 
-class _BidirectionalAssociateCollection(Generic[AssociateT, OwnerT], SingleTypeEntityCollection[AssociateT]):
-    __slots__ = '__owner', '_association'
+class _BidirectionalAssociateCollection(
+    Generic[AssociateT, OwnerT], SingleTypeEntityCollection[AssociateT]
+):
+    __slots__ = "__owner", "_association"
 
     def __init__(
         self,
         owner: OwnerT & Entity,
         association: BidirectionalEntityTypeAssociation[OwnerT, AssociateT],
     ):
         super().__init__(association.associate_type)
         self._association = association
         self.__owner = weakref.ref(owner)
 
     @property
     def _owner(self) -> OwnerT & Entity:
         owner = self.__owner()
         if owner is None:
-            raise RuntimeError("This associate collection's owner no longer exists in memory.")
+            raise RuntimeError(
+                "This associate collection's owner no longer exists in memory."
+            )
         return owner
 
     def _on_add(self, *entities: AssociateT & Entity) -> None:
         super()._on_add(*entities)
         for associate in entities:
             self._association.inverse().associate(associate, self._owner)
 
@@ -958,15 +1066,17 @@
         for associate in entities:
             self._association.inverse().disassociate(associate, self._owner)
 
 
 class AliasedEntity(Generic[EntityT]):
     def __init__(self, original_entity: EntityT, aliased_entity_id: str | None = None):
         self._entity = original_entity
-        self._id = GeneratedEntityId() if aliased_entity_id is None else aliased_entity_id
+        self._id = (
+            GeneratedEntityId() if aliased_entity_id is None else aliased_entity_id
+        )
 
     def __repr__(self) -> str:
         return repr_instance(self, id=self.id)
 
     @property
     def type(self) -> builtins.type[Entity]:
         return self._entity.type
@@ -987,73 +1097,71 @@
     Unalias a potentially aliased entity.
     """
     if isinstance(entity, AliasedEntity):
         return entity.unalias()
     return entity
 
 
-_EntityGraphBuilderEntities: TypeAlias = dict[type[Entity], dict[str, AliasableEntity[Entity]]]
+_EntityGraphBuilderEntities: TypeAlias = dict[
+    type[Entity], dict[str, AliasableEntity[Entity]]
+]
 
 
 _EntityGraphBuilderAssociations: TypeAlias = dict[
     type[Entity],  # The owner entity type.
     dict[
         str,  # The owner attribute name.
-        dict[
-            str,  # The owner ID.
-            list[AncestryEntityId]  # The associate IDs.
-        ]
-    ]
+        dict[str, list[AncestryEntityId]],  # The owner ID.  # The associate IDs.
+    ],
 ]
 
 
 class _EntityGraphBuilder:
     def __init__(self):
         self._entities: _EntityGraphBuilderEntities = defaultdict(dict)
-        self._associations: _EntityGraphBuilderAssociations = defaultdict(lambda: defaultdict(lambda: defaultdict(lambda: list())))
+        self._associations: _EntityGraphBuilderAssociations = defaultdict(
+            lambda: defaultdict(lambda: defaultdict(lambda: list()))
+        )
         self._built = False
 
     def _assert_unbuilt(self) -> None:
         if self._built:
-            raise RuntimeError('This entity graph has been built already.')
+            raise RuntimeError("This entity graph has been built already.")
 
     def _iter(self) -> Iterator[AliasableEntity[Entity]]:
         for entity_type in self._entities:
             yield from self._entities[entity_type].values()
 
     def _build_associations(self) -> None:
         for owner_type, owner_attrs in self._associations.items():
             for owner_attr_name, owner_associations in owner_attrs.items():
-                association = EntityTypeAssociationRegistry.get_association(owner_type, owner_attr_name)
+                association = EntityTypeAssociationRegistry.get_association(
+                    owner_type, owner_attr_name
+                )
                 for owner_id, associate_ancestry_ids in owner_associations.items():
                     associates = [
                         unalias(self._entities[associate_type][associate_id])
-                        for associate_type, associate_id
-                        in associate_ancestry_ids
+                        for associate_type, associate_id in associate_ancestry_ids
                     ]
                     owner = unalias(self._entities[owner_type][owner_id])
                     if isinstance(association, ToOneEntityTypeAssociation):
-                        association.set(
-                            owner,
-                            associates[0]
-                        )
+                        association.set(owner, associates[0])
                     else:
-                        association.set(
-                            owner,
-                            associates
-                        )
+                        association.set(owner, associates)
 
     def build(self) -> Iterator[Entity]:
         self._assert_unbuilt()
         self._built = True
 
-        unaliased_entities = list(map(
-            unalias,
-            self._iter(),
-        ))
+        unaliased_entities = list(
+            map(
+                unalias,
+                self._iter(),
+            )
+        )
 
         EntityTypeAssociationRegistry.initialize(*unaliased_entities)
         self._build_associations()
 
         yield from unaliased_entities
 
 
@@ -1070,24 +1178,23 @@
         owner_id: str,
         owner_attr_name: str,
         associate_type: type[Entity],
         associate_id: str,
     ) -> None:
         self._assert_unbuilt()
 
-        self._associations[owner_type][owner_attr_name][owner_id].append((associate_type, associate_id))
+        self._associations[owner_type][owner_attr_name][owner_id].append(
+            (associate_type, associate_id)
+        )
 
 
 @contextmanager
-def record_added(entities: EntityCollection[EntityT]) -> Iterator[MultipleTypesEntityCollection[EntityT]]:
+def record_added(
+    entities: EntityCollection[EntityT],
+) -> Iterator[MultipleTypesEntityCollection[EntityT]]:
     """
     Record all entities that are added to a collection.
     """
     original = [*entities]
     added = MultipleTypesEntityCollection[EntityT]()
     yield added
-    added.add(*[
-        entity
-        for entity
-        in entities
-        if entity not in original
-    ])
+    added.add(*[entity for entity in entities if entity not in original])
```

### Comparing `betty-0.3.3/betty/model/ancestry.py` & `betty-0.3.4/betty/model/ancestry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 """
 Provide Betty's main data model.
 """
+
 from __future__ import annotations
 
 from collections.abc import MutableSequence
 from contextlib import suppress
 from enum import Enum
 from pathlib import Path
 from reprlib import recursive_repr
 from typing import Iterable, Any, TYPE_CHECKING
 from urllib.parse import quote
 
 from geopy import Point
 
 from betty.classtools import repr_instance
-from betty.json.linked_data import LinkedDataDumpable, dump_context, dump_link, add_json_ld
+from betty.json.linked_data import (
+    LinkedDataDumpable,
+    dump_context,
+    dump_link,
+    add_json_ld,
+)
 from betty.json.schema import add_property, ref_json_schema
 from betty.locale import Localized, Datey, Str, Localizable, ref_datey
 from betty.media_type import MediaType
-from betty.model import many_to_many, Entity, one_to_many, many_to_one, many_to_one_to_many, \
-    MultipleTypesEntityCollection, EntityCollection, UserFacingEntity, EntityTypeAssociationRegistry, \
-    GeneratedEntityId, get_entity_type_name
+from betty.model import (
+    many_to_many,
+    Entity,
+    one_to_many,
+    many_to_one,
+    many_to_one_to_many,
+    MultipleTypesEntityCollection,
+    EntityCollection,
+    UserFacingEntity,
+    EntityTypeAssociationRegistry,
+    GeneratedEntityId,
+    get_entity_type_name,
+)
 from betty.model.event_type import EventType, UnknownEventType
 from betty.serde.dump import DictDump, Dump, dump_default
 from betty.string import camel_case_to_kebab_case
 from betty.warnings import deprecated
 
 if TYPE_CHECKING:
     from betty.app import App
@@ -43,15 +59,17 @@
         privacy: Privacy | None = None,
         public: bool | None = None,
         private: bool | None = None,
         **kwargs: Any,
     ):
         super().__init__(*args, **kwargs)
         if [privacy, public, private].count(None) < 2:
-            raise ValueError(f'Only one of the `privacy`, `public`, and `private` arguments to {type(self)}.__init__() may be given at a time.')
+            raise ValueError(
+                f"Only one of the `privacy`, `public`, and `private` arguments to {type(self)}.__init__() may be given at a time."
+            )
         if privacy is not None:
             self._privacy = privacy
         elif public is True:
             self._privacy = Privacy.PUBLIC
         elif private is True:
             self._privacy = Privacy.PRIVATE
         else:
@@ -91,28 +109,32 @@
 
     @public.setter
     def public(self, public: True) -> None:
         self.privacy = Privacy.PUBLIC
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
-        dump['private'] = self.private
+        dump["private"] = self.private
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'private', {
-            '$ref': '#/definitions/privacy',
-        })
-        definitions = dump_default(schema, 'definitions', dict)
-        if 'privacy' not in definitions:
-            definitions['privacy'] = {
-                'type': 'boolean',
-                'description': 'Whether this entity is private (true), or public (false).'
+        add_property(
+            schema,
+            "private",
+            {
+                "$ref": "#/definitions/privacy",
+            },
+        )
+        definitions = dump_default(schema, "definitions", dict)
+        if "privacy" not in definitions:
+            definitions["privacy"] = {
+                "type": "boolean",
+                "description": "Whether this entity is private (true), or public (false).",
             }
         return schema
 
 
 def is_private(target: Any) -> bool:
     """
     Check if the given target is private.
@@ -142,19 +164,15 @@
     return privacy.privacy
 
 
 def merge_privacies(*privacies: Privacy | HasPrivacy | None) -> Privacy:
     """
     Merge multiple privacies into one.
     """
-    privacies = {
-        resolve_privacy(privacy)
-        for privacy
-        in privacies
-    }
+    privacies = {resolve_privacy(privacy) for privacy in privacies}
     if Privacy.PRIVATE in privacies:
         return Privacy.PRIVATE
     if Privacy.UNDETERMINED in privacies:
         return Privacy.UNDETERMINED
     return Privacy.PUBLIC
 
 
@@ -167,23 +185,23 @@
     ):
         super().__init__(*args, **kwargs)
         self.date = date
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
         if self.date and is_public(self):
-            dump['date'] = await self.date.dump_linked_data(app)
+            dump["date"] = await self.date.dump_linked_data(app)
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        schema['type'] = 'object'
-        schema['additionalProperties'] = False
-        add_property(schema, 'date', await ref_datey(schema, app), False)
+        schema["type"] = "object"
+        schema["additionalProperties"] = False
+        add_property(schema, "date", await ref_datey(schema, app), False)
         return schema
 
 
 class Described(LinkedDataDumpable):
     def __init__(
         self,
         *args: Any,
@@ -192,28 +210,33 @@
     ):
         super().__init__(*args, **kwargs)
         self.description = description
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
         if self.description is not None:
-            dump['description'] = self.description
-            dump_context(dump, description='description')
+            dump["description"] = self.description
+            dump_context(dump, description="description")
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'description', {
-            '$ref': '#/definitions/description',
-        }, False)
-        definitions = dump_default(schema, 'definitions', dict)
-        if 'description' not in definitions:
-            definitions['description'] = {
-                'type': 'string',
+        add_property(
+            schema,
+            "description",
+            {
+                "$ref": "#/definitions/description",
+            },
+            False,
+        )
+        definitions = dump_default(schema, "definitions", dict)
+        if "description" not in definitions:
+            definitions["description"] = {
+                "type": "string",
             }
         return schema
 
 
 class HasMediaType(LinkedDataDumpable):
     def __init__(
         self,
@@ -224,36 +247,36 @@
         super().__init__(*args, **kwargs)
         self.media_type = media_type
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
         if is_public(self):
             if self.media_type is not None:
-                dump['mediaType'] = str(self.media_type)
+                dump["mediaType"] = str(self.media_type)
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'mediaType', ref_media_type(schema), False)
+        add_property(schema, "mediaType", ref_media_type(schema), False)
         return schema
 
 
 def ref_media_type(root_schema: DictDump[Dump]) -> DictDump[Dump]:
     """
     Reference the MediaType schema.
     """
-    definitions = dump_default(root_schema, 'definitions', dict)
-    if 'mediaType' not in definitions:
-        definitions['mediaType'] = {
-            'type': 'string',
-            'description': 'An IANA media type (https://www.iana.org/assignments/media-types/media-types.xhtml).'
+    definitions = dump_default(root_schema, "definitions", dict)
+    if "mediaType" not in definitions:
+        definitions["mediaType"] = {
+            "type": "string",
+            "description": "An IANA media type (https://www.iana.org/assignments/media-types/media-types.xhtml).",
         }
     return {
-        '$ref': '#/definitions/mediaType',
+        "$ref": "#/definitions/mediaType",
     }
 
 
 class Link(HasMediaType, Localized, Described, LinkedDataDumpable):
     url: str
     relationship: str | None
     label: str | None
@@ -275,69 +298,85 @@
         )
         self.url = url
         self.label = label
         self.relationship = relationship
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
-        dump['$schema'] = app.static_url_generator.generate('schema.json#/definitions/link', absolute=True)
-        dump['url'] = self.url
+        dump["$schema"] = app.static_url_generator.generate(
+            "schema.json#/definitions/link", absolute=True
+        )
+        dump["url"] = self.url
         if self.label is not None:
-            dump['label'] = self.label
+            dump["label"] = self.label
         if self.relationship is not None:
-            dump['relationship'] = self.relationship
+            dump["relationship"] = self.relationship
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        schema['type'] = 'object'
-        schema['additionalProperties'] = False
+        schema["type"] = "object"
+        schema["additionalProperties"] = False
         add_json_ld(schema)
-        add_property(schema, '$schema', ref_json_schema(schema))
-        add_property(schema, 'label', {
-            'type': 'string',
-            'description': 'The human-readable label, or link text.'
-        }, False)
-        add_property(schema, 'url', {
-            'type': 'string',
-            'format': 'uri',
-            'description': 'The full URL to the other resource.'
-        })
-        add_property(schema, 'relationship', {
-            'type': 'string',
-            'description': 'The relationship between this resource and the link target (https://en.wikipedia.org/wiki/Link_relation).'
-        }, False)
+        add_property(schema, "$schema", ref_json_schema(schema))
+        add_property(
+            schema,
+            "label",
+            {
+                "type": "string",
+                "description": "The human-readable label, or link text.",
+            },
+            False,
+        )
+        add_property(
+            schema,
+            "url",
+            {
+                "type": "string",
+                "format": "uri",
+                "description": "The full URL to the other resource.",
+            },
+        )
+        add_property(
+            schema,
+            "relationship",
+            {
+                "type": "string",
+                "description": "The relationship between this resource and the link target (https://en.wikipedia.org/wiki/Link_relation).",
+            },
+            False,
+        )
         return schema
 
 
 async def ref_link(root_schema: DictDump[Dump], app: App) -> DictDump[Dump]:
     """
     Reference the Link schema.
     """
-    definitions = dump_default(root_schema, 'definitions', dict)
-    if 'link' not in definitions:
-        definitions['link'] = await Link.linked_data_schema(app)
+    definitions = dump_default(root_schema, "definitions", dict)
+    if "link" not in definitions:
+        definitions["link"] = await Link.linked_data_schema(app)
     return {
-        '$ref': '#/definitions/link',
+        "$ref": "#/definitions/link",
     }
 
 
 async def ref_link_collection(root_schema: DictDump[Dump], app: App) -> DictDump[Dump]:
     """
     Reference the schema for a collection of Link instances.
     """
-    definitions = dump_default(root_schema, 'definitions', dict)
-    if 'linkCollection' not in definitions:
-        definitions['linkCollection'] = {
-            'type': 'array',
-            'items': await ref_link(root_schema, app),
+    definitions = dump_default(root_schema, "definitions", dict)
+    if "linkCollection" not in definitions:
+        definitions["linkCollection"] = {
+            "type": "array",
+            "items": await ref_link(root_schema, app),
         }
     return {
-        '$ref': '#/definitions/linkCollection',
+        "$ref": "#/definitions/linkCollection",
     }
 
 
 class HasLinks(LinkedDataDumpable):
     def __init__(
         self,
         *args: Any,
@@ -359,47 +398,58 @@
             *(self.links if is_public(self) else ()),
         )
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'links', await ref_link_collection(schema, app))
+        add_property(schema, "links", await ref_link_collection(schema, app))
         return schema
 
 
 class HasLinksEntity(HasLinks):
     async def dump_linked_data(  # type: ignore[misc]
         self: HasLinksEntity & Entity,
         app: App,
     ) -> DictDump[Dump]:
         dump: DictDump[Dump] = await super().dump_linked_data(app)  # type: ignore[misc]
 
         if not isinstance(self.id, GeneratedEntityId):
-            await dump_link(dump, app, Link(
-                app.static_url_generator.generate(f'/{camel_case_to_kebab_case(get_entity_type_name(self.type))}/{self.id}/index.json'),
-                relationship='canonical',
-                media_type=MediaType('application/ld+json'),
-            ))
+            await dump_link(
+                dump,
+                app,
+                Link(
+                    app.static_url_generator.generate(
+                        f"/{camel_case_to_kebab_case(get_entity_type_name(self.type))}/{self.id}/index.json"
+                    ),
+                    relationship="canonical",
+                    media_type=MediaType("application/ld+json"),
+                ),
+            )
             if is_public(self):
-                await dump_link(dump, app, *(
-                    Link(
-                        app.url_generator.generate(self, media_type='text/html', locale=locale),
-                        relationship='alternate',
-                        media_type=MediaType('text/html'),
-                        locale=locale,
-                    )
-                    for locale
-                    in app.project.configuration.locales
-                ))
+                await dump_link(
+                    dump,
+                    app,
+                    *(
+                        Link(
+                            app.url_generator.generate(
+                                self, media_type="text/html", locale=locale
+                            ),
+                            relationship="alternate",
+                            media_type=MediaType("text/html"),
+                            locale=locale,
+                        )
+                        for locale in app.project.configuration.locales
+                    ),
+                )
 
         return dump
 
 
-@many_to_one('entity', 'betty.model.ancestry.HasNotes', 'notes')
+@many_to_one("entity", "betty.model.ancestry.HasNotes", "notes")
 class Note(UserFacingEntity, HasPrivacy, HasLinksEntity, Entity):
     entity: HasNotes
 
     def __init__(
         self,
         text: str,
         *,
@@ -417,45 +467,43 @@
         )
         self._text = text
         if entity is not None:
             self.entity = entity
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._('Note')
+        return Str._("Note")
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._('Notes')
+        return Str._("Notes")
 
     @property
     def text(self) -> str:
         return self._text
 
     @property
     def label(self) -> Str:
         return Str.plain(self.text)
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
-        dump['@type'] = 'https://schema.org/Thing'
+        dump["@type"] = "https://schema.org/Thing"
         if self.public:
-            dump['text'] = self.text
+            dump["text"] = self.text
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'text', {
-            'type': 'string'
-        }, False)
+        add_property(schema, "text", {"type": "string"}, False)
         return schema
 
 
-@one_to_many('notes', 'betty.model.ancestry.Note', 'entity')
+@one_to_many("notes", "betty.model.ancestry.Note", "entity")
 class HasNotes(LinkedDataDumpable):
     def __init__(  # type: ignore[misc]
         self: HasNotes & Entity,
         *args: Any,
         notes: Iterable[Note] | None = None,
         **kwargs: Any,
     ):
@@ -476,32 +524,35 @@
 
     @notes.deleter
     def notes(self) -> None:
         pass
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
-        dump['notes'] = [
-            app.static_url_generator.generate(f'/note/{quote(note.id)}/index.json')
-            for note
-            in self.notes
+        dump["notes"] = [
+            app.static_url_generator.generate(f"/note/{quote(note.id)}/index.json")
+            for note in self.notes
             if not isinstance(note.id, GeneratedEntityId)
         ]
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'notes', {
-            '$ref': '#/definitions/entity/noteCollection',
-        })
+        add_property(
+            schema,
+            "notes",
+            {
+                "$ref": "#/definitions/entity/noteCollection",
+            },
+        )
         return schema
 
 
-@many_to_many('citations', 'betty.model.ancestry.Citation', 'facts')
+@many_to_many("citations", "betty.model.ancestry.Citation", "facts")
 class HasCitations(LinkedDataDumpable):
     def __init__(  # type: ignore[misc]
         self: HasCitations & Entity,
         *args: Any,
         citations: Iterable[Citation] | None = None,
         **kwargs: Any,
     ):
@@ -522,33 +573,47 @@
 
     @citations.deleter
     def citations(self) -> None:
         pass
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
-        dump['citations'] = [
-            app.static_url_generator.generate(f'/citation/{quote(citation.id)}/index.json')
-            for citation
-            in self.citations
+        dump["citations"] = [
+            app.static_url_generator.generate(
+                f"/citation/{quote(citation.id)}/index.json"
+            )
+            for citation in self.citations
             if not isinstance(citation.id, GeneratedEntityId)
         ]
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'citations', {
-            '$ref': '#/definitions/entity/citationCollection',
-        })
+        add_property(
+            schema,
+            "citations",
+            {
+                "$ref": "#/definitions/entity/citationCollection",
+            },
+        )
         return schema
 
 
-@many_to_many('entities', 'betty.model.ancestry.HasFiles', 'files')
-class File(Described, HasPrivacy, HasLinksEntity, HasMediaType, HasNotes, HasCitations, UserFacingEntity, Entity):
+@many_to_many("entities", "betty.model.ancestry.HasFiles", "files")
+class File(
+    Described,
+    HasPrivacy,
+    HasLinksEntity,
+    HasMediaType,
+    HasNotes,
+    HasCitations,
+    UserFacingEntity,
+    Entity,
+):
     def __init__(
         self,
         path: Path,
         *,
         id: str | None = None,
         media_type: MediaType | None = None,
         description: str | None = None,
@@ -582,52 +647,51 @@
 
     @entities.deleter
     def entities(self) -> None:
         pass
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._('File')
+        return Str._("File")
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._('Files')
+        return Str._("Files")
 
     @property
     def path(self) -> Path:
         return self._path
 
     @property
     def label(self) -> Str:
         return Str.plain(self.description) if self.description else super().label
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
-        dump['entities'] = [
-            app.static_url_generator.generate(f'/{camel_case_to_kebab_case(get_entity_type_name(entity))}/{quote(entity.id)}/index.json')
-            for entity
-            in self.entities
+        dump["entities"] = [
+            app.static_url_generator.generate(
+                f"/{camel_case_to_kebab_case(get_entity_type_name(entity))}/{quote(entity.id)}/index.json"
+            )
+            for entity in self.entities
             if not isinstance(entity.id, GeneratedEntityId)
         ]
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'entities', {
-            'type': 'array',
-            'items': {
-                'type': 'string',
-                'format': 'uri'
-            }
-        })
+        add_property(
+            schema,
+            "entities",
+            {"type": "array", "items": {"type": "string", "format": "uri"}},
+        )
         return schema
 
 
-@many_to_many('files', 'betty.model.ancestry.File', 'entities')
+@many_to_many("files", "betty.model.ancestry.File", "entities")
 class HasFiles:
     def __init__(  # type: ignore[misc]
         self: HasFiles & Entity,
         *args: Any,
         files: Iterable[File] | None = None,
         **kwargs: Any,
     ):
@@ -651,18 +715,20 @@
         pass
 
     @property
     def associated_files(self) -> Iterable[File]:
         return self.files
 
 
-@many_to_one('contained_by', 'betty.model.ancestry.Source', 'contains')
-@one_to_many('contains', 'betty.model.ancestry.Source', 'contained_by')
-@one_to_many('citations', 'betty.model.ancestry.Citation', 'source')
-class Source(Dated, HasFiles, HasNotes, HasLinksEntity, HasPrivacy, UserFacingEntity, Entity):
+@many_to_one("contained_by", "betty.model.ancestry.Source", "contains")
+@one_to_many("contains", "betty.model.ancestry.Source", "contained_by")
+@one_to_many("citations", "betty.model.ancestry.Citation", "source")
+class Source(
+    Dated, HasFiles, HasNotes, HasLinksEntity, HasPrivacy, UserFacingEntity, Entity
+):
     contained_by: Source | None
 
     def __init__(
         self,
         name: str | None = None,
         *,
         id: str | None = None,
@@ -724,99 +790,135 @@
 
     @citations.deleter
     def citations(self) -> None:
         pass
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._('Source')
+        return Str._("Source")
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._('Sources')
+        return Str._("Sources")
 
     @property
     def label(self) -> Str:
         return Str.plain(self.name) if self.name else super().label
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
-        dump['@type'] = 'https://schema.org/Thing'
-        dump['contains'] = [
-            app.static_url_generator.generate(f'/source/{quote(contained.id)}/index.json')
-            for contained
-            in self.contains
+        dump["@type"] = "https://schema.org/Thing"
+        dump["contains"] = [
+            app.static_url_generator.generate(
+                f"/source/{quote(contained.id)}/index.json"
+            )
+            for contained in self.contains
             if not isinstance(contained.id, GeneratedEntityId)
         ]
-        dump['citations'] = [
-            app.static_url_generator.generate(f'/citation/{quote(citation.id)}/index.json')
-            for citation
-            in self.citations
+        dump["citations"] = [
+            app.static_url_generator.generate(
+                f"/citation/{quote(citation.id)}/index.json"
+            )
+            for citation in self.citations
             if not isinstance(citation.id, GeneratedEntityId)
         ]
-        if self.contained_by is not None and not isinstance(self.contained_by.id, GeneratedEntityId):
-            dump['containedBy'] = app.static_url_generator.generate(f'/source/{quote(self.contained_by.id)}/index.json')
+        if self.contained_by is not None and not isinstance(
+            self.contained_by.id, GeneratedEntityId
+        ):
+            dump["containedBy"] = app.static_url_generator.generate(
+                f"/source/{quote(self.contained_by.id)}/index.json"
+            )
         if self.public:
             if self.name is not None:
-                dump_context(dump, name='name')
-                dump['name'] = self.name
+                dump_context(dump, name="name")
+                dump["name"] = self.name
             if self.author is not None:
-                dump['author'] = self.author
+                dump["author"] = self.author
             if self.publisher is not None:
-                dump['publisher'] = self.publisher
+                dump["publisher"] = self.publisher
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'name', {
-            'type': 'string',
-        }, False)
-        add_property(schema, 'author', {
-            'type': 'string',
-        }, False)
-        add_property(schema, 'publisher', {
-            'type': 'string',
-        }, False)
-        add_property(schema, 'contains', {
-            'type': 'array',
-            'items': {
-                'type': 'string',
-                'format': 'uri',
-            },
-        })
-        add_property(schema, 'citations', {
-            '$ref': '#/definitions/entity/citationCollection',
-        })
-        add_property(schema, 'containedBy', {
-            'type': 'string',
-            'format': 'uri',
-        }, False)
+        add_property(
+            schema,
+            "name",
+            {
+                "type": "string",
+            },
+            False,
+        )
+        add_property(
+            schema,
+            "author",
+            {
+                "type": "string",
+            },
+            False,
+        )
+        add_property(
+            schema,
+            "publisher",
+            {
+                "type": "string",
+            },
+            False,
+        )
+        add_property(
+            schema,
+            "contains",
+            {
+                "type": "array",
+                "items": {
+                    "type": "string",
+                    "format": "uri",
+                },
+            },
+        )
+        add_property(
+            schema,
+            "citations",
+            {
+                "$ref": "#/definitions/entity/citationCollection",
+            },
+        )
+        add_property(
+            schema,
+            "containedBy",
+            {
+                "type": "string",
+                "format": "uri",
+            },
+            False,
+        )
         return schema
 
 
-@deprecated(f'This class is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. No direct replacement is available. Instead, set the privacy for {Source} entities accordingly.')
+@deprecated(
+    f"This class is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. No direct replacement is available. Instead, set the privacy for {Source} entities accordingly."
+)
 class AnonymousSource(Source):
     @property  # type: ignore[override]
     def name(self) -> str:
-        return 'private'
+        return "private"
 
     @name.setter
     def name(self, _) -> None:
         # This is a no-op as the name is 'hardcoded'.
         pass
 
     @name.deleter
     def name(self) -> None:
         # This is a no-op as the name is 'hardcoded'.
         pass
 
 
-@many_to_many('facts', 'betty.model.ancestry.HasCitations', 'citations')
-@many_to_one('source', 'betty.model.ancestry.Source', 'citations')
+@many_to_many("facts", "betty.model.ancestry.HasCitations", "citations")
+@many_to_one("source", "betty.model.ancestry.Source", "citations")
 class Citation(Dated, HasFiles, HasPrivacy, HasLinksEntity, UserFacingEntity, Entity):
     def __init__(
         self,
         *,
         id: str | None = None,
         facts: Iterable[HasCitations] | None = None,
         source: Source | None = None,
@@ -856,55 +958,57 @@
 
     @facts.deleter
     def facts(self) -> None:
         pass
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._('Citation')
+        return Str._("Citation")
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._('Citations')
+        return Str._("Citations")
 
     @property
     def label(self) -> Str:
-        return self.location or Str.plain('')
+        return self.location or Str.plain("")
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
-        dump['@type'] = 'https://schema.org/Thing'
-        dump['facts'] = [
-            app.static_url_generator.generate(f'/{camel_case_to_kebab_case(get_entity_type_name(fact))}/{quote(fact.id)}/index.json')
-            for fact
-            in self.facts
+        dump["@type"] = "https://schema.org/Thing"
+        dump["facts"] = [
+            app.static_url_generator.generate(
+                f"/{camel_case_to_kebab_case(get_entity_type_name(fact))}/{quote(fact.id)}/index.json"
+            )
+            for fact in self.facts
             if not isinstance(fact.id, GeneratedEntityId)
         ]
-        if self.source is not None and not isinstance(self.source.id, GeneratedEntityId):
-            dump['source'] = app.static_url_generator.generate(f'/source/{quote(self.source.id)}/index.json')
+        if self.source is not None and not isinstance(
+            self.source.id, GeneratedEntityId
+        ):
+            dump["source"] = app.static_url_generator.generate(
+                f"/source/{quote(self.source.id)}/index.json"
+            )
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'source', {
-            'type': 'string',
-            'format': 'uri'
-        }, False)
-        add_property(schema, 'facts', {
-            'type': 'array',
-            'items': {
-                'type': 'string',
-                'format': 'uri'
-            }
-        })
+        add_property(schema, "source", {"type": "string", "format": "uri"}, False)
+        add_property(
+            schema,
+            "facts",
+            {"type": "array", "items": {"type": "string", "format": "uri"}},
+        )
         return schema
 
 
-@deprecated(f'This class is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. No direct replacement is available. Instead, set the privacy for {Citation} entities accordingly.')
+@deprecated(
+    f"This class is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. No direct replacement is available. Instead, set the privacy for {Citation} entities accordingly."
+)
 class AnonymousCitation(Citation):
     @property  # type: ignore[override]
     def location(self) -> Str:
         return Str._("private (in order to protect people's privacy)")
 
     @location.setter
     def location(self, _) -> None:
@@ -945,33 +1049,31 @@
 
     @property
     def name(self) -> str:
         return self._name
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
-        dump['name'] = self.name
+        dump["name"] = self.name
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'name', {
-            'type': 'string'
-        })
+        add_property(schema, "name", {"type": "string"})
         return schema
 
 
 @many_to_one_to_many(
-    'betty.model.ancestry.Place',
-    'enclosed_by',
-    'encloses',
-    'enclosed_by',
-    'betty.model.ancestry.Place',
-    'encloses',
+    "betty.model.ancestry.Place",
+    "enclosed_by",
+    "encloses",
+    "enclosed_by",
+    "betty.model.ancestry.Place",
+    "encloses",
 )
 class Enclosure(Dated, HasCitations, Entity):
     encloses: Place | None
     enclosed_by: Place | None
 
     def __init__(
         self,
@@ -980,24 +1082,24 @@
     ):
         super().__init__()
         self.encloses = encloses
         self.enclosed_by = enclosed_by
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._('Enclosure')
+        return Str._("Enclosure")
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._('Enclosures')
+        return Str._("Enclosures")
 
 
-@one_to_many('events', 'betty.model.ancestry.Event', 'place')
-@one_to_many('enclosed_by', 'betty.model.ancestry.Enclosure', 'encloses')
-@one_to_many('encloses', 'betty.model.ancestry.Enclosure', 'enclosed_by')
+@one_to_many("events", "betty.model.ancestry.Event", "place")
+@one_to_many("enclosed_by", "betty.model.ancestry.Enclosure", "encloses")
+@one_to_many("encloses", "betty.model.ancestry.Enclosure", "enclosed_by")
 class Place(HasLinksEntity, HasFiles, HasNotes, HasPrivacy, UserFacingEntity, Entity):
     def __init__(
         self,
         *,
         id: str | None = None,
         names: list[PlaceName] | None = None,
         events: Iterable[Event] | None = None,
@@ -1061,19 +1163,19 @@
 
     @events.deleter
     def events(self) -> None:
         pass
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._('Place')
+        return Str._("Place")
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._('Places')
+        return Str._("Places")
 
     @property
     def names(self) -> list[PlaceName]:
         return self._names
 
     @property
     def coordinates(self) -> Point | None:
@@ -1096,87 +1198,91 @@
         for event in self.events:
             yield from event.files
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
         dump_context(
             dump,
-            names='name',
-            events='event',
-            enclosedBy='containedInPlace',
-            encloses='containsPlace',
-        )
-        dump['@type'] = 'https://schema.org/Place'
-        dump['names'] = [
-            await name.dump_linked_data(app)
-            for name
-            in self.names
-        ]
-        dump['events'] = [
-            app.static_url_generator.generate(f'/event/{quote(event.id)}/index.json')
-            for event
-            in self.events
+            names="name",
+            events="event",
+            enclosedBy="containedInPlace",
+            encloses="containsPlace",
+        )
+        dump["@type"] = "https://schema.org/Place"
+        dump["names"] = [await name.dump_linked_data(app) for name in self.names]
+        dump["events"] = [
+            app.static_url_generator.generate(f"/event/{quote(event.id)}/index.json")
+            for event in self.events
             if not isinstance(event.id, GeneratedEntityId)
         ]
-        dump['enclosedBy'] = [
-            app.static_url_generator.generate(f'/place/{quote(enclosure.enclosed_by.id)}/index.json')
-            for enclosure
-            in self.enclosed_by
-            if enclosure.enclosed_by is not None and not isinstance(enclosure.enclosed_by.id, GeneratedEntityId)
+        dump["enclosedBy"] = [
+            app.static_url_generator.generate(
+                f"/place/{quote(enclosure.enclosed_by.id)}/index.json"
+            )
+            for enclosure in self.enclosed_by
+            if enclosure.enclosed_by is not None
+            and not isinstance(enclosure.enclosed_by.id, GeneratedEntityId)
         ]
-        dump['encloses'] = [
-            app.static_url_generator.generate(f'/place/{quote(enclosure.encloses.id)}/index.json')
-            for enclosure
-            in self.encloses
-            if enclosure.encloses is not None and not isinstance(enclosure.encloses.id, GeneratedEntityId)
+        dump["encloses"] = [
+            app.static_url_generator.generate(
+                f"/place/{quote(enclosure.encloses.id)}/index.json"
+            )
+            for enclosure in self.encloses
+            if enclosure.encloses is not None
+            and not isinstance(enclosure.encloses.id, GeneratedEntityId)
         ]
         if self.coordinates is not None:
-            dump['coordinates'] = {
-                '@type': 'https://schema.org/GeoCoordinates',
-                'latitude': self.coordinates.latitude,
-                'longitude': self.coordinates.longitude,
+            dump["coordinates"] = {
+                "@type": "https://schema.org/GeoCoordinates",
+                "latitude": self.coordinates.latitude,
+                "longitude": self.coordinates.longitude,
             }
-            dump_context(dump, coordinates='geo')
+            dump_context(dump, coordinates="geo")
             dump_context(
-                dump['coordinates'],  # type: ignore[arg-type]
-                latitude='latitude',
+                dump["coordinates"],  # type: ignore[arg-type]
+                latitude="latitude",
             )
             dump_context(
-                dump['coordinates'],  # type: ignore[arg-type]
-                longitude='longitude',
+                dump["coordinates"],  # type: ignore[arg-type]
+                longitude="longitude",
             )
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'names', {
-            'type': 'array',
-            'items': await PlaceName.linked_data_schema(app),
-        })
-        add_property(schema, 'enclosedBy', {
-            '$ref': '#/definitions/entity/placeCollection'
-        }, False)
-        add_property(schema, 'encloses', {
-            '$ref': '#/definitions/entity/placeCollection'
-        })
+        add_property(
+            schema,
+            "names",
+            {
+                "type": "array",
+                "items": await PlaceName.linked_data_schema(app),
+            },
+        )
+        add_property(
+            schema,
+            "enclosedBy",
+            {"$ref": "#/definitions/entity/placeCollection"},
+            False,
+        )
+        add_property(
+            schema, "encloses", {"$ref": "#/definitions/entity/placeCollection"}
+        )
         coordinate_schema: DictDump[Dump] = {
-            'type': 'number',
+            "type": "number",
         }
         coordinates_schema: DictDump[Dump] = {
-            'type': 'object',
-            'additionalProperties': False,
+            "type": "object",
+            "additionalProperties": False,
         }
-        add_property(coordinates_schema, 'latitude', coordinate_schema, False)
-        add_property(coordinates_schema, 'longitude', coordinate_schema, False)
+        add_property(coordinates_schema, "latitude", coordinate_schema, False)
+        add_property(coordinates_schema, "longitude", coordinate_schema, False)
         add_json_ld(coordinates_schema, schema)
-        add_property(schema, 'coordinates', coordinates_schema, False)
-        add_property(schema, 'events', {
-            '$ref': '#/definitions/entity/eventCollection'
-        })
+        add_property(schema, "coordinates", coordinates_schema, False)
+        add_property(schema, "events", {"$ref": "#/definitions/entity/eventCollection"})
         return schema
 
 
 class PresenceRole:
     @classmethod
     def name(cls) -> str:
         raise NotImplementedError(repr(cls))
@@ -1186,102 +1292,102 @@
         raise NotImplementedError(repr(self))
 
 
 def ref_role(root_schema: DictDump[Dump]) -> DictDump[Dump]:
     """
     Reference the PresenceRole schema.
     """
-    definitions = dump_default(root_schema, 'definitions', dict)
-    if 'role' not in definitions:
-        definitions['role'] = {
-            'type': 'string',
-            'description': "A person's role in an event.",
+    definitions = dump_default(root_schema, "definitions", dict)
+    if "role" not in definitions:
+        definitions["role"] = {
+            "type": "string",
+            "description": "A person's role in an event.",
         }
     return {
-        '$ref': '#/definitions/role',
+        "$ref": "#/definitions/role",
     }
 
 
 class Subject(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return 'subject'
+        return "subject"
 
     @property
     def label(self) -> Str:
-        return Str._('Subject')
+        return Str._("Subject")
 
 
 class Witness(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return 'witness'
+        return "witness"
 
     @property
     def label(self) -> Str:
-        return Str._('Witness')
+        return Str._("Witness")
 
 
 class Beneficiary(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return 'beneficiary'
+        return "beneficiary"
 
     @property
     def label(self) -> Str:
-        return Str._('Beneficiary')
+        return Str._("Beneficiary")
 
 
 class Attendee(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return 'attendee'
+        return "attendee"
 
     @property
     def label(self) -> Str:
-        return Str._('Attendee')
+        return Str._("Attendee")
 
 
 class Speaker(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return 'speaker'
+        return "speaker"
 
     @property
     def label(self) -> Str:
-        return Str._('Speaker')
+        return Str._("Speaker")
 
 
 class Celebrant(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return 'celebrant'
+        return "celebrant"
 
     @property
     def label(self) -> Str:
-        return Str._('Celebrant')
+        return Str._("Celebrant")
 
 
 class Organizer(PresenceRole):
     @classmethod
     def name(cls) -> str:
-        return 'organizer'
+        return "organizer"
 
     @property
     def label(self) -> Str:
-        return Str._('Organizer')
+        return Str._("Organizer")
 
 
 @many_to_one_to_many(
-    'betty.model.ancestry.Person',
-    'presences',
-    'person',
-    'event',
-    'betty.model.ancestry.Event',
-    'presences',
+    "betty.model.ancestry.Person",
+    "presences",
+    "person",
+    "event",
+    "betty.model.ancestry.Event",
+    "presences",
 )
 class Presence(HasPrivacy, Entity):
     person: Person | None
     event: Event | None
     role: PresenceRole
 
     def __init__(
@@ -1293,39 +1399,49 @@
         super().__init__(None)
         self.person = person
         self.role = role
         self.event = event
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._('Presence')
+        return Str._("Presence")
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._('Presences')
+        return Str._("Presences")
 
     @property
     def label(self) -> Str:
         return Str._(
-            'Presence of {person} at {event}',
-            person=self.person.label if self.person else Str._('Unknown'),
-            event=self.event.label if self.event else Str._('Unknown'),
+            "Presence of {person} at {event}",
+            person=self.person.label if self.person else Str._("Unknown"),
+            event=self.event.label if self.event else Str._("Unknown"),
         )
 
     def _get_effective_privacy(self) -> Privacy:
         return merge_privacies(
             super()._get_effective_privacy(),
             self.person,
             self.event,
         )
 
 
-@many_to_one('place', 'betty.model.ancestry.Place', 'events')
-@one_to_many('presences', 'betty.model.ancestry.Presence', 'event')
-class Event(Dated, HasFiles, HasCitations, HasNotes, Described, HasPrivacy, HasLinksEntity, UserFacingEntity, Entity):
+@many_to_one("place", "betty.model.ancestry.Place", "events")
+@one_to_many("presences", "betty.model.ancestry.Presence", "event")
+class Event(
+    Dated,
+    HasFiles,
+    HasCitations,
+    HasNotes,
+    Described,
+    HasPrivacy,
+    HasLinksEntity,
+    UserFacingEntity,
+    Entity,
+):
     place: Place | None
 
     def __init__(
         self,
         *,
         id: str | None = None,
         event_type: type[EventType] = UnknownEventType,
@@ -1353,36 +1469,44 @@
         self._event_type = event_type
         if place is not None:
             self.place = place
 
     @property
     def label(self) -> Str:
         format_kwargs: dict[str, str | Localizable] = {
-            'event_type': self._event_type.label(),
+            "event_type": self._event_type.label(),
         }
         subjects = [
             presence.person
-            for presence
-            in self.presences
-            if presence.public and isinstance(presence.role, Subject) and presence.person is not None and presence.person.public
+            for presence in self.presences
+            if presence.public
+            and isinstance(presence.role, Subject)
+            and presence.person is not None
+            and presence.person.public
         ]
         if subjects:
-            format_kwargs['subjects'] = Str.call(lambda localizer: ', '.join(person.label.localize(localizer) for person in subjects))
+            format_kwargs["subjects"] = Str.call(
+                lambda localizer: ", ".join(
+                    person.label.localize(localizer) for person in subjects
+                )
+            )
         if self.description is not None:
-            format_kwargs['event_description'] = self.description
+            format_kwargs["event_description"] = self.description
 
         if subjects:
             if self.description is None:
-                return Str._('{event_type} of {subjects}', **format_kwargs)
+                return Str._("{event_type} of {subjects}", **format_kwargs)
             else:
-                return Str._('{event_type} ({event_description}) of {subjects}', **format_kwargs)
+                return Str._(
+                    "{event_type} ({event_description}) of {subjects}", **format_kwargs
+                )
         if self.description is None:
-            return Str._('{event_type}', **format_kwargs)
+            return Str._("{event_type}", **format_kwargs)
         else:
-            return Str._('{event_type} ({event_description})', **format_kwargs)
+            return Str._("{event_type} ({event_description})", **format_kwargs)
 
     @recursive_repr()
     def __repr__(self) -> str:
         return repr_instance(self, id=self._id, type=self._event_type)
 
     @property
     def presences(self) -> EntityCollection[Presence]:  # type: ignore[empty-body]
@@ -1394,104 +1518,139 @@
 
     @presences.deleter
     def presences(self) -> None:
         pass
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._('Event')
+        return Str._("Event")
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._('Events')
+        return Str._("Events")
 
     @property
     def event_type(self) -> type[EventType]:
         return self._event_type
 
     @property
     def associated_files(self) -> Iterable[File]:
         files = [
             *self.files,
-            *[file for citation in self.citations for file in citation.associated_files],
+            *[
+                file
+                for citation in self.citations
+                for file in citation.associated_files
+            ],
         ]
         # Preserve the original order.
         seen = set()
         for file in files:
             if file in seen:
                 continue
             seen.add(file)
             yield file
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
-        dump_context(dump, presences='performer')
-        dump['@type'] = 'https://schema.org/Event'
-        dump['type'] = self.event_type.name()
-        dump['eventAttendanceMode'] = 'https://schema.org/OfflineEventAttendanceMode'
-        dump['eventStatus'] = 'https://schema.org/EventScheduled'
-        dump['presences'] = presences = []
+        dump_context(dump, presences="performer")
+        dump["@type"] = "https://schema.org/Event"
+        dump["type"] = self.event_type.name()
+        dump["eventAttendanceMode"] = "https://schema.org/OfflineEventAttendanceMode"
+        dump["eventStatus"] = "https://schema.org/EventScheduled"
+        dump["presences"] = presences = []
         if self.date is not None and self.public:
             await self.date.datey_dump_linked_data(
-                dump['date'],  # type: ignore[arg-type]
-                'startDate',
-                'endDate',
+                dump["date"],  # type: ignore[arg-type]
+                "startDate",
+                "endDate",
             )
         for presence in self.presences:
-            if presence.person and not isinstance(presence.person.id, GeneratedEntityId):
+            if presence.person and not isinstance(
+                presence.person.id, GeneratedEntityId
+            ):
                 presences.append(self._dump_event_presence(presence, app))
         if self.place is not None and not isinstance(self.place.id, GeneratedEntityId):
-            dump['place'] = app.static_url_generator.generate(f'/place/{quote(self.place.id)}/index.json')
-            dump_context(dump, place='location')
+            dump["place"] = app.static_url_generator.generate(
+                f"/place/{quote(self.place.id)}/index.json"
+            )
+            dump_context(dump, place="location")
         return dump
 
     def _dump_event_presence(self, presence: Presence, app: App) -> DictDump[Dump]:
         assert presence.person
         dump: DictDump[Dump] = {
-            '@type': 'https://schema.org/Person',
-            'person': app.static_url_generator.generate(f'/person/{quote(presence.person.id)}/index.json'),
+            "@type": "https://schema.org/Person",
+            "person": app.static_url_generator.generate(
+                f"/person/{quote(presence.person.id)}/index.json"
+            ),
         }
         if presence.public:
-            dump['role'] = presence.role.name()
+            dump["role"] = presence.role.name()
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'type', {
-            'type': 'string',
-        })
-        add_property(schema, 'place', {
-            'type': 'string',
-            'format': 'uri',
-        }, False)
+        add_property(
+            schema,
+            "type",
+            {
+                "type": "string",
+            },
+        )
+        add_property(
+            schema,
+            "place",
+            {
+                "type": "string",
+                "format": "uri",
+            },
+            False,
+        )
         presence_schema: DictDump[Dump] = {
-            'type': 'object',
-            'additionalProperties': False,
+            "type": "object",
+            "additionalProperties": False,
         }
-        add_property(presence_schema, 'role', ref_role(schema), False)
-        add_property(presence_schema, 'person', {
-            'type': 'string',
-            'format': 'uri',
-        })
+        add_property(presence_schema, "role", ref_role(schema), False)
+        add_property(
+            presence_schema,
+            "person",
+            {
+                "type": "string",
+                "format": "uri",
+            },
+        )
         add_json_ld(presence_schema, schema)
-        add_property(schema, 'presences', {
-            'type': 'array',
-            'items': presence_schema,
-        })
-        add_property(schema, 'eventStatus', {
-            'type': 'string',
-        })
-        add_property(schema, 'eventAttendanceMode', {
-            'type': 'string',
-        })
+        add_property(
+            schema,
+            "presences",
+            {
+                "type": "array",
+                "items": presence_schema,
+            },
+        )
+        add_property(
+            schema,
+            "eventStatus",
+            {
+                "type": "string",
+            },
+        )
+        add_property(
+            schema,
+            "eventAttendanceMode",
+            {
+                "type": "string",
+            },
+        )
         return schema
 
 
-@many_to_one('person', 'betty.model.ancestry.Person', 'names')
+@many_to_one("person", "betty.model.ancestry.Person", "names")
 class PersonName(Localized, HasCitations, HasPrivacy, Entity):
     person: Person | None
 
     def __init__(
         self,
         *,
         id: str | None = None,
@@ -1500,15 +1659,17 @@
         affiliation: str | None = None,
         privacy: Privacy | None = None,
         public: bool | None = None,
         private: bool | None = None,
         locale: str | None = None,
     ):
         if not individual and not affiliation:
-            raise ValueError('The individual and affiliation names must not both be empty.')
+            raise ValueError(
+                "The individual and affiliation names must not both be empty."
+            )
         super().__init__(
             id,
             privacy=privacy,
             public=public,
             private=private,
             locale=locale,
         )
@@ -1521,68 +1682,88 @@
     def _get_effective_privacy(self) -> Privacy:
         privacy = super()._get_effective_privacy()
         if self.person:
             return merge_privacies(privacy, self.person.privacy)
         return privacy
 
     def __repr__(self) -> str:
-        return repr_instance(self, id=self.id, individual=self.individual, affiliation=self.affiliation)
+        return repr_instance(
+            self, id=self.id, individual=self.individual, affiliation=self.affiliation
+        )
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._('Person name')
+        return Str._("Person name")
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._('Person names')
+        return Str._("Person names")
 
     @property
     def individual(self) -> str | None:
         return self._individual
 
     @property
     def affiliation(self) -> str | None:
         return self._affiliation
 
     @property
     def label(self) -> Str:
         return Str._(
-            '{individual_name} {affiliation_name}',
-            individual_name='…' if not self.individual else self.individual,
-            affiliation_name='…' if not self.affiliation else self.affiliation,
+            "{individual_name} {affiliation_name}",
+            individual_name="…" if not self.individual else self.individual,
+            affiliation_name="…" if not self.affiliation else self.affiliation,
         )
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
         if self.public:
             if self.individual is not None:
-                dump_context(dump, individual='givenName')
-                dump['individual'] = self.individual
+                dump_context(dump, individual="givenName")
+                dump["individual"] = self.individual
             if self.affiliation is not None:
-                dump_context(dump, affiliation='familyName')
-                dump['affiliation'] = self.affiliation
+                dump_context(dump, affiliation="familyName")
+                dump["affiliation"] = self.affiliation
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'individual', {
-            'type': 'string',
-        }, False)
-        add_property(schema, 'affiliation', {
-            'type': 'string',
-        }, False)
+        add_property(
+            schema,
+            "individual",
+            {
+                "type": "string",
+            },
+            False,
+        )
+        add_property(
+            schema,
+            "affiliation",
+            {
+                "type": "string",
+            },
+            False,
+        )
         return schema
 
 
-@many_to_many('parents', 'betty.model.ancestry.Person', 'children')
-@many_to_many('children', 'betty.model.ancestry.Person', 'parents')
-@one_to_many('presences', 'betty.model.ancestry.Presence', 'person')
-@one_to_many('names', 'betty.model.ancestry.PersonName', 'person')
-class Person(HasFiles, HasCitations, HasNotes, HasLinksEntity, HasPrivacy, UserFacingEntity, Entity):
+@many_to_many("parents", "betty.model.ancestry.Person", "children")
+@many_to_many("children", "betty.model.ancestry.Person", "parents")
+@one_to_many("presences", "betty.model.ancestry.Presence", "person")
+@one_to_many("names", "betty.model.ancestry.PersonName", "person")
+class Person(
+    HasFiles,
+    HasCitations,
+    HasNotes,
+    HasLinksEntity,
+    HasPrivacy,
+    UserFacingEntity,
+    Entity,
+):
     def __init__(
         self,
         *,
         id: str | None = None,
         files: Iterable[File] | None = None,
         citations: Iterable[Citation] | None = None,
         links: MutableSequence[Link] | None = None,
@@ -1660,19 +1841,19 @@
 
     @names.deleter
     def names(self) -> None:
         pass
 
     @classmethod
     def entity_type_label(cls) -> Str:
-        return Str._('Person')
+        return Str._("Person")
 
     @classmethod
     def entity_type_label_plural(cls) -> Str:
-        return Str._('People')
+        return Str._("People")
 
     @property
     def siblings(self) -> list[Person]:
         siblings = []
         for parent in self.parents:
             for sibling in parent.children:
                 if sibling != self and sibling not in siblings:
@@ -1681,29 +1862,24 @@
 
     @property
     def associated_files(self) -> Iterable[File]:
         files = [
             *self.files,
             *[
                 file
-                for name
-                in self.names
-                for citation
-                in name.citations
-                for file
-                in citation.associated_files
+                for name in self.names
+                for citation in name.citations
+                for file in citation.associated_files
             ],
             *[
                 file
-                for presence
-                in self.presences
+                for presence in self.presences
                 if presence.event is not None
-                for file
-                in presence.event.associated_files
-            ]
+                for file in presence.event.associated_files
+            ],
         ]
         # Preserve the original order.
         seen = set()
         for file in files:
             if file in seen:
                 continue
             seen.add(file)
@@ -1716,95 +1892,115 @@
                 return name.label
         return super().label
 
     async def dump_linked_data(self, app: App) -> DictDump[Dump]:
         dump = await super().dump_linked_data(app)
         dump_context(
             dump,
-            names='name',
-            parents='parent',
-            children='child',
-            siblings='sibling',
-        )
-        dump['@type'] = 'https://schema.org/Person'
-        dump['parents'] = [
-            app.static_url_generator.generate(f'/person/{quote(parent.id)}/index.json')
-            for parent
-            in self.parents
+            names="name",
+            parents="parent",
+            children="child",
+            siblings="sibling",
+        )
+        dump["@type"] = "https://schema.org/Person"
+        dump["parents"] = [
+            app.static_url_generator.generate(f"/person/{quote(parent.id)}/index.json")
+            for parent in self.parents
             if not isinstance(parent.id, GeneratedEntityId)
         ]
-        dump['children'] = [
-            app.static_url_generator.generate(f'/person/{quote(child.id)}/index.json')
-            for child
-            in self.children
+        dump["children"] = [
+            app.static_url_generator.generate(f"/person/{quote(child.id)}/index.json")
+            for child in self.children
             if not isinstance(child.id, GeneratedEntityId)
         ]
-        dump['siblings'] = [
-            app.static_url_generator.generate(f'/person/{quote(sibling.id)}/index.json')
-            for sibling
-            in self.siblings
+        dump["siblings"] = [
+            app.static_url_generator.generate(f"/person/{quote(sibling.id)}/index.json")
+            for sibling in self.siblings
             if not isinstance(sibling.id, GeneratedEntityId)
         ]
-        dump['presences'] = [
+        dump["presences"] = [
             self._dump_person_presence(presence, app)
-            for presence
-            in self.presences
-            if presence.event is not None and not isinstance(presence.event.id, GeneratedEntityId)
+            for presence in self.presences
+            if presence.event is not None
+            and not isinstance(presence.event.id, GeneratedEntityId)
         ]
         if self.public:
-            dump['names'] = [
-                await name.dump_linked_data(app)
-                for name
-                in self.names
-                if name.public
+            dump["names"] = [
+                await name.dump_linked_data(app) for name in self.names if name.public
             ]
         else:
-            dump['names'] = []
+            dump["names"] = []
         return dump
 
     def _dump_person_presence(self, presence: Presence, app: App) -> DictDump[Dump]:
         assert presence.event
         dump: DictDump[Dump] = {
-            'event': app.static_url_generator.generate(f'/event/{quote(presence.event.id)}/index.json'),
+            "event": app.static_url_generator.generate(
+                f"/event/{quote(presence.event.id)}/index.json"
+            ),
         }
-        dump_context(dump, event='performerIn')
+        dump_context(dump, event="performerIn")
         if presence.public:
-            dump['role'] = presence.role.name()
+            dump["role"] = presence.role.name()
         return dump
 
     @classmethod
     async def linked_data_schema(cls, app: App) -> DictDump[Dump]:
         schema = await super().linked_data_schema(app)
-        add_property(schema, 'names', {
-            'type': 'array',
-            'items': await PersonName.linked_data_schema(app),
-        })
-        add_property(schema, 'parents', {
-            '$ref': '#/definitions/entity/personCollection',
-        })
-        add_property(schema, 'children', {
-            '$ref': '#/definitions/entity/personCollection',
-        })
-        add_property(schema, 'siblings', {
-            '$ref': '#/definitions/entity/personCollection',
-        })
+        add_property(
+            schema,
+            "names",
+            {
+                "type": "array",
+                "items": await PersonName.linked_data_schema(app),
+            },
+        )
+        add_property(
+            schema,
+            "parents",
+            {
+                "$ref": "#/definitions/entity/personCollection",
+            },
+        )
+        add_property(
+            schema,
+            "children",
+            {
+                "$ref": "#/definitions/entity/personCollection",
+            },
+        )
+        add_property(
+            schema,
+            "siblings",
+            {
+                "$ref": "#/definitions/entity/personCollection",
+            },
+        )
         presence_schema: DictDump[Dump] = {
-            'type': 'object',
-            'additionalProperties': False,
+            "type": "object",
+            "additionalProperties": False,
         }
-        add_property(presence_schema, 'role', ref_role(schema), False)
-        add_property(presence_schema, 'event', {
-            'type': 'string',
-            'format': 'uri',
-        })
+        add_property(presence_schema, "role", ref_role(schema), False)
+        add_property(
+            presence_schema,
+            "event",
+            {
+                "type": "string",
+                "format": "uri",
+            },
+        )
         add_json_ld(presence_schema, schema)
-        add_property(schema, 'presences', {
-            'type': 'array',
-            'items': presence_schema,
-        })
+        add_property(
+            schema,
+            "presences",
+            {
+                "type": "array",
+                "items": presence_schema,
+            },
+        )
         return schema
 
 
 class Ancestry(MultipleTypesEntityCollection[Entity]):
     def __init__(self):
         super().__init__()
         self._check_graph = True
@@ -1819,10 +2015,14 @@
     def _on_add(self, *entities: Entity) -> None:
         super()._on_add(*entities)
         if self._check_graph:
             self.add(*self._get_associates(*entities))
 
     def _get_associates(self, *entities: Entity) -> Iterable[Entity]:
         for entity in entities:
-            for association in EntityTypeAssociationRegistry.get_all_associations(entity):
-                for associate in EntityTypeAssociationRegistry.get_associates(entity, association):
+            for association in EntityTypeAssociationRegistry.get_all_associations(
+                entity
+            ):
+                for associate in EntityTypeAssociationRegistry.get_associates(
+                    entity, association
+                ):
                     yield associate
```

### Comparing `betty-0.3.3/betty/model/event_type.py` & `betty-0.3.4/betty/model/event_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide Betty's ancestry event types.
 """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from betty.locale import Str, DEFAULT_LOCALIZER
 
 if TYPE_CHECKING:
@@ -15,15 +16,15 @@
     @property
     def entity_types(self) -> set[type[EventType]]:
         raise NotImplementedError(repr(self))
 
 
 class EventType:
     def __new__(cls):
-        raise RuntimeError('Event types cannot be instantiated.')
+        raise RuntimeError("Event types cannot be instantiated.")
 
     @classmethod
     def name(cls) -> str:
         raise NotImplementedError(repr(cls))
 
     @classmethod
     def label(cls) -> Str:
@@ -37,19 +38,19 @@
     def comes_after(cls) -> set[type[EventType]]:
         return set()
 
 
 class UnknownEventType(EventType):
     @classmethod
     def name(cls) -> str:
-        return 'unknown'
+        return "unknown"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Unknown')
+        return Str._("Unknown")
 
 
 class DerivableEventType(EventType):
     pass
 
 
 class CreatableDerivableEventType(DerivableEventType):
@@ -87,260 +88,264 @@
     def comes_after(cls) -> set[type[EventType]]:
         return {Death}
 
 
 class Birth(CreatableDerivableEventType, StartOfLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'birth'
+        return "birth"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Birth')
+        return Str._("Birth")
 
     @classmethod
     def comes_before(cls) -> set[type[EventType]]:
         return {DuringLifeEventType}
 
 
 class Baptism(DuringLifeEventType, StartOfLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'baptism'
+        return "baptism"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Baptism')
+        return Str._("Baptism")
 
 
 class Adoption(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'adoption'
+        return "adoption"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Adoption')
+        return Str._("Adoption")
 
 
 class Death(CreatableDerivableEventType, EndOfLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'death'
+        return "death"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Death')
+        return Str._("Death")
 
     @classmethod
     def comes_after(cls) -> set[type[EventType]]:
         return {DuringLifeEventType}
 
     @classmethod
     def may_create(cls, person: Person, lifetime_threshold: int) -> bool:
         from betty.privatizer import Privatizer
 
-        return Privatizer(lifetime_threshold, localizer=DEFAULT_LOCALIZER).has_expired(person, 1)
+        return Privatizer(lifetime_threshold, localizer=DEFAULT_LOCALIZER).has_expired(
+            person, 1
+        )
 
 
-class FinalDispositionEventType(PostDeathEventType, DerivableEventType, EndOfLifeEventType):
+class FinalDispositionEventType(
+    PostDeathEventType, DerivableEventType, EndOfLifeEventType
+):
     pass
 
 
 class Funeral(FinalDispositionEventType):
     @classmethod
     def name(cls) -> str:
-        return 'funeral'
+        return "funeral"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Funeral')
+        return Str._("Funeral")
 
 
 class Cremation(FinalDispositionEventType):
     @classmethod
     def name(cls) -> str:
-        return 'cremation'
+        return "cremation"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Cremation')
+        return Str._("Cremation")
 
 
 class Burial(FinalDispositionEventType):
     @classmethod
     def name(cls) -> str:
-        return 'burial'
+        return "burial"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Burial')
+        return Str._("Burial")
 
 
 class Will(PostDeathEventType):
     @classmethod
     def name(cls) -> str:
-        return 'will'
+        return "will"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Will')
+        return Str._("Will")
 
 
 class Engagement(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'engagement'
+        return "engagement"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Engagement')
+        return Str._("Engagement")
 
     @classmethod
     def comes_before(cls) -> set[type[EventType]]:
         return {Marriage}
 
 
 class Marriage(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'marriage'
+        return "marriage"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Marriage')
+        return Str._("Marriage")
 
 
 class MarriageAnnouncement(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'marriage-announcement'
+        return "marriage-announcement"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Announcement of marriage')
+        return Str._("Announcement of marriage")
 
     @classmethod
     def comes_before(cls) -> set[type[EventType]]:
         return {Marriage}
 
 
 class Divorce(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'divorce'
+        return "divorce"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Divorce')
+        return Str._("Divorce")
 
     @classmethod
     def comes_after(cls) -> set[type[EventType]]:
         return {Marriage}
 
 
 class DivorceAnnouncement(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'divorce-announcement'
+        return "divorce-announcement"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Announcement of divorce')
+        return Str._("Announcement of divorce")
 
     @classmethod
     def comes_after(cls) -> set[type[EventType]]:
         return {Marriage}
 
     @classmethod
     def comes_before(cls) -> set[type[EventType]]:
         return {Divorce}
 
 
 class Residence(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'residence'
+        return "residence"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Residence')
+        return Str._("Residence")
 
 
 class Immigration(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'immigration'
+        return "immigration"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Immigration')
+        return Str._("Immigration")
 
 
 class Emigration(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'emigration'
+        return "emigration"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Emigration')
+        return Str._("Emigration")
 
 
 class Occupation(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'occupation'
+        return "occupation"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Occupation')
+        return Str._("Occupation")
 
 
 class Retirement(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'retirement'
+        return "retirement"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Retirement')
+        return Str._("Retirement")
 
 
 class Correspondence(EventType):
     @classmethod
     def name(cls) -> str:
-        return 'correspondence'
+        return "correspondence"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Correspondence')
+        return Str._("Correspondence")
 
 
 class Confirmation(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'confirmation'
+        return "confirmation"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Confirmation')
+        return Str._("Confirmation")
 
 
 class Missing(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'missing'
+        return "missing"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Missing')
+        return Str._("Missing")
 
 
 class Conference(DuringLifeEventType):
     @classmethod
     def name(cls) -> str:
-        return 'conference'
+        return "conference"
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Conference')
+        return Str._("Conference")
```

### Comparing `betty-0.3.3/betty/os.py` & `betty-0.3.4/betty/os.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide OS interaction utilities.
 """
+
 from __future__ import annotations
 
 import asyncio
 import shutil
 from contextlib import suppress
 from pathlib import Path
```

### Comparing `betty-0.3.3/betty/privatizer.py` & `betty-0.3.4/betty/privatizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 """
 Provide an API to determine if information should be kept private.
 """
+
 from __future__ import annotations
 
 import logging
 from contextlib import suppress
 from datetime import datetime
 from typing import Iterator, TypeAlias, Any
 
 from betty.functools import walk
 from betty.locale import DateRange, Date, Localizer
 from betty.model import Entity
-from betty.model.ancestry import Person, Event, HasFiles, HasCitations, HasNotes, Source, \
-    Presence, Privacy, HasPrivacy, Subject, Place
+from betty.model.ancestry import (
+    Person,
+    Event,
+    HasFiles,
+    HasCitations,
+    HasNotes,
+    Source,
+    Presence,
+    Privacy,
+    HasPrivacy,
+    Subject,
+    Place,
+)
 from betty.model.event_type import EndOfLifeEventType
 
 Expirable: TypeAlias = Person | Event | Date | None
 
 
 class Privatizer:
     def __init__(
@@ -112,15 +124,17 @@
             self._mark_private(enclosure.encloses, place)
             self.privatize(enclosure.encloses)
         for enclosure in place.enclosed_by:
             if not enclosure.enclosed_by:
                 continue
             self.privatize(enclosure.enclosed_by)
 
-    def _privatize_has_citations(self, has_citations: HasCitations & HasPrivacy) -> None:
+    def _privatize_has_citations(
+        self, has_citations: HasCitations & HasPrivacy
+    ) -> None:
         if not has_citations.private:
             return
 
         for citation in has_citations.citations:
             self._mark_private(citation, has_citations)
             self.privatize(citation)
 
@@ -147,27 +161,31 @@
         if not has_notes.private:
             return
 
         for note in has_notes.notes:
             self._mark_private(note, has_notes)
             self.privatize(note)
 
-    def _ancestors_by_generation(self, person: Person, generations_ago: int = 1) -> Iterator[tuple[Person, int]]:
+    def _ancestors_by_generation(
+        self, person: Person, generations_ago: int = 1
+    ) -> Iterator[tuple[Person, int]]:
         for parent in person.parents:
             yield parent, generations_ago
             yield from self._ancestors_by_generation(parent, generations_ago + 1)
 
     def _determine_person_privacy(self, person: Person) -> None:
         # Do not change existing explicit privacy declarations.
         if person.privacy is not Privacy.UNDETERMINED:
             return
 
         # A dead person is not private, regardless of when they died.
         for presence in person.presences:
-            if presence.event and issubclass(presence.event.event_type, EndOfLifeEventType):
+            if presence.event and issubclass(
+                presence.event.event_type, EndOfLifeEventType
+            ):
                 if presence.event.date is None:
                     person.public = True
                     return
                 if self.has_expired(presence.event, 0):
                     person.public = True
                     return
 
@@ -177,24 +195,28 @@
 
         for ancestor, generations_ago in self._ancestors_by_generation(person):
             if self.has_expired(ancestor, generations_ago + 1):
                 person.public = True
                 return
 
         # If any descendant has any expired event, the person is considered not private.
-        for descendant in walk(person, 'children'):
+        for descendant in walk(person, "children"):
             if self.has_expired(descendant, 1):
                 person.public = True
                 return
 
         person.private = True
-        logging.getLogger(__name__).debug(self._localizer._('Privatized person {privatized_person_id} ({privatized_person}) because they are likely still alive.').format(
-            privatized_person_id=person.id,
-            privatized_person=person.label.localize(self._localizer),
-        ))
+        logging.getLogger(__name__).debug(
+            self._localizer._(
+                "Privatized person {privatized_person_id} ({privatized_person}) because they are likely still alive."
+            ).format(
+                privatized_person_id=person.id,
+                privatized_person=person.label.localize(self._localizer),
+            )
+        )
 
     def _determine_place_privacy(self, place: Place) -> None:
         # Do not change existing explicit privacy declarations.
         if place.privacy is not Privacy.UNDETERMINED:
             return
 
         # If there are non-private events, we will not privatize the place.
@@ -206,18 +228,22 @@
         for enclosure in place.encloses:
             if not enclosure.encloses:
                 continue
             if not enclosure.encloses.private:
                 return
 
         place.private = True
-        logging.getLogger(__name__).debug(self._localizer._('Privatized place {privatized_place_id} ({privatized_place}) because it is not associated with any public information.').format(
-            privatized_place_id=place.id,
-            privatized_place=place.label.localize(self._localizer),
-        ))
+        logging.getLogger(__name__).debug(
+            self._localizer._(
+                "Privatized place {privatized_place_id} ({privatized_place}) because it is not associated with any public information."
+            ).format(
+                privatized_place_id=place.id,
+                privatized_place=place.label.localize(self._localizer),
+            )
+        )
 
     def has_expired(
         self,
         subject: Expirable,
         generations_ago: int = 0,
     ) -> bool:
         if isinstance(subject, Person):
@@ -229,15 +255,17 @@
         if isinstance(subject, Date):
             return self._date_has_expired(subject, generations_ago)
 
         return False
 
     def _person_has_expired(self, person: Person, generations_ago: int) -> bool:
         for presence in person.presences:
-            if presence.event is not None and self._event_has_expired(presence.event, generations_ago):
+            if presence.event is not None and self._event_has_expired(
+                presence.event, generations_ago
+            ):
                 return True
         return False
 
     def _event_has_expired(self, event: Event, generations_ago: int) -> bool:
         date = event.date
 
         if isinstance(date, DateRange):
@@ -252,27 +280,39 @@
         self,
         date: Date,
         generations_ago: int,
     ) -> bool:
         if not date.comparable:
             return False
 
-        return date <= Date(datetime.now().year - self._lifetime_threshold * generations_ago, datetime.now().month, datetime.now().day)
+        return date <= Date(
+            datetime.now().year - self._lifetime_threshold * generations_ago,
+            datetime.now().month,
+            datetime.now().day,
+        )
 
     def _mark_private(self, target: HasPrivacy, reason: Any) -> None:
         # Do not change existing explicit privacy declarations.
         if target.own_privacy is not Privacy.UNDETERMINED:
             return
 
         target.private = True
         with suppress(ValueError):
             self._seen.remove(target)
 
         if isinstance(target, Entity) and isinstance(reason, Entity):
-            logging.getLogger(__name__).debug(self._localizer._('Privatized {privatized_entity_type} {privatized_entity_id} ({privatized_entity}) because of {reason_entity_type} {reason_entity_id} ({reason_entity}).').format(
-                privatized_entity_type=target.entity_type_label().localize(self._localizer),
-                privatized_entity_id=target.id,
-                privatized_entity=target.label.localize(self._localizer),
-                reason_entity_type=reason.entity_type_label().localize(self._localizer),
-                reason_entity_id=reason.id,
-                reason_entity=reason.label.localize(self._localizer),
-            ))
+            logging.getLogger(__name__).debug(
+                self._localizer._(
+                    "Privatized {privatized_entity_type} {privatized_entity_id} ({privatized_entity}) because of {reason_entity_type} {reason_entity_id} ({reason_entity})."
+                ).format(
+                    privatized_entity_type=target.entity_type_label().localize(
+                        self._localizer
+                    ),
+                    privatized_entity_id=target.id,
+                    privatized_entity=target.label.localize(self._localizer),
+                    reason_entity_type=reason.entity_type_label().localize(
+                        self._localizer
+                    ),
+                    reason_entity_id=reason.id,
+                    reason_entity=reason.label.localize(self._localizer),
+                )
+            )
```

### Comparing `betty-0.3.3/betty/project.py` & `betty-0.3.4/betty/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,49 @@
 """
 Provide the project API.
 """
+
 from __future__ import annotations
 
-import hashlib
 from contextlib import suppress
 from pathlib import Path
 from reprlib import recursive_repr
 from typing import Any, Generic, final, Iterable, cast, Self
 from urllib.parse import urlparse
 
 from betty.app.extension import Extension, ConfigurableExtension
 from betty.classtools import repr_instance
-from betty.config import Configuration, Configurable, FileBasedConfiguration, ConfigurationMapping, \
-    ConfigurationSequence
+from betty.config import (
+    Configuration,
+    Configurable,
+    FileBasedConfiguration,
+    ConfigurationMapping,
+    ConfigurationSequence,
+)
+from betty.hashid import hashid
 from betty.locale import get_data, Str
 from betty.model import Entity, get_entity_type_name, UserFacingEntity, EntityT
 from betty.model.ancestry import Ancestry, Person, Event, Place, Source
-from betty.serde.dump import Dump, VoidableDump, void_none, minimize, Void, VoidableDictDump
-from betty.serde.load import AssertionFailed, Fields, Assertions, Assertion, RequiredField, OptionalField, \
-    Asserter
+from betty.serde.dump import (
+    Dump,
+    VoidableDump,
+    void_none,
+    minimize,
+    Void,
+    VoidableDictDump,
+)
+from betty.serde.load import (
+    AssertionFailed,
+    Fields,
+    Assertions,
+    Assertion,
+    RequiredField,
+    OptionalField,
+    Asserter,
+)
 from betty.warnings import deprecate
 
 DEFAULT_LIFETIME_THRESHOLD = 125
 
 
 class EntityReference(Configuration, Generic[EntityT]):
     def __init__(
@@ -41,15 +61,17 @@
     @property
     def entity_type(self) -> type[EntityT] | None:
         return self._entity_type
 
     @entity_type.setter
     def entity_type(self, entity_type: type[EntityT]) -> None:
         if self._entity_type_is_constrained:
-            raise AttributeError(f'The entity type cannot be set, as it is already constrained to {self._entity_type}.')
+            raise AttributeError(
+                f"The entity type cannot be set, as it is already constrained to {self._entity_type}."
+            )
         self._entity_type = entity_type
         self._dispatch_change()
 
     @property
     def entity_id(self) -> str | None:
         return self._entity_id
 
@@ -78,50 +100,60 @@
         dump: Dump,
         configuration: Self | None = None,
     ) -> Self:
         if configuration is None:
             configuration = cls()
         asserter = Asserter()
         if isinstance(dump, dict) or not configuration.entity_type_is_constrained:
-            asserter.assert_record(Fields(
-                RequiredField(
-                    'entity_type',
-                    Assertions(asserter.assert_entity_type()) | asserter.assert_setattr(configuration, 'entity_type'),
-                ),
-                OptionalField(
-                    'entity_id',
-                    Assertions(asserter.assert_str()) | asserter.assert_setattr(configuration, 'entity_id'),
-                ),
-            ))(dump)
+            asserter.assert_record(
+                Fields(
+                    RequiredField(
+                        "entity_type",
+                        Assertions(asserter.assert_entity_type())
+                        | asserter.assert_setattr(configuration, "entity_type"),
+                    ),
+                    OptionalField(
+                        "entity_id",
+                        Assertions(asserter.assert_str())
+                        | asserter.assert_setattr(configuration, "entity_id"),
+                    ),
+                )
+            )(dump)
         else:
             asserter.assert_str()(dump)
-            asserter.assert_setattr(configuration, 'entity_id')(dump)  # type: ignore[arg-type]
+            asserter.assert_setattr(configuration, "entity_id")(dump)  # type: ignore[arg-type]
         return configuration
 
     def dump(self) -> VoidableDump:
         if self.entity_type_is_constrained:
             return void_none(self.entity_id)
 
         if self.entity_type is None or self.entity_id is None:
             return Void
 
         dump: VoidableDictDump[VoidableDump] = {
-            'entity_type': get_entity_type_name(self._entity_type) if self._entity_type else Void,
-            'entity_id': self._entity_id,
+            "entity_type": (
+                get_entity_type_name(self._entity_type) if self._entity_type else Void
+            ),
+            "entity_id": self._entity_id,
         }
 
         return minimize(dump)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, EntityReference):
             return NotImplemented
-        return self.entity_type == other.entity_type and self.entity_id == other.entity_id
+        return (
+            self.entity_type == other.entity_type and self.entity_id == other.entity_id
+        )
 
 
-class EntityReferenceSequence(Generic[EntityT], ConfigurationSequence[EntityReference[EntityT]]):
+class EntityReferenceSequence(
+    Generic[EntityT], ConfigurationSequence[EntityReference[EntityT]]
+):
     def __init__(
         self,
         entity_references: Iterable[EntityReference[EntityT]] | None = None,
         *,
         entity_type_constraint: type[EntityT] | None = None,
     ):
         self._entity_type_constraint = entity_type_constraint
@@ -136,52 +168,63 @@
 
         entity_type_constraint = self._entity_type_constraint
         entity_reference_entity_type = configuration._entity_type
 
         if entity_type_constraint is None:
             return
 
-        if entity_reference_entity_type == entity_type_constraint and configuration.entity_type_is_constrained:
+        if (
+            entity_reference_entity_type == entity_type_constraint
+            and configuration.entity_type_is_constrained
+        ):
             return
 
         expected_entity_type_name = get_entity_type_name(
             cast(type[Entity], entity_type_constraint),
         )
         expected_entity_type_label = entity_type_constraint.entity_type_label()
 
         if entity_reference_entity_type is None:
-            raise AssertionFailed(Str._(
-                'The entity reference must be for an entity of type {expected_entity_type_name} ({expected_entity_type_label}), but instead does not specify an entity type at all.',
-                expected_entity_type_name=expected_entity_type_name,
-                expected_entity_type_label=expected_entity_type_label,
-            ))
+            raise AssertionFailed(
+                Str._(
+                    "The entity reference must be for an entity of type {expected_entity_type_name} ({expected_entity_type_label}), but instead does not specify an entity type at all.",
+                    expected_entity_type_name=expected_entity_type_name,
+                    expected_entity_type_label=expected_entity_type_label,
+                )
+            )
 
         actual_entity_type_label = entity_type_constraint.entity_type_label()
 
-        raise AssertionFailed(Str._(
-            'The entity reference must be for an entity of type {expected_entity_type_name} ({expected_entity_type_label}), but instead is for an entity of type {actual_entity_type_name} ({actual_entity_type_label})',
-            expected_entity_type_name=expected_entity_type_name,
-            expected_entity_type_label=expected_entity_type_label,
-            actual_entity_type_name=get_entity_type_name(entity_reference_entity_type),
-            actual_entity_type_label=actual_entity_type_label,
-        ))
+        raise AssertionFailed(
+            Str._(
+                "The entity reference must be for an entity of type {expected_entity_type_name} ({expected_entity_type_label}), but instead is for an entity of type {actual_entity_type_name} ({actual_entity_type_label})",
+                expected_entity_type_name=expected_entity_type_name,
+                expected_entity_type_label=expected_entity_type_label,
+                actual_entity_type_name=get_entity_type_name(
+                    entity_reference_entity_type
+                ),
+                actual_entity_type_label=actual_entity_type_label,
+            )
+        )
 
 
 class ExtensionConfiguration(Configuration):
     def __init__(
         self,
         extension_type: type[Extension],
         *,
         enabled: bool = True,
         extension_configuration: Configuration | None = None,
     ):
         super().__init__()
         self._extension_type = extension_type
         self._enabled = enabled
-        if extension_configuration is None and issubclass(extension_type, ConfigurableExtension):
+        if extension_configuration is None and issubclass(
+            extension_type, ConfigurableExtension
+        ):
             extension_configuration = extension_type.default_configuration()
         if extension_configuration is not None:
             extension_configuration.on_change(self)
         self._extension_configuration = extension_configuration
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, self.__class__):
@@ -219,63 +262,88 @@
     @classmethod
     def load(
         cls,
         dump: Dump,
         configuration: Self | None = None,
     ) -> Self:
         asserter = Asserter()
-        extension_type = asserter.assert_field(RequiredField(
-            'extension',
-            Assertions(asserter.assert_extension_type()),
-        ))(dump)
+        extension_type = asserter.assert_field(
+            RequiredField(
+                "extension",
+                Assertions(asserter.assert_extension_type()),
+            )
+        )(dump)
         if configuration is None:
             configuration = cls(extension_type)
         else:
             # This MUST NOT fail. If it does, this is a bug in the calling code that must be fixed.
             assert extension_type is configuration.extension_type
-        asserter.assert_record(Fields(
-            RequiredField(
-                'extension',
-            ),
-            OptionalField(
-                'enabled',
-                Assertions(asserter.assert_bool()) | asserter.assert_setattr(configuration, 'enabled'),
-            ),
-            OptionalField(
-                'configuration',
-                Assertions(configuration._assert_load_extension_configuration(configuration.extension_type)),
-            ),
-        ))(dump)
+        asserter.assert_record(
+            Fields(
+                RequiredField(
+                    "extension",
+                ),
+                OptionalField(
+                    "enabled",
+                    Assertions(asserter.assert_bool())
+                    | asserter.assert_setattr(configuration, "enabled"),
+                ),
+                OptionalField(
+                    "configuration",
+                    Assertions(
+                        configuration._assert_load_extension_configuration(
+                            configuration.extension_type
+                        )
+                    ),
+                ),
+            )
+        )(dump)
         return configuration
 
-    def _assert_load_extension_configuration(self, extension_type: type[Extension]) -> Assertion[Any, Configuration]:
+    def _assert_load_extension_configuration(
+        self, extension_type: type[Extension]
+    ) -> Assertion[Any, Configuration]:
         def _assertion(value: Any) -> Configuration:
             extension_configuration = self._extension_configuration
             if isinstance(extension_configuration, Configuration):
                 return extension_configuration.load(value, extension_configuration)
-            raise AssertionFailed(Str._(
-                '{extension_type} is not configurable.',
-                extension_type=extension_type.name(),
-            ))
+            raise AssertionFailed(
+                Str._(
+                    "{extension_type} is not configurable.",
+                    extension_type=extension_type.name(),
+                )
+            )
+
         return _assertion
 
     def dump(self) -> VoidableDump:
-        return minimize({
-            'extension': self.extension_type.name(),
-            'enabled': self.enabled,
-            'configuration': minimize(self.extension_configuration.dump()) if issubclass(self.extension_type, Configurable) and self.extension_configuration else Void,
-        })
+        return minimize(
+            {
+                "extension": self.extension_type.name(),
+                "enabled": self.enabled,
+                "configuration": (
+                    minimize(self.extension_configuration.dump())
+                    if issubclass(self.extension_type, Configurable)
+                    and self.extension_configuration
+                    else Void
+                ),
+            }
+        )
 
 
-class ExtensionConfigurationMapping(ConfigurationMapping[type[Extension], ExtensionConfiguration]):
+class ExtensionConfigurationMapping(
+    ConfigurationMapping[type[Extension], ExtensionConfiguration]
+):
     def _minimize_item_dump(self) -> bool:
         return True
 
     @classmethod
-    def _create_default_item(cls, configuration_key: type[Extension]) -> ExtensionConfiguration:
+    def _create_default_item(
+        cls, configuration_key: type[Extension]
+    ) -> ExtensionConfiguration:
         return ExtensionConfiguration(configuration_key)
 
     def __init__(
         self,
         configurations: Iterable[ExtensionConfiguration] | None = None,
     ):
         super().__init__(configurations)
@@ -291,20 +359,20 @@
     def _load_key(
         cls,
         item_dump: Dump,
         key_dump: str,
     ) -> Dump:
         asserter = Asserter()
         dict_dump = asserter.assert_dict()(item_dump)
-        dict_dump['extension'] = key_dump
+        dict_dump["extension"] = key_dump
         return dict_dump
 
     def _dump_key(self, item_dump: VoidableDump) -> tuple[VoidableDump, str]:
         dict_dump = self._asserter.assert_dict()(item_dump)
-        return dict_dump, dict_dump.pop('extension')
+        return dict_dump, dict_dump.pop("extension")
 
     def enable(self, *extension_types: type[Extension]) -> None:
         for extension_type in extension_types:
             try:
                 self._configurations[extension_type].enabled = True
             except KeyError:
                 self.append(ExtensionConfiguration(extension_type))
@@ -342,59 +410,70 @@
     @property
     def generate_html_list(self) -> bool:
         return self._generate_html_list or False
 
     @generate_html_list.setter
     def generate_html_list(self, generate_html_list: bool | None) -> None:
         if generate_html_list and not issubclass(self._entity_type, UserFacingEntity):
-            raise AssertionFailed(Str._(
-                'Cannot generate pages for {entity_type}, because it is not a user-facing entity type.',
-                entity_type=get_entity_type_name(self._entity_type)
-            ))
+            raise AssertionFailed(
+                Str._(
+                    "Cannot generate pages for {entity_type}, because it is not a user-facing entity type.",
+                    entity_type=get_entity_type_name(self._entity_type),
+                )
+            )
         self._generate_html_list = generate_html_list
         self._dispatch_change()
 
     def update(self, other: Self) -> None:
         self._entity_type = other._entity_type
         self._generate_html_list = other._generate_html_list
         self._dispatch_change()
 
     @classmethod
     def load(
-            cls,
-            dump: Dump,
-            configuration: Self | None = None,
+        cls,
+        dump: Dump,
+        configuration: Self | None = None,
     ) -> Self:
         asserter = Asserter()
-        entity_type = asserter.assert_field(RequiredField[Any, type[Entity]](
-            'entity_type',
-            Assertions(asserter.assert_str()) | asserter.assert_entity_type()),
+        entity_type = asserter.assert_field(
+            RequiredField[Any, type[Entity]](
+                "entity_type",
+                Assertions(asserter.assert_str()) | asserter.assert_entity_type(),
+            ),
         )(dump)
         configuration = cls(entity_type)
-        asserter.assert_record(Fields(
-            OptionalField(
-                'entity_type',
-            ),
-            OptionalField(
-                'generate_html_list',
-                Assertions(asserter.assert_bool()) | asserter.assert_setattr(configuration, 'generate_html_list'),
-            ),
-        ))(dump)
+        asserter.assert_record(
+            Fields(
+                OptionalField(
+                    "entity_type",
+                ),
+                OptionalField(
+                    "generate_html_list",
+                    Assertions(asserter.assert_bool())
+                    | asserter.assert_setattr(configuration, "generate_html_list"),
+                ),
+            )
+        )(dump)
         return configuration
 
     def dump(self) -> VoidableDump:
         dump: VoidableDictDump[VoidableDump] = {
-            'entity_type': get_entity_type_name(self._entity_type),
-            'generate_html_list': Void if self._generate_html_list is None else self._generate_html_list,
+            "entity_type": get_entity_type_name(self._entity_type),
+            "generate_html_list": (
+                Void if self._generate_html_list is None else self._generate_html_list
+            ),
         }
 
         return minimize(dump)
 
 
-class EntityTypeConfigurationMapping(ConfigurationMapping[type[Entity], EntityTypeConfiguration]):
+class EntityTypeConfigurationMapping(
+    ConfigurationMapping[type[Entity], EntityTypeConfiguration]
+):
     def _minimize_item_dump(self) -> bool:
         return True
 
     def _get_key(self, configuration: EntityTypeConfiguration) -> type[Entity]:
         return configuration.entity_type
 
     @classmethod
@@ -402,41 +481,43 @@
         cls,
         item_dump: Dump,
         key_dump: str,
     ) -> Dump:
         asserter = Asserter()
         dict_dump = asserter.assert_dict()(item_dump)
         asserter.assert_entity_type()(key_dump)
-        dict_dump['entity_type'] = key_dump
+        dict_dump["entity_type"] = key_dump
         return dict_dump
 
     def _dump_key(self, item_dump: VoidableDump) -> tuple[VoidableDump, str]:
         dict_dump = self._asserter.assert_dict()(item_dump)
-        return dict_dump, dict_dump.pop('entity_type')
+        return dict_dump, dict_dump.pop("entity_type")
 
     @classmethod
     def _item_type(cls) -> type[EntityTypeConfiguration]:
         return EntityTypeConfiguration
 
     @classmethod
-    def _create_default_item(cls, configuration_key: type[Entity]) -> EntityTypeConfiguration:
+    def _create_default_item(
+        cls, configuration_key: type[Entity]
+    ) -> EntityTypeConfiguration:
         return EntityTypeConfiguration(configuration_key)
 
 
 class LocaleConfiguration(Configuration):
     def __init__(
         self,
         locale: str,
         *,
         alias: str | None = None,
     ):
         super().__init__()
         self._locale = locale
-        if alias is not None and '/' in alias:
-            raise AssertionFailed(Str._('Locale aliases must not contain slashes.'))
+        if alias is not None and "/" in alias:
+            raise AssertionFailed(Str._("Locale aliases must not contain slashes."))
         self._alias = alias
 
     @recursive_repr()
     def __repr__(self) -> str:
         return repr_instance(self, locale=self.locale, alias=self.alias)
 
     def __eq__(self, other: Any) -> bool:
@@ -468,84 +549,84 @@
 
     def update(self, other: Self) -> None:
         self._locale = other._locale
         self._alias = other._alias
 
     @classmethod
     def load(
-            cls,
-            dump: Dump,
-            configuration: Self | None = None,
+        cls,
+        dump: Dump,
+        configuration: Self | None = None,
     ) -> Self:
         asserter = Asserter()
-        locale = asserter.assert_field(RequiredField(
-            'locale',
-            Assertions(asserter.assert_locale())),
+        locale = asserter.assert_field(
+            RequiredField("locale", Assertions(asserter.assert_locale())),
         )(dump)
         if configuration is None:
             configuration = cls(locale)
-        asserter.assert_record(Fields(
-            RequiredField(
-                'locale'
-            ),
-            OptionalField(
-                'alias',
-                Assertions(asserter.assert_str()) | asserter.assert_setattr(configuration, 'alias'),
-            ),
-        ))(dump)
+        asserter.assert_record(
+            Fields(
+                RequiredField("locale"),
+                OptionalField(
+                    "alias",
+                    Assertions(asserter.assert_str())
+                    | asserter.assert_setattr(configuration, "alias"),
+                ),
+            )
+        )(dump)
         return configuration
 
     def dump(self) -> VoidableDump:
-        return minimize({
-            'locale': self.locale,
-            'alias': void_none(self._alias)
-        })
+        return minimize({"locale": self.locale, "alias": void_none(self._alias)})
 
 
 class LocaleConfigurationMapping(ConfigurationMapping[str, LocaleConfiguration]):
     @classmethod
     def _create_default_item(cls, configuration_key: str) -> LocaleConfiguration:
         return LocaleConfiguration(configuration_key)
 
     def __init__(
         self,
         configurations: Iterable[LocaleConfiguration] | None = None,
     ):
         super().__init__(configurations)
         if len(self) == 0:
-            self.append(LocaleConfiguration('en-US'))
+            self.append(LocaleConfiguration("en-US"))
 
     def _get_key(self, configuration: LocaleConfiguration) -> str:
         return configuration.locale
 
     @classmethod
     def _load_key(
         cls,
         item_dump: Dump,
         key_dump: str,
     ) -> Dump:
         asserter = Asserter()
         dict_item_dump = asserter.assert_dict()(item_dump)
-        dict_item_dump['locale'] = key_dump
+        dict_item_dump["locale"] = key_dump
         return dict_item_dump
 
     def _dump_key(self, item_dump: VoidableDump) -> tuple[VoidableDump, str]:
         dict_item_dump = self._asserter.assert_dict()(item_dump)
-        return dict_item_dump, dict_item_dump.pop('locale')
+        return dict_item_dump, dict_item_dump.pop("locale")
 
     @classmethod
     def _item_type(cls) -> type[LocaleConfiguration]:
         return LocaleConfiguration
 
     def _on_remove(self, configuration: LocaleConfiguration) -> None:
         if len(self._configurations) <= 1:
-            raise AssertionFailed(Str._(
-                'Cannot remove the last remaining locale {locale}',
-                locale=get_data(configuration.locale).get_display_name() or configuration.locale,
-            ))
+            raise AssertionFailed(
+                Str._(
+                    "Cannot remove the last remaining locale {locale}",
+                    locale=get_data(configuration.locale).get_display_name()
+                    or configuration.locale,
+                )
+            )
 
     @property
     def default(self) -> LocaleConfiguration:
         return next(iter(self._configurations.values()))
 
     @default.setter
     def default(self, configuration: LocaleConfiguration | str) -> None:
@@ -561,51 +642,54 @@
 
 
 @final
 class ProjectConfiguration(FileBasedConfiguration):
     def __init__(
         self,
         base_url: str | None = None,
-        root_path: str = '',
+        root_path: str = "",
         clean_urls: bool = False,
-        title: str = 'Betty',
+        title: str = "Betty",
         author: str | None = None,
         entity_types: Iterable[EntityTypeConfiguration] | None = None,
         extensions: Iterable[ExtensionConfiguration] | None = None,
         debug: bool = False,
         locales: Iterable[LocaleConfiguration] | None = None,
         lifetime_threshold: int = DEFAULT_LIFETIME_THRESHOLD,
         name: str | None = None,
     ):
         super().__init__()
         self._name = name
         self._computed_name: str | None = None
-        self._base_url = 'https://example.com' if base_url is None else base_url
+        self._base_url = "https://example.com" if base_url is None else base_url
         self._root_path = root_path
         self._clean_urls = clean_urls
         self._title = title
         self._author = author
-        self._entity_types = EntityTypeConfigurationMapping(entity_types or [
-            EntityTypeConfiguration(
-                entity_type=Person,
-                generate_html_list=True,
-            ),
-            EntityTypeConfiguration(
-                entity_type=Event,
-                generate_html_list=True,
-            ),
-            EntityTypeConfiguration(
-                entity_type=Place,
-                generate_html_list=True,
-            ),
-            EntityTypeConfiguration(
-                entity_type=Source,
-                generate_html_list=True,
-            ),
-        ])
+        self._entity_types = EntityTypeConfigurationMapping(
+            entity_types
+            or [
+                EntityTypeConfiguration(
+                    entity_type=Person,
+                    generate_html_list=True,
+                ),
+                EntityTypeConfiguration(
+                    entity_type=Event,
+                    generate_html_list=True,
+                ),
+                EntityTypeConfiguration(
+                    entity_type=Place,
+                    generate_html_list=True,
+                ),
+                EntityTypeConfiguration(
+                    entity_type=Source,
+                    generate_html_list=True,
+                ),
+            ]
+        )
         self._entity_types.on_change(self)
         self._extensions = ExtensionConfigurationMapping(extensions or ())
         self._extensions.on_change(self)
         self._debug = debug
         self._locales = LocaleConfigurationMapping(locales or ())
         self._locales.on_change(self)
         self._lifetime_threshold = lifetime_threshold
@@ -621,23 +705,23 @@
 
     @property
     def project_directory_path(self) -> Path:
         return self.configuration_file_path.parent
 
     @property
     def output_directory_path(self) -> Path:
-        return self.project_directory_path / 'output'
+        return self.project_directory_path / "output"
 
     @property
     def assets_directory_path(self) -> Path:
-        return self.project_directory_path / 'assets'
+        return self.project_directory_path / "assets"
 
     @property
     def www_directory_path(self) -> Path:
-        return self.output_directory_path / 'www'
+        return self.output_directory_path / "www"
 
     def localize_www_directory_path(self, locale: str) -> Path:
         if self.locales.multilingual:
             return self.www_directory_path / self.locales[locale].alias
         return self.www_directory_path
 
     @property
@@ -662,27 +746,31 @@
     def base_url(self) -> str:
         return self._base_url
 
     @base_url.setter
     def base_url(self, base_url: str) -> None:
         base_url_parts = urlparse(base_url)
         if not base_url_parts.scheme:
-            raise AssertionFailed(Str._('The base URL must start with a scheme such as https://, http://, or file://.'))
+            raise AssertionFailed(
+                Str._(
+                    "The base URL must start with a scheme such as https://, http://, or file://."
+                )
+            )
         if not base_url_parts.netloc:
-            raise AssertionFailed(Str._('The base URL must include a path.'))
-        self._base_url = '%s://%s' % (base_url_parts.scheme, base_url_parts.netloc)
+            raise AssertionFailed(Str._("The base URL must include a path."))
+        self._base_url = "%s://%s" % (base_url_parts.scheme, base_url_parts.netloc)
         self._dispatch_change()
 
     @property
     def root_path(self) -> str:
         return self._root_path
 
     @root_path.setter
     def root_path(self, root_path: str) -> None:
-        self._root_path = root_path.strip('/')
+        self._root_path = root_path.strip("/")
         self._dispatch_change()
 
     @property
     def clean_urls(self) -> bool:
         return self._clean_urls
 
     @clean_urls.setter
@@ -732,111 +820,134 @@
         self._locales.update(other._locales)
         self._extensions.update(other._extensions)
         self._entity_types.update(other._entity_types)
         self._dispatch_change()
 
     @classmethod
     def load(
-            cls,
-            dump: Dump,
-            configuration: Self | None = None,
+        cls,
+        dump: Dump,
+        configuration: Self | None = None,
     ) -> Self:
         if configuration is None:
             configuration = cls()
         asserter = Asserter()
-        asserter.assert_record(Fields(
-            OptionalField(
-                'name',
-                Assertions(asserter.assert_str()) | asserter.assert_setattr(configuration, 'name'),
-            ),
-            RequiredField(
-                'base_url',
-                Assertions(asserter.assert_str()) | asserter.assert_setattr(configuration, 'base_url'),
-            ),
-            OptionalField(
-                'title',
-                Assertions(asserter.assert_str()) | asserter.assert_setattr(configuration, 'title'),
-            ),
-            OptionalField(
-                'author',
-                Assertions(asserter.assert_str()) | asserter.assert_setattr(configuration, 'author'),
-            ),
-            OptionalField(
-                'root_path',
-                Assertions(asserter.assert_str()) | asserter.assert_setattr(configuration, 'root_path'),
-            ),
-            OptionalField(
-                'clean_urls',
-                Assertions(asserter.assert_bool()) | asserter.assert_setattr(configuration, 'clean_urls'),
-            ),
-            OptionalField(
-                'debug',
-                Assertions(asserter.assert_bool()) | asserter.assert_setattr(configuration, 'debug'),
-            ),
-            OptionalField(
-                'lifetime_threshold',
-                Assertions(asserter.assert_int()) | asserter.assert_setattr(configuration, 'lifetime_threshold'),
-            ),
-            OptionalField(
-                'locales',
-                Assertions(configuration._locales.assert_load(configuration.locales)),
-            ),
-            OptionalField(
-                'extensions',
-                Assertions(configuration._extensions.assert_load(configuration.extensions)),
-            ),
-            OptionalField(
-                'entity_types',
-                Assertions(configuration._entity_types.assert_load(configuration.entity_types)),
-            ),
-        ))(dump)
+        asserter.assert_record(
+            Fields(
+                OptionalField(
+                    "name",
+                    Assertions(asserter.assert_str())
+                    | asserter.assert_setattr(configuration, "name"),
+                ),
+                RequiredField(
+                    "base_url",
+                    Assertions(asserter.assert_str())
+                    | asserter.assert_setattr(configuration, "base_url"),
+                ),
+                OptionalField(
+                    "title",
+                    Assertions(asserter.assert_str())
+                    | asserter.assert_setattr(configuration, "title"),
+                ),
+                OptionalField(
+                    "author",
+                    Assertions(asserter.assert_str())
+                    | asserter.assert_setattr(configuration, "author"),
+                ),
+                OptionalField(
+                    "root_path",
+                    Assertions(asserter.assert_str())
+                    | asserter.assert_setattr(configuration, "root_path"),
+                ),
+                OptionalField(
+                    "clean_urls",
+                    Assertions(asserter.assert_bool())
+                    | asserter.assert_setattr(configuration, "clean_urls"),
+                ),
+                OptionalField(
+                    "debug",
+                    Assertions(asserter.assert_bool())
+                    | asserter.assert_setattr(configuration, "debug"),
+                ),
+                OptionalField(
+                    "lifetime_threshold",
+                    Assertions(asserter.assert_int())
+                    | asserter.assert_setattr(configuration, "lifetime_threshold"),
+                ),
+                OptionalField(
+                    "locales",
+                    Assertions(
+                        configuration._locales.assert_load(configuration.locales)
+                    ),
+                ),
+                OptionalField(
+                    "extensions",
+                    Assertions(
+                        configuration._extensions.assert_load(configuration.extensions)
+                    ),
+                ),
+                OptionalField(
+                    "entity_types",
+                    Assertions(
+                        configuration._entity_types.assert_load(
+                            configuration.entity_types
+                        )
+                    ),
+                ),
+            )
+        )(dump)
         return configuration
 
     def dump(self) -> VoidableDictDump[Dump]:
-        return minimize({  # type: ignore[return-value]
-            'name': void_none(self.name),
-            'base_url': self.base_url,
-            'title': self.title,
-            'root_path': void_none(self.root_path),
-            'clean_urls': void_none(self.clean_urls),
-            'author': void_none(self.author),
-            'debug': void_none(self.debug),
-            'lifetime_threshold': void_none(self.lifetime_threshold),
-            'locales': self.locales.dump(),
-            'extensions': self.extensions.dump(),
-            'entity_types': self.entity_types.dump(),
-        }, True)
+        return minimize(
+            {  # type: ignore[return-value]
+                "name": void_none(self.name),
+                "base_url": self.base_url,
+                "title": self.title,
+                "root_path": void_none(self.root_path),
+                "clean_urls": void_none(self.clean_urls),
+                "author": void_none(self.author),
+                "debug": void_none(self.debug),
+                "lifetime_threshold": void_none(self.lifetime_threshold),
+                "locales": self.locales.dump(),
+                "extensions": self.extensions.dump(),
+                "entity_types": self.entity_types.dump(),
+            },
+            True,
+        )
 
 
 class Project(Configurable[ProjectConfiguration]):
     def __init__(
         self,
         *,
         project_id: str | None = None,
         ancestry: Ancestry | None = None,
     ):
         super().__init__()
         if project_id is not None:
             deprecate(
-                f'Initializing {type(self)} with a project ID is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, set {type(self)}.configuration.name.',
+                f"Initializing {type(self)} with a project ID is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Instead, set {type(self)}.configuration.name.",
                 stacklevel=2,
             )
         self._id = project_id
         self._configuration = ProjectConfiguration()
         self._ancestry = Ancestry() if ancestry is None else ancestry
 
     @property
     def id(self) -> str:
-        deprecate(f'{type(self)}.id is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Insead, use {type(self)}.name.')
+        deprecate(
+            f"{type(self)}.id is deprecated as of Betty 0.3.2, and will be removed in Betty 0.4.x. Insead, use {type(self)}.name."
+        )
         if self._id is None:
             return self.name
         return self._id
 
     @property
     def name(self) -> str:
         if self._configuration.name is None:
-            return hashlib.md5(str(self._configuration.configuration_file_path).encode('utf-8')).hexdigest()
+            return hashid(str(self._configuration.configuration_file_path))
         return self._configuration.name
 
     @property
     def ancestry(self) -> Ancestry:
         return self._ancestry
```

### Comparing `betty-0.3.3/betty/render.py` & `betty-0.3.4/betty/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide the Render API.
 """
+
 from pathlib import Path
 
 from betty.locale import Localizer
 from betty.job import Context
 
 
 class Renderer:
@@ -23,18 +24,16 @@
 
 
 class SequentialRenderer(Renderer):
     def __init__(self, renderers: list[Renderer]):
         self._renderers = renderers
         self._file_extensions = {
             file_extension
-            for renderer
-            in self._renderers
-            for file_extension
-            in renderer.file_extensions
+            for renderer in self._renderers
+            for file_extension in renderer.file_extensions
         }
 
     @property
     def file_extensions(self) -> set[str]:
         return self._file_extensions
 
     async def render_file(
@@ -42,13 +41,15 @@
         file_path: Path,
         *,
         job_context: Context | None = None,
         localizer: Localizer | None = None,
     ) -> Path:
         for renderer in self._renderers:
             if file_path.suffix in renderer.file_extensions:
-                return await self.render_file(await renderer.render_file(
-                    file_path,
-                    job_context=job_context,
-                    localizer=localizer,
-                ))
+                return await self.render_file(
+                    await renderer.render_file(
+                        file_path,
+                        job_context=job_context,
+                        localizer=localizer,
+                    )
+                )
         return file_path
```

### Comparing `betty-0.3.3/betty/serde/dump.py` & `betty-0.3.4/betty/serde/dump.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,75 @@
 """
 Provide a serialization API.
 """
+
 from __future__ import annotations
 
 from typing import TypeVar, Sequence, Mapping, overload, Literal, TypeAlias, Any
 
-T = TypeVar('T')
-U = TypeVar('U')
+T = TypeVar("T")
+U = TypeVar("U")
 
 
 class Void:
     pass
 
 
-DumpType: TypeAlias = bool | int | float | str | None | list['Dump'] | dict[str, 'Dump']
-DumpTypeT = TypeVar('DumpTypeT', bound=DumpType)
+DumpType: TypeAlias = bool | int | float | str | None | list["Dump"] | dict[str, "Dump"]
+DumpTypeT = TypeVar("DumpTypeT", bound=DumpType)
 
-Dump: TypeAlias = bool | int | float | str | None | Sequence['Dump'] | Mapping[str, 'Dump']
-DumpT = TypeVar('DumpT', bound=Dump)
-DumpU = TypeVar('DumpU', bound=Dump)
+Dump: TypeAlias = (
+    bool | int | float | str | None | Sequence["Dump"] | Mapping[str, "Dump"]
+)
+DumpT = TypeVar("DumpT", bound=Dump)
+DumpU = TypeVar("DumpU", bound=Dump)
 
 VoidableDump: TypeAlias = Dump | type[Void]
-VoidableDumpT = TypeVar('VoidableDumpT', bound=VoidableDump)
-VoidableDumpU = TypeVar('VoidableDumpU', bound=VoidableDump)
+VoidableDumpT = TypeVar("VoidableDumpT", bound=VoidableDump)
+VoidableDumpU = TypeVar("VoidableDumpU", bound=VoidableDump)
 
 ListDump: TypeAlias = list[DumpT]
 
 DictDump: TypeAlias = dict[str, DumpT]
 
 VoidableListDump: TypeAlias = list[VoidableDumpT]
 
 VoidableDictDump: TypeAlias = dict[str, VoidableDumpT]
 
-_MinimizableDump: TypeAlias = VoidableDump | VoidableListDump[VoidableDumpT] | VoidableDictDump[VoidableDumpT]
+_MinimizableDump: TypeAlias = (
+    VoidableDump | VoidableListDump[VoidableDumpT] | VoidableDictDump[VoidableDumpT]
+)
 
 
 @overload
-def minimize(dump: _MinimizableDump[VoidableDump], voidable: Literal[True] = True) -> VoidableDump:
+def minimize(
+    dump: _MinimizableDump[VoidableDump], voidable: Literal[True] = True
+) -> VoidableDump:
     pass
 
 
 @overload
 def minimize(dump: _MinimizableDump[VoidableDump], voidable: Literal[False]) -> Dump:
     pass
 
 
-def minimize(dump: _MinimizableDump[VoidableDump], voidable: bool = True) -> VoidableDump:
+def minimize(
+    dump: _MinimizableDump[VoidableDump], voidable: bool = True
+) -> VoidableDump:
     """
     Minimize a configuration dump by removing any Void configurationfrom sequences and mappings.
     """
     if isinstance(dump, (Sequence, Mapping)) and not isinstance(dump, str):
         if isinstance(dump, Sequence):
-            dump = [
-                value
-                for value
-                in dump
-                if value is not Void
-            ]
+            dump = [value for value in dump if value is not Void]
             for key in reversed(range(len(dump))):
                 if dump[key] is Void:
                     del dump[key]
         if isinstance(dump, Mapping):
-            dump = {
-                key: value
-                for key, value
-                in dump.items()
-                if value is not Void
-            }
+            dump = {key: value for key, value in dump.items() if value is not Void}
         if len(dump) or not voidable:
             return dump  # type: ignore[return-value]
         return Void
     return dump
 
 
 def void_none(value: VoidableDump) -> VoidableDump:
@@ -84,20 +83,24 @@
     """
     Passthrough a value, but convert None to Void.
     """
     return None if value is Void else value
 
 
 @overload
-def dump_default(dump: DictDump[Dump], key: str, default_type: type[dict[Any, Any]]) -> DictDump[Dump]:
+def dump_default(
+    dump: DictDump[Dump], key: str, default_type: type[dict[Any, Any]]
+) -> DictDump[Dump]:
     pass
 
 
 @overload
-def dump_default(dump: DictDump[Dump], key: str, default_type: type[list[Any]]) -> ListDump[Dump]:
+def dump_default(
+    dump: DictDump[Dump], key: str, default_type: type[list[Any]]
+) -> ListDump[Dump]:
     pass
 
 
 def dump_default(dump, key, default_type):
     """
     Add a key and value to a dump, if the key does not exist yet.
     """
```

### Comparing `betty-0.3.3/betty/serde/error.py` & `betty-0.3.4/betty/serde/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,22 @@
     """
 
     def __init__(self, message: Localizable):
         super().__init__(message)
         self._contexts: tuple[Localizable, ...] = ()
 
     def localize(self, localizer: Localizer) -> str:
-        localized_contexts = map(lambda context: context.localize(localizer), self._contexts)
-        return (super().localize(localizer) + '\n' + indent('\n'.join(localized_contexts), '- ')).strip()
+        localized_contexts = map(
+            lambda context: context.localize(localizer), self._contexts
+        )
+        return (
+            super().localize(localizer)
+            + "\n"
+            + indent("\n".join(localized_contexts), "- ")
+        ).strip()
 
     def raised(self, error_type: type[SerdeError]) -> bool:
         return isinstance(self, error_type)
 
     @property
     def contexts(self) -> tuple[Localizable, ...]:
         return self._contexts
@@ -49,22 +55,22 @@
     A collection of zero or more serialization or deserialization errors.
     """
 
     def __init__(
         self,
         errors: list[SerdeError] | None = None,
     ):
-        super().__init__(Str._('The following errors occurred'))
+        super().__init__(Str._("The following errors occurred"))
         self._errors: list[SerdeError] = errors or []
 
     def __iter__(self) -> Iterator[SerdeError]:
         yield from self._errors
 
     def localize(self, localizer: Localizer) -> str:
-        return '\n\n'.join(map(lambda error: error.localize(localizer), self._errors))
+        return "\n\n".join(map(lambda error: error.localize(localizer), self._errors))
 
     def __reduce__(self) -> tuple[type[Self], tuple[list[SerdeError]]]:  # type: ignore[override]
         return type(self), (self._errors,)
 
     def __len__(self) -> int:
         return len(self._errors)
```

### Comparing `betty-0.3.3/betty/serde/format.py` & `betty-0.3.4/betty/serde/format.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide serialization formats.
 """
+
 from __future__ import annotations
 
 import json
 from typing import cast, Sequence
 
 import yaml
 
@@ -28,50 +29,54 @@
     def dump(self, dump: VoidableDump) -> str:
         raise NotImplementedError(repr(self))
 
 
 class Json(Format):
     @property
     def extensions(self) -> set[str]:
-        return {'json'}
+        return {"json"}
 
     @property
     def label(self) -> Str:
-        return Str.plain('JSON')
+        return Str.plain("JSON")
 
     def load(self, dump: str) -> Dump:
         try:
             return cast(Dump, json.loads(dump))
         except json.JSONDecodeError as e:
-            raise FormatError(Str._(
-                'Invalid JSON: {error}.',
-                error=str(e),
-            ))
+            raise FormatError(
+                Str._(
+                    "Invalid JSON: {error}.",
+                    error=str(e),
+                )
+            )
 
     def dump(self, dump: VoidableDump) -> str:
         return json.dumps(dump)
 
 
 class Yaml(Format):
     @property
     def extensions(self) -> set[str]:
-        return {'yaml', 'yml'}
+        return {"yaml", "yml"}
 
     @property
     def label(self) -> Str:
-        return Str.plain('YAML')
+        return Str.plain("YAML")
 
     def load(self, dump: str) -> Dump:
         try:
             return cast(Dump, yaml.safe_load(dump))
         except yaml.YAMLError as e:
-            raise FormatError(Str._(
-                'Invalid YAML: {error}.',
-                error=str(e),
-            ))
+            raise FormatError(
+                Str._(
+                    "Invalid YAML: {error}.",
+                    error=str(e),
+                )
+            )
 
     def dump(self, dump: VoidableDump) -> str:
         return yaml.safe_dump(dump)
 
 
 class FormatRepository:
     def __init__(
@@ -86,33 +91,35 @@
     @property
     def formats(self) -> tuple[Format, ...]:
         return self._formats
 
     @property
     def extensions(self) -> tuple[str, ...]:
         return tuple(
-            extension
-            for _format in self._formats
-            for extension in _format.extensions
+            extension for _format in self._formats for extension in _format.extensions
         )
 
     def format_for(self, extension: str) -> Format:
         for format in self._formats:
             if extension in format.extensions:
                 return format
-        raise FormatError(Str._(
-            'Unknown file format ".{extension}". Supported formats are: {supported_formats}.',
-            extension=extension,
-            supported_formats=FormatStr(self.formats),
-        ))
+        raise FormatError(
+            Str._(
+                'Unknown file format ".{extension}". Supported formats are: {supported_formats}.',
+                extension=extension,
+                supported_formats=FormatStr(self.formats),
+            )
+        )
 
 
 class FormatStr(Localizable):
     def __init__(self, formats: Sequence[Format]):
         self._formats = formats
 
     def localize(self, localizer: Localizer) -> str:
-        return ', '.join([
-            f'.{extension} ({format.label.localize(localizer)})'
-            for format in self._formats
-            for extension in format.extensions
-        ])
+        return ", ".join(
+            [
+                f".{extension} ({format.label.localize(localizer)})"
+                for format in self._formats
+                for extension in format.extensions
+            ]
+        )
```

### Comparing `betty-0.3.3/betty/serde/load.py` & `betty-0.3.4/betty/serde/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,54 @@
 """
 Provide a deserialization API.
 """
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Iterator, Callable, Any, Generic, TYPE_CHECKING, TypeVar, MutableSequence, MutableMapping, overload, \
-    cast, TypeAlias
+from typing import (
+    Iterator,
+    Callable,
+    Any,
+    Generic,
+    TYPE_CHECKING,
+    TypeVar,
+    MutableSequence,
+    MutableMapping,
+    overload,
+    cast,
+    TypeAlias,
+)
 
 from betty.functools import _Result
 from betty.locale import LocaleNotFoundError, get_data, Str
-from betty.model import Entity, get_entity_type, EntityTypeImportError, EntityTypeInvalidError, EntityTypeError
+from betty.model import (
+    Entity,
+    get_entity_type,
+    EntityTypeImportError,
+    EntityTypeInvalidError,
+    EntityTypeError,
+)
 from betty.serde.dump import DumpType, DumpTypeT, Void
 from betty.serde.error import SerdeError, SerdeErrorCollection
 
 if TYPE_CHECKING:
     from betty.app.extension import Extension
 
-T = TypeVar('T')
-ValueT = TypeVar('ValueT')
-ReturnT = TypeVar('ReturnT')
-ReturnU = TypeVar('ReturnU')
-CallValueT = TypeVar('CallValueT')
-CallReturnT = TypeVar('CallReturnT')
-FValueT = TypeVar('FValueT')
-MapReturnT = TypeVar('MapReturnT')
+T = TypeVar("T")
+ValueT = TypeVar("ValueT")
+ReturnT = TypeVar("ReturnT")
+ReturnU = TypeVar("ReturnU")
+CallValueT = TypeVar("CallValueT")
+CallReturnT = TypeVar("CallReturnT")
+FValueT = TypeVar("FValueT")
+MapReturnT = TypeVar("MapReturnT")
 Number: TypeAlias = int | float
-NumberT = TypeVar('NumberT', bound=Number)
+NumberT = TypeVar("NumberT", bound=Number)
 
 
 class LoadError(SerdeError):
     pass
 
 
 class AssertionFailed(LoadError):
@@ -49,30 +67,39 @@
 ]
 
 
 class _Assertions(Generic[CallValueT, CallReturnT, FValueT]):
     def __init__(self, _assertion: Assertion[FValueT, CallReturnT]):
         self._assertion = _assertion
 
-    def extend(self, _assertion: Assertion[CallReturnT, MapReturnT]) -> _Assertions[CallValueT, MapReturnT, CallReturnT]:
+    def extend(
+        self, _assertion: Assertion[CallReturnT, MapReturnT]
+    ) -> _Assertions[CallValueT, MapReturnT, CallReturnT]:
         return _AssertionExtension(_assertion, self)
 
-    def __or__(self, _assertion: Assertion[CallReturnT, MapReturnT]) -> _Assertions[CallValueT, MapReturnT, CallReturnT]:
+    def __or__(
+        self, _assertion: Assertion[CallReturnT, MapReturnT]
+    ) -> _Assertions[CallValueT, MapReturnT, CallReturnT]:
         return self.extend(_assertion)
 
     def __call__(self, value: CallValueT) -> _Result[CallReturnT]:
         raise NotImplementedError(repr(self))
 
 
-class Assertions(_Assertions[CallValueT, CallReturnT, CallValueT], Generic[CallValueT, CallReturnT]):
+class Assertions(
+    _Assertions[CallValueT, CallReturnT, CallValueT], Generic[CallValueT, CallReturnT]
+):
     def __call__(self, value: CallValueT) -> _Result[CallReturnT]:
         return _Result(value).map(self._assertion)
 
 
-class _AssertionExtension(_Assertions[CallValueT, CallReturnT, FValueT], Generic[CallValueT, CallReturnT, FValueT]):
+class _AssertionExtension(
+    _Assertions[CallValueT, CallReturnT, FValueT],
+    Generic[CallValueT, CallReturnT, FValueT],
+):
     def __init__(
         self,
         _assertion: Assertion[FValueT, CallReturnT],
         extended_assertion: _Assertions[CallValueT, FValueT, Any],
     ):
         super().__init__(_assertion)
         self._extended_assertion = extended_assertion
@@ -103,231 +130,290 @@
 
     def __iter__(self) -> Iterator[_Field[Any, Any]]:
         return (field for field in self._fields)
 
 
 _AssertionBuilderFunction = Callable[[ValueT], ReturnT]
 _AssertionBuilderMethod = Callable[[object, ValueT], ReturnT]
-_AssertionBuilder = '_AssertionBuilderFunction[ValueT, ReturnT] | _AssertionBuilderMethod[ValueT, ReturnT]'
+_AssertionBuilder = "_AssertionBuilderFunction[ValueT, ReturnT] | _AssertionBuilderMethod[ValueT, ReturnT]"
 
 
 class Asserter:
     def _assert_type_violation_error_message(
-            self,
-            asserted_type: type[DumpType],
+        self,
+        asserted_type: type[DumpType],
     ) -> Str:
         messages = {
-            None: Str._('This must be none/null.'),
-            bool: Str._('This must be a boolean.'),
-            int: Str._('This must be a whole number.'),
-            float: Str._('This must be a decimal number.'),
-            str: Str._('This must be a string.'),
-            list: Str._('This must be a list.'),
-            dict: Str._('This must be a key-value mapping.'),
+            None: Str._("This must be none/null."),
+            bool: Str._("This must be a boolean."),
+            int: Str._("This must be a whole number."),
+            float: Str._("This must be a decimal number."),
+            str: Str._("This must be a string."),
+            list: Str._("This must be a list."),
+            dict: Str._("This must be a key-value mapping."),
         }
         return messages[asserted_type]  # type: ignore[index]
 
     def _assert_type(
         self,
         value: Any,
         value_required_type: type[DumpTypeT],
         value_disallowed_type: type[DumpType] | None = None,
     ) -> DumpTypeT:
-        if isinstance(value, value_required_type) and (value_disallowed_type is None or not isinstance(value, value_disallowed_type)):
+        if isinstance(value, value_required_type) and (
+            value_disallowed_type is None
+            or not isinstance(value, value_disallowed_type)
+        ):
             return value
         raise AssertionFailed(
             self._assert_type_violation_error_message(
                 value_required_type,  # type: ignore[arg-type]
             )
         )
 
-    def assert_or(self, if_assertion: Assertion[ValueT, ReturnT], else_assertions: Assertion[ValueT, ReturnU]) -> Assertion[ValueT, ReturnT | ReturnU]:
+    def assert_or(
+        self,
+        if_assertion: Assertion[ValueT, ReturnT],
+        else_assertions: Assertion[ValueT, ReturnU],
+    ) -> Assertion[ValueT, ReturnT | ReturnU]:
         def _assert_or(value: Any) -> ReturnT | ReturnU:
             assertions = (if_assertion, else_assertions)
             errors = SerdeErrorCollection()
             for assertion in assertions:
                 try:
                     return assertion(value)
                 except SerdeError as e:
                     if e.raised(AssertionFailed):
                         errors.append(e)
             raise errors
+
         return _assert_or
 
     def assert_none(self) -> Assertion[Any, None]:
         def _assert_none(value: Any) -> None:
             self._assert_type(value, type(None))
+
         return _assert_none
 
     def assert_bool(self) -> Assertion[Any, bool]:
         def _assert_bool(value: Any) -> bool:
             return self._assert_type(value, bool)
+
         return _assert_bool
 
     def assert_int(self) -> Assertion[Any, int]:
         def _assert_int(value: Any) -> int:
             return self._assert_type(value, int, bool)
+
         return _assert_int
 
     def assert_float(self) -> Assertion[Any, float]:
         def _assert_float(value: Any) -> float:
             return self._assert_type(value, float)
+
         return _assert_float
 
     def assert_number(self) -> Assertion[Any, int | float]:
         return self.assert_or(self.assert_int(), self.assert_float())
 
     def assert_positive_number(self) -> Assertion[Any, Number]:
         def _assert_positive_number(
             value: Any,
         ) -> Number:
             value = self.assert_number()(value)
             if value <= 0:
-                raise AssertionFailed(Str._('This must be a positive number.'))
+                raise AssertionFailed(Str._("This must be a positive number."))
             return value
+
         return _assert_positive_number
 
     def assert_str(self) -> Assertion[Any, str]:
         def _assert_str(value: Any) -> str:
             return self._assert_type(value, str)
+
         return _assert_str
 
     def assert_list(self) -> Assertion[Any, list[Any]]:
         def _assert_list(value: Any) -> list[Any]:
             return self._assert_type(value, list)
+
         return _assert_list
 
     def assert_dict(self) -> Assertion[Any, dict[str, Any]]:
         def _assert_dict(value: Any) -> dict[str, Any]:
             return self._assert_type(value, dict)
+
         return _assert_dict
 
-    def assert_assertions(self, assertions: _Assertions[ValueT, ReturnT, Any]) -> Assertion[Any, ReturnT]:
+    def assert_assertions(
+        self, assertions: _Assertions[ValueT, ReturnT, Any]
+    ) -> Assertion[Any, ReturnT]:
         def _assert_assertions(value: Any) -> ReturnT:
             return assertions(value).value
+
         return _assert_assertions
 
-    def assert_sequence(self, item_assertion: Assertions[ValueT, ReturnT]) -> Assertion[Any, MutableSequence[ReturnT]]:
+    def assert_sequence(
+        self, item_assertion: Assertions[ValueT, ReturnT]
+    ) -> Assertion[Any, MutableSequence[ReturnT]]:
         def _assert_sequence(value: ValueT) -> MutableSequence[ReturnT]:
             list_value = self.assert_list()(value)
             sequence = []
             with SerdeErrorCollection().assert_valid() as errors:
                 for value_item_index, value_item_value in enumerate(list_value):
                     with errors.catch(Str.plain(value_item_index)):
-                        sequence.append(self.assert_assertions(item_assertion)(value_item_value))
+                        sequence.append(
+                            self.assert_assertions(item_assertion)(value_item_value)
+                        )
             return sequence
+
         return _assert_sequence
 
-    def assert_mapping(self, item_assertion: Assertions[ValueT, ReturnT]) -> Assertion[Any, MutableMapping[str, ReturnT]]:
+    def assert_mapping(
+        self, item_assertion: Assertions[ValueT, ReturnT]
+    ) -> Assertion[Any, MutableMapping[str, ReturnT]]:
         def _assert_mapping(value: ValueT) -> MutableMapping[str, ReturnT]:
             dict_value = self.assert_dict()(value)
             mapping = {}
             with SerdeErrorCollection().assert_valid() as errors:
                 for value_item_key, value_item_value in dict_value.items():
                     with errors.catch(Str.plain(value_item_key)):
-                        mapping[value_item_key] = self.assert_assertions(item_assertion)(value_item_value)
+                        mapping[value_item_key] = self.assert_assertions(
+                            item_assertion
+                        )(value_item_value)
             return mapping
+
         return _assert_mapping
 
     def assert_fields(self, fields: Fields) -> Assertion[Any, MutableMapping[str, Any]]:
         def _assert_fields(value: Any) -> MutableMapping[str, Any]:
             value_dict = self.assert_dict()(value)
             mapping = {}
             with SerdeErrorCollection().assert_valid() as errors:
                 for field in fields:
                     with errors.catch(Str.plain(field.name)):
                         if field.name in value_dict:
                             if field.assertion:
-                                mapping[field.name] = self.assert_assertions(field.assertion)(value_dict[field.name])
+                                mapping[field.name] = self.assert_assertions(
+                                    field.assertion
+                                )(value_dict[field.name])
                         elif isinstance(field, RequiredField):
-                            raise AssertionFailed(Str._('This field is required.'))
+                            raise AssertionFailed(Str._("This field is required."))
             return mapping
+
         return _assert_fields
 
     @overload
-    def assert_field(self, field: RequiredField[ValueT, ReturnT]) -> Assertion[ValueT, ReturnT]:
+    def assert_field(
+        self, field: RequiredField[ValueT, ReturnT]
+    ) -> Assertion[ValueT, ReturnT]:
         pass
 
     @overload
-    def assert_field(self, field: OptionalField[ValueT, ReturnT]) -> Assertion[ValueT, ReturnT | type[Void]]:
+    def assert_field(
+        self, field: OptionalField[ValueT, ReturnT]
+    ) -> Assertion[ValueT, ReturnT | type[Void]]:
         pass
 
-    def assert_field(self, field: _Field[ValueT, ReturnT]) -> Assertion[ValueT, ReturnT | type[Void]]:
+    def assert_field(
+        self, field: _Field[ValueT, ReturnT]
+    ) -> Assertion[ValueT, ReturnT | type[Void]]:
         def _assert_field(value: Any) -> ReturnT | type[Void]:
             fields = self.assert_fields(Fields(field))(value)
             try:
-                return cast('ReturnT | type[Void]', fields[field.name])
+                return cast("ReturnT | type[Void]", fields[field.name])
             except KeyError:
                 if isinstance(field, RequiredField):
                     raise
                 return Void
+
         return _assert_field
 
     def assert_record(self, fields: Fields) -> Assertion[Any, MutableMapping[str, Any]]:
         if not len(list(fields)):
-            raise ValueError('One or more fields are required.')
+            raise ValueError("One or more fields are required.")
 
         def _assert_record(value: Any) -> MutableMapping[str, Any]:
             dict_value = self.assert_dict()(value)
             known_keys = set(map(lambda x: x.name, fields))
             unknown_keys = set(dict_value.keys()) - known_keys
             with SerdeErrorCollection().assert_valid() as errors:
                 for unknown_key in unknown_keys:
                     with errors.catch(Str.plain(unknown_key)):
-                        raise AssertionFailed(Str._(
-                            'Unknown key: {unknown_key}. Did you mean {known_keys}?',
-                            unknown_key=f'"{unknown_key}"',
-                            known_keys=', '.join(map(lambda x: f'"{x}"', sorted(known_keys)))
-                        ))
+                        raise AssertionFailed(
+                            Str._(
+                                "Unknown key: {unknown_key}. Did you mean {known_keys}?",
+                                unknown_key=f'"{unknown_key}"',
+                                known_keys=", ".join(
+                                    map(lambda x: f'"{x}"', sorted(known_keys))
+                                ),
+                            )
+                        )
                 return self.assert_fields(fields)(dict_value)
+
         return _assert_record
 
     def assert_path(self) -> Assertion[Any, Path]:
         def _assert_path(value: Any) -> Path:
             self.assert_str()(value)
             return Path(value).expanduser().resolve()
+
         return _assert_path
 
     def assert_directory_path(self) -> Assertion[Any, Path]:
         def _assert_directory_path(value: Any) -> Path:
             directory_path = self.assert_path()(value)
             if directory_path.is_dir():
                 return directory_path
-            raise AssertionFailed(Str._(
-                '"{path}" is not a directory.',
-                path=value,
-            ))
+            raise AssertionFailed(
+                Str._(
+                    '"{path}" is not a directory.',
+                    path=value,
+                )
+            )
+
         return _assert_directory_path
 
     def assert_locale(self) -> Assertion[Any, str]:
         def _assert_locale(
             value: Any,
         ) -> str:
             value = self.assert_str()(value)
             try:
                 get_data(value)
                 return value
             except LocaleNotFoundError:
-                raise AssertionFailed(Str._(
-                    '"{locale}" is not a valid IETF BCP 47 language tag.',
-                    locale=value,
-                ))
+                raise AssertionFailed(
+                    Str._(
+                        '"{locale}" is not a valid IETF BCP 47 language tag.',
+                        locale=value,
+                    )
+                )
+
         return _assert_locale
 
-    def assert_setattr(self, instance: object, attr_name: str) -> Assertion[ValueT, ValueT]:
+    def assert_setattr(
+        self, instance: object, attr_name: str
+    ) -> Assertion[ValueT, ValueT]:
         def _assert_setattr(value: ValueT) -> ValueT:
             setattr(instance, attr_name, value)
             return value
+
         return _assert_setattr
 
     def assert_extension_type(self) -> Assertion[Any, type[Extension]]:
         def _assert_extension_type(
             value: Any,
         ) -> type[Extension]:
-            from betty.app.extension import get_extension_type, ExtensionTypeImportError, ExtensionTypeInvalidError, ExtensionTypeError
+            from betty.app.extension import (
+                get_extension_type,
+                ExtensionTypeImportError,
+                ExtensionTypeInvalidError,
+                ExtensionTypeError,
+            )
 
             self.assert_str()(value)
             try:
                 return get_extension_type(value)
             except ExtensionTypeImportError:
                 raise AssertionFailed(
                     Str._(
@@ -345,14 +431,15 @@
             except ExtensionTypeError:
                 raise AssertionFailed(
                     Str._(
                         'Cannot determine the extension type for "{extension_type}". Did you perhaps make a typo, or could it be that the extension type comes from another package that is not yet installed?',
                         extension_type=str(value),
                     )
                 )
+
         return _assert_extension_type
 
     def assert_entity_type(self) -> Assertion[Any, type[Entity]]:
         def _assert_entity_type(
             value: Any,
         ) -> type[Entity]:
             self.assert_str()(value)
@@ -375,8 +462,9 @@
             except EntityTypeError:
                 raise AssertionFailed(
                     Str._(
                         'Cannot determine the entity type for "{entity_type}". Did you perhaps make a typo, or could it be that the entity type comes from another package that is not yet installed?',
                         entity_type=str(value),
                     )
                 )
+
         return _assert_entity_type
```

### Comparing `betty-0.3.3/betty/serve.py` & `betty-0.3.4/betty/serve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide the Serve API to serve resources within the application.
 """
+
 from __future__ import annotations
 
 import contextlib
 import logging
 import threading
 import webbrowser
 from http.server import SimpleHTTPRequestHandler, HTTPServer
@@ -27,15 +28,17 @@
 
 class ServerNotStartedError(RuntimeError):
     pass
 
 
 class NoPublicUrlBecauseServerNotStartedError(ServerNotStartedError):
     def __init__(self):
-        super().__init__('Cannot get the public URL for a server that has not started yet.')
+        super().__init__(
+            "Cannot get the public URL for a server that has not started yet."
+        )
 
 
 class OsError(UserFacingError, OSError):
     pass
 
 
 class Server:
@@ -44,15 +47,15 @@
     """
 
     def __init__(self, localizer: Localizer):
         self._localizer = localizer
 
     @classmethod
     def name(cls) -> str:
-        return f'{cls.__module__}.{cls.__name__}'
+        return f"{cls.__module__}.{cls.__name__}"
 
     @classmethod
     def label(cls) -> Str:
         raise NotImplementedError(repr(cls))
 
     async def start(self) -> None:
         """
@@ -60,17 +63,19 @@
         """
         pass
 
     async def show(self) -> None:
         """
         Show the served site to the user.
         """
-        logging.getLogger(__name__).info(self._localizer._('Serving your site at {url}...').format(
-            url=self.public_url,
-        ))
+        logging.getLogger(__name__).info(
+            self._localizer._("Serving your site at {url}...").format(
+                url=self.public_url,
+            )
+        )
         webbrowser.open_new_tab(self.public_url)
 
     async def stop(self) -> None:
         """
         Stop the server.
         """
         pass
@@ -79,24 +84,31 @@
     def public_url(self) -> str:
         raise NotImplementedError(repr(self))
 
     async def __aenter__(self) -> Server:
         await self.start()
         return self
 
-    async def __aexit__(self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None) -> None:
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
         await self.stop()
 
     async def assert_available(self) -> None:
         # @todo In Betty 0.4.0, require the app's existing client session.
         async with ClientSession() as session:
             try:
                 await Do[Any, None](self._assert_available, session).until()
-            except BaseException:
-                raise UserFacingError(Str._('The server was unreachable after starting.'))
+            except Exception:
+                raise UserFacingError(
+                    Str._("The server was unreachable after starting.")
+                )
 
     async def _assert_available(self, session: ClientSession) -> None:
         async with session.get(self.public_url) as response:
             assert response.status == 200
 
 
 class AppServer(Server):
@@ -105,30 +117,34 @@
         self._app = app
 
     @staticmethod
     def get(app: App) -> AppServer:
         for server in app.servers.values():
             if isinstance(server, AppServer):
                 return server
-        raise RuntimeError(f'Cannot find a project server. This must never happen, because {BuiltinAppServer} should be the fallback.')
+        raise RuntimeError(
+            f"Cannot find a project server. This must never happen, because {BuiltinAppServer} should be the fallback."
+        )
 
     async def start(self) -> None:
-        await makedirs(self._app.project.configuration.www_directory_path, exist_ok=True)
+        await makedirs(
+            self._app.project.configuration.www_directory_path, exist_ok=True
+        )
         await super().start()
 
 
 class ServerProvider:
     @property
     def servers(self) -> Sequence[Server]:
         raise NotImplementedError(repr(self))
 
 
 class _BuiltinServerRequestHandler(SimpleHTTPRequestHandler):
     def end_headers(self) -> None:
-        self.send_header('Cache-Control', 'no-cache')
+        self.send_header("Cache-Control", "no-cache")
         super().end_headers()
 
 
 class BuiltinServer(Server):
     def __init__(
         self,
         www_directory_path: Path,
@@ -138,60 +154,68 @@
     ) -> None:
         super().__init__(localizer)
         self._www_directory_path = www_directory_path
         self._root_path = root_path
         self._http_server: HTTPServer | None = None
         self._port: int | None = None
         self._thread: threading.Thread | None = None
-        self._temporary_root_directory: AiofilesContextManagerTempDir[None, Any, Any] | None = None
+        self._temporary_root_directory: (
+            AiofilesContextManagerTempDir[None, Any, Any] | None
+        ) = None
 
     @classmethod
     def label(cls) -> Str:
-        return Str._('Python built-in')
+        return Str._("Python built-in")
 
     async def start(self) -> None:
         await super().start()
         if self._root_path:
             # To mimic the root path, symlink the project's WWW directory into a temporary
             # directory, so we do not have to make changes to any existing files.
             self._temporary_root_directory = TemporaryDirectory()
-            temporary_root_directory_path = Path(await self._temporary_root_directory.__aenter__())
+            temporary_root_directory_path = Path(
+                await self._temporary_root_directory.__aenter__()
+            )
             temporary_www_directory = temporary_root_directory_path
-            for root_path_component in self._root_path.split('/'):
+            for root_path_component in self._root_path.split("/"):
                 temporary_www_directory /= root_path_component
             if temporary_www_directory != temporary_root_directory_path:
                 await symlink(self._www_directory_path, temporary_www_directory)
             www_directory_path = temporary_root_directory_path
         else:
             www_directory_path = self._www_directory_path
-        logging.getLogger(__name__).info(self._localizer._("Starting Python's built-in web server..."))
+        logging.getLogger(__name__).info(
+            self._localizer._("Starting Python's built-in web server...")
+        )
         for self._port in range(DEFAULT_PORT, 65535):
             with contextlib.suppress(OSError):
                 self._http_server = HTTPServer(
-                    ('', self._port),
+                    ("", self._port),
                     lambda request, client_address, server: _BuiltinServerRequestHandler(
                         request,
                         client_address,
                         server,
                         directory=str(www_directory_path),
                     ),
                 )
                 break
         if self._http_server is None:
-            raise OsError(Str._('Cannot find an available port to bind the web server to.'))
+            raise OsError(
+                Str._("Cannot find an available port to bind the web server to.")
+            )
         self._thread = threading.Thread(target=self._serve)
         self._thread.start()
         await self.assert_available()
 
     @property
     def public_url(self) -> str:
         if self._port is not None:
-            url = f'http://localhost:{self._port}'
+            url = f"http://localhost:{self._port}"
             if self._root_path:
-                url = f'{url}/{self._root_path}'
+                url = f"{url}/{self._root_path}"
             return url
         raise NoPublicUrlBecauseServerNotStartedError()
 
     def _serve(self) -> None:
         with contextlib.redirect_stderr(StringIO()):
             assert self._http_server
             self._http_server.serve_forever()
@@ -209,15 +233,15 @@
 
 class BuiltinAppServer(AppServer):
     def __init__(self, app: App) -> None:
         super().__init__(app)
         self._server = BuiltinServer(
             self._app.project.configuration.www_directory_path,
             root_path=self._app.project.configuration.root_path,
-            localizer=self._app.localizer
+            localizer=self._app.localizer,
         )
 
     @classmethod
     def label(cls) -> Str:
         return BuiltinServer.label()
 
     @property
```

### Comparing `betty-0.3.3/betty/sphinx/extension/replacements.py` & `betty-0.3.4/betty/sphinx/extension/replacements.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 Provide a Sphinx plugin to apply string replacements to source code.
 """
+
 from sphinx.application import Sphinx
 
 
 def render_replacements(app: Sphinx, docname: str, source: list[str]) -> None:
     """
     Handle Sphinx's source-read event to perform string replacements.
     """
-    if app.builder.format != 'html':
+    if app.builder.format != "html":
         return
 
-    for token_name, value in app.env.config['html_context']['betty_replacements'].items():
-        source[0] = source[0].replace('{{{ ' + token_name + ' }}}', value)
+    for token_name, value in app.env.config["html_context"][
+        "betty_replacements"
+    ].items():
+        source[0] = source[0].replace("{{{ " + token_name + " }}}", value)
 
 
 def setup(app: Sphinx) -> None:
     """
     Implement Sphinx's extension setup.
     """
-    app.connect('source-read', render_replacements)
+    app.connect("source-read", render_replacements)
```

### Comparing `betty-0.3.3/betty/string.py` & `betty-0.3.4/betty/string.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 Provide string handling utilities.
 """
+
 import re
 
-_CAMEL_CASE_PATTERN = re.compile(r'(?<!^)(?=[A-Z])')
+_CAMEL_CASE_PATTERN = re.compile(r"(?<!^)(?=[A-Z])")
 
 
 def camel_case_to_snake_case(string: str) -> str:
     """
     Convert camel case to snake case.
     """
-    return _CAMEL_CASE_PATTERN.sub('_', string).lower()
+    return _CAMEL_CASE_PATTERN.sub("_", string).lower()
 
 
 def camel_case_to_kebab_case(string: str) -> str:
     """
     Convert camel case to kebab case.
     """
-    return _CAMEL_CASE_PATTERN.sub('-', string).lower()
+    return _CAMEL_CASE_PATTERN.sub("-", string).lower()
 
 
 def upper_camel_case_to_lower_camel_case(string: str) -> str:
     """
     Convert upper camel case to lower camel case.
     """
     return string[0].lower() + string[1:]
```

### Comparing `betty-0.3.3/betty/subprocess.py` & `betty-0.3.4/betty/subprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide a subprocess API.
 """
+
 import logging
 import os
 from asyncio import create_subprocess_exec, create_subprocess_shell
 from asyncio.subprocess import Process
 from pathlib import Path
 from subprocess import CalledProcessError, PIPE
 from traceback import format_exception
@@ -16,39 +17,53 @@
     shell: bool = False,
 ) -> Process:
     """
     Run a command in a subprocess.
     """
     command = " ".join(runnee)
     logger = logging.getLogger(__name__)
-    logger.debug(f'Running subprocess `{command}`...')
+    logger.debug(f"Running subprocess `{command}`...")
 
     try:
         if shell:
-            process = await create_subprocess_shell(' '.join(runnee), cwd=cwd, stderr=PIPE, stdout=PIPE)
+            process = await create_subprocess_shell(
+                " ".join(runnee), cwd=cwd, stderr=PIPE, stdout=PIPE
+            )
         else:
-            process = await create_subprocess_exec(*runnee, cwd=cwd, stderr=PIPE, stdout=PIPE)
+            process = await create_subprocess_exec(
+                *runnee, cwd=cwd, stderr=PIPE, stdout=PIPE
+            )
         await process.wait()
     except BaseException as error:
-        logger.debug(f'Subprocess `{command}` raised an error:\n{" ".join(format_exception(error))}')
+        logger.debug(
+            f'Subprocess `{command}` raised an error:\n{" ".join(format_exception(error))}'
+        )
         raise
 
     if process.returncode == 0:
         return process
 
     stdout = process.stdout
-    stdout_str = '' if stdout is None else '\n'.join((await stdout.read()).decode().split(os.linesep))
+    stdout_str = (
+        ""
+        if stdout is None
+        else "\n".join((await stdout.read()).decode().split(os.linesep))
+    )
     stderr = process.stderr
-    stderr_str = '' if stderr is None else '\n'.join((await stderr.read()).decode().split(os.linesep))
+    stderr_str = (
+        ""
+        if stderr is None
+        else "\n".join((await stderr.read()).decode().split(os.linesep))
+    )
 
     if stdout_str:
-        logger.debug(f'Subprocess `{command}` stdout:\n{stdout_str}')
+        logger.debug(f"Subprocess `{command}` stdout:\n{stdout_str}")
     if stderr_str:
-        logger.debug(f'Subprocess `{command}` stderr:\n{stderr_str}')
+        logger.debug(f"Subprocess `{command}` stderr:\n{stderr_str}")
 
     assert process.returncode is not None
     raise CalledProcessError(
         process.returncode,
-        ' '.join(runnee),
+        " ".join(runnee),
         stdout_str,
         stderr_str,
     )
```

### Comparing `betty-0.3.3/betty/url.py` & `betty-0.3.4/betty/url.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,97 @@
 """
 Provide a URL generation API.
 """
+
 from __future__ import annotations
 
 from contextlib import suppress
 from typing import Any
 from urllib.parse import quote
 
 from betty.app import App
 from betty.locale import negotiate_locale, Localey, to_locale
 from betty.model import get_entity_type_name, Entity
 from betty.project import ProjectConfiguration
 from betty.string import camel_case_to_kebab_case
 
 
 class LocalizedUrlGenerator:
-    def generate(self, resource: Any, media_type: str, absolute: bool = False, locale: Localey | None = None) -> str:
+    def generate(
+        self,
+        resource: Any,
+        media_type: str,
+        absolute: bool = False,
+        locale: Localey | None = None,
+    ) -> str:
         raise NotImplementedError(repr(self))
 
 
 class StaticUrlGenerator:
-    def generate(self, resource: Any, absolute: bool = False, ) -> str:
+    def generate(
+        self,
+        resource: Any,
+        absolute: bool = False,
+    ) -> str:
         raise NotImplementedError(repr(self))
 
 
 class LocalizedPathUrlGenerator(LocalizedUrlGenerator):
     def __init__(self, app: App):
         self._app = app
 
-    def generate(self, resource: Any, media_type: str, absolute: bool = False, locale: Localey | None = None) -> str:
+    def generate(
+        self,
+        resource: Any,
+        media_type: str,
+        absolute: bool = False,
+        locale: Localey | None = None,
+    ) -> str:
         return _generate_from_path(
             self._app.project.configuration,
             resource,
             absolute,
             self._app.localizer.locale if locale is None else locale,
         )
 
 
 class StaticPathUrlGenerator(StaticUrlGenerator):
     def __init__(self, configuration: ProjectConfiguration):
         self._configuration = configuration
 
-    def generate(self, resource: Any, absolute: bool = False, ) -> str:
+    def generate(
+        self,
+        resource: Any,
+        absolute: bool = False,
+    ) -> str:
         return _generate_from_path(self._configuration, resource, absolute)
 
 
 class _EntityUrlGenerator(LocalizedUrlGenerator):
     def __init__(self, app: App, entity_type: type[Entity]):
         self._app = app
         self._entity_type = entity_type
-        self._pattern = f'{camel_case_to_kebab_case(get_entity_type_name(entity_type))}/{{entity_id}}/index.{{extension}}'
+        self._pattern = f"{camel_case_to_kebab_case(get_entity_type_name(entity_type))}/{{entity_id}}/index.{{extension}}"
 
-    def generate(self, resource: Entity, media_type: str, absolute: bool = False, locale: Localey | None = None) -> str:
+    def generate(
+        self,
+        resource: Entity,
+        media_type: str,
+        absolute: bool = False,
+        locale: Localey | None = None,
+    ) -> str:
         if not isinstance(resource, self._entity_type):
-            raise ValueError('%s is not a %s' % (type(resource), self._entity_type))
+            raise ValueError("%s is not a %s" % (type(resource), self._entity_type))
 
-        if 'text/html' == media_type:
-            extension = 'html'
+        if "text/html" == media_type:
+            extension = "html"
             if locale is None:
                 locale = self._app.localizer.locale
-        elif 'application/json' == media_type:
-            extension = 'json'
+        elif "application/json" == media_type:
+            extension = "json"
             locale = None
         else:
             raise ValueError(f'Unknown entity media type "{media_type}".')
 
         return _generate_from_path(
             self._app.project.configuration,
             self._pattern.format(
@@ -82,38 +109,55 @@
             *(
                 _EntityUrlGenerator(app, entity_type)
                 for entity_type in app.entity_types
             ),
             LocalizedPathUrlGenerator(app),
         ]
 
-    def generate(self, resource: Any, media_type: str, absolute: bool = False, locale: Localey | None = None) -> str:
+    def generate(
+        self,
+        resource: Any,
+        media_type: str,
+        absolute: bool = False,
+        locale: Localey | None = None,
+    ) -> str:
         for generator in self._generators:
             with suppress(ValueError):
                 return generator.generate(resource, media_type, absolute, locale)
-        raise ValueError('No URL generator found for %s.' % (
-            resource if isinstance(resource, str) else type(resource)))
+        raise ValueError(
+            "No URL generator found for %s."
+            % (resource if isinstance(resource, str) else type(resource))
+        )
 
 
-def _generate_from_path(configuration: ProjectConfiguration, path: str, absolute: bool = False, localey: Localey | None = None) -> str:
-    url = configuration.base_url if absolute else ''
-    url += '/'
+def _generate_from_path(
+    configuration: ProjectConfiguration,
+    path: str,
+    absolute: bool = False,
+    localey: Localey | None = None,
+) -> str:
+    url = configuration.base_url if absolute else ""
+    url += "/"
     if configuration.root_path:
-        url += configuration.root_path + '/'
+        url += configuration.root_path + "/"
     if localey and configuration.locales.multilingual:
         locale = to_locale(localey)
         try:
             locale_configuration = configuration.locales[locale]
         except KeyError:
             project_locales = list(configuration.locales)
             try:
                 negotiated_locale_data = negotiate_locale(locale, project_locales)
                 if negotiated_locale_data is None:
                     raise KeyError
-                locale_configuration = configuration.locales[to_locale(negotiated_locale_data)]
+                locale_configuration = configuration.locales[
+                    to_locale(negotiated_locale_data)
+                ]
             except KeyError:
-                raise ValueError(f'Cannot generate URLs in "{locale}", because it cannot be resolved to any of the enabled project locales: {", ".join(project_locales)}')
-        url += locale_configuration.alias + '/'
-    url += path.strip('/')
-    if configuration.clean_urls and url.endswith('/index.html'):
+                raise ValueError(
+                    f'Cannot generate URLs in "{locale}", because it cannot be resolved to any of the enabled project locales: {", ".join(project_locales)}'
+                )
+        url += locale_configuration.alias + "/"
+    url += path.strip("/")
+    if configuration.clean_urls and url.endswith("/index.html"):
         url = url[:-10]
-    return url.rstrip('/')
+    return url.rstrip("/")
```

### Comparing `betty-0.3.3/betty/warnings.py` & `betty-0.3.4/betty/warnings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provide utilities for raising warnings.
 """
+
 import warnings
 
 import typing_extensions
 
 
 class BettyDeprecationWarning(DeprecationWarning):
     """
@@ -26,8 +27,10 @@
     Decorate a class, function, or overload to indicate that it is depreated.
 
     This is identical to :py:class:`warnings.deprecated`, but raises a Betty
     deprecation warning.
     """
 
     def __init__(self, message: str, stacklevel: int = 1):
-        super().__init__(message, category=BettyDeprecationWarning, stacklevel=stacklevel)
+        super().__init__(
+            message, category=BettyDeprecationWarning, stacklevel=stacklevel
+        )
```

### Comparing `betty-0.3.3/betty/wikipedia.py` & `betty-0.3.4/betty/wikipedia.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Fetch information from Wikipedia.
 """
+
 from __future__ import annotations
 
 import asyncio
-import hashlib
 import json
 import logging
 import re
 from collections.abc import Sequence, MutableSequence, Callable, Awaitable
 from contextlib import suppress
 from pathlib import Path
 from time import time
@@ -21,15 +21,23 @@
 
 from betty.app import App
 from betty.asyncio import gather
 from betty.cache import Cache, CacheItemValueT
 from betty.cache.file import BinaryFileCache
 from betty.concurrent import RateLimiter
 from betty.functools import filter_suppress
-from betty.locale import Localized, negotiate_locale, to_locale, get_data, LocaleNotFoundError, Localey
+from betty.hashid import hashid
+from betty.locale import (
+    Localized,
+    negotiate_locale,
+    to_locale,
+    get_data,
+    LocaleNotFoundError,
+    Localey,
+)
 from betty.media_type import MediaType
 from betty.model.ancestry import Link, HasLinks, Place, File, HasFiles
 
 
 class WikipediaError(BaseException):
     pass
 
@@ -38,15 +46,15 @@
     pass
 
 
 class RetrievalError(WikipediaError, RuntimeError):
     pass
 
 
-_URL_PATTERN = re.compile(r'^https?://([a-z]+)\.wikipedia\.org/wiki/([^/?#]+).*$')
+_URL_PATTERN = re.compile(r"^https?://([a-z]+)\.wikipedia\.org/wiki/([^/?#]+).*$")
 
 
 def _parse_url(url: str) -> tuple[str, str]:
     match = _URL_PATTERN.fullmatch(url)
     if match is None:
         raise NotAPageError
     return cast(tuple[str, str], match.groups())
@@ -61,15 +69,15 @@
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def url(self) -> str:
-        return 'https://%s.wikipedia.org/wiki/%s' % (self.locale, self._name)
+        return "https://%s.wikipedia.org/wiki/%s" % (self.locale, self._name)
 
     @property
     def title(self) -> str:
         return self._title
 
     @property
     def content(self) -> str:
@@ -127,47 +135,53 @@
 
     async def _fetch(
         self,
         url: str,
         cache: Cache[CacheItemValueT],
         response_mapper: Callable[[ClientResponse], Awaitable[CacheItemValueT]],
     ) -> tuple[CacheItemValueT, str]:
-        cache_item_id = hashlib.md5(url.encode('utf-8')).hexdigest()
+        cache_item_id = hashid(url)
 
         response_data: CacheItemValueT | None = None
         async with cache.getset(cache_item_id) as (cache_item, setter):
             if cache_item and cache_item.modified + self._ttl > time():
                 response_data = await cache_item.value()
             else:
                 async with self._rate_limiter:
-                    self._logger.debug(f'Fetching {url}...')
+                    self._logger.debug(f"Fetching {url}...")
                     try:
                         async with self._http_client.get(url) as response:
                             response_data = await response_mapper(response)
                     except aiohttp.ClientError as error:
-                        self._logger.warning(f'Could not successfully connect to {url}: {error}')
+                        self._logger.warning(
+                            f"Could not successfully connect to {url}: {error}"
+                        )
                     except asyncio.TimeoutError:
-                        self._logger.warning(f'Timeout when connecting to {url}')
+                        self._logger.warning(f"Timeout when connecting to {url}")
                     else:
                         await setter(response_data)
 
         if response_data is None:
             if cache_item:
                 response_data = await cache_item.value()
             else:
-                raise RetrievalError(f'Could neither fetch {url}, nor find an old version in the cache.')
+                raise RetrievalError(
+                    f"Could neither fetch {url}, nor find an old version in the cache."
+                )
 
         return response_data, cache_item_id
 
     async def fetch(self, url: str) -> str:
         response_data, _ = await self._fetch(url, self._cache, ClientResponse.text)
         return response_data
 
     async def fetch_file(self, url: str) -> Path:
-        _, cache_item_id = await self._fetch(url, self._binary_file_cache, ClientResponse.read)
+        _, cache_item_id = await self._fetch(
+            url, self._binary_file_cache, ClientResponse.read
+        )
         return self._binary_file_cache.cache_item_file_path(cache_item_id)
 
 
 class _Retriever:
     def __init__(
         self,
         http_client: aiohttp.ClientSession,
@@ -179,130 +193,158 @@
         self._fetcher = _Fetcher(http_client, cache, binary_file_cache, ttl)
         self._images: dict[str, Image | None] = {}
 
     async def _get_query_api_data(self, url: str) -> dict[str, Any]:
         response_data = await self._fetcher.fetch(url)
         api_data = json.loads(response_data)
         try:
-            return api_data['query']['pages'][0]  # type: ignore[no-any-return]
+            return api_data["query"]["pages"][0]  # type: ignore[no-any-return]
         except (LookupError, TypeError) as error:
-            raise RetrievalError(f'Could not successfully parse the JSON format returned by {url}: {error}')
+            raise RetrievalError(
+                f"Could not successfully parse the JSON format returned by {url}: {error}"
+            )
 
-    async def _get_page_query_api_data(self, page_language: str, page_name: str) -> dict[str, Any]:
+    async def _get_page_query_api_data(
+        self, page_language: str, page_name: str
+    ) -> dict[str, Any]:
         return await self._get_query_api_data(
-            f'https://{page_language}.wikipedia.org/w/api.php?action=query&titles={quote(page_name)}&prop=langlinks|pageimages|coordinates&lllimit=500&piprop=name&pilicense=free&pilimit=1&coprimary=primary&format=json&formatversion=2'
+            f"https://{page_language}.wikipedia.org/w/api.php?action=query&titles={quote(page_name)}&prop=langlinks|pageimages|coordinates&lllimit=500&piprop=name&pilicense=free&pilimit=1&coprimary=primary&format=json&formatversion=2"
         )
 
-    async def get_translations(self, page_language: str, page_name: str) -> dict[str, str]:
+    async def get_translations(
+        self, page_language: str, page_name: str
+    ) -> dict[str, str]:
         try:
             api_data = await self._get_page_query_api_data(page_language, page_name)
         except RetrievalError as error:
             logger = logging.getLogger(__name__)
             logger.warning(str(error))
             return {}
         try:
-            translations_data = api_data['langlinks']
+            translations_data = api_data["langlinks"]
         except KeyError:
             # There may not be any translations.
             return {}
-        return {translation_data['lang']: translation_data['title'] for translation_data in translations_data}
+        return {
+            translation_data["lang"]: translation_data["title"]
+            for translation_data in translations_data
+        }
 
     async def get_summary(self, page_language: str, page_name: str) -> Summary | None:
         logger = logging.getLogger(__name__)
         try:
-            url = f'https://{page_language}.wikipedia.org/api/rest_v1/page/summary/{page_name}'
+            url = f"https://{page_language}.wikipedia.org/api/rest_v1/page/summary/{page_name}"
             response_data = await self._fetcher.fetch(url)
             try:
                 api_data = json.loads(response_data)
                 return Summary(
                     page_language,
                     page_name,
-                    api_data['titles']['normalized'],
-                    api_data['extract_html'] if 'extract_html' in api_data else api_data['extract'],
+                    api_data["titles"]["normalized"],
+                    (
+                        api_data["extract_html"]
+                        if "extract_html" in api_data
+                        else api_data["extract"]
+                    ),
                 )
             except (json.JSONDecodeError, KeyError) as error:
-                raise RetrievalError(f'Could not successfully parse the JSON content returned by {url}: {error}')
+                raise RetrievalError(
+                    f"Could not successfully parse the JSON content returned by {url}: {error}"
+                )
         except RetrievalError as error:
             logger.warning(str(error))
         return None
 
     async def get_image(self, page_language: str, page_name: str) -> Image | None:
         try:
             api_data = await self._get_page_query_api_data(page_language, page_name)
             try:
-                page_image_name = api_data['pageimage']
+                page_image_name = api_data["pageimage"]
             except KeyError:
                 # There may not be any images.
                 return None
 
             if page_image_name in self._images:
                 return self._images[page_image_name]
 
-            url = f'https://en.wikipedia.org/w/api.php?action=query&prop=imageinfo&titles=File:{quote(page_image_name)}&iiprop=url|mime|canonicaltitle&format=json&formatversion=2'
+            url = f"https://en.wikipedia.org/w/api.php?action=query&prop=imageinfo&titles=File:{quote(page_image_name)}&iiprop=url|mime|canonicaltitle&format=json&formatversion=2"
             image_info_api_data = await self._get_query_api_data(url)
 
             try:
-                image_info = image_info_api_data['imageinfo'][0]
+                image_info = image_info_api_data["imageinfo"][0]
             except KeyError as error:
-                raise RetrievalError(f'Could not successfully parse the JSON content returned by {url}: {error}')
+                raise RetrievalError(
+                    f"Could not successfully parse the JSON content returned by {url}: {error}"
+                )
 
             image = Image(
-                await self._fetcher.fetch_file(image_info['url']),
-                MediaType(image_info['mime']),
+                await self._fetcher.fetch_file(image_info["url"]),
+                MediaType(image_info["mime"]),
                 # Strip "File:" or any translated equivalent from the beginning of the image's title.
-                image_info['canonicaltitle'][image_info['canonicaltitle'].index(':') + 1:],
-                image_info['descriptionurl'],
+                image_info["canonicaltitle"][
+                    image_info["canonicaltitle"].index(":") + 1 :
+                ],
+                image_info["descriptionurl"],
             )
 
             return image
         except RetrievalError as error:
             logger = logging.getLogger(__name__)
             logger.warning(str(error))
             return None
 
-    async def get_place_coordinates(self, page_language: str, page_name: str) -> Point | None:
+    async def get_place_coordinates(
+        self, page_language: str, page_name: str
+    ) -> Point | None:
         api_data = await self._get_page_query_api_data(page_language, page_name)
         try:
-            coordinates = api_data['coordinates'][0]
+            coordinates = api_data["coordinates"][0]
         except KeyError:
             # There may not be any coordinates.
             return None
         try:
-            if coordinates['globe'] != 'earth':
+            if coordinates["globe"] != "earth":
                 return None
-            return Point(coordinates['lat'], coordinates['lon'])
+            return Point(coordinates["lat"], coordinates["lon"])
         except KeyError as error:
-            raise RetrievalError(f'Could not successfully parse the JSON content: {error}')
+            raise RetrievalError(
+                f"Could not successfully parse the JSON content: {error}"
+            )
 
 
 class _Populator:
     def __init__(self, app: App, retriever: _Retriever):
         self._app = app
         self._retriever = retriever
         self._image_files: dict[Image, File] = {}
 
     async def populate(self) -> None:
-        locales = list(map(lambda x: x.alias, self._app.project.configuration.locales.values()))
-        await gather(*(
-            self._populate_entity(entity, locales)
-            for entity
-            in self._app.project.ancestry
-            if isinstance(entity, HasLinks)
-        ))
+        locales = list(
+            map(lambda x: x.alias, self._app.project.configuration.locales.values())
+        )
+        await gather(
+            *(
+                self._populate_entity(entity, locales)
+                for entity in self._app.project.ancestry
+                if isinstance(entity, HasLinks)
+            )
+        )
 
     async def _populate_entity(self, entity: HasLinks, locales: Sequence[str]) -> None:
         await self._populate_has_links(entity, locales)
 
         if isinstance(entity, HasFiles):
             await self._populate_has_files(entity)
 
         if isinstance(entity, Place):
             await self._populate_place(entity)
 
-    async def _populate_has_links(self, has_links: HasLinks, locales: Sequence[str]) -> None:
+    async def _populate_has_links(
+        self, has_links: HasLinks, locales: Sequence[str]
+    ) -> None:
         summary_links: MutableSequence[tuple[str, str]] = []
         for link in has_links.links:
             try:
                 page_language, page_name = _parse_url(link.url)
             except NotAPageError:
                 continue
             else:
@@ -312,56 +354,77 @@
                     continue
                 else:
                     summary_links.append((page_language, page_name))
 
             summary = None
             if link.label is None:
                 with suppress(RetrievalError):
-                    summary = await self._retriever.get_summary(page_language, page_name)
+                    summary = await self._retriever.get_summary(
+                        page_language, page_name
+                    )
             await self.populate_link(link, page_language, summary)
-        await self._populate_has_links_with_translation(has_links, locales, summary_links)
+        await self._populate_has_links_with_translation(
+            has_links, locales, summary_links
+        )
 
-    async def _populate_has_links_with_translation(self, has_links: HasLinks, locales: Sequence[str], summary_links: MutableSequence[tuple[str, str]]) -> None:
+    async def _populate_has_links_with_translation(
+        self,
+        has_links: HasLinks,
+        locales: Sequence[str],
+        summary_links: MutableSequence[tuple[str, str]],
+    ) -> None:
         for page_language, page_name in summary_links:
-            page_translations = await self._retriever.get_translations(page_language, page_name)
+            page_translations = await self._retriever.get_translations(
+                page_language, page_name
+            )
             if len(page_translations) == 0:
                 continue
-            page_translation_locale_datas: Sequence[Localey] = list(filter_suppress(get_data, LocaleNotFoundError, page_translations.keys()))
+            page_translation_locale_datas: Sequence[Localey] = list(
+                filter_suppress(get_data, LocaleNotFoundError, page_translations.keys())
+            )
             for locale in locales:
                 if locale == page_language:
                     continue
-                added_page_locale_data = negotiate_locale(locale, page_translation_locale_datas)
+                added_page_locale_data = negotiate_locale(
+                    locale, page_translation_locale_datas
+                )
                 if added_page_locale_data is None:
                     continue
                 added_page_language = to_locale(added_page_locale_data)
                 added_page_name = page_translations[added_page_language]
                 if (added_page_language, added_page_name) in summary_links:
                     continue
-                added_summary = await self._retriever.get_summary(added_page_language, added_page_name)
+                added_summary = await self._retriever.get_summary(
+                    added_page_language, added_page_name
+                )
                 if not added_summary:
                     continue
                 added_link = Link(added_summary.url)
                 await self.populate_link(added_link, added_page_language, added_summary)
                 has_links.links.append(added_link)
                 summary_links.append((added_page_language, added_page_name))
             return
 
-    async def populate_link(self, link: Link, summary_language: str, summary: Summary | None = None) -> None:
-        if link.url.startswith('http:'):
-            link.url = 'https:' + link.url[5:]
+    async def populate_link(
+        self, link: Link, summary_language: str, summary: Summary | None = None
+    ) -> None:
+        if link.url.startswith("http:"):
+            link.url = "https:" + link.url[5:]
         if link.media_type is None:
-            link.media_type = MediaType('text/html')
+            link.media_type = MediaType("text/html")
         if link.relationship is None:
-            link.relationship = 'external'
+            link.relationship = "external"
         if link.locale is None:
             link.locale = summary_language
         if link.description is None:
             # There are valid reasons for links in locales that aren't supported.
             with suppress(ValueError):
-                link.description = (await self._app.localizers.get_negotiated(link.locale))._('Read more on Wikipedia.')
+                link.description = (
+                    await self._app.localizers.get_negotiated(link.locale)
+                )._("Read more on Wikipedia.")
         if summary is not None and link.label is None:
             link.label = summary.title
 
     async def _populate_place(self, place: Place) -> None:
         await self._populate_place_coordinates(place)
 
     async def _populate_place_coordinates(self, place: Place) -> None:
@@ -370,15 +433,17 @@
 
         for link in place.links:
             try:
                 page_language, page_name = _parse_url(link.url)
             except NotAPageError:
                 continue
             else:
-                coordinates = await self._retriever.get_place_coordinates(page_language, page_name)
+                coordinates = await self._retriever.get_place_coordinates(
+                    page_language, page_name
+                )
                 if coordinates:
                     place.coordinates = coordinates
                     return
 
     async def _populate_has_files(self, has_files: HasFiles & HasLinks) -> None:
         for link in has_files.links:
             try:
@@ -389,28 +454,38 @@
                 image = await self._retriever.get_image(page_language, page_name)
                 if not image:
                     continue
 
                 try:
                     file = self._image_files[image]
                 except KeyError:
-                    file = File(
-                        id=f'wikipedia-{image.title}',
-                        path=image.path,
-                        media_type=image.media_type,
-                        links=[
+                    links = []
+                    for (
+                        locale_configuration
+                    ) in self._app.project.configuration.locales.values():
+                        localizer = await self._app.localizers.get(
+                            locale_configuration.locale
+                        )
+                        links.append(
                             Link(
-                                f'{image.wikimedia_commons_url}?uselang={locale_configuration.alias}',
-                                label=self._app.localizers[locale_configuration.locale]._('Description, licensing, and image history'),
-                                description=self._app.localizers[locale_configuration.locale]._('Find out more about this image on Wikimedia Commons.'),
+                                f"{image.wikimedia_commons_url}?uselang={locale_configuration.alias}",
+                                label=localizer._(
+                                    "Description, licensing, and image history"
+                                ),
+                                description=localizer._(
+                                    "Find out more about this image on Wikimedia Commons."
+                                ),
                                 locale=locale_configuration.locale,
-                                media_type=MediaType('text/html'),
+                                media_type=MediaType("text/html"),
                             )
-                            for locale_configuration
-                            in self._app.project.configuration.locales.values()
-                        ],
+                        )
+                    file = File(
+                        id=f"wikipedia-{image.title}",
+                        path=image.path,
+                        media_type=image.media_type,
+                        links=links,
                     )
                     self._image_files[image] = file
 
                 has_files.files.add(file)
                 self._app.project.ancestry.add(file)
                 return
```

### Comparing `betty-0.3.3/betty.egg-info/PKG-INFO` & `betty-0.3.4/betty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betty
-Version: 0.3.3
+Version: 0.3.4
 Summary: Betty helps you visualize and publish your family history by building interactive genealogy websites out of your Gramps and GECOM family trees
 Author-email: Bart Feenstra <bar@bartfeenstra.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,18 +683,19 @@
 Requires-Dist: pyinstaller>=6.1.0,~=6.1; extra == "pyinstaller"
 Provides-Extra: setuptools
 Requires-Dist: setuptools~=69.0; extra == "setuptools"
 Requires-Dist: twine~=5.0; extra == "setuptools"
 Requires-Dist: wheel>=0.40.0,~=0.40; extra == "setuptools"
 Provides-Extra: test
 Requires-Dist: aioresponses>=0.7.6,~=0.7; extra == "test"
-Requires-Dist: autopep8>=2.0.2,~=2.0; extra == "test"
 Requires-Dist: basedmypy>=2.2.1,~=2.0; extra == "test"
+Requires-Dist: black>=24.4.0,~=24.4; extra == "test"
 Requires-Dist: coverage>=7.2.4,~=7.2; extra == "test"
 Requires-Dist: flake8~=7.0; extra == "test"
+Requires-Dist: flake8-bugbear~=24.4; extra == "test"
 Requires-Dist: html5lib~=1.1; extra == "test"
 Requires-Dist: lxml~=5.0; sys_platform != "win32" and extra == "test"
 Requires-Dist: pip-licenses>=4.3.0,~=4.3; extra == "test"
 Requires-Dist: pydocstyle>=6.3.0,~=6.3; extra == "test"
 Requires-Dist: pytest>=7.3.1,~=7.3; extra == "test"
 Requires-Dist: pytest-aioresponses>=0.2.0,~=0.2; extra == "test"
 Requires-Dist: pytest-asyncio>=0.23.4,~=0.23; extra == "test"
@@ -710,14 +711,15 @@
 Requires-Dist: types-lxml>=2024.3.27; extra == "test"
 Requires-Dist: types-mock>=5.0.0.6,~=5.0; extra == "test"
 Requires-Dist: types-polib>=1.2.0.0,~=1.2; extra == "test"
 Requires-Dist: types-pyinstaller>=6.5.0.20240311,~=6.5; extra == "test"
 Requires-Dist: types-pyyaml>=6.0.6,~=6.0; extra == "test"
 Requires-Dist: types-requests>=2.29.0.0,~=2.29; extra == "test"
 Requires-Dist: types-setuptools~=69.0; extra == "test"
+Requires-Dist: virtualenv~=20.26; extra == "test"
 Requires-Dist: betty[pyinstaller]; extra == "test"
 Requires-Dist: betty[setuptools]; extra == "test"
 Provides-Extra: development
 Requires-Dist: pytest-repeat>=0.9.1,~=0.9; extra == "development"
 Requires-Dist: betty[test]; extra == "development"
 Provides-Extra: ci
 Requires-Dist: codecov>=2.1.12,~=2.1; extra == "ci"
@@ -726,10 +728,14 @@
 # Betty 👵
 
 ![Test status](https://github.com/bartfeenstra/betty/workflows/Test/badge.svg?branch=0.3.x) [![Code coverage](https://codecov.io/gh/bartfeenstra/betty/branch/0.3.x/graph/badge.svg)](https://codecov.io/gh/bartfeenstra/betty) [![PyPI releases](https://badge.fury.io/py/betty.svg)](https://pypi.org/project/betty/) [![Supported Python versions](https://img.shields.io/pypi/pyversions/betty.svg?logo=python&logoColor=FBE072)](https://pypi.org/project/betty/) [![Recent downloads](https://img.shields.io/pypi/dm/betty.svg)](https://pypi.org/project/betty/) [![Follow Betty on Twitter](https://img.shields.io/twitter/follow/Betty_Project.svg?label=Betty_Project&style=flat&logo=twitter&logoColor=4FADFF)](https://twitter.com/Betty_Project)
 
 Betty visualizes and publishes your family history by building interactive, encyclopedia-like genealogy websites out of your
 [Gramps](https://gramps-project.org/) and [GEDCOM](https://en.wikipedia.org/wiki/GEDCOM) family trees.
 
+## View an example site
+
+View a Betty example site at [ancestry.bartfeenstra.com](https://ancestry.bartfeenstra.com).
+
 ## Documentation
 
 View the documentation at [https://betty.readthedocs.io/](https://betty.readthedocs.io/).
```

### Comparing `betty-0.3.3/betty.egg-info/SOURCES.txt` & `betty-0.3.4/betty.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE.txt
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 betty/__init__.py
+betty/_npm.py
 betty/_patch.py
 betty/_resizeimage.py
 betty/about.py
 betty/asyncio.py
 betty/classtools.py
 betty/cli.py
 betty/concurrent.py
@@ -15,40 +17,44 @@
 betty/deriver.py
 betty/dispatch.py
 betty/documentation.py
 betty/error.py
 betty/fs.py
 betty/functools.py
 betty/generate.py
+betty/hashid.py
 betty/html.py
 betty/importlib.py
 betty/job.py
 betty/load.py
 betty/locale.py
 betty/logging.py
 betty/media_type.py
 betty/openapi.py
 betty/os.py
 betty/path.py
 betty/privatizer.py
 betty/project.py
 betty/py.typed
 betty/render.py
+betty/requirement.py
 betty/serve.py
 betty/string.py
 betty/subprocess.py
 betty/url.py
 betty/warnings.py
 betty/wikipedia.py
 betty.egg-info/PKG-INFO
 betty.egg-info/SOURCES.txt
 betty.egg-info/dependency_links.txt
 betty.egg-info/entry_points.txt
 betty.egg-info/requires.txt
 betty.egg-info/top_level.txt
+betty/../.browserslistrc
+betty/../tsconfig.json
 betty/_package/pyinstaller/__init__.py
 betty/_package/pyinstaller/main.py
 betty/_package/pyinstaller/hooks/__init__.py
 betty/_package/pyinstaller/hooks/hook-betty.py
 betty/app/__init__.py
 betty/app/extension/__init__.py
 betty/app/extension/requirement.py
@@ -65,68 +71,51 @@
 betty/assets/public/static/betty-512x512.png
 betty/assets/public/static/betty.ico
 betty/assets/public/static/index.html.j2
 betty/assets/public/static/robots.txt.j2
 betty/assets/templates/base.html.j2
 betty/assets/templates/head.html.j2
 betty/assets/templates/linked-data.html.j2
+betty/assets/templates/scripts.html.j2
 betty/assets/templates/sitemap-index.xml.j2
 betty/assets/templates/sitemap.xml.j2
+betty/assets/templates/stylesheets.html.j2
 betty/assets/templates/entity/page-list.html.j2
 betty/assets/templates/entity/page.html.j2
 betty/cache/__init__.py
 betty/cache/_base.py
 betty/cache/file.py
 betty/cache/memory.py
 betty/extension/__init__.py
 betty/extension/cotton_candy/__init__.py
 betty/extension/cotton_candy/gui.py
 betty/extension/cotton_candy/search.py
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/accessibility.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/citation.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/entity.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.js
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/file.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/main.js
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/main.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/meta.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/overlay.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/package.json
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/page.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/permalink.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/person.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.js
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/search.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/show.js
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/show.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/text.scss
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/variables.scss.j2
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/webpack.config.js
-betty/extension/cotton_candy/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
 betty/extension/cotton_candy/assets/public/localized/index.html.j2
 betty/extension/cotton_candy/assets/public/localized/search-index.json.j2
 betty/extension/cotton_candy/assets/public/static/betty.webmanifest
 betty/extension/cotton_candy/assets/public/static/search-configuration.json.j2
 betty/extension/cotton_candy/assets/templates/base.html.j2
 betty/extension/cotton_candy/assets/templates/event-dimensions.html.j2
 betty/extension/cotton_candy/assets/templates/file-extended--application--pdf.html.j2
 betty/extension/cotton_candy/assets/templates/file-extended--image.html.j2
 betty/extension/cotton_candy/assets/templates/file-extended.html.j2
 betty/extension/cotton_candy/assets/templates/file-summary--application--pdf.html.j2
 betty/extension/cotton_candy/assets/templates/file-summary--image.html.j2
 betty/extension/cotton_candy/assets/templates/file-summary.html.j2
 betty/extension/cotton_candy/assets/templates/file.html.j2
 betty/extension/cotton_candy/assets/templates/footer.html.j2
+betty/extension/cotton_candy/assets/templates/map.html.j2
 betty/extension/cotton_candy/assets/templates/media.html.j2
 betty/extension/cotton_candy/assets/templates/permalink.html.j2
 betty/extension/cotton_candy/assets/templates/references.html.j2
 betty/extension/cotton_candy/assets/templates/section-notes.html.j2
 betty/extension/cotton_candy/assets/templates/show-countable.html.j2
 betty/extension/cotton_candy/assets/templates/show.html.j2
 betty/extension/cotton_candy/assets/templates/timeline.html.j2
+betty/extension/cotton_candy/assets/templates/tree.html.j2
 betty/extension/cotton_candy/assets/templates/entity/featured--place.html.j2
 betty/extension/cotton_candy/assets/templates/entity/featured.html.j2
 betty/extension/cotton_candy/assets/templates/entity/label--citation.html.j2
 betty/extension/cotton_candy/assets/templates/entity/label--event.html.j2
 betty/extension/cotton_candy/assets/templates/entity/label--person-name.html.j2
 betty/extension/cotton_candy/assets/templates/entity/label--person.html.j2
 betty/extension/cotton_candy/assets/templates/entity/label--place.html.j2
@@ -156,44 +145,68 @@
 betty/extension/cotton_candy/assets/templates/macro/citation.html.j2
 betty/extension/cotton_candy/assets/templates/search/result-file.html.j2
 betty/extension/cotton_candy/assets/templates/search/result-person.html.j2
 betty/extension/cotton_candy/assets/templates/search/result-place.html.j2
 betty/extension/cotton_candy/assets/templates/search/result-with-image.html.j2
 betty/extension/cotton_candy/assets/templates/search/result.html.j2
 betty/extension/cotton_candy/assets/templates/search/results.html.j2
+betty/extension/cotton_candy/webpack/accessibility.scss
+betty/extension/cotton_candy/webpack/citation.scss
+betty/extension/cotton_candy/webpack/entity.scss
+betty/extension/cotton_candy/webpack/file.scss
+betty/extension/cotton_candy/webpack/file.ts
+betty/extension/cotton_candy/webpack/main.scss
+betty/extension/cotton_candy/webpack/main.ts
+betty/extension/cotton_candy/webpack/meta.scss
+betty/extension/cotton_candy/webpack/overlay.scss
+betty/extension/cotton_candy/webpack/package.json
+betty/extension/cotton_candy/webpack/page.scss
+betty/extension/cotton_candy/webpack/permalink.scss
+betty/extension/cotton_candy/webpack/person.scss
+betty/extension/cotton_candy/webpack/search.scss
+betty/extension/cotton_candy/webpack/search.ts
+betty/extension/cotton_candy/webpack/show.scss
+betty/extension/cotton_candy/webpack/show.ts
+betty/extension/cotton_candy/webpack/text.scss
+betty/extension/cotton_candy/webpack/variables.scss
 betty/extension/demo/__init__.py
 betty/extension/deriver/__init__.py
 betty/extension/gramps/__init__.py
 betty/extension/gramps/config.py
 betty/extension/gramps/gui.py
 betty/extension/http_api_doc/__init__.py
-betty/extension/http_api_doc/assets/betty.extension.npm._Npm/src/package.json
 betty/extension/http_api_doc/assets/public/static/api/index.html.j2
+betty/extension/http_api_doc/webpack/main.ts
+betty/extension/http_api_doc/webpack/package.json
 betty/extension/maps/__init__.py
-betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.css
-betty/extension/maps/assets/betty.extension.npm._Npm/src/maps.js
-betty/extension/maps/assets/betty.extension.npm._Npm/src/package.json
-betty/extension/maps/assets/betty.extension.npm._Npm/src/webpack.config.js
-betty/extension/maps/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
+betty/extension/maps/webpack/main.css
+betty/extension/maps/webpack/main.ts
+betty/extension/maps/webpack/maps.js
+betty/extension/maps/webpack/package.json
 betty/extension/nginx/__init__.py
 betty/extension/nginx/artifact.py
 betty/extension/nginx/docker.py
 betty/extension/nginx/serve.py
 betty/extension/nginx/assets/Dockerfile
 betty/extension/nginx/assets/content_negotiation.lua
 betty/extension/nginx/assets/nginx.conf.j2
-betty/extension/npm/__init__.py
 betty/extension/privatizer/__init__.py
 betty/extension/trees/__init__.py
-betty/extension/trees/assets/betty.extension.npm._Npm/src/package.json
-betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.css
-betty/extension/trees/assets/betty.extension.npm._Npm/src/trees.js
-betty/extension/trees/assets/betty.extension.npm._Npm/src/webpack.config.js
-betty/extension/trees/assets/betty.extension.npm._Npm/src/webpack.config.json.j2
 betty/extension/trees/assets/public/localized/people.json.j2
+betty/extension/trees/webpack/main.css
+betty/extension/trees/webpack/main.ts
+betty/extension/trees/webpack/package.json
+betty/extension/trees/webpack/trees.js
+betty/extension/webpack/__init__.py
+betty/extension/webpack/build.py
+betty/extension/webpack/assets/templates/webpack-entry-loader.html.j2
+betty/extension/webpack/jinja2/__init__.py
+betty/extension/webpack/jinja2/filter.py
+betty/extension/webpack/webpack/package.json
+betty/extension/webpack/webpack/webpack.config.js
 betty/extension/wikipedia/__init__.py
 betty/extension/wikipedia/assets/templates/wikipedia.html.j2
 betty/gramps/__init__.py
 betty/gramps/error.py
 betty/gramps/loader.py
 betty/gui/__init__.py
 betty/gui/app.py
@@ -218,10 +231,8 @@
 betty/serde/dump.py
 betty/serde/error.py
 betty/serde/format.py
 betty/serde/load.py
 betty/sphinx/__init__.py
 betty/sphinx/extension/__init__.py
 betty/sphinx/extension/replacements.py
-documentation/conf.py
-node_modules/flatted/python/flatted.py
-node_modules/flatted/python/test.py
+documentation/conf.py
```

### Comparing `betty-0.3.3/betty.egg-info/entry_points.txt` & `betty-0.3.4/betty.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `betty-0.3.3/betty.egg-info/requires.txt` & `betty-0.3.4/betty.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,19 @@
 [setuptools]
 setuptools~=69.0
 twine~=5.0
 wheel>=0.40.0,~=0.40
 
 [test]
 aioresponses>=0.7.6,~=0.7
-autopep8>=2.0.2,~=2.0
 basedmypy>=2.2.1,~=2.0
+black>=24.4.0,~=24.4
 coverage>=7.2.4,~=7.2
 flake8~=7.0
+flake8-bugbear~=24.4
 html5lib~=1.1
 pip-licenses>=4.3.0,~=4.3
 pydocstyle>=6.3.0,~=6.3
 pytest>=7.3.1,~=7.3
 pytest-aioresponses>=0.2.0,~=0.2
 pytest-asyncio>=0.23.4,~=0.23
 pytest-cov~=5.0
@@ -60,12 +61,13 @@
 types-lxml>=2024.3.27
 types-mock>=5.0.0.6,~=5.0
 types-polib>=1.2.0.0,~=1.2
 types-pyinstaller>=6.5.0.20240311,~=6.5
 types-pyyaml>=6.0.6,~=6.0
 types-requests>=2.29.0.0,~=2.29
 types-setuptools~=69.0
+virtualenv~=20.26
 betty[pyinstaller]
 betty[setuptools]
 
 [test:sys_platform != "win32"]
 lxml~=5.0
```

### Comparing `betty-0.3.3/documentation/conf.py` & `betty-0.3.4/documentation/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,54 +6,60 @@
 from betty.asyncio import wait_to_thread
 from betty.fs import ROOT_DIRECTORY_PATH, FileSystem
 from betty.locale import LocalizerRepository
 
 betty_replacements: dict[str, str] = {}
 
 assets = FileSystem()
-assets.prepend(fs.ASSETS_DIRECTORY_PATH, 'utf-8')
+assets.prepend(fs.ASSETS_DIRECTORY_PATH, "utf-8")
 localizers = LocalizerRepository(assets)
 for locale in localizers.locales:
     coverage = wait_to_thread(localizers.coverage(locale))
-    betty_replacements[f'translation-coverage-{locale}'] = str(int(round(100 / (coverage[1] / coverage[0]))))
+    betty_replacements[f"translation-coverage-{locale}"] = str(
+        int(round(100 / (coverage[1] / coverage[0])))
+    )
 
 sys.path.insert(0, path.dirname(path.dirname(betty.__file__)))
-project = 'Betty'
-version = wait_to_thread(about.version()) or ''
+project = "Betty"
+version = wait_to_thread(about.version()) or ""
 release = wait_to_thread(about.version_label())
-copyright = 'Bart Feenstra and contributors'
+copyright = "Bart Feenstra and contributors"
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3/', None),
-    'jinja2': ('https://jinja.palletsprojects.com/en/latest/', None),
+    "python": ("https://docs.python.org/3/", None),
+    "jinja2": ("https://jinja.palletsprojects.com/en/latest/", None),
 }
-html_favicon = str(ROOT_DIRECTORY_PATH / 'betty' / 'assets' / 'public' / 'static' / 'betty.ico')
-html_logo = str(ROOT_DIRECTORY_PATH / 'betty' / 'assets' / 'public' / 'static' / 'betty-32x32.png')
+html_favicon = str(
+    ROOT_DIRECTORY_PATH / "betty" / "assets" / "public" / "static" / "betty.ico"
+)
+html_logo = str(
+    ROOT_DIRECTORY_PATH / "betty" / "assets" / "public" / "static" / "betty-32x32.png"
+)
 html_context = {
-    'display_github': True,
-    'github_user': 'bartfeenstra',
-    'github_repo': 'betty',
-    'github_version': '0.3.x',
-    'conf_py_path': '/documentation/',
-    'betty_replacements': betty_replacements,
+    "display_github": True,
+    "github_user": "bartfeenstra",
+    "github_repo": "betty",
+    "github_version": "0.3.x",
+    "conf_py_path": "/documentation/",
+    "betty_replacements": betty_replacements,
 }
-html_theme = 'sphinx_immaterial'
-highlight_language = 'none'
-templates_path = ['_templates']
+html_theme = "sphinx_immaterial"
+highlight_language = "none"
+templates_path = ["_templates"]
 extensions = [
-    'betty.sphinx.extension.replacements',
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosectionlabel',
-    'sphinx.ext.viewcode',
-    'sphinx_autodoc_typehints',
-    'sphinx_design',
-    'sphinx_immaterial',
+    "betty.sphinx.extension.replacements",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosectionlabel",
+    "sphinx.ext.viewcode",
+    "sphinx_autodoc_typehints",
+    "sphinx_design",
+    "sphinx_immaterial",
 ]
 nitpicky = True
-modindex_common_prefix = ['betty.']
+modindex_common_prefix = ["betty."]
 
 # sphinx.ext.autodoc configuration.
-autodoc_member_order = 'alphabetical'
+autodoc_member_order = "alphabetical"
 
 # sphinx_autodoc_typehints configuration.
 set_type_checking_flag = True
 typehints_fully_qualified = True
 always_document_param_types = True
```

### Comparing `betty-0.3.3/pyproject.toml` & `betty-0.3.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -95,18 +95,19 @@
 setuptools = [
     'setuptools ~= 69.0',
     'twine ~= 5.0',
     'wheel ~= 0.40, >= 0.40.0',
 ]
 test = [
     'aioresponses ~= 0.7, >= 0.7.6',
-    'autopep8 ~= 2.0, >= 2.0.2',
     'basedmypy ~= 2.0, >= 2.2.1',
+    'black ~= 24.4, >= 24.4.0',
     'coverage ~= 7.2, >= 7.2.4',
     'flake8 ~= 7.0',
+    'flake8-bugbear ~= 24.4',
     'html5lib ~= 1.1',
     'lxml ~= 5.0; sys.platform != "win32"',
     'pip-licenses ~= 4.3, >= 4.3.0',
     'pydocstyle ~= 6.3, >= 6.3.0',
     'pytest ~= 7.3, >= 7.3.1',
     'pytest-aioresponses ~= 0.2, >= 0.2.0 ',
     'pytest-asyncio ~= 0.23, >= 0.23.4 ',
@@ -122,14 +123,15 @@
     'types-lxml >= 2024.3.27 ',
     'types-mock ~= 5.0, >= 5.0.0.6',
     'types-polib ~= 1.2, >= 1.2.0.0',
     'types-pyinstaller ~= 6.5, >= 6.5.0.20240311',
     'types-pyyaml ~= 6.0, >= 6.0.6',
     'types-requests ~= 2.29, >= 2.29.0.0',
     'types-setuptools ~= 69.0',
+    'virtualenv ~= 20.26',
     'betty[pyinstaller]',
     'betty[setuptools]',
 ]
 development = [
     'pytest-repeat ~= 0.9, >= 0.9.1',
     'betty[test]',
 ]
@@ -147,15 +149,22 @@
     'betty.tests',
     'betty.tests.*',
 ]
 
 [tool.setuptools.package-data]
 betty = [
     'py.typed',
+
+    # Assets.
     'assets/**',
     'extension/*/assets/**',
+
+    # Webpack.
+    '../.browserslistrc',
+    '../tsconfig.json',
+    'extension/*/webpack/**',
 ]
 
 [tool.setuptools.exclude-package-data]
 betty = [
     '__pycache__',
 ]
```

