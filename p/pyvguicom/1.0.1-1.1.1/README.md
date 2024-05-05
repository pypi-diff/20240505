# Comparing `tmp/pyvguicom-1.0.1.tar.gz` & `tmp/pyvguicom-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvguicom-1.0.1.tar", last modified: Wed Apr 24 16:19:56 2024, max compression
+gzip compressed data, was "pyvguicom-1.1.1.tar", last modified: Sun May  5 17:32:24 2024, max compression
```

## Comparing `pyvguicom-1.0.1.tar` & `pyvguicom-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:19:56.022504 pyvguicom-1.0.1/
--rw-r--r--   0 peterglen  (1000) users      (100)     3109 2024-04-24 16:19:56.022504 pyvguicom-1.0.1/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)     2377 2024-03-13 17:22:20.000000 pyvguicom-1.0.1/README.md
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:19:56.022504 pyvguicom-1.0.1/pyvguicom/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-24 07:51:41.000000 pyvguicom-1.0.1/pyvguicom/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7530 2023-09-14 20:07:28.000000 pyvguicom-1.0.1/pyvguicom/browsewin.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3693 2024-04-24 07:55:00.000000 pyvguicom-1.0.1/pyvguicom/custwidg.py
--rw-r--r--   0 peterglen  (1000) users      (100)    10064 2023-09-14 20:07:28.000000 pyvguicom-1.0.1/pyvguicom/htmledit.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    20271 2024-04-24 11:20:12.000000 pyvguicom-1.0.1/pyvguicom/pgbox.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6723 2024-04-24 06:56:13.000000 pyvguicom-1.0.1/pyvguicom/pgbutt.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     7882 2024-04-24 11:13:26.000000 pyvguicom-1.0.1/pyvguicom/pgentry.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    43189 2024-04-24 13:33:48.000000 pyvguicom-1.0.1/pyvguicom/pggui.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    13185 2024-04-24 11:17:09.000000 pyvguicom-1.0.1/pyvguicom/pgsel.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     7628 2024-04-24 13:25:59.000000 pyvguicom-1.0.1/pyvguicom/pgsimp.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    29341 2024-04-24 07:00:30.000000 pyvguicom-1.0.1/pyvguicom/pgtextview.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    41430 2024-04-24 16:03:58.000000 pyvguicom-1.0.1/pyvguicom/pgutils.py
--rw-r--r--   0 peterglen  (1000) users      (100)    25820 2023-09-14 20:07:28.000000 pyvguicom-1.0.1/pyvguicom/pgwkit.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1017 2023-09-14 20:07:28.000000 pyvguicom-1.0.1/pyvguicom/plug.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2901 2024-04-24 11:14:35.000000 pyvguicom-1.0.1/pyvguicom/testbutt.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     1149 2024-04-24 07:56:07.000000 pyvguicom-1.0.1/pyvguicom/testcust.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2658 2024-04-24 07:38:49.000000 pyvguicom-1.0.1/pyvguicom/testentry.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     8947 2023-09-14 20:07:28.000000 pyvguicom-1.0.1/pyvguicom/testicons.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3018 2024-04-24 03:27:26.000000 pyvguicom-1.0.1/pyvguicom/testlettsel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3213 2024-04-24 07:48:24.000000 pyvguicom-1.0.1/pyvguicom/testnums.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4082 2024-04-24 11:12:22.000000 pyvguicom-1.0.1/pyvguicom/testroot.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2355 2024-04-24 11:18:03.000000 pyvguicom-1.0.1/pyvguicom/testsimple.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     7124 2024-04-24 07:02:31.000000 pyvguicom-1.0.1/pyvguicom/testtextv.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:19:56.022504 pyvguicom-1.0.1/pyvguicom.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)     3109 2024-04-24 16:19:56.000000 pyvguicom-1.0.1/pyvguicom.egg-info/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)      646 2024-04-24 16:19:56.000000 pyvguicom-1.0.1/pyvguicom.egg-info/SOURCES.txt
--rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-04-24 16:19:56.000000 pyvguicom-1.0.1/pyvguicom.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       10 2024-04-24 16:19:56.000000 pyvguicom-1.0.1/pyvguicom.egg-info/top_level.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-24 16:19:56.022504 pyvguicom-1.0.1/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     1431 2024-04-24 16:19:44.000000 pyvguicom-1.0.1/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-05 17:32:24.395626 pyvguicom-1.1.1/
+-rw-r--r--   0 peterglen  (1000) users      (100)     3109 2024-05-05 17:32:24.391626 pyvguicom-1.1.1/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2377 2024-03-13 17:22:20.000000 pyvguicom-1.1.1/README.md
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-05 17:32:24.391626 pyvguicom-1.1.1/pyvguicom/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-24 07:51:41.000000 pyvguicom-1.1.1/pyvguicom/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     7590 2024-05-05 17:19:18.000000 pyvguicom-1.1.1/pyvguicom/browsewin.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3693 2024-04-24 07:55:00.000000 pyvguicom-1.1.1/pyvguicom/custwidg.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    10064 2023-09-14 20:07:28.000000 pyvguicom-1.1.1/pyvguicom/htmledit.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    20271 2024-04-24 11:20:12.000000 pyvguicom-1.1.1/pyvguicom/pgbox.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6723 2024-04-24 06:56:13.000000 pyvguicom-1.1.1/pyvguicom/pgbutt.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10486 2024-05-01 13:23:40.000000 pyvguicom-1.1.1/pyvguicom/pgentry.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    46488 2024-05-03 07:59:22.000000 pyvguicom-1.1.1/pyvguicom/pggui.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13350 2024-05-05 17:10:41.000000 pyvguicom-1.1.1/pyvguicom/pgsel.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     7628 2024-04-24 13:25:59.000000 pyvguicom-1.1.1/pyvguicom/pgsimp.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3228 2024-05-05 16:33:55.000000 pyvguicom-1.1.1/pyvguicom/pgtests.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    29341 2024-04-24 07:00:30.000000 pyvguicom-1.1.1/pyvguicom/pgtextview.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    31329 2024-05-05 16:33:34.000000 pyvguicom-1.1.1/pyvguicom/pgutils.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    26237 2024-05-05 17:19:38.000000 pyvguicom-1.1.1/pyvguicom/pgwkit.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1017 2023-09-14 20:07:28.000000 pyvguicom-1.1.1/pyvguicom/plug.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2902 2024-05-03 05:29:54.000000 pyvguicom-1.1.1/pyvguicom/testbutt.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     1150 2024-05-03 05:29:54.000000 pyvguicom-1.1.1/pyvguicom/testcust.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3091 2024-05-03 05:30:04.000000 pyvguicom-1.1.1/pyvguicom/testentry.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3624 2024-05-05 16:37:37.000000 pyvguicom-1.1.1/pyvguicom/testgui.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     8947 2023-09-14 20:07:28.000000 pyvguicom-1.1.1/pyvguicom/testicons.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3019 2024-05-03 05:32:33.000000 pyvguicom-1.1.1/pyvguicom/testlettsel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4067 2024-05-03 07:57:22.000000 pyvguicom-1.1.1/pyvguicom/testmsgs.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3214 2024-05-03 05:32:55.000000 pyvguicom-1.1.1/pyvguicom/testnums.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4082 2024-04-24 11:12:22.000000 pyvguicom-1.1.1/pyvguicom/testroot.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2371 2024-05-05 16:30:56.000000 pyvguicom-1.1.1/pyvguicom/testsimple.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     1883 2024-05-03 05:33:21.000000 pyvguicom-1.1.1/pyvguicom/testtests.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     7126 2024-05-03 05:34:29.000000 pyvguicom-1.1.1/pyvguicom/testtextv.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3965 2024-05-03 05:52:44.000000 pyvguicom-1.1.1/pyvguicom/testutils.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-05 17:32:24.391626 pyvguicom-1.1.1/pyvguicom.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)     3109 2024-05-05 17:32:24.000000 pyvguicom-1.1.1/pyvguicom.egg-info/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)      756 2024-05-05 17:32:24.000000 pyvguicom-1.1.1/pyvguicom.egg-info/SOURCES.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-05-05 17:32:24.000000 pyvguicom-1.1.1/pyvguicom.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       10 2024-05-05 17:32:24.000000 pyvguicom-1.1.1/pyvguicom.egg-info/top_level.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-05-05 17:32:24.395626 pyvguicom-1.1.1/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1826 2024-05-01 13:28:24.000000 pyvguicom-1.1.1/setup.py
```

### Comparing `pyvguicom-1.0.1/PKG-INFO` & `pyvguicom-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvguicom
-Version: 1.0.1
+Version: 1.1.1
 Summary: High power secure server GUI utility helpers.
 Home-page: https://github.com/pglen/pyguicom.git
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyvguicom-1.0.1/README.md` & `pyvguicom-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.1/pyvguicom/browsewin.py` & `pyvguicom-1.1.1/pyvguicom/browsewin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 #!/usr/bin/env python
 
 ''' This encapsulates the browser window wit the webkia an toolbars '''
 
 import os, sys, getopt, signal, random, time, warnings
 
 realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
-sys.path.append(realinc)
+if realinc not in sys.path:
+    sys.path.append(realinc)
 
 from pgutils import  *
 from pggui import  *
 from pgsimp import  *
 
 import gi
 gi.require_version("Gtk", "3.0")
-#gi.require_version('WebKit2', '4.0')
 
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 
-ret = ""
+from pedlib import pedconfig
 
-try:
-    import pgwkit
-except:
-    print("Cannot load WebKit2", sys.exc_info())
-    sys.exit(1)
+import pgwkit
+#print("pgwkit:", pgwkit)
 
-class  brow_win(Gtk.VBox):
+class  browserWin(Gtk.VBox):
 
     ''' Collection of URL bar, toolbar, status bar '''
 
     def __init__(self):
 
         try:
             Gtk.VBox.__init__(self)
@@ -51,17 +48,19 @@
         #    vbox.pack_start(hbox3, False, False, 2)
 
         self.scroll_win = Gtk.ScrolledWindow()
 
         try:
             self.webview = pgwkit.pgwebw(self)
         except:
-            print("Please install webkit2")
+            print("Please install WebKit2", sys.exc_info())
+            #if pedconfig.conf.verbose:
+            put_exception("start webview")
             #sys.exit(1)
-            raise
+            #raise
 
         #self.old_html = ""
         self.scroll_win.add(self.webview)
         self.webview.editor = self.webview
 
         self.toolbar2 = self.webview.ui.get_widget("/toolbar_format")
         self.pack_start(self.toolbar2, False, False, 0)
```

### Comparing `pyvguicom-1.0.1/pyvguicom/custwidg.py` & `pyvguicom-1.1.1/pyvguicom/custwidg.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.1/pyvguicom/htmledit.py` & `pyvguicom-1.1.1/pyvguicom/htmledit.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.1/pyvguicom/pgbox.py` & `pyvguicom-1.1.1/pyvguicom/pgbox.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.1/pyvguicom/pgbutt.py` & `pyvguicom-1.1.1/pyvguicom/pgbutt.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.1/pyvguicom/pgentry.py` & `pyvguicom-1.1.1/pyvguicom/pgentry.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,29 +16,68 @@
     sc = Gtk.ScrolledWindow()
     sc.set_hexpand(True)
     sc.set_vexpand(True)
     sc.add(cont)
     fr.add(sc)
     return fr, cont
 
+class Entryx(Gtk.Entry):
+
+    def __init__(self, noemit = False):
+        super(Entryx).__init__()
+        Gtk.Entry.__init__(self)
+        self.noemit = noemit    # do not emit move next on enter
+        self.connect("key-press-event", self.key_press_event)
+
+    def set_noemit(self, flag):
+        self.noemit = flag
+
+    def set_gray(self, flag):
+        if flag:
+            self.set_editable(False);
+            style = self.get_style_context()
+            color = style.get_background_color(Gtk.StateFlags.NORMAL)
+            color2 = Gdk.RGBA(color.red-.1, color.green-.1, color.blue-.1)
+            self.override_background_color(Gtk.StateFlags.NORMAL, color2)
+        else:
+            self.set_editable(True);
+            style = self.get_style_context()
+            color = style.get_background_color(Gtk.StateFlags.NORMAL)
+            self.override_background_color(Gtk.StateFlags.NORMAL, color)
+
+    def  key_press_event(self, arg1, event):
+        #print("keypress", event.keyval)
+        if event.keyval == Gdk.KEY_Tab or event.keyval == Gdk.KEY_ISO_Left_Tab:
+            #print("tab keypress ", event.keyval, event.state)
+            if event.state & Gdk.ModifierType.SHIFT_MASK:
+                self.emit("move-focus",  Gtk.DirectionType.TAB_BACKWARD)
+            else:
+                self.emit("move-focus",  Gtk.DirectionType.TAB_FORWARD)
+            return True
+
+        if event.keyval == Gdk.KEY_Return:
+            if not self.noemit:
+                self.emit("move-focus",  Gtk.DirectionType.TAB_FORWARD)
+                return True
+
 # Expects two tuples of stuff
 # labtext, labname, tip, defval = None:
 
 def entryquad(arr, vbox, entry1, entry2):
 
     hbox2 = Gtk.HBox(False, 2)
 
     lab1a = Gtk.Label(label="      ")
     hbox2.pack_start(lab1a, False, 0, 0)
     lab1 = Gtk.Label.new_with_mnemonic(entry1[0]) ; lab1.set_alignment(1, 0)
     lab1.set_tooltip_text(entry1[2])
     hbox2.pack_start(lab1, False, 0, 0)
     lab1a = Gtk.Label(label="      ")
     hbox2.pack_start(lab1a, False, 0, 0)
-    headx = Gtk.Entry();  headx.set_width_chars(33)
+    headx = Entryx();  headx.set_width_chars(33)
     lab1.set_mnemonic_widget(headx)
 
     if entry1[3] != None:
         headx.set_text(entry1[3][entry1[1]])
     hbox2.pack_start(headx, True, 0, 0)
     lab3 = Gtk.Label(label="        ")
     hbox2.pack_start(lab3, False, 0, 0)
@@ -47,15 +86,15 @@
     lab1b = Gtk.Label(label="      ")
     hbox2.pack_start(lab1b, False, 0, 0)
     lab2 = Gtk.Label.new_with_mnemonic(entry2[0])  ; lab2.set_alignment(1, 0)
     lab2.set_tooltip_text(entry2[2])
     hbox2.pack_start(lab2, False, 0, 0)
     lab1b = Gtk.Label(label="      ")
     hbox2.pack_start(lab1b, False, 0, 0)
-    headx2 = Gtk.Entry();  headx2.set_width_chars(33)
+    headx2 = Entryx();  headx2.set_width_chars(33)
     lab2.set_mnemonic_widget(headx2)
     if entry2[3] != None:
         headx2.set_text(entry2[3][entry2[1]])
     hbox2.pack_start(headx2, True, 0, 0)
     lab3b = Gtk.Label(label="        ")
     hbox2.pack_start(lab3b, False, 0, 0)
     arr.append((entry2[1], headx2))
@@ -123,71 +162,97 @@
 
 def gridquad(gridx, left, top, entry1, entry2, butt = None):
     lab1 = Gtk.Label.new_with_mnemonic(entry1[0] + "  ")
     lab1.set_alignment(1, 0)
     lab1.set_tooltip_text(entry1[2])
     gridx.attach(lab1, left, top, 1, 1)
 
-    headx = Gtk.Entry();
+    headx = Entryx();
     lab1.set_mnemonic_widget(headx)
     headx.set_width_chars(20)
     if entry1[3] != None:
         headx.set_text(entry1[3])
     gridx.attach(headx, left+1, top, 1, 1)
 
     lab2 = Gtk.Label.new_with_mnemonic("  " + entry2[0] + "  ")
     lab2.set_alignment(1, 0)
     lab2.set_tooltip_text(entry2[2])
     gridx.attach(lab2, left+2, top, 1, 1)
 
-    headx2 = Gtk.Entry();
+    headx2 = Entryx();
     lab2.set_mnemonic_widget(headx2)
 
     headx2.set_width_chars(20)
     if entry2[3] != None:
         headx2.set_text(entry2[3])
     gridx.attach(headx2, left+3, top, 1, 1)
     if butt:
         gridx.attach(butt, left+4, top, 1, 1)
     return headx, headx2
 
 def griddouble(gridx, left, top, entry1, buttx = None):
-    lab1 = Gtk.Label(entry1[0] + "   ")
+    lab1 = Gtk.Label.new_with_mnemonic(entry1[0] + "   ")
     lab1.set_alignment(1, 0)
     lab1.set_tooltip_text(entry1[2])
     gridx.attach(lab1, left, top, 1, 1)
 
-    headx = Gtk.Entry();
+    headx = Entryx();
+    lab1.set_mnemonic_widget(headx)
     headx.set_width_chars(40)
     if entry1[3] != None:
         headx.set_text(entry1[3])
     gridx.attach(headx, left+1, top, 2, 1)
     if buttx:
         gridx.attach(buttx, left+3, top, 1, 1)
     return headx
 
-
 class   TextViewx(Gtk.TextView):
 
+    ''' Override textview for simple deployment '''
+
     def __init__(self):
         super(TextViewx).__init__()
         GObject.GObject.__init__(self)
         self.buffer = Gtk.TextBuffer()
         self.set_buffer(self.buffer)
         self.single_line = False
         self.connect("key-press-event", self.key_press_event)
 
     def  key_press_event(self, arg1, event):
 
+        ''' Override tabs '''
+
         if event.keyval == Gdk.KEY_Tab or event.keyval == Gdk.KEY_ISO_Left_Tab:
             #print("tab keypress ", event.keyval, event.state)
             if event.state & Gdk.ModifierType.SHIFT_MASK:
                 self.emit("move-focus",  Gtk.DirectionType.TAB_BACKWARD)
             else:
                 self.emit("move-focus",  Gtk.DirectionType.TAB_FORWARD)
+            return True
+
+        # If reached last line, TAB it
+        if event.keyval == Gdk.KEY_Down:
+            pos = self.buffer.get_property("cursor-position")
+            #print("Down", pos)
+            #print(self.buffer.list_properties())
+            sss = self.buffer.get_start_iter()
+            eee = self.buffer.get_end_iter()
+            textx = self.buffer.get_text(sss, eee, True)
+            if pos == len(textx):
+                self.emit("move-focus",  Gtk.DirectionType.TAB_FORWARD)
+                return True
+
+        # If reached first line, TAB it
+        if event.keyval == Gdk.KEY_Up:
+            # Are we at the beginning:
+            pos = self.buffer.get_property("cursor-position")
+            #print("Up", pos)
+            if pos == 0:
+                self.emit("move-focus",  Gtk.DirectionType.TAB_BACKWARD)
+                return True
 
         if event.keyval == Gdk.KEY_Return:
             if event.state & Gdk.ModifierType.SHIFT_MASK:
                 #print("keypress shift ", event)
                 self.emit("move-focus",  Gtk.DirectionType.TAB_FORWARD)
                 return True
 
@@ -202,20 +267,22 @@
         startt = self.buffer.get_start_iter()
         endd = self.buffer.get_end_iter()
         self.buffer.delete(startt, endd)
         self.buffer.insert(startt, txt)
         self.buffer.set_modified(True)
 
 def gridsingle(gridx, left, top, entry1):
-    lab1 = Gtk.Label(entry1[0] + "   ")
+    lab1 = Gtk.Label.new_with_mnemonic(entry1[0] + "   ")
     lab1.set_alignment(1, 0)
     lab1.set_tooltip_text(entry1[2])
     gridx.attach(lab1, left, top, 1, 1)
 
     headx, cont = wrap(TextViewx())
+    lab1.set_mnemonic_widget(cont)
+
     if entry1[3] != None:
          headx.set_text(entry1[3])
     gridx.attach(headx, left+1, top, 3, 1)
 
     return cont
 
 def scrolledtext(arr, name, body = None):
