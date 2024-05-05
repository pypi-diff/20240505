# Comparing `tmp/limnoria-2023.9.24.tar.gz` & `tmp/limnoria-2024.4.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limnoria-2023.9.24.tar", last modified: Sun Sep 24 18:07:21 2023, max compression
+gzip compressed data, was "limnoria-2024.4.26.tar", last modified: Sun May  5 15:43:06 2024, max compression
```

## Comparing `limnoria-2023.9.24.tar` & `limnoria-2024.4.26.tar`

### file list

```diff
@@ -1,767 +1,767 @@
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.031319 limnoria-2023.9.24/
--rw-r--r--   0 val       (1000) val       (1000)     1654 2023-09-24 17:43:59.000000 limnoria-2023.9.24/LICENSE.md
--rw-r--r--   0 val       (1000) val       (1000)      117 2023-09-24 17:43:59.000000 limnoria-2023.9.24/MANIFEST.in
--rw-r--r--   0 val       (1000) val       (1000)      983 2023-09-24 17:43:59.000000 limnoria-2023.9.24/Makefile
--rw-r--r--   0 val       (1000) val       (1000)     1848 2023-09-24 18:07:21.031319 limnoria-2023.9.24/PKG-INFO
--rw-r--r--   0 val       (1000) val       (1000)     2292 2023-09-24 17:43:59.000000 limnoria-2023.9.24/README.md
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.983319 limnoria-2023.9.24/limnoria.egg-info/
--rw-r--r--   0 val       (1000) val       (1000)     1848 2023-09-24 18:07:20.000000 limnoria-2023.9.24/limnoria.egg-info/PKG-INFO
--rw-r--r--   0 val       (1000) val       (1000)    16256 2023-09-24 18:07:20.000000 limnoria-2023.9.24/limnoria.egg-info/SOURCES.txt
--rw-r--r--   0 val       (1000) val       (1000)        1 2023-09-24 18:07:20.000000 limnoria-2023.9.24/limnoria.egg-info/dependency_links.txt
--rw-r--r--   0 val       (1000) val       (1000)      934 2023-09-24 18:07:20.000000 limnoria-2023.9.24/limnoria.egg-info/entry_points.txt
--rw-r--r--   0 val       (1000) val       (1000)        8 2023-09-24 18:07:20.000000 limnoria-2023.9.24/limnoria.egg-info/top_level.txt
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.987320 limnoria-2023.9.24/locales/
--rw-r--r--   0 val       (1000) val       (1000)        0 2023-09-24 17:43:59.000000 limnoria-2023.9.24/locales/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    54113 2023-09-24 17:43:59.000000 limnoria-2023.9.24/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    76337 2023-09-24 17:43:59.000000 limnoria-2023.9.24/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    77441 2023-09-24 17:43:59.000000 limnoria-2023.9.24/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3749 2023-09-24 17:43:59.000000 limnoria-2023.9.24/locales/fr.py
--rw-r--r--   0 val       (1000) val       (1000)    69991 2023-09-24 17:43:59.000000 limnoria-2023.9.24/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    42399 2023-09-24 17:43:59.000000 limnoria-2023.9.24/locales/messages.pot
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.987320 limnoria-2023.9.24/man/
--rw-r--r--   0 val       (1000) val       (1000)     1196 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/limnoria-adduser.1
--rw-r--r--   0 val       (1000) val       (1000)     1487 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/limnoria-botchk.1
--rw-r--r--   0 val       (1000) val       (1000)     1125 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/limnoria-plugin-create.1
--rw-r--r--   0 val       (1000) val       (1000)     1378 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/limnoria-plugin-doc.1
--rw-r--r--   0 val       (1000) val       (1000)     1026 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/limnoria-reset-password.1
--rw-r--r--   0 val       (1000) val       (1000)     1499 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/limnoria-test.1
--rw-r--r--   0 val       (1000) val       (1000)     1191 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/limnoria-wizard.1
--rw-r--r--   0 val       (1000) val       (1000)     1970 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/limnoria.1
--rw-r--r--   0 val       (1000) val       (1000)     1196 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/supybot-adduser.1
--rw-r--r--   0 val       (1000) val       (1000)     1487 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/supybot-botchk.1
--rw-r--r--   0 val       (1000) val       (1000)     1125 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/supybot-plugin-create.1
--rw-r--r--   0 val       (1000) val       (1000)     1378 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/supybot-plugin-doc.1
--rw-r--r--   0 val       (1000) val       (1000)     1026 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/supybot-reset-password.1
--rw-r--r--   0 val       (1000) val       (1000)     1499 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/supybot-test.1
--rw-r--r--   0 val       (1000) val       (1000)     1191 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/supybot-wizard.1
--rw-r--r--   0 val       (1000) val       (1000)     1970 2023-09-24 17:43:59.000000 limnoria-2023.9.24/man/supybot.1
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.987320 limnoria-2023.9.24/plugins/
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.987320 limnoria-2023.9.24/plugins/Admin/
--rw-r--r--   0 val       (1000) val       (1000)     2422 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Admin/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2312 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Admin/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.987320 limnoria-2023.9.24/plugins/Admin/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8064 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Admin/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     8857 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Admin/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7809 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Admin/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     8112 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Admin/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    15152 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Admin/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5897 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Admin/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.987320 limnoria-2023.9.24/plugins/Aka/
--rw-r--r--   0 val       (1000) val       (1000)     2788 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Aka/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2979 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Aka/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.987320 limnoria-2023.9.24/plugins/Aka/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11022 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Aka/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    39586 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Aka/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    14785 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Aka/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.987320 limnoria-2023.9.24/plugins/Alias/
--rw-r--r--   0 val       (1000) val       (1000)     2655 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Alias/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2539 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Alias/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.987320 limnoria-2023.9.24/plugins/Alias/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4716 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Alias/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5751 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Alias/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5059 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Alias/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5176 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Alias/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     4919 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Alias/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    19130 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Alias/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     8039 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Alias/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.987320 limnoria-2023.9.24/plugins/Anonymous/
--rw-r--r--   0 val       (1000) val       (1000)     2528 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Anonymous/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3516 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Anonymous/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/Anonymous/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6558 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Anonymous/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     7384 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Anonymous/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5903 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Anonymous/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6893 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Anonymous/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     6535 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Anonymous/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9054 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Anonymous/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6882 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Anonymous/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/AutoMode/
--rw-r--r--   0 val       (1000) val       (1000)     2697 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/AutoMode/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4521 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/AutoMode/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/AutoMode/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4202 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/AutoMode/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5058 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/AutoMode/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4512 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/AutoMode/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4131 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/AutoMode/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     8029 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/AutoMode/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1787 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/AutoMode/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/Autocomplete/
--rw-r--r--   0 val       (1000) val       (1000)     2946 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Autocomplete/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2808 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Autocomplete/config.py
--rw-r--r--   0 val       (1000) val       (1000)     6158 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Autocomplete/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6635 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Autocomplete/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/BadWords/
--rw-r--r--   0 val       (1000) val       (1000)     2695 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/BadWords/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     6163 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/BadWords/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/BadWords/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6862 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/BadWords/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6112 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/BadWords/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6277 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/BadWords/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7475 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/BadWords/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3943 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/BadWords/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/Channel/
--rw-r--r--   0 val       (1000) val       (1000)     2480 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Channel/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3497 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Channel/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/Channel/locales/
--rw-r--r--   0 val       (1000) val       (1000)    32456 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Channel/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    35277 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Channel/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    32166 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Channel/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    32899 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Channel/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    33333 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Channel/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    44412 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Channel/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    13344 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Channel/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/ChannelLogger/
--rw-r--r--   0 val       (1000) val       (1000)     2531 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelLogger/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5994 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelLogger/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/ChannelLogger/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5491 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelLogger/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5340 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelLogger/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5607 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelLogger/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     5183 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelLogger/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    13745 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelLogger/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9242 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelLogger/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/ChannelStats/
--rw-r--r--   0 val       (1000) val       (1000)     2682 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelStats/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3449 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelStats/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/ChannelStats/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6426 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelStats/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6640 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelStats/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6242 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelStats/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    15391 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelStats/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4870 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ChannelStats/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.991320 limnoria-2023.9.24/plugins/Conditional/
--rw-r--r--   0 val       (1000) val       (1000)     2907 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Conditional/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2763 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Conditional/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Conditional/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8160 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Conditional/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7180 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Conditional/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7493 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Conditional/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    11342 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Conditional/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6497 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Conditional/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Config/
--rw-r--r--   0 val       (1000) val       (1000)     2325 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Config/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2528 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Config/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Config/locales/
--rw-r--r--   0 val       (1000) val       (1000)     9209 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Config/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     9329 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Config/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     9333 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Config/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     9333 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Config/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     9265 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Config/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    21747 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Config/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    25531 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Config/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Ctcp/
--rw-r--r--   0 val       (1000) val       (1000)     2420 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Ctcp/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3652 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Ctcp/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Ctcp/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2084 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Ctcp/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     2196 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Ctcp/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2072 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Ctcp/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2073 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Ctcp/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     1911 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Ctcp/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7136 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Ctcp/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1785 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Ctcp/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/DDG/
--rw-r--r--   0 val       (1000) val       (1000)     2670 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/DDG/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3332 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/DDG/config.py
--rw-r--r--   0 val       (1000) val       (1000)     6037 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/DDG/parser.py
--rw-r--r--   0 val       (1000) val       (1000)     6988 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/DDG/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2389 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/DDG/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Debug/
--rw-r--r--   0 val       (1000) val       (1000)     2377 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Debug/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2399 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Debug/config.py
--rw-r--r--   0 val       (1000) val       (1000)     7272 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Debug/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2648 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Debug/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Dict/
--rw-r--r--   0 val       (1000) val       (1000)     2559 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dict/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2877 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dict/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Dict/local/
--rw-r--r--   0 val       (1000) val       (1000)       58 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dict/local/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    12308 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dict/local/dictclient.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Dict/locales/
--rw-r--r--   0 val       (1000) val       (1000)     3731 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dict/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     3433 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dict/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3365 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dict/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     6458 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dict/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2548 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dict/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Dunno/
--rw-r--r--   0 val       (1000) val       (1000)     2817 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dunno/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2511 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dunno/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Dunno/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1414 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dunno/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     1637 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dunno/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1557 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dunno/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1441 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dunno/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3095 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dunno/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3446 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Dunno/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Factoids/
--rw-r--r--   0 val       (1000) val       (1000)     2738 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Factoids/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4867 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Factoids/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.995319 limnoria-2023.9.24/plugins/Factoids/locales/
--rw-r--r--   0 val       (1000) val       (1000)    14672 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Factoids/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    14207 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Factoids/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    13986 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Factoids/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    37539 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Factoids/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    10544 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Factoids/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/Fediverse/
--rw-r--r--   0 val       (1000) val       (1000)     2506 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Fediverse/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     9206 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Fediverse/activitypub.py
--rw-r--r--   0 val       (1000) val       (1000)     3583 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Fediverse/config.py
--rw-r--r--   0 val       (1000) val       (1000)    16631 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Fediverse/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    21650 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Fediverse/test.py
--rw-r--r--   0 val       (1000) val       (1000)    21570 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Fediverse/test_data.py
--rw-r--r--   0 val       (1000) val       (1000)     2553 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Fediverse/utils.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/Filter/
--rw-r--r--   0 val       (1000) val       (1000)     2691 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Filter/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3118 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Filter/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/Filter/locales/
--rw-r--r--   0 val       (1000) val       (1000)    14523 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Filter/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    13736 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Filter/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    14301 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Filter/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    27294 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Filter/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     7848 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Filter/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/Format/
--rw-r--r--   0 val       (1000) val       (1000)     2559 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Format/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2522 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Format/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/Format/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6742 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Format/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5998 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Format/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6115 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Format/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7452 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Format/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4078 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Format/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/GPG/
--rw-r--r--   0 val       (1000) val       (1000)     2606 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/GPG/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2996 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/GPG/config.py
--rw-r--r--   0 val       (1000) val       (1000)     9566 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/GPG/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5817 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/GPG/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/Games/
--rw-r--r--   0 val       (1000) val       (1000)     2660 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Games/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2313 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Games/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/Games/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4801 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Games/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5274 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Games/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4968 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Games/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4732 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Games/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7248 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Games/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2854 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Games/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/Geography/
--rw-r--r--   0 val       (1000) val       (1000)     2578 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Geography/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     1936 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Geography/common.py
--rw-r--r--   0 val       (1000) val       (1000)     2441 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Geography/config.py
--rw-r--r--   0 val       (1000) val       (1000)     2924 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Geography/nominatim.py
--rw-r--r--   0 val       (1000) val       (1000)     6528 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Geography/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    10102 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Geography/test.py
--rw-r--r--   0 val       (1000) val       (1000)     5422 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Geography/wikidata.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/Google/
--rw-r--r--   0 val       (1000) val       (1000)     2507 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Google/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     7042 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Google/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:20.999319 limnoria-2023.9.24/plugins/Google/locales/
--rw-r--r--   0 val       (1000) val       (1000)     9595 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Google/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     9003 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Google/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     9000 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Google/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     4460 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Google/parser.py
--rw-r--r--   0 val       (1000) val       (1000)    11693 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Google/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3095 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Google/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Hashes/
--rw-r--r--   0 val       (1000) val       (1000)     2585 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Hashes/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2244 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Hashes/config.py
--rw-r--r--   0 val       (1000) val       (1000)     4049 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Hashes/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2754 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Hashes/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Herald/
--rw-r--r--   0 val       (1000) val       (1000)     2423 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Herald/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3907 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Herald/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Herald/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7333 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Herald/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6711 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Herald/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6615 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Herald/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10794 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Herald/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1789 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Herald/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Internet/
--rw-r--r--   0 val       (1000) val       (1000)     2676 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Internet/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Internet/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Internet/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2313 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Internet/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1791 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Internet/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1769 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Internet/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     8887 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Internet/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2420 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Internet/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Karma/
--rw-r--r--   0 val       (1000) val       (1000)     2540 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Karma/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3929 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Karma/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Karma/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7837 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Karma/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7070 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Karma/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7143 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Karma/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    18303 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Karma/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9962 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Karma/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Lart/
--rw-r--r--   0 val       (1000) val       (1000)     2571 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Lart/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2679 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Lart/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Lart/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2427 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Lart/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2027 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Lart/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1956 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Lart/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     4264 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Lart/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2583 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Lart/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Later/
--rw-r--r--   0 val       (1000) val       (1000)     2650 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Later/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3413 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Later/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Later/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7371 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Later/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     7908 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Later/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6739 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Later/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7370 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Later/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    11043 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Later/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6360 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Later/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Limiter/
--rw-r--r--   0 val       (1000) val       (1000)     2662 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Limiter/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3141 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Limiter/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Limiter/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2685 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Limiter/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2688 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Limiter/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2724 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Limiter/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     2573 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Limiter/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3657 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Limiter/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2871 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Limiter/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/LogToIrc/
--rw-r--r--   0 val       (1000) val       (1000)     2457 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/LogToIrc/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5627 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/LogToIrc/config.py
--rw-r--r--   0 val       (1000) val       (1000)     6213 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/LogToIrc/handler.py
--rw-r--r--   0 val       (1000) val       (1000)     2710 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/LogToIrc/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1781 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/LogToIrc/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Math/
--rw-r--r--   0 val       (1000) val       (1000)     2528 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Math/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2516 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Math/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.003319 limnoria-2023.9.24/plugins/Math/local/
--rw-r--r--   0 val       (1000) val       (1000)       58 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Math/local/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    46378 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Math/local/convertcore.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/Math/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5920 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Math/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5424 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Math/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5331 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Math/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     5325 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Math/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    11324 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Math/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9441 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Math/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/MessageParser/
--rw-r--r--   0 val       (1000) val       (1000)     3026 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MessageParser/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4464 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MessageParser/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/MessageParser/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11282 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MessageParser/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    10121 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MessageParser/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    10440 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MessageParser/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    20338 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MessageParser/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    11746 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MessageParser/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/Misc/
--rw-r--r--   0 val       (1000) val       (1000)     2299 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Misc/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4131 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Misc/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/Misc/locales/
--rw-r--r--   0 val       (1000) val       (1000)    13201 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Misc/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    14554 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Misc/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    13747 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Misc/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    13209 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Misc/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    13537 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Misc/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    29646 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Misc/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    17530 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Misc/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/MoobotFactoids/
--rw-r--r--   0 val       (1000) val       (1000)     2648 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MoobotFactoids/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2740 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MoobotFactoids/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/MoobotFactoids/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11225 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MoobotFactoids/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    10014 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MoobotFactoids/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    10059 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MoobotFactoids/locales/it.po
--rwxr-xr-x   0 val       (1000) val       (1000)    29418 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MoobotFactoids/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    16971 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/MoobotFactoids/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/Network/
--rw-r--r--   0 val       (1000) val       (1000)     2514 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Network/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2528 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Network/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/Network/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7181 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Network/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     8612 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Network/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7289 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Network/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7472 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Network/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    12972 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Network/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3097 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Network/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/News/
--rw-r--r--   0 val       (1000) val       (1000)     2777 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/News/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2519 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/News/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/News/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4608 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/News/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4221 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/News/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4314 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/News/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     8659 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/News/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3616 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/News/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/NickAuth/
--rw-r--r--   0 val       (1000) val       (1000)     2574 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickAuth/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2495 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickAuth/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.007319 limnoria-2023.9.24/plugins/NickAuth/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4837 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickAuth/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     4838 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickAuth/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     9213 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickAuth/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6306 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickAuth/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/NickCapture/
--rw-r--r--   0 val       (1000) val       (1000)     2582 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickCapture/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2738 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickCapture/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/NickCapture/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1598 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickCapture/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     1716 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickCapture/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1592 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickCapture/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1500 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickCapture/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     5415 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickCapture/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1799 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/NickCapture/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/Nickometer/
--rw-r--r--   0 val       (1000) val       (1000)     3249 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Nickometer/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2616 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Nickometer/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/Nickometer/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1338 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Nickometer/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1027 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Nickometer/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)      952 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Nickometer/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9695 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Nickometer/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2183 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Nickometer/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/Note/
--rw-r--r--   0 val       (1000) val       (1000)     2645 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Note/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3477 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Note/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/Note/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4033 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Note/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     3453 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Note/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3399 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Note/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    16493 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Note/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4040 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Note/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/Owner/
--rw-r--r--   0 val       (1000) val       (1000)     2427 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Owner/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3252 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Owner/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/Owner/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8724 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Owner/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5600 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Owner/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     8546 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Owner/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     9038 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Owner/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     8811 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Owner/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    33701 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Owner/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9690 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Owner/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/Plugin/
--rw-r--r--   0 val       (1000) val       (1000)     2666 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Plugin/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2523 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Plugin/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/Plugin/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7234 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Plugin/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     7937 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Plugin/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6377 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Plugin/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7290 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Plugin/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9985 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Plugin/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4272 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Plugin/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/PluginDownloader/
--rw-r--r--   0 val       (1000) val       (1000)     2670 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/PluginDownloader/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2535 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/PluginDownloader/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/PluginDownloader/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4570 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/PluginDownloader/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6726 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/PluginDownloader/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6327 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/PluginDownloader/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5727 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/PluginDownloader/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    16307 2023-09-24 18:07:10.000000 limnoria-2023.9.24/plugins/PluginDownloader/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3847 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/PluginDownloader/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.011319 limnoria-2023.9.24/plugins/Poll/
--rw-r--r--   0 val       (1000) val       (1000)     2516 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Poll/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2922 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Poll/config.py
--rw-r--r--   0 val       (1000) val       (1000)     8542 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Poll/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6858 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Poll/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/Praise/
--rw-r--r--   0 val       (1000) val       (1000)     2528 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Praise/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2695 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Praise/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/Praise/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2548 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Praise/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2424 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Praise/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2352 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Praise/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     4348 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Praise/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1953 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Praise/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/Protector/
--rw-r--r--   0 val       (1000) val       (1000)     2594 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Protector/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2901 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Protector/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/Protector/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1626 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Protector/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1245 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Protector/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1153 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Protector/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7598 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Protector/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1789 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Protector/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/Quote/
--rw-r--r--   0 val       (1000) val       (1000)     2524 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Quote/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2519 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Quote/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/Quote/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1700 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Quote/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1418 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Quote/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1372 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Quote/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3106 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Quote/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Quote/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/QuoteGrabs/
--rw-r--r--   0 val       (1000) val       (1000)     2675 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/QuoteGrabs/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3670 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/QuoteGrabs/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/QuoteGrabs/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7337 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/QuoteGrabs/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6529 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/QuoteGrabs/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6636 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/QuoteGrabs/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    17122 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/QuoteGrabs/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     8560 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/QuoteGrabs/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/RSS/
--rw-r--r--   0 val       (1000) val       (1000)     2704 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/RSS/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     6867 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/RSS/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/RSS/locales/
--rw-r--r--   0 val       (1000) val       (1000)    12451 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/RSS/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    15597 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/RSS/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    13213 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/RSS/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    13001 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/RSS/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    12728 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/RSS/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    28414 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/RSS/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    20244 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/RSS/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/Relay/
--rw-r--r--   0 val       (1000) val       (1000)     2517 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Relay/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4744 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Relay/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/Relay/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8274 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Relay/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7545 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Relay/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7487 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Relay/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    19682 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Relay/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1787 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Relay/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/Reply/
--rw-r--r--   0 val       (1000) val       (1000)     2572 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Reply/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2519 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Reply/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.015319 limnoria-2023.9.24/plugins/Reply/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2384 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Reply/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     2630 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Reply/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2331 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Reply/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2669 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Reply/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     2433 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Reply/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3694 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Reply/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3051 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Reply/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/Scheduler/
--rw-r--r--   0 val       (1000) val       (1000)     2757 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Scheduler/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Scheduler/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/Scheduler/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4116 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Scheduler/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     3797 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Scheduler/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3850 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Scheduler/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    12852 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Scheduler/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     8402 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Scheduler/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/SedRegex/
--rw-r--r--   0 val       (1000) val       (1000)     2709 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/SedRegex/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4356 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/SedRegex/config.py
--rwxr-xr-x   0 val       (1000) val       (1000)      874 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/SedRegex/constants.py
--rw-r--r--   0 val       (1000) val       (1000)    10523 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/SedRegex/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    13147 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/SedRegex/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/Seen/
--rw-r--r--   0 val       (1000) val       (1000)     2637 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Seen/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2979 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Seen/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/Seen/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5779 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Seen/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6954 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Seen/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6235 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Seen/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5812 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Seen/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    15271 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Seen/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5431 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Seen/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/Services/
--rw-r--r--   0 val       (1000) val       (1000)     2607 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Services/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5658 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Services/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/Services/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11466 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Services/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    11843 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Services/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    11294 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Services/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    11525 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Services/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    35241 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Services/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    14436 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Services/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/ShrinkUrl/
--rw-r--r--   0 val       (1000) val       (1000)     2542 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ShrinkUrl/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5035 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ShrinkUrl/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/ShrinkUrl/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5983 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ShrinkUrl/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5213 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ShrinkUrl/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5243 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ShrinkUrl/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10186 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ShrinkUrl/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5286 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/ShrinkUrl/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/Status/
--rw-r--r--   0 val       (1000) val       (1000)     2457 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Status/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2901 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Status/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/Status/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5435 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Status/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6124 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Status/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5481 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Status/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5563 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Status/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10046 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Status/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3180 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Status/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/String/
--rw-r--r--   0 val       (1000) val       (1000)     2551 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/String/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3429 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/String/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/String/locales/
--rw-r--r--   0 val       (1000) val       (1000)     9469 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/String/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     8780 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/String/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     8557 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/String/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9911 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/String/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     7585 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/String/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/Success/
--rw-r--r--   0 val       (1000) val       (1000)     2646 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Success/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2751 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Success/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.019319 limnoria-2023.9.24/plugins/Success/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1578 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Success/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1435 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Success/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1323 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Success/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3471 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Success/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2272 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Success/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/Time/
--rw-r--r--   0 val       (1000) val       (1000)     2673 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Time/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2640 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Time/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/Time/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5480 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Time/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6313 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Time/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5483 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Time/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5849 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Time/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     5574 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Time/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10127 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Time/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5071 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Time/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/Todo/
--rw-r--r--   0 val       (1000) val       (1000)     2607 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Todo/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2683 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Todo/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/Todo/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4575 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Todo/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5089 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Todo/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4595 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Todo/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4664 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Todo/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10596 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Todo/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6654 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Todo/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/Topic/
--rw-r--r--   0 val       (1000) val       (1000)     2583 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Topic/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4776 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Topic/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/Topic/locales/
--rw-r--r--   0 val       (1000) val       (1000)    18502 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Topic/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    16877 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Topic/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    17231 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Topic/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    25153 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Topic/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    13078 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Topic/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/URL/
--rw-r--r--   0 val       (1000) val       (1000)     2661 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/URL/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2629 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/URL/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/URL/locales/
--rw-r--r--   0 val       (1000) val       (1000)     3421 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/URL/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2907 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/URL/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2841 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/URL/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     6765 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/URL/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4241 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/URL/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/Unix/
--rw-r--r--   0 val       (1000) val       (1000)     2669 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Unix/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     6252 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Unix/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/Unix/locales/
--rw-r--r--   0 val       (1000) val       (1000)    13680 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Unix/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    11967 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Unix/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    12075 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Unix/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    20048 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Unix/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     7736 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Unix/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/User/
--rw-r--r--   0 val       (1000) val       (1000)     2355 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/User/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2728 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/User/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/User/locales/
--rw-r--r--   0 val       (1000) val       (1000)    15416 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/User/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    21068 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/User/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    19566 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/User/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    10856 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/User/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    15349 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/User/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    23217 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/User/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9203 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/User/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/Utilities/
--rw-r--r--   0 val       (1000) val       (1000)     2407 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Utilities/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Utilities/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.023319 limnoria-2023.9.24/plugins/Utilities/locales/
--rw-r--r--   0 val       (1000) val       (1000)     3623 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Utilities/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     4827 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Utilities/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4250 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Utilities/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4335 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Utilities/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7065 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Utilities/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3958 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Utilities/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.027319 limnoria-2023.9.24/plugins/Web/
--rw-r--r--   0 val       (1000) val       (1000)     2446 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Web/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5246 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Web/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.027319 limnoria-2023.9.24/plugins/Web/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7308 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Web/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     8904 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Web/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7488 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Web/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7113 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Web/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    16701 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Web/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9130 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/Web/test.py
--rw-r--r--   0 val       (1000) val       (1000)    23695 2023-09-24 17:43:59.000000 limnoria-2023.9.24/plugins/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)      192 2023-09-24 17:43:59.000000 limnoria-2023.9.24/pyproject.toml
--rw-r--r--   0 val       (1000) val       (1000)      866 2023-09-24 17:43:59.000000 limnoria-2023.9.24/requirements.txt
--rw-r--r--   0 val       (1000) val       (1000)       38 2023-09-24 18:07:21.031319 limnoria-2023.9.24/setup.cfg
--rw-r--r--   0 val       (1000) val       (1000)     8446 2023-09-24 17:43:59.000000 limnoria-2023.9.24/setup.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.027319 limnoria-2023.9.24/src/
--rw-r--r--   0 val       (1000) val       (1000)     4117 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3548 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/ansi.py
--rw-r--r--   0 val       (1000) val       (1000)    75202 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/callbacks.py
--rw-r--r--   0 val       (1000) val       (1000)    14986 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/cdb.py
--rw-r--r--   0 val       (1000) val       (1000)    41479 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/commands.py
--rw-r--r--   0 val       (1000) val       (1000)    66991 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/conf.py
--rw-r--r--   0 val       (1000) val       (1000)    14165 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/dbi.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.027319 limnoria-2023.9.24/src/drivers/
--rw-r--r--   0 val       (1000) val       (1000)    19096 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/drivers/Socket.py
--rw-r--r--   0 val       (1000) val       (1000)     9696 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/drivers/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2350 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/dynamicScope.py
--rw-r--r--   0 val       (1000) val       (1000)     2997 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/gpg.py
--rw-r--r--   0 val       (1000) val       (1000)    17942 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/httpserver.py
--rw-r--r--   0 val       (1000) val       (1000)    13332 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/i18n.py
--rw-r--r--   0 val       (1000) val       (1000)    51899 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/ircdb.py
--rw-r--r--   0 val       (1000) val       (1000)    98073 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/irclib.py
--rw-r--r--   0 val       (1000) val       (1000)    38939 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/ircmsgs.py
--rw-r--r--   0 val       (1000) val       (1000)    43234 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/ircutils.py
--rw-r--r--   0 val       (1000) val       (1000)    16573 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/log.py
--rw-r--r--   0 val       (1000) val       (1000)     8379 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5342 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/questions.py
--rw-r--r--   0 val       (1000) val       (1000)    34261 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/registry.py
--rw-r--r--   0 val       (1000) val       (1000)     6156 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/schedule.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.027319 limnoria-2023.9.24/src/scripts/
--rw-r--r--   0 val       (1000) val       (1000)        0 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/scripts/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    15886 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/scripts/limnoria.py
--rw-r--r--   0 val       (1000) val       (1000)     5258 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/scripts/limnoria_adduser.py
--rw-r--r--   0 val       (1000) val       (1000)     5455 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/scripts/limnoria_botchk.py
--rw-r--r--   0 val       (1000) val       (1000)    10536 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/scripts/limnoria_plugin_create.py
--rw-r--r--   0 val       (1000) val       (1000)    14353 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/scripts/limnoria_plugin_doc.py
--rw-r--r--   0 val       (1000) val       (1000)     4453 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/scripts/limnoria_reset_password.py
--rw-r--r--   0 val       (1000) val       (1000)     9927 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/scripts/limnoria_test.py
--rw-r--r--   0 val       (1000) val       (1000)    37750 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/scripts/limnoria_wizard.py
--rw-r--r--   0 val       (1000) val       (1000)     4790 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/setup.py
--rw-r--r--   0 val       (1000) val       (1000)     8198 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/shlex.py
--rw-r--r--   0 val       (1000) val       (1000)    25444 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/test.py
--rw-r--r--   0 val       (1000) val       (1000)     3869 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/unpreserve.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.031319 limnoria-2023.9.24/src/utils/
--rw-r--r--   0 val       (1000) val       (1000)     2575 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     1741 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/crypt.py
--rw-r--r--   0 val       (1000) val       (1000)     1992 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/error.py
--rw-r--r--   0 val       (1000) val       (1000)     9475 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/file.py
--rw-r--r--   0 val       (1000) val       (1000)    11587 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/gen.py
--rw-r--r--   0 val       (1000) val       (1000)     5210 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/iter.py
--rw-r--r--   0 val       (1000) val       (1000)     6195 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/math_evaluator.py
--rw-r--r--   0 val       (1000) val       (1000)     3914 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/minisix.py
--rw-r--r--   0 val       (1000) val       (1000)     6526 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/net.py
--rw-r--r--   0 val       (1000) val       (1000)     7726 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/python.py
--rw-r--r--   0 val       (1000) val       (1000)     4169 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/seq.py
--rw-r--r--   0 val       (1000) val       (1000)    21873 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/str.py
--rw-r--r--   0 val       (1000) val       (1000)    19840 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/structures.py
--rw-r--r--   0 val       (1000) val       (1000)     2838 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/time.py
--rw-r--r--   0 val       (1000) val       (1000)     8826 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/transaction.py
--rw-r--r--   0 val       (1000) val       (1000)    10662 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/utils/web.py
--rw-r--r--   0 val       (1000) val       (1000)      175 2023-09-24 18:07:20.000000 limnoria-2023.9.24/src/version.py
--rw-r--r--   0 val       (1000) val       (1000)     7660 2023-09-24 17:43:59.000000 limnoria-2023.9.24/src/world.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2023-09-24 18:07:21.031319 limnoria-2023.9.24/test/
--rw-r--r--   0 val       (1000) val       (1000)     1754 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2265 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test.py
--rw-r--r--   0 val       (1000) val       (1000)    49573 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_callbacks.py
--rw-r--r--   0 val       (1000) val       (1000)     9002 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_commands.py
--rw-r--r--   0 val       (1000) val       (1000)     2813 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_conf.py
--rw-r--r--   0 val       (1000) val       (1000)     4122 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_drivers.py
--rw-r--r--   0 val       (1000) val       (1000)     2458 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_dynamicScope.py
--rw-r--r--   0 val       (1000) val       (1000)     3225 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_firewall.py
--rw-r--r--   0 val       (1000) val       (1000)     1925 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_format.py
--rw-r--r--   0 val       (1000) val       (1000)     2832 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_i18n.py
--rw-r--r--   0 val       (1000) val       (1000)    28459 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_ircdb.py
--rw-r--r--   0 val       (1000) val       (1000)    67775 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_irclib.py
--rw-r--r--   0 val       (1000) val       (1000)    14083 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_ircmsgs.py
--rw-r--r--   0 val       (1000) val       (1000)    22829 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_ircutils.py
--rw-r--r--   0 val       (1000) val       (1000)     3341 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_misc.py
--rw-r--r--   0 val       (1000) val       (1000)     2016 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4832 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_plugin_create.py
--rw-r--r--   0 val       (1000) val       (1000)     2430 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_plugins.py
--rw-r--r--   0 val       (1000) val       (1000)    13283 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_registry.py
--rw-r--r--   0 val       (1000) val       (1000)     4575 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_schedule.py
--rw-r--r--   0 val       (1000) val       (1000)     3759 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_standardSubstitute.py
--rw-r--r--   0 val       (1000) val       (1000)    49349 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_utils.py
--rw-r--r--   0 val       (1000) val       (1000)     3672 2023-09-24 17:43:59.000000 limnoria-2023.9.24/test/test_yn.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.326961 limnoria-2024.4.26/
+-rw-r--r--   0 val       (1000) val       (1000)     1654 2024-05-05 15:42:57.000000 limnoria-2024.4.26/LICENSE.md
+-rw-r--r--   0 val       (1000) val       (1000)      117 2024-05-05 15:42:57.000000 limnoria-2024.4.26/MANIFEST.in
+-rw-r--r--   0 val       (1000) val       (1000)      983 2024-05-05 15:42:57.000000 limnoria-2024.4.26/Makefile
+-rw-r--r--   0 val       (1000) val       (1000)     1848 2024-05-05 15:43:06.326961 limnoria-2024.4.26/PKG-INFO
+-rw-r--r--   0 val       (1000) val       (1000)     2292 2024-05-05 15:42:57.000000 limnoria-2024.4.26/README.md
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.282961 limnoria-2024.4.26/limnoria.egg-info/
+-rw-r--r--   0 val       (1000) val       (1000)     1848 2024-05-05 15:43:06.000000 limnoria-2024.4.26/limnoria.egg-info/PKG-INFO
+-rw-r--r--   0 val       (1000) val       (1000)    16256 2024-05-05 15:43:06.000000 limnoria-2024.4.26/limnoria.egg-info/SOURCES.txt
+-rw-r--r--   0 val       (1000) val       (1000)        1 2024-05-05 15:43:06.000000 limnoria-2024.4.26/limnoria.egg-info/dependency_links.txt
+-rw-r--r--   0 val       (1000) val       (1000)      934 2024-05-05 15:43:06.000000 limnoria-2024.4.26/limnoria.egg-info/entry_points.txt
+-rw-r--r--   0 val       (1000) val       (1000)        8 2024-05-05 15:43:06.000000 limnoria-2024.4.26/limnoria.egg-info/top_level.txt
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.282961 limnoria-2024.4.26/locales/
+-rw-r--r--   0 val       (1000) val       (1000)        0 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    54113 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    76337 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    77441 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3749 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/fr.py
+-rw-r--r--   0 val       (1000) val       (1000)    69991 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    42399 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/messages.pot
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.282961 limnoria-2024.4.26/man/
+-rw-r--r--   0 val       (1000) val       (1000)     1196 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-adduser.1
+-rw-r--r--   0 val       (1000) val       (1000)     1487 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-botchk.1
+-rw-r--r--   0 val       (1000) val       (1000)     1125 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-plugin-create.1
+-rw-r--r--   0 val       (1000) val       (1000)     1378 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-plugin-doc.1
+-rw-r--r--   0 val       (1000) val       (1000)     1026 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-reset-password.1
+-rw-r--r--   0 val       (1000) val       (1000)     1499 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-test.1
+-rw-r--r--   0 val       (1000) val       (1000)     1191 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-wizard.1
+-rw-r--r--   0 val       (1000) val       (1000)     1970 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria.1
+-rw-r--r--   0 val       (1000) val       (1000)     1196 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-adduser.1
+-rw-r--r--   0 val       (1000) val       (1000)     1487 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-botchk.1
+-rw-r--r--   0 val       (1000) val       (1000)     1125 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-plugin-create.1
+-rw-r--r--   0 val       (1000) val       (1000)     1378 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-plugin-doc.1
+-rw-r--r--   0 val       (1000) val       (1000)     1026 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-reset-password.1
+-rw-r--r--   0 val       (1000) val       (1000)     1499 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-test.1
+-rw-r--r--   0 val       (1000) val       (1000)     1191 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-wizard.1
+-rw-r--r--   0 val       (1000) val       (1000)     1970 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot.1
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Admin/
+-rw-r--r--   0 val       (1000) val       (1000)     2422 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2312 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Admin/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8064 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     8857 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7809 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     8112 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    15152 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6275 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Aka/
+-rw-r--r--   0 val       (1000) val       (1000)     2788 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Aka/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2979 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Aka/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Aka/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11022 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Aka/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    39586 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Aka/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    14785 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Aka/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Alias/
+-rw-r--r--   0 val       (1000) val       (1000)     2655 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2539 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Alias/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4716 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5751 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5059 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5176 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     4919 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    19130 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     8039 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Anonymous/
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3516 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Anonymous/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6558 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     7384 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5903 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6893 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     6535 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9054 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6882 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/AutoMode/
+-rw-r--r--   0 val       (1000) val       (1000)     2697 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4521 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/AutoMode/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4202 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5058 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4512 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4131 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     8029 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1787 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Autocomplete/
+-rw-r--r--   0 val       (1000) val       (1000)     2946 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Autocomplete/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2808 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Autocomplete/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     6158 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Autocomplete/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6635 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Autocomplete/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/BadWords/
+-rw-r--r--   0 val       (1000) val       (1000)     2695 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     6163 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/BadWords/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6862 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6112 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6277 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7475 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3943 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Channel/
+-rw-r--r--   0 val       (1000) val       (1000)     2480 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3497 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Channel/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    32456 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    35277 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    32166 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    32899 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    33333 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    44679 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    13344 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/ChannelLogger/
+-rw-r--r--   0 val       (1000) val       (1000)     2531 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5994 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/ChannelLogger/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5491 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5340 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5607 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     5183 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    13745 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9242 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/ChannelStats/
+-rw-r--r--   0 val       (1000) val       (1000)     2682 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3449 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/ChannelStats/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6426 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6640 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6242 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    15391 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4870 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Conditional/
+-rw-r--r--   0 val       (1000) val       (1000)     2907 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2763 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Conditional/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8160 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7180 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7493 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11342 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6497 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Config/
+-rw-r--r--   0 val       (1000) val       (1000)     2325 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Config/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     9209 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     9329 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     9333 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     9333 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     9265 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    21747 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    25531 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Ctcp/
+-rw-r--r--   0 val       (1000) val       (1000)     2420 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3652 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Ctcp/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2084 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     2196 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2072 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2073 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     1911 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7136 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1785 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/DDG/
+-rw-r--r--   0 val       (1000) val       (1000)     2670 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/DDG/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3332 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/DDG/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     6037 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/DDG/parser.py
+-rw-r--r--   0 val       (1000) val       (1000)     6988 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/DDG/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2389 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/DDG/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Debug/
+-rw-r--r--   0 val       (1000) val       (1000)     2377 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Debug/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2399 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Debug/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     7253 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Debug/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2648 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Debug/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Dict/
+-rw-r--r--   0 val       (1000) val       (1000)     2559 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2877 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Dict/local/
+-rw-r--r--   0 val       (1000) val       (1000)       58 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/local/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    12308 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/local/dictclient.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Dict/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     3731 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     3433 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3365 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     6458 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2548 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Dunno/
+-rw-r--r--   0 val       (1000) val       (1000)     2817 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2511 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Dunno/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1414 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     1637 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1557 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1441 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3095 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3446 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Factoids/
+-rw-r--r--   0 val       (1000) val       (1000)     2738 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4867 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Factoids/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    14672 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    14207 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    13986 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    37539 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    10544 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Fediverse/
+-rw-r--r--   0 val       (1000) val       (1000)     2506 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     9206 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/activitypub.py
+-rw-r--r--   0 val       (1000) val       (1000)     3583 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/config.py
+-rw-r--r--   0 val       (1000) val       (1000)    16853 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    21650 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/test.py
+-rw-r--r--   0 val       (1000) val       (1000)    21570 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/test_data.py
+-rw-r--r--   0 val       (1000) val       (1000)     2553 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/utils.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Filter/
+-rw-r--r--   0 val       (1000) val       (1000)     2691 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3118 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Filter/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    14523 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    13736 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    14301 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    27294 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     7848 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Format/
+-rw-r--r--   0 val       (1000) val       (1000)     2559 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2522 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Format/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6742 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5998 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6115 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7452 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4078 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/GPG/
+-rw-r--r--   0 val       (1000) val       (1000)     2606 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/GPG/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2996 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/GPG/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     9566 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/GPG/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5817 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/GPG/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Games/
+-rw-r--r--   0 val       (1000) val       (1000)     2660 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2313 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Games/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4801 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5274 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4968 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4732 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7248 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2854 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Geography/
+-rw-r--r--   0 val       (1000) val       (1000)     2578 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     1936 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/common.py
+-rw-r--r--   0 val       (1000) val       (1000)     2441 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     2924 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/nominatim.py
+-rw-r--r--   0 val       (1000) val       (1000)     6528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    10325 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/test.py
+-rw-r--r--   0 val       (1000) val       (1000)     5514 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/wikidata.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Google/
+-rw-r--r--   0 val       (1000) val       (1000)     2507 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     7042 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Google/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     9595 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     9003 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     9000 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     4460 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/parser.py
+-rw-r--r--   0 val       (1000) val       (1000)    11693 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3095 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Hashes/
+-rw-r--r--   0 val       (1000) val       (1000)     2585 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Hashes/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2244 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Hashes/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     4049 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Hashes/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2754 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Hashes/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Herald/
+-rw-r--r--   0 val       (1000) val       (1000)     2423 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3907 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Herald/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7333 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6711 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6615 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10794 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1789 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Internet/
+-rw-r--r--   0 val       (1000) val       (1000)     2676 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Internet/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2313 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1791 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1769 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     8888 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2420 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Karma/
+-rw-r--r--   0 val       (1000) val       (1000)     2540 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3929 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Karma/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7837 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7070 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7143 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    18303 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9962 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Lart/
+-rw-r--r--   0 val       (1000) val       (1000)     2571 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2679 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Lart/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2427 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2027 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1956 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     4264 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2583 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Later/
+-rw-r--r--   0 val       (1000) val       (1000)     2650 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3413 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Later/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7371 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     7908 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6739 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7370 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11043 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6360 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Limiter/
+-rw-r--r--   0 val       (1000) val       (1000)     2662 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3141 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Limiter/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2685 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2688 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2724 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     2573 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3657 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2871 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/LogToIrc/
+-rw-r--r--   0 val       (1000) val       (1000)     2457 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/LogToIrc/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5627 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/LogToIrc/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     6213 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/LogToIrc/handler.py
+-rw-r--r--   0 val       (1000) val       (1000)     2710 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/LogToIrc/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1781 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/LogToIrc/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Math/
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2516 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Math/local/
+-rw-r--r--   0 val       (1000) val       (1000)       58 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/local/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    46378 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/local/convertcore.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Math/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5920 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5424 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5331 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     5325 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11324 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9441 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/MessageParser/
+-rw-r--r--   0 val       (1000) val       (1000)     3026 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4464 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/MessageParser/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11282 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    10121 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    10440 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    20338 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    11746 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Misc/
+-rw-r--r--   0 val       (1000) val       (1000)     2299 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4131 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Misc/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    13201 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    14554 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    13747 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    13209 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    13537 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    29646 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    17530 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/MoobotFactoids/
+-rw-r--r--   0 val       (1000) val       (1000)     2648 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2740 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/MoobotFactoids/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11225 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    10014 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    10059 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/locales/it.po
+-rwxr-xr-x   0 val       (1000) val       (1000)    29418 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    16971 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Network/
+-rw-r--r--   0 val       (1000) val       (1000)     2514 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Network/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7181 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     8612 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7289 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7472 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    12972 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3097 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/News/
+-rw-r--r--   0 val       (1000) val       (1000)     2777 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2519 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/News/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4608 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4221 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4314 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     8659 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3616 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/NickAuth/
+-rw-r--r--   0 val       (1000) val       (1000)     2574 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2495 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/NickAuth/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4837 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     4838 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     9213 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6306 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/NickCapture/
+-rw-r--r--   0 val       (1000) val       (1000)     2582 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2738 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/NickCapture/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1598 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     1716 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1592 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1500 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     5415 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1799 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Nickometer/
+-rw-r--r--   0 val       (1000) val       (1000)     3249 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2616 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Nickometer/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1338 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1027 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)      952 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9695 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2183 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Note/
+-rw-r--r--   0 val       (1000) val       (1000)     2645 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3477 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Note/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4033 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     3453 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3399 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    16493 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4040 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Owner/
+-rw-r--r--   0 val       (1000) val       (1000)     2427 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3252 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Owner/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8724 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5600 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     8546 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     9038 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     8811 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    33701 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9690 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Plugin/
+-rw-r--r--   0 val       (1000) val       (1000)     2666 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2523 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Plugin/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7234 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     7937 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6377 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7290 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9985 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4272 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/PluginDownloader/
+-rw-r--r--   0 val       (1000) val       (1000)     2670 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2535 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/PluginDownloader/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4570 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6726 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6327 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5727 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    16307 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3847 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Poll/
+-rw-r--r--   0 val       (1000) val       (1000)     2516 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Poll/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2922 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Poll/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     8542 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Poll/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6858 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Poll/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Praise/
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2695 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Praise/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2548 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2424 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2352 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     4348 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1953 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Protector/
+-rw-r--r--   0 val       (1000) val       (1000)     2594 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2901 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Protector/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1626 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1245 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1153 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7598 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1789 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Quote/
+-rw-r--r--   0 val       (1000) val       (1000)     2524 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2519 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Quote/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1700 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1418 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1372 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3106 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/QuoteGrabs/
+-rw-r--r--   0 val       (1000) val       (1000)     2675 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3670 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/QuoteGrabs/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7337 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6529 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6636 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    17122 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     8560 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/RSS/
+-rw-r--r--   0 val       (1000) val       (1000)     2706 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     6867 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/RSS/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    12451 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    15597 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    13213 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    13001 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    12728 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    30557 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    25475 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Relay/
+-rw-r--r--   0 val       (1000) val       (1000)     2517 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4744 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Relay/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8274 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7545 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7487 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    19682 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1787 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Reply/
+-rw-r--r--   0 val       (1000) val       (1000)     2572 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2519 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Reply/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2384 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     2630 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2331 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2669 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     2433 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3694 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3051 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Scheduler/
+-rw-r--r--   0 val       (1000) val       (1000)     2757 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Scheduler/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4116 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     3797 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3850 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    12852 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     8402 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/SedRegex/
+-rw-r--r--   0 val       (1000) val       (1000)     2709 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/SedRegex/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4356 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/SedRegex/config.py
+-rwxr-xr-x   0 val       (1000) val       (1000)      874 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/SedRegex/constants.py
+-rw-r--r--   0 val       (1000) val       (1000)    10523 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/SedRegex/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    13147 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/SedRegex/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Seen/
+-rw-r--r--   0 val       (1000) val       (1000)     2637 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2979 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Seen/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5779 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6954 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6235 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5812 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    16735 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6414 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Services/
+-rw-r--r--   0 val       (1000) val       (1000)     2607 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5658 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Services/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11466 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    11843 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    11294 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    11525 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    35273 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    14436 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/ShrinkUrl/
+-rw-r--r--   0 val       (1000) val       (1000)     2542 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5035 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/ShrinkUrl/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5983 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5213 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5243 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10186 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5286 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Status/
+-rw-r--r--   0 val       (1000) val       (1000)     2457 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2901 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Status/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5435 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6124 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5481 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5563 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11461 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3180 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/String/
+-rw-r--r--   0 val       (1000) val       (1000)     2551 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3429 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/String/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     9469 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     8780 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     8557 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9911 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     7585 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Success/
+-rw-r--r--   0 val       (1000) val       (1000)     2646 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2751 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Success/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1578 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1435 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1323 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3471 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2272 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Time/
+-rw-r--r--   0 val       (1000) val       (1000)     2673 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2640 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Time/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5480 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6313 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5483 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5849 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     5574 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10127 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5071 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Todo/
+-rw-r--r--   0 val       (1000) val       (1000)     2607 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2683 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Todo/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4575 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5089 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4595 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4664 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10596 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6654 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Topic/
+-rw-r--r--   0 val       (1000) val       (1000)     2583 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4776 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Topic/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    18502 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    16877 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    17231 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    25153 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    13078 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/URL/
+-rw-r--r--   0 val       (1000) val       (1000)     2661 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2629 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/URL/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     3421 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2907 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2841 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     6765 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4241 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Unix/
+-rw-r--r--   0 val       (1000) val       (1000)     2669 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     6252 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Unix/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    13680 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    11967 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    12075 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    20048 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     7736 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/User/
+-rw-r--r--   0 val       (1000) val       (1000)     2355 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2728 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/User/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    15416 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    21068 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    19566 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    10856 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    15349 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    23217 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9203 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/Utilities/
+-rw-r--r--   0 val       (1000) val       (1000)     2407 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/Utilities/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     3623 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     4827 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4250 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4335 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7065 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3958 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/Web/
+-rw-r--r--   0 val       (1000) val       (1000)     2446 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5246 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/Web/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7308 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     8904 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7488 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7113 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    17047 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9430 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/test.py
+-rw-r--r--   0 val       (1000) val       (1000)    23695 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)      192 2024-05-05 15:42:57.000000 limnoria-2024.4.26/pyproject.toml
+-rw-r--r--   0 val       (1000) val       (1000)      946 2024-05-05 15:42:57.000000 limnoria-2024.4.26/requirements.txt
+-rw-r--r--   0 val       (1000) val       (1000)       38 2024-05-05 15:43:06.326961 limnoria-2024.4.26/setup.cfg
+-rw-r--r--   0 val       (1000) val       (1000)     8446 2024-05-05 15:42:57.000000 limnoria-2024.4.26/setup.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/src/
+-rw-r--r--   0 val       (1000) val       (1000)     4117 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3548 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/ansi.py
+-rw-r--r--   0 val       (1000) val       (1000)    75220 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/callbacks.py
+-rw-r--r--   0 val       (1000) val       (1000)    14986 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/cdb.py
+-rw-r--r--   0 val       (1000) val       (1000)    41479 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/commands.py
+-rw-r--r--   0 val       (1000) val       (1000)    67015 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/conf.py
+-rw-r--r--   0 val       (1000) val       (1000)    14165 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/dbi.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/src/drivers/
+-rw-r--r--   0 val       (1000) val       (1000)    19591 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/drivers/Socket.py
+-rw-r--r--   0 val       (1000) val       (1000)     9696 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/drivers/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2350 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/dynamicScope.py
+-rw-r--r--   0 val       (1000) val       (1000)     2997 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/gpg.py
+-rw-r--r--   0 val       (1000) val       (1000)    17964 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/httpserver.py
+-rw-r--r--   0 val       (1000) val       (1000)    13332 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/i18n.py
+-rw-r--r--   0 val       (1000) val       (1000)    52151 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/ircdb.py
+-rw-r--r--   0 val       (1000) val       (1000)    98073 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/irclib.py
+-rw-r--r--   0 val       (1000) val       (1000)    38939 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/ircmsgs.py
+-rw-r--r--   0 val       (1000) val       (1000)    43234 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/ircutils.py
+-rw-r--r--   0 val       (1000) val       (1000)    16573 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/log.py
+-rw-r--r--   0 val       (1000) val       (1000)     8379 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5342 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/questions.py
+-rw-r--r--   0 val       (1000) val       (1000)    34261 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/registry.py
+-rw-r--r--   0 val       (1000) val       (1000)     6156 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/schedule.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.326961 limnoria-2024.4.26/src/scripts/
+-rw-r--r--   0 val       (1000) val       (1000)        0 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    15886 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria.py
+-rw-r--r--   0 val       (1000) val       (1000)     5258 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_adduser.py
+-rw-r--r--   0 val       (1000) val       (1000)     5455 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_botchk.py
+-rw-r--r--   0 val       (1000) val       (1000)    10536 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_plugin_create.py
+-rw-r--r--   0 val       (1000) val       (1000)    14353 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_plugin_doc.py
+-rw-r--r--   0 val       (1000) val       (1000)     4454 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_reset_password.py
+-rw-r--r--   0 val       (1000) val       (1000)    10443 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_test.py
+-rw-r--r--   0 val       (1000) val       (1000)    37750 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_wizard.py
+-rw-r--r--   0 val       (1000) val       (1000)     4790 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/setup.py
+-rw-r--r--   0 val       (1000) val       (1000)     8198 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/shlex.py
+-rw-r--r--   0 val       (1000) val       (1000)    25444 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/test.py
+-rw-r--r--   0 val       (1000) val       (1000)     3869 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/unpreserve.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.326961 limnoria-2024.4.26/src/utils/
+-rw-r--r--   0 val       (1000) val       (1000)     2575 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     1741 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/crypt.py
+-rw-r--r--   0 val       (1000) val       (1000)     1992 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/error.py
+-rw-r--r--   0 val       (1000) val       (1000)     9475 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/file.py
+-rw-r--r--   0 val       (1000) val       (1000)    11587 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/gen.py
+-rw-r--r--   0 val       (1000) val       (1000)     5210 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/iter.py
+-rw-r--r--   0 val       (1000) val       (1000)     6195 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/math_evaluator.py
+-rw-r--r--   0 val       (1000) val       (1000)     3914 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/minisix.py
+-rw-r--r--   0 val       (1000) val       (1000)     6526 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/net.py
+-rw-r--r--   0 val       (1000) val       (1000)     7726 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/python.py
+-rw-r--r--   0 val       (1000) val       (1000)     4169 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/seq.py
+-rw-r--r--   0 val       (1000) val       (1000)    21873 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/str.py
+-rw-r--r--   0 val       (1000) val       (1000)    19840 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/structures.py
+-rw-r--r--   0 val       (1000) val       (1000)     2838 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/time.py
+-rw-r--r--   0 val       (1000) val       (1000)     8826 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/transaction.py
+-rw-r--r--   0 val       (1000) val       (1000)    10662 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/web.py
+-rw-r--r--   0 val       (1000) val       (1000)      175 2024-05-05 15:43:05.000000 limnoria-2024.4.26/src/version.py
+-rw-r--r--   0 val       (1000) val       (1000)     7660 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/world.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.326961 limnoria-2024.4.26/test/
+-rw-r--r--   0 val       (1000) val       (1000)     1754 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2265 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test.py
+-rw-r--r--   0 val       (1000) val       (1000)    49856 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_callbacks.py
+-rw-r--r--   0 val       (1000) val       (1000)     9002 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_commands.py
+-rw-r--r--   0 val       (1000) val       (1000)     2813 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_conf.py
+-rw-r--r--   0 val       (1000) val       (1000)     4122 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_drivers.py
+-rw-r--r--   0 val       (1000) val       (1000)     2458 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_dynamicScope.py
+-rw-r--r--   0 val       (1000) val       (1000)     3225 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_firewall.py
+-rw-r--r--   0 val       (1000) val       (1000)     1925 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_format.py
+-rw-r--r--   0 val       (1000) val       (1000)     2832 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_i18n.py
+-rw-r--r--   0 val       (1000) val       (1000)    29200 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_ircdb.py
+-rw-r--r--   0 val       (1000) val       (1000)    67775 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_irclib.py
+-rw-r--r--   0 val       (1000) val       (1000)    14083 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_ircmsgs.py
+-rw-r--r--   0 val       (1000) val       (1000)    22829 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_ircutils.py
+-rw-r--r--   0 val       (1000) val       (1000)     3341 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_misc.py
+-rw-r--r--   0 val       (1000) val       (1000)     2016 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4832 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_plugin_create.py
+-rw-r--r--   0 val       (1000) val       (1000)     2430 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_plugins.py
+-rw-r--r--   0 val       (1000) val       (1000)    13283 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_registry.py
+-rw-r--r--   0 val       (1000) val       (1000)     4575 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_schedule.py
+-rw-r--r--   0 val       (1000) val       (1000)     3759 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_standardSubstitute.py
+-rw-r--r--   0 val       (1000) val       (1000)    49349 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_utils.py
+-rw-r--r--   0 val       (1000) val       (1000)     3672 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_yn.py
```

### Comparing `limnoria-2023.9.24/LICENSE.md` & `limnoria-2024.4.26/LICENSE.md`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/Makefile` & `limnoria-2024.4.26/Makefile`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/PKG-INFO` & `limnoria-2024.4.26/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limnoria
-Version: 2023.9.24
+Version: 2024.4.26
 Summary: A multipurpose Python IRC bot, designed for flexibility and robustness , while being easy to install, set up, and maintain.
 Home-page: https://limnoria.net/
 Download-URL: https://pypi.python.org/pypi/limnoria
 Author: Valentin Lorentz
 Author-email: progval+limnoria@progval.net
 Platform: linux
 Platform: linux2
