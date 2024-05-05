# Comparing `tmp/pyams_workflow-2.0.3.tar.gz` & `tmp/pyams_workflow-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_workflow-2.0.3.tar", last modified: Thu Feb  1 17:12:29 2024, max compression
+gzip compressed data, was "dist/pyams_workflow-2.1.0.tar", last modified: Sun May  5 20:54:55 2024, max compression
```

## Comparing `pyams_workflow-2.0.3.tar` & `pyams_workflow-2.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3364 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/docs/
--rwxrwxrwx   0 root         (0) root         (0)     1639 2024-02-01 17:09:05.000000 pyams_workflow-2.0.3/docs/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1185 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/docs/README.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2588 2024-02-01 17:09:05.000000 pyams_workflow-2.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow/
--rw-rw-rw-   0 root         (0) root         (0)      869 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13570 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/content.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow/doctests/
--rw-rw-rw-   0 root         (0) root         (0)    26510 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/doctests/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      951 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/include.py
--rw-rw-rw-   0 root         (0) root         (0)    21258 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/interfaces.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5556 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.mo
--rw-rw-rw-   0 root         (0) root         (0)     7944 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.po
--rw-rw-rw-   0 root         (0) root         (0)     5733 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/locales/pyams_workflow.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1781 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)    14546 2024-02-01 17:09:05.000000 pyams_workflow-2.0.3/src/pyams_workflow/versions.py
--rw-rw-rw-   0 root         (0) root         (0)    13568 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow/zmi/
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5561 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/zmi/history.py
--rw-rw-rw-   0 root         (0) root         (0)     4952 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/zmi/transition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow/zmi/viewlet/
--rw-rw-rw-   0 root         (0) root         (0)      572 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/zmi/viewlet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2961 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/zmi/viewlet/transitions.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2024-01-03 15:38:06.000000 pyams_workflow-2.0.3/src/pyams_workflow/zmi/viewlet/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3364 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1120 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 17:12:22.000000 pyams_workflow-2.0.3/src/pyams_workflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      281 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-02-01 17:12:29.000000 pyams_workflow-2.0.3/src/pyams_workflow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3569 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     1844 2024-05-05 20:50:28.000000 pyams_workflow-2.1.0/docs/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/docs/README.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2588 2024-05-05 20:50:28.000000 pyams_workflow-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow/
+-rw-rw-rw-   0 root         (0) root         (0)      869 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13570 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)    26606 2024-05-05 20:50:28.000000 pyams_workflow-2.1.0/src/pyams_workflow/doctests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/include.py
+-rw-rw-rw-   0 root         (0) root         (0)    21258 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow/locales/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow/locales/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     5556 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.mo
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.po
+-rw-rw-rw-   0 root         (0) root         (0)     5733 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/locales/pyams_workflow.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)    14546 2024-02-01 17:09:05.000000 pyams_workflow-2.1.0/src/pyams_workflow/versions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13745 2024-05-05 20:50:28.000000 pyams_workflow-2.1.0/src/pyams_workflow/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5631 2024-05-05 20:50:28.000000 pyams_workflow-2.1.0/src/pyams_workflow/zmi/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     4952 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/zmi/transition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow/zmi/viewlet/
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/zmi/viewlet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3251 2024-05-05 20:50:28.000000 pyams_workflow-2.1.0/src/pyams_workflow/zmi/viewlet/transitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2024-01-03 15:38:06.000000 pyams_workflow-2.1.0/src/pyams_workflow/zmi/viewlet/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3569 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 20:54:48.000000 pyams_workflow-2.1.0/src/pyams_workflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      281 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-05 20:54:55.000000 pyams_workflow-2.1.0/src/pyams_workflow.egg-info/top_level.txt
```

### Comparing `pyams_workflow-2.0.3/LICENSE` & `pyams_workflow-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/PKG-INFO` & `pyams_workflow-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_workflow
-Version: 2.0.3
+Version: 2.1.0
 Summary: PyAMS workflow management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS workflow
 Classifier: License :: OSI Approved :: Zope Public License
@@ -47,14 +47,20 @@
 Please note however that this package doesn't provide any management interface, so can probably
 be reused easily outside of Pyramid.
 
 
 Changelog
 =========
 
+2.1.0
+-----
+ - added support for dividers in workflow transitions dropdown menu
+ - added marker interface to history table to support extension viewlets
+ - updated principal getter when firing transition
+
 2.0.3
 -----
  - added check in versions helper for contents not supporting versioning
 
 2.0.2
 -----
  - updated ZMI dependency
```

### Comparing `pyams_workflow-2.0.3/docs/HISTORY.rst` & `pyams_workflow-2.1.0/docs/HISTORY.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+2.1.0
+-----
+ - added support for dividers in workflow transitions dropdown menu
+ - added marker interface to history table to support extension viewlets
+ - updated principal getter when firing transition
+
 2.0.3
 -----
  - added check in versions helper for contents not supporting versioning
 
 2.0.2
 -----
  - updated ZMI dependency
