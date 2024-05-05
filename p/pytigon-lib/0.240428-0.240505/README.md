# Comparing `tmp/pytigon-lib-0.240428.tar.gz` & `tmp/pytigon-lib-0.240505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytigon-lib-0.240428.tar", last modified: Sun Apr 28 17:10:54 2024, max compression
+gzip compressed data, was "pytigon-lib-0.240505.tar", last modified: Sun May  5 11:44:54 2024, max compression
```

## Comparing `pytigon-lib-0.240428.tar` & `pytigon-lib-0.240505.tar`

### file list

```diff
@@ -1,134 +1,133 @@
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.166505 pytigon-lib-0.240428/
--rw-rw-r--   0 sch       (1000) sch       (1000)     7633 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/LICENSE
--rw-r--r--   0 sch       (1000) sch       (1000)     1462 2024-04-28 17:10:54.166505 pytigon-lib-0.240428/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)       13 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/README.md
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.150504 pytigon-lib-0.240428/pytigon_lib/
--rw-rw-r--   0 sch       (1000) sch       (1000)     3328 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/__init__.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.150504 pytigon-lib-0.240428/pytigon_lib/schandroid/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schandroid/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     7772 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schandroid/android_client.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.154505 pytigon-lib-0.240428/pytigon_lib/schdjangoext/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      582 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/allauth.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1773 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/django_ihtml.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2062 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/django_init.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1223 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/django_manage.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      888 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/django_settings.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2902 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/email.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5442 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/fastform.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    12243 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/fields.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3381 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/formfields.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5543 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/formwidgets.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1665 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/graphql.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5181 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/import_from_db.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9842 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/models.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1550 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/oauth_for_graphql.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    16441 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/python_style_template_loader.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5248 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/render.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2523 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/rest_tools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4038 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/server.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     7421 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/spreadsheet_render.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2098 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/tools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      354 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schdjangoext/widgets.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.154505 pytigon-lib-0.240428/pytigon_lib/schfs/
--rw-rw-r--   0 sch       (1000) sch       (1000)      986 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schfs/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1632 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schfs/tasks.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    14885 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schfs/vfstools.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.154505 pytigon-lib-0.240428/pytigon_lib/schhtml/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    12942 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/atom.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    19894 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/basedc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    16635 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/basehtmltags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    12020 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/cairodc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     6237 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/css.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    13853 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/docxdc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2422 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/html_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2764 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/htmltools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    14974 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/htmlviewer.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.154505 pytigon-lib-0.240428/pytigon_lib/schhtml/icss/
--rw-rw-r--   0 sch       (1000) sch       (1000)     6965 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/icss/wiki.icss
--rw-rw-r--   0 sch       (1000) sch       (1000)     1197 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/main.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5643 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/parser.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    13716 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/pdfdc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    11680 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/render_helpers.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.158505 pytigon-lib-0.240428/pytigon_lib/schhtml/tags/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/tags/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9267 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/tags/atom_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    10781 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/tags/block_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1796 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/tags/css_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2563 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/tags/extra_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    15761 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/tags/p_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2533 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/tags/page_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    25539 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/tags/table_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    13671 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/wxdc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9959 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/wxgc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    13494 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhtml/xlsxdc.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.158505 pytigon-lib-0.240428/pytigon_lib/schhttptools/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhttptools/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4659 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhttptools/asgi_bridge.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      694 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhttptools/get_oauth2_refresh_token.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    21255 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhttptools/httpclient.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2224 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhttptools/rest_client.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2814 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schhttptools/websocket.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.158505 pytigon-lib-0.240428/pytigon_lib/schindent/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schindent/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8784 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schindent/indent_markdown.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    29927 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schindent/indent_style.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8288 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schindent/indent_tools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      890 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schindent/py_to_js.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.158505 pytigon-lib-0.240428/pytigon_lib/schparser/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schparser/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     6553 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schparser/html_parsers.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.158505 pytigon-lib-0.240428/pytigon_lib/schspreadsheet/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schspreadsheet/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    12631 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schspreadsheet/odf_process.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    19135 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schspreadsheet/ooxml_process.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3323 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schspreadsheet/ooxml_tools.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.162505 pytigon-lib-0.240428/pytigon_lib/schtable/
--rw-rw-r--   0 sch       (1000) sch       (1000)      733 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtable/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9070 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtable/dbtable.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5880 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtable/table.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    13468 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtable/vfstable.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.162505 pytigon-lib-0.240428/pytigon_lib/schtasks/
--rw-rw-r--   0 sch       (1000) sch       (1000)        0 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtasks/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3435 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtasks/publish.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2449 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtasks/remote_screen.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    14934 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtasks/schschedule.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1420 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtasks/term_tools.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.162505 pytigon-lib-0.240428/pytigon_lib/schtools/
--rw-rw-r--   0 sch       (1000) sch       (1000)      897 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5383 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/cc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2713 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/createparm.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1902 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/env.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    17019 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/href_action.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3153 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/images.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3304 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/imap4client.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    11029 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/install.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9761 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/install_init.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1262 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/llvm_exec.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8367 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/main_paths.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2359 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/nim_ext.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3081 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/nim_integration.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      991 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/platform_info.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4657 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/process.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2535 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/schhtmlgen.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2625 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/schjson.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3423 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/screenshot.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4495 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/tools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4031 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schtools/wiki.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.166505 pytigon-lib-0.240428/pytigon_lib/schviews/
--rw-rw-r--   0 sch       (1000) sch       (1000)    67765 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schviews/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3237 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schviews/actions.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     7824 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schviews/form_fun.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4005 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schviews/perms.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4416 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schviews/tree.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    22012 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/pytigon_lib/schviews/viewtools.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-04-28 17:10:54.166505 pytigon-lib-0.240428/pytigon_lib.egg-info/
--rw-r--r--   0 sch       (1000) sch       (1000)     1462 2024-04-28 17:10:54.000000 pytigon-lib-0.240428/pytigon_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)     3980 2024-04-28 17:10:54.000000 pytigon-lib-0.240428/pytigon_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-04-28 17:10:54.000000 pytigon-lib-0.240428/pytigon_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)      111 2024-04-28 17:10:54.000000 pytigon-lib-0.240428/pytigon_lib.egg-info/requires.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       12 2024-04-28 17:10:54.000000 pytigon-lib-0.240428/pytigon_lib.egg-info/top_level.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)      111 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/requirements.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       38 2024-04-28 17:10:54.166505 pytigon-lib-0.240428/setup.cfg
--rw-rw-r--   0 sch       (1000) sch       (1000)     2033 2024-04-28 17:09:17.000000 pytigon-lib-0.240428/setup.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.543712 pytigon-lib-0.240505/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7633 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/LICENSE
+-rw-r--r--   0 sch       (1000) sch       (1000)     1509 2024-05-05 11:44:54.543712 pytigon-lib-0.240505/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)       13 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/README.md
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.527712 pytigon-lib-0.240505/pytigon_lib/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3328 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/__init__.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.527712 pytigon-lib-0.240505/pytigon_lib/schandroid/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schandroid/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7772 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schandroid/android_client.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.531712 pytigon-lib-0.240505/pytigon_lib/schdjangoext/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      582 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/allauth.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1773 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/django_ihtml.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2062 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/django_init.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1223 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/django_manage.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      888 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/django_settings.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2902 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/email.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5442 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/fastform.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    12243 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/fields.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3381 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/formfields.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5543 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/formwidgets.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1665 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/graphql.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5181 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/import_from_db.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9842 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/models.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1550 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/oauth_for_graphql.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    16441 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/python_style_template_loader.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5248 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/render.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2523 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/rest_tools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4038 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/server.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7421 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/spreadsheet_render.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2098 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/tools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      354 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schdjangoext/widgets.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.531712 pytigon-lib-0.240505/pytigon_lib/schfs/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      986 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schfs/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1632 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schfs/tasks.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    14885 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schfs/vfstools.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.531712 pytigon-lib-0.240505/pytigon_lib/schhtml/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    12942 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/atom.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    19894 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/basedc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    16635 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/basehtmltags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    12020 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/cairodc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6237 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/css.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    13853 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/docxdc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2422 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/html_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2764 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/htmltools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    14974 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/htmlviewer.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.531712 pytigon-lib-0.240505/pytigon_lib/schhtml/icss/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6965 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/icss/wiki.icss
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1197 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/main.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5643 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/parser.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    13716 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/pdfdc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    11680 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/render_helpers.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.535712 pytigon-lib-0.240505/pytigon_lib/schhtml/tags/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/tags/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9267 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/tags/atom_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    10781 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/tags/block_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1796 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/tags/css_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2563 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/tags/extra_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    15761 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/tags/p_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2533 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/tags/page_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    25539 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/tags/table_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    13671 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/wxdc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9959 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/wxgc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    13494 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhtml/xlsxdc.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.535712 pytigon-lib-0.240505/pytigon_lib/schhttptools/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhttptools/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4659 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhttptools/asgi_bridge.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      694 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhttptools/get_oauth2_refresh_token.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    21255 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhttptools/httpclient.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2224 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhttptools/rest_client.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2814 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schhttptools/websocket.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.535712 pytigon-lib-0.240505/pytigon_lib/schindent/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schindent/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8784 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schindent/indent_markdown.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    29927 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schindent/indent_style.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8288 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schindent/indent_tools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      890 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schindent/py_to_js.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.535712 pytigon-lib-0.240505/pytigon_lib/schparser/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schparser/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6553 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schparser/html_parsers.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.535712 pytigon-lib-0.240505/pytigon_lib/schspreadsheet/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schspreadsheet/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    12631 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schspreadsheet/odf_process.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    19135 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schspreadsheet/ooxml_process.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3323 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schspreadsheet/ooxml_tools.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.535712 pytigon-lib-0.240505/pytigon_lib/schtable/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      733 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtable/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9070 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtable/dbtable.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5880 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtable/table.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    13468 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtable/vfstable.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.539712 pytigon-lib-0.240505/pytigon_lib/schtasks/
+-rw-rw-r--   0 sch       (1000) sch       (1000)        0 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtasks/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3435 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtasks/publish.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2449 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtasks/remote_screen.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    14934 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtasks/schschedule.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1420 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtasks/term_tools.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.539712 pytigon-lib-0.240505/pytigon_lib/schtools/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      897 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2713 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/createparm.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1902 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/env.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    17019 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/href_action.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3153 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/images.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3304 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/imap4client.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    10970 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/install.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9720 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/install_init.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1262 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/llvm_exec.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8367 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/main_paths.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2359 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/nim_ext.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3097 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/nim_integration.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      991 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/platform_info.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4678 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/process.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2535 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/schhtmlgen.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2625 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/schjson.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3423 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/screenshot.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4495 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/tools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4031 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schtools/wiki.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.543712 pytigon-lib-0.240505/pytigon_lib/schviews/
+-rw-rw-r--   0 sch       (1000) sch       (1000)    67765 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schviews/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3237 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schviews/actions.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7824 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schviews/form_fun.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4005 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schviews/perms.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4416 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schviews/tree.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    22012 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/pytigon_lib/schviews/viewtools.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2024-05-05 11:44:54.543712 pytigon-lib-0.240505/pytigon_lib.egg-info/
+-rw-r--r--   0 sch       (1000) sch       (1000)     1509 2024-05-05 11:44:54.000000 pytigon-lib-0.240505/pytigon_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3953 2024-05-05 11:44:54.000000 pytigon-lib-0.240505/pytigon_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)        1 2024-05-05 11:44:54.000000 pytigon-lib-0.240505/pytigon_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)      128 2024-05-05 11:44:54.000000 pytigon-lib-0.240505/pytigon_lib.egg-info/requires.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       12 2024-05-05 11:44:54.000000 pytigon-lib-0.240505/pytigon_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)      128 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/requirements.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       38 2024-05-05 11:44:54.543712 pytigon-lib-0.240505/setup.cfg
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2043 2024-05-05 11:43:53.000000 pytigon-lib-0.240505/setup.py
```

### Comparing `pytigon-lib-0.240428/LICENSE` & `pytigon-lib-0.240505/LICENSE`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/PKG-INFO` & `pytigon-lib-0.240505/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-lib
-Version: 0.240428
+Version: 0.240505
 Summary: Pytigon library
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -32,7 +32,9 @@
 Requires-Dist: django-environ
 Requires-Dist: pyexcel
 Requires-Dist: pyexcel-xlsx
 Requires-Dist: pyexcel-ods3
 Requires-Dist: python-docx
 Requires-Dist: fpdf2
 Requires-Dist: python-dateutil
+Requires-Dist: markdown
+Requires-Dist: pyquery
```