```

### Comparing `limnoria-2023.9.24/README.md` & `limnoria-2024.4.26/README.md`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/limnoria.egg-info/PKG-INFO` & `limnoria-2024.4.26/limnoria.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limnoria
-Version: 2023.9.24
+Version: 2024.4.26
 Summary: A multipurpose Python IRC bot, designed for flexibility and robustness , while being easy to install, set up, and maintain.
 Home-page: https://limnoria.net/
 Download-URL: https://pypi.python.org/pypi/limnoria
 Author: Valentin Lorentz
 Author-email: progval+limnoria@progval.net
 Platform: linux
 Platform: linux2
```

### Comparing `limnoria-2023.9.24/limnoria.egg-info/SOURCES.txt` & `limnoria-2024.4.26/limnoria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/limnoria.egg-info/entry_points.txt` & `limnoria-2024.4.26/limnoria.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/locales/de.po` & `limnoria-2024.4.26/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/locales/fi.po` & `limnoria-2024.4.26/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/locales/fr.po` & `limnoria-2024.4.26/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/locales/fr.py` & `limnoria-2024.4.26/locales/fr.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/locales/it.po` & `limnoria-2024.4.26/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/locales/messages.pot` & `limnoria-2024.4.26/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/limnoria-adduser.1` & `limnoria-2024.4.26/man/limnoria-adduser.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/limnoria-botchk.1` & `limnoria-2024.4.26/man/limnoria-botchk.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/limnoria-plugin-create.1` & `limnoria-2024.4.26/man/limnoria-plugin-create.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/limnoria-plugin-doc.1` & `limnoria-2024.4.26/man/limnoria-plugin-doc.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/limnoria-reset-password.1` & `limnoria-2024.4.26/man/limnoria-reset-password.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/limnoria-test.1` & `limnoria-2024.4.26/man/limnoria-test.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/limnoria-wizard.1` & `limnoria-2024.4.26/man/limnoria-wizard.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/limnoria.1` & `limnoria-2024.4.26/man/limnoria.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/supybot-adduser.1` & `limnoria-2024.4.26/man/supybot-adduser.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/supybot-botchk.1` & `limnoria-2024.4.26/man/supybot-botchk.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/supybot-plugin-create.1` & `limnoria-2024.4.26/man/supybot-plugin-create.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/supybot-plugin-doc.1` & `limnoria-2024.4.26/man/supybot-plugin-doc.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/supybot-reset-password.1` & `limnoria-2024.4.26/man/supybot-reset-password.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/supybot-test.1` & `limnoria-2024.4.26/man/supybot-test.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/supybot-wizard.1` & `limnoria-2024.4.26/man/supybot-wizard.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/man/supybot.1` & `limnoria-2024.4.26/man/supybot.1`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Admin/__init__.py` & `limnoria-2024.4.26/plugins/Admin/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Admin/config.py` & `limnoria-2024.4.26/plugins/Admin/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Admin/locales/de.po` & `limnoria-2024.4.26/plugins/Admin/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Admin/locales/fi.po` & `limnoria-2024.4.26/plugins/Admin/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Admin/locales/fr.po` & `limnoria-2024.4.26/plugins/Admin/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Admin/locales/it.po` & `limnoria-2024.4.26/plugins/Admin/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Admin/plugin.py` & `limnoria-2024.4.26/plugins/Admin/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Admin/test.py` & `limnoria-2024.4.26/plugins/Admin/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         self.assertRegexp('channels', '#foo')
         self.irc.feedMsg(ircmsgs.join('#bar', prefix=self.prefix))
         getAfterJoinMessages()
         self.assertRegexp('channels', '#bar and #foo')
         self.irc.feedMsg(ircmsgs.join('#Baz', prefix=self.prefix))
         getAfterJoinMessages()
         self.assertRegexp('channels', '#bar, #Baz, and #foo')
