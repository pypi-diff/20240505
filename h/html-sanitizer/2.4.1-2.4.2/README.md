# Comparing `tmp/html_sanitizer-2.4.1.tar.gz` & `tmp/html_sanitizer-2.4.2.tar.gz`

## Comparing `html_sanitizer-2.4.1.tar` & `html_sanitizer-2.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/.editorconfig
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/CHANGELOG.rst
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/tox.ini
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/html_sanitizer/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/html_sanitizer/__main__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/html_sanitizer/django.py
--rw-r--r--   0        0        0    13787 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/html_sanitizer/sanitizer.py
--rw-r--r--   0        0        0    24288 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/html_sanitizer/tests.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/.gitignore
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/LICENSE
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/README.rst
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 html_sanitizer-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/.editorconfig
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/CHANGELOG.rst
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/tox.ini
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/html_sanitizer/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/html_sanitizer/__main__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/html_sanitizer/django.py
+-rw-r--r--   0        0        0    13787 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/html_sanitizer/sanitizer.py
+-rw-r--r--   0        0        0    24536 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/html_sanitizer/tests.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/.gitignore
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/LICENSE
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/README.rst
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 html_sanitizer-2.4.2/PKG-INFO
```

### Comparing `html_sanitizer-2.4.1/.pre-commit-config.yaml` & `html_sanitizer-2.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.1/CHANGELOG.rst` & `html_sanitizer-2.4.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 ==========
 Change log
 ==========
 
 Next version
 ============
 
+- **Vulnerability:** Fixed an issue where normalizing unicode too late in the
+  process would keep disallowed tags when using specially crafted HTML. Fixed
+  in 2.4.2.
+
+
 2.4 (2024-04-01)
 ================
 
 - Fixed an edge case where ``br`` tag attributes weren't removed if the br tag
   appears first.
 - Updated the ``lxml`` dependency to 5.2 and added the now-required
   ``lxml[html_clean]`` extra.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_mcpiy3bb_/tmp9lsr2aqb_TarContainer/0/2.rst", line 184, column 0: CDATA terminal not found*

```diff
@@ -1,11 +1,13 @@
-========== Change log ========== Next version ============ 2.4 (2024-04-01)
-================ - Fixed an edge case where ``br`` tag attributes weren't
-removed if the br tag appears first. - Updated the ``lxml`` dependency to 5.2
-and added the now-required ``lxml[html_clean]`` extra. 2.3 (2024-02-07)
+========== Change log ========== Next version ============ - **Vulnerability:**
+Fixed an issue where normalizing unicode too late in the process would keep
+disallowed tags when using specially crafted HTML. Fixed in 2.4.2. 2.4 (2024-
+04-01) ================ - Fixed an edge case where ``br`` tag attributes
+weren't removed if the br tag appears first. - Updated the ``lxml`` dependency
+to 5.2 and added the now-required ``lxml[html_clean]`` extra. 2.3 (2024-02-07)
 ================ - Avoided adding whitespace when merging tags of the same
 type. - Updated the tests. - Switched from black to the ruff formatter. 2.2
 (2023-07-03) ================ - Changed ``keep_normalized_whitespace`` to
 preserve whitespace at the tail of tags, not just between tags. - Changed the
 parameters of ``normalize_whitespace_in_text_or_tail`` to be keyword-only. 2.1
 (2023-06-29) ================ - Added a test for a type of misconfiguration. -
 Changed the sanitizer configuration validation to not allow unexpected data
```

### Comparing `html_sanitizer-2.4.1/.github/workflows/test.yml` & `html_sanitizer-2.4.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.1/html_sanitizer/django.py` & `html_sanitizer-2.4.2/html_sanitizer/django.py`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.1/html_sanitizer/sanitizer.py` & `html_sanitizer-2.4.2/html_sanitizer/sanitizer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,20 @@
         Clean HTML code from ugly copy-pasted CSS and empty elements
 
         Removes everything not explicitly allowed in ``self.allowed_tags``.
 
         Requires ``lxml`` and, for especially broken HTML, ``beautifulsoup4``.
         """
 
+        # normalize unicode
+        if self.keep_typographic_whitespace:
+            html = unicodedata.normalize("NFC", html)
+        else:
+            html = unicodedata.normalize("NFKC", html)
+
         html = normalize_overall_whitespace(
             html,
             keep_typographic_whitespace=self.keep_typographic_whitespace,
             whitespace_re=self.whitespace_re,
         )
         html = "<div>%s</div>" % html
         try:
@@ -416,14 +422,8 @@
 
         # add a space before the closing slash in empty tags
         html = re.sub(r"<([^/>]+)/>", r"<\1 />", html)
 
         # remove wrapping tag needed by XML parser
         html = re.sub(r"^<div>|</div>$", "", html)
 
-        # normalize unicode
-        if self.keep_typographic_whitespace:
-            html = unicodedata.normalize("NFC", html)
-        else:
-            html = unicodedata.normalize("NFKC", html)
-
         return html
```

### Comparing `html_sanitizer-2.4.1/html_sanitizer/tests.py` & `html_sanitizer-2.4.2/html_sanitizer/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -651,7 +651,17 @@
         self.run_tests(
             [
                 ("<p><br hello=\"alert('world');\"/><br></p>", ""),
                 ('<p hello="world"></p>', ""),
                 ("<br hello=\"alert('world');\"/><br>", "<br>"),
             ]
         )
+
+    def test_normalize_early(self):
+        self.run_tests(
+            [
+                (
+                    "\uff1cimg src=x onerror=\uff02alert(window.location)\uff02\uff1e",
+                    "",
+                ),
+            ]
+        )
```

### Comparing `html_sanitizer-2.4.1/LICENSE` & `html_sanitizer-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.1/README.rst` & `html_sanitizer-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.1/pyproject.toml` & `html_sanitizer-2.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html_sanitizer-2.4.1/PKG-INFO` & `html_sanitizer-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-sanitizer
-Version: 2.4.1
+Version: 2.4.2
 Summary: HTML sanitizer
 Project-URL: Homepage, https://github.com/matthiask/html-sanitizer/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