```

### Comparing `pyams_workflow-2.0.3/docs/README.rst` & `pyams_workflow-2.1.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/setup.py` & `pyams_workflow-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.rst')
 HISTORY = os.path.join(DOCS, 'HISTORY.rst')
 
-version = '2.0.3'
+version = '2.1.0'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_zmi > 2.1.0',
     'pyramid_zcml',
     'zope.exceptions'
 ]
```

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/__init__.py` & `pyams_workflow-2.1.0/src/pyams_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/content.py` & `pyams_workflow-2.1.0/src/pyams_workflow/content.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/doctests/README.rst` & `pyams_workflow-2.1.0/src/pyams_workflow/doctests/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -192,14 +192,15 @@
     >>> delete = Transition(transition_id='delete',
     ...                     title="Delete version",
     ...                     source=DRAFT,
     ...                     destination=DELETED,
     ...                     condition=can_delete_version,
     ...                     action=delete_action,
     ...                     menu_icon_class='fab fa-trash',
+    ...                     menu_divider=True,
     ...                     history_label="Version deleted",
     ...                     order=99)
 
     >>> wf_transitions = {init,
     ...                   draft_to_published,
     ...                   published_to_archived,
     ...                   published_to_draft,
@@ -711,14 +712,15 @@
             <a class="dropdown-item pl-3 "
                href="http://example.com/content/++versions++/4/wf-transition.html?workflow.widgets.transition_id=draft_to_published"
                data-toggle="modal"
                data-ams-modules="modal">
                 <i class="fa fa-fw mr-1"></i>
                 Publish
             </a>
+            <div class="dropdown-divider"></div>
             <a class="dropdown-item pl-3 "
                href="http://example.com/content/++versions++/4/wf-transition.html?workflow.widgets.transition_id=delete"
                data-toggle="modal"
                data-ams-modules="modal">
                 <i class="fab fa-trash fa-fw mr-1"></i>
                 Delete version
             </a>
```

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/include.py` & `pyams_workflow-2.1.0/src/pyams_workflow/include.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/interfaces.py` & `pyams_workflow-2.1.0/src/pyams_workflow/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.mo` & `pyams_workflow-2.1.0/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.mo`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.po` & `pyams_workflow-2.1.0/src/pyams_workflow/locales/fr/LC_MESSAGES/pyams_workflow.po`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/locales/pyams_workflow.pot` & `pyams_workflow-2.1.0/src/pyams_workflow/locales/pyams_workflow.pot`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/tests/__init__.py` & `pyams_workflow-2.1.0/src/pyams_workflow/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/tests/test_utilsdocs.py` & `pyams_workflow-2.1.0/src/pyams_workflow/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/tests/test_utilsdocstrings.py` & `pyams_workflow-2.1.0/src/pyams_workflow/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/versions.py` & `pyams_workflow-2.1.0/src/pyams_workflow/versions.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/workflow.py` & `pyams_workflow-2.1.0/src/pyams_workflow/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 from pyramid.httpexceptions import HTTPUnauthorized
 from zope.component import getUtilitiesFor
 from zope.interface import implementer
 from zope.lifecycleevent import ObjectModifiedEvent
 from zope.schema.vocabulary import SimpleTerm, SimpleVocabulary
 
+from pyams_security.interfaces.base import IPrincipalInfo
 from pyams_utils.adapter import adapter_config
 from pyams_utils.registry import get_utility
 from pyams_utils.request import check_request
 from pyams_utils.traversing import get_parent
 from pyams_utils.vocabulary import vocabulary_config
 from pyams_workflow.interfaces import AUTOMATIC_TRANSITION, AmbiguousTransitionError, \
     ConditionFailedError, IWorkflow, IWorkflowInfo, IWorkflowManagedContent, IWorkflowState, \
@@ -170,15 +171,16 @@
     def fire_transition(self, transition_id, comment=None, side_effect=None,
                         check_security=True, principal=None, request=None):
         # pylint: disable=too-many-arguments
         """Fire transition with given ID"""
         versions = IWorkflowVersions(self.parent)
         state = IWorkflowState(self.context)
         if request is None:
-            request = check_request()
+            principal_id = principal.id if IPrincipalInfo.providedBy(principal) else principal
+            request = check_request(principal_id=principal_id)
         # this raises InvalidTransitionError if id is invalid for current state
         transition = self.wf.get_transition(state.state, transition_id)
         # check whether we may execute this workflow transition
         if check_security and transition.permission:
             if not request.has_permission(transition.permission, context=self.context):
                 raise HTTPUnauthorized()
         # now make sure transition can still work in this context
@@ -292,15 +294,15 @@
 
     def get_fireable_transition_ids_toward(self, state, check_security=True):
         """Get IDs of transitions which can be fired to access given state"""
         result = []
         for transition_id in self.get_fireable_transition_ids(check_security):
             transition = self.wf.get_transition_by_id(transition_id)
             if transition.destination == state:
-                result.append( transition_id)
+                result.append(transition_id)
         return result
 
     def get_automatic_transition_ids(self):
         """Get IDs of automatic transitions"""
         return [
             transition.transition_id
             for transition in self._get_transitions(AUTOMATIC_TRANSITION)
```

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/zmi/__init__.py` & `pyams_workflow-2.1.0/src/pyams_workflow/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/zmi/history.py` & `pyams_workflow-2.1.0/src/pyams_workflow/zmi/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # FOR A PARTICULAR PURPOSE.
 #
 
 """PyAMS_workflow.zmi.versions module
 
 """
 