+        self.assertNotRegexp('config networks.test.channels', '.*#foo.*')
 
     def testIgnoreAddRemove(self):
         self.assertNotError('admin ignore add foo!bar@baz')
         self.assertError('admin ignore add alsdkfjlasd')
         self.assertNotError('admin ignore remove foo!bar@baz')
         self.assertError('admin ignore remove foo!bar@baz')
 
@@ -83,48 +84,55 @@
         self.assertIn('bar', u.capabilities)
         self.assertError('removecapability foo bar')
         self.assertNotError('capability remove foo bar')
         self.assertNotIn('bar', u.capabilities)
         ircdb.users.delUser(u.id)
 
     def testJoin(self):
-        m = self.getMsg('join #foo')
-        self.assertEqual(m.command, 'JOIN')
-        self.assertEqual(m.args[0], '#foo')
-        m = self.getMsg('join #foo key')
-        self.assertEqual(m.command, 'JOIN')
-        self.assertEqual(m.args[0], '#foo')
-        self.assertEqual(m.args[1], 'key')
+        try:
+            m = self.getMsg('join #foo')
+            self.assertEqual(m.command, 'JOIN')
+            self.assertEqual(m.args[0], '#foo')
+            m = self.getMsg('join #foo key')
+            self.assertEqual(m.command, 'JOIN')
+            self.assertEqual(m.args[0], '#foo')
+            self.assertEqual(m.args[1], 'key')
+        finally:
+            conf.supybot.networks.test.channels.setValue('')
 
     def testNick(self):
         try:
             m = self.getMsg('nick foobar')
             self.assertEqual(m.command, 'NICK')
             self.assertEqual(m.args[0], 'foobar')
         finally:
             conf.supybot.networks.test.nick.setValue('')
 
     def testAddCapabilityOwner(self):
         self.assertError('admin capability add %s owner' % self.nick)
 
     def testJoinOnOwnerInvite(self):
