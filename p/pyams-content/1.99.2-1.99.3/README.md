# Comparing `tmp/pyams_content-1.99.2.tar.gz` & `tmp/pyams_content-1.99.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_content-1.99.2.tar", last modified: Sun Apr 28 15:31:16 2024, max compression
+gzip compressed data, was "dist/pyams_content-1.99.3.tar", last modified: Sun May  5 21:03:27 2024, max compression
```

## Comparing `pyams_content-1.99.2.tar` & `pyams_content-1.99.3.tar`

### file list

```diff
@@ -1,659 +1,659 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-02-26 23:15:27.000000 pyams_content-1.99.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-02-26 23:15:27.000000 pyams_content-1.99.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2488 2024-04-28 15:31:16.000000 pyams_content-1.99.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/docs/
--rwxrwxrwx   0 root         (0) root         (0)      655 2024-04-28 15:24:34.000000 pyams_content-1.99.2/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-02-26 23:15:27.000000 pyams_content-1.99.2/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-28 15:31:16.000000 pyams_content-1.99.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3377 2024-04-28 15:24:34.000000 pyams_content-1.99.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/association/
--rw-rw-rw-   0 root         (0) root         (0)     3402 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4072 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3230 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2091 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2162 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1514 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/templates/association-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1960 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/skin/templates/association-viewlet.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/association/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5882 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9011 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/association/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2039 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/association/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/calendar/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/cards/
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2619 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/templates/cards-masonry.pt
--rw-rw-rw-   0 root         (0) root         (0)     1773 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/skin/templates/cards.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/cards/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2094 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/cards/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/contact/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/component/contact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/
--rw-rw-rw-   0 root         (0) root         (0)     7387 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4426 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     9775 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2467 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3254 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt
--rw-rw-rw-   0 root         (0) root         (0)     2798 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/
--rw-rw-rw-   0 root         (0) root         (0)      571 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3504 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5218 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/mail.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/fields/handler/zmi/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1814 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/templates/form-submit.pt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/skin/templates/paragraph-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/fields/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/fields/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/file/
--rw-rw-rw-   0 root         (0) root         (0)     1583 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/frame/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/component/frame/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/frame/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/
--rw-rw-rw-   0 root         (0) root         (0)     6052 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4672 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/file.py
--rw-rw-rw-   0 root         (0) root         (0)     5095 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     1661 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4654 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2175 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt
--rw-rw-rw-   0 root         (0) root         (0)     2954 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1242 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/zmi/templates/gallery-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/
--rw-rw-rw-   0 root         (0) root         (0)     4053 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt
--rw-rw-rw-   0 root         (0) root         (0)     2891 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1185 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-random.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8399 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11894 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/file.py
--rw-rw-rw-   0 root         (0) root         (0)     1995 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/
--rw-rw-rw-   0 root         (0) root         (0)     7780 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4725 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2005 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6710 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2989 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1390 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     2530 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1328 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/zmi/templates/illustration-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6234 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4472 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/illustration.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2087 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/illustration-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     2388 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/illustration-side.pt
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     5108 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5143 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/paragraph.py
--rw-rw-rw-   0 root         (0) root         (0)     1989 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/keynumber/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/keynumber/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/links/
--rw-rw-rw-   0 root         (0) root         (0)    10891 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4819 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/html.py
--rw-rw-rw-   0 root         (0) root         (0)     5037 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/links/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8653 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2658 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/links/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/map/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/map/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/milestone/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/milestone/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/
--rw-rw-rw-   0 root         (0) root         (0)     6756 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5966 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/container.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     5173 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/interfaces/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4693 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5340 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     7591 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4105 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      606 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/templates/navigation-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7323 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/interfaces/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      899 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/templates/html.pt
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/templates/raw-code.pt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/templates/raw.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    17744 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17906 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     4263 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/html.py
--rw-rw-rw-   0 root         (0) root         (0)     1494 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/templates/title-toolbar.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/pictogram/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/component/pictogram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/
--rw-rw-rw-   0 root         (0) root         (0)     7603 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2699 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/skin/templates/tags.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    12144 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     6509 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/verbatim/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/component/verbatim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/
--rw-rw-rw-   0 root         (0) root         (0)     2307 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/
--rw-rw-rw-   0 root         (0) root         (0)     2984 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3286 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/dailymotion.py
--rw-rw-rw-   0 root         (0) root         (0)     9322 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2895 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/vimeo.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/provider/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2151 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/
--rw-rw-rw-   0 root         (0) root         (0)     2159 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/dailymotion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/custom-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      450 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/dailymotion-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      542 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/youtube-render.pt
--rw-rw-rw-   0 root         (0) root         (0)     1503 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/vimeo.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/youtube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/skin/templates/video-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/component/video/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12014 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/component/video/zmi/paragraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/doctests/
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/
--rw-rw-rw-   0 root         (0) root         (0)     3608 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2142 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1882 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/skin/templates/alerts.pt
--rw-rw-rw-   0 root         (0) root         (0)     1098 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/skin/templates/context-alerts.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2205 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/alert/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/audit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/feature/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6737 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1803 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/sitemap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/glossary-sitemap.pt
--rw-rw-rw-   0 root         (0) root         (0)      929 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/glossary.pt
--rw-rw-rw-   0 root         (0) root         (0)     1731 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-associations.pt
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-body.pt
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-footer.pt
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      767 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     3568 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/term.py
--rw-rw-rw-   0 root         (0) root         (0)     3180 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3093 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/glossary/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/history/
--rw-rw-rw-   0 root         (0) root         (0)     3000 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/history/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/history/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/history/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/history/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/history/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/history/zmi/templates/history.pt
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/history/zmi/viewlet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/html/
--rw-rw-rw-   0 root         (0) root         (0)     3125 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/html/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/
--rw-rw-rw-   0 root         (0) root         (0)     6800 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     3392 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     3551 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2154 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1339 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3353 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7344 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/container.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/
--rw-rw-rw-   0 root         (0) root         (0)      570 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2670 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/qrcode/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/feature/qrcode/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/redirect/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/feature/redirect/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/renderer/
--rw-rw-rw-   0 root         (0) root         (0)     5451 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/renderer/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/review/
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3253 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/chat.py
--rw-rw-rw-   0 root         (0) root         (0)     3206 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4664 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    11045 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/comment.pt
--rw-rw-rw-   0 root         (0) root         (0)     2784 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/comments.pt
--rw-rw-rw-   0 root         (0) root         (0)     1787 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/mail-notification.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/
--rw-rw-rw-   0 root         (0) root         (0)     3169 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7419 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3804 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/search/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4861 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2527 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)    11035 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6230 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1282 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt
--rw-rw-rw-   0 root         (0) root         (0)     5146 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt
--rw-rw-rw-   0 root         (0) root         (0)     5176 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt
--rw-rw-rw-   0 root         (0) root         (0)     4985 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1187 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt
--rw-rw-rw-   0 root         (0) root         (0)     5184 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt
--rw-rw-rw-   0 root         (0) root         (0)     4002 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/zmi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1258 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      708 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     4276 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/search/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/search/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     7625 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3101 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/search/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/zmi/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     3955 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/feature/search/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/share/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/feature/share/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/
--rw-rw-rw-   0 root         (0) root         (0)     4558 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/templates/
--rw-rw-rw-   0 root         (0) root         (0)      299 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/templates/humans.pt
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/templates/robots.pt
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/templates/root-sitemap.pt
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/feature/sitemap/templates/tool-sitemap.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/feature/toolbox/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/feature/toolbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/generations/
--rw-rw-rw-   0 root         (0) root         (0)    10545 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9656 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     4659 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)   124893 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo
--rw-rw-rw-   0 root         (0) root         (0)   224270 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po
--rw-rw-rw-   0 root         (0) root         (0)   162061 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/locales/pyams_content.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/
--rw-rw-rw-   0 root         (0) root         (0)     4561 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/
--rw-rw-rw-   0 root         (0) root         (0)     1996 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2917 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     6747 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     3851 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/templates/pictogram-header.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)     2896 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2831 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/templates/selection-layout.pt
--rw-rw-rw-   0 root         (0) root         (0)     3174 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4440 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/reference/zmi/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/reference/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     1974 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/reference/zmi/viewlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/root/
--rw-rw-rw-   0 root         (0) root         (0)     4904 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6721 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4841 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/root/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3885 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/root/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25806 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    13639 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     5338 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/root/zmi/sites.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/
--rw-rw-rw-   0 root         (0) root         (0)      561 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/
--rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5270 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2824 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4288 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     3268 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     9134 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/blog/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/blog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/calendar/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/calendar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/
--rw-rw-rw-   0 root         (0) root         (0)    11763 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)    15461 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5998 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/interfaces/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2282 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/header.py
--rw-rw-rw-   0 root         (0) root         (0)     5197 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1762 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2618 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/templates/specificities-default.pt
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/templates/title-default.pt
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/title.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/specificities.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/title.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      658 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1386 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1435 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      644 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/templates/specificities-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/templates/title-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     1369 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/title.py
--rw-rw-rw-   0 root         (0) root         (0)     9807 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)     3877 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/shared/common/security.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2333 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/breadcrumb.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/oid.py
--rw-rw-rw-   0 root         (0) root         (0)     1765 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/specificities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/templates/breadcrumbs.pt
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/templates/card-datatype.pt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/templates/publication-date.pt
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/title.py
--rw-rw-rw-   0 root         (0) root         (0)     2556 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/types.py
--rw-rw-rw-   0 root         (0) root         (0)     4801 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/url.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/skin/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    12425 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/
--rw-rw-rw-   0 root         (0) root         (0)    23132 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14620 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/content.py
--rw-rw-rw-   0 root         (0) root         (0)    36824 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3872 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/header.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4679 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    18561 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/owner.py
--rw-rw-rw-   0 root         (0) root         (0)     3030 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/portal.py
--rw-rw-rw-   0 root         (0) root         (0)     2899 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/reference.py
--rw-rw-rw-   0 root         (0) root         (0)    18640 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/restrictions.py
--rw-rw-rw-   0 root         (0) root         (0)    17565 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     8992 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/content-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/content-workflow.pt
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/owner-change.pt
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/quick-search.pt
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/sequence-header.pt
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/
--rw-rw-rw-   0 root         (0) root         (0)     7226 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5005 2024-04-28 15:24:34.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/container.py
--rw-rw-rw-   0 root         (0) root         (0)     2605 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/content.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     3179 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29957 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/common/zmi/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/file/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/file/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/form/
--rw-rw-rw-   0 root         (0) root         (0)     2560 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/form/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/form/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/form/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/form/skin/
--rw-rw-rw-   0 root         (0) root         (0)     2046 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/form/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/form/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/form/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/hub/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/hub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/logo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/shared/logo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/logo/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1149 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/logo/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/news/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/shared/news/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-28 15:30:31.000000 pyams_content-1.99.2/src/pyams_content/shared/resource/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/site/
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4564 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/container.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     8784 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     7205 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/link.py
--rw-rw-rw-   0 root         (0) root         (0)     5429 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2845 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/topic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8526 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/folder.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)    15922 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/link.py
--rw-rw-rw-   0 root         (0) root         (0)     8144 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5391 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/rename.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/search.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/topic.py
--rw-rw-rw-   0 root         (0) root         (0)    21405 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)     1899 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/viewlet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/topic/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/
--rw-rw-rw-   0 root         (0) root         (0)     8677 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     7663 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/query.py
--rw-rw-rw-   0 root         (0) root         (0)     5853 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     6223 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/merge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/
--rw-rw-rw-   0 root         (0) root         (0)     4700 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5886 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/
--rw-rw-rw-   0 root         (0) root         (0)     6787 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt
--rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt
--rw-rw-rw-   0 root         (0) root         (0)     2449 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt
--rw-rw-rw-   0 root         (0) root         (0)     2666 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/zmi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     1287 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     6586 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/query.py
--rw-rw-rw-   0 root         (0) root         (0)     6661 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/reference.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/skin/
--rw-rw-rw-   0 root         (0) root         (0)     1398 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/skin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/skin/templates/
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/skin/templates/preview.pt
--rw-rw-rw-   0 root         (0) root         (0)     7845 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/shared/view/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     4191 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/shared/view/zmi/references.py
--rw-rw-rw-   0 root         (0) root         (0)     6188 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/shared/view/zmi/thesaurus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/skin/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/skin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2024-04-09 20:44:10.000000 pyams_content-1.99.2/src/pyams_content/skin/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/tests/
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1829 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/tests/test_utilsdocstrings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/workflow/
--rw-rw-rw-   0 root         (0) root         (0)    43555 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21211 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/basic.py
--rw-rw-rw-   0 root         (0) root         (0)     1227 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4984 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/notify.py
--rw-rw-rw-   0 root         (0) root         (0)     6272 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3222 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/publication.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/workflow/zmi/templates/publication-header.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      777 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7680 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)     2383 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/html.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/properties.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/
--rw-rw-rw-   0 root         (0) root         (0)    19424 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/content.js
--rw-rw-rw-   0 root         (0) root         (0)    10283 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/content.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/headers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/headers/langs/
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/headers/langs/fr.js
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js
--rw-rw-rw-   0 root         (0) root         (0)     5919 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/viewlet/toplinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/seo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1260 2024-02-26 23:15:27.000000 pyams_content-1.99.2/src/pyams_content/zmi/widget/templates/seo-textline-input.pt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2488 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24617 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 15:31:04.000000 pyams_content-1.99.2/src/pyams_content.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-28 15:31:16.000000 pyams_content-1.99.2/src/pyams_content.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-05 21:02:51.000000 pyams_content-1.99.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-05-05 21:02:51.000000 pyams_content-1.99.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2753 2024-05-05 21:03:27.000000 pyams_content-1.99.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      920 2024-05-05 21:02:51.000000 pyams_content-1.99.3/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-05 21:02:51.000000 pyams_content-1.99.3/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 21:03:27.000000 pyams_content-1.99.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3377 2024-05-05 21:02:51.000000 pyams_content-1.99.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/association/
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4072 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3230 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1514 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/templates/association-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1960 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/skin/templates/association-viewlet.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/association/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5882 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9011 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2039 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/association/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/cards/
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/templates/cards-masonry.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/skin/templates/cards.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/cards/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/cards/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/contact/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/contact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/
+-rw-rw-rw-   0 root         (0) root         (0)     7387 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     9775 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3254 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2798 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3504 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5218 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/mail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/handler/zmi/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1814 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/templates/form-submit.pt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/skin/templates/paragraph-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/fields/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/fields/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/file/
+-rw-rw-rw-   0 root         (0) root         (0)     1583 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/frame/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/frame/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/frame/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4672 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     5095 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1661 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2175 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/zmi/templates/gallery-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     4053 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2891 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-random.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8399 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11985 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/file.py
+-rw-rw-rw-   0 root         (0) root         (0)     1995 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/
+-rw-rw-rw-   0 root         (0) root         (0)     7780 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6710 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1390 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/zmi/templates/illustration-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6234 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/illustration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/illustration-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/illustration-side.pt
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     5108 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5143 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/paragraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/keynumber/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/keynumber/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/links/
+-rw-rw-rw-   0 root         (0) root         (0)    10891 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4819 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     5037 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/links/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8653 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2658 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/links/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/map/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/map/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/milestone/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/milestone/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/
+-rw-rw-rw-   0 root         (0) root         (0)     6756 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5966 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     5173 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/interfaces/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     7591 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/templates/navigation-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7323 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/interfaces/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/templates/html.pt
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/templates/raw-code.pt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/templates/raw.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    17744 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17950 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4263 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/templates/title-toolbar.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/pictogram/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/pictogram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/
+-rw-rw-rw-   0 root         (0) root         (0)     7603 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/skin/templates/tags.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    12144 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     6509 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/verbatim/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/verbatim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/
+-rw-rw-rw-   0 root         (0) root         (0)     2307 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3286 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/dailymotion.py
+-rw-rw-rw-   0 root         (0) root         (0)     9322 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2895 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/vimeo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/provider/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2159 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/dailymotion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/custom-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/dailymotion-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      542 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/youtube-render.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/vimeo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/youtube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/skin/templates/video-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/component/video/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12014 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/component/video/zmi/paragraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/doctests/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/
+-rw-rw-rw-   0 root         (0) root         (0)     3608 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2142 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1882 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/skin/templates/alerts.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/skin/templates/context-alerts.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/alert/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/audit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6737 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1803 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/sitemap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/glossary-sitemap.pt
+-rw-rw-rw-   0 root         (0) root         (0)      929 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/glossary.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-associations.pt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-body.pt
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-footer.pt
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      767 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3568 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     3180 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/glossary/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/history/
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/history/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/history/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/history/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/history/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/history/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/history/zmi/templates/history.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/history/zmi/viewlet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/html/
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/html/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/
+-rw-rw-rw-   0 root         (0) root         (0)     6800 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     3392 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     3551 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7344 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/
+-rw-rw-rw-   0 root         (0) root         (0)      570 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2670 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/qrcode/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/qrcode/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/redirect/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/redirect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     5451 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/renderer/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/review/
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3253 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/chat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    11045 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/comment.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2784 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/comments.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/mail-notification.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/
+-rw-rw-rw-   0 root         (0) root         (0)     3169 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7419 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3804 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4861 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2527 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)    11035 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6230 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5146 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5176 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4985 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt
+-rw-rw-rw-   0 root         (0) root         (0)     5184 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4002 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/zmi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/search/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     7625 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/zmi/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/search/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/share/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/share/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/templates/humans.pt
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/templates/robots.pt
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/templates/root-sitemap.pt
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/sitemap/templates/tool-sitemap.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/feature/toolbox/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/feature/toolbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/generations/
+-rw-rw-rw-   0 root         (0) root         (0)    10545 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9656 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/include.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)   125110 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo
+-rw-rw-rw-   0 root         (0) root         (0)   225312 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po
+-rw-rw-rw-   0 root         (0) root         (0)   162899 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/locales/pyams_content.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     4561 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2917 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     6747 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     3851 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/templates/pictogram-header.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2831 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/templates/selection-layout.pt
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4440 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/zmi/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/reference/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1974 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/reference/zmi/viewlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/root/
+-rw-rw-rw-   0 root         (0) root         (0)     4904 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6721 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4841 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/root/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3885 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25806 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13639 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     5338 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/root/zmi/sites.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5270 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     3268 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     9134 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/blog/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/blog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/calendar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/
+-rw-rw-rw-   0 root         (0) root         (0)    11763 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)    15461 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5998 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/interfaces/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     5197 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1762 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/templates/specificities-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/templates/title-default.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/specificities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/title.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1386 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1435 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/templates/specificities-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/templates/title-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     9807 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3877 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/security.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2333 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/breadcrumb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/oid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/specificities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/templates/breadcrumbs.pt
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/templates/card-datatype.pt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/templates/publication-date.pt
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/title.py
+-rw-rw-rw-   0 root         (0) root         (0)     2556 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     4801 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/skin/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    12425 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)    23132 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14934 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/content.py
+-rw-rw-rw-   0 root         (0) root         (0)    36824 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3872 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    18561 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/owner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/portal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2899 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    18640 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/restrictions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17565 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     8992 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      537 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/content-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/content-workflow.pt
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/owner-change.pt
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/quick-search.pt
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/sequence-header.pt
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/
+-rw-rw-rw-   0 root         (0) root         (0)     7226 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5005 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/content.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     3179 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29957 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/common/zmi/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/file/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/form/
+-rw-rw-rw-   0 root         (0) root         (0)     2560 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/form/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/form/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/form/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/form/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/form/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/form/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/form/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/hub/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/hub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/logo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/logo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/logo/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/logo/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/news/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/news/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/resource/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/site/
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     5188 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     8784 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     7205 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     5429 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/topic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8526 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    15922 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     8144 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5391 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/rename.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/topic.py
+-rw-rw-rw-   0 root         (0) root         (0)    21405 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/viewlet/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/topic/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/
+-rw-rw-rw-   0 root         (0) root         (0)     8677 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     7663 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     5853 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     6223 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/merge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/
+-rw-rw-rw-   0 root         (0) root         (0)     4700 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5886 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     6787 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/zmi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     6586 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     6661 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/reference.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/skin/
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/skin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/skin/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/skin/templates/preview.pt
+-rw-rw-rw-   0 root         (0) root         (0)     7845 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/shared/view/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     4191 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/zmi/references.py
+-rw-rw-rw-   0 root         (0) root         (0)     6188 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/shared/view/zmi/thesaurus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/skin/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/skin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/skin/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/tests/test_utilsdocstrings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/workflow/
+-rw-rw-rw-   0 root         (0) root         (0)    48067 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21211 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/basic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4984 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/notify.py
+-rw-rw-rw-   0 root         (0) root         (0)     6360 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3222 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/publication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/workflow/zmi/templates/publication-header.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      777 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7680 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2383 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/properties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/
+-rw-rw-rw-   0 root         (0) root         (0)    19424 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/content.js
+-rw-rw-rw-   0 root         (0) root         (0)    10283 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/content.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/headers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/headers/langs/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/headers/langs/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/viewlet/toplinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/seo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2024-05-05 21:02:51.000000 pyams_content-1.99.3/src/pyams_content/zmi/widget/templates/seo-textline-input.pt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2753 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24617 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 21:03:18.000000 pyams_content-1.99.3/src/pyams_content.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-05 21:03:27.000000 pyams_content-1.99.3/src/pyams_content.egg-info/top_level.txt
```

### Comparing `pyams_content-1.99.2/LICENSE` & `pyams_content-1.99.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/PKG-INFO` & `pyams_content-1.99.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_content
-Version: 1.99.2
+Version: 1.99.3
 Summary: PyAMS content management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS CMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -48,14 +48,21 @@
 Please note that PyAMS_content only provide a basic Bootstrap based skin, so you will have to
 include other extension packages (like PyAMS_content_themes) to get more advanced graphical themes.
 
 
 Changelog
 =========
 