@@ -230,15 +297,14 @@
     sw = Gtk.ScrolledWindow()
     sw.textx = textx
     sw.add(textx)
     sw.set_shadow_type(Gtk.ShadowType.ETCHED_IN)
     sw.set_policy(Gtk.PolicyType.AUTOMATIC, Gtk.PolicyType.AUTOMATIC)
     return sw
 
-
 def imgbutt(imgfile, txt, func, win):
     hbb = Gtk.HBox(); vbb = Gtk.VBox();  ic = Gtk.Image();
     ic.set_from_file(imgfile)
     pb = ic.get_pixbuf();
     #pb2 = pb.scale_simple(150, 150, GdkPixbuf.InterpType.BILINEAR)
     pb2 = pb.scale_simple(150, 150, 0)
     ic2 = Gtk.Image.new_from_pixbuf(pb2)
```

### Comparing `pyvguicom-1.0.1/pyvguicom/pggui.py` & `pyvguicom-1.1.1/pyvguicom/pggui.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 sys.path.append(realinc)
 
 import pgutils
 import pgsimp
 
 IDXERR = "Index is larger than the available number of controls."
 
+VERSION = "1.1.1"
+
 gui_testmode = 0
 
 def randcol():
     return random.randint(0, 255)
 
 def randcolstr(start = 0, endd = 255):
     rr =  random.randint(start, endd)
@@ -42,14 +44,16 @@
       style.text, style.base, style.text_aa):
 for st in (gtk.STATE_NORMAL, gtk.STATE_INSENSITIVE,
            gtk.STATE_PRELIGHT, gtk.STATE_SELECTED,
            gtk.STATE_ACTIVE):
     a[st] = gtk.gdk.Color(0, 34251, 0)
 '''
 
+def version():
+    return VERSION
 
 # ------------------------------------------------------------------------
 # Bemd some of the parameters for us
 
 class CairoHelper():
 
     def __init__(self, cr):
@@ -114,14 +118,16 @@
         self.cr.move_to(rect[0], rect[1])
         self.cr.line_to(midx, rect[1] + rect[3])
         self.cr.line_to(rect[0] + rect[2], rect[1])
         self.cr.line_to(rect[0], rect[1])
 
 class   TextTable(Gtk.Table):
 
+    ''' YTable of text entries '''
+
     def __init__(self, confarr, main = None, textwidth = 24):
         GObject.GObject.__init__(self)
         self.texts = []
         #self.set_homogeneous(False)
         self.main = main
         row = 0
         for aa, bb in confarr:
@@ -188,15 +194,14 @@
             #ee.string = "\t"
             #e.state = event.state
             #super().emit("key-release-event", ee)
             #super().foreach(self.callb)
             '''
             pass
 
-
     def callb(self, arg1):
         #print ("callb arg1", arg1)
         pass
 
     def edit_key(self, textbox, event):
         #print(textbox, event.string, event.keyval)
         if event.string == "\t":
@@ -281,14 +286,15 @@
         GObject.GObject.__init__(self)
         #self.size_allocate();
         #self.size_request()
         self.border = border
         self.set_size_request(size + border, size + border)
         self.connect("draw", self.draw)
         self.color =  color
+        self.orgcolor =  color
 
     def set_color(self, col):
         self.color = col
         self.queue_draw()
 
     def draw(self, area, cr):
         rect = self.get_allocation()
@@ -417,71 +423,75 @@
         #super().__init__(self)
         GObject.GObject.__init__(self)
         self.set_label(" " * space + labelx + " " * space)
         self.set_use_underline (True)
         if callme:
             self.connect("clicked", callme)
 
-class FrameTextView(Gtk.TextView):
+class FrameTextView(Gtk.Frame):
 
     def __init__(self, callme = None):
 
         GObject.GObject.__init__(self)
+        #super().__init__(self)
+
+        self.tview = Gtk.TextView()
+        #self.tview.set_buffer(Gtk.TextBuffer())
+
         self.scroll = Gtk.ScrolledWindow()
         self.scroll.set_size_request(100, 100)
-        self.scroll.add_with_viewport(self)
-        self.frame = Gtk.Frame()
-        self.frame.add(self.scroll)
+        self.scroll.add_with_viewport(self.tview)
+        #self.frame = Gtk.Frame()
+        self.add(self.scroll)
 
-        self.set_buffer(Gtk.TextBuffer())
-        self.set_size_request(150, 150)
+        #self.set_size_request(150, 150)
         ls = self.get_style_context()
         fd = ls.get_font(Gtk.StateFlags.NORMAL)
         #newfd = fd.to_string() + " " + str(fd.get_size() / Pango.SCALE + 4)
         #print("newfd", newfd)
         self.modify_font(Pango.FontDescription("Sans 13"))
 
     def append(self, strx):
-        buff = self.get_buffer()
+        buff = self.tview.get_buffer()
         old = buff.get_text(buff.get_start_iter(), buff.get_end_iter(), False)
-        buff.set_text(old + "\n" +  strx)
+        buff.set_text(old + strx)
         pgutils.usleep(20)
         #mainwin.statb2.scroll_to_iter(buff.get_end_iter(), 1.0, True, 0.1, 0.1)
         sb = self.scroll.get_vscrollbar()
         sb.set_value(2000000)
 
 class Label(Gtk.Label):
-    def __init__(self, textm = "", widget = None, tooltip=None, font = None):
+    def __init__(self, textm = "", widget = None, tooltip=None, font=None):
         GObject.GObject.__init__(self)
         self.set_text_with_mnemonic(textm)
         if widget:
             self.set_mnemonic_widget(widget)
         if tooltip:
             self.set_tooltip_text(tooltip)
         if font:
             self.override_font(Pango.FontDescription(font))
 
 class Logo(Gtk.VBox):
 
-    def __init__(self, labelx, tooltip = None, callme = None):
+    def __init__(self, labelx, tooltip=None, callme=None, font="Times 45"):
 
         GObject.GObject.__init__(self)
 
         self.logolab = Gtk.Label(labelx)
         self.logolab.set_has_window(True)
         if tooltip:
             self.logolab.set_tooltip_text(tooltip)
 
         self.logolab.set_events( Gdk.EventMask.BUTTON_PRESS_MASK |
                              Gdk.EventMask.BUTTON_RELEASE_MASK )
 
         if callme:
             self.logolab.connect("button-press-event", callme)
 
-        self.logolab.modify_font(Pango.FontDescription('Times 45'))
+        self.logolab.modify_font(Pango.FontDescription(font))
 
         #self.pack_start(Spacer(), 0, 0, False)
         self.pack_start(self.logolab, 0, 0, False)
         #self.pack_start(Spacer(), 0, 0, False)
 
     def forallcallb(self, arg1):
         #print ("arg1", arg1)
@@ -493,15 +503,15 @@
 
 # ------------------------------------------------------------------------
 # This override covers / hides the complexity of the treeview and the
 # textlisbox did not have the needed detail
 
 class ListBox(Gtk.TreeView):
 
-    def __init__(self, limit = -1, colname = ''):
+    def __init__(self, callb = None, limit = -1, colname = ''):
 
         self.limit = limit
         self.treestore = Gtk.TreeStore(str)
         Gtk.TreeView.__init__(self, self.treestore)
 
         cell = Gtk.CellRendererText()
         # create the TreeViewColumn to display the data
@@ -512,15 +522,15 @@
         # set the cell "text" attribute to column 0 - retrieve text
         tvcolumn.add_attribute(cell, 'text', 0)
 
         # add tvcolumn to treeview
         self.append_column(tvcolumn)
         self.set_activate_on_single_click (True)
 
-        self.callb = None
+        self.callb = callb
         self.connect("row-activated",  self.tree_sel)
 
     def tree_sel(self, xtree, xiter, xpath):
         #print("tree_sel", xtree, xiter, xpath)
         sel = xtree.get_selection()
         xmodel, xiter = sel.get_selected()
         if xiter:
@@ -657,39 +667,18 @@
 # Highlite test items
 
 def set_testmode(flag):
     global gui_testmode
     gui_testmode = flag
 
 # ------------------------------------------------------------------------
-# An N pixel horizontal spacer. Defaults to X pix  get_center
-#
-#def hspacer(hbox, xstr = "    ", expand = False):
-#    lab = Gtk.Label(label=xstr)
-#    hbox.pack_start(lab, expand, 0, 0)
-#
-#def vspacer(vbox, xstr = "     ", expand = False):
-#    lab = Gtk.Label(label=xstr)
-#    vbox.pack_start(lab, expand , 0, 0)
-#def vspacer(sp = 8):
-#    lab = Gtk.VBox()
-#    lab.set_size_request(sp, sp)
-#
-#    if gui_testmode:
-#        lab.override_background_color(
-#                    Gtk.StateFlags.NORMAL, Gdk.RGBA(1, .5, .5) )
-#    return lab
-
-# ------------------------------------------------------------------------
 # An N pixel spacer. Defaults to 1 char height / width
 
 class Spacer(Gtk.Label):
 
-    global box_testmode
-
     def __init__(self, sp = 1, title=None, left=False, bottom=False, test=False):
 
         GObject.GObject.__init__(self)
 
         #sp *= 1000
         #self.set_markup("<span  size=\"" + str(sp) + "\"> </span>")
         #self.set_text(" " * sp)
@@ -701,15 +690,15 @@
 
         if left:
             self.set_xalign(0)
 
         if bottom:
             self.set_yalign(1)
 
-        if test or box_testmode:
+        if test or gui_testmode:
             self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#888888"))
 
         #self.set_property("angle", 15)
         #attr = self.get_property("attributes")
         #attr2 = Pango.AttrList()
         #print ("attr", dir(attr))
         #attr.
@@ -743,49 +732,14 @@
             col = randcolstr(100, 200)
             self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse(col))
         if sp == None:
             sp = 6
         self.set_size_request(sp, sp)
 
 # ------------------------------------------------------------------------