-        self.irc.feedMsg(ircmsgs.invite(conf.supybot.nick(), '#foo', prefix=self.prefix))
-        m = self.getMsg(' ')
-        self.assertEqual(m.command, 'JOIN')
-        self.assertEqual(m.args[0], '#foo')
+        try:
+            self.irc.feedMsg(ircmsgs.invite(conf.supybot.nick(), '#foo', prefix=self.prefix))
+            m = self.getMsg(' ')
+            self.assertEqual(m.command, 'JOIN')
+            self.assertEqual(m.args[0], '#foo')
+        finally:
+            conf.supybot.networks.test.channels.setValue('')
 
     def testNoJoinOnUnprivilegedInvite(self):
         try:
             world.testing = False
             for channel in '#foo', '#foo\u0009':
                 self.irc.feedMsg(ircmsgs.invite(conf.supybot.nick(), channel, prefix='foo!bar@baz'))
                 self.assertResponse('somecommand',
                     'Error: "somecommand" is not a valid command.')
         finally:
             world.testing = True
+            self.assertNotRegexp('config networks.test.channels', '.*#foo.*')
 
     def testAcmd(self):
         self.irc.feedMsg(ircmsgs.join('#foo', prefix=self.prefix))
         self.irc.feedMsg(ircmsgs.join('#bar', prefix=self.prefix))
         while self.irc.takeMsg():
             pass
         msgs = []
```

### Comparing `limnoria-2023.9.24/plugins/Aka/__init__.py` & `limnoria-2024.4.26/plugins/Aka/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Aka/config.py` & `limnoria-2024.4.26/plugins/Aka/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Aka/locales/fi.po` & `limnoria-2024.4.26/plugins/Aka/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Aka/plugin.py` & `limnoria-2024.4.26/plugins/Aka/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Aka/test.py` & `limnoria-2024.4.26/plugins/Aka/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Alias/__init__.py` & `limnoria-2024.4.26/plugins/Alias/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Alias/config.py` & `limnoria-2024.4.26/plugins/Alias/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Alias/locales/de.po` & `limnoria-2024.4.26/plugins/Alias/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Alias/locales/fi.po` & `limnoria-2024.4.26/plugins/Alias/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Alias/locales/fr.po` & `limnoria-2024.4.26/plugins/Alias/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Alias/locales/hu.po` & `limnoria-2024.4.26/plugins/Alias/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Alias/locales/it.po` & `limnoria-2024.4.26/plugins/Alias/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Alias/plugin.py` & `limnoria-2024.4.26/plugins/Alias/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Alias/test.py` & `limnoria-2024.4.26/plugins/Alias/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Anonymous/__init__.py` & `limnoria-2024.4.26/plugins/Anonymous/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Anonymous/config.py` & `limnoria-2024.4.26/plugins/Anonymous/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Anonymous/locales/de.po` & `limnoria-2024.4.26/plugins/Anonymous/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Anonymous/locales/fi.po` & `limnoria-2024.4.26/plugins/Anonymous/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Anonymous/locales/fr.po` & `limnoria-2024.4.26/plugins/Anonymous/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Anonymous/locales/hu.po` & `limnoria-2024.4.26/plugins/Anonymous/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Anonymous/locales/it.po` & `limnoria-2024.4.26/plugins/Anonymous/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Anonymous/plugin.py` & `limnoria-2024.4.26/plugins/Anonymous/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Anonymous/test.py` & `limnoria-2024.4.26/plugins/Anonymous/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/AutoMode/__init__.py` & `limnoria-2024.4.26/plugins/AutoMode/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/AutoMode/config.py` & `limnoria-2024.4.26/plugins/AutoMode/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/AutoMode/locales/de.po` & `limnoria-2024.4.26/plugins/AutoMode/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/AutoMode/locales/fi.po` & `limnoria-2024.4.26/plugins/AutoMode/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/AutoMode/locales/fr.po` & `limnoria-2024.4.26/plugins/AutoMode/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/AutoMode/locales/it.po` & `limnoria-2024.4.26/plugins/AutoMode/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/AutoMode/plugin.py` & `limnoria-2024.4.26/plugins/AutoMode/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/AutoMode/test.py` & `limnoria-2024.4.26/plugins/AutoMode/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Autocomplete/__init__.py` & `limnoria-2024.4.26/plugins/Autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Autocomplete/config.py` & `limnoria-2024.4.26/plugins/Autocomplete/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Autocomplete/plugin.py` & `limnoria-2024.4.26/plugins/Autocomplete/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Autocomplete/test.py` & `limnoria-2024.4.26/plugins/Autocomplete/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/BadWords/__init__.py` & `limnoria-2024.4.26/plugins/BadWords/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/BadWords/config.py` & `limnoria-2024.4.26/plugins/BadWords/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/BadWords/locales/fi.po` & `limnoria-2024.4.26/plugins/BadWords/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/BadWords/locales/fr.po` & `limnoria-2024.4.26/plugins/BadWords/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/BadWords/locales/it.po` & `limnoria-2024.4.26/plugins/BadWords/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/BadWords/plugin.py` & `limnoria-2024.4.26/plugins/BadWords/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/BadWords/test.py` & `limnoria-2024.4.26/plugins/BadWords/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Channel/__init__.py` & `limnoria-2024.4.26/plugins/Channel/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Channel/config.py` & `limnoria-2024.4.26/plugins/Channel/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Channel/locales/de.po` & `limnoria-2024.4.26/plugins/Channel/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Channel/locales/fi.po` & `limnoria-2024.4.26/plugins/Channel/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Channel/locales/fr.po` & `limnoria-2024.4.26/plugins/Channel/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Channel/locales/hu.po` & `limnoria-2024.4.26/plugins/Channel/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Channel/locales/it.po` & `limnoria-2024.4.26/plugins/Channel/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Channel/plugin.py` & `limnoria-2024.4.26/plugins/Channel/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -987,17 +987,22 @@
         capability = ircdb.makeChannelCapability(channel, 'op')
         if not ircdb.checkCapabilities(msg.prefix, [capability, 'admin']):
             irc.errorNoCapability(capability, Raise=True)
         try:
             network = conf.supybot.networks.get(irc.network)
             network.channels().remove(channel)
         except KeyError:
-            pass
-        if channel not in irc.state.channels:
-            irc.error(_('I\'m not in %s.') % channel, Raise=True)
+            if channel not in irc.state.channels:
+                # Not configured AND not in the channel
+                irc.error(_('I\'m not in %s.') % channel, Raise=True)
+        else:
+            if channel not in irc.state.channels:
+                # Configured, but not in the channel
+                irc.reply(_('%s removed from configured join list.') % channel)
+                return
         reason = (reason or self.registryValue("partMsg", channel, irc.network))
         reason = ircutils.standardSubstitute(irc, msg, reason)
         irc.queueMsg(ircmsgs.part(channel, reason))
         if msg.nick in irc.state.channels[channel].users:
             irc.noReply()
         else:
             irc.replySuccess()
```

### Comparing `limnoria-2023.9.24/plugins/Channel/test.py` & `limnoria-2024.4.26/plugins/Channel/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelLogger/__init__.py` & `limnoria-2024.4.26/plugins/ChannelLogger/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelLogger/config.py` & `limnoria-2024.4.26/plugins/ChannelLogger/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelLogger/locales/fi.po` & `limnoria-2024.4.26/plugins/ChannelLogger/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelLogger/locales/fr.po` & `limnoria-2024.4.26/plugins/ChannelLogger/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelLogger/locales/hu.po` & `limnoria-2024.4.26/plugins/ChannelLogger/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelLogger/locales/it.po` & `limnoria-2024.4.26/plugins/ChannelLogger/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelLogger/plugin.py` & `limnoria-2024.4.26/plugins/ChannelLogger/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelLogger/test.py` & `limnoria-2024.4.26/plugins/ChannelLogger/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelStats/__init__.py` & `limnoria-2024.4.26/plugins/ChannelStats/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelStats/config.py` & `limnoria-2024.4.26/plugins/ChannelStats/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelStats/locales/fi.po` & `limnoria-2024.4.26/plugins/ChannelStats/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelStats/locales/fr.po` & `limnoria-2024.4.26/plugins/ChannelStats/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelStats/locales/it.po` & `limnoria-2024.4.26/plugins/ChannelStats/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelStats/plugin.py` & `limnoria-2024.4.26/plugins/ChannelStats/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ChannelStats/test.py` & `limnoria-2024.4.26/plugins/ChannelStats/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Conditional/__init__.py` & `limnoria-2024.4.26/plugins/Conditional/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Conditional/config.py` & `limnoria-2024.4.26/plugins/Conditional/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Conditional/locales/fi.po` & `limnoria-2024.4.26/plugins/Conditional/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Conditional/locales/fr.po` & `limnoria-2024.4.26/plugins/Conditional/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Conditional/locales/it.po` & `limnoria-2024.4.26/plugins/Conditional/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Conditional/plugin.py` & `limnoria-2024.4.26/plugins/Conditional/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Conditional/test.py` & `limnoria-2024.4.26/plugins/Conditional/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Config/__init__.py` & `limnoria-2024.4.26/plugins/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Config/config.py` & `limnoria-2024.4.26/plugins/Config/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Config/locales/de.po` & `limnoria-2024.4.26/plugins/Config/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Config/locales/fi.po` & `limnoria-2024.4.26/plugins/Config/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Config/locales/fr.po` & `limnoria-2024.4.26/plugins/Config/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Config/locales/hu.po` & `limnoria-2024.4.26/plugins/Config/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Config/locales/it.po` & `limnoria-2024.4.26/plugins/Config/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Config/plugin.py` & `limnoria-2024.4.26/plugins/Config/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Config/test.py` & `limnoria-2024.4.26/plugins/Config/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Ctcp/__init__.py` & `limnoria-2024.4.26/plugins/Ctcp/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Ctcp/config.py` & `limnoria-2024.4.26/plugins/Ctcp/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Ctcp/locales/de.po` & `limnoria-2024.4.26/plugins/Ctcp/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Ctcp/locales/fi.po` & `limnoria-2024.4.26/plugins/Ctcp/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Ctcp/locales/fr.po` & `limnoria-2024.4.26/plugins/Ctcp/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Ctcp/locales/hu.po` & `limnoria-2024.4.26/plugins/Ctcp/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Ctcp/locales/it.po` & `limnoria-2024.4.26/plugins/Ctcp/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Ctcp/plugin.py` & `limnoria-2024.4.26/plugins/Ctcp/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Ctcp/test.py` & `limnoria-2024.4.26/plugins/Ctcp/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/DDG/__init__.py` & `limnoria-2024.4.26/plugins/DDG/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/DDG/config.py` & `limnoria-2024.4.26/plugins/DDG/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/DDG/parser.py` & `limnoria-2024.4.26/plugins/DDG/parser.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/DDG/plugin.py` & `limnoria-2024.4.26/plugins/DDG/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/DDG/test.py` & `limnoria-2024.4.26/plugins/DDG/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Debug/__init__.py` & `limnoria-2024.4.26/plugins/Debug/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Debug/config.py` & `limnoria-2024.4.26/plugins/Debug/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Debug/plugin.py` & `limnoria-2024.4.26/plugins/Debug/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/python
-
 ###
 # Copyright (c) 2002-2005, Jeremiah Fincher
 # Copyright (c) 2010-2021, Valentin Lorentz
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
```

### Comparing `limnoria-2023.9.24/plugins/Debug/test.py` & `limnoria-2024.4.26/plugins/Debug/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dict/__init__.py` & `limnoria-2024.4.26/plugins/Dict/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dict/config.py` & `limnoria-2024.4.26/plugins/Dict/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dict/local/dictclient.py` & `limnoria-2024.4.26/plugins/Dict/local/dictclient.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dict/locales/fi.po` & `limnoria-2024.4.26/plugins/Dict/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dict/locales/fr.po` & `limnoria-2024.4.26/plugins/Dict/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dict/locales/it.po` & `limnoria-2024.4.26/plugins/Dict/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dict/plugin.py` & `limnoria-2024.4.26/plugins/Dict/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dict/test.py` & `limnoria-2024.4.26/plugins/Dict/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dunno/__init__.py` & `limnoria-2024.4.26/plugins/Dunno/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dunno/config.py` & `limnoria-2024.4.26/plugins/Dunno/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dunno/locales/de.po` & `limnoria-2024.4.26/plugins/Dunno/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dunno/locales/fi.po` & `limnoria-2024.4.26/plugins/Dunno/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dunno/locales/fr.po` & `limnoria-2024.4.26/plugins/Dunno/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dunno/locales/it.po` & `limnoria-2024.4.26/plugins/Dunno/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dunno/plugin.py` & `limnoria-2024.4.26/plugins/Dunno/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Dunno/test.py` & `limnoria-2024.4.26/plugins/Dunno/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Factoids/__init__.py` & `limnoria-2024.4.26/plugins/Factoids/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Factoids/config.py` & `limnoria-2024.4.26/plugins/Factoids/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Factoids/locales/fi.po` & `limnoria-2024.4.26/plugins/Factoids/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Factoids/locales/fr.po` & `limnoria-2024.4.26/plugins/Factoids/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Factoids/locales/it.po` & `limnoria-2024.4.26/plugins/Factoids/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Factoids/plugin.py` & `limnoria-2024.4.26/plugins/Factoids/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Factoids/test.py` & `limnoria-2024.4.26/plugins/Factoids/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Fediverse/__init__.py` & `limnoria-2024.4.26/plugins/Fediverse/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Fediverse/activitypub.py` & `limnoria-2024.4.26/plugins/Fediverse/activitypub.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Fediverse/config.py` & `limnoria-2024.4.26/plugins/Fediverse/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Fediverse/plugin.py` & `limnoria-2024.4.26/plugins/Fediverse/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,17 +173,23 @@
         super().die()
 
     def _stopHttp(self):
         httpserver.unhook("fediverse")
 
     def _has_webfinger_support(self, hostname):
         if hostname not in self._webfinger_support_cache:
-            self._webfinger_support_cache[hostname] = ap.has_webfinger_support(
-                hostname
-            )
+            try:
+                self._webfinger_support_cache[hostname] = ap.has_webfinger_support(
+                    hostname
+                )
+            except Exception as e:
+                self.log.error(
+                    "Checking Webfinger support for %s raised %s", hostname, e
+                )
+                return False
         return self._webfinger_support_cache[hostname]
 
     def _get_actor(self, irc, username):
         if username in self._actor_cache:
             return self._actor_cache[username]
         match = _username_regexp.match(username)
         if match:
```

### Comparing `limnoria-2023.9.24/plugins/Fediverse/test.py` & `limnoria-2024.4.26/plugins/Fediverse/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Fediverse/test_data.py` & `limnoria-2024.4.26/plugins/Fediverse/test_data.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Fediverse/utils.py` & `limnoria-2024.4.26/plugins/Fediverse/utils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Filter/__init__.py` & `limnoria-2024.4.26/plugins/Filter/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Filter/config.py` & `limnoria-2024.4.26/plugins/Filter/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Filter/locales/fi.po` & `limnoria-2024.4.26/plugins/Filter/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Filter/locales/fr.po` & `limnoria-2024.4.26/plugins/Filter/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Filter/locales/it.po` & `limnoria-2024.4.26/plugins/Filter/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Filter/plugin.py` & `limnoria-2024.4.26/plugins/Filter/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Filter/test.py` & `limnoria-2024.4.26/plugins/Filter/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Format/__init__.py` & `limnoria-2024.4.26/plugins/Format/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Format/config.py` & `limnoria-2024.4.26/plugins/Format/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Format/locales/fi.po` & `limnoria-2024.4.26/plugins/Format/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Format/locales/fr.po` & `limnoria-2024.4.26/plugins/Format/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Format/locales/it.po` & `limnoria-2024.4.26/plugins/Format/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Format/plugin.py` & `limnoria-2024.4.26/plugins/Format/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Format/test.py` & `limnoria-2024.4.26/plugins/Format/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/GPG/__init__.py` & `limnoria-2024.4.26/plugins/GPG/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/GPG/config.py` & `limnoria-2024.4.26/plugins/GPG/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/GPG/plugin.py` & `limnoria-2024.4.26/plugins/GPG/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/GPG/test.py` & `limnoria-2024.4.26/plugins/GPG/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Games/__init__.py` & `limnoria-2024.4.26/plugins/Games/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Games/config.py` & `limnoria-2024.4.26/plugins/Games/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Games/locales/de.po` & `limnoria-2024.4.26/plugins/Games/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Games/locales/fi.po` & `limnoria-2024.4.26/plugins/Games/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Games/locales/fr.po` & `limnoria-2024.4.26/plugins/Games/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Games/locales/it.po` & `limnoria-2024.4.26/plugins/Games/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Games/plugin.py` & `limnoria-2024.4.26/plugins/Games/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Games/test.py` & `limnoria-2024.4.26/plugins/Games/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Geography/__init__.py` & `limnoria-2024.4.26/plugins/Geography/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Geography/common.py` & `limnoria-2024.4.26/plugins/Geography/common.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Geography/config.py` & `limnoria-2024.4.26/plugins/Geography/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Geography/nominatim.py` & `limnoria-2024.4.26/plugins/Geography/nominatim.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Geography/plugin.py` & `limnoria-2024.4.26/plugins/Geography/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Geography/test.py` & `limnoria-2024.4.26/plugins/Geography/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,23 +183,29 @@
     def testLocaltimeIntegration(self):
         self.assertRegexp("localtime Metz, France", r".*\+0[12]00$")
         self.assertRegexp("localtime Saint-Denis, La Réunion", r".*\+0400$")
 
 
 class GeographyWikidataTestCase(SupyTestCase):
     @skipIf(not network, "Network test")
-    def testOsmidToTimezone(self):
+    def testRelationOsmidToTimezone(self):
         self.assertEqual(
             wikidata.uri_from_osmid(450381),
             "http://www.wikidata.org/entity/Q22690",
         )
         self.assertEqual(
             wikidata.uri_from_osmid(192468),
             "http://www.wikidata.org/entity/Q47045",
         )