-from zope.interface import Interface
+from pyramid.interfaces import IView
+from zope.interface import Interface, implementer
 
 from pyams_layer.interfaces import IPyAMSLayer
 from pyams_pagelet.pagelet import pagelet_config
 from pyams_security.interfaces.base import VIEW_SYSTEM_PERMISSION
 from pyams_security.principal import MissingPrincipal
 from pyams_security.utility import get_principal
 from pyams_table.column import GetAttrColumn
@@ -46,14 +47,15 @@
     """Workflow history menu item"""
 
     label = _("Version history")
     icon_class = 'fas fa-history'
     href = '#version-history.html'
 
 
+@implementer(IView)
 class WorkflowVersionHistoryTable(Table):
     """Workflow version history table"""
 
     object_data = {
         'responsive': True,
         'auto-width': False,
         'searching': False,
```

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/zmi/transition.py` & `pyams_workflow-2.1.0/src/pyams_workflow/zmi/transition.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/zmi/viewlet/__init__.py` & `pyams_workflow-2.1.0/src/pyams_workflow/zmi/viewlet/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/zmi/viewlet/transitions.py` & `pyams_workflow-2.1.0/src/pyams_workflow/zmi/viewlet/transitions.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 This module defines a viewlet which can be used to display a dropdown menu
 of all available content transitions.
 """
 
 from zope.interface import Interface
 
-from pyams_skin.viewlet.menu import DropdownMenu, MenuItem
+from pyams_skin.viewlet.menu import DropdownMenu, MenuDivider, MenuItem
 from pyams_utils.registry import get_utility
 from pyams_utils.traversing import get_parent
 from pyams_utils.url import absolute_url
 from pyams_viewlet.viewlet import viewlet_config
 from pyams_workflow.interfaces import IWorkflow, IWorkflowInfo, IWorkflowManagedContent, \
     IWorkflowVersion
 from pyams_zmi.interfaces import IAdminLayer
@@ -43,15 +43,15 @@
         self.label = transition.title
         self.icon_class = transition.user_data.get('menu_icon_class') or 'fa'
         self.href = '{url}?workflow.widgets.transition_id={transition}'.format(
             url=absolute_url(context, request,
                              transition.user_data.get('view_name', 'wf-transition.html')),
             transition=transition.transition_id)
         self.modal_target = True
-        self.weight = transition.order
+        self.weight = transition.order * 10
 
 
 @viewlet_config(name='pyams_workflow.transitions',
                 context=IWorkflowVersion, layer=IAdminLayer, view=Interface,
                 manager=IToolbarViewletManager, weight=200)
 class WorkflowTransitionsMenu(DropdownMenu):
     """Workflow transitions menu"""
@@ -65,10 +65,14 @@
         content = get_parent(self.context, IWorkflowManagedContent)
         wf = get_utility(IWorkflow, name=content.workflow_name)  # pylint: disable=invalid-name
         if wf is None:
             return viewlets
         info = IWorkflowInfo(self.context)
         for transition_id in info.get_manual_transition_ids():
             transition = wf.get_transition_by_id(transition_id)
+            if transition.user_data.get('menu_divider'):
+                divider = MenuDivider(self.context, self.request, self.view, None)
+                divider.weight = (transition.order * 10) - 1
+                viewlets.append((f'{transition_id}_divider', divider))
             menu = TransitionMenuItem(self.context, self.request, self.view, self, transition)
             viewlets.append((transition_id, menu))
         return sorted(viewlets, key=lambda x: x[1].weight)
```

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow/zmi/viewlet/versions.py` & `pyams_workflow-2.1.0/src/pyams_workflow/zmi/viewlet/versions.py`

 * *Files identical despite different names*

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow.egg-info/PKG-INFO` & `pyams_workflow-2.1.0/src/pyams_workflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-workflow
-Version: 2.0.3
+Version: 2.1.0
 Summary: PyAMS workflow management package
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Keywords: Pyramid PyAMS workflow
 Classifier: License :: OSI Approved :: Zope Public License
@@ -47,14 +47,20 @@
 Please note however that this package doesn't provide any management interface, so can probably
 be reused easily outside of Pyramid.
 
 
 Changelog
 =========
 
+2.1.0
+-----
+ - added support for dividers in workflow transitions dropdown menu
+ - added marker interface to history table to support extension viewlets
+ - updated principal getter when firing transition
+
 2.0.3
 -----
  - added check in versions helper for contents not supporting versioning
 
 2.0.2
 -----
  - updated ZMI dependency
```

### Comparing `pyams_workflow-2.0.3/src/pyams_workflow.egg-info/SOURCES.txt` & `pyams_workflow-2.1.0/src/pyams_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