### Comparing `pytigon-lib-0.240428/pytigon_lib/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schandroid/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schandroid/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schandroid/android_client.py` & `pytigon-lib-0.240505/pytigon_lib/schandroid/android_client.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/allauth.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/allauth.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/django_ihtml.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/django_ihtml.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/django_init.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/django_init.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/django_manage.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/django_manage.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/django_settings.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/django_settings.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/email.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/email.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/fastform.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/fastform.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/fields.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/fields.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/formfields.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/formfields.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/formwidgets.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/formwidgets.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/graphql.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/graphql.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/import_from_db.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/import_from_db.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/models.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/models.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/oauth_for_graphql.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/oauth_for_graphql.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/python_style_template_loader.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/python_style_template_loader.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/render.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/render.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/rest_tools.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/rest_tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/server.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/server.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/spreadsheet_render.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/spreadsheet_render.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schdjangoext/tools.py` & `pytigon-lib-0.240505/pytigon_lib/schdjangoext/tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schfs/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schfs/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schfs/tasks.py` & `pytigon-lib-0.240505/pytigon_lib/schfs/tasks.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schfs/vfstools.py` & `pytigon-lib-0.240505/pytigon_lib/schfs/vfstools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/atom.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/atom.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/basedc.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/basedc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/basehtmltags.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/basehtmltags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/cairodc.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/cairodc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/css.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/css.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/docxdc.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/docxdc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/html_tags.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/html_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/htmltools.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/htmltools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/htmlviewer.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/htmlviewer.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/icss/wiki.icss` & `pytigon-lib-0.240505/pytigon_lib/schhtml/icss/wiki.icss`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/main.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/main.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/parser.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/parser.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/pdfdc.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/pdfdc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/render_helpers.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/render_helpers.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/tags/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/tags/atom_tags.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/tags/atom_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/tags/block_tags.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/tags/block_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/tags/css_tags.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/tags/css_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/tags/extra_tags.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/tags/extra_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/tags/p_tags.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/tags/p_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/tags/page_tags.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/tags/page_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/tags/table_tags.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/tags/table_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/wxdc.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/wxdc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/wxgc.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/wxgc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhtml/xlsxdc.py` & `pytigon-lib-0.240505/pytigon_lib/schhtml/xlsxdc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhttptools/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schhttptools/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhttptools/asgi_bridge.py` & `pytigon-lib-0.240505/pytigon_lib/schhttptools/asgi_bridge.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhttptools/get_oauth2_refresh_token.py` & `pytigon-lib-0.240505/pytigon_lib/schhttptools/get_oauth2_refresh_token.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhttptools/httpclient.py` & `pytigon-lib-0.240505/pytigon_lib/schhttptools/httpclient.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhttptools/rest_client.py` & `pytigon-lib-0.240505/pytigon_lib/schhttptools/rest_client.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schhttptools/websocket.py` & `pytigon-lib-0.240505/pytigon_lib/schhttptools/websocket.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schindent/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schindent/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schindent/indent_markdown.py` & `pytigon-lib-0.240505/pytigon_lib/schindent/indent_markdown.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schindent/indent_style.py` & `pytigon-lib-0.240505/pytigon_lib/schindent/indent_style.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schindent/indent_tools.py` & `pytigon-lib-0.240505/pytigon_lib/schindent/indent_tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schindent/py_to_js.py` & `pytigon-lib-0.240505/pytigon_lib/schindent/py_to_js.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schparser/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schparser/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schparser/html_parsers.py` & `pytigon-lib-0.240505/pytigon_lib/schparser/html_parsers.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schspreadsheet/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schspreadsheet/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schspreadsheet/odf_process.py` & `pytigon-lib-0.240505/pytigon_lib/schspreadsheet/odf_process.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schspreadsheet/ooxml_process.py` & `pytigon-lib-0.240505/pytigon_lib/schspreadsheet/ooxml_process.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schspreadsheet/ooxml_tools.py` & `pytigon-lib-0.240505/pytigon_lib/schspreadsheet/ooxml_tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtable/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schtable/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtable/dbtable.py` & `pytigon-lib-0.240505/pytigon_lib/schtable/dbtable.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtable/table.py` & `pytigon-lib-0.240505/pytigon_lib/schtable/table.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtable/vfstable.py` & `pytigon-lib-0.240505/pytigon_lib/schtable/vfstable.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtasks/publish.py` & `pytigon-lib-0.240505/pytigon_lib/schtasks/publish.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtasks/remote_screen.py` & `pytigon-lib-0.240505/pytigon_lib/schtasks/remote_screen.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtasks/schschedule.py` & `pytigon-lib-0.240505/pytigon_lib/schtasks/schschedule.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtasks/term_tools.py` & `pytigon-lib-0.240505/pytigon_lib/schtasks/term_tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/createparm.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/createparm.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/env.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/env.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/href_action.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/href_action.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/images.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/images.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/imap4client.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/imap4client.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/install.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/install.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,18 @@
 # copyright: "Copyright (C) ????/2012 Slawomir Cholaj"
 # license: "LGPL 3.0"
 # version: "0.1a"
 
 import datetime
 import zipfile
 import io
