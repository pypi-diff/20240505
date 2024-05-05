# Comparing `tmp/dalle3_gen_save-0.1.0.tar.gz` & `tmp/dalle3_gen_save-0.1.1.tar.gz`

## Comparing `dalle3_gen_save-0.1.0.tar` & `dalle3_gen_save-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,9 @@
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3_gen_save.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/setup.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/MANIFEST.in
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/README.md
--rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/dalle3_gen_save.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/requirements.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/setup.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/dalle3_gen_save.egg-info/PKG-INFO
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/dalle3_gen_save.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/dalle3_gen_save.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/dalle3_gen_save.egg-info/entry_points.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/dalle3_gen_save.egg-info/requires.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/dalle3_gen_save.egg-info/top_level.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/dist/dalle3_gen_save-4.5.50-py3-none-any.whl
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3-gen-save-4.5.50/dist/dalle3_gen_save-4.5.50.tar.gz
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3_gen_save.egg-info/PKG-INFO
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3_gen_save.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3_gen_save.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3_gen_save.egg-info/requires.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/dalle3_gen_save.egg-info/top_level.txt
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/sh/install.sh
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/sh/push.sh
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/sh/to_pip.sh
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/.gitignore
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/README.md
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.1/README.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.1/dalle3_gen_save.py
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.1/sh/build.sh
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.1/sh/install.sh
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.1/sh/push.sh
+-rwxr-xr-x   0        0        0       58 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.1/sh/to_pip.sh
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.1/.gitignore
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 dalle3_gen_save-0.1.1/PKG-INFO
```

### Comparing `dalle3_gen_save-0.1.0/dalle3_gen_save.py` & `dalle3_gen_save-0.1.1/dalle3_gen_save.py`

 * *Files identical despite different names*