+1.99.3
+------
+ - updated shared content header viewlet to add button to go back to dashboard
+ - added status to scheduler tasks execution result
+ - added support for direct content retiring or archiving for managers
+ - added support for custom modal content class
+
 1.99.2
 ------
  - added permission and role to manage references tables
  - disable cache when using aggregated search results portlet renderer
  - always open switcher in associations paragraph
  - added method to paragraphs container to get iterator over paragraphs matching a given set of factories
  - removed required flag on gallery files author
```

### Comparing `pyams_content-1.99.2/docs/README.rst` & `pyams_content-1.99.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/setup.py` & `pyams_content-1.99.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '1.99.2'
+version = '1.99.3'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_security_views',
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
```

### Comparing `pyams_content-1.99.2/src/pyams_content/__init__.py` & `pyams_content-1.99.3/src/pyams_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/association/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/container.py` & `pyams_content-1.99.3/src/pyams_content/component/association/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/association/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/association/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/association/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/skin/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/association/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/skin/templates/association-viewlet.pt` & `pyams_content-1.99.3/src/pyams_content/component/association/skin/templates/association-viewlet.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/association/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/zmi/container.py` & `pyams_content-1.99.3/src/pyams_content/component/association/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/association/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/association/zmi/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/association/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/calendar/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/cards/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/cards/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/cards/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/cards/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/cards/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/cards/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/cards/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/cards/skin/templates/cards-masonry.pt` & `pyams_content-1.99.3/src/pyams_content/component/cards/skin/templates/cards-masonry.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/cards/skin/templates/cards.pt` & `pyams_content-1.99.3/src/pyams_content/component/cards/skin/templates/cards.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/cards/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/cards/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/extfile/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/extfile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/extfile/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/extfile/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/extfile/manager.py` & `pyams_content-1.99.3/src/pyams_content/component/extfile/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/manager.py` & `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt` & `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/templates/extfile-title-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt` & `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/templates/extfile-title-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/extfile/zmi/widget.py` & `pyams_content-1.99.3/src/pyams_content/component/extfile/zmi/widget.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/handler/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/handler/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/handler/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/handler/mail.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/handler/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/handler/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/handler/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/handler/zmi/mail.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/handler/zmi/mail.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/skin/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/fields/zmi/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/fields/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/file/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/file/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/frame/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/frame/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/file.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/file.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt` & `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-carousel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt` & `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt` & `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/skin/templates/gallery-random.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/portlet/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt` & `pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-carousel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-default.pt` & `pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/skin/templates/gallery-random.pt` & `pyams_content-1.99.3/src/pyams_content/component/gallery/skin/templates/gallery-random.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/file.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,14 +183,16 @@
     @property
     def hint(self):
         """Hint getter"""
         if self.can_edit:
             return _("Show/hide media")
         return None
 
+    css_class = 'btn-sm px-1'
+
     @property
     def icon_class(self):
         """Icon class getter"""
         if IGalleryFile(self.context).visible:
             icon_class = 'far fa-fw fa-eye'
         else:
             icon_class = 'far fa-fw fa-eye-slash text-danger'
@@ -236,14 +238,15 @@
                 context=IGalleryFile, layer=IAdminLayer, view=Interface,
                 manager=IContextActionsViewletManager, weight=20,
                 permission=VIEW_SYSTEM_PERMISSION)
 class GalleryFilePropertiesAction(ContextAction):
     """Gallery file properties action"""
 
     hint = _("Media properties")
+    css_class = 'btn-sm px-1'
     icon_class = 'far fa-edit'
 
     href = 'properties.html'
     modal_target = True
 
 
 @ajax_form_config(name='properties.html',
@@ -300,28 +303,29 @@
 
 #
 # Gallery file remover
 #
 
 @viewlet_config(name='delete-media.action',
                 context=IGalleryFile, layer=IAdminLayer, view=Interface,
-                manager=IContextActionsViewletManager, weight=30,
+                manager=IContextActionsViewletManager, weight=99,
                 permission=VIEW_SYSTEM_PERMISSION)
 class GalleryFileDeleteAction(ContextAction):
     """Gallery file delete action"""
 
     def __new__(cls, context, request, view, manager):
         gallery = get_parent(context, IGalleryContainer)
         if gallery is not None:
             edit_permission = get_edit_permission(request, context=gallery, view=view)
             if not request.has_permission(edit_permission, context=context):
                 return None
         return ContextAction.__new__(cls)
 
     hint = _("Delete media")
+    css_class = 'btn-sm px-1'
     icon_class = 'fas fa-trash'
 
     def get_href(self):
         """Icon URL getter"""
         return None
 
     click_handler = 'MyAMS.content.galleries.removeMedia'
```

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/helpers.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/helpers.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt` & `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-medias.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt` & `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-thumbnail.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt` & `pyams_content-1.99.3/src/pyams_content/component/gallery/zmi/templates/gallery-view.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt` & `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/templates/illustration-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt` & `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/skin/templates/illustration-side.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/portlet/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/illustration.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/illustration.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/illustration-default.pt` & `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/illustration-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/illustration-side.pt` & `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/illustration-side.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt` & `pyams_content-1.99.3/src/pyams_content/component/illustration/skin/templates/paragraph-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/thesaurus.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/illustration/zmi/thesaurus.py` & `pyams_content-1.99.3/src/pyams_content/component/illustration/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/keynumber/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/keynumber/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/links/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/links/html.py` & `pyams_content-1.99.3/src/pyams_content/component/links/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/links/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/links/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/links/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/links/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/links/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/links/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/links/zmi/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/links/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/map/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/map/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/milestone/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/milestone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/container.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/html.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/interfaces/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/interfaces/html.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/interfaces/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/templates/container-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/skin/templates/navigation-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/portlet/zmi/templates/container-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/settings.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/html.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/interfaces/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/interfaces/html.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/interfaces/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/skin/templates/html.pt` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/skin/templates/html.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/container.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,14 +389,15 @@
                 context=IParagraphContainerTarget, layer=IPyAMSLayer,
                 permission=VIEW_SYSTEM_PERMISSION)
 class ParagraphsContainerModalView(AdminModalDisplayForm):
     """Paragraphs container modal view"""
 
     subtitle = _("Paragraphs")
     modal_class = 'modal-xl'
+    modal_content_class = 'min-height-50vh'
 
 
 @adapter_config(required=(IParagraphContainerTarget, IAdminLayer, ParagraphsContainerModalView),
                 provides=IFormTitle)
 def paragraph_container_modal_view_title(context, request, view):
     """Paragraph container modal view title"""
     hint = get_object_hint(context, request, view)
```

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/helper.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/helper.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/html.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/paragraph/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/paragraph/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/thesaurus/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/thesaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/thesaurus/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/thesaurus/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/thesaurus/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/thesaurus/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/thesaurus/zmi/manager.py` & `pyams_content-1.99.3/src/pyams_content/component/thesaurus/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/video/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/video/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/video/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/provider/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/video/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/provider/dailymotion.py` & `pyams_content-1.99.3/src/pyams_content/component/video/provider/dailymotion.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/provider/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/video/provider/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/provider/vimeo.py` & `pyams_content-1.99.3/src/pyams_content/component/video/provider/vimeo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/provider/youtube.py` & `pyams_content-1.99.3/src/pyams_content/component/video/provider/youtube.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/video/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/component/video/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/dailymotion.py` & `pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/dailymotion.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt` & `pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/templates/vimeo-render.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/vimeo.py` & `pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/vimeo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/skin/provider/youtube.py` & `pyams_content-1.99.3/src/pyams_content/component/video/skin/provider/youtube.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/skin/templates/video-default.pt` & `pyams_content-1.99.3/src/pyams_content/component/video/skin/templates/video-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/component/video/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/component/video/zmi/paragraph.py` & `pyams_content-1.99.3/src/pyams_content/component/video/zmi/paragraph.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/doctests/README.rst` & `pyams_content-1.99.3/src/pyams_content/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/alert/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/alert/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/alert/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/alert/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/alert/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/alert/skin/templates/alerts.pt` & `pyams_content-1.99.3/src/pyams_content/feature/alert/skin/templates/alerts.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/alert/skin/templates/context-alerts.pt` & `pyams_content-1.99.3/src/pyams_content/feature/alert/skin/templates/context-alerts.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/alert/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/alert/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/sitemap.py` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/sitemap.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/glossary-term.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/glossary.pt` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/glossary.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-associations.pt` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-associations.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/templates/term-illustration.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/skin/term.py` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/skin/term.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/task.py` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/glossary/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/glossary/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/history/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/history/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/history/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/history/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/history/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/history/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/history/zmi/viewlet.py` & `pyams_content-1.99.3/src/pyams_content/feature/history/zmi/viewlet.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/html/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/html/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/templates/double-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/skin/templates/simple-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/templates/double-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/portlet/zmi/templates/simple-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/container.py` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/navigation/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/navigation/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/preview/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/preview/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/preview/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt` & `pyams_content-1.99.3/src/pyams_content/feature/preview/zmi/templates/modal-preview.pt`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div class="modal-dialog ${view.modal_class | ''}">
-	<div class="modal-content">
+	<div class="modal-content ${view.modal_content_class | ''}">
 		<div class="modal-header">
 			<div tal:define="header provider:pyams.header"
 				 tal:condition="header">
 				<i tal:omit-tag="">${structure:provider:pyams.header}</i>
 			</div>
 			<button type="button" class="close"
 					data-dismiss="modal" aria-label="Close">
