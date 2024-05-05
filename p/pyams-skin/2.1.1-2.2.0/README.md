# Comparing `tmp/pyams_skin-2.1.1.tar.gz` & `tmp/pyams_skin-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_skin-2.1.1.tar", last modified: Wed Mar 13 17:08:32 2024, max compression
+gzip compressed data, was "dist/pyams_skin-2.2.0.tar", last modified: Sun May  5 19:57:39 2024, max compression
```

## Comparing `pyams_skin-2.1.1.tar` & `pyams_skin-2.2.0.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5323 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)     3758 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2439 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/
--rw-rw-rw-   0 root         (0) root         (0)      859 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    21980 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2445 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/doctests/metas.rst
--rw-rw-rw-   0 root         (0) root         (0)      765 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     1813 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1651 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/form.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/metas.py
--rw-rw-rw-   0 root         (0) root         (0)     3130 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/
--rw-rw-rw-   0 root         (0) root         (0)      927 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/bootstrap-devices-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      888 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/bootstrap-devices-input.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/bootstrap-selection-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1542 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/bootstrap-selection-input.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/button-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1289 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/button-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      412 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/checkbox-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      671 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/checkbox-input.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/close-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      902 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/close-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1242 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/color-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1251 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/color-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1499 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/date-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     2043 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/date-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/dates-range-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/dates-range-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/datetime-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     2018 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/datetime-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1934 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/form-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1673 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/form-group.pt
--rw-rw-rw-   0 root         (0) root         (0)     1393 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/form-tabform.pt
--rw-rw-rw-   0 root         (0) root         (0)     2983 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/form.pt
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/fullpage-modal-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/html-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      937 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/html-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      599 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/http-method-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      703 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/http-method-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/inner-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/modal-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1035 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/object-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1130 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/object-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      480 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/object-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/ordered-list-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      754 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/ordered-list-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/ordered-select-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/password-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1056 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/password-input.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/reset-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      878 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/reset-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1209 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/select-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1762 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/select-input.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/submit-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1005 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/submit-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1488 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/text-copy-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/text-copy-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/text-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1039 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/text-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/textarea-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/textarea-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      653 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/textlines-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/textlines-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     1500 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/time-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     2041 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/time-input.pt
--rw-rw-rw-   0 root         (0) root         (0)      787 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/widget-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     1936 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/view.py
--rw-rw-rw-   0 root         (0) root         (0)     4891 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/viewlet.py
--rw-rw-rw-   0 root         (0) root         (0)    11056 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/interfaces/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.mo
--rw-rw-rw-   0 root         (0) root         (0)     4978 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.po
--rw-rw-rw-   0 root         (0) root         (0)     2751 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/locales/pyams_skin.pot
--rw-rw-rw-   0 root         (0) root         (0)     3620 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/metas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/schema/
--rw-rw-rw-   0 root         (0) root         (0)     4057 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/schema/button.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/tests/
--rw-rw-rw-   0 root         (0) root         (0)      799 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1855 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      564 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2993 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1339 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)     3360 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/breadcrumb.py
--rw-rw-rw-   0 root         (0) root         (0)     1189 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/footer.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/header.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/help.py
--rw-rw-rw-   0 root         (0) root         (0)     2278 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/menu.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/metas.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/prefix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/action.pt
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/actions-menu.pt
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/actions.pt
--rw-rw-rw-   0 root         (0) root         (0)      373 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/alert.pt
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/breadcrumbs.pt
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/errors.pt
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/menu-divider.pt
--rw-rw-rw-   0 root         (0) root         (0)      439 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/menu-dropdown.pt
--rw-rw-rw-   0 root         (0) root         (0)      452 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/menu-item.pt
--rw-rw-rw-   0 root         (0) root         (0)      331 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/widget.pt
--rw-rw-rw-   0 root         (0) root         (0)     1107 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/viewlet/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin/widget/
--rw-rw-rw-   0 root         (0) root         (0)      563 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1146 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/bool.py
--rw-rw-rw-   0 root         (0) root         (0)     5420 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/button.py
--rw-rw-rw-   0 root         (0) root         (0)     1319 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/color.py
--rw-rw-rw-   0 root         (0) root         (0)     4672 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/datetime.py
--rw-rw-rw-   0 root         (0) root         (0)     2586 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/html.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/http.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/list.py
--rw-rw-rw-   0 root         (0) root         (0)     3106 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/select.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-03-13 17:08:06.000000 pyams_skin-2.1.1/src/pyams_skin/widget/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5323 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5208 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 17:08:25.000000 pyams_skin-2.1.1/src/pyams_skin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      180 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-13 17:08:32.000000 pyams_skin-2.1.1/src/pyams_skin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5404 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     3819 2024-05-05 19:55:32.000000 pyams_skin-2.2.0/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2439 2024-05-05 19:55:32.000000 pyams_skin-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/
+-rw-rw-rw-   0 root         (0) root         (0)      859 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    21980 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2445 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/doctests/metas.rst
+-rw-rw-rw-   0 root         (0) root         (0)      765 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1651 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/metas.py
+-rw-rw-rw-   0 root         (0) root         (0)     3130 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/bootstrap-devices-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      888 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/bootstrap-devices-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 19:57:25.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/bootstrap-selection-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/bootstrap-selection-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 19:57:25.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/button-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/button-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      412 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/checkbox-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/checkbox-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 19:57:25.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/close-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      902 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/close-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/color-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/color-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/date-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/date-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/dates-range-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/dates-range-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/datetime-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/datetime-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/form-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/form-group.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/form-tabform.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2983 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/form.pt
+-rw-rw-rw-   0 root         (0) root         (0)      670 2024-05-05 19:55:32.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/fullpage-modal-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/html-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      937 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/html-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      599 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/http-method-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/http-method-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/inner-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-05-05 19:55:32.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/modal-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/object-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/object-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/object-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/ordered-list-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      754 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/ordered-list-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/ordered-select-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/password-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/password-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 19:57:25.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/reset-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/reset-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/select-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/select-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 19:57:25.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/submit-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/submit-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/text-copy-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/text-copy-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/text-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/text-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/textarea-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/textarea-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      653 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/textlines-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/textlines-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/time-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/time-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)      787 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/widget-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2024-05-05 19:55:32.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/view.py
+-rw-rw-rw-   0 root         (0) root         (0)     4891 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/viewlet.py
+-rw-rw-rw-   0 root         (0) root         (0)    11056 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/interfaces/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.mo
+-rw-rw-rw-   0 root         (0) root         (0)     4978 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.po
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/locales/pyams_skin.pot
+-rw-rw-rw-   0 root         (0) root         (0)     3620 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/metas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     4057 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/schema/button.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1855 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      564 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2993 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)     3360 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/breadcrumb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1189 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/footer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/help.py
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/menu.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/metas.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/prefix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/action.pt
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/actions-menu.pt
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/actions.pt
+-rw-rw-rw-   0 root         (0) root         (0)      373 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/alert.pt
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/breadcrumbs.pt
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/errors.pt
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/menu-divider.pt
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/menu-dropdown.pt
+-rw-rw-rw-   0 root         (0) root         (0)      452 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/menu-item.pt
+-rw-rw-rw-   0 root         (0) root         (0)      331 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/widget.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/viewlet/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/bool.py
+-rw-rw-rw-   0 root         (0) root         (0)     5420 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/button.py
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/color.py
+-rw-rw-rw-   0 root         (0) root         (0)     4672 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3106 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/select.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-03-13 17:08:07.000000 pyams_skin-2.2.0/src/pyams_skin/widget/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5404 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5208 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-05 19:57:39.000000 pyams_skin-2.2.0/src/pyams_skin.egg-info/top_level.txt
```

### Comparing `pyams_skin-2.1.1/LICENSE` & `pyams_skin-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/PKG-INFO` & `pyams_skin-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyams_skin
-Version: 2.1.1
+Version: 2.2.0
 Summary: PyAMS base skin management features
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: test
@@ -47,14 +48,18 @@
 It also provides a small set of custom form widgets and buttons, and overrides default templates
 of many widgets provided by PyAMS_form package.
 
 
 Changelog
 =========
 