-# An N pixel spacer. Defaults to 1 char height / width
-
-class Spacer(Gtk.Label):
-
-    global gui_testmode
-
-    def __init__(self, sp = 1, title=None, left=False, bottom=False, test=False):
-
-        GObject.GObject.__init__(self)
-
-        #sp *= 1000
-        #self.set_markup("<span  size=\"" + str(sp) + "\"> </span>")
-        #self.set_text(" " * sp)
-
-        if title:
-            self.set_text(title)
-        else:
-            self.set_text(" " * sp)
-        if left:
-            self.set_xalign(0)
-        if bottom:
-            self.set_yalign(1)
-        if test or gui_testmode:
-            self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#888888"))
-
-        #self.set_property("angle", 15)
-        #attr = self.get_property("attributes")
-        #attr2 = Pango.AttrList()
-        #print ("attr", dir(attr))
-        #attr.
-        #self.set_property("attributes", attr)
-        #self.set_property("label", "wtf")
-        #self.set_property("background-set", True)
-
-# ------------------------------------------------------------------------
 # Added convenience methods
 
 class   xVBox(Gtk.VBox):
 
     def __init__(self, col = None):
         GObject.GObject.__init__(self)
         self.pad = 0
@@ -820,21 +774,29 @@
             pad = self.pad
         self.pack_start(obj, expand, expand, pad)
 
 # ------------------------------------------------------------------------
 
 class   RadioGroup(Gtk.Frame):
 
-    def __init__(self, rad_arr, call_me):
+    def __init__(self, rad_arr, call_me = None, horiz = False):
 
         GObject.GObject.__init__(self)
         self.buttons = []
         self.callme = call_me
-        vbox6 = Gtk.VBox(); vbox6.set_spacing(4);
-        vbox6.set_border_width(6)
+        if horiz:
+            vbox6 = Gtk.HBox();
+            vbox6.set_spacing(6);
+            vbox6.set_border_width(4)
+        else:
+            vbox6 = Gtk.VBox();
+            vbox6.set_spacing(4);
+            vbox6.set_border_width(6)
+
+
 
         if gui_testmode:
             self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#778888"))
 
         self.radio = Gtk.RadioButton.new_with_mnemonic(None, "None")
 
         for aa in range(len(rad_arr)):
@@ -1050,30 +1012,28 @@
     def select(self, num):
         self.listbox.select(num)
 
 # ------------------------------------------------------------------------
 
 class   ComboBox(Gtk.ComboBox):
 
-    def __init__(self, init_cont = [], callme = None):
+    def __init__(self, init_cont, callme = None):
+
+        self.callme = callme
 
         self.store = Gtk.ListStore(str)
         Gtk.ComboBox.__init__(self)
-
         self.set_model(self.store)
         cell = Gtk.CellRendererText()
 
         cell.set_property("text", "hello")
         #cell.set_property("background", "#ffff00")
         #cell.set_property("background-set", True)
         cell.set_padding(10, 0)
 
-        if callme:
-            self.connect("changed", callme)
-
         #cell.set_property("foreground", "#ffff00")
         #cell.set_property("foreground-set", True)
         #print("background-set", cell.get_property("background-set"))
         #print("foreground-set", cell.get_property("foreground-set"))
         #print(" list_properties", cell.list_properties())
 
         self.pack_start(cell, True)
@@ -1096,14 +1056,17 @@
             else:
                 entry = combo.get_child()
                 name = entry.get_text()
                 #print("Entered: %s" % name)
         except:
             pass
 
+        if self.callme:
+            self.callme(name)
+
         #print("Combo new selection / entry: '%s'" % name)
 
     def delall(self):
          # Delete previous contents
         try:
             while True:
                 root = self.store.get_iter_first()
@@ -1376,35 +1339,171 @@
     def clicked(self, arg1):
         pass
         #print("clicked", arg1)
         #if self.callme:
         #    self.callme(arg1)
 
 
-def message(msg):
-    dialog = Gtk.MessageDialog(None, Gtk.DialogFlags.DESTROY_WITH_PARENT,
-        Gtk.MessageType.INFO, Gtk.ButtonsType.CLOSE, text=msg)
+# ------------------------------------------------------------------------
+# Show a regular message:
+
+def message(strx, parent = None, title = None, icon = Gtk.MessageType.INFO):
 
-    #    'Action: "%s" of type "%s"' % (action.get_name(), type(action)))
+    #dialog = Gtk.MessageDialog(parent, Gtk.DialogFlags.DESTROY_WITH_PARENT,
+    #    icon, Gtk.ButtonsType.CLOSE, strx)
+
+    dialog = Gtk.MessageDialog(title=title, buttons=Gtk.ButtonsType.CLOSE,
+                text=strx, destroy_with_parent=True, modal=True,)
+
+    if parent:
+        dialog.set_transient_for(parent)
+
+    if title:
+        dialog.set_title(title)
+    else:
+        dialog.set_title("Message")
 
     # Close dialog on user response
-    dialog.connect ("response", lambda d, r: d.destroy())
+    dialog.connect("response", lambda d, r: d.destroy())
+    dialog.show_all()
     return dialog.run()
 
-def yesno(msg):
-    dialog = Gtk.MessageDialog(None, Gtk.DialogFlags.DESTROY_WITH_PARENT,
-        Gtk.MessageType.INFO, Gtk.ButtonsType.YES_NO, text=msg)
+def yes_no(message, title = "Question", parent=None, default="Yes"):
 
-    #    'Action: "%s" of type "%s"' % (action.get_name(), type(action)))
+    dialog = Gtk.MessageDialog(title=title)
+
+    img = Gtk.Image.new_from_stock(Gtk.STOCK_DIALOG_QUESTION, Gtk.IconSize.DIALOG)
+    dialog.set_image(img)
+    dialog.set_markup(message)
+
+    if default == "Yes":
+        dialog.set_default_response(Gtk.ResponseType.YES)
+        dialog.add_button("_Yes", Gtk.ResponseType.YES)
+        dialog.add_button("_No", Gtk.ResponseType.NO)
+    else:
+        dialog.set_default_response(Gtk.ResponseType.NO)
+        dialog.add_button("_No", Gtk.ResponseType.NO)
+        dialog.add_button("_Yes", Gtk.ResponseType.YES)
+
+    if parent:
+        dialog.set_transient_for(parent)
+
+    def _yn_key(win, event, cancel):
+        #print("_y_n key", event.keyval)
+        if event.keyval == Gdk.KEY_y or \
+            event.keyval == Gdk.KEY_Y:
+            win.response(Gtk.ResponseType.YES)
+        if event.keyval == Gdk.KEY_n or \
+            event.keyval == Gdk.KEY_N:
+            win.response(Gtk.ResponseType.NO)
+        #if cancel:
+        #    if event.keyval == Gdk.KEY_c or \
+        #        event.keyval == Gdk.KEY_C:
+        #        win.response(Gtk.ResponseType.CANCEL)
+
+    dialog.connect("key-press-event", _yn_key, 0)
+    # Fri 03.May.2024 destroyed return value
+    #dialog.connect("response", lambda d, r: d.destroy())
+    dialog.show_all()
+    response = dialog.run()
+    dialog.destroy()
+    #print("response", response, resp2str(response))
+
+    # Convert all other responses to default
+    if response == Gtk.ResponseType.REJECT or \
+          response == Gtk.ResponseType.CLOSE  or \
+             response == Gtk.ResponseType.DELETE_EVENT:
+        response = Gtk.ResponseType.NO
+
+        # Cancel means no
+        #if default == "Yes":
+        #    response = Gtk.ResponseType.YES
+        #else:
+        #    response = Gtk.ResponseType.NO
+
+    return response
+
+# ------------------------------------------------------------------------
+
+def yes_no_cancel(message, title="Question", default="Yes"):
+
+    dialog = Gtk.MessageDialog(title=title)
+
+    if default == "Yes":
+        dialog.set_default_response(Gtk.ResponseType.YES)
+        dialog.add_button("_Yes", Gtk.ResponseType.YES)
+        dialog.add_button("_No", Gtk.ResponseType.NO)
+        dialog.add_button("_Cancel", Gtk.ResponseType.CANCEL)
+    elif default == "No":
+        dialog.set_default_response(Gtk.ResponseType.NO)
+        dialog.add_button("_No", Gtk.ResponseType.NO)
+        dialog.add_button("_Yes", Gtk.ResponseType.YES)
+        dialog.add_button("_Cancel", Gtk.ResponseType.CANCEL)
+    else:
+        dialog.set_default_response(Gtk.ResponseType.CANCEL)
+        dialog.add_button("_Cancel", Gtk.ResponseType.CANCEL)
+        dialog.add_button("_Yes", Gtk.ResponseType.YES)
+        dialog.add_button("_No", Gtk.ResponseType.NO)
+
+    img = Gtk.Image.new_from_stock(Gtk.STOCK_DIALOG_QUESTION, Gtk.IconSize.DIALOG)
+    dialog.set_image(img)
+    dialog.set_markup(message)
+
+    def _yn_keyc(win, event):
+        #print("key:",  event)
+        if event.keyval == Gdk.KEY_y or \
+            event.keyval == Gdk.KEY_Y:
+            win.response(Gtk.ResponseType.YES)
+        if event.keyval == Gdk.KEY_n or \
+            event.keyval == Gdk.KEY_N:
+            win.response(Gtk.ResponseType.NO)
+        if event.keyval == Gdk.KEY_c or \
+            event.keyval == Gdk.KEY_C:
+            win.response(Gtk.ResponseType.CANCEL)
+
+    dialog.connect("key-press-event", _yn_keyc)
+    dialog.show_all()
+    response = dialog.run()
+
+    # Convert all other responses to cancel
+    if  response == Gtk.ResponseType.CANCEL or \
+            response == Gtk.ResponseType.REJECT or \
+                response == Gtk.ResponseType.CLOSE  or \
+                    response == Gtk.ResponseType.DELETE_EVENT:
+        response = Gtk.ResponseType.CANCEL
 
-    # Close dialog on user response
-    #dialog.connect ("response", lambda d, r: d.destroy())
-    ret = dialog.run()
     dialog.destroy()