```

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/renderer/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/renderer/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/renderer/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/review/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/review/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/review/chat.py` & `pyams_content-1.99.3/src/pyams_content/feature/review/chat.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/review/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/review/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/review/manager.py` & `pyams_content-1.99.3/src/pyams_content/feature/review/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/review/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/review/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/comment.pt` & `pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/comment.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/comments.pt` & `pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/comments.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/review/zmi/templates/mail-notification.pt` & `pyams_content-1.99.3/src/pyams_content/feature/review/zmi/templates/mail-notification.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/manager.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-card.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-cards-masonry.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-cards.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-panel.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-panels.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/templates/search-result.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/skin/zmi.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/skin/zmi.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt` & `pyams_content-1.99.3/src/pyams_content/feature/search/portlet/zmi/templates/search-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/thesaurus.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/zmi/manager.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/zmi/reference.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/zmi/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/search/zmi/thesaurus.py` & `pyams_content-1.99.3/src/pyams_content/feature/search/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/sitemap/__init__.py` & `pyams_content-1.99.3/src/pyams_content/feature/sitemap/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/feature/sitemap/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/feature/sitemap/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/generations/__init__.py` & `pyams_content-1.99.3/src/pyams_content/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/include.py` & `pyams_content-1.99.3/src/pyams_content/include.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/interfaces/__init__.py` & `pyams_content-1.99.3/src/pyams_content/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo` & `pyams_content-1.99.3/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -266,17 +266,14 @@
 
 msgid "Archive request"
 msgstr "Demande d'archivage"
 
 msgid "Archive request canceled"
 msgstr "Annulation de la demande d'archivage"
 
-msgid "Archive retired content"
-msgstr "Archivage automatique d'un contenu retiré"
-
 msgid "Archive retiring content"
 msgstr "Archivage automatique d'un contenu en attente de retrait"
 
 msgid "Archived"
 msgstr "Archivé"
 
 msgid "Archiving"
@@ -360,14 +357,17 @@
 
 msgid "Auto play?"
 msgstr "Lecture automatique"
 
 msgid "Available pictograms"
 msgstr "Pictogrammes disponibles"
 
+msgid "Back to dashboard"
+msgstr "Revenir au tableau de bord"
+
 msgid "Back to previous page"
 msgstr "Revenir à la page précédente"
 
 msgid "Back-office label"
 msgstr "Libellé back-office"
 
 msgid "Base URL of the public site"
@@ -569,15 +569,17 @@
 msgid "Click icon to enable or disable alert type"
 msgstr "Cliquer pour activer ou désactiver ce type d'alerte"
 
 msgid "Click icon to enable or disable content type"
 msgstr "Cliquer pour activer ou désactiver ce type de contenu"
 
 msgid "Click to lock/unlock paragraph"
-msgstr "Cliquer pour (dé)verrouiller ce bloc"
+msgstr ""
+"Cliquer pour (dé)verrouiller ce bloc ; un bloc verrouillé ne peut pas être "
+"supprimé par les contributeurs (mais il peut être masqué)"
 
 msgid "Click to open/close all folders"
 msgstr "Afficher/masquer toutes les rubriques"
 
 msgid "Click to set/unset paragraph as navigation anchor"
 msgstr "Cliquer pour (dés)activer l'ancre de navigation sur ce bloc"
 
@@ -2674,14 +2676,17 @@
 msgstr ""
 "Position à laquelle la vidéo doit s'arrêter, en secondes ou sous la forme "
 "'minutes:secondes'"
 
 msgid "Pre-publish content"
 msgstr "Pré-publier le contenu"
 
+msgid "Pre-publish retired content"
+msgstr "Pré-publier le contenu retiré"
+
 msgid "Presentation template used for associations"
 msgstr "Mode de rendu utilisé pour ce bloc"
 
 msgid "Presentation template used for cards"
 msgstr "Mode de rendu utilisé pour ce bloc de contenu"
 
 msgid "Presentation template used for form fields"
@@ -2787,14 +2792,17 @@
 
 msgid "Publish content"
 msgstr "Publier le contenu"
 
 msgid "Publish or retire existing content"
 msgstr "Publier ou retirer un contenu"
 
+msgid "Publish retired content"
+msgstr "Re-publier le contenu"
+
 msgid "Published"
 msgstr "Publié"
 
 msgid "Published (waiting)"
 msgstr "Publié (en attente)"
 
 msgid "Published version creation date"
```

### Comparing `pyams_content-1.99.2/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po` & `pyams_content-1.99.3/src/pyams_content/locales/fr/LC_MESSAGES/pyams_content.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2024-04-24 23:44+0200\n"
+"POT-Creation-Date: 2024-05-05 16:18+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -98,15 +98,15 @@
 #: src/pyams_content/zmi/dashboard.py:85
 msgid "Visible element?"
 msgstr ""
 "Un élément peut ne pas être visible s'il n'a pas encore été publié ou si son "
 "niveau parent n'est pas publié"
 
 #: src/pyams_content/zmi/dashboard.py:112
-#: src/pyams_content/reference/zmi/table.py:98
+#: src/pyams_content/reference/zmi/table.py:99
 #: src/pyams_content/feature/navigation/portlet/interfaces.py:33
 #: src/pyams_content/feature/navigation/portlet/interfaces.py:47
 #: src/pyams_content/feature/search/portlet/interfaces.py:44
 #: src/pyams_content/interfaces/__init__.py:122
 #: src/pyams_content/component/paragraph/zmi/container.py:236
 #: src/pyams_content/component/paragraph/portlet/interfaces.py:33
 #: src/pyams_content/component/gallery/interfaces.py:118
@@ -170,32 +170,28 @@
 msgid "Table managers"
 msgstr "Gestionnaires"
 
 #: src/pyams_content/reference/interfaces.py:49
 msgid "Table managers can handle all table contents"
 msgstr "Liste des gestionnaires autorisés à gérer le contenu de cette table"
 
-#: src/pyams_content/reference/zmi/table.py:50
+#: src/pyams_content/reference/zmi/table.py:51
 #: src/pyams_content/shared/site/zmi/manager.py:167
 #: src/pyams_content/shared/site/zmi/folder.py:180
 #: src/pyams_content/shared/common/zmi/manager.py:82
 #: src/pyams_content/shared/common/zmi/__init__.py:305
 #: src/pyams_content/root/zmi/__init__.py:63
 msgid "Properties"
 msgstr "Propriétés"
 
-#: src/pyams_content/reference/zmi/table.py:61
-msgid "Pictograms table"
-msgstr "Table des pictogrammes"
-
-#: src/pyams_content/reference/zmi/table.py:62
+#: src/pyams_content/reference/zmi/table.py:63
 msgid "Edit table properties"
 msgstr "Propriétés de la table"
 
-#: src/pyams_content/reference/zmi/table.py:72
+#: src/pyams_content/reference/zmi/table.py:73
 msgid "Table management"
 msgstr "Gérer cette table"
 
 #: src/pyams_content/reference/zmi/__init__.py:33
 #: src/pyams_content/shared/view/zmi/references.py:50
 msgid "References"
 msgstr "Références"
@@ -246,28 +242,32 @@
 msgstr "Pictogrammes sélectionnés"
 
 #: src/pyams_content/reference/pictogram/interfaces.py:74
 msgid "List of selected pictograms which will be available to shared contents"
 msgstr ""
 "Liste des pictogrammes qui seront rendus disponibles aux contenus partagés"
 
-#: src/pyams_content/reference/pictogram/zmi/table.py:41
-#: src/pyams_content/reference/pictogram/zmi/table.py:101
+#: src/pyams_content/reference/pictogram/zmi/table.py:42
+#: src/pyams_content/reference/pictogram/zmi/table.py:102
 #: src/pyams_content/shared/common/zmi/types/__init__.py:187
 msgid "Pictograms"
 msgstr "Pictogrammes"
 
-#: src/pyams_content/reference/pictogram/zmi/table.py:59
+#: src/pyams_content/reference/pictogram/zmi/table.py:60
 msgid "Table contents"
 msgstr "Contenu"
 
-#: src/pyams_content/reference/pictogram/zmi/table.py:103
+#: src/pyams_content/reference/pictogram/zmi/table.py:105
 msgid "Pictograms list"
 msgstr "Liste des pictogrammes"
 
+#: src/pyams_content/reference/pictogram/zmi/table.py:113
+msgid "Pictograms table"
+msgstr "Table des pictogrammes"
+
 #: src/pyams_content/reference/pictogram/zmi/manager.py:49
 msgid "Pictograms selection"
 msgstr "Sélection des pictogrammes"
 
 #: src/pyams_content/reference/pictogram/zmi/manager.py:59
 msgid "Pictograms management"
 msgstr "Gestion des pictogrammes"
@@ -338,467 +338,484 @@
 
 #: src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt:26
 #: src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt:61
 msgid "Switch pictogram selection"
 msgstr "(Dé)sélectionner le pictogramme"
 
 #: src/pyams_content/workflow/basic.py:69
-#: src/pyams_content/workflow/__init__.py:83
+#: src/pyams_content/workflow/__init__.py:84
 msgid "Draft"
 msgstr "Brouillon"
 
 #: src/pyams_content/workflow/basic.py:70
-#: src/pyams_content/workflow/__init__.py:87
+#: src/pyams_content/workflow/__init__.py:88
 msgid "Published (waiting)"
 msgstr "Publié (en attente)"
 
 #: src/pyams_content/workflow/basic.py:71
-#: src/pyams_content/workflow/__init__.py:88
+#: src/pyams_content/workflow/__init__.py:89
 #: src/pyams_content/shared/common/zmi/header.py:66
 #: src/pyams_content/shared/common/zmi/header.py:69
 #: src/pyams_content/shared/common/zmi/header.py:76
 msgid "Published"
 msgstr "Publié"
 
 #: src/pyams_content/workflow/basic.py:72
-#: src/pyams_content/workflow/__init__.py:92
+#: src/pyams_content/workflow/__init__.py:93
 msgid "Archived"
 msgstr "Archivé"
 
 #: src/pyams_content/workflow/basic.py:73
-#: src/pyams_content/workflow/__init__.py:93
+#: src/pyams_content/workflow/__init__.py:94
 msgid "Deleted"
 msgstr "Supprimé"
 
 #: src/pyams_content/workflow/basic.py:82
-#: src/pyams_content/workflow/__init__.py:102
+#: src/pyams_content/workflow/__init__.py:103
 msgid "draft created"
 msgstr "brouillon créé"
 
 #: src/pyams_content/workflow/basic.py:83
-#: src/pyams_content/workflow/__init__.py:104
+#: src/pyams_content/workflow/__init__.py:105
 msgid "published (waiting)"
 msgstr "publié (en attente)"
 
 #: src/pyams_content/workflow/basic.py:84
-#: src/pyams_content/workflow/__init__.py:105
+#: src/pyams_content/workflow/__init__.py:106
 msgid "published"
 msgstr "publié"
 
 #: src/pyams_content/workflow/basic.py:85
-#: src/pyams_content/workflow/__init__.py:109
+#: src/pyams_content/workflow/__init__.py:110
 msgid "archived"
 msgstr "archivé"
 
 #: src/pyams_content/workflow/basic.py:249
-#: src/pyams_content/workflow/__init__.py:345
+#: src/pyams_content/workflow/__init__.py:353
 #, python-format
 msgid "Published version {0}"
 msgstr "Publication de la version {0}"
 
 #: src/pyams_content/workflow/basic.py:304
-#: src/pyams_content/workflow/__init__.py:405
+#: src/pyams_content/workflow/__init__.py:413
 msgid "Initialize"
 msgstr "Création"
 
 #: src/pyams_content/workflow/basic.py:307
-#: src/pyams_content/workflow/__init__.py:408
+#: src/pyams_content/workflow/__init__.py:416
 msgid "Draft creation"
 msgstr "Création du brouillon"
 
 #: src/pyams_content/workflow/basic.py:310
-#: src/pyams_content/workflow/__init__.py:429
-#: src/pyams_content/workflow/__init__.py:542
+#: src/pyams_content/workflow/__init__.py:437
+#: src/pyams_content/workflow/__init__.py:550
 msgid "Pre-publish content"
 msgstr "Pré-publier le contenu"
 
 #: src/pyams_content/workflow/basic.py:315
-#: src/pyams_content/workflow/__init__.py:434
-#: src/pyams_content/workflow/__init__.py:547
+#: src/pyams_content/workflow/__init__.py:442
+#: src/pyams_content/workflow/__init__.py:555
+#: src/pyams_content/workflow/__init__.py:686
 msgid "Content pre-published"
 msgstr "Contenu pré-publié"
 
 #: src/pyams_content/workflow/basic.py:317
 #: src/pyams_content/workflow/basic.py:332
 #: src/pyams_content/workflow/basic.py:357
-#: src/pyams_content/workflow/__init__.py:436
-#: src/pyams_content/workflow/__init__.py:453
-#: src/pyams_content/workflow/__init__.py:549
-#: src/pyams_content/workflow/__init__.py:573
-#: src/pyams_content/workflow/__init__.py:591
+#: src/pyams_content/workflow/__init__.py:444
+#: src/pyams_content/workflow/__init__.py:461
+#: src/pyams_content/workflow/__init__.py:557
+#: src/pyams_content/workflow/__init__.py:581
+#: src/pyams_content/workflow/__init__.py:599
+#: src/pyams_content/workflow/__init__.py:688
+#: src/pyams_content/workflow/__init__.py:705
 msgid "Content publication"
 msgstr "Publication de contenu"
 
 #: src/pyams_content/workflow/basic.py:318
-#: src/pyams_content/workflow/__init__.py:437
-#: src/pyams_content/workflow/__init__.py:550
+#: src/pyams_content/workflow/__init__.py:445
+#: src/pyams_content/workflow/__init__.py:558
+#: src/pyams_content/workflow/__init__.py:689
 #, python-format
 msgid "{principal} pre-published the content « {title} »"
 msgstr "{principal} a pré-publié le contenu « {title} »"
 
 #: src/pyams_content/workflow/basic.py:322
-#: src/pyams_content/workflow/__init__.py:562
+#: src/pyams_content/workflow/__init__.py:570
 msgid "Cancel publication"
 msgstr "Annuler la publication"
 
 #: src/pyams_content/workflow/basic.py:330
-#: src/pyams_content/workflow/__init__.py:570
+#: src/pyams_content/workflow/__init__.py:578
 msgid "Publication canceled"
 msgstr "Publication annulée"
 
 #: src/pyams_content/workflow/basic.py:333
-#: src/pyams_content/workflow/__init__.py:574
+#: src/pyams_content/workflow/__init__.py:582
 #, python-format
 msgid "{principal} cancelled the publication for content « {title} »"
 msgstr "{principal} a annulé la publication du contenu « {title} »"
 
 #: src/pyams_content/workflow/basic.py:338
 #: src/pyams_content/workflow/basic.py:346