+2.2.0
+-----
+ - added support for custom modal content class
+
 2.1.1
 -----
  - added translation for Bootstrap status labels
 
 2.1.0
 -----
  - updated modal page layout
@@ -228,7 +233,9 @@
 1.0.1
 -----
  - updated Gitlab-CI configuration
 
 1.0.0
 -----
  - initial release
+
+
```

### Comparing `pyams_skin-2.1.1/docs/HISTORY.rst` & `pyams_skin-2.2.0/docs/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+2.2.0
+-----
+ - added support for custom modal content class
+
 2.1.1
 -----
  - added translation for Bootstrap status labels
 
 2.1.0
 -----
  - updated modal page layout
```

### Comparing `pyams_skin-2.1.1/docs/README.rst` & `pyams_skin-2.2.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/setup.py` & `pyams_skin-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.1.1'
+version = '2.2.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_skin-2.1.1/src/pyams_skin/__init__.py` & `pyams_skin-2.2.0/src/pyams_skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/doctests/README.rst` & `pyams_skin-2.2.0/src/pyams_skin/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/doctests/metas.rst` & `pyams_skin-2.2.0/src/pyams_skin/doctests/metas.rst`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/include.py` & `pyams_skin-2.2.0/src/pyams_skin/include.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/__init__.py` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/form.py` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/form.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/metas.py` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/metas.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/schema.py` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/schema.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/bootstrap-devices-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/bootstrap-devices-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/bootstrap-devices-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/bootstrap-devices-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/bootstrap-selection-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/bootstrap-selection-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/button-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/button-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/checkbox-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/checkbox-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/close-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/close-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/color-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/color-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/color-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/color-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/date-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/date-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/date-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/date-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/dates-range-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/dates-range-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/datetime-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/datetime-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/datetime-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/datetime-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/form-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/form-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/form-group.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/form-group.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/form-tabform.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/form-tabform.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/form.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/form.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/html-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/html-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/http-method-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/http-method-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/http-method-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/http-method-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/modal-layout.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/modal-layout.pt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div class="modal-dialog ${view.modal_class | ''}">
-	<div class="modal-content">
+	<div class="modal-content ${view.modal_content_class | ''}">
 		<h4 class="modal-header bg-secondary-modal mb-0">
 			<span class="d-block">
 				<i tal:omit-tag="">${structure:request.localizer.translate(view.title)}</i>
 			</span>
 			<button type="button" class="close"
 					data-dismiss="modal" aria-label="Close">
 				<i class="far fa-times-circle" aria-hidden="true"></i>
