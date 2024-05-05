# Comparing `tmp/yerba-0.0.1a0.dev1.tar.gz` & `tmp/yerba-0.0.2a0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yerba-0.0.1a0.dev1.tar", last modified: Mon Jan 15 19:25:49 2024, max compression
+gzip compressed data, was "yerba-0.0.2a0.dev0.tar", last modified: Sun May  5 19:37:47 2024, max compression
```

## Comparing `yerba-0.0.1a0.dev1.tar` & `yerba-0.0.2a0.dev0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 19:25:49.561478 yerba-0.0.1a0.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-15 19:25:37.000000 yerba-0.0.1a0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-01-15 19:25:49.561478 yerba-0.0.1a0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-01-15 19:25:37.000000 yerba-0.0.1a0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-01-15 19:25:37.000000 yerba-0.0.1a0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 19:25:49.561478 yerba-0.0.1a0.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 19:25:49.561478 yerba-0.0.1a0.dev1/yerba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-01-15 19:25:49.000000 yerba-0.0.1a0.dev1/yerba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-15 19:25:49.000000 yerba-0.0.1a0.dev1/yerba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 19:25:49.000000 yerba-0.0.1a0.dev1/yerba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-15 19:25:49.000000 yerba-0.0.1a0.dev1/yerba.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-15 19:25:49.000000 yerba-0.0.1a0.dev1/yerba.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 19:25:49.000000 yerba-0.0.1a0.dev1/yerba.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:37:47.754475 yerba-0.0.2a0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-05 19:37:43.000000 yerba-0.0.2a0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-05 19:37:47.754475 yerba-0.0.2a0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-05 19:37:43.000000 yerba-0.0.2a0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-05 19:37:43.000000 yerba-0.0.2a0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 19:37:47.754475 yerba-0.0.2a0.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:37:47.754475 yerba-0.0.2a0.dev0/yerba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-05 19:37:47.000000 yerba-0.0.2a0.dev0/yerba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-05 19:37:47.000000 yerba-0.0.2a0.dev0/yerba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 19:37:47.000000 yerba-0.0.2a0.dev0/yerba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-05 19:37:47.000000 yerba-0.0.2a0.dev0/yerba.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-05 19:37:47.000000 yerba-0.0.2a0.dev0/yerba.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 19:37:47.000000 yerba-0.0.2a0.dev0/yerba.egg-info/top_level.txt
```

### Comparing `yerba-0.0.1a0.dev1/LICENSE` & `yerba-0.0.2a0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `yerba-0.0.1a0.dev1/PKG-INFO` & `yerba-0.0.2a0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yerba
-Version: 0.0.1a0.dev1
+Version: 0.0.2a0.dev0
 Author-email: "Bernardo L. Español" <esp.bernardo@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: manim
 Requires-Dist: manim-mobject-svg
 Requires-Dist: markdown-it-py
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yerba Version: 0.0.1a0.dev1 Author-email: "Bernardo
+Metadata-Version: 2.1 Name: yerba Version: 0.0.2a0.dev0 Author-email: "Bernardo
 L. EspaÃ±ol"
 gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: manim Requires-Dist: manim-mobject-svg
 Requires-Dist: markdown-it-py Requires-Dist: mdformat Requires-Dist: mdit-py-
 plugins Requires-Dist: numpy Requires-Dist: pillow Requires-Dist: pyyaml
       _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_b_e_r_s_p_/_y_e_r_b_a_/_m_a_i_n_/_l_o_g_o_/_Y_e_r_b_a_._p_n_g_]
```

### Comparing `yerba-0.0.1a0.dev1/README.md` & `yerba-0.0.2a0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `yerba-0.0.1a0.dev1/yerba.egg-info/PKG-INFO` & `yerba-0.0.2a0.dev0/yerba.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yerba
-Version: 0.0.1a0.dev1
+Version: 0.0.2a0.dev0
 Author-email: "Bernardo L. Español" <esp.bernardo@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: manim
 Requires-Dist: manim-mobject-svg
 Requires-Dist: markdown-it-py
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yerba Version: 0.0.1a0.dev1 Author-email: "Bernardo
+Metadata-Version: 2.1 Name: yerba Version: 0.0.2a0.dev0 Author-email: "Bernardo
 L. EspaÃ±ol"
 gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: manim Requires-Dist: manim-mobject-svg
 Requires-Dist: markdown-it-py Requires-Dist: mdformat Requires-Dist: mdit-py-
 plugins Requires-Dist: numpy Requires-Dist: pillow Requires-Dist: pyyaml
       _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_b_e_r_s_p_/_y_e_r_b_a_/_m_a_i_n_/_l_o_g_o_/_Y_e_r_b_a_._p_n_g_]
```