-#: src/pyams_content/workflow/__init__.py:441
-#: src/pyams_content/workflow/__init__.py:554
-#: src/pyams_content/workflow/__init__.py:579
+#: src/pyams_content/workflow/__init__.py:449
+#: src/pyams_content/workflow/__init__.py:562
+#: src/pyams_content/workflow/__init__.py:587
 msgid "Publish content"
 msgstr "Publier le contenu"
 
 #: src/pyams_content/workflow/basic.py:343
 #: src/pyams_content/workflow/basic.py:355
-#: src/pyams_content/workflow/__init__.py:451
-#: src/pyams_content/workflow/__init__.py:559
-#: src/pyams_content/workflow/__init__.py:589
+#: src/pyams_content/workflow/__init__.py:459
+#: src/pyams_content/workflow/__init__.py:567
+#: src/pyams_content/workflow/__init__.py:597
+#: src/pyams_content/workflow/__init__.py:703
 msgid "Content published"
 msgstr "Publication"
 
 #: src/pyams_content/workflow/basic.py:358
-#: src/pyams_content/workflow/__init__.py:454
-#: src/pyams_content/workflow/__init__.py:592
+#: src/pyams_content/workflow/__init__.py:462
+#: src/pyams_content/workflow/__init__.py:600
+#: src/pyams_content/workflow/__init__.py:706
 #, python-format
 msgid "{principal} published the content « {title} »"
 msgstr "{principal} a publié le contenu « {title} »"
 
 #: src/pyams_content/workflow/basic.py:363
-#: src/pyams_content/workflow/__init__.py:689
+#: src/pyams_content/workflow/__init__.py:729
+#: src/pyams_content/workflow/__init__.py:762
 msgid "Archive content"
 msgstr "Archiver le contenu"
 
 #: src/pyams_content/workflow/basic.py:372
-#: src/pyams_content/workflow/__init__.py:698
+#: src/pyams_content/workflow/__init__.py:738
+#: src/pyams_content/workflow/__init__.py:771
 msgid "Content archived"
 msgstr "Archivage"
 
 #: src/pyams_content/workflow/basic.py:374
-#: src/pyams_content/workflow/__init__.py:702
+#: src/pyams_content/workflow/__init__.py:742
+#: src/pyams_content/workflow/__init__.py:775
 #, python-format
 msgid "{principal} archived content « {title} »"
 msgstr "{principal} a archivé le contenu « {title} »"
 
 #: src/pyams_content/workflow/basic.py:378
 #: src/pyams_content/workflow/basic.py:390
-#: src/pyams_content/workflow/__init__.py:730
-#: src/pyams_content/workflow/__init__.py:742
-#: src/pyams_content/workflow/__init__.py:754
-#: src/pyams_content/workflow/__init__.py:766
-#: src/pyams_content/workflow/__init__.py:778
+#: src/pyams_content/workflow/__init__.py:795
+#: src/pyams_content/workflow/__init__.py:808
+#: src/pyams_content/workflow/__init__.py:821
+#: src/pyams_content/workflow/__init__.py:834
+#: src/pyams_content/workflow/__init__.py:847
 msgid "Create new version"
 msgstr "Créer une nouvelle version"
 
 #: src/pyams_content/workflow/basic.py:386
 #: src/pyams_content/workflow/basic.py:398
-#: src/pyams_content/workflow/__init__.py:738
-#: src/pyams_content/workflow/__init__.py:750
-#: src/pyams_content/workflow/__init__.py:762
-#: src/pyams_content/workflow/__init__.py:774
-#: src/pyams_content/workflow/__init__.py:786
+#: src/pyams_content/workflow/__init__.py:804
+#: src/pyams_content/workflow/__init__.py:817
+#: src/pyams_content/workflow/__init__.py:830
+#: src/pyams_content/workflow/__init__.py:843
+#: src/pyams_content/workflow/__init__.py:856
 msgid "New version created"
 msgstr "Création d'une nouvelle version"
 
 #: src/pyams_content/workflow/basic.py:402
-#: src/pyams_content/workflow/__init__.py:790
+#: src/pyams_content/workflow/__init__.py:860
 msgid "Delete version"
 msgstr "Supprimer cette version"
 
 #: src/pyams_content/workflow/basic.py:410
-#: src/pyams_content/workflow/__init__.py:798
+#: src/pyams_content/workflow/__init__.py:869
 msgid "Version deleted"
 msgstr "Version supprimée"
 
 #: src/pyams_content/workflow/basic.py:428
 msgid "PyAMS basic workflow"
 msgstr "Workflow basique"
 
 #: src/pyams_content/workflow/basic.py:447
 #: src/pyams_content/workflow/basic.py:484
-#: src/pyams_content/workflow/__init__.py:859
-#: src/pyams_content/workflow/__init__.py:896
+#: src/pyams_content/workflow/__init__.py:933
+#: src/pyams_content/workflow/__init__.py:970
 #: src/pyams_content/shared/common/zmi/workflow.py:166
 #, python-format
 msgid "{state} {date}"
 msgstr "{state} {date}"
 
 #: src/pyams_content/workflow/basic.py:451
 #: src/pyams_content/workflow/basic.py:476
-#: src/pyams_content/workflow/__init__.py:863
-#: src/pyams_content/workflow/__init__.py:888
+#: src/pyams_content/workflow/__init__.py:937
+#: src/pyams_content/workflow/__init__.py:962
 msgid "Unknown state"
 msgstr "(statut inconnu)"
 
 #: src/pyams_content/workflow/basic.py:474
-#: src/pyams_content/workflow/__init__.py:886
+#: src/pyams_content/workflow/__init__.py:960
 msgid "new version created"
 msgstr "nouvelle version en préparation"
 
 #: src/pyams_content/workflow/basic.py:480
-#: src/pyams_content/workflow/__init__.py:892
+#: src/pyams_content/workflow/__init__.py:966
 msgid "publication request cancelled"
 msgstr "demande de publication annulée"
 
 #: src/pyams_content/workflow/basic.py:482
-#: src/pyams_content/workflow/__init__.py:894
+#: src/pyams_content/workflow/__init__.py:968
 msgid "publication refused"
 msgstr "publication refusée"
 
 #: src/pyams_content/workflow/task.py:52
 msgid "Content publisher task"
 msgstr "Publication d'un contenu"
 
-#: src/pyams_content/workflow/task.py:88
+#: src/pyams_content/workflow/task.py:89
 msgid "Content archiver task"
 msgstr "Archivage d'un contenu"
 
-#: src/pyams_content/workflow/__init__.py:84
+#: src/pyams_content/workflow/__init__.py:85
 msgid "Proposed"
 msgstr "Proposé à la publication"
 
-#: src/pyams_content/workflow/__init__.py:85
+#: src/pyams_content/workflow/__init__.py:86
 msgid "Canceled"
 msgstr "Annulé"
 
-#: src/pyams_content/workflow/__init__.py:86
+#: src/pyams_content/workflow/__init__.py:87
 msgid "Refused"
 msgstr "Refusé"
 
-#: src/pyams_content/workflow/__init__.py:89
+#: src/pyams_content/workflow/__init__.py:90
 msgid "Retiring"
 msgstr "Retrait demandé"
 
-#: src/pyams_content/workflow/__init__.py:90
+#: src/pyams_content/workflow/__init__.py:91
 #: src/pyams_content/shared/common/zmi/header.py:63
 msgid "Retired"
 msgstr "Retiré"
 
-#: src/pyams_content/workflow/__init__.py:91
+#: src/pyams_content/workflow/__init__.py:92
 msgid "Archiving"
 msgstr "Archivage demandé"
 
-#: src/pyams_content/workflow/__init__.py:103
+#: src/pyams_content/workflow/__init__.py:104
 msgid "publication requested"
 msgstr "publication demandée"
 
-#: src/pyams_content/workflow/__init__.py:106
+#: src/pyams_content/workflow/__init__.py:107
 msgid "retiring requested"
 msgstr "retrait demandé"
 
-#: src/pyams_content/workflow/__init__.py:107
+#: src/pyams_content/workflow/__init__.py:108
 msgid "retired"
 msgstr "retiré"
 
-#: src/pyams_content/workflow/__init__.py:108
+#: src/pyams_content/workflow/__init__.py:109
 msgid "archiving requested"
 msgstr "archivage demandé"
 
-#: src/pyams_content/workflow/__init__.py:411
-#: src/pyams_content/workflow/__init__.py:459
+#: src/pyams_content/workflow/__init__.py:419
+#: src/pyams_content/workflow/__init__.py:467
 msgid "Propose publication"
 msgstr "Demander la publication"
 
-#: src/pyams_content/workflow/__init__.py:418
-#: src/pyams_content/workflow/__init__.py:423
-#: src/pyams_content/workflow/__init__.py:466
-#: src/pyams_content/workflow/__init__.py:471
-#: src/pyams_content/workflow/__init__.py:488
-#: src/pyams_content/workflow/__init__.py:520
+#: src/pyams_content/workflow/__init__.py:426
+#: src/pyams_content/workflow/__init__.py:431
+#: src/pyams_content/workflow/__init__.py:474
+#: src/pyams_content/workflow/__init__.py:479
+#: src/pyams_content/workflow/__init__.py:496
+#: src/pyams_content/workflow/__init__.py:528
 msgid "Publication request"
 msgstr "Demande de publication"
 
-#: src/pyams_content/workflow/__init__.py:419
-#: src/pyams_content/workflow/__init__.py:467
-#: src/pyams_content/workflow/__init__.py:604
-#: src/pyams_content/workflow/__init__.py:662
+#: src/pyams_content/workflow/__init__.py:427
+#: src/pyams_content/workflow/__init__.py:475
+#: src/pyams_content/workflow/__init__.py:612
+#: src/pyams_content/workflow/__init__.py:718
 msgid ""
 "content managers authorized to take charge of your content are going to be "
 "notified of your request."
 msgstr ""
 "les responsables habilités à prendre en charge votre demande vont être "
 "sollicités."
 
-#: src/pyams_content/workflow/__init__.py:424
-#: src/pyams_content/workflow/__init__.py:472
+#: src/pyams_content/workflow/__init__.py:432
+#: src/pyams_content/workflow/__init__.py:480
 #, python-format
 msgid "{principal} submitted a publication request for content « {title} »"
 msgstr "{principal} a demandé la publication du contenu « {title} »"
 
-#: src/pyams_content/workflow/__init__.py:477
+#: src/pyams_content/workflow/__init__.py:485
 msgid "Cancel publication request"
 msgstr "Annuler la demande de publication"
 
-#: src/pyams_content/workflow/__init__.py:485
+#: src/pyams_content/workflow/__init__.py:493
 msgid "Publication request canceled"
 msgstr "Annulation de la demande de publication"
 
-#: src/pyams_content/workflow/__init__.py:489
+#: src/pyams_content/workflow/__init__.py:497
 #, python-format
 msgid "{principal} cancelled the publication request for content « {title} »"
 msgstr ""
 "{principal} a annulé la demande de publication pour le contenu « {title} »"
 
-#: src/pyams_content/workflow/__init__.py:494
+#: src/pyams_content/workflow/__init__.py:502
 msgid "Reset canceled publication to draft"
 msgstr "Retour automatique en statut 'brouillon'"
 
-#: src/pyams_content/workflow/__init__.py:498
-#: src/pyams_content/workflow/__init__.py:530
+#: src/pyams_content/workflow/__init__.py:506
+#: src/pyams_content/workflow/__init__.py:538
 msgid "State reset to 'draft' (automatic)"
 msgstr "Retour automatique en statut 'brouillon'"
 
-#: src/pyams_content/workflow/__init__.py:502
+#: src/pyams_content/workflow/__init__.py:510
 msgid "Reset canceled publication to retired"
 msgstr "Retour automatique en statut 'retiré'"
 
-#: src/pyams_content/workflow/__init__.py:506
+#: src/pyams_content/workflow/__init__.py:514
 msgid "State reset to 'retired' (automatic)"
 msgstr "Retour automatique en statut 'retiré'"
 
-#: src/pyams_content/workflow/__init__.py:510
+#: src/pyams_content/workflow/__init__.py:518
 msgid "Refuse publication"
 msgstr "Refuser la publication"
 
-#: src/pyams_content/workflow/__init__.py:518
+#: src/pyams_content/workflow/__init__.py:526
 msgid "Publication refused"
 msgstr "Refus de publication"
 
-#: src/pyams_content/workflow/__init__.py:521
+#: src/pyams_content/workflow/__init__.py:529
 #, python-format
 msgid "{principal} refused the publication request for content « {title} »"
 msgstr "{principal} a refusé la publication du contenu « {title} »"
 
-#: src/pyams_content/workflow/__init__.py:526
+#: src/pyams_content/workflow/__init__.py:534
 msgid "Reset refused publication to draft"
 msgstr "Publication refusée"
 
-#: src/pyams_content/workflow/__init__.py:534
+#: src/pyams_content/workflow/__init__.py:542
 msgid "Reset refused publication to retired"
 msgstr "Publication refusée"
 
-#: src/pyams_content/workflow/__init__.py:538
+#: src/pyams_content/workflow/__init__.py:546
 msgid "State reset to 'refused' (automatic)"
 msgstr "Retour automatique en statut 'refusé'"
 
-#: src/pyams_content/workflow/__init__.py:597
+#: src/pyams_content/workflow/__init__.py:605
 msgid "Request retiring"
 msgstr "Demander le retrait"
 
-#: src/pyams_content/workflow/__init__.py:603
+#: src/pyams_content/workflow/__init__.py:611
 msgid "Retire request"
 msgstr "Demande de retrait"
 
-#: src/pyams_content/workflow/__init__.py:609
-#: src/pyams_content/workflow/__init__.py:632
-#: src/pyams_content/workflow/__init__.py:650
+#: src/pyams_content/workflow/__init__.py:617
+#: src/pyams_content/workflow/__init__.py:635
+#: src/pyams_content/workflow/__init__.py:658
+#: src/pyams_content/workflow/__init__.py:676
 msgid "Content removal"
 msgstr "Retrait de contenu"
 
-#: src/pyams_content/workflow/__init__.py:610
+#: src/pyams_content/workflow/__init__.py:618
 #, python-format
 msgid "{principal} submitted a retire request for content « {title} »"
 msgstr "{principal} a demandé le retrait du contenu « {title} »"
 
-#: src/pyams_content/workflow/__init__.py:615
+#: src/pyams_content/workflow/__init__.py:623
+#: src/pyams_content/workflow/__init__.py:640
 msgid "Retired content"
 msgstr "Retirer le contenu"
 
-#: src/pyams_content/workflow/__init__.py:619
+#: src/pyams_content/workflow/__init__.py:632
+#: src/pyams_content/workflow/__init__.py:673
+msgid "Content retired"
+msgstr "Retrait"
+
+#: src/pyams_content/workflow/__init__.py:636
+#: src/pyams_content/workflow/__init__.py:677
+#, python-format
+msgid "{principal} retired content « {title} »"
+msgstr "{principal} a retiré le contenu « {title} »"
+
+#: src/pyams_content/workflow/__init__.py:645
 msgid "Content retired after passed expiration date"
 msgstr "Retrait automatique après la date de fin de publication"
 
-#: src/pyams_content/workflow/__init__.py:622
+#: src/pyams_content/workflow/__init__.py:648
 msgid "Cancel retiring request"
 msgstr "Annuler la demande de retrait"
 