-    return  ret
+
+    #print("yes_no_cancel() result:", response);
+    return  response
+
+def resp2str(resp):
+
+    ''' Translate response to string '''
+
+    strx = "None"
+    if  resp == Gtk.ResponseType.YES:
+        strx =  "Yes"
+    if  resp == Gtk.ResponseType.NO:
+        strx =  "No"
+    if  resp == Gtk.ResponseType.OK:
+        strx =  "OK"
+    if  resp == Gtk.ResponseType.CANCEL:
+        strx =  "Cancel"
+    if  resp == Gtk.ResponseType.NONE:
+        strx =  "None"
+    if  resp == Gtk.ResponseType.ACCEPT:
+        strx =  "Accept"
+    if resp == Gtk.ResponseType.REJECT:
+        strx =  "Reject"
+    if resp == Gtk.ResponseType.CLOSE:
+        strx =  "CLlose"
+    if resp == Gtk.ResponseType.DELETE_EVENT:
+        strx =  "Delete Event"
+    return strx
 
 # ------------------------------------------------------------------------
 # Highlite test items
 
 def set_gui_testmode(flag):
     global gui_testmode
     gui_testmode = flag
```

### Comparing `pyvguicom-1.0.1/pyvguicom/pgsel.py` & `pyvguicom-1.1.1/pyvguicom/pgsel.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.simsel2.connect("leave_notify_event", self.leave_label)
 
         self.connect("focus_in_event", self.focus_label)
         self.connect("focus_out_event", self.focus_out_label)
 
         vbox = Gtk.VBox()
         vbox.pack_start(hbox3a, 0, 0, False)
-        vbox.pack_start(pggui.ySpacer(4), 0, 0, False)
+        #vbox.pack_start(pggui.ySpacer(), 0, 0, False)
         vbox.pack_start(hbox3b, 0, 0, False)
 
         self.frame = Gtk.Frame()
         self.frame.set_shadow_type(Gtk.ShadowType.NONE)
 
         self.frame.add(vbox)
         self.pack_start(self.frame, 0, 0, False)
@@ -139,25 +139,27 @@
                     self.curr.idx = 0
             self.curr.exec_index(True)
             return True
 
         if event.keyval == Gdk.KEY_Down:
             if self.curr == self.simsel:
                 self.curr = self.simsel2
+                self.curr.exec_index(True)
             else:
-                self.curr = self.simsel
-            self.curr.exec_index(True)
+                # Thu 02.May.2024 tab instead
+                self.emit("move-focus",  Gtk.DirectionType.TAB_FORWARD)
             return True
 
         if event.keyval == Gdk.KEY_Up:
-            if self.curr == self.simsel:
-                self.curr = self.simsel2
-            else:
+            if self.curr == self.simsel2:
                 self.curr = self.simsel
-            self.curr.exec_index(True)
+                self.curr.exec_index(True)
+            else:
+                # Thu 02.May.2024 tab instead
+                self.emit("move-focus",  Gtk.DirectionType.TAB_BACKWARD)
             return True
 
         if event.keyval == Gdk.KEY_Home:
             self.curr.idx = 0
             self.curr.exec_index(True)
             return True
```

### Comparing `pyvguicom-1.0.1/pyvguicom/pgsimp.py` & `pyvguicom-1.1.1/pyvguicom/pgsimp.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.1/pyvguicom/pgtextview.py` & `pyvguicom-1.1.1/pyvguicom/pgtextview.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.1/pyvguicom/pgutils.py` & `pyvguicom-1.1.1/pyvguicom/pgutils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,173 +1,34 @@
 #!/usr/bin/python
 
 # pylint: disable=C0103
 # pylint: disable=C0209
 # pylint: disable=C0321
 
-import os, sys, getopt, string,  math, warnings
+import os, sys, getopt, string,  math
 import random, time, traceback, stat
 import platform
 
+#import warmings
+
 if sys.version_info.major < 3:
     pass
 else:
     import inspect
     if inspect.isbuiltin(time.process_time):
         time.clock = time.process_time
 
 ''' General utility fiunctions '''
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GObject
-
-# Add the new line twice for more balaced string
-
-allcr =    " " + "\r" + "\n" + \
-            "\r" + "\n"
-
-                   #string.punctuation +
-
-allstr =    " " + \
-            string.ascii_lowercase +  string.ascii_uppercase +  \
-                string.digits
-
-allasc =      string.ascii_lowercase +  string.ascii_uppercase +  \
-                string.digits + "_"
-alllett =      string.ascii_lowercase +  string.ascii_uppercase
-testmode = 0
-
-# -----------------------------------------------------------------------
-# Sleep just a little, but allow the system to breed
-
-def  usleep2(msec):
-
-    if sys.version_info[0] < 3 or \
-        (sys.version_info[0] == 3 and sys.version_info[1] < 3):
-        timefunc = time.clock
-    else:
-        timefunc = time.process_time
-
-    got_clock = timefunc() + float(msec) / 1000
-    #print( got_clock)
-    while True:
-        if timefunc() > got_clock:
-            break
-        #print ("Sleeping")
-        Gtk.main_iteration_do(False)
-
-# -----------------------------------------------------------------------
-# Pull up a message box
-
-def message2(strx, title = "Dialog", parent=None):
-
-    dialog = Gtk.MessageDialog()
-    # Close dialog on user response
-    dialog.add_button("Close", Gtk.ButtonsType.CLOSE)
-    if title:
-        dialog.set_title(title)
-    #box = dialog.get_content_area()
-    #box.add(Gtk.Label(strx))
-    dialog.set_markup(strx)
-    if parent:
-        dialog.set_transient_for(parent)
-    dialog.connect ("response", lambda d, r: d.destroy())
-    dialog.show_all()
-
-def yes_no2(message, title = "Question", parent=None):
-
-    dialog = Gtk.MessageDialog()
-    if title:
-        dialog.set_title(title)
-    dialog.add_button("_Yes", Gtk.ResponseType.YES)
-    dialog.add_button("_No", Gtk.ResponseType.NO)
-    dialog.set_markup(message)
-    img = Gtk.Image.new_from_stock(Gtk.STOCK_DIALOG_QUESTION, Gtk.IconSize.DIALOG)
-    dialog.set_image(img)
-    if parent:
-        dialog.set_transient_for(parent)
-    dialog.connect("key-press-event", yn_key, 0)
-    #dialog.connect ("response", lambda d, r: d.destroy())
-    dialog.show_all()
-    response = dialog.run()
-    dialog.destroy()
-
-    return response
-
-# ------------------------------------------------------------------------
-# Do dialog
-
-def yes_no_cancel2(message, title = "Question", cancel = True):
-
-    warnings.simplefilter("ignore")
-
-    dialog = Gtk.Dialog(title,
-                   None,
-                   Gtk.DialogFlags.MODAL | Gtk.DialogFlags.DESTROY_WITH_PARENT)
-
-    dialog.set_default_response(Gtk.ResponseType.YES)
-    dialog.set_position(Gtk.WindowPosition.CENTER)
-
-    sp = "     "
-    label = Gtk.Label(message)
-    label2 = Gtk.Label(sp);      label3 = Gtk.Label(sp)
-    label2a = Gtk.Label(sp);     label3a = Gtk.Label(sp)
-
-    hbox = Gtk.HBox()
-
-    hbox.pack_start(label2, 0, 0, 0)
-    hbox.pack_start(label, 1, 1, 0)
-    hbox.pack_start(label3, 0, 0, 0)
-
-    dialog.vbox.pack_start(label2a, 0, 0, 0)
-    dialog.vbox.pack_start(hbox, 0, 0, 0)
-    dialog.vbox.pack_start(label3a, 0, 0, 0)
-
-    dialog.add_button("_Yes", Gtk.ResponseType.YES)
-    dialog.add_button("_No", Gtk.ResponseType.NO)
-
-    if cancel:
-        dialog.add_button("_Cancel", Gtk.ResponseType.CANCEL)
-
-    dialog.connect("key-press-event", _yn_key, cancel)
-    #dialog.connect("key-release-event", _yn_key, cancel)
-    warnings.simplefilter("default")
-
-    dialog.show_all()
-    response = dialog.run()
-
-    # Convert all responses to cancel
-    if  response == Gtk.ResponseType.CANCEL or \
-            response == Gtk.ResponseType.REJECT or \
-                response == Gtk.ResponseType.CLOSE  or \
-                    response == Gtk.ResponseType.DELETE_EVENT:
-        response = Gtk.ResponseType.CANCEL
-
-    dialog.destroy()
-
-    #print("YNC result:", response);
-    return  response
-
-def _yn_key(win, event, cancel):
-    #print event
-    if event.keyval == Gdk.KEY_y or \
-        event.keyval == Gdk.KEY_Y:
-        win.response(Gtk.ResponseType.YES)
-
-    if event.keyval == Gdk.KEY_n or \
-        event.keyval == Gdk.KEY_N:
-        win.response(Gtk.ResponseType.NO)
-
-    if cancel:
-        if event.keyval == Gdk.KEY_c or \
-            event.keyval == Gdk.KEY_C:
-            win.response(Gtk.ResponseType.CANCEL)
+from gi.repository import GdkPixbuf
 
 # ------------------------------------------------------------------------
 # Resolve path name
 
 def respath(fname):
 
     try:
@@ -177,20 +38,14 @@
             if os.path.isfile(str(ttt)):
                 return ttt
     except:
         print ("Cannot resolve path", fname, sys.exc_info())
     return None
 
 # ------------------------------------------------------------------------
-# Random colors
-
-def randcol():
-    return random.randint(0, 255)
-
-# ------------------------------------------------------------------------
 # Color conversions
 
 def str2col(strx):
     ccc = str2float(strx)
     return float2col(ccc)
 
 def str2float( col):
@@ -245,15 +100,15 @@
             pass
             print(xstr, file=sys.stderr)
 
     except:
         print( "Failed on debug output.")
         print( sys.exc_info())
 
-def put_exception_old(xstr):
+def put_exception(xstr):
 
     cumm = xstr + " "
     a,b,c = sys.exc_info()
     if a != None:
         cumm += str(a) + " " + str(b) + "\n"
         try:
             #cumm += str(traceback.format_tb(c, 10))
@@ -261,15 +116,15 @@
             for aa in ttt:
                 cumm += "File: " + os.path.basename(aa[0]) + \
                         "  Line: " + str(aa[1]) + "\n" +  \
                         "    Context: " + aa[2] + " -> " + aa[3] + "\n"
         except:
             print( "Could not print trace stack. ", sys.exc_info())
 