-from shutil import move
 
 from pytigon_lib.schdjangoext.django_manage import *
 from pytigon_lib.schfs.vfstools import extractall
 from pytigon_lib.schtools.process import py_run
-from pytigon_lib.schtools.cc import make
 from pytigon_lib.schtools.main_paths import get_prj_name
 
 
 def install():
     os.environ.setdefault("DJANGO_SETTINGS_MODULE", "settings_app")
     from django.conf import settings
 
@@ -105,18 +103,18 @@
             cmd(["loaddata", "--database", "default", json_path, "--traceback"])
             from django.contrib.auth.models import User
 
             User.objects.db_manager("default").create_superuser(
                 "auto", "auto@pytigon.com", "anawa"
             )
 
-    ret = make(data_path, prj_path, prj_name)
-    if ret:
-        for pos in ret:
-            print(pos)
+    # ret = make(data_path, prj_path, prj_name)
+    # if ret:
+    #    for pos in ret:
+    #        print(pos)
 
 
 def export_to_db(withoutapp=None, to_local_db=True):
     os.environ.setdefault("DJANGO_SETTINGS_MODULE", "settings_app")
     from django.conf import settings
 
     if "local" in settings.DATABASES:
```

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/install_init.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/install_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import sys
 import zipfile
 import shutil
 import configparser
 import multiprocessing
 from pytigon_lib.schfs import extractall
 from pytigon_lib.schtools.process import py_manage
-from pytigon_lib.schtools.cc import make
 from pytigon_lib.schtools.process import py_run
 from pytigon_lib.schtools.nim_integration import install_nim
 
 
 def _mkdir(path, ext=None):
     if ext:
         p = os.path.join(path, ext)
```

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/llvm_exec.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/llvm_exec.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/main_paths.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/main_paths.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/nim_ext.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/nim_ext.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/nim_integration.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/nim_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             nim_path, "bin", "zigcc.exe" if os.name == "nt" else "zigcc"
         )
         zigcc_c = os.path.join(temp_dir, "zigcc.c")
         with open(zigcc_c, "wt") as f:
             f.write(ZIG_CC_C)
 
         exit_code, output_tab, err_tab = run(
-            ["ptig", "zig", "cc", "-o", zigcc_bin, zigcc_c]
+            ["ptig", "zig", "cc", "-o", zigcc_bin, zigcc_c], env=os.environ
         )
         if err_tab:
             print(err_tab)
 
         if os.name != "nt":
             st = os.stat(zigcc_bin)
             os.chmod(zigcc_bin, st.st_mode | stat.S_IEXEC)