-#: src/pyams_content/workflow/__init__.py:629
+#: src/pyams_content/workflow/__init__.py:655
 msgid "Retire request canceled"
 msgstr "Annulation de la demande de retrait"
 
-#: src/pyams_content/workflow/__init__.py:633
+#: src/pyams_content/workflow/__init__.py:659
 #, python-format
 msgid "{principal} cancelled the retiring request for content « {title} »"
 msgstr "{principal} a annulé la demande de retrait du contenu « {title} »"
 
-#: src/pyams_content/workflow/__init__.py:638
+#: src/pyams_content/workflow/__init__.py:664
 msgid "Retire content"
 msgstr "Retirer le contenu"
 
-#: src/pyams_content/workflow/__init__.py:647
-msgid "Content retired"
-msgstr "Retrait"
-
-#: src/pyams_content/workflow/__init__.py:651
-#, python-format
-msgid "{principal} retired content « {title} »"
-msgstr "{principal} a retiré le contenu « {title} »"
+#: src/pyams_content/workflow/__init__.py:681
+msgid "Pre-publish retired content"
+msgstr "Pré-publier le contenu retiré"
+
+#: src/pyams_content/workflow/__init__.py:693
+msgid "Publish retired content"
+msgstr "Re-publier le contenu"
 
-#: src/pyams_content/workflow/__init__.py:655
+#: src/pyams_content/workflow/__init__.py:711
 msgid "Request archive"
 msgstr "Demander l'archivage"
 
-#: src/pyams_content/workflow/__init__.py:661
+#: src/pyams_content/workflow/__init__.py:717
 msgid "Archive request"
 msgstr "Demande d'archivage"
 
-#: src/pyams_content/workflow/__init__.py:667
-#: src/pyams_content/workflow/__init__.py:683
-#: src/pyams_content/workflow/__init__.py:701
+#: src/pyams_content/workflow/__init__.py:723
+#: src/pyams_content/workflow/__init__.py:741
+#: src/pyams_content/workflow/__init__.py:756
+#: src/pyams_content/workflow/__init__.py:774
 msgid "Content archiving"
 msgstr "Archivage de contenu"
 
-#: src/pyams_content/workflow/__init__.py:668
+#: src/pyams_content/workflow/__init__.py:724
 #, python-format
 msgid "{principal} submitted an archive request for content « {title} »"
 msgstr "{principal} a demandé l'archivage du contenu « {title} »"
 
-#: src/pyams_content/workflow/__init__.py:673
+#: src/pyams_content/workflow/__init__.py:746
 msgid "Cancel archiving request"
 msgstr "Annuler la demande d'archivage"
 
-#: src/pyams_content/workflow/__init__.py:680
+#: src/pyams_content/workflow/__init__.py:753
 msgid "Archive request canceled"
 msgstr "Annulation de la demande d'archivage"
 
-#: src/pyams_content/workflow/__init__.py:684
+#: src/pyams_content/workflow/__init__.py:757
 #, python-format
 msgid "{principal} cancelled the archive request for content « {title} »"
 msgstr "{principal} a annulé la demande d'archivage du contenu « {title} »"
 
-#: src/pyams_content/workflow/__init__.py:706
+#: src/pyams_content/workflow/__init__.py:779
 msgid "Archive published content"
 msgstr "Archivage automatique d'un contenu publié"
 
-#: src/pyams_content/workflow/__init__.py:710
-#: src/pyams_content/workflow/__init__.py:718
-#: src/pyams_content/workflow/__init__.py:726
+#: src/pyams_content/workflow/__init__.py:783
+#: src/pyams_content/workflow/__init__.py:791
 msgid "Content archived after version publication"
 msgstr "Archivage automatique après publication"
 
-#: src/pyams_content/workflow/__init__.py:714
+#: src/pyams_content/workflow/__init__.py:787
 msgid "Archive retiring content"
 msgstr "Archivage automatique d'un contenu en attente de retrait"
 
-#: src/pyams_content/workflow/__init__.py:722
-msgid "Archive retired content"
-msgstr "Archivage automatique d'un contenu retiré"
-
-#: src/pyams_content/workflow/__init__.py:840
+#: src/pyams_content/workflow/__init__.py:914
 msgid "PyAMS content workflow"
 msgstr "Workflow standard"
 
 #: src/pyams_content/workflow/zmi/publication.py:48
 #: src/pyams_content/shared/common/zmi/summary.py:148
 msgid "Publication dates"
 msgstr "Dates de publication"
@@ -2208,15 +2225,17 @@
 
 #: src/pyams_content/component/paragraph/zmi/container.py:251
 msgid "Click to show/hide paragraph editor"
 msgstr "Cliquer pour afficher/masquer l'éditeur du bloc"
 
 #: src/pyams_content/component/paragraph/zmi/container.py:307
 msgid "Click to lock/unlock paragraph"
-msgstr "Cliquer pour (dé)verrouiller ce bloc"
+msgstr ""
+"Cliquer pour (dé)verrouiller ce bloc ; un bloc verrouillé ne peut pas être "
+"supprimé par les contributeurs (mais il peut être masqué)"
 
 #: src/pyams_content/component/paragraph/zmi/container.py:309
 msgid "This paragraph is locked and can't be removed!"
 msgstr "Ce bloc est verrouillé et ne peut pas être supprimé !"
 
 #: src/pyams_content/component/paragraph/zmi/container.py:311
 msgid "This paragraph is not locked"
@@ -2231,19 +2250,19 @@
 msgid "Paragraphs list"
 msgstr "Liste des blocs de contenu"
 
 #: src/pyams_content/component/paragraph/zmi/container.py:379
 msgid "Default paragraphs"
 msgstr "Blocs de contenu par défaut"
 
-#: src/pyams_content/component/paragraph/zmi/container.py:465
+#: src/pyams_content/component/paragraph/zmi/container.py:466
 msgid "Links and attachments"
 msgstr "Récap. liens et pièces jointes"
 
-#: src/pyams_content/component/paragraph/zmi/container.py:486
+#: src/pyams_content/component/paragraph/zmi/container.py:487
 msgid "Content blocks links and attachments"
 msgstr "Liens et pièces jointes par bloc de contenu"
 
 #: src/pyams_content/component/paragraph/zmi/__init__.py:78
 msgid "Paragraphs types"
 msgstr "Types de blocs de contenu"
 
@@ -4254,15 +4273,15 @@
 "All versions of this content which are not archived will be transferred to "
 "newly selected owner"
 msgstr ""
 "La propriété de toutes les versions de ce contenu qui ne sont pas archivées "
 "sera transférée au nouveau propriétaire sélectionné."
 
 #: src/pyams_content/shared/common/zmi/dashboard.py:110
-#: src/pyams_content/shared/common/zmi/content.py:214
+#: src/pyams_content/shared/common/zmi/content.py:223
 msgid "Content publication start date is not passed yet"
 msgstr "La date de début de publication de ce contenu n'est pas encore passée"
 
 #: src/pyams_content/shared/common/zmi/dashboard.py:292
 #: src/pyams_content/root/zmi/dashboard.py:96
 msgid "Users activity"
 msgstr "Suivre l'activité"
@@ -4518,47 +4537,47 @@
 msgstr "Texte recherché"
 
 #: src/pyams_content/shared/common/zmi/search.py:211
 #: src/pyams_content/root/zmi/search.py:150
 msgid "Entered text will be search in title only"
 msgstr "La requête s'applique au titre uniquement..."
 
-#: src/pyams_content/shared/common/zmi/content.py:161
+#: src/pyams_content/shared/common/zmi/content.py:170
 #, python-format
 msgid "from {}"
 msgstr "de {}"
 
 #. init state format
-#: src/pyams_content/shared/common/zmi/content.py:200
+#: src/pyams_content/shared/common/zmi/content.py:209
 #, python-format
 msgid "{state} <span class=\"px-1\">by</span> {principal}"
 msgstr "{state} <span class=\"px-1\">par</span> {principal}"
 
-#: src/pyams_content/shared/common/zmi/content.py:239
+#: src/pyams_content/shared/common/zmi/content.py:248
 #, python-format
 msgid "since {date}"
 msgstr "depuis {date}"
 
-#: src/pyams_content/shared/common/zmi/content.py:252
+#: src/pyams_content/shared/common/zmi/content.py:261
 msgid "access published version"
 msgstr "accéder à la version publiée"
 
-#: src/pyams_content/shared/common/zmi/content.py:261
+#: src/pyams_content/shared/common/zmi/content.py:270
 msgid "access new version"
 msgstr "accéder à la version en préparation"
 
-#: src/pyams_content/shared/common/zmi/content.py:273
+#: src/pyams_content/shared/common/zmi/content.py:282
 msgid "access waiting version"
 msgstr "accéder à la version en attente"
 
-#: src/pyams_content/shared/common/zmi/content.py:288
+#: src/pyams_content/shared/common/zmi/content.py:297
 msgid "access retired version"
 msgstr "accéder à la version retirée"
 
-#: src/pyams_content/shared/common/zmi/content.py:301
+#: src/pyams_content/shared/common/zmi/content.py:310
 msgid "access archived version"
 msgstr "accéder à la version archivée"
 
 #: src/pyams_content/shared/common/zmi/manager.py:71
 msgid "Shared content management"
 msgstr "Gérer ce gabarit"
 
@@ -4694,14 +4713,18 @@
 msgid "Search..."
 msgstr "Recherche rapide..."
 
 #: src/pyams_content/shared/common/zmi/templates/quick-search.pt:20
 msgid "Advanced search..."
 msgstr "Recherche avancée..."
 
+#: src/pyams_content/shared/common/zmi/templates/content-header.pt:7
+msgid "Back to dashboard"
+msgstr "Revenir au tableau de bord"
+
 #: src/pyams_content/shared/common/zmi/viewlet/__init__.py:40
 msgid "Shared contents"
 msgstr "Gabarits"
 
 #: src/pyams_content/shared/common/zmi/viewlet/__init__.py:64
 msgid "Shared tools"
 msgstr "Outils"
@@ -5915,14 +5938,17 @@
 msgid "Main site management"
 msgstr "Gérer le portail"
 
 #: src/pyams_content/root/zmi/__init__.py:75
 msgid "Site information"
 msgstr "Informations générales"
 
+#~ msgid "Archive retired content"
+#~ msgstr "Archivage automatique d'un contenu retiré"
+
 #~ msgid "End of alert"
 #~ msgstr "Fin d'alerte"
 
 #~ msgid "Information"
 #~ msgstr "Information"
 
 #~ msgid "Warning"
