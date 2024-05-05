# Comparing `tmp/MyProx-0.5.0.tar.gz` & `tmp/MyProx-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyProx-0.5.0.tar", last modified: Tue Nov  1 07:42:41 2022, max compression
+gzip compressed data, was "MyProx-0.6.0.tar", last modified: Sun May  5 09:52:25 2024, max compression
```

## Comparing `MyProx-0.5.0.tar` & `MyProx-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-01 07:42:40.982205 MyProx-0.5.0/
--rw-r--r--   0 root         (0) root         (0)    34523 2022-09-09 12:05:38.000000 MyProx-0.5.0/LICENSE
--rwxrw-r--   0 root         (0) root         (0)       99 2022-08-05 16:10:50.000000 MyProx-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3776 2022-11-01 07:42:40.954205 MyProx-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2086 2022-09-09 14:27:33.000000 MyProx-0.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-01 07:42:41.010204 MyProx-0.5.0/setup.cfg
--rwxrw-r--   0 root         (0) root         (0)     1797 2022-10-31 10:09:00.000000 MyProx-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-01 07:42:37.530264 MyProx-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-01 07:42:38.670244 MyProx-0.5.0/src/MyProx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3776 2022-11-01 07:42:36.000000 MyProx-0.5.0/src/MyProx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      753 2022-11-01 07:42:36.000000 MyProx-0.5.0/src/MyProx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-01 07:42:36.000000 MyProx-0.5.0/src/MyProx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2022-11-01 07:42:36.000000 MyProx-0.5.0/src/MyProx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2022-11-01 07:42:36.000000 MyProx-0.5.0/src/MyProx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-11-01 07:42:36.000000 MyProx-0.5.0/src/MyProx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-01 07:42:39.330233 MyProx-0.5.0/src/myprox/
--rwxrw-r--   0 root         (0) root         (0)     1105 2022-07-04 10:18:32.000000 MyProx-0.5.0/src/myprox/__init__.py
--rwxrw-r--   0 root         (0) root         (0)     5974 2022-10-31 09:33:50.000000 MyProx-0.5.0/src/myprox/config.py
--rwxrw-r--   0 root         (0) root         (0)     4632 2022-09-08 14:39:00.000000 MyProx-0.5.0/src/myprox/myproxapi.py
--rwxrw-r--   0 root         (0) root         (0)     6683 2022-10-31 10:01:08.000000 MyProx-0.5.0/src/myprox/proxapi.py
--rwxrw-r--   0 root         (0) root         (0)      416 2022-09-10 18:55:54.000000 MyProx-0.5.0/src/myprox/setupenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-01 07:42:40.370215 MyProx-0.5.0/src/myprox/templates/
--rwxrw-r--   0 root         (0) root         (0)      566 2022-09-09 19:14:03.000000 MyProx-0.5.0/src/myprox/templates/base.html
--rwxrw-r--   0 root         (0) root         (0)     1472 2020-11-26 21:11:48.000000 MyProx-0.5.0/src/myprox/templates/edit.html
--rwxrw-r--   0 root         (0) root         (0)     1825 2022-10-01 11:08:32.000000 MyProx-0.5.0/src/myprox/templates/index.html
--rwxrw-r--   0 root         (0) root         (0)     1061 2022-07-04 11:46:42.000000 MyProx-0.5.0/src/myprox/templates/login.html
--rwxrw-r--   0 root         (0) root         (0)     3306 2022-10-31 09:58:26.000000 MyProx-0.5.0/src/myprox/templates/manage.html
--rwxrw-r--   0 root         (0) root         (0)     1821 2022-09-13 19:42:14.000000 MyProx-0.5.0/src/myprox/templates/myprox.conf
--rwxrw-r--   0 root         (0) root         (0)      365 2022-07-21 20:38:34.000000 MyProx-0.5.0/src/myprox/templates/part_header.html
--rwxrw-r--   0 root         (0) root         (0)    11734 2022-10-31 09:57:55.000000 MyProx-0.5.0/src/myprox/webapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-01 07:42:37.610262 MyProx-0.5.0/src/myprox/webroot/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-01 07:42:40.818207 MyProx-0.5.0/src/myprox/webroot/static/
--rwxrw-r--   0 root         (0) root         (0)     3774 2022-07-05 14:25:02.000000 MyProx-0.5.0/src/myprox/webroot/static/favicon.ico
--rwxrw-r--   0 root         (0) root         (0)      604 2022-07-05 14:25:02.000000 MyProx-0.5.0/src/myprox/webroot/static/logo.png
--rwxrw-r--   0 root         (0) root         (0)     9576 2022-07-05 14:19:00.000000 MyProx-0.5.0/src/myprox/webroot/static/logo.svg
--rwxrw-r--   0 root         (0) root         (0)     3026 2022-09-15 18:36:51.000000 MyProx-0.5.0/src/myprox/webroot/static/styles.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 09:52:25.109055 MyProx-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)    34523 2022-09-09 12:05:38.000000 MyProx-0.6.0/LICENSE
+-rwxrw-r--   0 root         (0) root         (0)       99 2022-08-05 16:10:50.000000 MyProx-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3237 2024-05-05 09:52:25.105055 MyProx-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2086 2022-09-09 14:27:33.000000 MyProx-0.6.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 09:52:25.109055 MyProx-0.6.0/setup.cfg
+-rwxrw-r--   0 root         (0) root         (0)     1807 2024-05-05 09:50:58.000000 MyProx-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 09:52:25.009056 MyProx-0.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 09:52:25.045055 MyProx-0.6.0/src/MyProx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3237 2024-05-05 09:52:24.000000 MyProx-0.6.0/src/MyProx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-05 09:52:24.000000 MyProx-0.6.0/src/MyProx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 09:52:24.000000 MyProx-0.6.0/src/MyProx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-05 09:52:24.000000 MyProx-0.6.0/src/MyProx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-05 09:52:24.000000 MyProx-0.6.0/src/MyProx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-05 09:52:24.000000 MyProx-0.6.0/src/MyProx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 09:52:25.061055 MyProx-0.6.0/src/myprox/
+-rwxrw-r--   0 root         (0) root         (0)     1105 2022-07-04 10:18:32.000000 MyProx-0.6.0/src/myprox/__init__.py
+-rwxrw-r--   0 root         (0) root         (0)     5974 2022-10-31 09:33:50.000000 MyProx-0.6.0/src/myprox/config.py
+-rwxrw-r--   0 root         (0) root         (0)     4632 2022-09-08 14:39:00.000000 MyProx-0.6.0/src/myprox/myproxapi.py
+-rwxrw-r--   0 root         (0) root         (0)     6683 2022-10-31 10:01:08.000000 MyProx-0.6.0/src/myprox/proxapi.py
+-rwxrw-r--   0 root         (0) root         (0)      416 2022-09-10 18:55:54.000000 MyProx-0.6.0/src/myprox/setupenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 09:52:25.085055 MyProx-0.6.0/src/myprox/templates/
+-rwxrw-r--   0 root         (0) root         (0)      566 2022-09-09 19:14:03.000000 MyProx-0.6.0/src/myprox/templates/base.html
+-rwxrw-r--   0 root         (0) root         (0)     1472 2020-11-26 21:11:48.000000 MyProx-0.6.0/src/myprox/templates/edit.html
+-rwxrw-r--   0 root         (0) root         (0)     1825 2022-10-01 11:08:32.000000 MyProx-0.6.0/src/myprox/templates/index.html
+-rwxrw-r--   0 root         (0) root         (0)     1061 2022-07-04 11:46:42.000000 MyProx-0.6.0/src/myprox/templates/login.html
+-rwxrw-r--   0 root         (0) root         (0)     3306 2022-10-31 09:58:26.000000 MyProx-0.6.0/src/myprox/templates/manage.html
+-rwxrw-r--   0 root         (0) root         (0)     1821 2022-09-13 19:42:14.000000 MyProx-0.6.0/src/myprox/templates/myprox.conf
+-rwxrw-r--   0 root         (0) root         (0)      365 2022-07-21 20:38:34.000000 MyProx-0.6.0/src/myprox/templates/part_header.html
+-rwxrw-r--   0 root         (0) root         (0)    11707 2024-05-04 20:13:06.000000 MyProx-0.6.0/src/myprox/webapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 09:52:25.013056 MyProx-0.6.0/src/myprox/webroot/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 09:52:25.101055 MyProx-0.6.0/src/myprox/webroot/static/
+-rwxrw-r--   0 root         (0) root         (0)     3774 2022-07-05 14:25:02.000000 MyProx-0.6.0/src/myprox/webroot/static/favicon.ico
+-rwxrw-r--   0 root         (0) root         (0)      604 2022-07-05 14:25:02.000000 MyProx-0.6.0/src/myprox/webroot/static/logo.png
+-rwxrw-r--   0 root         (0) root         (0)     9576 2022-07-05 14:19:00.000000 MyProx-0.6.0/src/myprox/webroot/static/logo.svg
+-rwxrw-r--   0 root         (0) root         (0)     3049 2024-05-04 19:15:04.000000 MyProx-0.6.0/src/myprox/webroot/static/styles.css
```

### Comparing `MyProx-0.5.0/LICENSE` & `MyProx-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/PKG-INFO` & `MyProx-0.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,105 @@
 Metadata-Version: 2.1
 Name: MyProx