```

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/platform_info.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/platform_info.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/process.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,29 +56,29 @@
         for module in to_delete:
             del sys.modules[module]
 
         for pos in self.to_restore:
             sys.modules[pos] = self.to_restore[pos]
 
 
-def run(cmd, shell=True):
+def run(cmd, shell=False, env=False):
     """run extern command
 
     args:
         cmd - array of parameters
 
     returns:
         array:
             return code,
             return stdout data
             return stderr data
     example:
         run(["ls" "-la",])
     """
-    process = Popen(cmd, stdout=PIPE, stderr=PIPE, shell=shell)
+    process = Popen(cmd, stdout=PIPE, stderr=PIPE, shell=shell, env=env)
     (output, err) = process.communicate()
     exit_code = process.wait()
     if output:
         if type(output) != str:
             s = output.decode("utf-8")
         else:
             s = output
```

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/schhtmlgen.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/schhtmlgen.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/schjson.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/schjson.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/screenshot.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/screenshot.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/tools.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schtools/wiki.py` & `pytigon-lib-0.240505/pytigon_lib/schtools/wiki.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schviews/__init__.py` & `pytigon-lib-0.240505/pytigon_lib/schviews/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schviews/actions.py` & `pytigon-lib-0.240505/pytigon_lib/schviews/actions.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schviews/form_fun.py` & `pytigon-lib-0.240505/pytigon_lib/schviews/form_fun.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schviews/perms.py` & `pytigon-lib-0.240505/pytigon_lib/schviews/perms.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schviews/tree.py` & `pytigon-lib-0.240505/pytigon_lib/schviews/tree.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib/schviews/viewtools.py` & `pytigon-lib-0.240505/pytigon_lib/schviews/viewtools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.240428/pytigon_lib.egg-info/PKG-INFO` & `pytigon-lib-0.240505/pytigon_lib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-lib
-Version: 0.240428
+Version: 0.240505
 Summary: Pytigon library
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -32,7 +32,9 @@
 Requires-Dist: django-environ
 Requires-Dist: pyexcel
 Requires-Dist: pyexcel-xlsx
 Requires-Dist: pyexcel-ods3
 Requires-Dist: python-docx
 Requires-Dist: fpdf2
 Requires-Dist: python-dateutil