```

### Comparing `pyams_content-1.99.2/src/pyams_content/locales/pyams_content.pot` & `pyams_content-1.99.3/src/pyams_content/locales/pyams_content.pot`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2024-04-24 23:44+0200\n"
+"POT-Creation-Date: 2024-05-05 16:18+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -97,15 +97,15 @@
 msgstr ""
 
 #: ./src/pyams_content/zmi/dashboard.py:85
 msgid "Visible element?"
 msgstr ""
 
 #: ./src/pyams_content/zmi/dashboard.py:112
-#: ./src/pyams_content/reference/zmi/table.py:98
+#: ./src/pyams_content/reference/zmi/table.py:99
 #: ./src/pyams_content/feature/navigation/portlet/interfaces.py:33
 #: ./src/pyams_content/feature/navigation/portlet/interfaces.py:47
 #: ./src/pyams_content/feature/search/portlet/interfaces.py:44
 #: ./src/pyams_content/interfaces/__init__.py:122
 #: ./src/pyams_content/component/paragraph/zmi/container.py:236
 #: ./src/pyams_content/component/paragraph/portlet/interfaces.py:33
 #: ./src/pyams_content/component/gallery/interfaces.py:118
@@ -169,32 +169,28 @@
 msgid "Table managers"
 msgstr ""
 
 #: ./src/pyams_content/reference/interfaces.py:49
 msgid "Table managers can handle all table contents"
 msgstr ""
 
-#: ./src/pyams_content/reference/zmi/table.py:50
+#: ./src/pyams_content/reference/zmi/table.py:51
 #: ./src/pyams_content/shared/site/zmi/manager.py:167
 #: ./src/pyams_content/shared/site/zmi/folder.py:180
 #: ./src/pyams_content/shared/common/zmi/manager.py:82
 #: ./src/pyams_content/shared/common/zmi/__init__.py:305
 #: ./src/pyams_content/root/zmi/__init__.py:63
 msgid "Properties"
 msgstr ""
 
-#: ./src/pyams_content/reference/zmi/table.py:61
-msgid "Pictograms table"
-msgstr ""
-
-#: ./src/pyams_content/reference/zmi/table.py:62
+#: ./src/pyams_content/reference/zmi/table.py:63
 msgid "Edit table properties"
 msgstr ""
 
-#: ./src/pyams_content/reference/zmi/table.py:72
+#: ./src/pyams_content/reference/zmi/table.py:73
 msgid "Table management"
 msgstr ""
 
 #: ./src/pyams_content/reference/zmi/__init__.py:33
 #: ./src/pyams_content/shared/view/zmi/references.py:50
 msgid "References"
 msgstr ""
@@ -240,28 +236,32 @@
 msgid "Selected pictograms"
 msgstr ""
 
 #: ./src/pyams_content/reference/pictogram/interfaces.py:74
 msgid "List of selected pictograms which will be available to shared contents"
 msgstr ""
 
-#: ./src/pyams_content/reference/pictogram/zmi/table.py:41
-#: ./src/pyams_content/reference/pictogram/zmi/table.py:101
+#: ./src/pyams_content/reference/pictogram/zmi/table.py:42
+#: ./src/pyams_content/reference/pictogram/zmi/table.py:102
 #: ./src/pyams_content/shared/common/zmi/types/__init__.py:187
 msgid "Pictograms"
 msgstr ""
 
-#: ./src/pyams_content/reference/pictogram/zmi/table.py:59
+#: ./src/pyams_content/reference/pictogram/zmi/table.py:60
 msgid "Table contents"
 msgstr ""
 
-#: ./src/pyams_content/reference/pictogram/zmi/table.py:103
+#: ./src/pyams_content/reference/pictogram/zmi/table.py:105
 msgid "Pictograms list"
 msgstr ""
 
+#: ./src/pyams_content/reference/pictogram/zmi/table.py:113
+msgid "Pictograms table"
+msgstr ""
+
 #: ./src/pyams_content/reference/pictogram/zmi/manager.py:49
 msgid "Pictograms selection"
 msgstr ""
 
 #: ./src/pyams_content/reference/pictogram/zmi/manager.py:59
 msgid "Pictograms management"
 msgstr ""
@@ -322,464 +322,481 @@
 
 #: ./src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt:26
 #: ./src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt:61
 msgid "Switch pictogram selection"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:69
-#: ./src/pyams_content/workflow/__init__.py:83
+#: ./src/pyams_content/workflow/__init__.py:84
 msgid "Draft"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:70
-#: ./src/pyams_content/workflow/__init__.py:87
+#: ./src/pyams_content/workflow/__init__.py:88
 msgid "Published (waiting)"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:71
-#: ./src/pyams_content/workflow/__init__.py:88
+#: ./src/pyams_content/workflow/__init__.py:89
 #: ./src/pyams_content/shared/common/zmi/header.py:66
 #: ./src/pyams_content/shared/common/zmi/header.py:69
 #: ./src/pyams_content/shared/common/zmi/header.py:76
 msgid "Published"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:72
-#: ./src/pyams_content/workflow/__init__.py:92
+#: ./src/pyams_content/workflow/__init__.py:93
 msgid "Archived"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:73
-#: ./src/pyams_content/workflow/__init__.py:93
+#: ./src/pyams_content/workflow/__init__.py:94
 msgid "Deleted"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:82
-#: ./src/pyams_content/workflow/__init__.py:102
+#: ./src/pyams_content/workflow/__init__.py:103
 msgid "draft created"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:83
-#: ./src/pyams_content/workflow/__init__.py:104
+#: ./src/pyams_content/workflow/__init__.py:105
 msgid "published (waiting)"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:84
-#: ./src/pyams_content/workflow/__init__.py:105
+#: ./src/pyams_content/workflow/__init__.py:106
 msgid "published"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:85
-#: ./src/pyams_content/workflow/__init__.py:109
+#: ./src/pyams_content/workflow/__init__.py:110
 msgid "archived"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:249
-#: ./src/pyams_content/workflow/__init__.py:345
+#: ./src/pyams_content/workflow/__init__.py:353
 #, python-format
 msgid "Published version {0}"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:304
-#: ./src/pyams_content/workflow/__init__.py:405
+#: ./src/pyams_content/workflow/__init__.py:413
 msgid "Initialize"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:307
-#: ./src/pyams_content/workflow/__init__.py:408
+#: ./src/pyams_content/workflow/__init__.py:416
 msgid "Draft creation"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:310
-#: ./src/pyams_content/workflow/__init__.py:429
-#: ./src/pyams_content/workflow/__init__.py:542
+#: ./src/pyams_content/workflow/__init__.py:437
+#: ./src/pyams_content/workflow/__init__.py:550
 msgid "Pre-publish content"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:315
-#: ./src/pyams_content/workflow/__init__.py:434
-#: ./src/pyams_content/workflow/__init__.py:547
+#: ./src/pyams_content/workflow/__init__.py:442
+#: ./src/pyams_content/workflow/__init__.py:555
+#: ./src/pyams_content/workflow/__init__.py:686
 msgid "Content pre-published"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:317
 #: ./src/pyams_content/workflow/basic.py:332
 #: ./src/pyams_content/workflow/basic.py:357
-#: ./src/pyams_content/workflow/__init__.py:436
-#: ./src/pyams_content/workflow/__init__.py:453
-#: ./src/pyams_content/workflow/__init__.py:549
-#: ./src/pyams_content/workflow/__init__.py:573
-#: ./src/pyams_content/workflow/__init__.py:591
+#: ./src/pyams_content/workflow/__init__.py:444
+#: ./src/pyams_content/workflow/__init__.py:461
+#: ./src/pyams_content/workflow/__init__.py:557
+#: ./src/pyams_content/workflow/__init__.py:581
+#: ./src/pyams_content/workflow/__init__.py:599
+#: ./src/pyams_content/workflow/__init__.py:688
+#: ./src/pyams_content/workflow/__init__.py:705
 msgid "Content publication"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:318
-#: ./src/pyams_content/workflow/__init__.py:437
-#: ./src/pyams_content/workflow/__init__.py:550
+#: ./src/pyams_content/workflow/__init__.py:445
+#: ./src/pyams_content/workflow/__init__.py:558
+#: ./src/pyams_content/workflow/__init__.py:689
 #, python-format
 msgid "{principal} pre-published the content « {title} »"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:322
-#: ./src/pyams_content/workflow/__init__.py:562
+#: ./src/pyams_content/workflow/__init__.py:570
 msgid "Cancel publication"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:330
-#: ./src/pyams_content/workflow/__init__.py:570
+#: ./src/pyams_content/workflow/__init__.py:578
 msgid "Publication canceled"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:333
-#: ./src/pyams_content/workflow/__init__.py:574
+#: ./src/pyams_content/workflow/__init__.py:582
 #, python-format
 msgid "{principal} cancelled the publication for content « {title} »"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:338
 #: ./src/pyams_content/workflow/basic.py:346
-#: ./src/pyams_content/workflow/__init__.py:441
-#: ./src/pyams_content/workflow/__init__.py:554
-#: ./src/pyams_content/workflow/__init__.py:579
+#: ./src/pyams_content/workflow/__init__.py:449
+#: ./src/pyams_content/workflow/__init__.py:562
+#: ./src/pyams_content/workflow/__init__.py:587
 msgid "Publish content"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:343
 #: ./src/pyams_content/workflow/basic.py:355
-#: ./src/pyams_content/workflow/__init__.py:451
-#: ./src/pyams_content/workflow/__init__.py:559
-#: ./src/pyams_content/workflow/__init__.py:589
+#: ./src/pyams_content/workflow/__init__.py:459
+#: ./src/pyams_content/workflow/__init__.py:567
+#: ./src/pyams_content/workflow/__init__.py:597
+#: ./src/pyams_content/workflow/__init__.py:703
 msgid "Content published"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:358
-#: ./src/pyams_content/workflow/__init__.py:454
-#: ./src/pyams_content/workflow/__init__.py:592
+#: ./src/pyams_content/workflow/__init__.py:462
+#: ./src/pyams_content/workflow/__init__.py:600
+#: ./src/pyams_content/workflow/__init__.py:706
 #, python-format
 msgid "{principal} published the content « {title} »"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:363
-#: ./src/pyams_content/workflow/__init__.py:689
+#: ./src/pyams_content/workflow/__init__.py:729
+#: ./src/pyams_content/workflow/__init__.py:762
 msgid "Archive content"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:372
-#: ./src/pyams_content/workflow/__init__.py:698
+#: ./src/pyams_content/workflow/__init__.py:738
+#: ./src/pyams_content/workflow/__init__.py:771
 msgid "Content archived"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:374
-#: ./src/pyams_content/workflow/__init__.py:702
+#: ./src/pyams_content/workflow/__init__.py:742
+#: ./src/pyams_content/workflow/__init__.py:775
 #, python-format
 msgid "{principal} archived content « {title} »"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:378
 #: ./src/pyams_content/workflow/basic.py:390
-#: ./src/pyams_content/workflow/__init__.py:730
-#: ./src/pyams_content/workflow/__init__.py:742
-#: ./src/pyams_content/workflow/__init__.py:754
-#: ./src/pyams_content/workflow/__init__.py:766
-#: ./src/pyams_content/workflow/__init__.py:778
+#: ./src/pyams_content/workflow/__init__.py:795
+#: ./src/pyams_content/workflow/__init__.py:808
+#: ./src/pyams_content/workflow/__init__.py:821
+#: ./src/pyams_content/workflow/__init__.py:834
+#: ./src/pyams_content/workflow/__init__.py:847
 msgid "Create new version"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:386
 #: ./src/pyams_content/workflow/basic.py:398
-#: ./src/pyams_content/workflow/__init__.py:738
-#: ./src/pyams_content/workflow/__init__.py:750
-#: ./src/pyams_content/workflow/__init__.py:762
-#: ./src/pyams_content/workflow/__init__.py:774
-#: ./src/pyams_content/workflow/__init__.py:786
+#: ./src/pyams_content/workflow/__init__.py:804
+#: ./src/pyams_content/workflow/__init__.py:817
+#: ./src/pyams_content/workflow/__init__.py:830
+#: ./src/pyams_content/workflow/__init__.py:843
+#: ./src/pyams_content/workflow/__init__.py:856
 msgid "New version created"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:402
-#: ./src/pyams_content/workflow/__init__.py:790
+#: ./src/pyams_content/workflow/__init__.py:860
 msgid "Delete version"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:410
-#: ./src/pyams_content/workflow/__init__.py:798
+#: ./src/pyams_content/workflow/__init__.py:869
 msgid "Version deleted"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:428
 msgid "PyAMS basic workflow"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:447
 #: ./src/pyams_content/workflow/basic.py:484
-#: ./src/pyams_content/workflow/__init__.py:859
-#: ./src/pyams_content/workflow/__init__.py:896
+#: ./src/pyams_content/workflow/__init__.py:933
+#: ./src/pyams_content/workflow/__init__.py:970
 #: ./src/pyams_content/shared/common/zmi/workflow.py:166
 #, python-format
 msgid "{state} {date}"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:451
 #: ./src/pyams_content/workflow/basic.py:476
-#: ./src/pyams_content/workflow/__init__.py:863
-#: ./src/pyams_content/workflow/__init__.py:888
+#: ./src/pyams_content/workflow/__init__.py:937
+#: ./src/pyams_content/workflow/__init__.py:962
 msgid "Unknown state"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:474
-#: ./src/pyams_content/workflow/__init__.py:886
+#: ./src/pyams_content/workflow/__init__.py:960
 msgid "new version created"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:480
-#: ./src/pyams_content/workflow/__init__.py:892
+#: ./src/pyams_content/workflow/__init__.py:966
 msgid "publication request cancelled"
 msgstr ""
 
 #: ./src/pyams_content/workflow/basic.py:482
-#: ./src/pyams_content/workflow/__init__.py:894
+#: ./src/pyams_content/workflow/__init__.py:968
 msgid "publication refused"
 msgstr ""
 
 #: ./src/pyams_content/workflow/task.py:52
 msgid "Content publisher task"
 msgstr ""
 
-#: ./src/pyams_content/workflow/task.py:88
+#: ./src/pyams_content/workflow/task.py:89
 msgid "Content archiver task"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:84
+#: ./src/pyams_content/workflow/__init__.py:85
 msgid "Proposed"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:85
+#: ./src/pyams_content/workflow/__init__.py:86
 msgid "Canceled"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:86
+#: ./src/pyams_content/workflow/__init__.py:87
 msgid "Refused"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:89
+#: ./src/pyams_content/workflow/__init__.py:90
 msgid "Retiring"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:90
+#: ./src/pyams_content/workflow/__init__.py:91
 #: ./src/pyams_content/shared/common/zmi/header.py:63
 msgid "Retired"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:91
+#: ./src/pyams_content/workflow/__init__.py:92
 msgid "Archiving"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:103
+#: ./src/pyams_content/workflow/__init__.py:104
 msgid "publication requested"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:106
+#: ./src/pyams_content/workflow/__init__.py:107
 msgid "retiring requested"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:107
+#: ./src/pyams_content/workflow/__init__.py:108
 msgid "retired"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:108
+#: ./src/pyams_content/workflow/__init__.py:109
 msgid "archiving requested"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:411
-#: ./src/pyams_content/workflow/__init__.py:459
+#: ./src/pyams_content/workflow/__init__.py:419
+#: ./src/pyams_content/workflow/__init__.py:467
 msgid "Propose publication"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:418
-#: ./src/pyams_content/workflow/__init__.py:423
-#: ./src/pyams_content/workflow/__init__.py:466
-#: ./src/pyams_content/workflow/__init__.py:471
-#: ./src/pyams_content/workflow/__init__.py:488
-#: ./src/pyams_content/workflow/__init__.py:520
+#: ./src/pyams_content/workflow/__init__.py:426
+#: ./src/pyams_content/workflow/__init__.py:431
+#: ./src/pyams_content/workflow/__init__.py:474
+#: ./src/pyams_content/workflow/__init__.py:479
+#: ./src/pyams_content/workflow/__init__.py:496
+#: ./src/pyams_content/workflow/__init__.py:528
 msgid "Publication request"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:419
-#: ./src/pyams_content/workflow/__init__.py:467
-#: ./src/pyams_content/workflow/__init__.py:604
-#: ./src/pyams_content/workflow/__init__.py:662
+#: ./src/pyams_content/workflow/__init__.py:427
+#: ./src/pyams_content/workflow/__init__.py:475
+#: ./src/pyams_content/workflow/__init__.py:612
+#: ./src/pyams_content/workflow/__init__.py:718
 msgid ""
 "content managers authorized to take charge of your content are going to be "
 "notified of your request."
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:424
-#: ./src/pyams_content/workflow/__init__.py:472
+#: ./src/pyams_content/workflow/__init__.py:432
+#: ./src/pyams_content/workflow/__init__.py:480
 #, python-format
 msgid "{principal} submitted a publication request for content « {title} »"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:477
+#: ./src/pyams_content/workflow/__init__.py:485
 msgid "Cancel publication request"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:485
+#: ./src/pyams_content/workflow/__init__.py:493
 msgid "Publication request canceled"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:489
+#: ./src/pyams_content/workflow/__init__.py:497
 #, python-format
 msgid "{principal} cancelled the publication request for content « {title} »"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:494
+#: ./src/pyams_content/workflow/__init__.py:502
 msgid "Reset canceled publication to draft"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:498
-#: ./src/pyams_content/workflow/__init__.py:530
+#: ./src/pyams_content/workflow/__init__.py:506
+#: ./src/pyams_content/workflow/__init__.py:538
 msgid "State reset to 'draft' (automatic)"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:502
+#: ./src/pyams_content/workflow/__init__.py:510
 msgid "Reset canceled publication to retired"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:506
+#: ./src/pyams_content/workflow/__init__.py:514
 msgid "State reset to 'retired' (automatic)"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:510
+#: ./src/pyams_content/workflow/__init__.py:518
 msgid "Refuse publication"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:518
+#: ./src/pyams_content/workflow/__init__.py:526
 msgid "Publication refused"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:521
+#: ./src/pyams_content/workflow/__init__.py:529
 #, python-format
 msgid "{principal} refused the publication request for content « {title} »"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:526
+#: ./src/pyams_content/workflow/__init__.py:534
 msgid "Reset refused publication to draft"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:534
+#: ./src/pyams_content/workflow/__init__.py:542
 msgid "Reset refused publication to retired"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:538
+#: ./src/pyams_content/workflow/__init__.py:546
 msgid "State reset to 'refused' (automatic)"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:597
+#: ./src/pyams_content/workflow/__init__.py:605
 msgid "Request retiring"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:603
+#: ./src/pyams_content/workflow/__init__.py:611
 msgid "Retire request"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:609
-#: ./src/pyams_content/workflow/__init__.py:632
-#: ./src/pyams_content/workflow/__init__.py:650
+#: ./src/pyams_content/workflow/__init__.py:617
+#: ./src/pyams_content/workflow/__init__.py:635
+#: ./src/pyams_content/workflow/__init__.py:658
+#: ./src/pyams_content/workflow/__init__.py:676
 msgid "Content removal"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:610
+#: ./src/pyams_content/workflow/__init__.py:618
 #, python-format
 msgid "{principal} submitted a retire request for content « {title} »"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:615
+#: ./src/pyams_content/workflow/__init__.py:623
+#: ./src/pyams_content/workflow/__init__.py:640
 msgid "Retired content"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:619
+#: ./src/pyams_content/workflow/__init__.py:632
+#: ./src/pyams_content/workflow/__init__.py:673
+msgid "Content retired"
+msgstr ""
+
+#: ./src/pyams_content/workflow/__init__.py:636
+#: ./src/pyams_content/workflow/__init__.py:677
+#, python-format
+msgid "{principal} retired content « {title} »"
+msgstr ""
+
+#: ./src/pyams_content/workflow/__init__.py:645
 msgid "Content retired after passed expiration date"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:622
+#: ./src/pyams_content/workflow/__init__.py:648
 msgid "Cancel retiring request"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:629
+#: ./src/pyams_content/workflow/__init__.py:655
 msgid "Retire request canceled"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:633
+#: ./src/pyams_content/workflow/__init__.py:659
 #, python-format
 msgid "{principal} cancelled the retiring request for content « {title} »"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:638
+#: ./src/pyams_content/workflow/__init__.py:664
 msgid "Retire content"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:647
-msgid "Content retired"
+#: ./src/pyams_content/workflow/__init__.py:681
+msgid "Pre-publish retired content"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:651
-#, python-format
-msgid "{principal} retired content « {title} »"
+#: ./src/pyams_content/workflow/__init__.py:693
+msgid "Publish retired content"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:655
+#: ./src/pyams_content/workflow/__init__.py:711
 msgid "Request archive"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:661
+#: ./src/pyams_content/workflow/__init__.py:717
 msgid "Archive request"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:667
-#: ./src/pyams_content/workflow/__init__.py:683
-#: ./src/pyams_content/workflow/__init__.py:701
+#: ./src/pyams_content/workflow/__init__.py:723
+#: ./src/pyams_content/workflow/__init__.py:741
+#: ./src/pyams_content/workflow/__init__.py:756
+#: ./src/pyams_content/workflow/__init__.py:774
 msgid "Content archiving"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:668
+#: ./src/pyams_content/workflow/__init__.py:724
 #, python-format
 msgid "{principal} submitted an archive request for content « {title} »"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:673
+#: ./src/pyams_content/workflow/__init__.py:746
 msgid "Cancel archiving request"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:680
+#: ./src/pyams_content/workflow/__init__.py:753
 msgid "Archive request canceled"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:684
+#: ./src/pyams_content/workflow/__init__.py:757
 #, python-format
 msgid "{principal} cancelled the archive request for content « {title} »"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:706
+#: ./src/pyams_content/workflow/__init__.py:779
 msgid "Archive published content"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:710
-#: ./src/pyams_content/workflow/__init__.py:718
-#: ./src/pyams_content/workflow/__init__.py:726
+#: ./src/pyams_content/workflow/__init__.py:783
+#: ./src/pyams_content/workflow/__init__.py:791
 msgid "Content archived after version publication"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:714
+#: ./src/pyams_content/workflow/__init__.py:787
 msgid "Archive retiring content"
 msgstr ""
 
-#: ./src/pyams_content/workflow/__init__.py:722
-msgid "Archive retired content"
-msgstr ""
-
-#: ./src/pyams_content/workflow/__init__.py:840
+#: ./src/pyams_content/workflow/__init__.py:914
 msgid "PyAMS content workflow"
 msgstr ""
 
 #: ./src/pyams_content/workflow/zmi/publication.py:48
 #: ./src/pyams_content/shared/common/zmi/summary.py:148
 msgid "Publication dates"
 msgstr ""
@@ -2108,19 +2125,19 @@
 msgid "Paragraphs list"
 msgstr ""
 
 #: ./src/pyams_content/component/paragraph/zmi/container.py:379
 msgid "Default paragraphs"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/zmi/container.py:465
+#: ./src/pyams_content/component/paragraph/zmi/container.py:466
 msgid "Links and attachments"
 msgstr ""
 
-#: ./src/pyams_content/component/paragraph/zmi/container.py:486
+#: ./src/pyams_content/component/paragraph/zmi/container.py:487
 msgid "Content blocks links and attachments"
 msgstr ""
 
 #: ./src/pyams_content/component/paragraph/zmi/__init__.py:78
 msgid "Paragraphs types"
 msgstr ""
 
@@ -3934,15 +3951,15 @@
 #: ./src/pyams_content/shared/common/zmi/owner.py:458
 msgid ""
 "All versions of this content which are not archived will be transferred to "
 "newly selected owner"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/dashboard.py:110
-#: ./src/pyams_content/shared/common/zmi/content.py:214
+#: ./src/pyams_content/shared/common/zmi/content.py:223
 msgid "Content publication start date is not passed yet"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/dashboard.py:292
 #: ./src/pyams_content/root/zmi/dashboard.py:96
 msgid "Users activity"
 msgstr ""
@@ -4195,47 +4212,47 @@
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/search.py:211
 #: ./src/pyams_content/root/zmi/search.py:150
 msgid "Entered text will be search in title only"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/zmi/content.py:161
+#: ./src/pyams_content/shared/common/zmi/content.py:170
 #, python-format
 msgid "from {}"
 msgstr ""
 
 #. init state format
-#: ./src/pyams_content/shared/common/zmi/content.py:200
+#: ./src/pyams_content/shared/common/zmi/content.py:209
 #, python-format
 msgid "{state} <span class=\"px-1\">by</span> {principal}"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/zmi/content.py:239
+#: ./src/pyams_content/shared/common/zmi/content.py:248
 #, python-format
 msgid "since {date}"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/zmi/content.py:252
+#: ./src/pyams_content/shared/common/zmi/content.py:261
 msgid "access published version"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/zmi/content.py:261
+#: ./src/pyams_content/shared/common/zmi/content.py:270
 msgid "access new version"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/zmi/content.py:273
+#: ./src/pyams_content/shared/common/zmi/content.py:282
 msgid "access waiting version"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/zmi/content.py:288
+#: ./src/pyams_content/shared/common/zmi/content.py:297
 msgid "access retired version"
 msgstr ""
 
-#: ./src/pyams_content/shared/common/zmi/content.py:301
+#: ./src/pyams_content/shared/common/zmi/content.py:310
 msgid "access archived version"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/manager.py:71
 msgid "Shared content management"
 msgstr ""
 
@@ -4364,14 +4381,18 @@
 msgid "Search..."
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/templates/quick-search.pt:20
 msgid "Advanced search..."
 msgstr ""
 
+#: ./src/pyams_content/shared/common/zmi/templates/content-header.pt:7
+msgid "Back to dashboard"
+msgstr ""
+
 #: ./src/pyams_content/shared/common/zmi/viewlet/__init__.py:40
 msgid "Shared contents"
 msgstr ""
 
 #: ./src/pyams_content/shared/common/zmi/viewlet/__init__.py:64
 msgid "Shared tools"
 msgstr ""
```

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/__init__.py` & `pyams_content-1.99.3/src/pyams_content/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/reference/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/pictogram/__init__.py` & `pyams_content-1.99.3/src/pyams_content/reference/pictogram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/pictogram/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/reference/pictogram/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/pictogram/manager.py` & `pyams_content-1.99.3/src/pyams_content/reference/pictogram/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/manager.py` & `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/table.py` & `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/table.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/__init__.py` & `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/manager.py` & `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt` & `pyams_content-1.99.3/src/pyams_content/reference/pictogram/zmi/widget/templates/selection.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/reference/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/zmi/table.py` & `pyams_content-1.99.3/src/pyams_content/reference/zmi/table.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/reference/zmi/viewlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/reference/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/root/__init__.py` & `pyams_content-1.99.3/src/pyams_content/root/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/root/configuration.py` & `pyams_content-1.99.3/src/pyams_content/root/configuration.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/root/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/root/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/root/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/root/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/root/zmi/dashboard.py` & `pyams_content-1.99.3/src/pyams_content/root/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/root/zmi/search.py` & `pyams_content-1.99.3/src/pyams_content/root/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/root/zmi/sites.py` & `pyams_content-1.99.3/src/pyams_content/root/zmi/sites.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/alert/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/alert/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/alert/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/alert/manager.py` & `pyams_content-1.99.3/src/pyams_content/shared/alert/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/alert/types.py` & `pyams_content-1.99.3/src/pyams_content/shared/alert/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/alert/zmi/types.py` & `pyams_content-1.99.3/src/pyams_content/shared/alert/zmi/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/blog/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/blog/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/calendar/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/interfaces/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/interfaces/types.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/interfaces/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/manager.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portal.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portal.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/header.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/header.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/specificities.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/templates/header-default.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/skin/title.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/skin/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/specificities.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/title.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/header.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/specificities.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/templates/header-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/portlet/zmi/title.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/portlet/zmi/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/restrictions.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/security.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/security.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/skin/breadcrumb.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/skin/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/skin/oid.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/skin/oid.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/skin/specificities.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/skin/specificities.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/skin/title.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/skin/title.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/skin/types.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/skin/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/skin/url.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/skin/url.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/skin/workflow.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/skin/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/types.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/types.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/content.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """PyAMS_content.shared.common.zmi.content module
 
 This module provides common management components for shared contents.
 """
 
 from zope.interface import Interface
 
