# Comparing `tmp/tmrl-0.6.3.tar.gz` & `tmp/tmrl-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmrl-0.6.3.tar", last modified: Fri Apr 26 07:50:12 2024, max compression
+gzip compressed data, was "tmrl-0.6.4.tar", last modified: Sun May  5 18:48:32 2024, max compression
```

## Comparing `tmrl-0.6.3.tar` & `tmrl-0.6.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 07:50:12.138832 tmrl-0.6.3/
--rw-rw-rw-   0        0        0     1089 2024-04-08 03:24:28.000000 tmrl-0.6.3/LICENSE
--rw-rw-rw-   0        0        0       43 2024-04-08 03:28:54.000000 tmrl-0.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2052 2024-04-26 07:50:12.138832 tmrl-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0    31154 2024-04-08 03:28:54.000000 tmrl-0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 07:50:11.652002 tmrl-0.6.3/readme/
--rw-rw-rw-   0        0        0     1067 2024-04-08 03:28:54.000000 tmrl-0.6.3/readme/pypi.md
--rw-rw-rw-   0        0        0       42 2024-04-26 07:50:12.138832 tmrl-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     6314 2024-04-26 07:47:33.000000 tmrl-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:50:11.761878 tmrl-0.6.3/tmrl/
--rw-rw-rw-   0        0        0     1590 2024-04-23 05:21:02.000000 tmrl-0.6.3/tmrl/__init__.py
--rw-rw-rw-   0        0        0     4262 2024-04-23 05:21:02.000000 tmrl-0.6.3/tmrl/__main__.py
--rw-rw-rw-   0        0        0     5386 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/actor.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:50:11.812741 tmrl-0.6.3/tmrl/config/
--rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/config/__init__.py
--rw-rw-rw-   0        0        0     6165 2024-04-23 05:21:02.000000 tmrl-0.6.3/tmrl/config/config_constants.py
--rw-rw-rw-   0        0        0     8564 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/config/config_objects.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:50:11.918994 tmrl-0.6.3/tmrl/custom/
--rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/__init__.py
--rw-rw-rw-   0        0        0    18803 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/custom_algorithms.py
--rw-rw-rw-   0        0        0     9431 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/custom_checkpoints.py
--rw-rw-rw-   0        0        0    12796 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/custom_gym_interfaces.py
--rw-rw-rw-   0        0        0    23958 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/custom_memories.py
--rw-rw-rw-   0        0        0    29938 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/custom_models.py
--rw-rw-rw-   0        0        0     1387 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/custom_preprocessors.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:50:12.075773 tmrl-0.6.3/tmrl/custom/utils/
--rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/__init__.py
--rw-rw-rw-   0        0        0     5463 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/utils/compute_reward.py
--rw-rw-rw-   0        0        0     2248 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/control_gamepad.py
--rw-rw-rw-   0        0        0     3981 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/control_keyboard.py
--rw-rw-rw-   0        0        0     1710 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/control_mouse.py
--rw-rw-rw-   0        0        0     9041 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/custom/utils/nn.py
--rw-rw-rw-   0        0        0     5019 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/tools.py
--rw-rw-rw-   0        0        0     9247 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/custom/utils/window.py
--rw-rw-rw-   0        0        0     1291 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/envs.py
--rw-rw-rw-   0        0        0     9555 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/memory.py
--rw-rw-rw-   0        0        0    41597 2024-04-08 03:28:54.000000 tmrl-0.6.3/tmrl/networking.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:50:12.091343 tmrl-0.6.3/tmrl/tools/
--rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/tools/__init__.py
--rw-rw-rw-   0        0        0     2922 2024-04-26 07:47:33.000000 tmrl-0.6.3/tmrl/tools/check_environment.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:50:12.124322 tmrl-0.6.3/tmrl/tools/init_package/
--rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/tools/init_package/__init__.py
--rw-rw-rw-   0        0        0    27288 2024-04-23 05:21:02.000000 tmrl-0.6.3/tmrl/tools/init_package/init_pywin32.py
--rw-rw-rw-   0        0        0     4882 2024-04-23 05:21:02.000000 tmrl-0.6.3/tmrl/tools/init_package/init_tmrl.py
--rw-rw-rw-   0        0        0     3238 2024-04-26 07:13:45.000000 tmrl-0.6.3/tmrl/tools/record.py
--rw-rw-rw-   0        0        0     1279 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/tools/save_replays.py
--rw-rw-rw-   0        0        0     1390 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/training.py
--rw-rw-rw-   0        0        0    10895 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/training_offline.py
--rw-rw-rw-   0        0        0    10255 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/util.py
--rw-rw-rw-   0        0        0     2031 2024-04-08 03:24:28.000000 tmrl-0.6.3/tmrl/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-04-26 07:50:11.793131 tmrl-0.6.3/tmrl.egg-info/
--rw-rw-rw-   0        0        0     2052 2024-04-26 07:50:11.000000 tmrl-0.6.3/tmrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2024-04-26 07:50:11.000000 tmrl-0.6.3/tmrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 07:50:11.000000 tmrl-0.6.3/tmrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2024-04-26 07:50:11.000000 tmrl-0.6.3/tmrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-26 07:50:11.000000 tmrl-0.6.3/tmrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 18:48:32.613344 tmrl-0.6.4/
+-rw-rw-rw-   0        0        0     1089 2024-04-08 03:24:28.000000 tmrl-0.6.4/LICENSE
+-rw-rw-rw-   0        0        0       43 2024-04-08 03:28:54.000000 tmrl-0.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2052 2024-05-05 18:48:32.597706 tmrl-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0    31211 2024-04-30 04:38:25.000000 tmrl-0.6.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 18:48:32.094647 tmrl-0.6.4/readme/
+-rw-rw-rw-   0        0        0     1067 2024-04-08 03:28:54.000000 tmrl-0.6.4/readme/pypi.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:48:32.613344 tmrl-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     6314 2024-05-05 18:27:36.000000 tmrl-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:48:32.235758 tmrl-0.6.4/tmrl/
+-rw-rw-rw-   0        0        0     1590 2024-05-05 18:46:33.000000 tmrl-0.6.4/tmrl/__init__.py
+-rw-rw-rw-   0        0        0     4262 2024-05-05 18:36:06.000000 tmrl-0.6.4/tmrl/__main__.py
+-rw-rw-rw-   0        0        0     5386 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/actor.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:48:32.269832 tmrl-0.6.4/tmrl/config/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/config/__init__.py
+-rw-rw-rw-   0        0        0     6165 2024-04-23 05:21:02.000000 tmrl-0.6.4/tmrl/config/config_constants.py
+-rw-rw-rw-   0        0        0     8564 2024-05-05 18:46:28.000000 tmrl-0.6.4/tmrl/config/config_objects.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:48:32.377708 tmrl-0.6.4/tmrl/custom/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/custom/__init__.py
+-rw-rw-rw-   0        0        0    18803 2024-04-08 03:28:54.000000 tmrl-0.6.4/tmrl/custom/custom_algorithms.py
+-rw-rw-rw-   0        0        0     9431 2024-04-08 03:28:54.000000 tmrl-0.6.4/tmrl/custom/custom_checkpoints.py
+-rw-rw-rw-   0        0        0    12796 2024-04-08 03:28:54.000000 tmrl-0.6.4/tmrl/custom/custom_gym_interfaces.py
+-rw-rw-rw-   0        0        0    23958 2024-04-08 03:28:54.000000 tmrl-0.6.4/tmrl/custom/custom_memories.py
+-rw-rw-rw-   0        0        0    29938 2024-04-08 03:28:54.000000 tmrl-0.6.4/tmrl/custom/custom_models.py
+-rw-rw-rw-   0        0        0     1387 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/custom/custom_preprocessors.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:48:32.519059 tmrl-0.6.4/tmrl/custom/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/custom/utils/__init__.py
+-rw-rw-rw-   0        0        0     5463 2024-04-08 03:28:54.000000 tmrl-0.6.4/tmrl/custom/utils/compute_reward.py
+-rw-rw-rw-   0        0        0     2248 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/custom/utils/control_gamepad.py
+-rw-rw-rw-   0        0        0     3981 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/custom/utils/control_keyboard.py
+-rw-rw-rw-   0        0        0     1710 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/custom/utils/control_mouse.py
+-rw-rw-rw-   0        0        0     9041 2024-04-08 03:28:54.000000 tmrl-0.6.4/tmrl/custom/utils/nn.py
+-rw-rw-rw-   0        0        0     5019 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/custom/utils/tools.py
+-rw-rw-rw-   0        0        0     9247 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/custom/utils/window.py
+-rw-rw-rw-   0        0        0     1291 2024-04-08 03:28:54.000000 tmrl-0.6.4/tmrl/envs.py
+-rw-rw-rw-   0        0        0     9555 2024-04-08 03:28:54.000000 tmrl-0.6.4/tmrl/memory.py
+-rw-rw-rw-   0        0        0    41597 2024-04-08 03:28:54.000000 tmrl-0.6.4/tmrl/networking.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:48:32.550300 tmrl-0.6.4/tmrl/tools/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/tools/__init__.py
+-rw-rw-rw-   0        0        0     2922 2024-04-26 07:47:33.000000 tmrl-0.6.4/tmrl/tools/check_environment.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:48:32.597706 tmrl-0.6.4/tmrl/tools/init_package/
+-rw-rw-rw-   0        0        0        0 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/tools/init_package/__init__.py
+-rw-rw-rw-   0        0        0    27288 2024-04-23 05:21:02.000000 tmrl-0.6.4/tmrl/tools/init_package/init_pywin32.py
+-rw-rw-rw-   0        0        0     4882 2024-04-23 05:21:02.000000 tmrl-0.6.4/tmrl/tools/init_package/init_tmrl.py
+-rw-rw-rw-   0        0        0     2861 2024-05-05 18:22:16.000000 tmrl-0.6.4/tmrl/tools/record.py
+-rw-rw-rw-   0        0        0     1279 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/tools/save_replays.py
+-rw-rw-rw-   0        0        0     1390 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/training.py
+-rw-rw-rw-   0        0        0    10895 2024-05-05 18:46:41.000000 tmrl-0.6.4/tmrl/training_offline.py
+-rw-rw-rw-   0        0        0    10255 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/util.py
+-rw-rw-rw-   0        0        0     2031 2024-04-08 03:24:28.000000 tmrl-0.6.4/tmrl/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:48:32.267463 tmrl-0.6.4/tmrl.egg-info/
+-rw-rw-rw-   0        0        0     2052 2024-05-05 18:48:31.000000 tmrl-0.6.4/tmrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1140 2024-05-05 18:48:31.000000 tmrl-0.6.4/tmrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:48:31.000000 tmrl-0.6.4/tmrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2024-05-05 18:48:31.000000 tmrl-0.6.4/tmrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-05 18:48:31.000000 tmrl-0.6.4/tmrl.egg-info/top_level.txt
```

### Comparing `tmrl-0.6.3/LICENSE` & `tmrl-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/PKG-INFO` & `tmrl-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tmrl
-Version: 0.6.3
+Version: 0.6.4
 Summary: Network-based framework for real-time robot learning
 Home-page: https://github.com/trackmania-rl/tmrl
-Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.3.tar.gz
+Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.4.tar.gz
 Author: Yann Bouteiller, Edouard Geze
 Author-email: yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr
 License: MIT
 Keywords: reinforcement learning,robot learning,trackmania,self driving,roborace
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `tmrl-0.6.3/README.md` & `tmrl-0.6.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     - [User features](#user-features-trackmania-example-pipeline)
     - [Developer features](#developer-features-real-world-applications-in-python)
     - [TMRL in the media](#tmrl-in-the-media)
   - [Installation](readme/Install.md)
     - [Windows](readme/Install.md)
     - [Linux](readme/install_linux.md)
   - [Getting started](readme/get_started.md)
+    - [Quick reference guide](readme/reference_guide.md)
   - [TMRL python library for robot learning](readme/tuto_library.md)
     - [API reference](https://tmrl.readthedocs.io/en/latest/)
   - [Security (important)](#security)
 - [TrackMania applications](#autonomous-driving-in-trackmania)
   - [TrackMania Roborace League](readme/competition.md)
   - [TrackMania Gymnasium environment](#trackmania-gymnasium-environment)
     - [LIDAR environment](#lidar-environment)
```

### Comparing `tmrl-0.6.3/readme/pypi.md` & `tmrl-0.6.4/readme/pypi.md`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/setup.py` & `tmrl-0.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,21 +133,21 @@
 HERE = os.path.abspath(os.path.dirname(__file__))
 README_FOLDER = os.path.join(HERE, "readme")
 with open(os.path.join(README_FOLDER, "pypi.md")) as fid:
     README = fid.read()
 
 setup(
     name='tmrl',
-    version='0.6.3',
+    version='0.6.4',
     description='Network-based framework for real-time robot learning',
     long_description=README,
     long_description_content_type='text/markdown',
     keywords='reinforcement learning, robot learning, trackmania, self driving, roborace',
     url='https://github.com/trackmania-rl/tmrl',
-    download_url='https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.3.tar.gz',
+    download_url='https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.4.tar.gz',
     author='Yann Bouteiller, Edouard Geze',
     author_email='yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr',
     license='MIT',
     install_requires=install_req,
     classifiers=[
             'Development Status :: 4 - Beta',
             'Intended Audience :: Developers',
```

### Comparing `tmrl-0.6.3/tmrl/__init__.py` & `tmrl-0.6.4/tmrl/__init__.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/__main__.py` & `tmrl-0.6.4/tmrl/__main__.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/actor.py` & `tmrl-0.6.4/tmrl/actor.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/config/config_constants.py` & `tmrl-0.6.4/tmrl/config/config_constants.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/config/config_objects.py` & `tmrl-0.6.4/tmrl/config/config_objects.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/custom_algorithms.py` & `tmrl-0.6.4/tmrl/custom/custom_algorithms.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/custom_checkpoints.py` & `tmrl-0.6.4/tmrl/custom/custom_checkpoints.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/custom_gym_interfaces.py` & `tmrl-0.6.4/tmrl/custom/custom_gym_interfaces.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/custom_memories.py` & `tmrl-0.6.4/tmrl/custom/custom_memories.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/custom_models.py` & `tmrl-0.6.4/tmrl/custom/custom_models.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/custom_preprocessors.py` & `tmrl-0.6.4/tmrl/custom/custom_preprocessors.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/utils/compute_reward.py` & `tmrl-0.6.4/tmrl/custom/utils/compute_reward.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/utils/control_gamepad.py` & `tmrl-0.6.4/tmrl/custom/utils/control_gamepad.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/utils/control_keyboard.py` & `tmrl-0.6.4/tmrl/custom/utils/control_keyboard.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/utils/control_mouse.py` & `tmrl-0.6.4/tmrl/custom/utils/control_mouse.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/utils/nn.py` & `tmrl-0.6.4/tmrl/custom/utils/nn.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/utils/tools.py` & `tmrl-0.6.4/tmrl/custom/utils/tools.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/custom/utils/window.py` & `tmrl-0.6.4/tmrl/custom/utils/window.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/envs.py` & `tmrl-0.6.4/tmrl/envs.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/memory.py` & `tmrl-0.6.4/tmrl/memory.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/networking.py` & `tmrl-0.6.4/tmrl/networking.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/tools/check_environment.py` & `tmrl-0.6.4/tmrl/tools/check_environment.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/tools/init_package/init_pywin32.py` & `tmrl-0.6.4/tmrl/tools/init_package/init_pywin32.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/tools/init_package/init_tmrl.py` & `tmrl-0.6.4/tmrl/tools/init_package/init_tmrl.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/tools/record.py` & `tmrl-0.6.4/tmrl/tools/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,43 +9,31 @@
 import tmrl.config.config_constants as cfg
 from tmrl.custom.utils.tools import TM2020OpenPlanetClient
 import logging
 
 
 PATH_REWARD = cfg.REWARD_PATH
 DATASET_PATH = cfg.DATASET_PATH
-SYSTEM = cfg.SYSTEM
-
-if SYSTEM == "Windows":
-    import keyboard
 
 
 def record_reward_dist(path_reward=PATH_REWARD):
     positions = []
     client = TM2020OpenPlanetClient()
     path = path_reward
 
     is_recording = False
     while True:
         if not is_recording:
-            if SYSTEM == "Windows":
-                if keyboard.is_pressed('e'):
-                    logging.info(f"start recording")
-                    is_recording = True
-            else:
-                logging.info(f"start recording")
-                is_recording = True
+            logging.info(f"start recording")
+            is_recording = True
 
         if is_recording:
             data = client.retrieve_data(sleep_if_empty=0.01)  # we need many points to build a smooth curve
             terminated = bool(data[8])
-            if SYSTEM == "Windows":
-                early_stop = keyboard.is_pressed('q')
-            else:
-                early_stop = False
+            early_stop = False
             if early_stop or terminated:
                 logging.info(f"Computing reward function checkpoints from captured positions...")
                 logging.info(f"Initial number of captured positions: {len(positions)}")
                 positions = np.array(positions)
 
                 final_positions = [positions[0]]
                 dist_between_points = 0.1
```

### Comparing `tmrl-0.6.3/tmrl/tools/save_replays.py` & `tmrl-0.6.4/tmrl/tools/save_replays.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/training.py` & `tmrl-0.6.4/tmrl/training.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/training_offline.py` & `tmrl-0.6.4/tmrl/training_offline.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/util.py` & `tmrl-0.6.4/tmrl/util.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl/wrappers.py` & `tmrl-0.6.4/tmrl/wrappers.py`

 * *Files identical despite different names*

### Comparing `tmrl-0.6.3/tmrl.egg-info/PKG-INFO` & `tmrl-0.6.4/tmrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tmrl
-Version: 0.6.3
+Version: 0.6.4
 Summary: Network-based framework for real-time robot learning
 Home-page: https://github.com/trackmania-rl/tmrl
-Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.3.tar.gz
+Download-URL: https://github.com/trackmania-rl/tmrl/archive/refs/tags/v0.6.4.tar.gz
 Author: Yann Bouteiller, Edouard Geze
 Author-email: yann.bouteiller@polymtl.ca, edouard.geze@hotmail.fr
 License: MIT
 Keywords: reinforcement learning,robot learning,trackmania,self driving,roborace
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `tmrl-0.6.3/tmrl.egg-info/SOURCES.txt` & `tmrl-0.6.4/tmrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