+Requires-Dist: markdown
+Requires-Dist: pyquery
```

### Comparing `pytigon-lib-0.240428/pytigon_lib.egg-info/SOURCES.txt` & `pytigon-lib-0.240505/pytigon_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 pytigon_lib/schtable/vfstable.py
 pytigon_lib/schtasks/__init__.py
 pytigon_lib/schtasks/publish.py
 pytigon_lib/schtasks/remote_screen.py
 pytigon_lib/schtasks/schschedule.py
 pytigon_lib/schtasks/term_tools.py
 pytigon_lib/schtools/__init__.py
-pytigon_lib/schtools/cc.py
 pytigon_lib/schtools/createparm.py
 pytigon_lib/schtools/env.py
 pytigon_lib/schtools/href_action.py
 pytigon_lib/schtools/images.py
 pytigon_lib/schtools/imap4client.py
 pytigon_lib/schtools/install.py
 pytigon_lib/schtools/install_init.py
```

### Comparing `pytigon-lib-0.240428/setup.py` & `pytigon-lib-0.240505/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from setuptools import setup, find_packages
+import os
 
 
 def package_files(directory, ext=None):
     paths = []
     for path, directories, filenames in os.walk(directory):
         for filename in filenames:
             if not ext or (ext and filename.endswith(ext)):
@@ -15,15 +16,15 @@
 with open("requirements.txt") as f:
     tmp = f.read().strip().split("\n")
     install_requires = [pos for pos in tmp if "://" not in pos]
     dependency_links = [pos for pos in tmp if "://" in pos]
 
 setup(
     name="pytigon-lib",
-    version="0.240428",
+    version="0.240505",
     description="Pytigon library",
     author="Sławomir Chołaj",
     author_email="slawomir.cholaj@gmail.com",
     license="LGPLv3",
     packages=find_packages(),
     package_data={
         "": extra_files,
```