-    put_debug2(cumm)
+    print(cumm)
     #syslog.syslog("%s %s %s" % (xstr, a, b))
 
 def decode_bits(numx):
     mask = 0x80
     retx = ""
     for aa in range(8):
         strx = "0"
@@ -278,21 +133,14 @@
         retx += "B%d=%s  " % (7-aa, strx)
         if aa == 3:
             retx += "\r"
         mask >>= 1
 
     return retx
 
-def randcolstr(start = 0, endd = 255):
-    rr =  random.randint(start, endd)
-    gg =  random.randint(start, endd)
-    bb =  random.randint(start, endd)
-    strx = "#%02x%02x%02x" % (rr, gg, bb)
-    return strx
-
 # ------------------------------------------------------------------------
 # Remove non printables
 
 def clean_str(strx):
 
     stry = ""
     for aa in range(len(strx)):
@@ -383,47 +231,14 @@
         except (OSError, serial.SerialException):
             pass
     #print ("result", result)
     return result
 '''
 
 # ------------------------------------------------------------------------
-# Get random str
-
-def randstr(lenx):
-
-    strx = ""
-    for aa in range(lenx):
-        ridx = random.randint(0, len(allstr)-1)
-        rr = allstr[ridx]
-        strx += str(rr)
-
-    return strx
-
-def randasc(lenx):
-
-    strx = ""
-    for aa in range(lenx):
-        ridx = random.randint(0, len(allasc)-1)
-        rr = allasc[ridx]
-        strx += str(rr)
-
-    return strx
-
-def randlett(lenx):
-
-    strx = ""
-    for aa in range(lenx):
-        ridx = random.randint(0, len(alllett)-1)
-        rr = alllett[ridx]
-        strx += str(rr)
-
-    return strx
-
-# ------------------------------------------------------------------------
 # Convert octal string to integer
 
 def oct2int(strx):
     retx = 0
     for aa in strx:
         num = ord(aa) - ord("0")
         if num > 7 or num < 0:
@@ -843,174 +658,93 @@
                         if self.optarr[bb][2] != None:
                             self.__dict__[self.optarr[bb][1]] = 1
                         #print( "call", self.optarr[bb][3])
                         if self.optarr[bb][3] != None:
                             self.optarr[bb][3]()
         return args
 
-# ------------------------------------------------------------------------
-
-def yes_no_cancel(title, message, cancel = True):
-
-    warnings.simplefilter("ignore")
-
-    dialog = Gtk.Dialog(title,
-                   None,
-                   Gtk.DialogFlags.MODAL | Gtk.DialogFlags.DESTROY_WITH_PARENT)
-
-    dialog.set_default_response(Gtk.ResponseType.YES)
-    dialog.set_position(Gtk.WindowPosition.CENTER)
-    #dialog.set_transient_for(pedconfig.conf.pedwin.mywin)
-
-    sp = "     "
-    label = Gtk.Label(message)
-    label2 = Gtk.Label(sp)
-    label3 = Gtk.Label(sp)
-    label2a = Gtk.Label(sp)
-    label3a = Gtk.Label(sp)
-
-    hbox = Gtk.HBox()
-
-    hbox.pack_start(label2, 0, 0, 0)
-    hbox.pack_start(label, 1, 1, 0)
-    hbox.pack_start(label3, 0, 0, 0)
-
-    dialog.vbox.pack_start(label2a, 0, 0, 0)
-    dialog.vbox.pack_start(hbox, 0, 0, 0)
-    dialog.vbox.pack_start(label3a, 0, 0, 0)
-
-    dialog.add_button("_Yes", Gtk.ResponseType.YES)
-    dialog.add_button("_No", Gtk.ResponseType.NO)
-
-    if cancel:
-        dialog.add_button("_Cancel", Gtk.ResponseType.CANCEL)
-
-    dialog.connect("key-press-event", _yn_key, cancel)
-    #dialog.connect("key-release-event", _yn_key, cancel)
-    warnings.simplefilter("default")
-
-    dialog.show_all()
-    response = dialog.run()
-
-    # Convert all responses to cancel
-    if  response == Gtk.ResponseType.CANCEL or \
-            response == Gtk.ResponseType.REJECT or \
-                response == Gtk.ResponseType.CLOSE  or \
-                    response == Gtk.ResponseType.DELETE_EVENT:
-        response = Gtk.ResponseType.CANCEL
-
-    dialog.destroy()
-
-    #print("YNC result:", response);
-    return  response
-
-def _yn_key(win, event, cancel):
-    #print event
-    if event.keyval == Gdk.KEY_y or \
-        event.keyval == Gdk.KEY_Y:
-        win.response(Gtk.ResponseType.YES)
-
-    if event.keyval == Gdk.KEY_n or \
-        event.keyval == Gdk.KEY_N:
-        win.response(Gtk.ResponseType.NO)
-
-    if cancel:
-        if event.keyval == Gdk.KEY_c or \
-            event.keyval == Gdk.KEY_C:
-            win.response(Gtk.ResponseType.CANCEL)
-
-def  about2(self2):
+def  about(progname, verstr = "1.0.0", imgfile = "icon.png"):
 
     ''' Show About dialog: '''
 
     dialog = Gtk.AboutDialog()
-    dialog.set_name(pedconfig.conf.progname +  " - Python Editor ")
+    dialog.set_name(progname)
 
-    dialog.set_version(str(pedconfig.conf.version))
+    dialog.set_version(verstr)
     gver = (Gtk.get_major_version(), \
                         Gtk.get_minor_version(), \
                             Gtk.get_micro_version())
 
     dialog.set_position(Gtk.WindowPosition.CENTER)
-    dialog.set_transient_for(pedconfig.conf.pedwin.mywin)
+    #dialog.set_transient_for(pedconfig.conf.pedwin.mywin)
 
     #"\nRunning PyGObject %d.%d.%d" % GObject.pygobject_version +\
 
-    ddd = os.path.join(os.path.dirname(__file__), "../")
+    ddd = os.path.join(os.path.dirname(__file__))
 
     # GLib.pyglib_version
     vvv = gi.version_info
-    comm = "Python based easily configurable editor\n"\
-        "with time accounting module, spell "\
-        "check \n and macro recording.\n"\
-        "\nRunning PyGtk %d.%d.%d" % vvv +\
-        "\non GTK %d.%d.%d\n" % gver +\
+    comm = \
+        "Running PyGtk %d.%d.%d" % vvv +\
+        "\non GTK %d.%d.%d" % gver +\
         "\nRunning Python %s" % platform.python_version() +\
-        "\non %s %s\n" % (platform.system(), platform.release()) +\
-        "\nPyedPro Build Date: %s\n" % pedconfig.conf.build_date +\
-        "Exe Path:\n%s\n" % os.path.realpath(ddd)
+        "\non %s %s" % (platform.system(), platform.release()) +\
+        "\nExe Path:\n%s" % os.path.realpath(ddd)
 
     dialog.set_comments(comm)
-    dialog.set_copyright(pedconfig.conf.progname + " Created by Peter Glen.\n"
+    dialog.set_copyright(progname + " Created by Peter Glen.\n"
                           "Project is in the Public Domain.")
-    dialog.set_program_name(pedconfig.conf.progname)
-    img_dir = os.path.join(os.path.dirname(__file__), 'images')
-    #img_path = os.path.join(img_dir, 'gtk-logo-rgb.gif')
-    img_path = os.path.join(img_dir, 'pyedpro.png')
+    dialog.set_program_name(progname)
+    img_path = os.path.join(os.path.dirname(__file__), imgfile)
 
     try:
         pixbuf = GdkPixbuf.Pixbuf.new_from_file(img_path)
         #print "loaded pixbuf"
         dialog.set_logo(pixbuf)
 
     except:
         print("Cannot load logo for about dialog", img_path)
         print(sys.exc_info())
 
     #dialog.set_website("")
 
     ## Close dialog on user response
     dialog.connect ("response", lambda d, r: d.destroy())
-    dialog.connect("key-press-event", about_key)
+    dialog.connect("key-press-event", _about_key)
 
     dialog.show()
 
-def about_key(win, event):
+def _about_key(win, event):
     #print "about_key", event
     if  event.type == Gdk.EventType.KEY_PRESS:
         if event.keyval == Gdk.KEY_x or event.keyval == Gdk.KEY_X:
             if event.state & Gdk.ModifierType.MOD1_MASK:
                 win.destroy()
 
 # ------------------------------------------------------------------------
 # Show a regular message:
-
-def message3(strx, title = None):
-
-    #print("called: message()", strx)
-
-    icon = Gtk.STOCK_INFO
-    dialog = Gtk.MessageDialog(buttons=Gtk.ButtonsType.CLOSE,
-                               message_type=Gtk.MessageType.INFO)
-
-    dialog.props.text = strx
-
-    #dialog.set_transient_for()
-
-    if title:
-        dialog.set_title(title)
-    else:
-        dialog.set_title("PyEdPro")
-
-    dialog.set_position(Gtk.WindowPosition.CENTER)
-
-    # Close dialog on user response
-    dialog.connect("response", lambda d, r: d.destroy())
-    dialog.show()
-    dialog.run()
+#
+#def message3(strx, title = None):
+#
+#    #print("called: message()", strx)
+#
+#    icon = Gtk.STOCK_INFO
+#    dialog = Gtk.MessageDialog(buttons=Gtk.ButtonsType.CLOSE,
+#                               message_type=Gtk.MessageType.INFO)
+#    dialog.props.text = strx
+#    #dialog.set_transient_for()
+#    if title:
+#        dialog.set_title(title)
+#    else:
+#        dialog.set_title("PyEdPro")
+#    dialog.set_position(Gtk.WindowPosition.CENTER)
+#    # Close dialog on user response
+#    dialog.connect("response", lambda d, r: d.destroy())
+#    dialog.show()
+#    dialog.run()
 
 # -----------------------------------------------------------------------
 # Call func with all processes, func called with stat as its argument
 # Function may return True to stop iteration
 
 def withps(func, opt = None):
 
@@ -1046,17 +780,17 @@
 
     self.dialog = dialog
 
     label3 = Gtk.Label("   ");  label4 = Gtk.Label("   ")
     label5 = Gtk.Label("   ");  label6 = Gtk.Label("   ")
     label7 = Gtk.Label("   ");  label8 = Gtk.Label("   ")
 
-    warnings.simplefilter("ignore")
+    #warmings.simplefilter("ignore")
     entry = Gtk.Entry()
-    warnings.simplefilter("default")
+    #warmings.simplefilter("default")
     entry.set_text(self.oldfind)
 
     entry.set_activates_default(True)
 
     dialog.vbox.pack_start(label4)
 
     hbox2 = Gtk.HBox()
@@ -1141,34 +875,14 @@
                 cumm += "File: " + os.path.basename(aa[0]) + \
                         " Line: " + str(aa[1]) + "\n" +  \
                     "   Context: " + aa[2] + " -> " + aa[3] + "\n"
         except:
             print("Could not print trace stack. ", sys.exc_info())
     print( cumm)
 
-
-# ------------------------------------------------------------------------
-# Show a regular message:
-
-def message(strx, parent = None, title = None, icon = Gtk.MessageType.INFO):
-
-    dialog = Gtk.MessageDialog(parent, Gtk.DialogFlags.DESTROY_WITH_PARENT,
-        icon, Gtk.ButtonsType.CLOSE, strx)
-
-    dialog.set_modal(True)
-
-    if title:
-        dialog.set_title(title)
-    else:
-        dialog.set_title("DBGui Message")
-
-    # Close dialog on user response
-    dialog.connect("response", lambda d, r: d.destroy())
-    dialog.show()
-
 # -----------------------------------------------------------------------
 # Sleep just a little, but allow the system to breed
 
 def  usleep(msec):
 
     if sys.version_info[0] < 3 or \
         (sys.version_info[0] == 3 and sys.version_info[1] < 3):
@@ -1242,80 +956,14 @@
     return sss
 
 def time_s2n(sss):
     rrr = time.strptime(sss)
     ttt = time.mktime(rrr)
     return ttt
 
-def yes_no_cancel(title, message, cancel = True, parent = None):
-
-    #warnings.simplefilter("ignore")
-    dialog = Gtk.Dialog(title,
-                   None,
-                   Gtk.DialogFlags.MODAL | Gtk.DialogFlags.DESTROY_WITH_PARENT)
-
-
-    dialog.set_default_response(Gtk.ResponseType.YES)
-    dialog.set_position(Gtk.WindowPosition.CENTER)
-    dialog.set_transient_for(parent)
-
-    sp = "     "
-    label = Gtk.Label(message)
-    label2 = Gtk.Label(sp)
-    label3 = Gtk.Label(sp)
-    label2a = Gtk.Label(sp)
-    label3a = Gtk.Label(sp)
-
-    hbox = Gtk.HBox()
-
-    hbox.pack_start(label2, 0, 0, 0)
-    hbox.pack_start(label, 1, 1, 0)
-    hbox.pack_start(label3, 0, 0, 0)
-
-    dialog.vbox.pack_start(label2a, 0, 0, 0)
-    dialog.vbox.pack_start(hbox, 0, 0, 0)
-    dialog.vbox.pack_start(label3a, 0, 0, 0)
-
-    dialog.add_button("_Yes", Gtk.ResponseType.YES)
-    dialog.add_button("_No", Gtk.ResponseType.NO)
-
-    if cancel:
-        dialog.add_button("_Cancel", Gtk.ResponseType.CANCEL)
-
-    dialog.connect("key-press-event", yn_key, cancel)
-    #dialog.connect("key-release-event", yn_key, cancel)
-    #warnings.simplefilter("default")
-
-    dialog.show_all()
-    response = dialog.run()
-    # Convert all responses to cancel
-    if  response == Gtk.ResponseType.CANCEL or \
-        response == Gtk.ResponseType.REJECT or \
-        response == Gtk.ResponseType.CLOSE  or \
-        response == Gtk.ResponseType.DELETE_EVENT:
-        response = Gtk.ResponseType.CANCEL
-    dialog.destroy()
-
-    return  response
-
-def yn_key(win, event, cancel):
-    #print( event)
-    if event.keyval == Gdk.KEY_y or \
-        event.keyval == Gdk.KEY_Y:
-        win.response(Gtk.ResponseType.YES)
-
-    if event.keyval == Gdk.KEY_n or \
-        event.keyval == Gdk.KEY_N:
-        win.response(Gtk.ResponseType.NO)
-
-    if cancel:
-        if event.keyval == Gdk.KEY_c or \
-            event.keyval == Gdk.KEY_C:
-            win.response(Gtk.ResponseType.CANCEL)
-
 def opendialog(parent=None):
 
     # We create an array, so it is passed around by reference
     fname = [""]
 
     def makefilter(mask, name):
         filter =  Gtk.FileFilter.new()
```

### Comparing `pyvguicom-1.0.1/pyvguicom/pgwkit.py` & `pyvguicom-1.1.1/pyvguicom/pgwkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 
-''' This encapsulates the webkit '''
+''' This encapsulates the webkit import and failure thereof '''
 
 import os, sys, getopt, signal, random, time, warnings
 import inspect
 
-realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
-sys.path.append(realinc)
+#realinc = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pycommon")
+#sys.path.append(realinc)
 
 from pgutils import  *
 from pggui import  *
 from pgsimp import  *
 from pgtextview import  *
 
 import gi
@@ -18,33 +18,56 @@
 
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 
-class dummywebview():
+WebKit2 = None
+
+class dummywebview(Gtk.VBox):
+
+    def __int__(self):
+        super().__init__(self)
+        #self.pack_start(Gtk.Label(label="No WebView"), 1, 1, 0)
     def set_editable(self, flag):
+        self.pack_start(Gtk.Label(label="No WebView Available"), 1, 1, 0)
         pass
-    def load_html(self, ff, kk):
+    def load_html(self, ff, kk = None):
         pass
     def connect(self, aa, bb):
         pass
 
 class dummywebkit():
     WebView = dummywebview
-    def __init(self):
-        pass
-
-# Here is where / how the toolbar is constructed
 
-#    <toolitem action="new" />
-#    <toolitem action="open" />
-#    <toolitem action="save" tooltip="Hello" accelarator="<Ctrl>s"/>
-#    <separator />
+try:
+    gi.require_version("WebKit2", '4.1')
+    from gi.repository import WebKit2
+    #present = 1
+except:
+    try:
+        #print("Trying V 4.0:", sys.exc_info())
+        gi.require_version("WebKit2", '4.0')
+        from gi.repository import WebKit2
+    except:
+        try:
+            #print("Trying with jno qualifier")
+            #gi.require_version("WebKit2", '4.0')
+            from gi.repository import WebKit2
+        except:
+            # Giving up, patch fake one
+            print("Cannot import:", sys.exc_info())
+            print("WebWiew is not available.")
+            try:
+                WebKit2 = dummywebkit
+            except:
+                print("Fake kit Exc:", sys.exc_info())
+            #print("Fake kit:", WebKit2)
+            #raise
 
 ui_def = """
         <ui>
             <toolbar name="toolbar_format">
                 <toolitem action="cut" />
                 <toolitem action="copy" />
                 <toolitem action="paste" />
@@ -76,28 +99,14 @@
                 <toolitem action="H2" />
                 <toolitem action="H3" />
                 <toolitem action="H4" />
             </toolbar>
         </ui>
         """
 
-try:
-    gi.require_version('WebKit2', '4.0')
-    from gi.repository import WebKit2
-
-    #print(WebKit2)
-    #print("Webkit ver", WebKit2.get_major_version(), WebKit2.get_minor_version(), WebKit2.get_micro_version())
-    present = 1
-
-except:
-    print("Cannot import webkit2, web functions may not be available.")
-    present = 0
-    WebKit2 = dummywebkit
-    #raise
-
 #unmask_reserved =   Gdk.ModifierType.GDK_MODIFIER_RESERVED_13_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_14_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_15_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_16_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_17_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_18_MASK | \
 #                    Gdk.ModifierType.GDK_MODIFIER_RESERVED_19_MASK | \
```

### Comparing `pyvguicom-1.0.1/pyvguicom/plug.py` & `pyvguicom-1.1.1/pyvguicom/plug.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.1/pyvguicom/testbutt.py` & `pyvguicom-1.1.1/pyvguicom/testbutt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 import sys
 
 import gi
 gi.require_version("Gtk", "3.0")
 
 from gi.repository import Gtk
```

### Comparing `pyvguicom-1.0.1/pyvguicom/testcust.py` & `pyvguicom-1.1.1/pyvguicom/testcust.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 import os, sys, getopt, signal, select, string, time
 import struct, stat, base64, random, zlib
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
```

### Comparing `pyvguicom-1.0.1/pyvguicom/testentry.py` & `pyvguicom-1.1.1/pyvguicom/testnums.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,93 +1,127 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 from __future__ import print_function
 
 import os, sys, getopt, signal, select, string, time
 import struct, stat, base64, random, zlib
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GObject
 from gi.repository import GLib
 
-import pgentry
-import pgutils
-import pggui
+from pgsel import *
+from pgutils import *
+from pggui import *
+from pgbox import *
+
+#def OnExit(arg1, arg2):
+#    #print("Exiting", arg1, arg2)
+#    Gtk.main_quit()
 
 # ------------------------------------------------------------------------
 class testwin(Gtk.Window):
 
     def __init__(self):
         Gtk.Window.__init__(self)
+        #self.set_default_size(1024, 768)
         #self.set_default_size(800, 600)
         self.set_position(Gtk.WindowPosition.CENTER)
         self.connect("unmap", Gtk.main_quit)
 
 # ------------------------------------------------------------------------
 
 class pgtestwin(testwin):
 
     def __init__(self):
 
         testwin.__init__(self)
 
+        hbox  = Gtk.HBox(); hbox3 = Gtk.HBox()
+        hbox2 = Gtk.HBox(); hbox4 = Gtk.HBox()
         hbox5 = Gtk.HBox()
 
         self.label = Gtk.Label.new("Test strings here")
         hbox5.pack_start(self.label, 1, 1, 2)
 
-        gridx = Gtk.Grid()
-        gridx.set_column_spacing(6)
-        gridx.set_row_spacing(6)
-
         vbox  = Gtk.VBox()
 
-        rowcnt = 0
-        self.dat_dict = {}
-        sumx = Gtk.HBox()
-        buttx2 = Gtk.Button.new_with_mnemonic("Sele_ct Date")
-        tp1 =("Full Nam_e: ", "name", "Enter full name (TAB to advance)", None)
-        tp2 = ("Date o_f birth: ", "dob", "Date of birth, YYYY/MM/DD", None)
-        lab1, lab2 = pgentry.gridquad(gridx, rowcnt, 0, tp1, tp2, buttx2)
-        #buttx2.connect("clicked", self.pressed_dob, lab2)
-        self.dat_dict['name'] = lab1
-        self.dat_dict['dob'] = lab2
-        rowcnt += 1
-
-        #gridx.attach(pggui.vspacer(8), 0, rowcnt, 1, 1)
-
-        tp3 = ("Location of birth: ", "lob", "Location: City / Country", None)
-        tp4 = ("Nick Name: ", "nick", "Enter nick name / Alias if available", None)
-        lab3, lab4 = pgentry.gridquad(gridx, 0, rowcnt, tp3, tp4)
-        self.dat_dict['lob'] = lab3
-        self.dat_dict['nick'] = lab4
-        rowcnt += 1
-
-        tp6x = ("Notes: ", "", "Text for Notes. Press Shift Enter to advance", None)
-        lab6x = pgentry.gridsingle(gridx, 0, rowcnt, tp6x)
-        self.dat_dict['notes'] = lab6x
-        rowcnt += 1
+        vbox.pack_start(hbox2, 0, 0, 2)
+
+        hbox3.pack_start(Label("       Hour:  "), 0, 0, 2)
 
-        #gridx.attach(pggui.vspacer(8), 0, rowcnt, 1, 1)
-        #rowcnt += 1
+        self.hs2 = Spinner(0, 23, 0, self.change_hs2);
+        hbox3.pack_start(self.hs2, 0, 0, 2)
 
-        hbox2 = Gtk.HBox()
-        hbox2.pack_start(gridx, 1, 1, 2)
+        hbox3.pack_start(Label("       Min:  "), 0, 0, 2)
+        self.ms2 = Spinner(0, 59, 0, self.change_ms2);
+        hbox3.pack_start(self.ms2, 0, 0, 2)
 
-        vbox.pack_start(hbox2, 0, 0, 2)
+        hbox3.pack_start(Label(" "), 0, 0, 2)
+
+        hbox4.pack_start(Label(" "), 0, 0, 2)
+        self.ts4 = HourSel(self.change_ts4);
+        hbox4.pack_start(self.ts4, 0, 0, 2)
+
+        hbox4.pack_start(Label(" "), 0, 0, 2)
+        self.ts4a = MinSel(self.change_ts4a);
+        hbox4.pack_start(self.ts4a, 0, 0, 2)
+
+        vbox.pack_start(hbox3, 0, 0, 2)
+        vbox.pack_start(hbox4, 0, 0, 2)
+        vbox.pack_start(hbox, 1, 1, 2)
         vbox.pack_start(hbox5, 0, 0, 2)
 
         butt = Gtk.Button.new_with_mnemonic("E_xit")
         butt.connect("clicked", Gtk.main_quit)
         vbox.pack_start(butt, 0, 0, 2)
 
         self.add(vbox)
         self.show_all()
 
+    def  letterfilter(self, letter):
+        #print("letterfilter", letter)
+        self.label.set_text(letter)
+
+    def change_hs2(self, val):
+        #print("change_hs2", val)
+        self.label.set_text("hour: " + str(val))
+        pass
+
+    def change_ms2(self, val):
+        #print("change_ms2", val)
+        self.label.set_text("minute: " + str(val))
+        pass
+
+    def change_ts4(self, val):
+        #print("change_ms2", val)
+        self.label.set_text("H click: " + str(val))
+        pass
+
+    def change_ts4a(self, val):
+        #print("change_ms2", val)
+        self.label.set_text("M click: " + str(val))
+        pass
+
 tw = pgtestwin()
-#print("test")
-Gtk.main()
+cnt = 0;
+
+def  handler_tick(ww):
+
+    global cnt
+    #print("handler_tick", ww)
+
+    if cnt % 2 == 0:
+        tw.hs2.set_value(cnt)
+    else:
+        tw.ms2.set_value(cnt)
 
-# EOF
+    cnt += 1
+    GLib.timeout_add(1000, handler_tick, ww)
+
+
+GLib.timeout_add(1000, handler_tick, tw)
+
+Gtk.main()
```

### Comparing `pyvguicom-1.0.1/pyvguicom/testicons.py` & `pyvguicom-1.1.1/pyvguicom/testicons.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.1/pyvguicom/testlettsel.py` & `pyvguicom-1.1.1/pyvguicom/testlettsel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 from __future__ import print_function
 
 import os, sys, getopt, signal, select, string, time
 import struct, stat, base64, random, zlib
 
 from pgsel import *
```

### Comparing `pyvguicom-1.0.1/pyvguicom/testroot.py` & `pyvguicom-1.1.1/pyvguicom/testroot.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.1/pyvguicom/testsimple.py` & `pyvguicom-1.1.1/pyvguicom/testsimple.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 from __future__ import print_function
 
 import os, sys, getopt, signal, select, string, time
 import struct, stat, base64, random, zlib
 
 import gi
@@ -11,14 +11,15 @@
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 
 import pgsimp
 import pgutils
+import pgtests
 
 # ------------------------------------------------------------------------
 class testwin(Gtk.Window):
 
     def __init__(self):
         Gtk.Window.__init__(self)
         #self.set_default_size(1024, 768)
@@ -67,16 +68,16 @@
 tw = pgtestwin()
 
 #print("test")
 
 def fillrand():
     aaa = []
     for aa in range(10):
-        aaa.append( (pgutils.randstr(12), pgutils.randstr(12),
-                        pgutils.randstr(12), pgutils.randstr(12)) )
+        aaa.append( (pgtests.randstr(12), pgtests.randstr(12),
+                        pgtests.randstr(12), pgtests.randstr(12)) )
     return aaa
 
 aaa = fillrand()
 tw.treeview.clear()
 for aa in aaa:
     try:
         tw.treeview.append(aa)
```

### Comparing `pyvguicom-1.0.1/pyvguicom/testtextv.py` & `pyvguicom-1.1.1/pyvguicom/testtextv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 '''
   This is a test application for driving the pgTextView control;
   It has load / save functionality.
 '''
 import os, sys, getopt, signal, random, time, warnings
 
@@ -14,15 +14,15 @@
 from gi.repository import GObject
 from gi.repository import Pango
 
 import pgutils
 import pgtextview
 
 #deftext = "It puzzles me when I see a person lacking fundamentals is \
-#  able to amass a fortune to the tune of billions. What is even more \
+#  able to amass a fortune to the tune of billions. What is even more \3
 #puzziling is that they beleive their own 'BS' and openly flout all."
 
 # The pango example text
 
 deftext = \
 '''
 Text sizes: <span size="xx-small">tiny</span> <span size="x-small">very small</span> <span size="small">small</span> <span size="medium">normal</span> <span size="large">large</span> <span size="x-large">very large</span> <span size="xx-large">huge</span>