+    @skipIf(not network, "Network test")
+    def testNodeOsmidToTimezone(self):
+        self.assertEqual(
+            wikidata.uri_from_osmid(436012592),
+            "http://www.wikidata.org/entity/Q933",
+        )
 
     @skipIf(not network, "Network test")
     def testDirect(self):
         # The queried object directly has a timezone property
         self.assertEqual(
             # New York
             wikidata.timezone_from_uri("http://www.wikidata.org/entity/Q1384"),
```

### Comparing `limnoria-2023.9.24/plugins/Geography/wikidata.py` & `limnoria-2024.4.26/plugins/Geography/wikidata.py`

 * *Files 10% similar despite different names*

```diff
@@ -111,15 +111,22 @@
 LIMIT 1
 """
 )
 
 OSMID_QUERY = string.Template(
     """
 SELECT ?item WHERE {
-  ?item wdt:P402 "$osmid".
+  {
+    ?item wdt:P402 "$osmid".  # OSM relation ID
+  }
+  UNION
+  {
+    ?item wdt:P11693 "$osmid".  # OSM node ID
+  }
+
 }
 LIMIT 1
 """
 )
 
 
 def _query_sparql(query):
```

### Comparing `limnoria-2023.9.24/plugins/Google/__init__.py` & `limnoria-2024.4.26/plugins/Google/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Google/config.py` & `limnoria-2024.4.26/plugins/Google/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Google/locales/fi.po` & `limnoria-2024.4.26/plugins/Google/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Google/locales/fr.po` & `limnoria-2024.4.26/plugins/Google/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Google/locales/it.po` & `limnoria-2024.4.26/plugins/Google/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Google/parser.py` & `limnoria-2024.4.26/plugins/Google/parser.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Google/plugin.py` & `limnoria-2024.4.26/plugins/Google/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Google/test.py` & `limnoria-2024.4.26/plugins/Google/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Hashes/__init__.py` & `limnoria-2024.4.26/plugins/Hashes/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Hashes/config.py` & `limnoria-2024.4.26/plugins/Hashes/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Hashes/plugin.py` & `limnoria-2024.4.26/plugins/Hashes/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Hashes/test.py` & `limnoria-2024.4.26/plugins/Hashes/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Herald/__init__.py` & `limnoria-2024.4.26/plugins/Herald/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Herald/config.py` & `limnoria-2024.4.26/plugins/Herald/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Herald/locales/fi.po` & `limnoria-2024.4.26/plugins/Herald/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Herald/locales/fr.po` & `limnoria-2024.4.26/plugins/Herald/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Herald/locales/it.po` & `limnoria-2024.4.26/plugins/Herald/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Herald/plugin.py` & `limnoria-2024.4.26/plugins/Herald/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Herald/test.py` & `limnoria-2024.4.26/plugins/Herald/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Internet/__init__.py` & `limnoria-2024.4.26/plugins/Internet/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Internet/config.py` & `limnoria-2024.4.26/plugins/Internet/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Internet/locales/fi.po` & `limnoria-2024.4.26/plugins/Internet/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Internet/locales/fr.po` & `limnoria-2024.4.26/plugins/Internet/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Internet/locales/it.po` & `limnoria-2024.4.26/plugins/Internet/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Internet/plugin.py` & `limnoria-2024.4.26/plugins/Internet/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                 s = ':'.join(line.split(':')[1:]).strip()
                 expires = _('expires %s') % s
             elif not status and any(line.startswith, self._status):
                 status = ':'.join(line.split(':')[1:]).strip().lower()
         if not status:
             status = 'unknown'
         try:
-            t = telnetlib.Telnet('whois.pir.org', 43)
+            t = telnetlib.Telnet('whois.iana.org', 43)
         except socket.error as e:
             irc.error(str(e))
             return
         t.write(b'registrar ')
         t.write(registrar.split('(')[0].strip().encode('ascii'))
         t.write(b'\n')
         s = t.read_all()
```

### Comparing `limnoria-2023.9.24/plugins/Internet/test.py` & `limnoria-2024.4.26/plugins/Internet/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Karma/__init__.py` & `limnoria-2024.4.26/plugins/Karma/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Karma/config.py` & `limnoria-2024.4.26/plugins/Karma/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Karma/locales/fi.po` & `limnoria-2024.4.26/plugins/Karma/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Karma/locales/fr.po` & `limnoria-2024.4.26/plugins/Karma/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Karma/locales/it.po` & `limnoria-2024.4.26/plugins/Karma/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Karma/plugin.py` & `limnoria-2024.4.26/plugins/Karma/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Karma/test.py` & `limnoria-2024.4.26/plugins/Karma/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Lart/__init__.py` & `limnoria-2024.4.26/plugins/Lart/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Lart/config.py` & `limnoria-2024.4.26/plugins/Lart/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Lart/locales/fi.po` & `limnoria-2024.4.26/plugins/Lart/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Lart/locales/fr.po` & `limnoria-2024.4.26/plugins/Lart/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Lart/locales/it.po` & `limnoria-2024.4.26/plugins/Lart/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Lart/plugin.py` & `limnoria-2024.4.26/plugins/Lart/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Lart/test.py` & `limnoria-2024.4.26/plugins/Lart/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Later/__init__.py` & `limnoria-2024.4.26/plugins/Later/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Later/config.py` & `limnoria-2024.4.26/plugins/Later/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Later/locales/de.po` & `limnoria-2024.4.26/plugins/Later/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Later/locales/fi.po` & `limnoria-2024.4.26/plugins/Later/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Later/locales/fr.po` & `limnoria-2024.4.26/plugins/Later/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Later/locales/it.po` & `limnoria-2024.4.26/plugins/Later/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Later/plugin.py` & `limnoria-2024.4.26/plugins/Later/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Later/test.py` & `limnoria-2024.4.26/plugins/Later/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Limiter/__init__.py` & `limnoria-2024.4.26/plugins/Limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Limiter/config.py` & `limnoria-2024.4.26/plugins/Limiter/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Limiter/locales/fi.po` & `limnoria-2024.4.26/plugins/Limiter/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Limiter/locales/fr.po` & `limnoria-2024.4.26/plugins/Limiter/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Limiter/locales/hu.po` & `limnoria-2024.4.26/plugins/Limiter/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Limiter/locales/it.po` & `limnoria-2024.4.26/plugins/Limiter/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Limiter/plugin.py` & `limnoria-2024.4.26/plugins/Limiter/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Limiter/test.py` & `limnoria-2024.4.26/plugins/Limiter/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/LogToIrc/__init__.py` & `limnoria-2024.4.26/plugins/LogToIrc/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/LogToIrc/config.py` & `limnoria-2024.4.26/plugins/LogToIrc/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/LogToIrc/handler.py` & `limnoria-2024.4.26/plugins/LogToIrc/handler.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/LogToIrc/plugin.py` & `limnoria-2024.4.26/plugins/LogToIrc/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/LogToIrc/test.py` & `limnoria-2024.4.26/plugins/LogToIrc/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Math/__init__.py` & `limnoria-2024.4.26/plugins/Math/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Math/config.py` & `limnoria-2024.4.26/plugins/Math/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Math/local/convertcore.py` & `limnoria-2024.4.26/plugins/Math/local/convertcore.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Math/locales/fi.po` & `limnoria-2024.4.26/plugins/Math/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Math/locales/fr.po` & `limnoria-2024.4.26/plugins/Math/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Math/locales/hu.po` & `limnoria-2024.4.26/plugins/Math/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Math/locales/it.po` & `limnoria-2024.4.26/plugins/Math/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Math/plugin.py` & `limnoria-2024.4.26/plugins/Math/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Math/test.py` & `limnoria-2024.4.26/plugins/Math/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MessageParser/__init__.py` & `limnoria-2024.4.26/plugins/MessageParser/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MessageParser/config.py` & `limnoria-2024.4.26/plugins/MessageParser/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MessageParser/locales/fi.po` & `limnoria-2024.4.26/plugins/MessageParser/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MessageParser/locales/fr.po` & `limnoria-2024.4.26/plugins/MessageParser/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MessageParser/locales/it.po` & `limnoria-2024.4.26/plugins/MessageParser/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MessageParser/plugin.py` & `limnoria-2024.4.26/plugins/MessageParser/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MessageParser/test.py` & `limnoria-2024.4.26/plugins/MessageParser/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Misc/__init__.py` & `limnoria-2024.4.26/plugins/Misc/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Misc/config.py` & `limnoria-2024.4.26/plugins/Misc/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Misc/locales/de.po` & `limnoria-2024.4.26/plugins/Misc/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Misc/locales/fi.po` & `limnoria-2024.4.26/plugins/Misc/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Misc/locales/fr.po` & `limnoria-2024.4.26/plugins/Misc/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Misc/locales/hu.po` & `limnoria-2024.4.26/plugins/Misc/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Misc/locales/it.po` & `limnoria-2024.4.26/plugins/Misc/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Misc/plugin.py` & `limnoria-2024.4.26/plugins/Misc/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Misc/test.py` & `limnoria-2024.4.26/plugins/Misc/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MoobotFactoids/__init__.py` & `limnoria-2024.4.26/plugins/MoobotFactoids/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MoobotFactoids/config.py` & `limnoria-2024.4.26/plugins/MoobotFactoids/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MoobotFactoids/locales/fi.po` & `limnoria-2024.4.26/plugins/MoobotFactoids/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MoobotFactoids/locales/fr.po` & `limnoria-2024.4.26/plugins/MoobotFactoids/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MoobotFactoids/locales/it.po` & `limnoria-2024.4.26/plugins/MoobotFactoids/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MoobotFactoids/plugin.py` & `limnoria-2024.4.26/plugins/MoobotFactoids/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/MoobotFactoids/test.py` & `limnoria-2024.4.26/plugins/MoobotFactoids/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Network/__init__.py` & `limnoria-2024.4.26/plugins/Network/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Network/config.py` & `limnoria-2024.4.26/plugins/Network/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Network/locales/de.po` & `limnoria-2024.4.26/plugins/Network/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Network/locales/fi.po` & `limnoria-2024.4.26/plugins/Network/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Network/locales/fr.po` & `limnoria-2024.4.26/plugins/Network/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Network/locales/it.po` & `limnoria-2024.4.26/plugins/Network/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Network/plugin.py` & `limnoria-2024.4.26/plugins/Network/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Network/test.py` & `limnoria-2024.4.26/plugins/Network/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/News/__init__.py` & `limnoria-2024.4.26/plugins/News/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/News/config.py` & `limnoria-2024.4.26/plugins/News/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/News/locales/fi.po` & `limnoria-2024.4.26/plugins/News/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/News/locales/fr.po` & `limnoria-2024.4.26/plugins/News/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/News/locales/it.po` & `limnoria-2024.4.26/plugins/News/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/News/plugin.py` & `limnoria-2024.4.26/plugins/News/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/News/test.py` & `limnoria-2024.4.26/plugins/News/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/NickAuth/__init__.py` & `limnoria-2024.4.26/plugins/NickAuth/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/NickAuth/config.py` & `limnoria-2024.4.26/plugins/NickAuth/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/NickAuth/locales/de.po` & `limnoria-2024.4.26/plugins/NickAuth/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/NickAuth/locales/fi.po` & `limnoria-2024.4.26/plugins/NickAuth/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/NickAuth/plugin.py` & `limnoria-2024.4.26/plugins/NickAuth/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/NickAuth/test.py` & `limnoria-2024.4.26/plugins/NickAuth/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/NickCapture/__init__.py` & `limnoria-2024.4.26/plugins/NickCapture/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/NickCapture/config.py` & `limnoria-2024.4.26/plugins/NickCapture/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/NickCapture/locales/de.po` & `limnoria-2024.4.26/plugins/NickCapture/locales/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 "    will check whether its nick ISON."
 msgstr ""
 "Legt fest wie oft (in Sekunden) der Bot checkt ob der Nick verfügbar ist."
 
 #: plugin.py:41
 msgid ""
 "This plugin constantly tries to take whatever nick is configured as\n"
-"    supybot.nick.  Just make sure that's set appropriately, and thus plugin\n"
+"    supybot.nick.  Just make sure that's set appropriately, and this plugin\n"
 "    will do the rest."
 msgstr ""
 "Dieses Plugin versucht dauernd den Nick der in supybot.nick konfiguriert ist "
 "zu bekommen. Stelle nur sicher das dieser richtig gesetzt wurde und das "
 "Plugin macht den Rest."
 
 #: plugin.py:106
```

### Comparing `limnoria-2023.9.24/plugins/NickCapture/locales/fi.po` & `limnoria-2024.4.26/plugins/NickCapture/locales/fi.po`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 msgstr ""
 "Määrittää kuinka usein (sekunteina) botti\n"
 "    tarkistaa nimimerkkinsä ISON komennolla."
 
 #: plugin.py:41
 msgid ""
 "This plugin constantly tries to take whatever nick is configured as\n"
-"    supybot.nick.  Just make sure that's set appropriately, and thus plugin\n"
+"    supybot.nick.  Just make sure that's set appropriately, and this plugin\n"
 "    will do the rest."
 msgstr ""
 "Tämä lisäosa yrittää jatkuvasti ottaa sen nimimerkin, joka on määritetty\n"
 "    asetusarvossa supybot.nick.  Tee vain varmaksi, että se on määritetty "
 "kunnolla\n"
 "    ja tämä lisäosa hoitaa loput."
```

### Comparing `limnoria-2023.9.24/plugins/NickCapture/locales/fr.po` & `limnoria-2024.4.26/plugins/NickCapture/locales/fr.po`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 msgstr ""
 "Détermine tous les combien de temps (en secondes) le bot vérifiera son nick "
 "via ISON"
 
 #: plugin.py:41
 msgid ""
 "This plugin constantly tries to take whatever nick is configured as\n"
-"    supybot.nick.  Just make sure that's set appropriately, and thus plugin\n"
+"    supybot.nick.  Just make sure that's set appropriately, and this plugin\n"
 "    will do the rest."
 msgstr ""
 "Ce plugin essaye constament de récupérer le nick configuré dans supybot."
 "nick. Assurez-vous de le configurer correctement, et ce plugin fera le reste."
 
 #: plugin.py:106
 msgid "This is returned by the ISON command."
```

### Comparing `limnoria-2023.9.24/plugins/NickCapture/locales/it.po` & `limnoria-2024.4.26/plugins/NickCapture/locales/it.po`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 "    will check whether its nick ISON."
 msgstr ""
 "Determina quanto spesso (in secondi) il bot controllerà il suo nick con ISON."
 
 #: plugin.py:41
 msgid ""
 "This plugin constantly tries to take whatever nick is configured as\n"
-"    supybot.nick.  Just make sure that's set appropriately, and thus plugin\n"
+"    supybot.nick.  Just make sure that's set appropriately, and this plugin\n"
 "    will do the rest."
 msgstr ""
 "Questo plugin cerca costantemente di ottenere qualsiasi nick sia impostato\n"
 "    come supybot.nick. Assicurati che questa sia configurata correttamente\n"
 "    e il plugin farà il resto."
 
 #: plugin.py:106
```

### Comparing `limnoria-2023.9.24/plugins/NickCapture/plugin.py` & `limnoria-2024.4.26/plugins/NickCapture/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 import supybot.ircutils as ircutils
 import supybot.callbacks as callbacks
 from supybot.i18n import PluginInternationalization, internationalizeDocstring
 _ = PluginInternationalization('NickCapture')
 
 class NickCapture(callbacks.Plugin):
     """This plugin constantly tries to take whatever nick is configured as
-    supybot.nick.  Just make sure that's set appropriately, and thus plugin
+    supybot.nick.  Just make sure that's set appropriately, and this plugin
     will do the rest."""
     public = False
     def __init__(self, irc):
         self.__parent = super(NickCapture, self)
         self.__parent.__init__(irc)
         self.lastIson = 0
         self.monitoring = []
```

### Comparing `limnoria-2023.9.24/plugins/NickCapture/test.py` & `limnoria-2024.4.26/plugins/NickCapture/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Nickometer/__init__.py` & `limnoria-2024.4.26/plugins/Nickometer/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Nickometer/config.py` & `limnoria-2024.4.26/plugins/Nickometer/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Nickometer/locales/fi.po` & `limnoria-2024.4.26/plugins/Nickometer/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Nickometer/locales/fr.po` & `limnoria-2024.4.26/plugins/Nickometer/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Nickometer/locales/it.po` & `limnoria-2024.4.26/plugins/Nickometer/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Nickometer/plugin.py` & `limnoria-2024.4.26/plugins/Nickometer/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Nickometer/test.py` & `limnoria-2024.4.26/plugins/Nickometer/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Note/__init__.py` & `limnoria-2024.4.26/plugins/Note/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Note/config.py` & `limnoria-2024.4.26/plugins/Note/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Note/locales/fi.po` & `limnoria-2024.4.26/plugins/Note/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Note/locales/fr.po` & `limnoria-2024.4.26/plugins/Note/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Note/locales/it.po` & `limnoria-2024.4.26/plugins/Note/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Note/plugin.py` & `limnoria-2024.4.26/plugins/Note/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Note/test.py` & `limnoria-2024.4.26/plugins/Note/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Owner/__init__.py` & `limnoria-2024.4.26/plugins/Owner/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Owner/config.py` & `limnoria-2024.4.26/plugins/Owner/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Owner/locales/de.po` & `limnoria-2024.4.26/plugins/Owner/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Owner/locales/fi.po` & `limnoria-2024.4.26/plugins/Owner/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Owner/locales/fr.po` & `limnoria-2024.4.26/plugins/Owner/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Owner/locales/hu.po` & `limnoria-2024.4.26/plugins/Owner/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Owner/locales/it.po` & `limnoria-2024.4.26/plugins/Owner/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Owner/plugin.py` & `limnoria-2024.4.26/plugins/Owner/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Owner/test.py` & `limnoria-2024.4.26/plugins/Owner/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Plugin/__init__.py` & `limnoria-2024.4.26/plugins/Plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Plugin/config.py` & `limnoria-2024.4.26/plugins/Plugin/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Plugin/locales/de.po` & `limnoria-2024.4.26/plugins/Plugin/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Plugin/locales/fi.po` & `limnoria-2024.4.26/plugins/Plugin/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Plugin/locales/fr.po` & `limnoria-2024.4.26/plugins/Plugin/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Plugin/locales/it.po` & `limnoria-2024.4.26/plugins/Plugin/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Plugin/plugin.py` & `limnoria-2024.4.26/plugins/Plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Plugin/test.py` & `limnoria-2024.4.26/plugins/Plugin/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/PluginDownloader/__init__.py` & `limnoria-2024.4.26/plugins/PluginDownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/PluginDownloader/config.py` & `limnoria-2024.4.26/plugins/PluginDownloader/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/PluginDownloader/locales/de.po` & `limnoria-2024.4.26/plugins/PluginDownloader/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/PluginDownloader/locales/fi.po` & `limnoria-2024.4.26/plugins/PluginDownloader/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/PluginDownloader/locales/fr.po` & `limnoria-2024.4.26/plugins/PluginDownloader/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/PluginDownloader/locales/it.po` & `limnoria-2024.4.26/plugins/PluginDownloader/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/PluginDownloader/plugin.py` & `limnoria-2024.4.26/plugins/PluginDownloader/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/PluginDownloader/test.py` & `limnoria-2024.4.26/plugins/PluginDownloader/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Poll/__init__.py` & `limnoria-2024.4.26/plugins/Poll/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Poll/config.py` & `limnoria-2024.4.26/plugins/Poll/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Poll/plugin.py` & `limnoria-2024.4.26/plugins/Poll/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Poll/test.py` & `limnoria-2024.4.26/plugins/Poll/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Praise/__init__.py` & `limnoria-2024.4.26/plugins/Praise/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Praise/config.py` & `limnoria-2024.4.26/plugins/Praise/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Praise/locales/fi.po` & `limnoria-2024.4.26/plugins/Praise/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Praise/locales/fr.po` & `limnoria-2024.4.26/plugins/Praise/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Praise/locales/it.po` & `limnoria-2024.4.26/plugins/Praise/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Praise/plugin.py` & `limnoria-2024.4.26/plugins/Praise/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Praise/test.py` & `limnoria-2024.4.26/plugins/Praise/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Protector/__init__.py` & `limnoria-2024.4.26/plugins/Protector/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Protector/config.py` & `limnoria-2024.4.26/plugins/Protector/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Protector/locales/fi.po` & `limnoria-2024.4.26/plugins/Protector/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Protector/locales/fr.po` & `limnoria-2024.4.26/plugins/Protector/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Protector/locales/it.po` & `limnoria-2024.4.26/plugins/Protector/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Protector/plugin.py` & `limnoria-2024.4.26/plugins/Protector/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Protector/test.py` & `limnoria-2024.4.26/plugins/Protector/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Quote/__init__.py` & `limnoria-2024.4.26/plugins/Quote/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Quote/config.py` & `limnoria-2024.4.26/plugins/Quote/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Quote/locales/fi.po` & `limnoria-2024.4.26/plugins/Quote/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Quote/locales/fr.po` & `limnoria-2024.4.26/plugins/Quote/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Quote/locales/it.po` & `limnoria-2024.4.26/plugins/Quote/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Quote/plugin.py` & `limnoria-2024.4.26/plugins/Quote/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Quote/test.py` & `limnoria-2024.4.26/plugins/Quote/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/QuoteGrabs/__init__.py` & `limnoria-2024.4.26/plugins/QuoteGrabs/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/QuoteGrabs/config.py` & `limnoria-2024.4.26/plugins/QuoteGrabs/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/QuoteGrabs/locales/fi.po` & `limnoria-2024.4.26/plugins/QuoteGrabs/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/QuoteGrabs/locales/fr.po` & `limnoria-2024.4.26/plugins/QuoteGrabs/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/QuoteGrabs/locales/it.po` & `limnoria-2024.4.26/plugins/QuoteGrabs/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/QuoteGrabs/plugin.py` & `limnoria-2024.4.26/plugins/QuoteGrabs/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/QuoteGrabs/test.py` & `limnoria-2024.4.26/plugins/QuoteGrabs/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/RSS/__init__.py` & `limnoria-2024.4.26/plugins/RSS/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,16 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 ###
 
 """
 Provides basic functionality for handling RSS/RDF feeds, and allows announcing
 them periodically to channels.
-In order to use this plugin you must have the following modules
-installed:
-* feedparser: http://feedparser.org/
+In order to use this plugin you must have `python3-feedparser
+<https://pypi.org/project/feedparser/>`_ installed.
 """
 
 import supybot
 import supybot.world as world
 
 # Use this for the version of this plugin.  You may wish to put a CVS keyword
 # in here if you're keeping the plugin in CVS or some similar system.
```

### Comparing `limnoria-2023.9.24/plugins/RSS/config.py` & `limnoria-2024.4.26/plugins/RSS/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/RSS/locales/de.po` & `limnoria-2024.4.26/plugins/RSS/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/RSS/locales/fi.po` & `limnoria-2024.4.26/plugins/RSS/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/RSS/locales/fr.po` & `limnoria-2024.4.26/plugins/RSS/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/RSS/locales/hu.po` & `limnoria-2024.4.26/plugins/RSS/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/RSS/locales/it.po` & `limnoria-2024.4.26/plugins/RSS/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/RSS/plugin.py` & `limnoria-2024.4.26/plugins/RSS/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -360,14 +360,19 @@
                 d = feedparser.parse(feed.url, etag=feed.etag,
                         modified=feed.modified, handlers=handlers)
             except socket.error as e:
                 self.log.warning("Network error while fetching <%s>: %s",
                                feed.url, e)
                 feed.last_exception = e
                 return
+            except http.client.HTTPException as e:
+                self.log.warning("HTTP error while fetching <%s>: %s",
+                               feed.url, e)
+                feed.last_exception = e
+                return
             except Exception as e:
                 self.log.error("Failed to fetch <%s>: %s", feed.url, e)
                 raise  # reraise so @log.firewall prints the traceback
             if 'status' not in d or d.status != 304: # Not modified
                 if 'etag' in d:
                     feed.etag = d.etag
                 if 'modified' in d:
@@ -493,14 +498,56 @@
             template = self.registryValue(key_name, channel, network)
         date = entry.get('published_parsed')
         date = utils.str.timestamp(date)
         kwargs = {"feed_%s" % k: v for (k, v) in feed.data.items() if
                   isinstance(v, str)}
         kwargs["feed_name"] = feed.name
         kwargs.update(entry)
+        for (key, value) in list(kwargs.items()):
+            # First look for plain text
+            if isinstance(value, list):
+                for item in value:
+                    if isinstance(item, dict) and 'value' in item and \
+                            item.get('type') == 'text/plain':
+                        value = item['value']
+                        break
+            # Then look for HTML text or URL
+            if isinstance(value, list):
+                for item in value:
+                    if isinstance(item, dict) and item.get('type') in \
+                            ('text/html', 'application/xhtml+xml'):
+                        if 'value' in item:
+                            value = utils.web.htmlToText(item['value'])
+                        elif 'href' in item:
+                            value = item['href']
+            # Then fall back to any URL
+            if isinstance(value, list):
+                for item in value:
+                    if isinstance(item, dict) and 'href' in item:
+                        value = item['href']
+                        break
+            # Finally, as a last resort, use the value as-is
+            if isinstance(value, list):
+                for item in value:
+                    if isinstance(item, dict) and 'value' in item:
+                        value = item['value']
+            kwargs[key] = value
+
+        for key in ('summary', 'title'):
+            detail = kwargs.get('%s_detail' % key)
+            if isinstance(detail, dict) and detail.get('type') in \
+                    ('text/html', 'application/xhtml+xml'):
+                kwargs[key] = utils.web.htmlToText(detail['value'])
+
+                if 'description' not in kwargs and kwargs[key]:
+                    kwargs['description'] = kwargs[key]
+
+        if 'description' not in kwargs and kwargs.get('content'):
+            kwargs['description'] = kwargs['content']
+
         s = string.Template(template).safe_substitute(entry, **kwargs, date=date)
         return self._normalize_entry(s)
 
     def announce_entry(self, irc, channel, feed, entry):
         if self.should_send_entry(irc.network, channel, entry):
             s = self.format_entry(irc.network, channel, feed, entry, True)
             if self.registryValue('notice', channel, irc.network):
```

### Comparing `limnoria-2023.9.24/plugins/RSS/test.py` & `limnoria-2024.4.26/plugins/RSS/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 	<link>http://example.com/</link>
 	<description>this dummy feed has no elements</description>
 	<language>en</language>
 </channel>
 </rss>
 """
 
-
 class MockResponse:
     headers = {}
     url = ''
     def read(self):
         return self._data.encode()
 
     def close(self):
@@ -356,14 +355,138 @@
         timeFastForward(1.1)
         with conf.supybot.plugins.RSS.format.context('$description'):
             mock._data = xkcd_new
             self.assertRegexp('rss http://xkcd.com/rss.xml',
                     'On the other hand, the refractor\'s')
 
     @mock_urllib
+    def testAtomContentHtmlOnly(self, mock):
+        timeFastForward(1.1)
+        mock._data = """
+<?xml version="1.0" encoding="UTF-8"?>
+<feed xmlns="http://www.w3.org/2005/Atom" xmlns:media="http://search.yahoo.com/mrss/" xml:lang="en-US">
+  <title>Recent Commits to anope:2.0</title>
+  <updated>2023-10-04T16:14:39Z</updated>
+  <entry>
+    <title>title with &lt;pre&gt;HTML&lt;/pre&gt;</title>
+    <updated>2023-10-04T16:14:39Z</updated>
+    <content type="html">
+      content with &lt;pre&gt;HTML&lt;/pre&gt;
+    </content>
+  </entry>
+</feed>"""
+        with conf.supybot.plugins.RSS.format.context('$content'):
+            self.assertRegexp('rss https://example.org',
+                    'content with HTML')
+        with conf.supybot.plugins.RSS.format.context('$description'):
+            self.assertRegexp('rss https://example.org',
+                    'content with HTML')
+
+    @mock_urllib
+    def testAtomContentXhtmlOnly(self, mock):
+        timeFastForward(1.1)
+        mock._data = """
+<?xml version="1.0" encoding="UTF-8"?>
+<feed xmlns="http://www.w3.org/2005/Atom" xmlns:media="http://search.yahoo.com/mrss/" xml:lang="en-US">
+  <title>Recent Commits to anope:2.0</title>
+  <updated>2023-10-04T16:14:39Z</updated>
+  <entry>
+    <title>title with &lt;pre&gt;HTML&lt;/pre&gt;</title>
+    <updated>2023-10-04T16:14:39Z</updated>
+    <content type="xhtml">
+      <div xmlns="http://www.w3.org/1999/xhtml">
+        content with <pre>XHTML</pre>
+      </div>
+    </content>
+  </entry>
+</feed>"""
+        with conf.supybot.plugins.RSS.format.context('$content'):
+            self.assertRegexp('rss https://example.org',
+                    'content with XHTML')
+        with conf.supybot.plugins.RSS.format.context('$description'):
+            self.assertRegexp('rss https://example.org',
+                    'content with XHTML')
+
+    @mock_urllib
+    def testAtomContentHtmlAndPlaintext(self, mock):
+        timeFastForward(1.1)
+        mock._data = """
+<?xml version="1.0" encoding="UTF-8"?>
+<feed xmlns="http://www.w3.org/2005/Atom" xmlns:media="http://search.yahoo.com/mrss/" xml:lang="en-US">
+  <title>Recent Commits to anope:2.0</title>
+  <updated>2023-10-04T16:14:39Z</updated>
+  <entry>
+    <title>title with &lt;pre&gt;HTML&lt;/pre&gt;</title>
+    <updated>2023-10-04T16:14:39Z</updated>
+    <!-- Atom spec says multiple contents is invalid, feedparser says it's not.
+         I like having the option, so let's make sure we support it. -->
+    <content type="html">
+      content with &lt;pre&gt;HTML&lt;/pre&gt;
+    </content>
+    <content type="text">
+      content with plaintext
+    </content>
+  </entry>
+</feed>"""
+        with conf.supybot.plugins.RSS.format.context('$content'):
+            self.assertRegexp('rss https://example.org',
+                    'content with plaintext')
+        with conf.supybot.plugins.RSS.format.context('$description'):
+            self.assertRegexp('rss https://example.org',
+                    'content with plaintext')
+
+    @mock_urllib
+    def testAtomContentPlaintextAndHtml(self, mock):
+        timeFastForward(1.1)
+        mock._data = """
+<?xml version="1.0" encoding="UTF-8"?>
+<feed xmlns="http://www.w3.org/2005/Atom" xmlns:media="http://search.yahoo.com/mrss/" xml:lang="en-US">
+  <title>Recent Commits to anope:2.0</title>
+  <updated>2023-10-04T16:14:39Z</updated>
+  <entry>
+    <title>title with &lt;pre&gt;HTML&lt;/pre&gt;</title>
+    <updated>2023-10-04T16:14:39Z</updated>
+    <!-- Atom spec says multiple contents is invalid, feedparser says it's not.
+         I like having the option, so let's make sure we support it. -->
+    <content type="text">
+      content with plaintext
+    </content>
+    <content type="html">
+      content with &lt;pre&gt;HTML&lt;/pre&gt;
+    </content>
+  </entry>
+</feed>"""
+        with conf.supybot.plugins.RSS.format.context('$content'):
+            self.assertRegexp('rss https://example.org',
+                    'content with plaintext')
+        with conf.supybot.plugins.RSS.format.context('$description'):
+            self.assertRegexp('rss https://example.org',
+                    'content with plaintext')
+
+    @mock_urllib
+    def testRssDescriptionHtml(self, mock):
+        timeFastForward(1.1)
+        mock._data = """
+<?xml version="1.0" encoding="utf-8"?>
+<rss xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:atom="http://www.w3.org/2005/Atom" xmlns:content="http://purl.org/rss/1.0/modules/content/" xmlns:foaf="http://xmlns.com/foaf/0.1/" xmlns:og="http://ogp.me/ns#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:schema="http://schema.org/" xmlns:sioc="http://rdfs.org/sioc/ns#" xmlns:sioct="http://rdfs.org/sioc/types#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" version="2.0">
+  <channel>
+    <title>feed title</title>
+    <description/>
+    <language>en</language>
+    <item>
+    <title>title with &lt;pre&gt;HTML&lt;/pre&gt;</title>
+    <description>description with &lt;pre&gt;HTML&lt;/pre&gt;</description>
+    </item>
+  </channel>
+</feed>"""
+        with conf.supybot.plugins.RSS.format.context('$description'):
+            self.assertRegexp('rss https://example.org',
+                    'description with HTML')
+
+    @mock_urllib
     def testFeedAttribute(self, mock):
         timeFastForward(1.1)
         with conf.supybot.plugins.RSS.format.context('$feed_title: $title'):
             mock._data = xkcd_new
             self.assertRegexp('rss http://xkcd.com/rss.xml',
                               r'xkcd\.com: Telescopes')
```

### Comparing `limnoria-2023.9.24/plugins/Relay/__init__.py` & `limnoria-2024.4.26/plugins/Relay/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Relay/config.py` & `limnoria-2024.4.26/plugins/Relay/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Relay/locales/fi.po` & `limnoria-2024.4.26/plugins/Relay/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Relay/locales/fr.po` & `limnoria-2024.4.26/plugins/Relay/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Relay/locales/it.po` & `limnoria-2024.4.26/plugins/Relay/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Relay/plugin.py` & `limnoria-2024.4.26/plugins/Relay/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Relay/test.py` & `limnoria-2024.4.26/plugins/Relay/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Reply/__init__.py` & `limnoria-2024.4.26/plugins/Reply/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Reply/config.py` & `limnoria-2024.4.26/plugins/Reply/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Reply/locales/de.po` & `limnoria-2024.4.26/plugins/Reply/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Reply/locales/fi.po` & `limnoria-2024.4.26/plugins/Reply/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Reply/locales/fr.po` & `limnoria-2024.4.26/plugins/Reply/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Reply/locales/hu.po` & `limnoria-2024.4.26/plugins/Reply/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Reply/locales/it.po` & `limnoria-2024.4.26/plugins/Reply/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Reply/plugin.py` & `limnoria-2024.4.26/plugins/Reply/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Reply/test.py` & `limnoria-2024.4.26/plugins/Reply/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Scheduler/__init__.py` & `limnoria-2024.4.26/plugins/Scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Scheduler/config.py` & `limnoria-2024.4.26/plugins/Scheduler/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Scheduler/locales/fi.po` & `limnoria-2024.4.26/plugins/Scheduler/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Scheduler/locales/fr.po` & `limnoria-2024.4.26/plugins/Scheduler/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Scheduler/locales/it.po` & `limnoria-2024.4.26/plugins/Scheduler/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Scheduler/plugin.py` & `limnoria-2024.4.26/plugins/Scheduler/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Scheduler/test.py` & `limnoria-2024.4.26/plugins/Scheduler/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/SedRegex/__init__.py` & `limnoria-2024.4.26/plugins/SedRegex/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/SedRegex/config.py` & `limnoria-2024.4.26/plugins/SedRegex/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/SedRegex/constants.py` & `limnoria-2024.4.26/plugins/SedRegex/constants.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/SedRegex/plugin.py` & `limnoria-2024.4.26/plugins/SedRegex/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/SedRegex/test.py` & `limnoria-2024.4.26/plugins/SedRegex/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Seen/__init__.py` & `limnoria-2024.4.26/plugins/Seen/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Seen/config.py` & `limnoria-2024.4.26/plugins/Seen/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Seen/locales/de.po` & `limnoria-2024.4.26/plugins/Seen/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Seen/locales/fi.po` & `limnoria-2024.4.26/plugins/Seen/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Seen/locales/fr.po` & `limnoria-2024.4.26/plugins/Seen/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Seen/locales/it.po` & `limnoria-2024.4.26/plugins/Seen/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Seen/plugin.py` & `limnoria-2024.4.26/plugins/Seen/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -191,33 +191,45 @@
                             Raise=True)
                 results = db.seenWildcard(channel, name)
             else:
                 results = [[name, db.seen(channel, name)]]
             if len(results) == 1:
                 (nick, info) = results[0]
                 (when, said) = info
