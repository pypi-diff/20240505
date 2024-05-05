# Comparing `tmp/onboardme-1.7.1.tar.gz` & `tmp/onboardme-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardme-1.7.1.tar", max compression
+gzip compressed data, was "onboardme-1.8.0.tar", max compression
```

## Comparing `onboardme-1.7.1.tar` & `onboardme-1.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34523 2024-03-19 09:09:10.018936 onboardme-1.7.1/LICENSE.txt
--rw-r--r--   0        0        0    13530 2024-03-19 09:09:10.018936 onboardme-1.7.1/README.md
--rwxr-xr-x   0        0        0     7600 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/__init__.py
--rwxr-xr-x   0        0        0     3760 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/config/firewall/iptables.sh
--rw-r--r--   0        0        0       98 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/config/firewall/ufw/discord
--rw-r--r--   0        0        0     3093 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/console_logging.py
--rw-r--r--   0        0        0     2095 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/constants.py
--rw-r--r--   0        0        0     5641 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/dot_files.py
--rwxr-xr-x   0        0        0     6182 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/env_config.py
--rw-r--r--   0        0        0     2278 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/firewall.py
--rwxr-xr-x   0        0        0     6276 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/help_text.py
--rw-r--r--   0        0        0     3296 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/ide_setup.py
--rw-r--r--   0        0        0      760 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/misc.py
--rwxr-xr-x   0        0        0     8720 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/pkg_management.py
--rwxr-xr-x   0        0        0      233 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/scripts/update_apt_sources.sh
--rw-r--r--   0        0        0     3612 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/subproc.py
--rw-r--r--   0        0        0     1509 2024-03-19 09:09:10.042935 onboardme-1.7.1/onboardme/sudo_setup.py
--rw-r--r--   0        0        0     1738 2024-03-19 09:09:10.042935 onboardme-1.7.1/pyproject.toml
--rw-r--r--   0        0        0    14911 1970-01-01 00:00:00.000000 onboardme-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-05 11:01:40.521736 onboardme-1.8.0/LICENSE.txt
+-rw-r--r--   0        0        0    13512 2024-05-05 11:01:40.521736 onboardme-1.8.0/README.md
+-rwxr-xr-x   0        0        0     7598 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/__init__.py
+-rwxr-xr-x   0        0        0     3760 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/config/firewall/iptables.sh
+-rw-r--r--   0        0        0       98 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/config/firewall/ufw/discord
+-rw-r--r--   0        0        0     3093 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/console_logging.py
+-rw-r--r--   0        0        0     2069 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/constants.py
+-rw-r--r--   0        0        0     5641 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/dot_files.py
+-rwxr-xr-x   0        0        0     6204 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/env_config.py
+-rw-r--r--   0        0        0     2278 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/firewall.py
+-rwxr-xr-x   0        0        0     6276 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/help_text.py
+-rw-r--r--   0        0        0     3296 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/ide_setup.py
+-rw-r--r--   0        0        0      760 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/misc.py
+-rwxr-xr-x   0        0        0     8708 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/pkg_management.py
+-rwxr-xr-x   0        0        0      233 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/scripts/update_apt_sources.sh
+-rw-r--r--   0        0        0     3612 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/subproc.py
+-rw-r--r--   0        0        0     1483 2024-05-05 11:01:40.549736 onboardme-1.8.0/onboardme/sudo_setup.py
+-rw-r--r--   0        0        0     1803 2024-05-05 11:01:40.549736 onboardme-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0    14894 1970-01-01 00:00:00.000000 onboardme-1.8.0/PKG-INFO
```

### Comparing `onboardme-1.7.1/LICENSE.txt` & `onboardme-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onboardme-1.7.1/README.md` & `onboardme-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,52 +18,52 @@
 <img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/image_in_terminal.png' alt='screenshot of color samples and image of dog using a computer using sixel'>
 </p>
 
 ## Features
 
 <details>
   <summary><h4>Keep your Dot Files Up To Date Across multiple systems</h4></summary>
-  
+
 `onboardme` can manage your [dot files] using a git by turning your home directory into a repo.
 We even provide default dot files, so you don't have to manage them
 - The [default dot files] are open source, and the maintainers use these themselves
 - They cover a lot of common apps/tools you probably want anyway
 - They have consistent colorschemes accross different CLI/TUI programs 😃
 - They set all the helpful BASH aliases you could need (zsh support coming soon)
 
 </details>
 
 <details>
   <summary><h4>Package management accross multiple package managers<h4></summary>