-Version: 0.5.0
+Version: 0.6.0
 Summary: simple web frontend for Proxmox VE users
 Home-page: https://www.github.com/towalink/myprox
 Author: Dirk Henrici
 Author-email: pypi.myprox@henrici.name
-License: UNKNOWN
 Project-URL: Project homepage, https://www.henrici.name/projects/myprox
 Project-URL: Repository, https://www.github.com/towalink/myprox
 Project-URL: Documentation, https://www.github.com/towalink/myprox
-Description: # MyProx
-        
-        A simple web frontend for accessing and managing VMs running on Proxmox VE. It is targeted on end-users.
-        
-        ---
-        
-        ## Main Features
-        
-        - List all VMs a user has permissions on
-        - Manage VM state, e.g. starting and stopping
-        - Open SPICE console (virt-viewer)
-        - Authentication against Proxmox
-        - Web frontend has responsive design
-        - Does not require root privileges
-        - Built on light-weight CherryPy framework
-        - No JavaScript bloat; no external font/JS includes
-        - Simple installation using pip, few dependencies
-        
-        ---
-        
-        ## Installation
-        
-        Install using PyPi:
-        
-        ```shell
-        pip3 install myprox
-        ```
-        
-        ---
-        
-        ## Quickstart
-        
-        After installing "MyProx" as shown above, just execute the tool to get it running:
-        
-        ```shell
-        myprox
-        ```
-        
-        Configuration can be done in the file `/etc/myprox/myprox.conf`. A commented example file can be downloaded at <a href="https://github.com/towalink/myprox/blob/main/src/myprox/templates/myprox.conf" target="_blank">https://github.com/towalink/myprox/blob/main/src/myprox/templates/myprox.conf</a>.
-        
-        ---
-        
-        ## Screenshots
-        
-        <img src="https://raw.githubusercontent.com/towalink/myprox/main/screenshots/list-machines.png" width="450" alt="screenshot: show list of VMs">
-        
-        See additional screenshots in the "screenshots" folder.
-        
-        ---
-        
-        ## Reporting bugs
-        
-        In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
-        
-        ---
-        
-        ## Developers
-        
-        ### Clone repository
-        
-        Clone this repo to your local machine using `https://github.com/towalink/myprox.git`
-        
-        Install the module temporarily to make it available in your Python installation:
-        ```shell
-        pip3 install -e <path to directory with setup.py>
-        ```
-        
-        ---
-        
-        ## License
-        
-        [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
-        
-        - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-        - Copyright 2022 © <a href="https://github.com/towalink/myprox" target="_blank">Dirk Henrici</a>.
-        - Note: This project is not affiliated with [Proxmox](https://www.proxmox.com/), it just accesses its REST API.
-        
 Keywords: Proxmox frontend gui
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Systems Administration
 Classifier: Framework :: CherryPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cherrypy
+Requires-Dist: requests
+Requires-Dist: jinja2
+Requires-Dist: proxmoxer
+
+# MyProx
+
+A simple web frontend for accessing and managing VMs running on Proxmox VE. It is targeted on end-users.
+
+---
+
+## Main Features
+
+- List all VMs a user has permissions on
+- Manage VM state, e.g. starting and stopping
+- Open SPICE console (virt-viewer)
+- Authentication against Proxmox
+- Web frontend has responsive design
+- Does not require root privileges
+- Built on light-weight CherryPy framework
+- No JavaScript bloat; no external font/JS includes
+- Simple installation using pip, few dependencies
+
+---
+
+## Installation
+
+Install using PyPi:
+
+```shell
+pip3 install myprox
+```
+
+---
+
+## Quickstart
+
+After installing "MyProx" as shown above, just execute the tool to get it running:
+
+```shell
+myprox
+```
+
+Configuration can be done in the file `/etc/myprox/myprox.conf`. A commented example file can be downloaded at <a href="https://github.com/towalink/myprox/blob/main/src/myprox/templates/myprox.conf" target="_blank">https://github.com/towalink/myprox/blob/main/src/myprox/templates/myprox.conf</a>.
+
+---
+
+## Screenshots
+
+<img src="https://raw.githubusercontent.com/towalink/myprox/main/screenshots/list-machines.png" width="450" alt="screenshot: show list of VMs">
+
+See additional screenshots in the "screenshots" folder.
+
+---
+
+## Reporting bugs
+
+In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
+
+---
+
+## Developers
+
+### Clone repository
+
+Clone this repo to your local machine using `https://github.com/towalink/myprox.git`
+
+Install the module temporarily to make it available in your Python installation:
+```shell
+pip3 install -e <path to directory with setup.py>
+```
+
+---
+
+## License
+
+[![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
+
+- **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
+- Copyright 2022 © <a href="https://github.com/towalink/myprox" target="_blank">Dirk Henrici</a>.
+- Note: This project is not affiliated with [Proxmox](https://www.proxmox.com/), it just accesses its REST API.
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
-Metadata-Version: 2.1 Name: MyProx Version: 0.5.0 Summary: simple web frontend
+Metadata-Version: 2.1 Name: MyProx Version: 0.6.0 Summary: simple web frontend
 for Proxmox VE users Home-page: https://www.github.com/towalink/myprox Author:
-Dirk Henrici Author-email: pypi.myprox@henrici.name License: UNKNOWN Project-
-URL: Project homepage, https://www.henrici.name/projects/myprox Project-URL:
-Repository, https://www.github.com/towalink/myprox Project-URL: Documentation,
-https://www.github.com/towalink/myprox Description: # MyProx A simple web
-frontend for accessing and managing VMs running on Proxmox VE. It is targeted
-on end-users. --- ## Main Features - List all VMs a user has permissions on -
-Manage VM state, e.g. starting and stopping - Open SPICE console (virt-viewer)
-- Authentication against Proxmox - Web frontend has responsive design - Does
-not require root privileges - Built on light-weight CherryPy framework - No
-JavaScript bloat; no external font/JS includes - Simple installation using pip,
-few dependencies --- ## Installation Install using PyPi: ```shell pip3 install
-myprox ``` --- ## Quickstart After installing "MyProx" as shown above, just
-execute the tool to get it running: ```shell myprox ``` Configuration can be
-done in the file `/etc/myprox/myprox.conf`. A commented example file can be
-downloaded at _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_t_o_w_a_l_i_n_k_/_m_y_p_r_o_x_/_b_l_o_b_/_m_a_i_n_/_s_r_c_/_m_y_p_r_o_x_/
-_t_e_m_p_l_a_t_e_s_/_m_y_p_r_o_x_._c_o_n_f. --- ## Screenshots [screenshot: show list of VMs]See
-additional screenshots in the "screenshots" folder. --- ## Reporting bugs In
-case you encounter any bugs, please report the expected behavior and the actual
-behavior so that the issue can be reproduced and fixed. --- ## Developers ###
-Clone repository Clone this repo to your local machine using `https://
-github.com/towalink/myprox.git` Install the module temporarily to make it
-available in your Python installation: ```shell pip3 install -e ``` --- ##
-License [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-
-square)](https://opensource.org/licenses/AGPL-3.0) - **[AGPL3 license](https://
-opensource.org/licenses/AGPL-3.0)** - Copyright 2022 Â© _D_i_r_k_ _H_e_n_r_i_c_i. - Note:
-This project is not affiliated with [Proxmox](https://www.proxmox.com/), it
-just accesses its REST API. Keywords: Proxmox frontend gui Platform: UNKNOWN
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: GNU Affero General Public
-License v3 or later (AGPLv3+) Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience :: End
-Users/Desktop Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Information Technology Classifier: Topic ::
-System :: Systems Administration Classifier: Framework :: CherryPy Requires-
-Python: >=3.6 Description-Content-Type: text/markdown
+Dirk Henrici Author-email: pypi.myprox@henrici.name Project-URL: Project
+homepage, https://www.henrici.name/projects/myprox Project-URL: Repository,
+https://www.github.com/towalink/myprox Project-URL: Documentation, https://
+www.github.com/towalink/myprox Keywords: Proxmox frontend gui Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or
+later (AGPLv3+) Classifier: Operating System :: POSIX :: Linux Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: End Users/
+Desktop Classifier: Intended Audience :: System Administrators Classifier:
+Intended Audience :: Information Technology Classifier: Topic :: System ::
+Systems Administration Classifier: Framework :: CherryPy Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+cherrypy Requires-Dist: requests Requires-Dist: jinja2 Requires-Dist: proxmoxer
+# MyProx A simple web frontend for accessing and managing VMs running on
+Proxmox VE. It is targeted on end-users. --- ## Main Features - List all VMs a
+user has permissions on - Manage VM state, e.g. starting and stopping - Open
+SPICE console (virt-viewer) - Authentication against Proxmox - Web frontend has
+responsive design - Does not require root privileges - Built on light-weight
+CherryPy framework - No JavaScript bloat; no external font/JS includes - Simple
+installation using pip, few dependencies --- ## Installation Install using
+PyPi: ```shell pip3 install myprox ``` --- ## Quickstart After installing
+"MyProx" as shown above, just execute the tool to get it running: ```shell
+myprox ``` Configuration can be done in the file `/etc/myprox/myprox.conf`. A
+commented example file can be downloaded at _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_t_o_w_a_l_i_n_k_/_m_y_p_r_o_x_/
+_b_l_o_b_/_m_a_i_n_/_s_r_c_/_m_y_p_r_o_x_/_t_e_m_p_l_a_t_e_s_/_m_y_p_r_o_x_._c_o_n_f. --- ## Screenshots [screenshot:
+show list of VMs]See additional screenshots in the "screenshots" folder. --- ##
+Reporting bugs In case you encounter any bugs, please report the expected
+behavior and the actual behavior so that the issue can be reproduced and fixed.
+--- ## Developers ### Clone repository Clone this repo to your local machine
+using `https://github.com/towalink/myprox.git` Install the module temporarily
+to make it available in your Python installation: ```shell pip3 install -e ```
+--- ## License [![License](http://img.shields.io/:license-agpl3-
+blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0) - **
+[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)** - Copyright 2022 Â©
+_D_i_r_k_ _H_e_n_r_i_c_i. - Note: This project is not affiliated with [Proxmox](https://
+www.proxmox.com/), it just accesses its REST API.
```

### Comparing `MyProx-0.5.0/README.md` & `MyProx-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/setup.py` & `MyProx-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'MyProx',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'author': 'Dirk Henrici',
     'author_email': 'pypi.myprox@henrici.name',
     'description': 'simple web frontend for Proxmox VE users',
     'long_description': long_description,
     'long_description_content_type': 'text/markdown',
     'url': 'https://www.github.com/towalink/myprox',
-    'packages': setuptools.find_packages('src'),
+    'packages': setuptools.find_namespace_packages('src'),
     'package_dir': {'': 'src'},
     'include_package_data': True,
     'install_requires': ['cherrypy',
                          'requests',
                          'jinja2',
                          'proxmoxer',
                         ],
```

### Comparing `MyProx-0.5.0/src/MyProx.egg-info/PKG-INFO` & `MyProx-0.6.0/src/MyProx.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,105 @@
 Metadata-Version: 2.1
 Name: MyProx
-Version: 0.5.0
+Version: 0.6.0
 Summary: simple web frontend for Proxmox VE users
 Home-page: https://www.github.com/towalink/myprox
 Author: Dirk Henrici
 Author-email: pypi.myprox@henrici.name
-License: UNKNOWN
 Project-URL: Project homepage, https://www.henrici.name/projects/myprox
 Project-URL: Repository, https://www.github.com/towalink/myprox
 Project-URL: Documentation, https://www.github.com/towalink/myprox
-Description: # MyProx
-        
-        A simple web frontend for accessing and managing VMs running on Proxmox VE. It is targeted on end-users.
-        
-        ---
-        
-        ## Main Features
-        
-        - List all VMs a user has permissions on
-        - Manage VM state, e.g. starting and stopping
-        - Open SPICE console (virt-viewer)
-        - Authentication against Proxmox
-        - Web frontend has responsive design
-        - Does not require root privileges
-        - Built on light-weight CherryPy framework
-        - No JavaScript bloat; no external font/JS includes
-        - Simple installation using pip, few dependencies
-        
-        ---
-        
-        ## Installation
-        
-        Install using PyPi:
-        
-        ```shell
-        pip3 install myprox
-        ```
-        
-        ---
-        
-        ## Quickstart
-        
-        After installing "MyProx" as shown above, just execute the tool to get it running:
-        
-        ```shell
-        myprox
-        ```
-        
-        Configuration can be done in the file `/etc/myprox/myprox.conf`. A commented example file can be downloaded at <a href="https://github.com/towalink/myprox/blob/main/src/myprox/templates/myprox.conf" target="_blank">https://github.com/towalink/myprox/blob/main/src/myprox/templates/myprox.conf</a>.
-        
-        ---
-        
-        ## Screenshots
-        
-        <img src="https://raw.githubusercontent.com/towalink/myprox/main/screenshots/list-machines.png" width="450" alt="screenshot: show list of VMs">
-        
-        See additional screenshots in the "screenshots" folder.
-        
-        ---
-        
-        ## Reporting bugs
-        
-        In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
-        
-        ---
-        
-        ## Developers
-        
-        ### Clone repository
-        
-        Clone this repo to your local machine using `https://github.com/towalink/myprox.git`
-        
-        Install the module temporarily to make it available in your Python installation:
-        ```shell
-        pip3 install -e <path to directory with setup.py>
-        ```
-        
-        ---
-        
-        ## License
-        
-        [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
-        
-        - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-        - Copyright 2022 © <a href="https://github.com/towalink/myprox" target="_blank">Dirk Henrici</a>.
-        - Note: This project is not affiliated with [Proxmox](https://www.proxmox.com/), it just accesses its REST API.
-        
 Keywords: Proxmox frontend gui
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Systems Administration
 Classifier: Framework :: CherryPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cherrypy
+Requires-Dist: requests
+Requires-Dist: jinja2
+Requires-Dist: proxmoxer
+
+# MyProx
+
+A simple web frontend for accessing and managing VMs running on Proxmox VE. It is targeted on end-users.
+
+---
+
+## Main Features
+
+- List all VMs a user has permissions on
+- Manage VM state, e.g. starting and stopping
+- Open SPICE console (virt-viewer)
+- Authentication against Proxmox
+- Web frontend has responsive design
+- Does not require root privileges
+- Built on light-weight CherryPy framework
+- No JavaScript bloat; no external font/JS includes
+- Simple installation using pip, few dependencies
+
+---
+
+## Installation
+
+Install using PyPi:
+
+```shell
+pip3 install myprox
+```
+
+---
+
+## Quickstart
+
+After installing "MyProx" as shown above, just execute the tool to get it running:
+
+```shell
+myprox
+```
+
+Configuration can be done in the file `/etc/myprox/myprox.conf`. A commented example file can be downloaded at <a href="https://github.com/towalink/myprox/blob/main/src/myprox/templates/myprox.conf" target="_blank">https://github.com/towalink/myprox/blob/main/src/myprox/templates/myprox.conf</a>.
+
+---
+
+## Screenshots
+
+<img src="https://raw.githubusercontent.com/towalink/myprox/main/screenshots/list-machines.png" width="450" alt="screenshot: show list of VMs">
+
+See additional screenshots in the "screenshots" folder.
+
+---
+
+## Reporting bugs
+
+In case you encounter any bugs, please report the expected behavior and the actual behavior so that the issue can be reproduced and fixed.
+
+---
+
+## Developers
+
+### Clone repository
+
+Clone this repo to your local machine using `https://github.com/towalink/myprox.git`
+
+Install the module temporarily to make it available in your Python installation:
+```shell
+pip3 install -e <path to directory with setup.py>
+```
+
+---
+
+## License
+
+[![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
+
+- **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
+- Copyright 2022 © <a href="https://github.com/towalink/myprox" target="_blank">Dirk Henrici</a>.
+- Note: This project is not affiliated with [Proxmox](https://www.proxmox.com/), it just accesses its REST API.
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
-Metadata-Version: 2.1 Name: MyProx Version: 0.5.0 Summary: simple web frontend
+Metadata-Version: 2.1 Name: MyProx Version: 0.6.0 Summary: simple web frontend
 for Proxmox VE users Home-page: https://www.github.com/towalink/myprox Author:
-Dirk Henrici Author-email: pypi.myprox@henrici.name License: UNKNOWN Project-
-URL: Project homepage, https://www.henrici.name/projects/myprox Project-URL:
-Repository, https://www.github.com/towalink/myprox Project-URL: Documentation,
-https://www.github.com/towalink/myprox Description: # MyProx A simple web
-frontend for accessing and managing VMs running on Proxmox VE. It is targeted
-on end-users. --- ## Main Features - List all VMs a user has permissions on -
-Manage VM state, e.g. starting and stopping - Open SPICE console (virt-viewer)
-- Authentication against Proxmox - Web frontend has responsive design - Does
-not require root privileges - Built on light-weight CherryPy framework - No
-JavaScript bloat; no external font/JS includes - Simple installation using pip,
-few dependencies --- ## Installation Install using PyPi: ```shell pip3 install
-myprox ``` --- ## Quickstart After installing "MyProx" as shown above, just
-execute the tool to get it running: ```shell myprox ``` Configuration can be
-done in the file `/etc/myprox/myprox.conf`. A commented example file can be
-downloaded at _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_t_o_w_a_l_i_n_k_/_m_y_p_r_o_x_/_b_l_o_b_/_m_a_i_n_/_s_r_c_/_m_y_p_r_o_x_/
-_t_e_m_p_l_a_t_e_s_/_m_y_p_r_o_x_._c_o_n_f. --- ## Screenshots [screenshot: show list of VMs]See
-additional screenshots in the "screenshots" folder. --- ## Reporting bugs In
-case you encounter any bugs, please report the expected behavior and the actual
-behavior so that the issue can be reproduced and fixed. --- ## Developers ###
-Clone repository Clone this repo to your local machine using `https://
-github.com/towalink/myprox.git` Install the module temporarily to make it
-available in your Python installation: ```shell pip3 install -e ``` --- ##
-License [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-
-square)](https://opensource.org/licenses/AGPL-3.0) - **[AGPL3 license](https://
-opensource.org/licenses/AGPL-3.0)** - Copyright 2022 Â© _D_i_r_k_ _H_e_n_r_i_c_i. - Note:
-This project is not affiliated with [Proxmox](https://www.proxmox.com/), it
-just accesses its REST API. Keywords: Proxmox frontend gui Platform: UNKNOWN
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: GNU Affero General Public
-License v3 or later (AGPLv3+) Classifier: Operating System :: POSIX :: Linux
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience :: End
-Users/Desktop Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Information Technology Classifier: Topic ::
-System :: Systems Administration Classifier: Framework :: CherryPy Requires-
-Python: >=3.6 Description-Content-Type: text/markdown
+Dirk Henrici Author-email: pypi.myprox@henrici.name Project-URL: Project
+homepage, https://www.henrici.name/projects/myprox Project-URL: Repository,
+https://www.github.com/towalink/myprox Project-URL: Documentation, https://
+www.github.com/towalink/myprox Keywords: Proxmox frontend gui Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or
+later (AGPLv3+) Classifier: Operating System :: POSIX :: Linux Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: End Users/
+Desktop Classifier: Intended Audience :: System Administrators Classifier:
+Intended Audience :: Information Technology Classifier: Topic :: System ::
+Systems Administration Classifier: Framework :: CherryPy Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+cherrypy Requires-Dist: requests Requires-Dist: jinja2 Requires-Dist: proxmoxer
+# MyProx A simple web frontend for accessing and managing VMs running on
+Proxmox VE. It is targeted on end-users. --- ## Main Features - List all VMs a
+user has permissions on - Manage VM state, e.g. starting and stopping - Open
+SPICE console (virt-viewer) - Authentication against Proxmox - Web frontend has
+responsive design - Does not require root privileges - Built on light-weight
+CherryPy framework - No JavaScript bloat; no external font/JS includes - Simple
+installation using pip, few dependencies --- ## Installation Install using
+PyPi: ```shell pip3 install myprox ``` --- ## Quickstart After installing
+"MyProx" as shown above, just execute the tool to get it running: ```shell
+myprox ``` Configuration can be done in the file `/etc/myprox/myprox.conf`. A
+commented example file can be downloaded at _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_t_o_w_a_l_i_n_k_/_m_y_p_r_o_x_/
+_b_l_o_b_/_m_a_i_n_/_s_r_c_/_m_y_p_r_o_x_/_t_e_m_p_l_a_t_e_s_/_m_y_p_r_o_x_._c_o_n_f. --- ## Screenshots [screenshot:
+show list of VMs]See additional screenshots in the "screenshots" folder. --- ##
+Reporting bugs In case you encounter any bugs, please report the expected
+behavior and the actual behavior so that the issue can be reproduced and fixed.
+--- ## Developers ### Clone repository Clone this repo to your local machine
+using `https://github.com/towalink/myprox.git` Install the module temporarily
+to make it available in your Python installation: ```shell pip3 install -e ```
+--- ## License [![License](http://img.shields.io/:license-agpl3-
+blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0) - **
+[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)** - Copyright 2022 Â©
+_D_i_r_k_ _H_e_n_r_i_c_i. - Note: This project is not affiliated with [Proxmox](https://
+www.proxmox.com/), it just accesses its REST API.
```

### Comparing `MyProx-0.5.0/src/MyProx.egg-info/SOURCES.txt` & `MyProx-0.6.0/src/MyProx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/__init__.py` & `MyProx-0.6.0/src/myprox/__init__.py`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/config.py` & `MyProx-0.6.0/src/myprox/config.py`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/myproxapi.py` & `MyProx-0.6.0/src/myprox/myproxapi.py`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/proxapi.py` & `MyProx-0.6.0/src/myprox/proxapi.py`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/templates/base.html` & `MyProx-0.6.0/src/myprox/templates/base.html`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/templates/edit.html` & `MyProx-0.6.0/src/myprox/templates/edit.html`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/templates/index.html` & `MyProx-0.6.0/src/myprox/templates/index.html`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/templates/login.html` & `MyProx-0.6.0/src/myprox/templates/login.html`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/templates/manage.html` & `MyProx-0.6.0/src/myprox/templates/manage.html`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/templates/myprox.conf` & `MyProx-0.6.0/src/myprox/templates/myprox.conf`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/webapp.py` & `MyProx-0.6.0/src/myprox/webapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         """Provide a connection file for download"""
         cherrypy.log(f'Attempting to download connection file for [{id}] by user [{cherrypy.session["username"]}]', context='WEBAPP', severity=logging.INFO, traceback=False)
         try:
             file_dict = cherrypy.session['proxmox'].get_spice(id)
             file_data = '[virt-viewer]\n'
             for key, value in file_dict.items():
                 file_data += f'{key}={value}\n'
-            cherrypy.log(str(file_data), context='WEBAPP', severity=logging.INFO, traceback=False)
+            cherrypy.log(str(file_data), context='WEBAPP', severity=logging.DEBUG, traceback=False)
             filename = ''.join([random.choice(string.ascii_letters + string.digits) for n in range(6)])
             #cherrypy.response.headers['Content-Disposition'] = f'attachment; filename={filename}.vv'
             cherrypy.response.headers['Content-Disposition'] = f'inline; filename={filename}.vv'
             cherrypy.response.headers['Content-Type'] = 'application/x-virt-viewer'
             return file_data.encode('utf-8')
         except Exception as e:
             return str(e)
@@ -169,22 +169,41 @@
         cherrypy.log('Error calling on_change_command', context='WEBAPP', severity=logging.ERROR, traceback=False)
 
 
 def run_webapp(cfg):
     """Runs the CherryPy web application with the provided configuration data"""
     script_path = os.path.dirname(os.path.abspath(__file__))
     app = WebApp(cfg)
+    # Use SSL if certificate files exist
+    ssl = os.path.exists(cfg.sslcertfile) and os.path.exists(cfg.sslkeyfile)
+    if ssl:
+        # Use ssl/tls if certificate files are present
+        cherrypy.server.ssl_module = 'builtin'
+        cherrypy.server.ssl_certificate = cfg.sslcertfile
+        cherrypy.server.ssl_private_key = cfg.sslkeyfile
+    else:
+        cherrypy.log(f'Not using SSL/TLS due to certificate files [{cfg.sslcertfile}] and [{cfg.sslkeyfile}] not being present', context='SETUP', severity=logging.WARNING, traceback=False)
+    # Define socket parameters
+    cherrypy.config.update({'server.socket_host': cfg.socket_host,
+                            'server.socket_port': cfg.socket_port,
+                           })
+    # Select environment
+    cherrypy.config.update({'staging':
+                             {
+                               'environment' : 'production'
+                             }
+                           })
     # Configure the web application
     app_conf = {
       'global': {
          'environment' : 'production'
        },
        '/': {
             'tools.sessions.on': True,
-            'tools.sessions.secure': (cherrypy.server.ssl_certificate is not None),
+            'tools.sessions.secure': ssl,
             'tools.sessions.httponly': True,
             'tools.staticdir.root': os.path.join(script_path, 'webroot'),
             'tools.session_auth.on': True,
             'tools.session_auth.login_screen': app.login_screen,
             'tools.session_auth.check_username_and_password': app.check_username_and_password,
             },
         '/static': {
@@ -195,32 +214,14 @@
         '/favicon.ico':
         {
             'tools.session_auth.on': False,
             'tools.staticfile.on': True,
             'tools.staticfile.filename': os.path.join(script_path, 'webroot', 'static', 'favicon.ico')
         }
     }
-    # Use SSL if certificate files exist
-    if os.path.exists(cfg.sslcertfile) and os.path.exists(cfg.sslkeyfile):
-        # Use ssl/tls if certificate files are present
-        cherrypy.server.ssl_module = 'builtin'
-        cherrypy.server.ssl_certificate = cfg.sslcertfile
-        cherrypy.server.ssl_private_key = cfg.sslkeyfile
-    else:
-        cherrypy.log(f'Not using SSL/TLS due to certificate files [{cfg.sslcertfile}] and [{cfg.sslkeyfile}] not being present', context='SETUP', severity=logging.WARNING, traceback=False)
-    # Define socket parameters
-    cherrypy.config.update({'server.socket_host': cfg.socket_host,
-                            'server.socket_port': cfg.socket_port,
-                           })
-    # Select environment
-    cherrypy.config.update({'staging':
-                             {
-                               'environment' : 'production'
-                             }
-                           })
     # Start CherryPy
     cherrypy.tree.mount(app, config=app_conf)
     if setupenv.is_root():
         # Drop privileges
         cherrypy.log(f'MyProx was started as root; attempting to drop privileges to user "{cfg.webserver_user}" and group "{cfg.webserver_group}"', context='SETUP', severity=logging.INFO, traceback=False)
         try:
             uid, gid = setupenv.get_uid_gid(cfg.webserver_user, cfg.webserver_group)
```

### Comparing `MyProx-0.5.0/src/myprox/webroot/static/favicon.ico` & `MyProx-0.6.0/src/myprox/webroot/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/webroot/static/logo.png` & `MyProx-0.6.0/src/myprox/webroot/static/logo.png`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/webroot/static/logo.svg` & `MyProx-0.6.0/src/myprox/webroot/static/logo.svg`

 * *Files identical despite different names*

### Comparing `MyProx-0.5.0/src/myprox/webroot/static/styles.css` & `MyProx-0.6.0/src/myprox/webroot/static/styles.css`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 html {
   font: normal 16px sans-serif;
   background-color: #f3f3f3;
   color: #000;
 }
 
+body {
+  min-height: 100vh;
+  display: flex;
+  flex-direction: column;
+}
+
 a {
   text-decoration: none;
   color: inherit;
   cursor: pointer;
   opacity: 0.9;
 }
 
@@ -116,15 +122,15 @@
   color: #000;
   font-size: 14px;
   text-align: right;
 }
 
 section {
   width: 100%;
-  display: flex;
+  flex: 1;
   padding: 10px 250px;
   background-color: #f3f3f3;
 }
 
 .content {
   width: 100%;
 }
@@ -166,32 +172,27 @@
   margin-top: 1em;
 }
 
 .instructions {
   font-size: 14px;
 }
 
-
 @media screen and (max-width: 1000px) {
   .table, .table-row {
     display: block;
   }
   .table-cell {
     display: block;
   }
   .bordertop2{
     border-top: 0;
   }
 }
 
-
 footer {
-  position: fixed;
-  left: 0;
-  bottom: 0;
   width: 100%;
   background-color: #dddddd;
   color: red;
   font-size: 12px;
   text-align: center;
   padding: 3px 5px;
 }
```

