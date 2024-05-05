# Comparing `tmp/ciscoconfaudit-0.1.2.tar.gz` & `tmp/ciscoconfaudit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciscoconfaudit-0.1.2.tar", last modified: Thu Feb 15 08:27:01 2024, max compression
+gzip compressed data, was "ciscoconfaudit-0.2.0.tar", last modified: Sun May  5 15:22:41 2024, max compression
```

## Comparing `ciscoconfaudit-0.1.2.tar` & `ciscoconfaudit-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-15 08:27:01.867103 ciscoconfaudit-0.1.2/
--rw-rw-rw-   0        0        0    35553 2024-02-14 23:04:52.000000 ciscoconfaudit-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      721 2024-02-14 23:11:25.000000 ciscoconfaudit-0.1.2/NOTICE
--rw-rw-rw-   0        0        0    45572 2024-02-15 08:27:01.866098 ciscoconfaudit-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2841 2024-02-15 07:52:14.000000 ciscoconfaudit-0.1.2/README.md
--rw-rw-rw-   0        0        0     2250 2024-02-15 08:26:43.000000 ciscoconfaudit-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-15 08:27:01.867103 ciscoconfaudit-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-15 08:27:01.825097 ciscoconfaudit-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-02-15 08:27:01.843105 ciscoconfaudit-0.1.2/src/ciscoconfaudit/
--rw-rw-rw-   0        0        0    30444 2024-02-15 08:26:43.000000 ciscoconfaudit-0.1.2/src/ciscoconfaudit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-15 08:27:01.865098 ciscoconfaudit-0.1.2/src/ciscoconfaudit.egg-info/
--rw-rw-rw-   0        0        0    45572 2024-02-15 08:27:01.000000 ciscoconfaudit-0.1.2/src/ciscoconfaudit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-02-15 08:27:01.000000 ciscoconfaudit-0.1.2/src/ciscoconfaudit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-15 08:27:01.000000 ciscoconfaudit-0.1.2/src/ciscoconfaudit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-02-15 08:27:01.000000 ciscoconfaudit-0.1.2/src/ciscoconfaudit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-15 08:27:01.000000 ciscoconfaudit-0.1.2/src/ciscoconfaudit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 15:22:41.611920 ciscoconfaudit-0.2.0/
+-rw-rw-rw-   0        0        0    35553 2024-02-14 23:04:52.000000 ciscoconfaudit-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      721 2024-02-14 23:11:25.000000 ciscoconfaudit-0.2.0/NOTICE
+-rw-rw-rw-   0        0        0    46460 2024-05-05 15:22:41.609917 ciscoconfaudit-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3501 2024-04-28 12:24:03.000000 ciscoconfaudit-0.2.0/README.md
+-rw-rw-rw-   0        0        0     2412 2024-05-05 15:21:55.000000 ciscoconfaudit-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:22:41.611920 ciscoconfaudit-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 15:22:41.588918 ciscoconfaudit-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 15:22:41.591918 ciscoconfaudit-0.2.0/src/ciscoconfaudit/
+-rw-rw-rw-   0        0        0    32225 2024-05-05 15:20:20.000000 ciscoconfaudit-0.2.0/src/ciscoconfaudit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:22:41.608917 ciscoconfaudit-0.2.0/src/ciscoconfaudit.egg-info/
+-rw-rw-rw-   0        0        0    46460 2024-05-05 15:22:41.000000 ciscoconfaudit-0.2.0/src/ciscoconfaudit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-05 15:22:41.000000 ciscoconfaudit-0.2.0/src/ciscoconfaudit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:22:41.000000 ciscoconfaudit-0.2.0/src/ciscoconfaudit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-05 15:22:41.000000 ciscoconfaudit-0.2.0/src/ciscoconfaudit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-05 15:22:41.000000 ciscoconfaudit-0.2.0/src/ciscoconfaudit.egg-info/top_level.txt
```

### Comparing `ciscoconfaudit-0.1.2/LICENSE` & `ciscoconfaudit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ciscoconfaudit-0.1.2/NOTICE` & `ciscoconfaudit-0.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `ciscoconfaudit-0.1.2/PKG-INFO` & `ciscoconfaudit-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscoconfaudit
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Cisco IOS & IOS-XE configuration audit tool
 Author-email: Osama Abbas <oabbas2512@gmail.com>
 Maintainer-email: Osama Abbas <oabbas2512@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -676,17 +676,19 @@
         into proprietary programs. If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library. If this is what you want to do, use the GNU Lesser General
         Public License instead of this License. But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/Tes3awy/cisco-config-auditor/
-Project-URL: Bug Tracker, https://github.com/Tes3awy/cisco-config-auditor/issues/
+Project-URL: Repository, https://github.com/Tes3awy/cisco-config-auditor/
+Project-URL: Issues, https://github.com/Tes3awy/cisco-config-auditor/issues/
 Project-URL: Say Thanks!, https://saythanks.io/to/Tes3awy
 Project-URL: Source, https://github.com/Tes3awy/cisco-config-auditor/
+Project-URL: Changelog, https://github.com/Tes3awy/cisco-config-auditor/CHANGELOG.md
 Keywords: cisco,audit,configuration audit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
@@ -697,33 +699,38 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Classifier: Typing :: Typed
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: ciscoconfparse
 Requires-Dist: rich
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 
-# Cisco Config Auditor
+# ciscoconfaudit
 
 [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/Tes3awy/cisco-config-auditor)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ciscoconfaudit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![LICENSE](https://img.shields.io/github/license/Tes3awy/cisco-config-auditor?color=purple&style=flat-square&label=LICENSE)
 ![Commit Activity](https://img.shields.io/github/commit-activity/m/Tes3awy/cisco-config-auditor/main?logo=github&style=flat-square)
+![PyPI - Version](https://img.shields.io/pypi/v/ciscoconfaudit)
+![PyPI - Status](https://img.shields.io/pypi/status/ciscoconfaudit)
+[![Downloads](https://static.pepy.tech/badge/ciscoconfaudit)](https://pepy.tech/project/ciscoconfaudit)
 [![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/Tes3awy)
 
 > Based on [Use Cisco IOS XE Hardening Guide](https://www.cisco.com/c/en/us/support/docs/ios-nx-os-software/ios-xe-16/220270-use-cisco-ios-xe-hardening-guide.html) and some opinionated best practices.
 
 This package gives an overview of the hardening techniques that can be used to secure a Cisco network device. Network security is not a one-layer thing, yet, it depends on multiple factors. If you harden your devices, then it is a good starting point that increases the overall security of the environment you manage.
 
 ## Installation
@@ -732,31 +739,35 @@
 
 ```bash
 $ pip install ciscoconfaudit
 ```
 
 ## Usage
 
-You can try out two examples in the repo.
+You can try out _two examples_ in the repo in [examples](https://github.com/Tes3awy/cisco-config-auditor/tree/main/examples).
 
 ```bash