-    
+
 We install and upgrade libraries and apps using common package managers. We also provide a currated list of default packages.
-  
+
 - checkout the [default packages]
 - supports `brew`, `apt`, `snap`, `flatpak`, and `pip` (and you can add your own 😄)
 - group together packages for different kinds of environments
   - onboardme provides default package groups:
     - default (no desktop GUI apps installed by default, always installed)
     - macOS (default apps for _macOS only_ apps, always installed on macOS)
     - gui (default GUI apps for Linux desktops, optionally installed)
     - devops (devops related tooling, optionally installed)
- 
+
 <sub>**Linux ARM Users NOTE**: `brew` is currently [unsupported on linux/arm64](https://docs.brew.sh/Homebrew-on-Linux#arm-unsupported), and as we'd have to compile everything from source anyway, we don't support running the brew package manager via onboardme on linux/arm64 or (AArch64) at all right now._
 We do have a docker image ([jessebot/onboardme:latest-arm](https://hub.docker.com/r/jessebot/onboardme)) optimized for arm though that you can run on AArch64 and it's perfect for a dockerized dev environment on an M1 or later mac or any other ARM 64 device that runs docker :)</sub>
 
 </details>
 
 <details>
   <summary><h4>NeoVim Plugin Installtion and Updates<h4></summary>
 
 
 `onboardme` keeps your neovim plugins installed and up to date with [lazy.nvim] under the hood.
-  
+
 <h4>Why no vim though?</h4>
-  
-If you haven't already made the switch from Vim to [NeoVim], you can try out NeoVim today with `onboardme` :D We used to support both neovim _and_ vim, but these days none of the primary developers of this repo use pure vim anymore, so we can't ensure it's up to standards. All of your knowledge from vim is still helpful in neovim though, and we highly recommend switching as neovim has a lot more features and a very active plugin community :) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/doc/user/nvim.html#nvim-from-vim). 
+
+If you haven't already made the switch from Vim to [NeoVim], you can try out NeoVim today with `onboardme` :D We used to support both neovim _and_ vim, but these days none of the primary developers of this repo use pure vim anymore, so we can't ensure it's up to standards. All of your knowledge from vim is still helpful in neovim though, and we highly recommend switching as neovim has a lot more features and a very active plugin community :) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/doc/user/nvim.html#nvim-from-vim).
 
 </details>
 
 <details>
   <summary><h4>Easy <code>yaml</code> config files using XDG Base Directory Spec<h4></summary>
 
 We use use [XDG Base Directory Spec] for config files, so you always know where they are :)
@@ -80,15 +80,15 @@
 The docker image is built nightly, and on push to `main` via GHA. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
 See the [dockerhub page](https://hub.docker.com/r/jessebot/onboardme) for more info!
 
 </details>
 
 <details>
   <summary><h4>Other optional configurations<h4></summary>
-    
+
 - Enable touchID for sudo on macOS
 - Add your user to the docker group
 - Install [nerdfonts](https://www.nerdfonts.com) (defaults to mononoki and Symbols Only)
 
 </details>
 
 ### Screenshots
@@ -127,15 +127,15 @@
 
 </details>
 
 # Installation
 
 ## Install Locally
 
-You'll need `curl`, `brew`, `git`, and Python 3.11 to get started. We have a setup script to install those (except `curl`) and help you get your environment to the XDG spec under <b>Locally</b>. For docker, see the section below.
+You'll need `curl`, `brew`, `git`, and Python 3.12 to get started. We have a setup script to install those (except `curl`) and help you get your environment to the XDG spec under <b>Locally</b>. For docker, see the section below.
 
 <details>
   <summary>Local prereq install script</summary>
 .
 <details>
   <summary><code>curl</code>, a pre-prereq</summary>
 
@@ -217,18 +217,18 @@
 # can also be done with: onboardme -O
 onboardme --overwrite
 ```
 
 You can read more in depth at the [Getting Started Docs] 💙! There's also more [docs] on basically every program that onboardme touches.
 
 ### Upgrades
-If you're on python 3.11, you should be able to do:
+If you're on python 3.12, you should be able to do:
 
 ```bash
-pip3.11 install --upgrade onboardme
+pip3.12 install --upgrade onboardme
 ```
 
 ## Under the Hood
 Made and tested for these operating systems:
 
 [![Tested on Ventura 13.4 with a 13-inch M1 Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en)
 [![Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://www.debian.org/)
```

### Comparing `onboardme-1.7.1/onboardme/__init__.py` & `onboardme-1.8.0/onboardme/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,23 +153,23 @@
         default=False,
         is_flag=True)
 @option('--version',
         is_flag=True,
         help=HELP['version'],
         default=False)
 def main(log_level, log_file,
-         steps, 
+         steps,
          git_url, git_branch, git_config_dir, overwrite,
          pkg_managers, pkg_groups,
          firewall, remote_host,
          no_upgrade,
          version) -> bool:
     """
-    If run with no options on Linux, it will install brew, pip3.11, apt,
-    flatpak, and snap packages. On mac, it only installs brew/pip3.11 packages.
+    If run with no options on Linux, it will install brew, pip3.12, apt,
+    flatpak, and snap packages. On mac, it only installs brew/pip3.12 packages.
     config loading tries to load: cli options and then defaults back to:
     $XDG_CONFIG_HOME/onboardme/config.yml
     """
 
     # only return the version if --version was passed in
     if version:
         print(f'\n🎉 v{VERSION}\n')
@@ -179,15 +179,15 @@
     check_os_support()
 
     # setup logging immediately
     log = setup_logger(log_level, log_file)
 
     # makes sure we only overwrite config file prefs if cli opts are passed in
     usr_pref = process_configs(overwrite, git_url, git_branch, git_config_dir,
-                               pkg_managers, pkg_groups, 
+                               pkg_managers, pkg_groups,
                                firewall, remote_host,
                                steps,
                                log_file, log_level)
 
     if log:
         log.debug(f"User passed in the following preferences:\n{usr_pref}\n")
     else:
```

### Comparing `onboardme-1.7.1/onboardme/config/firewall/iptables.sh` & `onboardme-1.8.0/onboardme/config/firewall/iptables.sh`

 * *Files identical despite different names*

### Comparing `onboardme-1.7.1/onboardme/console_logging.py` & `onboardme-1.8.0/onboardme/console_logging.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.7.1/onboardme/constants.py` & `onboardme-1.8.0/onboardme/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3.11
 """
        Name:
 DESCRIPTION:
      AUTHOR:
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version 3
 """
 from importlib.metadata import version as get_version
@@ -29,15 +28,15 @@
 
 # step config is different per OS
 STEPS = ['dot_files','packages','font_setup','neovim_setup','group_setup']
 if OS[0] == 'Darwin':
     STEPS.append('sudo_setup')
 
 # package manager config is different per OS
-PKG_MNGRS = ['brew','pip3.11']
+PKG_MNGRS = ['brew','pip3.12']
 if OS[0] == 'Linux':
     PKG_MNGRS.extend(['apt','snap','flatpak'])
 
 
 default_dotfiles = ("https://raw.githubusercontent.com/jessebot/dot_files/"
                     "main/.config/onboardme/")
```

### Comparing `onboardme-1.7.1/onboardme/dot_files.py` & `onboardme-1.8.0/onboardme/dot_files.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.7.1/onboardme/env_config.py` & `onboardme-1.8.0/onboardme/env_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,17 @@
 
 def sort_pkgmngrs(package_managers_list: list) -> list:
     """
     make sure the package managers are in the right order 🤦
     e.g. apt installs snap and flatpak, so niether can be run until apt is run
 
     Takes list of package manager str and reorders them be (if they exist):
-       ['brew', 'pip3.11', 'apt', 'snap', 'flatpak']
+       ['brew', 'pip3.12', 'pip3.11', 'apt', 'snap', 'flatpak']
     """
-    pkg_mngr_default_order = ['brew', 'pip3.11', 'apt', 'snap', 'flatpak']
+    pkg_mngr_default_order = ['brew', 'pip3.12', 'pip3.11', 'apt', 'snap', 'flatpak']
 
     # Rearrange list by other list order Using list comprehension
     return [ele for ele in pkg_mngr_default_order if ele in package_managers_list]
 
 
 def fill_in_defaults(defaults: dict, user_config: dict,
                      always_prefer_default=False) -> dict:
```

### Comparing `onboardme-1.7.1/onboardme/firewall.py` & `onboardme-1.8.0/onboardme/firewall.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.7.1/onboardme/help_text.py` & `onboardme-1.8.0/onboardme/help_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         '[b]Overwrites[/b] existing dot files with files from configured '
         "[option]--git_url[/option] repo. If you've set overwrite: true in "
         'your config, then --overwrite on the command line will act as a '
         'toggle, so it will NOT overwrite your dot files.',
 
         'pkg_managers':
         f'Specific [meta]PKG_MANAGER[/] to run. {pkg_mngr_choices}'
-        '\nExample: [switch]-p[/] [meta]brew[/] [switch]-p[/] [meta]pip3.11',
+        '\nExample: [switch]-p[/] [meta]brew[/] [switch]-p[/] [meta]pip3.12',
 
         'pkg_groups':
         f"Package groups to install.\n{pkg_group_choices}\nExample:"
         " [switch]-g[/] [meta]devops[/] [switch]-g[/switch] [meta]gaming",
 
         'no_upgrade':
         "Do not upgrade the existing brew or apt packages.",
```

### Comparing `onboardme-1.7.1/onboardme/ide_setup.py` & `onboardme-1.8.0/onboardme/ide_setup.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.7.1/onboardme/misc.py` & `onboardme-1.8.0/onboardme/misc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.7.1/onboardme/pkg_management.py` & `onboardme-1.8.0/onboardme/pkg_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
     # the new github.com keys are not automatically added :( so we do it here
     with open(known_hosts_file, 'a') as known_hosts:
         for line in github_keys.split('/n'):
             known_hosts.write(line)
 
 
-def run_preinstall_cmds(cmd_list: list, 
-                        pkg_groups: list, 
+def run_preinstall_cmds(cmd_list: list,
+                        pkg_groups: list,
                         no_upgrade: bool) -> None:
     """
     takes a list of package manager pre-install commands and runs them
     if second list of package groups contains gaming, runs additional commands
     returns True
     """
     run_gaming_setup = False
@@ -73,15 +73,15 @@
 
             subproc([cmd_list[pre_cmd]], spinner=SPINNER)
             sub_header(f"[b]{pre_cmd.title()}[/b] completed.")
 
 
 def run_pkg_mngrs(pkg_mngrs: list, pkg_groups=[], no_upgrade=bool) -> None:
     """
-    Installs brew and pip3.11 packages. Also apt, snap, and flatpak on Linux.
+    Installs brew and pip3.12 packages. Also apt, snap, and flatpak on Linux.
     Takes optional variables:
       - pkg_groups: list of optional package groups
       - pkg_mngrs: list of package managers to run
     Returns True
     """
     log.debug(f"passed in pkg_mngrs: {pkg_mngrs}\npkg_groups: {pkg_groups}")
 
@@ -90,15 +90,15 @@
     pkg_mngrs_list_of_dicts = load_cfg('packages.yml')
     # we iterate through pkg_mngrs which should already be sorted
     for pkg_mngr in pkg_mngrs:
         pkg_mngr_dict = pkg_mngrs_list_of_dicts[pkg_mngr]
 
         available_pkg_groups = pkg_mngr_dict['packages']
         log.debug(f"pkg groups for {pkg_mngr} are {available_pkg_groups}")
-        
+
         # brew has a special flow because it works on both linux and mac
         if pkg_mngr == 'brew':
             if 'Darwin' in OS:
                 if 'default' in pkg_groups:
                     if type(pkg_groups) is tuple:
                         pkg_groups = list(pkg_groups)
                     pkg_groups.append("macOS")
@@ -152,17 +152,17 @@
 
             # run final cleanup commands, if any
             if 'cleanup' in pkg_cmds:
                 subproc([pkg_cmds['cleanup']])
                 sub_header("[b]Cleanup[/b] step Completed.")
 
 
-def install_pkg_group(install_cmd: str, 
+def install_pkg_group(install_cmd: str,
                       pkgs_to_install: list,
-                      installed_pkgs: list, 
+                      installed_pkgs: list,
                       install_env_vars: dict,
                       no_upgrade: bool
                       ) -> None:
     """
     Installs packages if they are not already installed.
     provided install command string.
     Returns True.
```

### Comparing `onboardme-1.7.1/onboardme/subproc.py` & `onboardme-1.8.0/onboardme/subproc.py`

 * *Files identical despite different names*

### Comparing `onboardme-1.7.1/onboardme/sudo_setup.py` & `onboardme-1.8.0/onboardme/sudo_setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3.11
 """
        Name: onbaordme.sudo_setup
 DESCRIPTION: setup pam module for sudo and add user to sudo group
      AUTHOR: Jesse Hitch
     LICENSE: GNU AFFERO GENERAL PUBLIC LICENSE Version 3
 """
 from os import geteuid
```

### Comparing `onboardme-1.7.1/pyproject.toml` & `onboardme-1.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [tool.poetry]
 name          = "onboardme"
-version       = "1.7.1"
+version       = "1.8.0"
 description   = "Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS."
 authors       = [
     "Jesse Hitch <jessebot@linux.com>",
     "Max Roby <emax@cloudydev.net>"
 ]
 license       = "AGPL-3.0-or-later"
 readme        = "README.md"
 documentation = "https://jessebot.github.io/onboardme/onboardme"
 repository    = "http://github.com/jessebot/onboardme"
 keywords      = ["onboardme", "onboarding", "desktop-setup", "development-environment"]
 classifiers   = ["Development Status :: 3 - Alpha",
                  "Programming Language :: Python :: 3.11",
+                 "Programming Language :: Python :: 3.12",
                  "Operating System :: MacOS :: MacOS X",
                  "Operating System :: POSIX :: Linux",
                  "Intended Audience :: End Users/Desktop",
                  "Topic :: System :: Installation/Setup",
                  "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)"]
 packages      = [{include = "onboardme"}]
 include       = ["onboardme/scripts/update_apt_sources.sh"]
 
 [tool.poetry.dependencies]
-python              = "^3.11"
+python             = ">=3.11,<3.13"
 click               = "^8.1"
 rich                = "^13.6"
 PyYAML              = "^6.0"
 GitPython           = "^3.1"
 wget                = "^3.2"
 xdg-base-dirs       = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.5"
+pre-commit = "^3.7"
 
 [tool.poetry.plugins."onboardme.application.plugin"]
 "onboardme" = "onboardme:main"
 
 [tool.poetry.scripts]
 onboardme = 'onboardme:main'
```

### Comparing `onboardme-1.7.1/PKG-INFO` & `onboardme-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: onboardme
-Version: 1.7.1
+Version: 1.8.0
 Summary: Install dot files and packages, including a base mode with sensible defaults to run on most computers running Debian based distros or macOS.
 Home-page: http://github.com/jessebot/onboardme
 License: AGPL-3.0-or-later
 Keywords: onboardme,onboarding,desktop-setup,development-environment
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11,<3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -48,52 +48,52 @@
 <img width="90%" src='https://raw.githubusercontent.com/jessebot/onboardme/main/docs/onboardme/screenshots/image_in_terminal.png' alt='screenshot of color samples and image of dog using a computer using sixel'>
 </p>
 
 ## Features
 
 <details>
   <summary><h4>Keep your Dot Files Up To Date Across multiple systems</h4></summary>
-  
+
 `onboardme` can manage your [dot files] using a git by turning your home directory into a repo.
 We even provide default dot files, so you don't have to manage them
 - The [default dot files] are open source, and the maintainers use these themselves
 - They cover a lot of common apps/tools you probably want anyway
 - They have consistent colorschemes accross different CLI/TUI programs 😃
 - They set all the helpful BASH aliases you could need (zsh support coming soon)
 
 </details>
 
 <details>
   <summary><h4>Package management accross multiple package managers<h4></summary>
-    
+
 We install and upgrade libraries and apps using common package managers. We also provide a currated list of default packages.
-  
+
 - checkout the [default packages]
 - supports `brew`, `apt`, `snap`, `flatpak`, and `pip` (and you can add your own 😄)
 - group together packages for different kinds of environments
   - onboardme provides default package groups:
     - default (no desktop GUI apps installed by default, always installed)
     - macOS (default apps for _macOS only_ apps, always installed on macOS)
     - gui (default GUI apps for Linux desktops, optionally installed)
     - devops (devops related tooling, optionally installed)
- 
+
 <sub>**Linux ARM Users NOTE**: `brew` is currently [unsupported on linux/arm64](https://docs.brew.sh/Homebrew-on-Linux#arm-unsupported), and as we'd have to compile everything from source anyway, we don't support running the brew package manager via onboardme on linux/arm64 or (AArch64) at all right now._
 We do have a docker image ([jessebot/onboardme:latest-arm](https://hub.docker.com/r/jessebot/onboardme)) optimized for arm though that you can run on AArch64 and it's perfect for a dockerized dev environment on an M1 or later mac or any other ARM 64 device that runs docker :)</sub>
 
 </details>
 
 <details>
   <summary><h4>NeoVim Plugin Installtion and Updates<h4></summary>
 
 
 `onboardme` keeps your neovim plugins installed and up to date with [lazy.nvim] under the hood.
-  
+
 <h4>Why no vim though?</h4>
-  
-If you haven't already made the switch from Vim to [NeoVim], you can try out NeoVim today with `onboardme` :D We used to support both neovim _and_ vim, but these days none of the primary developers of this repo use pure vim anymore, so we can't ensure it's up to standards. All of your knowledge from vim is still helpful in neovim though, and we highly recommend switching as neovim has a lot more features and a very active plugin community :) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/doc/user/nvim.html#nvim-from-vim). 
+
+If you haven't already made the switch from Vim to [NeoVim], you can try out NeoVim today with `onboardme` :D We used to support both neovim _and_ vim, but these days none of the primary developers of this repo use pure vim anymore, so we can't ensure it's up to standards. All of your knowledge from vim is still helpful in neovim though, and we highly recommend switching as neovim has a lot more features and a very active plugin community :) NeoVim maintains a guide on how to switch from vim [here](https://neovim.io/doc/user/nvim.html#nvim-from-vim).
 
 </details>
 
 <details>
   <summary><h4>Easy <code>yaml</code> config files using XDG Base Directory Spec<h4></summary>
 
 We use use [XDG Base Directory Spec] for config files, so you always know where they are :)
@@ -110,15 +110,15 @@
 The docker image is built nightly, and on push to `main` via GHA. The base image is `debian:bookworm`, but we will rollout support for Ubuntu down the line :)
 See the [dockerhub page](https://hub.docker.com/r/jessebot/onboardme) for more info!
 
 </details>
 
 <details>
   <summary><h4>Other optional configurations<h4></summary>
-    
+
 - Enable touchID for sudo on macOS
 - Add your user to the docker group
 - Install [nerdfonts](https://www.nerdfonts.com) (defaults to mononoki and Symbols Only)
 
 </details>
 
 ### Screenshots
@@ -157,15 +157,15 @@
 
 </details>
 
 # Installation
 
 ## Install Locally
 
-You'll need `curl`, `brew`, `git`, and Python 3.11 to get started. We have a setup script to install those (except `curl`) and help you get your environment to the XDG spec under <b>Locally</b>. For docker, see the section below.
+You'll need `curl`, `brew`, `git`, and Python 3.12 to get started. We have a setup script to install those (except `curl`) and help you get your environment to the XDG spec under <b>Locally</b>. For docker, see the section below.
 
 <details>
   <summary>Local prereq install script</summary>
 .
 <details>
   <summary><code>curl</code>, a pre-prereq</summary>
 
@@ -247,18 +247,18 @@
 # can also be done with: onboardme -O
 onboardme --overwrite
 ```
 
 You can read more in depth at the [Getting Started Docs] 💙! There's also more [docs] on basically every program that onboardme touches.
 
 ### Upgrades
-If you're on python 3.11, you should be able to do:
+If you're on python 3.12, you should be able to do:
 
 ```bash
-pip3.11 install --upgrade onboardme
+pip3.12 install --upgrade onboardme
 ```
 
 ## Under the Hood
 Made and tested for these operating systems:
 
 [![Tested on Ventura 13.4 with a 13-inch M1 Macbook pro and a 13-inch AMD 1,4 GHz Quad-Core Intel Core i5 2020 Macbook Pro](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)](https://wikiless.org/wiki/MacOS?lang=en)
 [![Tested only on Debian Bookworm (debian:bookworm)](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)](https://www.debian.org/)
```