+from pyams_content.shared.common import IBaseSharedTool
 from pyams_content.shared.common.interfaces import ISharedContent, IWfSharedContent, IWfSharedContentRoles
 from pyams_content.shared.common.interfaces.types import IWfTypedSharedContent
 from pyams_content.zmi.interfaces import IDashboardColumn, IDashboardContentNumber, \
     IDashboardContentOwner, IDashboardContentType, ISiteRootDashboardContentType
 from pyams_i18n.interfaces import II18n
 from pyams_security.utility import get_principal
 from pyams_security_views.interfaces.login import ILoginView
@@ -149,14 +150,22 @@
                 context=IWfSharedContent, layer=IAdminLayer,
                 manager=IHeaderViewletManager, weight=10)
 @template_config(template='templates/content-header.pt')
 class SharedContentHeaderViewlet(ContentHeaderViewlet):
     """Shared content header viewlet"""
 
     @property
+    def parent_target_url(self):
+        """Parent target URL"""
+        tool = get_parent(self.context, IBaseSharedTool)
+        if tool is None:
+            return None
+        return absolute_url(tool, self.request, 'admin#dashboard.html')
+
+    @property
     def owner(self):
         """Owner getter"""
         owner = IWfSharedContentRoles(self.context).owner
         if owner:
             translate = self.request.localizer.translate
             return translate(_("from {}")).format(
                 get_principal(self.request, next(iter(owner))).title)
```

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/dashboard.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/header.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/header.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/manager.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/owner.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/owner.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/portal.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/portal.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/reference.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/restrictions.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/restrictions.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/search.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/summary.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/summary.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/quick-search.pt` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/quick-search.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/templates/wf-transition-info.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/container.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/content.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/content.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/types/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/types/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/viewlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/common/zmi/workflow.py` & `pyams_content-1.99.3/src/pyams_content/shared/common/zmi/workflow.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/file/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/file/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/form/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/form/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/form/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/form/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/form/manager.py` & `pyams_content-1.99.3/src/pyams_content/shared/form/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/form/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/form/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/form/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/form/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/hub/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/logo/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/logo/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/container.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/container.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/folder.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/link.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/link.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/manager.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/topic.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/topic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/folder.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/link.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/link.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/manager.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/rename.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/rename.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/search.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/search.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/topic.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/topic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/tree.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/tree.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/viewlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/folder.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/folder.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt` & `pyams_content-1.99.3/src/pyams_content/shared/site/zmi/widget/templates/folder-select-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/topic/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/topic/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/topic/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/topic/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/topic/manager.py` & `pyams_content-1.99.3/src/pyams_content/shared/topic/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/topic/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/topic/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/query.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/query.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/interfaces/settings.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/interfaces/settings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/manager.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/manager.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/merge.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/merge.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt` & `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-list-horizontal.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt` & `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-list-vertical.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt` & `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/templates/view-panels.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/skin/zmi.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/skin/zmi.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt` & `pyams_content-1.99.3/src/pyams_content/shared/view/portlet/zmi/templates/view-preview.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/query.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/query.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/reference.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/reference.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/thesaurus.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/zmi/references.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/zmi/references.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/shared/view/zmi/thesaurus.py` & `pyams_content-1.99.3/src/pyams_content/shared/view/zmi/thesaurus.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/skin/__init__.py` & `pyams_content-1.99.3/src/pyams_content/skin/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/skin/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/skin/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/tests/__init__.py` & `pyams_content-1.99.3/src/pyams_content/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/tests/test_utilsdocs.py` & `pyams_content-1.99.3/src/pyams_content/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/tests/test_utilsdocstrings.py` & `pyams_content-1.99.3/src/pyams_content/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/utils/__init__.py` & `pyams_content-1.99.3/src/pyams_content/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/workflow/__init__.py` & `pyams_content-1.99.3/src/pyams_content/workflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from pyams_content.shared.common.interfaces import DEFAULT_CONTENT_WORKFLOW, IContributorRestrictions, \
     IManagerRestrictions, IWfSharedContentRoles
 from pyams_content.workflow.interfaces import IContentWorkflow
 from pyams_content.workflow.task import ContentArchivingTask, ContentPublishingTask
 from pyams_scheduler.interfaces import IScheduler
 from pyams_scheduler.interfaces.task import IDateTaskScheduling, SCHEDULER_TASK_DATE_MODE
 from pyams_security.interfaces import IRoleProtectedObject
+from pyams_security.interfaces.names import INTERNAL_USER_ID
 from pyams_sequence.interfaces import ISequentialIdInfo
 from pyams_utils.adapter import ContextAdapter, adapter_config
 from pyams_utils.date import format_datetime
 from pyams_utils.registry import get_current_registry, get_utility, query_utility, utility_config
 from pyams_utils.request import check_request
 from pyams_utils.timezone import gmtime
 from pyams_workflow.interfaces import AUTOMATIC_TRANSITION, IWorkflow, IWorkflowInfo, \
@@ -136,14 +137,20 @@
 ARCHIVED_STATES = (ARCHIVED, )
 
 
 #
 # Workflow conditions
 #
 
+def is_internal_user_id(wf, context):
+    """Check if current request principal is internal user ID"""
+    request = check_request()
+    return request.principal.id == INTERNAL_USER_ID
+
+
 def can_propose_content(wf, context):
     """Check if a content can be proposed"""
     # can't propose content if another proposed version already exists
     versions = IWorkflowVersions(context)
     if versions.has_version(PROPOSED):
         return False
     request = check_request()
@@ -338,15 +345,16 @@
     publication_info.publication_date = datetime.utcnow()
     publication_info.publisher = request.principal.id
     version_id = IWorkflowState(context).version_id
     for version in IWorkflowVersions(context).get_versions((PRE_PUBLISHED, PUBLISHED, RETIRING,
                                                             RETIRED, ARCHIVING)):
         if version is not context:
             IWorkflowInfo(version).fire_transition_toward(
-                ARCHIVED, comment=translate(_("Published version {0}")).format(version_id))
+                ARCHIVED,
+                comment=translate(_("Published version {0}")).format(version_id))
     # check expiration date and create auto-archiving task if needed
     # we compare expiration date with current date to handle the case where content is
     # published automatically at application startup, and we add a small amount of time
     # to be sure that scheduler and indexer processes are started
     if publication_info.publication_expiration_date:
         scheduler = query_utility(IScheduler)
         if scheduler is not None:
@@ -611,16 +619,34 @@
                                                     "for content « {title} »"),
                                    order=7)
 
 published_to_retired = Transition(transition_id='published_to_retired',
                                   title=_("Retired content"),
                                   source=PUBLISHED,
                                   destination=RETIRED,
-                                  trigger=SYSTEM_TRANSITION,
-                                  history_label=_("Content retired after passed expiration date"))
+                                  permission=PUBLISH_CONTENT_PERMISSION,
+                                  condition=can_manage_content,
+                                  action=unpublish_action,
+                                  menu_icon_class='far fa-fw fa-stop-circle',
+                                  view_name='wf-retire.html',
+                                  show_operator_warning=True,
+                                  history_label=_("Content retired"),
+                                  notify_roles={WEBMASTER_ROLE, PILOT_ROLE, MANAGER_ROLE,
+                                                OWNER_ROLE},
+                                  notify_title=_("Content removal"),
+                                  notify_message=_("{principal} retired content « {title} »"),
+                                  order=9)
+
+published_to_retired_by_task = Transition(transition_id='published_to_retired_by_task',
+                                          title=_("Retired content"),
+                                          source=PUBLISHED,
+                                          destination=RETIRED,
+                                          trigger=SYSTEM_TRANSITION,
+                                          condition=is_internal_user_id,
+                                          history_label=_("Content retired after passed expiration date"))
 
 retiring_to_published = Transition(transition_id='retiring_to_published',
                                    title=_("Cancel retiring request"),
                                    source=RETIRING,
                                    destination=PUBLISHED,
                                    permission=MANAGE_CONTENT_PERMISSION,
                                    condition=can_cancel_operation,
@@ -647,32 +673,79 @@
                                  history_label=_("Content retired"),
                                  notify_roles={WEBMASTER_ROLE, PILOT_ROLE, MANAGER_ROLE,
                                                OWNER_ROLE},
                                  notify_title=_("Content removal"),
                                  notify_message=_("{principal} retired content « {title} »"),
                                  order=9)
 
+retired_to_prepublished = Transition(transition_id='retired_to_prepublished',
+                                     title=_("Pre-publish retired content"),
+                                     source=RETIRED,
+                                     destination=PRE_PUBLISHED,
+                                     trigger=SYSTEM_TRANSITION,
+                                     action=prepublish_action,
+                                     history_label=_("Content pre-published"),
+                                     notify_roles={'*'},
+                                     notify_title=_("Content publication"),
+                                     notify_message=_("{principal} pre-published the content "
+                                                      "« {title} »"))
+
+retired_to_published = Transition(transition_id='retired_to_published',
+                                  title=_("Publish retired content"),
+                                  source=RETIRED,
+                                  destination=PUBLISHED,
+                                  permission=PUBLISH_CONTENT_PERMISSION,
+                                  condition=can_manage_content,
+                                  action=publish_action,
+                                  prepared_transition=retired_to_prepublished,
+                                  menu_icon_class='fas fa-fw fa-thumbs-up',
+                                  view_name='wf-publish.html',
+                                  show_operator_warning=True,
+                                  history_label=_("Content published"),
+                                  notify_roles={'*'},
+                                  notify_title=_("Content publication"),
+                                  notify_message=_("{principal} published the content "
+                                                   "« {title} »"),
+                                  order=4)
+
 retired_to_archiving = Transition(transition_id='retired_to_archiving',
                                   title=_("Request archive"),
                                   source=RETIRED,
                                   destination=ARCHIVING,
                                   permission=MANAGE_CONTENT_PERMISSION,
-                                  menu_icon_class='fas fa-fw fa-archive',
+                                  menu_icon_class='fas fa-fw fa-eye',
                                   view_name='wf-archiving.html',
                                   history_label=_("Archive request"),
                                   next_step=_("content managers authorized to take charge of "
                                               "your content are going to be notified of your "
                                               "request."),
                                   notify_roles={WEBMASTER_ROLE, PILOT_ROLE, MANAGER_ROLE,
                                                 OWNER_ROLE},
                                   notify_title=_("Content archiving"),
                                   notify_message=_("{principal} submitted an archive request "
                                                    "for content « {title} »"),
                                   order=10)
 
+retired_to_archived = Transition(transition_id='retired_to_archived',
+                                 title=_("Archive content"),
+                                 source=RETIRED,
+                                 destination=ARCHIVED,
+                                 permission=PUBLISH_CONTENT_PERMISSION,
+                                 condition=can_manage_content,
+                                 action=archive_action,
+                                 menu_icon_class='fas fa-fw fa-archive',
+                                 view_name='wf-archive.html',
+                                 show_operator_warning=True,
+                                 history_label=_("Content archived"),
+                                 notify_roles={WEBMASTER_ROLE, PILOT_ROLE, MANAGER_ROLE,
+                                               OWNER_ROLE},
+                                 notify_title=_("Content archiving"),
+                                 notify_message=_("{principal} archived content « {title} »"),
+                                 order=12)
+
 archiving_to_retired = Transition(transition_id='archiving_to_retired',
                                   title=_("Cancel archiving request"),
                                   source=ARCHIVING,
                                   destination=RETIRED,
                                   permission=MANAGE_CONTENT_PERMISSION,
                                   condition=can_cancel_operation,
                                   menu_icon_class='fas fa-fw fa-reply',
@@ -698,106 +771,104 @@
                                    history_label=_("Content archived"),
                                    notify_roles={WEBMASTER_ROLE, PILOT_ROLE, MANAGER_ROLE,
                                                  OWNER_ROLE},
                                    notify_title=_("Content archiving"),
                                    notify_message=_("{principal} archived content « {title} »"),
                                    order=12)
 
-published_to_archived = Transition(transition_id='published_to_archived',
-                                   title=_("Archive published content"),
-                                   source=PUBLISHED,
-                                   destination=ARCHIVED,
-                                   trigger=SYSTEM_TRANSITION,
-                                   history_label=_("Content archived after version publication"),
-                                   action=archive_action)
-
-retiring_to_archived = Transition(transition_id='retiring_to_archived',
-                                  title=_("Archive retiring content"),
-                                  source=RETIRING,
-                                  destination=ARCHIVED,
-                                  trigger=SYSTEM_TRANSITION,
-                                  history_label=_("Content archived after version publication"),
-                                  action=archive_action)
-
-retired_to_archived = Transition(transition_id='retired_to_archived',
-                                 title=_("Archive retired content"),
-                                 source=RETIRED,
-                                 destination=ARCHIVED,
-                                 trigger=SYSTEM_TRANSITION,
-                                 history_label=_("Content archived after version publication"),
-                                 action=archive_action)
+published_to_archived_by_version = Transition(transition_id='published_to_archived',
+                                              title=_("Archive published content"),
+                                              source=PUBLISHED,
+                                              destination=ARCHIVED,
+                                              trigger=SYSTEM_TRANSITION,
+                                              history_label=_("Content archived after version publication"),
+                                              action=archive_action)
+
+retiring_to_archived_by_version = Transition(transition_id='retiring_to_archived',
+                                             title=_("Archive retiring content"),
+                                             source=RETIRING,
+                                             destination=ARCHIVED,
+                                             trigger=SYSTEM_TRANSITION,
+                                             history_label=_("Content archived after version publication"),
+                                             action=archive_action)
 
 published_to_draft = Transition(transition_id='published_to_draft',
                                 title=_("Create new version"),
                                 source=PUBLISHED,
                                 destination=DRAFT,
                                 permission=CREATE_VERSION_PERMISSION,
                                 condition=can_create_new_version,
                                 action=clone_action,
                                 menu_icon_class='far fa-fw fa-file',
+                                menu_divider=True,
                                 view_name='wf-clone.html',
                                 history_label=_("New version created"),
                                 order=13)
 
 retiring_to_draft = Transition(transition_id='retiring_to_draft',
                                title=_("Create new version"),
                                source=RETIRING,
                                destination=DRAFT,
                                permission=CREATE_VERSION_PERMISSION,
                                condition=can_create_new_version,
                                action=clone_action,
                                menu_icon_class='far fa-fw fa-file',
+                               menu_divider=True,
                                view_name='wf-clone.html',
                                history_label=_("New version created"),
                                order=14)
 
 retired_to_draft = Transition(transition_id='retired_to_draft',
                               title=_("Create new version"),
                               source=RETIRED,
                               destination=DRAFT,
                               permission=CREATE_VERSION_PERMISSION,
                               condition=can_create_new_version,
                               action=clone_action,
                               menu_icon_class='far fa-fw fa-file',
+                              menu_divider=True,
                               view_name='wf-clone.html',
                               history_label=_("New version created"),
                               order=15)
 
 archiving_to_draft = Transition(transition_id='archiving_to_draft',
                                 title=_("Create new version"),
                                 source=ARCHIVING,
                                 destination=DRAFT,
                                 permission=CREATE_VERSION_PERMISSION,
                                 condition=can_create_new_version,
                                 action=clone_action,
                                 menu_icon_class='far fa-fw fa-file',
+                                menu_divider=True,
                                 view_name='wf-clone.html',
                                 history_label=_("New version created"),
                                 order=16)
 
 archived_to_draft = Transition(transition_id='archived_to_draft',
                                title=_("Create new version"),
                                source=ARCHIVED,
                                destination=DRAFT,
                                permission=CREATE_VERSION_PERMISSION,
                                condition=can_create_new_version,
                                action=clone_action,
                                menu_icon_class='far fa-fw fa-file',
+                               menu_divider=True,
                                view_name='wf-clone.html',
                                history_label=_("New version created"),
                                order=17)
 
 delete = Transition(transition_id='delete',
                     title=_("Delete version"),
                     source=DRAFT,
                     destination=DELETED,
                     permission=MANAGE_CONTENT_PERMISSION,
                     condition=can_delete_version,
                     action=delete_action,
                     menu_icon_class='fas fa-fw fa-trash',
+                    menu_divider=True,
                     view_name='wf-delete.html',
                     history_label=_("Version deleted"),
                     order=99)
 
 wf_transitions = [
     init,
     draft_to_proposed,
@@ -812,22 +883,25 @@
     refused_to_retired,
     proposed_to_prepublished,
     prepublished_to_published,
     prepublished_to_proposed,
     proposed_to_published,
     published_to_retiring,
     published_to_retired,
+    published_to_retired_by_task,
     retiring_to_published,
     retiring_to_retired,
     retired_to_archiving,
     archiving_to_retired,
-    published_to_archived,
-    retiring_to_archived,
+    retired_to_prepublished,
+    retired_to_published,
     retired_to_archived,
     archiving_to_archived,
+    published_to_archived_by_version,
+    retiring_to_archived_by_version,
     published_to_draft,
     retiring_to_draft,
     retired_to_draft,
     archiving_to_draft,
     archived_to_draft,
     delete
 ]
```

### Comparing `pyams_content-1.99.2/src/pyams_content/workflow/basic.py` & `pyams_content-1.99.3/src/pyams_content/workflow/basic.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/workflow/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/workflow/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/workflow/notify.py` & `pyams_content-1.99.3/src/pyams_content/workflow/notify.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/workflow/task.py` & `pyams_content-1.99.3/src/pyams_content/workflow/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from pyramid.events import subscriber
 from transaction.interfaces import ITransactionManager
 from zope.interface import implementer
 from zope.intid import IIntIds
 
 from pyams_content.workflow.interfaces import IWorkflowManagementTask
 from pyams_scheduler.interfaces import ISchedulerProcess, SCHEDULER_NAME
-from pyams_scheduler.interfaces.task import IDateTaskScheduling
+from pyams_scheduler.interfaces.task import IDateTaskScheduling, TASK_STATUS_OK
 from pyams_scheduler.process import TaskResettingThread
 from pyams_scheduler.task import Task
 from pyams_security.interfaces.names import INTERNAL_USER_ID
 from pyams_site.interfaces import PYAMS_APPLICATION_SETTINGS_KEY, PYAMS_APPLICATION_DEFAULT_NAME
 from pyams_utils.registry import get_pyramid_registry, get_utility
 from pyams_utils.timezone import gmtime
 from pyams_utils.zodb import ZODBConnection
@@ -75,14 +75,15 @@
                 info.fire_transition(self.transition_id,
                                      check_security=False,
                                      principal=self.principal_id)
                 info.fire_automatic()
         # remove task after execution!
         if self.__parent__ is not None:
             del self.__parent__[self.__name__]
+        return TASK_STATUS_OK, None
 
 
 @implementer(IWorkflowManagementTask)
 class ContentArchivingTask(Task):
     """Content archiving task"""
 
     label = _("Content archiver task")
@@ -110,14 +111,15 @@
                 info.fire_transition_toward(workflow.auto_retired_state,
                                             check_security=False,
                                             principal=self.principal_id)
                 info.fire_automatic()
         # remove task after execution!
         if self.__parent__ is not None:
             del self.__parent__[self.__name__]
+        return TASK_STATUS_OK, None
 
 
 @subscriber(IZMQProcessStartedEvent, context_selector=ISchedulerProcess)
 def handle_scheduler_start(event):
     """Check for scheduler tasks
 
     Workflow management tasks are typically automatically deleted after their execution.
```

### Comparing `pyams_content-1.99.2/src/pyams_content/workflow/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/workflow/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/workflow/zmi/publication.py` & `pyams_content-1.99.3/src/pyams_content/workflow/zmi/publication.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/workflow/zmi/task.py` & `pyams_content-1.99.3/src/pyams_content/workflow/zmi/task.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/__init__.py` & `pyams_content-1.99.3/src/pyams_content/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/dashboard.py` & `pyams_content-1.99.3/src/pyams_content/zmi/dashboard.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/html.py` & `pyams_content-1.99.3/src/pyams_content/zmi/html.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/properties.py` & `pyams_content-1.99.3/src/pyams_content/zmi/properties.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/resources/js/content.js` & `pyams_content-1.99.3/src/pyams_content/zmi/resources/js/content.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/resources/js/content.min.js` & `pyams_content-1.99.3/src/pyams_content/zmi/resources/js/content.min.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js` & `pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/headers/plugin.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js` & `pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/langs/fr.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js` & `pyams_content-1.99.3/src/pyams_content/zmi/resources/js/tinymce/internal-link/plugin.js`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/viewlet/__init__.py` & `pyams_content-1.99.3/src/pyams_content/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/viewlet/toplinks.py` & `pyams_content-1.99.3/src/pyams_content/zmi/viewlet/toplinks.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/widget/__init__.py` & `pyams_content-1.99.3/src/pyams_content/zmi/widget/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/widget/interfaces.py` & `pyams_content-1.99.3/src/pyams_content/zmi/widget/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/widget/seo.py` & `pyams_content-1.99.3/src/pyams_content/zmi/widget/seo.py`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content/zmi/widget/templates/seo-textline-input.pt` & `pyams_content-1.99.3/src/pyams_content/zmi/widget/templates/seo-textline-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content.egg-info/PKG-INFO` & `pyams_content-1.99.3/src/pyams_content.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-content
-Version: 1.99.2
+Version: 1.99.3
 Summary: PyAMS content management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS CMS
 Classifier: License :: OSI Approved :: Zope Public License
@@ -48,14 +48,21 @@
 Please note that PyAMS_content only provide a basic Bootstrap based skin, so you will have to
 include other extension packages (like PyAMS_content_themes) to get more advanced graphical themes.
 
 
 Changelog
 =========
 
+1.99.3
+------
+ - updated shared content header viewlet to add button to go back to dashboard
+ - added status to scheduler tasks execution result
+ - added support for direct content retiring or archiving for managers
+ - added support for custom modal content class
+
 1.99.2
 ------
  - added permission and role to manage references tables
  - disable cache when using aggregated search results portlet renderer
  - always open switcher in associations paragraph
  - added method to paragraphs container to get iterator over paragraphs matching a given set of factories
  - removed required flag on gallery files author
```

### Comparing `pyams_content-1.99.2/src/pyams_content.egg-info/SOURCES.txt` & `pyams_content-1.99.3/src/pyams_content.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyams_content-1.99.2/src/pyams_content.egg-info/requires.txt` & `pyams_content-1.99.3/src/pyams_content.egg-info/requires.txt`

 * *Files identical despite different names*