```

### Comparing `pyvguicom-1.0.1/pyvguicom.egg-info/PKG-INFO` & `pyvguicom-1.1.1/pyvguicom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvguicom
-Version: 1.0.1
+Version: 1.1.1
 Summary: High power secure server GUI utility helpers.
 Home-page: https://github.com/pglen/pyguicom.git
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `pyvguicom-1.0.1/pyvguicom.egg-info/SOURCES.txt` & `pyvguicom-1.1.1/pyvguicom.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,29 @@
 pyvguicom/htmledit.py
 pyvguicom/pgbox.py
 pyvguicom/pgbutt.py
 pyvguicom/pgentry.py
 pyvguicom/pggui.py
 pyvguicom/pgsel.py
 pyvguicom/pgsimp.py
+pyvguicom/pgtests.py
 pyvguicom/pgtextview.py
 pyvguicom/pgutils.py
 pyvguicom/pgwkit.py
 pyvguicom/plug.py
 pyvguicom/testbutt.py
 pyvguicom/testcust.py
 pyvguicom/testentry.py
+pyvguicom/testgui.py
 pyvguicom/testicons.py
 pyvguicom/testlettsel.py
+pyvguicom/testmsgs.py
 pyvguicom/testnums.py
 pyvguicom/testroot.py
 pyvguicom/testsimple.py
+pyvguicom/testtests.py
 pyvguicom/testtextv.py
+pyvguicom/testutils.py
 pyvguicom.egg-info/PKG-INFO
 pyvguicom.egg-info/SOURCES.txt
 pyvguicom.egg-info/dependency_links.txt
 pyvguicom.egg-info/top_level.txt
```

### Comparing `pyvguicom-1.0.1/setup.py` & `pyvguicom-1.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,17 +19,31 @@
           'Programming Language :: Python',
           'Topic :: Software Development :: Libraries',
         ]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+# Get version number from the file:
+fp = open("pyvguicom/pggui.py", "rt")
+vvv = fp.read(); fp.close()
+loc_vers =  '1.0.0'     # Default
+for aa in vvv.split("\n"):
+    idx = aa.find("VERSION =")
+    if idx == 0:        # At the beginning of line
+        try:
+            loc_vers = aa.split()[2].replace('"', "")
+            break
+        except:
+            pass
+#print("loc_vers:", loc_vers)
+
 setuptools.setup(
     name="pyvguicom",
-    version="1.0.1",
+    version=loc_vers,
     author="Peter Glen",
     author_email="peterglen99@gmail.com",
     description="High power secure server GUI utility helpers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pglen/pyguicom.git",
     classifiers= classx,
```

