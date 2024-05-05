# Comparing `tmp/bootstrap_email-0.3.0.tar.gz` & `tmp/bootstrap_email-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootstrap_email-0.3.0.tar", last modified: Thu Apr 25 16:08:17 2024, max compression
+gzip compressed data, was "bootstrap_email-0.4.0.tar", last modified: Sun May  5 15:04:49 2024, max compression
```

## Comparing `bootstrap_email-0.3.0.tar` & `bootstrap_email-0.4.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.115337 bootstrap_email-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-25 16:08:17.115337 bootstrap_email-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.103337 bootstrap_email-0.3.0/bootstrap_email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/bootstrap-email.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/bootstrap-head.scss
--rw-r--r--   0 runner    (1001) docker     (127)    21441 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.103337 bootstrap_email-0.3.0/bootstrap_email/scss/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/_helpers.scss
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/_reboot_email.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/_reboot_head.scss
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/_variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.103337 bootstrap_email-0.3.0/bootstrap_email/scss/components/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_alert.scss
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_badge.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_button.scss
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_card.scss
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_container.scss
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_grid.scss
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_hr.scss
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_image.scss
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_preview.scss
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_stack.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/components/_table.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.103337 bootstrap_email-0.3.0/bootstrap_email/scss/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/helpers/_functions.scss
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/helpers/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/helpers/_selectors_for_utils.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.107337 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_background.scss
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_border-radius.scss
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_border.scss
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_color.scss
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_display.scss
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_sizing.scss
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_spacing.scss
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_text-decoration.scss
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_valign.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.107337 bootstrap_email-0.3.0/bootstrap_email/scss/variables/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/variables/_body.scss
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/variables/_borders.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/variables/_buttons.scss
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/variables/_colors.scss
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/variables/_tables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/variables/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/scss/variables/_utilities.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.107337 bootstrap_email-0.3.0/bootstrap_email/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/templates/body.html
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/templates/container.html
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/templates/div.html
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/templates/table-left.html
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/templates/table-to-tbody.html
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/templates/table-to-tr.html
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/templates/table.html
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/templates/td.html
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/bootstrap_email/templates/tr.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.115337 bootstrap_email-0.3.0/bootstrap_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-25 16:08:17.000000 bootstrap_email-0.3.0/bootstrap_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-25 16:08:17.000000 bootstrap_email-0.3.0/bootstrap_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 16:08:17.000000 bootstrap_email-0.3.0/bootstrap_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-25 16:08:17.000000 bootstrap_email-0.3.0/bootstrap_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-25 16:08:17.000000 bootstrap_email-0.3.0/bootstrap_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 16:08:17.115337 bootstrap_email-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.111337 bootstrap_email-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.099337 bootstrap_email-0.3.0/tests/input/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.111337 bootstrap_email-0.3.0/tests/input/end-to-end/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/end-to-end/receipt.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.111337 bootstrap_email-0.3.0/tests/input/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/alert.html
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/align.html
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/badge.html
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/block.html
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/body.html
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/button.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/card.html
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/container-fluid.html
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/container.html
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/hr.html
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/padding.html
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/preview.html
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/spacing-2.html
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/spacing.html
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/stack.html
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/input/integration/table.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.099337 bootstrap_email-0.3.0/tests/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.111337 bootstrap_email-0.3.0/tests/output/end-to-end/
--rw-r--r--   0 runner    (1001) docker     (127)    27846 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/end-to-end/receipt.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 16:08:17.115337 bootstrap_email-0.3.0/tests/output/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/alert.html
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/align.html
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/badge.html
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/block.html
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/body.html
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/button.html
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/card.html
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/container-fluid.html
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/container.html
--rw-r--r--   0 runner    (1001) docker     (127)    14650 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/grid.html
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/hr.html
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/padding.html
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/preview.html
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/spacing-2.html
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/spacing.html
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/stack.html
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/output/integration/table.html
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-25 16:08:09.000000 bootstrap_email-0.3.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.093309 bootstrap_email-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-05 15:04:49.093309 bootstrap_email-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.077309 bootstrap_email-0.4.0/bootstrap_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/bootstrap-email.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/bootstrap-head.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    21441 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.077309 bootstrap_email-0.4.0/bootstrap_email/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/_helpers.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/_reboot_email.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/_reboot_head.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/_variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.081309 bootstrap_email-0.4.0/bootstrap_email/scss/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_alert.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_badge.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_button.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_card.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_container.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_grid.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_hr.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_image.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_preview.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_stack.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/components/_table.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.081309 bootstrap_email-0.4.0/bootstrap_email/scss/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/helpers/_functions.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/helpers/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/helpers/_selectors_for_utils.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.081309 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_background.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_border-radius.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_border.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_color.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_display.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_sizing.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_spacing.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_text-decoration.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_valign.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.085309 bootstrap_email-0.4.0/bootstrap_email/scss/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/variables/_body.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/variables/_borders.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/variables/_buttons.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/variables/_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/variables/_tables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/variables/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/scss/variables/_utilities.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.085309 bootstrap_email-0.4.0/bootstrap_email/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/templates/body.html
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/templates/container.html
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/templates/div.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/templates/table-left.html
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/templates/table-to-tbody.html
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/templates/table-to-tr.html
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/templates/table.html
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/templates/td.html
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/bootstrap_email/templates/tr.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.089310 bootstrap_email-0.4.0/bootstrap_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-05 15:04:49.000000 bootstrap_email-0.4.0/bootstrap_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-05 15:04:49.000000 bootstrap_email-0.4.0/bootstrap_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 15:04:49.000000 bootstrap_email-0.4.0/bootstrap_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-05 15:04:49.000000 bootstrap_email-0.4.0/bootstrap_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 15:04:49.000000 bootstrap_email-0.4.0/bootstrap_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 15:04:49.093309 bootstrap_email-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.085309 bootstrap_email-0.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.077309 bootstrap_email-0.4.0/tests/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.085309 bootstrap_email-0.4.0/tests/input/end-to-end/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/end-to-end/receipt.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.089310 bootstrap_email-0.4.0/tests/input/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/align.html
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/badge.html
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/block.html
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/body.html
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/button.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/card.html
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/container-fluid.html
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/container.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/hr.html
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/padding.html
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/preview.html
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/spacing-2.html
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/spacing.html
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/stack.html
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/input/integration/table.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.077309 bootstrap_email-0.4.0/tests/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.089310 bootstrap_email-0.4.0/tests/output/end-to-end/
+-rw-r--r--   0 runner    (1001) docker     (127)    27846 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/end-to-end/receipt.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:04:49.089310 bootstrap_email-0.4.0/tests/output/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/align.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/badge.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/block.html
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/body.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/button.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/card.html
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/container-fluid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/container.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14650 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/grid.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/hr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/padding.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/preview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/spacing-2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/spacing.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/stack.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/output/integration/table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-05 15:04:42.000000 bootstrap_email-0.4.0/tests/test.py
```

### Comparing `bootstrap_email-0.3.0/LICENSE` & `bootstrap_email-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/PKG-INFO` & `bootstrap_email-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootstrap-email
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python port of the bootstrap-email Ruby library - Bootstrap 5+ stylesheet, compiler, and inliner for responsive and consistent emails with the Bootstrap syntax you know and love.
 Author: Jeremy Thompson
 License: MIT License
         
         Copyright (c) 2023 Jeremy Thompson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bootstrap_email-0.3.0/bootstrap_email/bootstrap-email.scss` & `bootstrap_email-0.4.0/bootstrap_email/bootstrap-email.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/bootstrap-head.scss` & `bootstrap_email-0.4.0/bootstrap_email/bootstrap-head.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/compiler.py` & `bootstrap_email-0.4.0/bootstrap_email/compiler.py`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/_reboot_email.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/_reboot_email.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/_reboot_head.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/_reboot_head.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/components/_button.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/components/_button.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/components/_grid.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/components/_grid.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/components/_stack.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/components/_stack.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/components/_table.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/components/_table.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/helpers/_functions.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/helpers/_functions.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/helpers/_mixins.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/helpers/_mixins.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/helpers/_selectors_for_utils.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/helpers/_selectors_for_utils.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_border-radius.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_border.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_border.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_sizing.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_sizing.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/utilities/_typography.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/utilities/_typography.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/variables/_buttons.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/variables/_buttons.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/variables/_colors.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/variables/_colors.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/variables/_typography.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/variables/_typography.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/scss/variables/_utilities.scss` & `bootstrap_email-0.4.0/bootstrap_email/scss/variables/_utilities.scss`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email/templates/container.html` & `bootstrap_email-0.4.0/bootstrap_email/templates/container.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/bootstrap_email.egg-info/PKG-INFO` & `bootstrap_email-0.4.0/bootstrap_email.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootstrap-email
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python port of the bootstrap-email Ruby library - Bootstrap 5+ stylesheet, compiler, and inliner for responsive and consistent emails with the Bootstrap syntax you know and love.
 Author: Jeremy Thompson
 License: MIT License
         
         Copyright (c) 2023 Jeremy Thompson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `bootstrap_email-0.3.0/bootstrap_email.egg-info/SOURCES.txt` & `bootstrap_email-0.4.0/bootstrap_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/pyproject.toml` & `bootstrap_email-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bootstrap-email"
-version = "0.3.0"
+version = "0.4.0"
 description = "Python port of the bootstrap-email Ruby library - Bootstrap 5+ stylesheet, compiler, and inliner for responsive and consistent emails with the Bootstrap syntax you know and love."
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [{name = "Jeremy Thompson"}]
 license = {file = "LICENSE"}
 dependencies = [
     "premailer",
```