-                reply = format(_('%s was last seen in %s %s ago'),
-                                 nick, channel,
-                                 utils.timeElapsed(time.time()-when))
+                if nick in irc.state.channels[channel].users:
+                    reply = format(_('%s was last seen in %s %s ago, and is in the channel now'),
+                                     nick, channel,
+                                     utils.timeElapsed(time.time()-when))
+                else:
+                    reply = format(_('%s was last seen in %s %s ago'),
+                                     nick, channel,
+                                     utils.timeElapsed(time.time()-when))
                 if self.registryValue('showLastMessage', channel, irc.network):
                     if minisix.PY2:
                         said = said.decode('utf8')
                     reply = _('%s: %s') % (reply, said)
                 irc.reply(reply)
             elif len(results) > 1:
                 L = []
                 for (nick, info) in results:
                     (when, said) = info
-                    L.append(format(_('%s (%s ago)'), nick,
-                                    utils.timeElapsed(time.time()-when)))
+                    if nick in irc.state.channels[channel].users:
+                        L.append(format(_('%s (%s ago, and is in the channel now)'), nick,
+                                        utils.timeElapsed(time.time()-when)))
+                    else:
+                        L.append(format(_('%s (%s ago)'), nick,
+                                        utils.timeElapsed(time.time()-when)))
                 irc.reply(format(_('%s could be %L'), name, (L, _('or'))))
             else:
                 irc.reply(format(_('I haven\'t seen anyone matching %s.'), name))
         except KeyError:
-            irc.reply(format(_('I have not seen %s.'), name))
+            if name in irc.state.channels[channel].users:
+                irc.reply(format(_("%s is in the channel right now."), name))
+            else:
+                irc.reply(format(_('I have not seen %s.'), name))
 
     def _checkChannelPresence(self, irc, channel, target, you):
         if channel not in irc.state.channels:
             irc.error(_("I'm not in %s." % channel), Raise=True)
         if target not in irc.state.channels[channel].users:
             if you:
                 msg = format(_('You must be in %s to use this command.'), channel)
@@ -273,16 +285,21 @@
     def _last(self, irc, channel, any=False):
         if any:
             db = self.anydb
         else:
             db = self.db
         try:
             (when, said) = db.seen(channel, '<last>')
-            reply = format(_('Someone was last seen in %s %s ago'),
-                             channel, utils.timeElapsed(time.time()-when))
+            pattern = r'<(.*?)>'
+            match = re.search(pattern, said)
+            if not match:
+                irc.error(format(_('I couldn\'t parse the nick of the speaker of the last line.')), Raise=True)
+            nick = match.group(1)
+            reply = format(_('Last seen in %s was %s, %s ago'),
+                 channel, nick, utils.timeElapsed(time.time()-when))
             if self.registryValue('showLastMessage', channel, irc.network):
                 reply = _('%s: %s') % (reply, said)
             irc.reply(reply)
         except KeyError:
             irc.reply(_('I have never seen anyone.'))
 
     @internationalizeDocstring
@@ -299,22 +316,30 @@
     def _user(self, irc, channel, user, any=False):
         if any:
             db = self.anydb
         else:
             db = self.db
         try:
             (when, said) = db.seen(channel, user.id)
-            reply = format(_('%s was last seen in %s %s ago'),
-                             user.name, channel,
-                             utils.timeElapsed(time.time()-when))
+            if user.name in irc.state.channels[channel].users:
+                reply = format(_('%s was last seen in %s %s ago and is in the channel now'),
+                                 user.name, channel,
+                                 utils.timeElapsed(time.time()-when))
+            else:
+                reply = format(_('%s was last seen in %s %s ago'),
+                                 user.name, channel,
+                                 utils.timeElapsed(time.time()-when))
             if self.registryValue('showLastMessage', channel, irc.network):
                 reply = _('%s: %s') % (reply, said)
             irc.reply(reply)
         except KeyError:
-            irc.reply(format(_('I have not seen %s.'), user.name))
+            if user.name in irc.state.channels[channel].users:
+                irc.reply(format(_("%s is in the channel right now."), user.name))
+            else:
+                irc.reply(format(_('I have not seen %s.'), user.name))
 
     @internationalizeDocstring
     def user(self, irc, msg, args, channel, user):
         """[<channel>] <name>
 
         Returns the last time <name> was seen and what <name> was last seen
         saying.  This looks up <name> in the user seen database, which means
```

### Comparing `limnoria-2023.9.24/plugins/Seen/test.py` & `limnoria-2024.4.26/plugins/Seen/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,32 +79,52 @@
 
     def testSeen(self):
         self.irc.feedMsg(ircmsgs.join(self.channel, self.irc.nick,
                                          prefix=self.prefix))
         self.assertNotError('seen last')
         self.assertNotError('list')
         self.assertNotError('config plugins.Seen.minimumNonWildcard 2')
-        self.assertError('seen *')
-        self.assertNotError('seen %s' % self.nick)
-        m = self.assertNotError('seen %s' % self.nick.upper())
-        self.assertIn(self.nick.upper(), m.args[1])
         self.assertRegexp('seen user %s' % self.nick,
                           '^%s was last seen' % self.nick)
+        self.assertError('seen *')
+        self.assertNotError('seen %s' % self.nick)
         self.assertNotError('config plugins.Seen.minimumNonWildcard 0')
         orig = conf.supybot.protocols.irc.strictRfc()
         try:
             for state in (True, False):
                 conf.supybot.protocols.irc.strictRfc.setValue(state)
                 for wildcard in self.wildcardTest:
                     self.assertRegexp('seen %s' % wildcard,
                                       '^%s was last seen' % self.nick)
                 self.assertRegexp('seen bar*', '^I haven\'t seen anyone matching')
         finally:
             conf.supybot.protocols.irc.strictRfc.setValue(orig)
 
+
+    def testSeenNickInChannel(self):
+        # Test case: 'seen' with a nick (user in channel)
+        self.irc.feedMsg(ircmsgs.join(self.channel, self.irc.nick,
+                                         prefix=self.prefix))
+        self.assertRegexp('seen %s' % self.nick, 'is in the channel right now')
+        m = self.assertNotError('seen %s' % self.nick.upper())
+        self.assertIn(self.nick.upper(), m.args[1])
+
+    def testSeenUserInChannel(self):
+        # Test case: 'seen' with a user (user in channel)
+        self.irc.feedMsg(ircmsgs.join(self.channel, self.irc.nick,
+                                         prefix=self.prefix))
+        self.assertRegexp('seen user %s' % self.nick, 'is in the channel right now')
+
+    def testSeenNickNotInChannel(self):
+        # Test case: 'seen' with a nick (user not in channel)
+        testnick = "user123"
+        self.irc.feedMsg(ircmsgs.join(self.channel, testnick, "user123!baz"))
+        self.irc.feedMsg(ircmsgs.part(self.channel, prefix="user123!baz"))
+        self.assertNotRegexp("seen %s" % testnick, "is in the channel right now")
+
     def testSeenNoUser(self):
         self.irc.feedMsg(ircmsgs.join(self.channel, self.irc.nick,
                                          prefix=self.prefix))
         self.assertNotRegexp('seen user alsdkfjalsdfkj', 'KeyError')
 
 
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2023.9.24/plugins/Services/__init__.py` & `limnoria-2024.4.26/plugins/Services/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Services/config.py` & `limnoria-2024.4.26/plugins/Services/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Services/locales/de.po` & `limnoria-2024.4.26/plugins/Services/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Services/locales/fi.po` & `limnoria-2024.4.26/plugins/Services/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Services/locales/fr.po` & `limnoria-2024.4.26/plugins/Services/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Services/locales/it.po` & `limnoria-2024.4.26/plugins/Services/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Services/plugin.py` & `limnoria-2024.4.26/plugins/Services/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,17 +120,19 @@
             return
         if nick is None:
             nick = self._getNick(irc.network)
         if nick not in self.registryValue('nicks', network=irc.network):
             return
         nickserv = self.registryValue('NickServ', network=irc.network)
         password = self._getNickServPassword(nick, irc.network)
-        if not nickserv or not password:
-            s = 'Tried to identify without a NickServ or password set.'
-            self.log.warning(s)
+        if not nickserv:
+            self.log.warning('Tried to identify without a NickServ set.')
+            return
+        if not password:
+            self.log.warning('Tried to identify without a password set.')
             return
         assert ircutils.strEqual(irc.nick, nick), \
                'Identifying with not normal nick.'
         self.log.info('Sending identify (current nick: %s)', irc.nick)
         identify = 'IDENTIFY %s' % password
         # It's important that this next statement is irc.sendMsg, not
         # irc.queueMsg.  We want this message to get through before any
@@ -146,24 +148,23 @@
         if nick not in self.registryValue('nicks', network=irc.network):
             return
         nickserv = self.registryValue('NickServ', network=irc.network)
         password = self._getNickServPassword(nick, irc.network)
         ghostDelay = self.registryValue('ghostDelay', network=irc.network)
         if not ghostDelay:
             return
-        if not nickserv or not password:
-            s = 'Tried to ghost without a NickServ or password set.'
-            self.log.warning(s)
+        if not nickserv:
+            self.log.warning('Tried to ghost without a NickServ set.')
+            return
+        if not password:
+            self.log.warning('Tried to ghost without a password set.')
             return
         if state.sentGhost and time.time() < (state.sentGhost + ghostDelay):
             self.log.warning('Refusing to send GHOST more than once every '
                              '%s seconds.' % ghostDelay)
-        elif not password:
-            self.log.warning('Not ghosting: no password set.')
-            return
         else:
             self.log.info('Sending ghost (current nick: %s; ghosting: %s)',
                           irc.nick, nick)
             ghostCommand = self.registryValue('ghostCommand', network=irc.network)
             ghost = '%s %s %s' % (ghostCommand, nick, password)
             # Ditto about the sendMsg (see _doIdentify).
             irc.sendMsg(ircmsgs.privmsg(nickserv, ghost))
```

### Comparing `limnoria-2023.9.24/plugins/Services/test.py` & `limnoria-2024.4.26/plugins/Services/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ShrinkUrl/__init__.py` & `limnoria-2024.4.26/plugins/ShrinkUrl/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ShrinkUrl/config.py` & `limnoria-2024.4.26/plugins/ShrinkUrl/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ShrinkUrl/locales/fi.po` & `limnoria-2024.4.26/plugins/ShrinkUrl/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ShrinkUrl/locales/fr.po` & `limnoria-2024.4.26/plugins/ShrinkUrl/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ShrinkUrl/locales/it.po` & `limnoria-2024.4.26/plugins/ShrinkUrl/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ShrinkUrl/plugin.py` & `limnoria-2024.4.26/plugins/ShrinkUrl/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/ShrinkUrl/test.py` & `limnoria-2024.4.26/plugins/ShrinkUrl/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Status/__init__.py` & `limnoria-2024.4.26/plugins/Status/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Status/config.py` & `limnoria-2024.4.26/plugins/Status/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Status/locales/de.po` & `limnoria-2024.4.26/plugins/Status/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Status/locales/fi.po` & `limnoria-2024.4.26/plugins/Status/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Status/locales/fr.po` & `limnoria-2024.4.26/plugins/Status/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Status/locales/it.po` & `limnoria-2024.4.26/plugins/Status/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Status/plugin.py` & `limnoria-2024.4.26/plugins/Status/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,25 +72,61 @@
 
     @internationalizeDocstring
     def status(self, irc, msg, args):
         """takes no arguments
 
         Returns the status of the bot.
         """
+        # Initialize dictionaries 
+        nicks = {}
         networks = {}
+        # Iterate through each IRC network
         for Irc in world.ircs:
-            networks.setdefault(Irc.network, []).append(Irc.nick)
-        networks = sorted(networks.items())
-        networks = [format(_('%s as %L'), net, nicks) for (net,nicks) in networks]
-        L = [format(_('I am connected to %L.'), networks)]
+            network_name = Irc.network
+            channels = Irc.state.channels
+    
+            # Initialize counts for this network
+            channel_counts = len(channels)
+            op_counts = sum(1 for channel in channels.values() if Irc.nick in channel.ops)
+            halfop_counts = sum(1 for channel in channels.values() if Irc.nick in channel.halfops)
+            voice_counts = sum(1 for channel in channels.values() if Irc.nick in channel.voices)
+            normal_counts = sum(1 for channel in channels.values() if Irc.nick in channel.users)
+    
+            # Store the counts in dictionaries
+            nicks[network_name] = Irc.nick
+            networks[network_name] = {
+                'Channels': channel_counts,
+                'Ops': op_counts,
+                'Half-Ops': halfop_counts,
+                'Voiced': voice_counts,
+                'Regular': normal_counts
+            }
+    
+        # Prepare the response
+        response_lines = []
+        for network_name, counts in networks.items():
+            response_lines.append(
+                format(
+                    _('I am connected to %s as %s: Channels: %s, Ops: %s, Half-Ops: %s, Voiced: %s, Regular: %s'),
+                    network_name,
+                    nicks[network_name],
+                    counts['Channels'],
+                    counts['Ops'],
+                    counts['Half-Ops'],
+                    counts['Voiced'],
+                    counts['Regular']
+                )
+            )
+    
         if world.profiling:
-            L.append(_('I am currently in code profiling mode.'))
-        irc.reply('  '.join(L))
+            response_lines.append(_('I am currently in code profiling mode.'))
+        response = format(_("%L"), response_lines)
+        irc.reply(response)
     status = wrap(status)
-
+   
     @internationalizeDocstring
     def threads(self, irc, msg, args):
         """takes no arguments
 
         Returns the current threads that are active.
         """
         threads = [t.getName() for t in threading.enumerate()]
```

### Comparing `limnoria-2023.9.24/plugins/Status/test.py` & `limnoria-2024.4.26/plugins/Status/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/String/__init__.py` & `limnoria-2024.4.26/plugins/String/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/String/config.py` & `limnoria-2024.4.26/plugins/String/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/String/locales/fi.po` & `limnoria-2024.4.26/plugins/String/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/String/locales/fr.po` & `limnoria-2024.4.26/plugins/String/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/String/locales/it.po` & `limnoria-2024.4.26/plugins/String/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/String/plugin.py` & `limnoria-2024.4.26/plugins/String/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/String/test.py` & `limnoria-2024.4.26/plugins/String/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Success/__init__.py` & `limnoria-2024.4.26/plugins/Success/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Success/config.py` & `limnoria-2024.4.26/plugins/Success/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Success/locales/fi.po` & `limnoria-2024.4.26/plugins/Success/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Success/locales/fr.po` & `limnoria-2024.4.26/plugins/Success/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Success/locales/it.po` & `limnoria-2024.4.26/plugins/Success/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Success/plugin.py` & `limnoria-2024.4.26/plugins/Success/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Success/test.py` & `limnoria-2024.4.26/plugins/Success/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Time/__init__.py` & `limnoria-2024.4.26/plugins/Time/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Time/config.py` & `limnoria-2024.4.26/plugins/Time/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Time/locales/de.po` & `limnoria-2024.4.26/plugins/Time/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Time/locales/fi.po` & `limnoria-2024.4.26/plugins/Time/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Time/locales/fr.po` & `limnoria-2024.4.26/plugins/Time/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Time/locales/hu.po` & `limnoria-2024.4.26/plugins/Time/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Time/locales/it.po` & `limnoria-2024.4.26/plugins/Time/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Time/plugin.py` & `limnoria-2024.4.26/plugins/Time/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Time/test.py` & `limnoria-2024.4.26/plugins/Time/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Todo/__init__.py` & `limnoria-2024.4.26/plugins/Todo/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Todo/config.py` & `limnoria-2024.4.26/plugins/Todo/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Todo/locales/de.po` & `limnoria-2024.4.26/plugins/Todo/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Todo/locales/fi.po` & `limnoria-2024.4.26/plugins/Todo/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Todo/locales/fr.po` & `limnoria-2024.4.26/plugins/Todo/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Todo/locales/it.po` & `limnoria-2024.4.26/plugins/Todo/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Todo/plugin.py` & `limnoria-2024.4.26/plugins/Todo/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Todo/test.py` & `limnoria-2024.4.26/plugins/Todo/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Topic/__init__.py` & `limnoria-2024.4.26/plugins/Topic/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Topic/config.py` & `limnoria-2024.4.26/plugins/Topic/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Topic/locales/fi.po` & `limnoria-2024.4.26/plugins/Topic/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Topic/locales/fr.po` & `limnoria-2024.4.26/plugins/Topic/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Topic/locales/it.po` & `limnoria-2024.4.26/plugins/Topic/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Topic/plugin.py` & `limnoria-2024.4.26/plugins/Topic/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Topic/test.py` & `limnoria-2024.4.26/plugins/Topic/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/URL/__init__.py` & `limnoria-2024.4.26/plugins/URL/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/URL/config.py` & `limnoria-2024.4.26/plugins/URL/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/URL/locales/fi.po` & `limnoria-2024.4.26/plugins/URL/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/URL/locales/fr.po` & `limnoria-2024.4.26/plugins/URL/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/URL/locales/it.po` & `limnoria-2024.4.26/plugins/URL/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/URL/plugin.py` & `limnoria-2024.4.26/plugins/URL/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/URL/test.py` & `limnoria-2024.4.26/plugins/URL/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Unix/__init__.py` & `limnoria-2024.4.26/plugins/Unix/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Unix/config.py` & `limnoria-2024.4.26/plugins/Unix/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Unix/locales/fi.po` & `limnoria-2024.4.26/plugins/Unix/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Unix/locales/fr.po` & `limnoria-2024.4.26/plugins/Unix/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Unix/locales/it.po` & `limnoria-2024.4.26/plugins/Unix/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Unix/plugin.py` & `limnoria-2024.4.26/plugins/Unix/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Unix/test.py` & `limnoria-2024.4.26/plugins/Unix/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/User/__init__.py` & `limnoria-2024.4.26/plugins/User/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/User/config.py` & `limnoria-2024.4.26/plugins/User/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/User/locales/de.po` & `limnoria-2024.4.26/plugins/User/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/User/locales/fi.po` & `limnoria-2024.4.26/plugins/User/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/User/locales/fr.po` & `limnoria-2024.4.26/plugins/User/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/User/locales/hu.po` & `limnoria-2024.4.26/plugins/User/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/User/locales/it.po` & `limnoria-2024.4.26/plugins/User/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/User/plugin.py` & `limnoria-2024.4.26/plugins/User/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/User/test.py` & `limnoria-2024.4.26/plugins/User/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Utilities/__init__.py` & `limnoria-2024.4.26/plugins/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Utilities/config.py` & `limnoria-2024.4.26/plugins/Utilities/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Utilities/locales/de.po` & `limnoria-2024.4.26/plugins/Utilities/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Utilities/locales/fi.po` & `limnoria-2024.4.26/plugins/Utilities/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Utilities/locales/fr.po` & `limnoria-2024.4.26/plugins/Utilities/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Utilities/locales/it.po` & `limnoria-2024.4.26/plugins/Utilities/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Utilities/plugin.py` & `limnoria-2024.4.26/plugins/Utilities/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Utilities/test.py` & `limnoria-2024.4.26/plugins/Utilities/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Web/__init__.py` & `limnoria-2024.4.26/plugins/Web/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Web/config.py` & `limnoria-2024.4.26/plugins/Web/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Web/locales/de.po` & `limnoria-2024.4.26/plugins/Web/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Web/locales/fi.po` & `limnoria-2024.4.26/plugins/Web/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Web/locales/fr.po` & `limnoria-2024.4.26/plugins/Web/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Web/locales/it.po` & `limnoria-2024.4.26/plugins/Web/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/plugins/Web/plugin.py` & `limnoria-2024.4.26/plugins/Web/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     def getTitle(self, irc, url, raiseErrors, msg):
         size = conf.supybot.protocols.http.peekSize()
 
         parsed_url = utils.web.urlparse(url)
         if parsed_url.netloc == 'youtube.com' \
                 or parsed_url.netloc.endswith(('.youtube.com')):
             # there is a lot of Javascript before the <title>
-            size = max(409600, size)
+            size = max(819200, size)
         if parsed_url.netloc in ('reddit.com', 'www.reddit.com', 'new.reddit.com'):
             # Since 2022-03, New Reddit has 'Reddit - Dive into anything' as
             # <title> on every page.
             parsed_url = parsed_url._replace(netloc='old.reddit.com')
             url = utils.web.urlunparse(parsed_url)
 
         timeout = self.registryValue('timeout')
@@ -169,30 +169,36 @@
             text = fd.read(size)
             response_headers = fd.headers
             fd.close()
         except socket.timeout:
             if raiseErrors:
                 irc.error(_('Connection to %s timed out') % url, Raise=True)
             else:
-                selg.log.info('Web plugins TitleSnarfer: URL <%s> timed out',
+                self.log.info('Web plugins TitleSnarfer: URL <%s> timed out',
                               url)
+                return
         except Exception as e:
             if raiseErrors:
                 irc.error(_('That URL raised <' + str(e)) + '>',
                           Raise=True)
             else:
                 self.log.info('Web plugin TitleSnarfer: URL <%s> raised <%s>',
                               url, str(e))
                 return
 
         encoding = None
         if 'Content-Type' in fd.headers:
-            mime_params = [p.split('=', 1)
+            # using p.partition('=') instead of 'p.split('=', 1)' because,
+            # unlike RFC 7231, RFC 9110 allows an empty parameter list
+            # after ';':
+            # * https://www.rfc-editor.org/rfc/rfc9110.html#name-media-type
+            # * https://www.rfc-editor.org/rfc/rfc9110.html#parameter
+            mime_params = [p.partition('=')
                 for p in fd.headers['Content-Type'].split(';')[1:]]
-            mime_params = {k.strip(): v.strip() for (k, v) in mime_params}
+            mime_params = {k.strip(): v.strip() for (k, sep, v) in mime_params}
             if mime_params.get('charset'):
                 encoding = mime_params['charset']
 
         encoding = encoding or utils.web.getEncoding(text) or 'utf8'
 
         try:
             text = text.decode(encoding, 'replace')
```

### Comparing `limnoria-2023.9.24/plugins/Web/test.py` & `limnoria-2024.4.26/plugins/Web/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,20 @@
                 'Pianoforte')
 
         def testtitleReddit(self):
             self.assertRegexp(
                 'title https://www.reddit.com/r/irc/',
                 'Internet Relay Chat')
 
+        def testTitleMarcinfo(self):
+            # Checks that we don't crash on 'Content-Type: text/html;'
+            self.assertResponse(
+                    'title https://marc.info/?l=openbsd-tech&m=169841790407370&w=2',
+                    "'Removing syscall(2) from libc and kernel' - MARC")
+
         def testTitleSnarfer(self):
             try:
                 conf.supybot.plugins.Web.titleSnarfer.setValue(True)
                 self.assertSnarfRegexp('http://microsoft.com/',
                                          'Microsoft')
             finally:
                 conf.supybot.plugins.Web.titleSnarfer.setValue(False)
```

### Comparing `limnoria-2023.9.24/plugins/__init__.py` & `limnoria-2024.4.26/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/requirements.txt` & `limnoria-2024.4.26/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 
 # optional plugin dependencies:
 
 cryptography                # required to load the Fediverse plugin (used to implement HTTP signatures to support Mastodon instances with AUTHORIZED_FETCH=true)
 feedparser                  # required to load the RSS plugin
 pytz;python_version<'3.9'   # enables timezone manipulation in the Time and Geography plugins. On Python >=3.9, the standard library is used instead
 python-dateutil             # enable fancy time string parsing in the Time plugin
+ddate                       # required for the ddate command in the Time plugin
```

### Comparing `limnoria-2023.9.24/setup.py` & `limnoria-2024.4.26/setup.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/__init__.py` & `limnoria-2024.4.26/src/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/ansi.py` & `limnoria-2024.4.26/src/ansi.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/callbacks.py` & `limnoria-2024.4.26/src/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,16 +132,16 @@
                         continue
                     if ircutils.nickEqual(maybeNick, nick):
                         return rest
                     else:
                         continue
                 except ValueError: # split didn't work.
                     continue
-            elif whenAddressedByNickAtEnd and lowered.endswith(nick):
-                rest = payload[:-len(nick)]
+            elif whenAddressedByNickAtEnd and lowered.rstrip().endswith(nick):
+                rest = payload.rstrip()[:-len(nick)]
                 possiblePayload = rest.rstrip(' \t,;')
                 if possiblePayload != rest:
                     # There should be some separator between the nick and the
                     # previous alphanumeric character.
                     return possiblePayload
     if get(conf.supybot.reply.whenNotAddressed):
         return payload
```

### Comparing `limnoria-2023.9.24/src/cdb.py` & `limnoria-2024.4.26/src/cdb.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/commands.py` & `limnoria-2024.4.26/src/commands.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/conf.py` & `limnoria-2024.4.26/src/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -937,28 +937,28 @@
         return v
 
     def dirize(self, filename):
         myself = self()
         if os.path.isabs(filename):
             filename = os.path.abspath(filename)
             selfAbs = os.path.abspath(myself)
-            commonPrefix = os.path.commonprefix([selfAbs, filename])
+            commonPrefix = os.path.commonpath([selfAbs, filename])
             filename = filename[len(commonPrefix):]
         elif not os.path.isabs(myself):
             if filename.startswith(myself):
                 filename = filename[len(myself):]
         filename = filename.lstrip(os.path.sep) # Stupid os.path.join!
         return os.path.join(myself, filename)
 
 class DataFilename(registry.String):
     __slots__ = ()
     def __call__(self):
         v = super(DataFilename, self).__call__()
         dataDir = supybot.directories.data()
-        if not v.startswith(dataDir):
+        if not v.startswith("/") and not v.startswith(dataDir):
             v = os.path.basename(v)
             v = os.path.join(dataDir, v)
         self.setValue(v)
         return v
 
 class DataFilenameDirectory(DataFilename, Directory):
     __slots__ = ()
```

### Comparing `limnoria-2023.9.24/src/dbi.py` & `limnoria-2024.4.26/src/dbi.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/drivers/Socket.py` & `limnoria-2024.4.26/src/drivers/Socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,21 @@
         self._sendIfMsgs()
         self._select()
 
     def _read(self):
         """Called by _select() when we can read data."""
         try:
             new_data = self.conn.recv(1024)
+            if hasattr(self.conn, "pending") and self.conn.pending():
+                # This is a TLS socket and there are decrypted bytes in the
+                # buffer. We need to read them now, or we would not get them
+                # until the next time select() returns this socket (which may
+                # be in a very long time, as select() does not know recv() on
+                # the TLS wrapper would not block).
+                new_data += self.conn.recv(self.conn.pending())
             if not new_data:
                 # Socket was closed
                 self._handleSocketError(None)
                 return
 
             self.inbuffer += new_data
             self.eagains = 0 # If we successfully recv'ed, we can reset this.
```

### Comparing `limnoria-2023.9.24/src/drivers/__init__.py` & `limnoria-2024.4.26/src/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/dynamicScope.py` & `limnoria-2024.4.26/src/dynamicScope.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/gpg.py` & `limnoria-2024.4.26/src/gpg.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/httpserver.py` & `limnoria-2024.4.26/src/httpserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
     fullpath = True
     name = 'static'
     defaultResponse = _('Request not handled')
     def __init__(self, mimetype='text/plain; charset=utf-8'):
         super(Static, self).__init__()
         self._mimetype = mimetype
     def doGetOrHead(self, handler, path, write_content):
-        response = get_template(path)
+        response = get_template(path[1:]) # strip leading /
         if minisix.PY3:
             response = response.encode()
         handler.send_response(200)
         self.send_header('Content-type', self._mimetype)
         self.send_header('Content-Length', len(response))
         self.end_headers()
         if write_content:
```

### Comparing `limnoria-2023.9.24/src/i18n.py` & `limnoria-2024.4.26/src/i18n.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/ircdb.py` & `limnoria-2024.4.26/src/ircdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,15 +464,20 @@
 
     def checkIgnored(self, hostmask):
         """Checks whether a given hostmask is to be ignored by the channel."""
         if self.lobotomized:
             return True
         if world.testing:
             return False
-        assert ircutils.isUserHostmask(hostmask), 'got %s' % hostmask
+        if not ircutils.isUserHostmask(hostmask):
+            # Treat messages from a server (e.g. snomasks) as not ignored, as
+            # the ignores system doesn't understand them
+            if '.' not in hostmask:
+                raise ValueError("Expected full prefix, got %r" % hostmask)
+            return False
         if self.checkBan(hostmask):
             return True
         if self.ignores.match(hostmask):
             return True
         return False
 
     def preserve(self, fd, indent=''):
```

### Comparing `limnoria-2023.9.24/src/irclib.py` & `limnoria-2024.4.26/src/irclib.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/ircmsgs.py` & `limnoria-2024.4.26/src/ircmsgs.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/ircutils.py` & `limnoria-2024.4.26/src/ircutils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/log.py` & `limnoria-2024.4.26/src/log.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/plugin.py` & `limnoria-2024.4.26/src/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/questions.py` & `limnoria-2024.4.26/src/questions.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/registry.py` & `limnoria-2024.4.26/src/registry.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/schedule.py` & `limnoria-2024.4.26/src/schedule.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/scripts/limnoria.py` & `limnoria-2024.4.26/src/scripts/limnoria.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/scripts/limnoria_adduser.py` & `limnoria-2024.4.26/src/scripts/limnoria_adduser.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/scripts/limnoria_botchk.py` & `limnoria-2024.4.26/src/scripts/limnoria_botchk.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/scripts/limnoria_plugin_create.py` & `limnoria-2024.4.26/src/scripts/limnoria_plugin_create.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/scripts/limnoria_plugin_doc.py` & `limnoria-2024.4.26/src/scripts/limnoria_plugin_doc.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/scripts/limnoria_reset_password.py` & `limnoria-2024.4.26/src/scripts/limnoria_reset_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     ircdb.users.setUser(user)
     ircdb.users.flush()
     ircdb.users.close()
     print('User %s\'s password reset!' % name)
 
 def main():
     try:
-        main()
+        _main()
     except KeyboardInterrupt:
         pass
 
 if __name__ == '__main__':
     main()
 
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2023.9.24/src/scripts/limnoria_test.py` & `limnoria-2024.4.26/src/scripts/limnoria_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,47 +32,54 @@
 ###
 
 import os
 import sys
 import time
 import shutil
 import fnmatch
+from tempfile import TemporaryDirectory
 started = time.time()
 
 import supybot
 import logging
 import traceback
 
 # We need to do this before we import conf.
-if not os.path.exists('test-conf'):
-    os.mkdir('test-conf')
+main_temp_dir = TemporaryDirectory()
 
-registryFilename = os.path.join('test-conf', 'test.conf')
-fd = open(registryFilename, 'w')
-fd.write("""
+os.makedirs(os.path.join(main_temp_dir.name, 'conf'))
+os.makedirs(os.path.join(main_temp_dir.name, 'data'))
+os.makedirs(os.path.join(main_temp_dir.name, 'logs'))
+
+registryFilename = os.path.join(main_temp_dir.name, 'conf', 'test.conf')
+with open(registryFilename, 'w') as fd:
+    fd.write("""
 supybot.directories.backup: /dev/null
-supybot.directories.conf: %(base_dir)s/test-conf
-supybot.directories.data: %(base_dir)s/test-data
-supybot.directories.log: %(base_dir)s/test-logs
+supybot.directories.conf: {temp_conf}
+supybot.directories.data: {temp_data}
+supybot.directories.log: {temp_logs}
 supybot.reply.whenNotCommand: True
 supybot.log.stdout: False
 supybot.log.stdout.level: ERROR
 supybot.log.level: DEBUG
-supybot.log.format: %%(levelname)s %%(message)s
+supybot.log.format: %(levelname)s %(message)s
 supybot.log.plugins.individualLogfiles: False
 supybot.protocols.irc.throttleTime: 0
 supybot.reply.whenAddressedBy.chars: @
 supybot.networks.test.server: should.not.need.this
 supybot.networks.testnet1.server: should.not.need.this
 supybot.networks.testnet2.server: should.not.need.this
 supybot.networks.testnet3.server: should.not.need.this
 supybot.nick: test
 supybot.databases.users.allowUnregistration: True
-""" % {'base_dir': os.getcwd()})
-fd.close()
+""".format(
+        temp_conf=os.path.join(main_temp_dir.name, 'conf'),
+        temp_data=os.path.join(main_temp_dir.name, 'data'),
+        temp_logs=os.path.join(main_temp_dir.name, 'logs')
+    ))
 
 import supybot.registry as registry
 registry.open_registry(registryFilename)
 
 import supybot.log as log
 import supybot.conf as conf
 conf.allowEval = True
@@ -247,14 +254,17 @@
         shutil.rmtree(conf.supybot.directories.log())
         shutil.rmtree(conf.supybot.directories.conf())
         shutil.rmtree(conf.supybot.directories.data())
 
     if result.wasSuccessful():
         sys.exit(0)
     else:
+        # Deactivate autocleaning for the temporary directiories to allow inspection.
+        main_temp_dir._finalizer.detach()
+        print(f"Temporary directory path: {main_temp_dir.name}")
         sys.exit(1)
 
 
 if __name__ == '__main__':
     main()
 
 # vim:set shiftwidth=4 softtabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2023.9.24/src/scripts/limnoria_wizard.py` & `limnoria-2024.4.26/src/scripts/limnoria_wizard.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/setup.py` & `limnoria-2024.4.26/src/setup.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/shlex.py` & `limnoria-2024.4.26/src/shlex.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/test.py` & `limnoria-2024.4.26/src/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/unpreserve.py` & `limnoria-2024.4.26/src/unpreserve.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/__init__.py` & `limnoria-2024.4.26/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/crypt.py` & `limnoria-2024.4.26/src/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/error.py` & `limnoria-2024.4.26/src/utils/error.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/file.py` & `limnoria-2024.4.26/src/utils/file.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/gen.py` & `limnoria-2024.4.26/src/utils/gen.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/iter.py` & `limnoria-2024.4.26/src/utils/iter.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/math_evaluator.py` & `limnoria-2024.4.26/src/utils/math_evaluator.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/minisix.py` & `limnoria-2024.4.26/src/utils/minisix.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/net.py` & `limnoria-2024.4.26/src/utils/net.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/python.py` & `limnoria-2024.4.26/src/utils/python.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/seq.py` & `limnoria-2024.4.26/src/utils/seq.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/str.py` & `limnoria-2024.4.26/src/utils/str.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/structures.py` & `limnoria-2024.4.26/src/utils/structures.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/time.py` & `limnoria-2024.4.26/src/utils/time.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/transaction.py` & `limnoria-2024.4.26/src/utils/transaction.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/utils/web.py` & `limnoria-2024.4.26/src/utils/web.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/src/world.py` & `limnoria-2024.4.26/src/world.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/__init__.py` & `limnoria-2024.4.26/test/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test.py` & `limnoria-2024.4.26/test/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_callbacks.py` & `limnoria-2024.4.26/test/test_callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,20 @@
     def testAddressedWithNickAtEnd(self):
         irc = getTestIrc()
         msg = ircmsgs.privmsg('#foo', 'baz, bar')
         irc._tagMsg(msg)
         self.assertEqual(callbacks.addressed('bar', msg,
                                              whenAddressedByNickAtEnd=True),
                          'baz')
+        # Test that it still works with trailing whitespace:
+        msg = ircmsgs.privmsg('#foo', 'baz, bar   \t')
+        self.assertEqual(callbacks.addressed('bar', msg,
+                                             whenAddressedByNickAtEnd=True),
+                         'baz')
+
 
     def testAddressedPrefixCharsTakePrecedenceOverNickAtEnd(self):
         irc = getTestIrc()
         msg = ircmsgs.privmsg('#foo', '@echo foo')
         irc._tagMsg(msg)
         self.assertEqual(callbacks.addressed('foo', msg,
                                              whenAddressedByNickAtEnd=True,
```

### Comparing `limnoria-2023.9.24/test/test_commands.py` & `limnoria-2024.4.26/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_conf.py` & `limnoria-2024.4.26/test/test_conf.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_drivers.py` & `limnoria-2024.4.26/test/test_drivers.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_dynamicScope.py` & `limnoria-2024.4.26/test/test_dynamicScope.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_firewall.py` & `limnoria-2024.4.26/test/test_firewall.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_format.py` & `limnoria-2024.4.26/test/test_format.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_i18n.py` & `limnoria-2024.4.26/test/test_i18n.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_ircdb.py` & `limnoria-2024.4.26/test/test_ircdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,14 +346,31 @@
         c.removeIgnore(banmask)
         self.assertFalse(c.checkIgnored(prefix))
         c.addBan(banmask)
         self.assertTrue(c.checkIgnored(prefix))
         c.removeBan(banmask)
         self.assertFalse(c.checkIgnored(prefix))
 
+        # Only full n!u@h is accepted here
+        self.assertRaises(ValueError, c.checkIgnored, 'foo')
+
+    def testIgnoredServerNames(self):
+        c = ircdb.IrcChannel()
+        # Server names are not handled by the ignores system, so this is false
+        self.assertFalse(c.checkIgnored('irc.example.com'))
+        # But we should treat full prefixes that match nick!user@host normally,
+        # even if they include "." like a server name
+        prefix = 'irc.example.com!bar@baz'
+        banmask = ircutils.banmask(prefix)
+        self.assertFalse(c.checkIgnored(prefix))
+        c.addIgnore(banmask)
+        self.assertTrue(c.checkIgnored(prefix))
+        c.removeIgnore(banmask)
+        self.assertFalse(c.checkIgnored(prefix))
+
 class IrcNetworkTestCase(IrcdbTestCase):
     def testDefaults(self):
         n = ircdb.IrcNetwork()
         self.assertEqual(n.stsPolicies, {})
         self.assertEqual(n.lastDisconnectTimes, {})
 
     def testStsPolicy(self):
```

### Comparing `limnoria-2023.9.24/test/test_irclib.py` & `limnoria-2024.4.26/test/test_irclib.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_ircmsgs.py` & `limnoria-2024.4.26/test/test_ircmsgs.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_ircutils.py` & `limnoria-2024.4.26/test/test_ircutils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_misc.py` & `limnoria-2024.4.26/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_plugin.py` & `limnoria-2024.4.26/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_plugin_create.py` & `limnoria-2024.4.26/test/test_plugin_create.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_plugins.py` & `limnoria-2024.4.26/test/test_plugins.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_registry.py` & `limnoria-2024.4.26/test/test_registry.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_schedule.py` & `limnoria-2024.4.26/test/test_schedule.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_standardSubstitute.py` & `limnoria-2024.4.26/test/test_standardSubstitute.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_utils.py` & `limnoria-2024.4.26/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2023.9.24/test/test_yn.py` & `limnoria-2024.4.26/test/test_yn.py`

 * *Files identical despite different names*

