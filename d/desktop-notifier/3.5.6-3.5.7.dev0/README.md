# Comparing `tmp/desktop-notifier-3.5.6.tar.gz` & `tmp/desktop_notifier-3.5.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desktop-notifier-3.5.6.tar", last modified: Tue Jul 11 07:03:06 2023, max compression
+gzip compressed data, was "desktop_notifier-3.5.7.dev0.tar", last modified: Sun May  5 12:30:13 2024, max compression
```

## Comparing `desktop-notifier-3.5.6.tar` & `desktop_notifier-3.5.7.dev0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:03:06.227639 desktop-notifier-3.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-11 07:03:06.223639 desktop-notifier-3.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 07:03:06.227639 desktop-notifier-3.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:03:06.219639 desktop-notifier-3.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:03:06.223639 desktop-notifier-3.5.6/src/desktop_notifier/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/dbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14957 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/macos_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/macos_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    13403 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:03:06.223639 desktop-notifier-3.5.6/src/desktop_notifier/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/resources/python.png
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-11 07:02:53.000000 desktop-notifier-3.5.6/src/desktop_notifier/winrt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 07:03:06.223639 desktop-notifier-3.5.6/src/desktop_notifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-07-11 07:03:06.000000 desktop-notifier-3.5.6/src/desktop_notifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-11 07:03:06.000000 desktop-notifier-3.5.6/src/desktop_notifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 07:03:06.000000 desktop-notifier-3.5.6/src/desktop_notifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-11 07:03:06.000000 desktop-notifier-3.5.6/src/desktop_notifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 07:03:06.000000 desktop-notifier-3.5.6/src/desktop_notifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:30:13.241673 desktop_notifier-3.5.7.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-05 12:30:13.241673 desktop_notifier-3.5.7.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:30:13.241673 desktop_notifier-3.5.7.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:30:13.233673 desktop_notifier-3.5.7.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:30:13.237673 desktop_notifier-3.5.7.dev0/src/desktop_notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/dbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15022 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/macos_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/macos_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:30:13.237673 desktop_notifier-3.5.7.dev0/src/desktop_notifier/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/resources/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-05 12:30:06.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier/winrt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:30:13.237673 desktop_notifier-3.5.7.dev0/src/desktop_notifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-05 12:30:13.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-05 12:30:13.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:30:13.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-05 12:30:13.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-05 12:30:13.000000 desktop_notifier-3.5.7.dev0/src/desktop_notifier.egg-info/top_level.txt
```

### Comparing `desktop-notifier-3.5.6/LICENSE` & `desktop_notifier-3.5.7.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.6/PKG-INFO` & `desktop_notifier-3.5.7.dev0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.6
+Version: 3.5.7.dev0
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -15,30 +15,50 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: packaging
+Requires-Dist: dbus-next; sys_platform == "linux"
+Requires-Dist: rubicon-objc; sys_platform == "darwin"
+Requires-Dist: winrt-windows.applicationmodel.core; sys_platform == "win32"
+Requires-Dist: winrt-windows.data.xml.dom; sys_platform == "win32"
+Requires-Dist: winrt-windows.foundation; sys_platform == "win32"
+Requires-Dist: winrt-windows.foundation.collections; sys_platform == "win32"
+Requires-Dist: winrt-windows.foundation.interop; sys_platform == "win32"
+Requires-Dist: winrt-windows.ui.notifications; sys_platform == "win32"
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bump2version; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: flake8-pyproject; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: furo==2024.4.27; extra == "docs"
+Requires-Dist: sphinx==7.3.7; extra == "docs"
+Requires-Dist: sphinx-autoapi==3.0.0; extra == "docs"
+Requires-Dist: sphinx-mdinclude==0.6.0; extra == "docs"
 
 [![PyPi Release](https://img.shields.io/pypi/v/desktop-notifier.svg)](https://pypi.org/project/desktop-notifier/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/desktop-notifier.svg)](https://pypi.org/pypi/desktop-notifier/)
 [![Documentation Status](https://readthedocs.org/projects/desktop-notifier/badge/?version=latest)](https://desktop-notifier.readthedocs.io/en/latest/?badge=latest)
 
 # Desktop Notifier
 
 `desktop-notifier`  is a Python library for cross-platform desktop notifications.
 Currently supported platforms are:
 
 * Linux via the dbus service org.freedesktop.Notifications
 * macOS and iOS via the Notification Center framework
-* [**exprimental**] Windows via the WinRT / Python bridge.
+* [**experimental**] Windows via the WinRT / Python bridge.
 
 ![gif](screenshots/macOS.gif)
 
 ## Features
 
 `desktop-notifier` aims to be a good citizen of the platforms which it supports. It
 therefore stays within the limits of the native platform APIs and does not try to work
```

### Comparing `desktop-notifier-3.5.6/README.md` & `desktop_notifier-3.5.7.dev0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Desktop Notifier
 
 `desktop-notifier`  is a Python library for cross-platform desktop notifications.
 Currently supported platforms are:
 
 * Linux via the dbus service org.freedesktop.Notifications
 * macOS and iOS via the Notification Center framework
-* [**exprimental**] Windows via the WinRT / Python bridge.
+* [**experimental**] Windows via the WinRT / Python bridge.
 
 ![gif](screenshots/macOS.gif)
 
 ## Features
 
 `desktop-notifier` aims to be a good citizen of the platforms which it supports. It
 therefore stays within the limits of the native platform APIs and does not try to work
```

### Comparing `desktop-notifier-3.5.6/pyproject.toml` & `desktop_notifier-3.5.7.dev0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "desktop-notifier"
-version = "3.5.6"
+version = "3.5.7.dev0"
 authors = [{name = "Sam Schott", email = "sam.schott@outlook.com"}]
 license = {text = "MIT"}
 description = "Python library for cross-platform desktop notifications"
 keywords = ["desktop-notifier"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
@@ -23,15 +23,20 @@
     "Programming Language :: Python :: 3 :: Only",
 ]
 requires-python = ">=3.7"
 dependencies = [
     "packaging",
     "dbus-next;sys_platform=='linux'",
     "rubicon-objc;sys_platform=='darwin'",
-    "winsdk==1.0.0b9;sys_platform=='win32'",
+    "winrt-windows.applicationmodel.core;sys_platform=='win32'",
+    "winrt-windows.data.xml.dom;sys_platform=='win32'",
+    "winrt-windows.foundation;sys_platform=='win32'",
+    "winrt-windows.foundation.collections;sys_platform=='win32'",
+    "winrt-windows.foundation.interop;sys_platform=='win32'",
+    "winrt-windows.ui.notifications;sys_platform=='win32'",
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
@@ -40,23 +45,22 @@
 [project.optional-dependencies]
 dev = [
     "black",
     "bump2version",
     "flake8",
     "flake8-pyproject",
     "mypy",
-    "pre-commit",
     "pytest",
     "pytest-cov",
 ]
 docs = [
-    "furo==2023.5.20",
-    "sphinx==7.0.1",
-    "sphinx-autoapi==2.1.1",
-    "sphinx-mdinclude==0.5.3",
+    "furo==2024.4.27",
+    "sphinx==7.3.7",
+    "sphinx-autoapi==3.0.0",
+    "sphinx-mdinclude==0.6.0",
 ]
 
 [tool.setuptools.package-data]
 desktop_notifier = ["**/*.png"]
 
 [tool.flake8]
 ignore = "E203,E501,W503,H306"
```

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier/base.py` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 must inherit from :class:`DesktopNotifierBase`.
 """
 
 from __future__ import annotations
 
 # system imports
 import logging
+import platform
 from enum import Enum
 from collections import deque
 from pathlib import Path
 from typing import (
     Dict,
     Callable,
     Any,
@@ -132,40 +133,44 @@
         on_clicked: Callable[[], Any] | None = None,
         on_dismissed: Callable[[], Any] | None = None,
         attachment: str | None = None,
         sound: bool = False,
         thread: str | None = None,
         timeout: int = -1,
     ) -> None:
-        self._identifier: str | int | None = None
+        self._winrt_identifier = ""
+        self._macos_identifier = ""
+        self._dbus_identifier = 0
+
         self.title = title
         self.message = message
         self.urgency = urgency
         self.icon = icon
         self.buttons = buttons
         self.reply_field = reply_field
         self.on_clicked = on_clicked
         self.on_dismissed = on_dismissed
         self.attachment = attachment
         self.sound = sound
         self.thread = thread
         self.timeout = timeout
 
     @property
-    def identifier(self) -> str | int | None:
-        """
-        An platform identifier which gets assigned to the notification after it was
-        sent. This may be a str or int.
-        """
-        return self._identifier
-
-    @identifier.setter
-    def identifier(self, value: str | int | None) -> None:
-        """Setter: identifier"""
-        self._identifier = value
+    def identifier(self) -> str:
+        if platform.system() == "Darwin":
+            return self._macos_identifier
+        elif platform.system() == "Linux":
+            if self._dbus_identifier == 0:
+                return ""
+            else:
+                return str(self._dbus_identifier)
+        elif platform.system() == "Windows":
+            return self._winrt_identifier
+        else:
+            raise RuntimeError(f"Unsupported platform {platform.system()}")
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}(title='{self.title}', message='{self.message}')>"
 
 
 class DesktopNotifierBase:
     """Base class for desktop notifier implementations
@@ -213,27 +218,26 @@
 
         if len(self._current_notifications) == self.notification_limit:
             notification_to_replace = self._current_notifications.popleft()
         else:
             notification_to_replace = None
 
         try:
-            platform_nid = await self._send(notification, notification_to_replace)
+            await self._send(notification, notification_to_replace)
         except Exception:
             # Notifications can fail for many reasons:
             # The dbus service may not be available, we might be in a headless session,
             # etc. Since notifications are not critical to an application, we only emit
             # a warning.
             if notification_to_replace:
                 self._current_notifications.appendleft(notification_to_replace)
             logger.warning("Notification failed", exc_info=True)
         else:
-            notification.identifier = platform_nid
             self._current_notifications.append(notification)
-            self._notification_for_nid[platform_nid] = notification
+            self._notification_for_nid[notification.identifier] = notification
 
     def _clear_notification_from_cache(self, notification: Notification) -> None:
         """
         Removes the notification from our cache. Should be called by backends when the
         notification is closed.
         """
         try:
@@ -247,15 +251,15 @@
             except KeyError:
                 pass
 
     async def _send(
         self,
         notification: Notification,
         notification_to_replace: Notification | None,
-    ) -> str | int:
+    ) -> None:
         """
         Method to send a notification via the platform. This should be implemented by
         subclasses.
 
         Implementations must raise an exception when the notification could not be
         delivered. If the notification could be delivered but not fully as intended,
         e.g., because associated resources could not be loaded, implementations should
```

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier/dbus.py` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier/dbus.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 event loop.
 """
 
 from __future__ import annotations
 
 # system imports
 import logging
-from typing import TypeVar, cast
+from typing import TypeVar
 
 # external imports
-from dbus_next import Variant
-from dbus_next.aio import MessageBus, ProxyInterface
+from dbus_next.signature import Variant
+from dbus_next.aio.message_bus import MessageBus
+from dbus_next.aio.proxy_object import ProxyInterface
 
 # local imports
 from .base import Notification, DesktopNotifierBase, Urgency
 
 
 __all__ = ["DBusDesktopNotifier"]
 
@@ -35,17 +36,14 @@
     """DBus notification backend for Linux
 
     This implements the org.freedesktop.Notifications standard. The DBUS connection is
     created in a thread with a running asyncio loop to handle clicked notifications.
 
     :param app_name: The name of the app. If it matches the application name in an
         existing desktop entry, the icon from that entry will be used by default.
-    :param app_icon: The default icon to use for notifications. Will take precedence
-        over any icon from the desktop file. Should be a URI or a name in a
-        freedesktop.org-compliant icon theme.
     :param notification_limit: Maximum number of notifications to keep in the system's
         notification center.
     """
 
     _to_native_urgency = {
         Urgency.Low: Variant("y", 0),
         Urgency.Normal: Variant("y", 1),
@@ -85,43 +83,41 @@
             introspection,
         )
         self.interface = self.proxy_object.get_interface(
             "org.freedesktop.Notifications"
         )
 
         # Some older interfaces may not support notification actions.
-
         if hasattr(self.interface, "on_notification_closed"):
             self.interface.on_notification_closed(self._on_closed)
 
         if hasattr(self.interface, "on_action_invoked"):
             self.interface.on_action_invoked(self._on_action)
 
         return self.interface
 
     async def _send(
         self,
         notification: Notification,
         notification_to_replace: Notification | None,
-    ) -> int:
+    ) -> None:
         """
         Asynchronously sends a notification via the Dbus interface.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
         if not self.interface:
             self.interface = await self._init_dbus()
 
         if notification_to_replace:
-            replaces_nid = notification_to_replace.identifier
+            replaces_nid = notification_to_replace._dbus_identifier
         else:
             replaces_nid = 0
 
-        # Create list of actions for a user interacting with the notification.
         actions = []
 
         if notification.on_clicked:
             # The "default" action is typically invoked when clicking on the
             # notification body itself, see
             # https://specifications.freedesktop.org/notification-spec. There are some
             # exceptions though, such as XFCE, where this will result in a separate
@@ -130,59 +126,61 @@
             actions = ["default", ""]
 
         for n, button in enumerate(notification.buttons):
             actions += [str(n), button.title]
 
         hints = {"urgency": self._to_native_urgency[notification.urgency]}
 
-        # sound
         if notification.sound:
             hints["sound-name"] = Variant("s", "message-new-instant")
 
-        # attachment
         if notification.attachment:
             hints["image-path"] = Variant("s", notification.attachment)
 
-        # get the timeout in ms
         timeout = notification.timeout * 1000 if notification.timeout != -1 else -1
 
-        # Post the new notification and record the platform ID assigned to it.
-        platform_nid = await self.interface.call_notify(
-            self.app_name,  # app_name
-            replaces_nid,  # replaces_id
-            notification.icon or "",  # app_icon
-            notification.title,  # summary
-            notification.message,  # body
-            actions,  # actions
-            hints,  # hints
-            timeout,  # expire_timeout (-1 = default)
-        )
+        # dbus_next proxy APIs are generated at runtime.
+        if hasattr(self.interface, "call_notify"):
+            platform_nid = await self.interface.call_notify(
+                self.app_name,
+                replaces_nid,
+                notification.icon or "",
+                notification.title,
+                notification.message,
+                actions,
+                hints,
+                timeout,
+            )
 
-        return cast(int, platform_nid)
+            notification._dbus_identifier = platform_nid
 
     async def _clear(self, notification: Notification) -> None:
         """
         Asynchronously removes a notification from the notification center
         """
-
         if not self.interface:
             return
 
-        await self.interface.call_close_notification(notification.identifier)
+        # dbus_next proxy APIs are generated at runtime.
+        if hasattr(self.interface, "call_close_notification"):
+            await self.interface.call_close_notification(notification._dbus_identifier)
 
     async def _clear_all(self) -> None:
         """
         Asynchronously clears all notifications from notification center
         """
-
         if not self.interface:
             return
 
-        for notification in self.current_notifications:
-            await self.interface.call_close_notification(notification.identifier)
+        # dbus_next proxy APIs are generated at runtime.
+        if hasattr(self.interface, "call_close_notification"):
+            for notification in self.current_notifications:
+                await self.interface.call_close_notification(
+                    notification._dbus_identifier
+                )
 
     # Note that _on_action and _on_closed might be called for the same notification
     # with some notification servers. This is not a problem because the _on_action
     # call will come first, in which case we are no longer interested in calling the
     # on_dismissed callback.
 
     def _on_action(self, nid: int, action_key: str) -> None:
```

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier/dummy.py` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier/dummy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Dummy backend for unsupported platforms.
 """
 
 from __future__ import annotations
 
-# system imports
-import uuid
-
 # local imports
 from .base import Notification, DesktopNotifierBase
 
 
 class DummyNotificationCenter(DesktopNotifierBase):
     """A dummy backend for unsupported platforms"""
 
@@ -36,18 +33,15 @@
         """
         return True
 
     async def _send(
         self,
         notification: Notification,
         notification_to_replace: Notification | None,
-    ) -> str:
-        if notification_to_replace:
-            return str(notification_to_replace.identifier)
-        else:
-            return str(uuid.uuid4())
+    ) -> None:
+        pass
 
     async def _clear(self, notification: Notification) -> None:
         pass
 
     async def _clear_all(self) -> None:
         pass
```

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier/macos.py` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier/macos.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     """Delegate to handle user interactions with notifications"""
 
     @objc_method  # type:ignore
     def userNotificationCenter_didReceiveNotificationResponse_withCompletionHandler_(
         self, center, response, completion_handler: objc_block
     ) -> None:
         # Get the notification which was clicked from the platform ID.
-        platform_nid = py_from_ns(response.notification.request.identifier)
+        platform_nid = py_from_ns(response.notification.request._macos_identifier)
         py_notification = self.interface._notification_for_nid[platform_nid]
         py_notification = cast(Notification, py_notification)
 
         self.interface._clear_notification_from_cache(py_notification)
 
         # Invoke the callback which corresponds to the user interaction.
         if response.actionIdentifier == UNNotificationDefaultActionIdentifier:
@@ -223,24 +223,24 @@
 
         return authorized
 
     async def _send(
         self,
         notification: Notification,
         notification_to_replace: Optional[Notification],
-    ) -> str:
+    ) -> None:
         """
         Uses UNUserNotificationCenter to schedule a notification.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
 
         if notification_to_replace:
-            platform_nid = str(notification_to_replace.identifier)
+            platform_nid = notification_to_replace._macos_identifier
         else:
             platform_nid = str(uuid.uuid4())
 
         # On macOS, we need to register a new notification category for every
         # unique set of buttons.
         category_id = await self._create_category_for_notification(notification)
 
@@ -303,15 +303,15 @@
                     # the error.
                     logger.warning(
                         f"{error.localizedDescription}: {notification.attachment}"  # type:ignore
                     )
             else:
                 raise RuntimeError(error.localizedDescription)  # type:ignore
 
-        return platform_nid
+        notification._macos_identifier = platform_nid
 
     async def _create_category_for_notification(
         self, notification: Notification
     ) -> Optional[str]:
         """
         Registers a new notification category with UNNotificationCenter for the given
         notification or retrieves an existing one if it exists for our set of buttons.
@@ -392,15 +392,17 @@
 
     async def _clear(self, notification: Notification) -> None:
         """
         Removes a notifications from the notification center
 
         :param notification: Notification to clear.
         """
-        self.nc.removeDeliveredNotificationsWithIdentifiers([notification.identifier])
+        self.nc.removeDeliveredNotificationsWithIdentifiers(
+            [notification._macos_identifier]
+        )
 
     async def _clear_all(self) -> None:
         """
         Clears all notifications from notification center. This method does not affect
         any notification requests that are scheduled, but have not yet been delivered.
         """
         self.nc.removeAllDeliveredNotifications()
```

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier/macos_legacy.py` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier/macos_legacy.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 class NotificationCenterDelegate(NSObject):  # type: ignore
     """Delegate to handle user interactions with notifications"""
 
     @objc_method  # type:ignore
     def userNotificationCenter_didActivateNotification_(
         self, center, notification
     ) -> None:
-        platform_nid = py_from_ns(notification.identifier)
+        platform_nid = py_from_ns(notification._macos_identifier)
         py_notification = self.interface._notification_for_nid[platform_nid]
         py_notification = cast(Notification, py_notification)
 
         self.interface._clear_notification_from_cache(py_notification)
 
         if (
             notification.activationType
@@ -110,23 +110,23 @@
         """
         return True
 
     async def _send(
         self,
         notification: Notification,
         notification_to_replace: Optional[Notification],
-    ) -> str:
+    ) -> None:
         """
         Uses NSUserNotificationCenter to schedule a notification.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
         if notification_to_replace:
-            platform_nid = str(notification_to_replace.identifier)
+            platform_nid = notification_to_replace._macos_identifier
         else:
             platform_nid = str(uuid.uuid4())
 
         n = NSUserNotification.alloc().init()
         n.title = notification.title
         n.informativeText = notification.message
         n.identifier = platform_nid
@@ -144,15 +144,15 @@
                     "NSUserNotificationCenter: only a single button is supported"
                 )
             n.hasActionButton = True
             n.actionButtonTitle = notification.buttons[0].title
 
         self.nc.scheduleNotification(n)
 
-        return platform_nid
+        notification._macos_identifier = platform_nid
 
     async def _clear(self, notification: Notification) -> None:
         """
         Removes a notifications from the notification center
 
         :param notification: Notification to clear.
         """
```

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier/macos_support.py` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier/macos_support.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier/main.py` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier/main.py`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier/resources/python.png` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier/resources/python.png`

 * *Files identical despite different names*

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier/winrt.py` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier/winrt.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,54 +6,57 @@
 the Windows Runtime and uses the winrt package with compiled components published by
 Microsoft (https://github.com/microsoft/xlang, https://pypi.org/project/winrt/).
 """
 
 from __future__ import annotations
 
 # system imports
+import sys
 import uuid
 import logging
 from xml.etree.ElementTree import Element, SubElement, tostring
-from typing import TypeVar, Any, cast
+from typing import TypeVar
 
 # external imports
 import winreg
-from winsdk.windows.ui.notifications import (
+from winrt.windows.foundation.interop import unbox
+from winrt.windows.ui.notifications import (
     ToastNotificationManager,
     ToastNotificationPriority,
     NotificationSetting,
     ToastNotification,
     ToastActivatedEventArgs,
     ToastDismissalReason,
+    ToastDismissedEventArgs,
+    ToastFailedEventArgs,
 )
-from winsdk.windows.data.xml import dom
-from winsdk.windows.applicationmodel.core import CoreApplication
-from winsdk.windows.foundation import IPropertyValue, PropertyType
-import winsdk._winrt as _winrt
+from winrt.windows.data.xml.dom import XmlDocument
+from winrt.windows.applicationmodel.core import CoreApplication
+from winrt.system import Object as WinRTObject
 
 # local imports
 from .base import Notification, DesktopNotifierBase, Urgency
 
 
 __all__ = ["WinRTDesktopNotifier"]
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 def register_hkey(app_id: str, app_name: str) -> None:
-    winreg.ConnectRegistry(None, winreg.HKEY_CURRENT_USER)  # type:ignore
+    # mypy type guard
+    if not sys.platform == "win32":
+        return
+
+    winreg.ConnectRegistry(None, winreg.HKEY_CURRENT_USER)
     key_path = f"SOFTWARE\\Classes\\AppUserModelId\\{app_id}"
-    with winreg.CreateKeyEx(  # type:ignore
-        winreg.HKEY_CURRENT_USER, key_path  # type:ignore
-    ) as master_key:
-        winreg.SetValueEx(  # type:ignore
-            master_key, "DisplayName", 0, winreg.REG_SZ, app_name  # type:ignore
-        )
+    with winreg.CreateKeyEx(winreg.HKEY_CURRENT_USER, key_path) as master_key:
+        winreg.SetValueEx(master_key, "DisplayName", 0, winreg.REG_SZ, app_name)
 
 
 class WinRTDesktopNotifier(DesktopNotifierBase):
     """Notification backend for the Windows Runtime
 
     :param app_name: The name of the app. This has no effect since the app name will be
         automatically determined.
@@ -74,52 +77,68 @@
 
     def __init__(
         self,
         app_name: str = "Python",
         notification_limit: int | None = None,
     ) -> None:
         super().__init__(app_name, notification_limit)
-        self.manager = ToastNotificationManager.get_default()
+
+        manager = ToastNotificationManager.get_default()
+
+        if not manager:
+            raise RuntimeError("Could not get ToastNotificationManagerForUser")
+
+        self.manager = manager
 
         # Prefer using the real App ID if detected, fall back to user-provided name
         # and icon otherwise.
         if CoreApplication.id != "":
             self.app_id = CoreApplication.id
         else:
             self.app_id = app_name
-            register_hkey(app_name, app_name)
-        self.notifier = self.manager.create_toast_notifier(self.app_id)
+            register_hkey(app_id=app_name, app_name=app_name)
+
+        notifier = self.manager.create_toast_notifier(self.app_id)
+
+        if not notifier:
+            raise RuntimeError(f"Could not get ToastNotifier for app_id: {self.app_id}")
+
+        self.notifier = notifier
 
     async def request_authorisation(self) -> bool:
         """
         Request authorisation to send notifications.
 
         :returns: Whether authorisation has been granted.
         """
-        return bool(self.notifier.setting == NotificationSetting.ENABLED)
+        return await self.has_authorisation()
 
     async def has_authorisation(self) -> bool:
         """
         Whether we have authorisation to send notifications.
         """
-        return bool(self.notifier.setting == NotificationSetting.ENABLED)
+        try:
+            return bool(self.notifier.setting == NotificationSetting.ENABLED)
+        except OSError:
+            # See https://github.com/samschott/desktop-notifier/issues/95.
+            return True
 
     async def _send(
         self,
         notification: Notification,
         notification_to_replace: Notification | None,
-    ) -> str:
+    ) -> None:
         """
         Asynchronously sends a notification.
 
         :param notification: Notification to send.
         :param notification_to_replace: Notification to replace, if any.
         """
         if notification_to_replace:
-            platform_nid = cast(str, notification_to_replace.identifier)
+            platform_nid = notification_to_replace._winrt_identifier
         else:
             platform_nid = str(uuid.uuid4())
 
         # Create notification XML.
         toast_xml = Element("toast", {"launch": WinRTDesktopNotifier.DEFAULT_ACTION})
         visual_xml = SubElement(toast_xml, "visual")
         actions_xml = SubElement(toast_xml, "actions")
@@ -193,91 +212,94 @@
         if notification.sound:
             SubElement(
                 toast_xml, "audio", {"src": "ms-winsoundevent:Notification.Default"}
             )
         else:
             SubElement(toast_xml, "audio", {"silent": "true"})
 
-        xml_document = dom.XmlDocument()
+        xml_document = XmlDocument()
         xml_document.load_xml(tostring(toast_xml, encoding="unicode"))
 
         native = ToastNotification(xml_document)
         native.tag = platform_nid
         native.priority = self._to_native_urgency[notification.urgency]
 
-        def on_activated(sender, boxed_activated_args) -> None:  # type:ignore
-            activated_args = ToastActivatedEventArgs._from(boxed_activated_args)
-            action_id = cast(str, activated_args.arguments)
+        def on_activated(
+            sender: ToastNotification | None, boxed_activated_args: WinRTObject | None
+        ) -> None:
+            if not sender or not boxed_activated_args:
+                return
+
+            try:
+                activated_args = ToastActivatedEventArgs._from(boxed_activated_args)
+            except Exception:
+                return
+
+            action_id = activated_args.arguments
 
             if action_id == WinRTDesktopNotifier.DEFAULT_ACTION:
                 if notification.on_clicked:
                     notification.on_clicked()
             elif action_id == WinRTDesktopNotifier.REPLY_ACTION:
-                if notification.reply_field and notification.reply_field.on_replied:
+                if (
+                    notification.reply_field
+                    and notification.reply_field.on_replied
+                    and activated_args.user_input
+                ):
                     boxed_text = activated_args.user_input[
                         WinRTDesktopNotifier.REPLY_TEXTBOX_NAME
                     ]
-                    text = unbox_winrt(boxed_text)
+                    text = unbox(boxed_text)
                     notification.reply_field.on_replied(text)
             elif action_id.startswith(WinRTDesktopNotifier.BUTTON_ACTION_PREFIX):
                 action_number_str = action_id.replace(
                     WinRTDesktopNotifier.BUTTON_ACTION_PREFIX, ""
                 )
                 action_number = int(action_number_str)
                 callback = notification.buttons[action_number].on_pressed
                 if callback:
                     callback()
 
-        def on_dismissed(sender, dismissed_args) -> None:  # type:ignore
+        def on_dismissed(
+            sender: ToastNotification | None,
+            dismissed_args: ToastDismissedEventArgs | None,
+        ) -> None:
             self._clear_notification_from_cache(notification)
 
-            if dismissed_args.reason == ToastDismissalReason.USER_CANCELED:
+            if (
+                dismissed_args
+                and dismissed_args.reason == ToastDismissalReason.USER_CANCELED
+            ):
                 if notification.on_dismissed:
                     notification.on_dismissed()
 
-        def on_failed(sender, failed_args) -> None:  # type:ignore
-            logger.warning(
-                f"Notification failed (error code {failed_args.error_code.value})"
-            )
+        def on_failed(
+            sender: ToastNotification | None, failed_args: ToastFailedEventArgs | None
+        ) -> None:
+            if failed_args:
+                logger.warning(
+                    f"Notification failed (error code {failed_args.error_code.value})"
+                )
+            else:
+                logger.warning("Notification failed (unknown error code)")
 
         native.add_activated(on_activated)
         native.add_dismissed(on_dismissed)
         native.add_failed(on_failed)
 
         self.notifier.show(native)
 
-        return platform_nid
+        notification._winrt_identifier = platform_nid
 
     async def _clear(self, notification: Notification) -> None:
         """
         Asynchronously removes a notification from the notification center.
         """
-        self.manager.history.remove(notification.identifier)
+        if self.manager.history:
+            self.manager.history.remove(notification._winrt_identifier)
 
     async def _clear_all(self) -> None:
         """
         Asynchronously clears all notifications from notification center.
         """
-        self.manager.history.clear(self.app_id)
-
-
-def unbox_winrt(boxed_value: _winrt.Object) -> Any:
-    """
-    Unbox winrt object. See https://github.com/pywinrt/pywinrt/issues/8.
-    """
-    if boxed_value is None:
-        return boxed_value
-
-    value = IPropertyValue._from(boxed_value)
-
-    if value.type is PropertyType.EMPTY:
-        return None
-    elif value.type is PropertyType.UINT8:
-        return value.get_uint8()
-    elif value.type is PropertyType.INT16:
-        return value.get_int16()
-    elif value.type is PropertyType.UINT16:
-        return value.get_uint16()
-    elif value.type is PropertyType.STRING:
-        return value.get_string()
-    else:
-        raise NotImplementedError(f"Unboxing {value.type} is not yet supported")
+        if self.manager.history:
+            self.manager.history.clear(self.app_id)
```

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier.egg-info/PKG-INFO` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desktop-notifier
-Version: 3.5.6
+Version: 3.5.7.dev0
 Summary: Python library for cross-platform desktop notifications
 Author-email: Sam Schott <sam.schott@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/samschott/desktop-notifier
 Keywords: desktop-notifier
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -15,30 +15,50 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: packaging
+Requires-Dist: dbus-next; sys_platform == "linux"
+Requires-Dist: rubicon-objc; sys_platform == "darwin"
+Requires-Dist: winrt-windows.applicationmodel.core; sys_platform == "win32"
+Requires-Dist: winrt-windows.data.xml.dom; sys_platform == "win32"
+Requires-Dist: winrt-windows.foundation; sys_platform == "win32"
+Requires-Dist: winrt-windows.foundation.collections; sys_platform == "win32"
+Requires-Dist: winrt-windows.foundation.interop; sys_platform == "win32"
+Requires-Dist: winrt-windows.ui.notifications; sys_platform == "win32"
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bump2version; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: flake8-pyproject; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: furo==2024.4.27; extra == "docs"
+Requires-Dist: sphinx==7.3.7; extra == "docs"
+Requires-Dist: sphinx-autoapi==3.0.0; extra == "docs"
+Requires-Dist: sphinx-mdinclude==0.6.0; extra == "docs"
 
 [![PyPi Release](https://img.shields.io/pypi/v/desktop-notifier.svg)](https://pypi.org/project/desktop-notifier/)
 [![Pyversions](https://img.shields.io/pypi/pyversions/desktop-notifier.svg)](https://pypi.org/pypi/desktop-notifier/)
 [![Documentation Status](https://readthedocs.org/projects/desktop-notifier/badge/?version=latest)](https://desktop-notifier.readthedocs.io/en/latest/?badge=latest)
 
 # Desktop Notifier
 
 `desktop-notifier`  is a Python library for cross-platform desktop notifications.
 Currently supported platforms are:
 
 * Linux via the dbus service org.freedesktop.Notifications
 * macOS and iOS via the Notification Center framework
-* [**exprimental**] Windows via the WinRT / Python bridge.
+* [**experimental**] Windows via the WinRT / Python bridge.
 
 ![gif](screenshots/macOS.gif)
 
 ## Features
 
 `desktop-notifier` aims to be a good citizen of the platforms which it supports. It
 therefore stays within the limits of the native platform APIs and does not try to work
```

### Comparing `desktop-notifier-3.5.6/src/desktop_notifier.egg-info/SOURCES.txt` & `desktop_notifier-3.5.7.dev0/src/desktop_notifier.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/desktop_notifier/base.py
 src/desktop_notifier/dbus.py
 src/desktop_notifier/dummy.py
 src/desktop_notifier/macos.py
 src/desktop_notifier/macos_legacy.py
 src/desktop_notifier/macos_support.py
 src/desktop_notifier/main.py
+src/desktop_notifier/py.typed
 src/desktop_notifier/winrt.py
 src/desktop_notifier.egg-info/PKG-INFO
 src/desktop_notifier.egg-info/SOURCES.txt
 src/desktop_notifier.egg-info/dependency_links.txt
 src/desktop_notifier.egg-info/requires.txt
 src/desktop_notifier.egg-info/top_level.txt
 src/desktop_notifier/resources/__init__.py
```