### Comparing `bootstrap_email-0.3.0/tests/input/end-to-end/receipt.html` & `bootstrap_email-0.4.0/tests/input/end-to-end/receipt.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/input/integration/grid.html` & `bootstrap_email-0.4.0/tests/input/integration/grid.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/input/integration/table.html` & `bootstrap_email-0.4.0/tests/input/integration/table.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/end-to-end/receipt.html` & `bootstrap_email-0.4.0/tests/output/end-to-end/receipt.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/alert.html` & `bootstrap_email-0.4.0/tests/output/integration/alert.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/align.html` & `bootstrap_email-0.4.0/tests/output/integration/align.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/badge.html` & `bootstrap_email-0.4.0/tests/output/integration/badge.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/block.html` & `bootstrap_email-0.4.0/tests/output/integration/block.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/body.html` & `bootstrap_email-0.4.0/tests/output/integration/body.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/button.html` & `bootstrap_email-0.4.0/tests/output/integration/button.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/card.html` & `bootstrap_email-0.4.0/tests/output/integration/card.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/container-fluid.html` & `bootstrap_email-0.4.0/tests/output/integration/container-fluid.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/container.html` & `bootstrap_email-0.4.0/tests/output/integration/container.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/grid.html` & `bootstrap_email-0.4.0/tests/output/integration/grid.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/hr.html` & `bootstrap_email-0.4.0/tests/output/integration/hr.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/padding.html` & `bootstrap_email-0.4.0/tests/output/integration/padding.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/preview.html` & `bootstrap_email-0.4.0/tests/output/integration/preview.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/spacing-2.html` & `bootstrap_email-0.4.0/tests/output/integration/spacing-2.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/spacing.html` & `bootstrap_email-0.4.0/tests/output/integration/spacing.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/stack.html` & `bootstrap_email-0.4.0/tests/output/integration/stack.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/output/integration/table.html` & `bootstrap_email-0.4.0/tests/output/integration/table.html`

 * *Files identical despite different names*

### Comparing `bootstrap_email-0.3.0/tests/test.py` & `bootstrap_email-0.4.0/tests/test.py`

 * *Files identical despite different names*