-(.venv) $ python3 online.py   # Parses config from a device (Uses netmiko)
-(.venv) $ python3 offline.py  # Parses config from text file
+(.venv) $ python3 basic_online.py   # Parses config from a device (Uses netmiko)
+(.venv) $ python3 basic_offline.py  # Parses config from text file
 ```
 
 ### Example Output
 
 | Global Config Audit (Sample)                                                                                     | Interface-Level Audit                                                                                                |
 | ---------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
 | ![Global Config Audit](https://github.com/Tes3awy/cisco-config-auditor/blob/main/assets/global-config-audit.jpg) | ![Interface Level Audit](https://github.com/Tes3awy/cisco-config-auditor/blob/main/assets/interface-level-audit.jpg) |
 
-## Credits
+## Use Case
 
-This package was inspired by [jonarm](https://github.com/jonarm) from [cisco-ios-audit](https://github.com/jonarm/cisco-ios-audit).
+- Ever been tired of checking whether the Cisco hardneing technqiues (_[here](https://www.cisco.com/c/en/us/support/docs/ios-nx-os-software/ios-xe-16/220270-use-cisco-ios-xe-hardening-guide.html)_) are applied to your network devices one by one? This package is very handy in generating a tabular report for you.
 
 ## Author
 
 [Osama Abbas](https://github.com/Tes3awy)
 
+## Credits
+
+This package was inspired by [jonarm](https://github.com/jonarm) from [cisco-ios-audit](https://github.com/jonarm/cisco-ios-audit).
+
 ## Contributions
 
 You are welcome to contribute to this Cisco [Swiss army knife](https://en.wikipedia.org/wiki/Swiss_Army_knife).
```