```

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/object-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/object-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/object-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/object-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/ordered-list-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/ordered-list-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/ordered-select-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/ordered-select-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/password-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/password-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/password-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/password-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/reset-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/reset-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/select-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/select-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/select-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/select-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/submit-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/submit-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/text-copy-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/text-copy-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/text-copy-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/text-copy-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/text-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/text-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/text-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/text-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/textarea-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/textarea-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/textlines-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/textlines-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/textlines-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/textlines-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/time-display.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/time-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/time-input.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/time-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/templates/widget-layout.pt` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/templates/widget-layout.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/view.py` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/view.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,27 +34,33 @@
 @layout_config(template='templates/fullpage-modal-layout.pt', layer=IPyAMSLayer)
 class IModalFullPage(IFullPage):
     """Full page modal dialog view marker interface"""
 
     modal_class = TextLine(title="Modal dialog CSS class",
                            default='modal-lg')
 
+    modal_content_class = TextLine(title="Modal dialog content CSS class",
+                                   default='')
+
 
 @layout_config(template='templates/inner-layout.pt', layer=IPyAMSLayer)
 class IInnerPage(IView):
     """Inner page view marker interface"""
 
 
 @layout_config(template='templates/modal-layout.pt', layer=IPyAMSLayer)
 class IModalPage(IView):
     """Modal page view marker interface"""
 
     modal_class = TextLine(title="Modal dialog CSS class",
                            default='modal-lg')
 
+    modal_content_class = TextLine(title="Modal dialog content CSS class",
+                                   default='')
+
 
 class IModalAddForm(IModalPage):
     """Modal add form marker interface"""
 
 
 class IModalEditForm(IModalPage):
     """Modal edit form marker interface"""
```

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/viewlet.py` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/interfaces/widget.py` & `pyams_skin-2.2.0/src/pyams_skin/interfaces/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.mo` & `pyams_skin-2.2.0/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.mo`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.po` & `pyams_skin-2.2.0/src/pyams_skin/locales/fr/LC_MESSAGES/pyams_skin.po`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/locales/pyams_skin.pot` & `pyams_skin-2.2.0/src/pyams_skin/locales/pyams_skin.pot`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/metas.py` & `pyams_skin-2.2.0/src/pyams_skin/metas.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/schema/__init__.py` & `pyams_skin-2.2.0/src/pyams_skin/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/schema/button.py` & `pyams_skin-2.2.0/src/pyams_skin/schema/button.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/tests/__init__.py` & `pyams_skin-2.2.0/src/pyams_skin/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/tests/test_utilsdocs.py` & `pyams_skin-2.2.0/src/pyams_skin/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/tests/test_utilsdocstrings.py` & `pyams_skin-2.2.0/src/pyams_skin/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/__init__.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/actions.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/actions.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/bootstrap.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/breadcrumb.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/errors.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/errors.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/footer.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/footer.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/header.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/header.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/help.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/help.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/menu.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/menu.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/metas.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/metas.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/prefix.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/prefix.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/action.pt` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/action.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/templates/errors.pt` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/templates/errors.pt`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/viewlet/widget.py` & `pyams_skin-2.2.0/src/pyams_skin/viewlet/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/__init__.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/bool.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/bool.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/bootstrap.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/button.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/button.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/color.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/color.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/datetime.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/datetime.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/html.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/html.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/http.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/http.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/list.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/select.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/select.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin/widget/text.py` & `pyams_skin-2.2.0/src/pyams_skin/widget/text.py`

 * *Files identical despite different names*

### Comparing `pyams_skin-2.1.1/src/pyams_skin.egg-info/PKG-INFO` & `pyams_skin-2.2.0/src/pyams_skin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyams-skin
-Version: 2.1.1
+Version: 2.2.0
 Summary: PyAMS base skin management features
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Framework :: Pyramid
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: test
@@ -47,14 +48,18 @@
 It also provides a small set of custom form widgets and buttons, and overrides default templates
 of many widgets provided by PyAMS_form package.
 
 
 Changelog
 =========
 
+2.2.0
+-----
+ - added support for custom modal content class
+
 2.1.1
 -----
  - added translation for Bootstrap status labels
 
 2.1.0
 -----
  - updated modal page layout
@@ -228,7 +233,9 @@
 1.0.1
 -----
  - updated Gitlab-CI configuration
 
 1.0.0
 -----
  - initial release
+
+
```

### Comparing `pyams_skin-2.1.1/src/pyams_skin.egg-info/SOURCES.txt` & `pyams_skin-2.2.0/src/pyams_skin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