### Comparing `ciscoconfaudit-0.1.2/README.md` & `ciscoconfaudit-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-# Cisco Config Auditor
+# ciscoconfaudit
 
 [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/Tes3awy/cisco-config-auditor)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ciscoconfaudit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![LICENSE](https://img.shields.io/github/license/Tes3awy/cisco-config-auditor?color=purple&style=flat-square&label=LICENSE)
 ![Commit Activity](https://img.shields.io/github/commit-activity/m/Tes3awy/cisco-config-auditor/main?logo=github&style=flat-square)
+![PyPI - Version](https://img.shields.io/pypi/v/ciscoconfaudit)
+![PyPI - Status](https://img.shields.io/pypi/status/ciscoconfaudit)
+[![Downloads](https://static.pepy.tech/badge/ciscoconfaudit)](https://pepy.tech/project/ciscoconfaudit)
 [![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/Tes3awy)
 
 > Based on [Use Cisco IOS XE Hardening Guide](https://www.cisco.com/c/en/us/support/docs/ios-nx-os-software/ios-xe-16/220270-use-cisco-ios-xe-hardening-guide.html) and some opinionated best practices.
 
 This package gives an overview of the hardening techniques that can be used to secure a Cisco network device. Network security is not a one-layer thing, yet, it depends on multiple factors. If you harden your devices, then it is a good starting point that increases the overall security of the environment you manage.
 
 ## Installation
@@ -18,31 +21,35 @@
 
 ```bash
 $ pip install ciscoconfaudit
 ```
 
 ## Usage
 
-You can try out two examples in the repo.
+You can try out _two examples_ in the repo in [examples](https://github.com/Tes3awy/cisco-config-auditor/tree/main/examples).
 
 ```bash
-(.venv) $ python3 online.py   # Parses config from a device (Uses netmiko)
-(.venv) $ python3 offline.py  # Parses config from text file
+(.venv) $ python3 basic_online.py   # Parses config from a device (Uses netmiko)
+(.venv) $ python3 basic_offline.py  # Parses config from text file
 ```
 
 ### Example Output
 
 | Global Config Audit (Sample)                                                                                     | Interface-Level Audit                                                                                                |
 | ---------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
 | ![Global Config Audit](https://github.com/Tes3awy/cisco-config-auditor/blob/main/assets/global-config-audit.jpg) | ![Interface Level Audit](https://github.com/Tes3awy/cisco-config-auditor/blob/main/assets/interface-level-audit.jpg) |
 
-## Credits
+## Use Case
 
-This package was inspired by [jonarm](https://github.com/jonarm) from [cisco-ios-audit](https://github.com/jonarm/cisco-ios-audit).
+- Ever been tired of checking whether the Cisco hardneing technqiues (_[here](https://www.cisco.com/c/en/us/support/docs/ios-nx-os-software/ios-xe-16/220270-use-cisco-ios-xe-hardening-guide.html)_) are applied to your network devices one by one? This package is very handy in generating a tabular report for you.
 
 ## Author
 
 [Osama Abbas](https://github.com/Tes3awy)
 
+## Credits
+
+This package was inspired by [jonarm](https://github.com/jonarm) from [cisco-ios-audit](https://github.com/jonarm/cisco-ios-audit).
+
 ## Contributions
 
 You are welcome to contribute to this Cisco [Swiss army knife](https://en.wikipedia.org/wiki/Swiss_Army_knife).
```

### Comparing `ciscoconfaudit-0.1.2/pyproject.toml` & `ciscoconfaudit-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "ciscoconfaudit"
-version = "0.1.2"
+version = "0.2.0"
 description = "A Cisco IOS & IOS-XE configuration audit tool"
-readme = "README.md"
-requires-python = ">=3.8"
+readme = { file = "README.md", content-type = "text/markdown" }
+requires-python = ">=3.8, <4"
 license = { file = "LICENSE" }
 keywords = ["cisco", "audit", "configuration audit"]
 authors = [{ name = "Osama Abbas", email = "oabbas2512@gmail.com" }]
 maintainers = [{ name = "Osama Abbas", email = "oabbas2512@gmail.com" }]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -22,39 +22,42 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Typing :: Typed",
 ]
 dependencies = ["ciscoconfparse", "rich"]
 
 [project.optional-dependencies]
-dev = ["pre-commit", "black", "isort"]
+dev = ["pre-commit", "bumpver", "black", "isort"]
 
 [project.urls]
-"Homepage" = "https://github.com/Tes3awy/cisco-config-auditor/"
-"Bug Tracker" = "https://github.com/Tes3awy/cisco-config-auditor/issues/"
+Homepage = "https://github.com/Tes3awy/cisco-config-auditor/"
+Repository = "https://github.com/Tes3awy/cisco-config-auditor/"
+Issues = "https://github.com/Tes3awy/cisco-config-auditor/issues/"
 "Say Thanks!" = "https://saythanks.io/to/Tes3awy"
-"Source" = "https://github.com/Tes3awy/cisco-config-auditor/"
+Source = "https://github.com/Tes3awy/cisco-config-auditor/"
+Changelog = "https://github.com/Tes3awy/cisco-config-auditor/CHANGELOG.md"
 
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.isort]
+profile = "black"
+
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 tag_message = "{new_version}"
 tag_scope = "default"
-pre_commit_hook = ""
-post_commit_hook = ""
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "src/ciscoconfaudit/__init__.py" = ['^__version__ = "{version}"$']
-"README.md" = ["{version}", "{pep440_version}"]
```

### Comparing `ciscoconfaudit-0.1.2/src/ciscoconfaudit/__init__.py` & `ciscoconfaudit-0.2.0/src/ciscoconfaudit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from ciscoconfparse import CiscoConfParse
 from rich.console import Console
 from rich.table import Table
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
 __all__ = ["ciscoconfaudit"]
 PY_MAJ_VER = 3
 PY_MIN_VER = 8
 MIN_PYTHON_VER = "3.8"
 
 FAIL = "[bold red]:heavy_multiplication_x: FAIL[/bold red]"
 PASS = "[bold green]:heavy_check_mark: PASS[/bold green]"
@@ -68,15 +68,15 @@
         else:
             self.global_table.add_row(cmd, RECOMMENDED)
 
     # Global Config Audit
     def global_config(self, running_config: str):
         # Parse configuration
         self.parse = CiscoConfParse(
-            running_config.splitlines(), syntax="ios", factory=True
+            running_config.splitlines(), syntax="ios", factory=True, read_only=True
         )
         hostname = self.parse.re_match_iter_typed(
             r"^hostname\s+(\S+)", default="Device"
         )
         self.global_table = self.create_table(f"{hostname} Global Config Audit")
         # Perform checks and populate the table
         self.check_service(
@@ -139,16 +139,20 @@
             "ip arp inspection vlan <vlan-range>",
         )
         self.check_config(
             r"^ip\sdhcp\ssnooping\sinformation\soption$",
             "ip dhcp snooping information option",
         )
         self.check_config(r"^ip\sssh\sversion\s2$", "ip ssh version 2")
+        self.check_config(r"^ip\sssh\stime-out\s60$", "ip ssh time-out 60")
+        self.check_config(
+            r"^ip\sssh\sauthentication-retries\s3$", "ip ssh authentication-retries 3"
+        )
         self.check_config(
-            r"^ip\sssh\sdh\smin\ssize\s\d{3,4}$", "ip ssh dh min size 2048"
+            r"^ip\sssh\sdh\smin\ssize\s(2048|4096)$", "ip ssh dh min size 2048|4096"
         )
         self.check_optional_config(
             r"^ip\sssh\sserver\salgorithm\sencryption\saes\d{3}-ctr\saes\d{3}-ctr\saes\d{3}-ctr$",
             "ip ssh server algorithm encryption aes128-ctr aes192-ctr aes256-ctr",
         )
         self.check_optional_config(
             r"^ip\sssh\sclient\salgorithm\sencryption\saes\d{3}-ctr\saes\d{3}-ctr\saes\d{3}-ctr$",
@@ -156,14 +160,15 @@
         )
         self.check_config(r"^no\sip\ssource-route$", "no ip source-route")
         self.check_config(r"^no\sipv6\ssource-route$", "no ipv6 source-route")
         self.check_config(
             r"^no\sip\sgratuitous-arps$|^no\sip\sarp\sgratuitous$",
             "no ip gratuitous-arps | no ip arp gratuitous",
         )
+        self.check_config(r"^ip\soptions\sdrop$", "ip options drop")
         self.check_config(r"^no\svstack$", "no vstack")
         self.check_config(r"^no\slogging\sconsole$", "no logging console")
         self.check_config(r"^no\slogging\smonitor$", "no logging monitor")
         self.check_config(
             r"^memory\sfree\slow-watermark\sprocessor\s\d{1,7}$",
             "memory free low-watermark processor <threshold>",
         )
@@ -175,16 +180,15 @@
             r"^memory\sreserve\scritical\s\d{1,10}$", "memory reserve critical <value>"
         )
         self.check_optional_config(
             r"^exception\scrashinfo\smaximum\sfiles\s\d+$",
             "exception crashinfo maximum files <number-of-files>",
         )
         self.check_optional_config(
-            r"^vtp\smode\stransparent$|^vtp\smode\soff$",
-            "vtp mode transparent | vtp mode off",
+            r"^vtp\smode\s(transparent|off)$", "vtp mode transparent|off"
         )
         self.check_optional_config(
             r"^no\ssystem\signore\sstartupconfig\sswitch\sall$",
             "no system ignore startupconfig switch all",
         )
         self.check_optional_config(
             r"^diagnostic\sbootup\slevel\sminimal$", "diagnostic bootup level minimal"
@@ -198,24 +202,28 @@
         self.check_optional_config(r"^login\son-success\slog$", "login on-success log")
         self.check_optional_config(r"^login\son-failure\slog$", "login on-failure log")
         self.check_optional_config(
             r"^clock\stimezone\s\w{3,4}\s-?\d{1,2}\s-?\d{1,2}$",
             "clock timezone <timezone> <hours_offset> <mintues_offset>",
         )
         self.check_config(r"^ntp\sserver\s\d", "ntp server")
+        # IOS and IOS-XE versions only
+        self.check_config(
+            r"^no\sntp\sallow\smode\scontrol\s0$", "no ntp allow mode control 0"
+        )
         self.check_config(
             r"^username\s\w+\sprivilege\s\d{1,2}\ssecret\s[8-9]\s",
             "username <username> privilege <priv_level> secret [8-9] <password>",
         )
         self.check_config(
             r"^enable\salgorithm-type\sscrypt\ssecret\s",
             "enable algorithm-type scrypt secret <password>",
         )
         # Check for AAA settings
-        if self.parse.find_lines("^no\saaa\snew-model$"):
+        if self.parse.find_lines(r"^no\saaa\snew-model$"):
             self.global_table.add_row("aaa new-model", FAIL)
         else:
             self.global_table.add_row("aaa new-model", PASS)
             # Authentication
             self.check_config(
                 r"^aaa\sauthentication\slogin\sdefault\sgroup\stacacs\+\senable$",
                 "aaa authentication login default group tacacs+ enable",
@@ -255,18 +263,18 @@
                 "aaa accounting commands 0 default start-stop group tacacs",
             )
             self.check_config(
                 r"^aaa\saccounting\scommands\s15\sdefault\sstart-stop\sgroup\stacacs",
                 "aaa accounting commands 15 default start-stop group tacacs",
             )
 
-        # Check for weak SNMP community strings
+        # Check for weak SNMPv2c community strings
         self.check_vuln_config(
             r"^snmp-server\scommunity\sprivate\srw$|^snmp-server\scommunity\spublic\sro$",
-            "Weak snmpv2c community string (Trivial authentication)",
+            "Weak SNMPv2c community string (Trivial authentication)",
         )
 
     # Interface-Level Audit
     def interface_config(self, running_config: str):
         self.parse = CiscoConfParse(
             running_config.splitlines(), syntax="ios", factory=True
         )
@@ -279,14 +287,15 @@
         self.check_port_security(self.parse)
         self.check_stp_portfast(self.parse)
         self.check_stp_bpdu(self.parse)
         self.check_stp_root(self.parse)
         self.check_cdp(self.parse)
         self.check_lldp(self.parse)
         self.check_ip_src_verify(self.parse)
+        self.check_sticky_mac(self.parse)
         self.check_arp_proxy(self.parse)
         self.check_ip_redirects(self.parse)
         self.check_ip_unreachables(self.parse)
         self.check_directed_broadcast(self.parse)
         self.check_lines(self.parse)
 
     def check_vlan1(self, parse: CiscoConfParse):
@@ -520,14 +529,44 @@
             if src_verify_pass / src_verify_total == 1:
                 self.interface_table.add_row(
                     "ip verify source (All access interfaces)", PASS
                 )
         except ZeroDivisionError:
             self.interface_table.add_row(f"ip verify source {ACC_INTF_VERIFY}", WARN)
 
+    def check_sticky_mac(self, parse: CiscoConfParse):
+        mac_sticky_total, mac_stick_pass = 0, 0
+        mac_sticky_intfs = parse.find_objects_w_child(
+            parentspec=r"^interface\s", childspec=IS_ACCESS_PORT
+        )
+        for mac_sticky_obj in mac_sticky_intfs:
+            if (
+                not mac_sticky_obj.re_search_children(r"^\sswitchport\sport-security$")
+                and mac_sticky_obj.re_search_children(
+                    r"^\sswitchport\sport-security\smac-address\ssticky$"
+                )
+                and not mac_sticky_obj.re_search_children(r"^\sshutdown$")
+            ):
+                self.interface_table.add_row(
+                    f"'{mac_sticky_obj.text}' switchport port-security mac-address sticky",
+                    FAIL,
+                )
+            else:
+                mac_stick_pass += 1
+            mac_sticky_total += 1
+        try:
+            if mac_stick_pass / mac_sticky_total == 1:
+                self.interface_table.add_row(
+                    "switchport port-security (All access interfaces)", PASS
+                )
+        except ZeroDivisionError:
+            self.interface_table.add_row(
+                f"switchport port-security mac-address sticky {ACC_INTF_VERIFY}", WARN
+            )
+
     # L3 interfaces
     def check_arp_proxy(self, parse: CiscoConfParse):
         if not bool(parse.find_objects(r"^ip\sarp\sproxy\sdisable$")):
             arp_intfs_total, arp_intfs_pass = 0, 0
             arp_intfs = parse.find_objects_w_child(
                 parentspec=r"^interface\s", childspec=r"^\sip\saddress\s"
             )
```

### Comparing `ciscoconfaudit-0.1.2/src/ciscoconfaudit.egg-info/PKG-INFO` & `ciscoconfaudit-0.2.0/src/ciscoconfaudit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscoconfaudit
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Cisco IOS & IOS-XE configuration audit tool
 Author-email: Osama Abbas <oabbas2512@gmail.com>
 Maintainer-email: Osama Abbas <oabbas2512@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -676,17 +676,19 @@
         into proprietary programs. If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library. If this is what you want to do, use the GNU Lesser General
         Public License instead of this License. But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://github.com/Tes3awy/cisco-config-auditor/
-Project-URL: Bug Tracker, https://github.com/Tes3awy/cisco-config-auditor/issues/
+Project-URL: Repository, https://github.com/Tes3awy/cisco-config-auditor/
+Project-URL: Issues, https://github.com/Tes3awy/cisco-config-auditor/issues/
 Project-URL: Say Thanks!, https://saythanks.io/to/Tes3awy
 Project-URL: Source, https://github.com/Tes3awy/cisco-config-auditor/
+Project-URL: Changelog, https://github.com/Tes3awy/cisco-config-auditor/CHANGELOG.md
 Keywords: cisco,audit,configuration audit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
@@ -697,33 +699,38 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
+Classifier: Typing :: Typed
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: ciscoconfparse
 Requires-Dist: rich
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 
-# Cisco Config Auditor
+# ciscoconfaudit
 
 [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/Tes3awy/cisco-config-auditor)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ciscoconfaudit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat-square&labelColor=ef8336)](https://pycqa.github.io/isort/)
 ![LICENSE](https://img.shields.io/github/license/Tes3awy/cisco-config-auditor?color=purple&style=flat-square&label=LICENSE)
 ![Commit Activity](https://img.shields.io/github/commit-activity/m/Tes3awy/cisco-config-auditor/main?logo=github&style=flat-square)
+![PyPI - Version](https://img.shields.io/pypi/v/ciscoconfaudit)
+![PyPI - Status](https://img.shields.io/pypi/status/ciscoconfaudit)
+[![Downloads](https://static.pepy.tech/badge/ciscoconfaudit)](https://pepy.tech/project/ciscoconfaudit)
 [![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/Tes3awy)
 
 > Based on [Use Cisco IOS XE Hardening Guide](https://www.cisco.com/c/en/us/support/docs/ios-nx-os-software/ios-xe-16/220270-use-cisco-ios-xe-hardening-guide.html) and some opinionated best practices.
 
 This package gives an overview of the hardening techniques that can be used to secure a Cisco network device. Network security is not a one-layer thing, yet, it depends on multiple factors. If you harden your devices, then it is a good starting point that increases the overall security of the environment you manage.
 
 ## Installation
@@ -732,31 +739,35 @@
 
 ```bash
 $ pip install ciscoconfaudit
 ```
 
 ## Usage
 
-You can try out two examples in the repo.
+You can try out _two examples_ in the repo in [examples](https://github.com/Tes3awy/cisco-config-auditor/tree/main/examples).
 
 ```bash
-(.venv) $ python3 online.py   # Parses config from a device (Uses netmiko)
-(.venv) $ python3 offline.py  # Parses config from text file
+(.venv) $ python3 basic_online.py   # Parses config from a device (Uses netmiko)
+(.venv) $ python3 basic_offline.py  # Parses config from text file
 ```
 
 ### Example Output
 
 | Global Config Audit (Sample)                                                                                     | Interface-Level Audit                                                                                                |
 | ---------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
 | ![Global Config Audit](https://github.com/Tes3awy/cisco-config-auditor/blob/main/assets/global-config-audit.jpg) | ![Interface Level Audit](https://github.com/Tes3awy/cisco-config-auditor/blob/main/assets/interface-level-audit.jpg) |
 
-## Credits
+## Use Case
 
-This package was inspired by [jonarm](https://github.com/jonarm) from [cisco-ios-audit](https://github.com/jonarm/cisco-ios-audit).
+- Ever been tired of checking whether the Cisco hardneing technqiues (_[here](https://www.cisco.com/c/en/us/support/docs/ios-nx-os-software/ios-xe-16/220270-use-cisco-ios-xe-hardening-guide.html)_) are applied to your network devices one by one? This package is very handy in generating a tabular report for you.
 
 ## Author
 
 [Osama Abbas](https://github.com/Tes3awy)
 
+## Credits
+
+This package was inspired by [jonarm](https://github.com/jonarm) from [cisco-ios-audit](https://github.com/jonarm/cisco-ios-audit).
+
 ## Contributions
 
 You are welcome to contribute to this Cisco [Swiss army knife](https://en.wikipedia.org/wiki/Swiss_Army_knife).
```

