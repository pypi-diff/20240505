# Comparing `tmp/django_regex_match-0.2.5.tar.gz` & `tmp/django_regex_match-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_regex_match-0.2.5.tar", last modified: Wed Apr 17 21:49:39 2024, max compression
+gzip compressed data, was "django_regex_match-0.2.6.tar", last modified: Sun May  5 18:22:33 2024, max compression
```

## Comparing `django_regex_match-0.2.5.tar` & `django_regex_match-0.2.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-17 21:49:39.476656 django_regex_match-0.2.5/
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      116 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/MANIFEST.in
--rw-r--r--   0 sebastiang  (1000) sebastiang  (1000)      564 2024-04-17 21:49:39.476656 django_regex_match-0.2.5/PKG-INFO
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1597 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/README.md
-drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-17 21:49:39.476656 django_regex_match-0.2.5/django_regex_match.egg-info/
--rw-r--r--   0 sebastiang  (1000) sebastiang  (1000)      564 2024-04-17 21:49:39.000000 django_regex_match-0.2.5/django_regex_match.egg-info/PKG-INFO
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1246 2024-04-17 21:49:39.000000 django_regex_match-0.2.5/django_regex_match.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)        1 2024-04-17 21:49:39.000000 django_regex_match-0.2.5/django_regex_match.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)        1 2024-04-17 21:49:39.000000 django_regex_match-0.2.5/django_regex_match.egg-info/not-zip-safe
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)       79 2024-04-17 21:49:39.000000 django_regex_match-0.2.5/django_regex_match.egg-info/requires.txt
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      102 2024-04-17 21:49:39.000000 django_regex_match-0.2.5/django_regex_match.egg-info/top_level.txt
-drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-17 21:49:39.472656 django_regex_match-0.2.5/regex_match/
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      170 2024-04-17 21:46:55.000000 django_regex_match-0.2.5/regex_match/__init__.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1336 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/factory.py
-drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-17 21:49:39.476656 django_regex_match-0.2.5/regex_match/migrations/
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     5016 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/migrations/0001_initial.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      405 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/migrations/0002_modelrule_priority.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      374 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/migrations/0003_auto_20151110_1315.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      408 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/migrations/0004_auto_20151112_1808.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      409 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/migrations/0005_auto_20151117_2133.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      703 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/migrations/0006_auto_20160916_1428.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      494 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/migrations/0007_auto_20200715_1610.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/migrations/__init__.py
-drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-17 21:49:39.476656 django_regex_match-0.2.5/regex_match/models/
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      879 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/models/__init__.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      255 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/models/exception_parser.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      848 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/models/matching_rule.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      572 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/models/model_exception.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      707 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/models/model_rule.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      862 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/models/parser.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      290 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/models/parser_method.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      683 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/models/regex_rule.py
-drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-17 21:49:39.476656 django_regex_match-0.2.5/regex_match/objects/
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      880 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/objects/__init__.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      605 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/objects/exception_parser.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     2701 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/objects/model_matcher.py
-drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-04-17 21:49:39.476656 django_regex_match-0.2.5/regex_match/objects/parsers/
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      888 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/objects/parsers/__init__.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     6900 2024-04-17 21:48:54.000000 django_regex_match-0.2.5/regex_match/objects/parsers/url.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     2016 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/regex_match/objects/parsers/url_parser.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     3422 2024-04-17 21:48:06.000000 django_regex_match-0.2.5/regex_match/objects/url_to_matching_rule.py
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)       38 2024-04-17 21:49:39.476656 django_regex_match-0.2.5/setup.cfg
--rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1611 2024-04-17 21:46:28.000000 django_regex_match-0.2.5/setup.py
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-05-05 18:22:33.527535 django_regex_match-0.2.6/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      116 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/MANIFEST.in
+-rw-r--r--   0 sebastiang  (1000) sebastiang  (1000)      564 2024-05-05 18:22:33.527535 django_regex_match-0.2.6/PKG-INFO
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1597 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/README.md
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-05-05 18:22:33.527535 django_regex_match-0.2.6/django_regex_match.egg-info/
+-rw-r--r--   0 sebastiang  (1000) sebastiang  (1000)      564 2024-05-05 18:22:33.000000 django_regex_match-0.2.6/django_regex_match.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1246 2024-05-05 18:22:33.000000 django_regex_match-0.2.6/django_regex_match.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)        1 2024-05-05 18:22:33.000000 django_regex_match-0.2.6/django_regex_match.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)        1 2024-05-05 18:22:33.000000 django_regex_match-0.2.6/django_regex_match.egg-info/not-zip-safe
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)       79 2024-05-05 18:22:33.000000 django_regex_match-0.2.6/django_regex_match.egg-info/requires.txt
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      102 2024-05-05 18:22:33.000000 django_regex_match-0.2.6/django_regex_match.egg-info/top_level.txt
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-05-05 18:22:33.523535 django_regex_match-0.2.6/regex_match/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      170 2024-05-05 18:20:03.000000 django_regex_match-0.2.6/regex_match/__init__.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1336 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/factory.py
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-05-05 18:22:33.527535 django_regex_match-0.2.6/regex_match/migrations/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     5016 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/migrations/0001_initial.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      405 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/migrations/0002_modelrule_priority.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      374 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/migrations/0003_auto_20151110_1315.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      408 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/migrations/0004_auto_20151112_1808.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      409 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/migrations/0005_auto_20151117_2133.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      703 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/migrations/0006_auto_20160916_1428.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      494 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/migrations/0007_auto_20200715_1610.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)        0 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/migrations/__init__.py
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-05-05 18:22:33.527535 django_regex_match-0.2.6/regex_match/models/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      879 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/models/__init__.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      255 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/models/exception_parser.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      848 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/models/matching_rule.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      572 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/models/model_exception.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      707 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/models/model_rule.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      862 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/models/parser.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      290 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/models/parser_method.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      683 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/models/regex_rule.py
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-05-05 18:22:33.527535 django_regex_match-0.2.6/regex_match/objects/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      880 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/objects/__init__.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      605 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/objects/exception_parser.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     2701 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/objects/model_matcher.py
+drwxrwxr-x   0 sebastiang  (1000) sebastiang  (1000)        0 2024-05-05 18:22:33.527535 django_regex_match-0.2.6/regex_match/objects/parsers/
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)      888 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/objects/parsers/__init__.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     6892 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/objects/parsers/url.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     2016 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/regex_match/objects/parsers/url_parser.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     3100 2024-05-05 18:22:01.000000 django_regex_match-0.2.6/regex_match/objects/url_to_matching_rule.py
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)       38 2024-05-05 18:22:33.527535 django_regex_match-0.2.6/setup.cfg
+-rw-rw-r--   0 sebastiang  (1000) sebastiang  (1000)     1611 2024-05-05 18:16:58.000000 django_regex_match-0.2.6/setup.py
```

### Comparing `django_regex_match-0.2.5/PKG-INFO` & `django_regex_match-0.2.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-regex-match
-Version: 0.2.5
+Version: 0.2.6
 Home-page: http://www.admetricks.com/
 Author: Dev Admx
 Author-email: dev@admetricks.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `django_regex_match-0.2.5/README.md` & `django_regex_match-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/django_regex_match.egg-info/PKG-INFO` & `django_regex_match-0.2.6/django_regex_match.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-regex-match
-Version: 0.2.5
+Version: 0.2.6
 Home-page: http://www.admetricks.com/
 Author: Dev Admx
 Author-email: dev@admetricks.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `django_regex_match-0.2.5/django_regex_match.egg-info/SOURCES.txt` & `django_regex_match-0.2.6/django_regex_match.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/factory.py` & `django_regex_match-0.2.6/regex_match/factory.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/migrations/0001_initial.py` & `django_regex_match-0.2.6/regex_match/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/migrations/0006_auto_20160916_1428.py` & `django_regex_match-0.2.6/regex_match/migrations/0006_auto_20160916_1428.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/models/__init__.py` & `django_regex_match-0.2.6/regex_match/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/models/matching_rule.py` & `django_regex_match-0.2.6/regex_match/models/matching_rule.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/models/model_exception.py` & `django_regex_match-0.2.6/regex_match/models/model_exception.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/models/model_rule.py` & `django_regex_match-0.2.6/regex_match/models/model_rule.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/models/parser.py` & `django_regex_match-0.2.6/regex_match/models/parser.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/models/regex_rule.py` & `django_regex_match-0.2.6/regex_match/models/regex_rule.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/objects/__init__.py` & `django_regex_match-0.2.6/regex_match/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/objects/exception_parser.py` & `django_regex_match-0.2.6/regex_match/objects/exception_parser.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/objects/model_matcher.py` & `django_regex_match-0.2.6/regex_match/objects/model_matcher.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/objects/parsers/__init__.py` & `django_regex_match-0.2.6/regex_match/objects/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/objects/parsers/url.py` & `django_regex_match-0.2.6/regex_match/objects/parsers/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 raise ValueError("bad query field: %r" % (name_value,))
             # Handle case of a control-name with no equal sign
             if keep_blank_values:
                 nv.append('')
             else:
                 continue
         if len(nv[1]) or keep_blank_values:
-            # name = nv[0].replace('+', ' ')  noqa
+            name = nv[0].replace('+', ' ')
             name = unquote(name, encoding=encoding, errors=errors)
             name = _coerce_result(name)
             value = nv[1]
             r.append((name, value))
     return r
```

### Comparing `django_regex_match-0.2.5/regex_match/objects/parsers/url_parser.py` & `django_regex_match-0.2.6/regex_match/objects/parsers/url_parser.py`

 * *Files identical despite different names*

### Comparing `django_regex_match-0.2.5/regex_match/objects/url_to_matching_rule.py` & `django_regex_match-0.2.6/regex_match/objects/url_to_matching_rule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,77 @@
 from funcy import keep
 
 from regex_match.models import MatchingRule, ParserMethod, RegexRule
 from regex_match.objects.parsers import UrlParser
 
 
 class UrlToMatchingRule(object):
-    default_regex_template_domain = "((^.*[.])|^){}$"
-    default_regex_template_path = "^{}(/.*|)$"
-    default_regex_template_query = "(^|.+&){}={}($|&.+)"
+    default_regex_template_domain = '((^.*[.])|^){}$'
+    default_regex_template_path = '^{}(/.*|)$'
+    default_regex_template_query = '(^|.+(&|\?)){}={}($|&.+)'
 
     def __init__(
-        self,
-        model_rule,
-        urls,
-        priority_func=None,
-        description="",
-        regex_template_domain=None,
-        regex_template_path=None,
-        regex_template_query=None,
-    ):
-        self.regex_template_domain = (
-            regex_template_domain or self.default_regex_template_domain
-        )
-        self.regex_template_path = (
-            regex_template_path or self.default_regex_template_path
-        )
-        self.regex_template_query = (
-            regex_template_query or self.default_regex_template_query
-        )
+            self, model_rule, urls, priority_func=None, description='',
+            regex_template_domain=None, regex_template_path=None,
+            regex_template_query=None):
+        self.regex_template_domain = regex_template_domain or self.default_regex_template_domain
+        self.regex_template_path = regex_template_path or self.default_regex_template_path
+        self.regex_template_query = regex_template_query or self.default_regex_template_query
 
         self.model_rule = model_rule
         self.urls = urls
         self.priority_func = priority_func
         self.description = description
 
     def create(self):
         matching_rule_array = keep(self._create_matching_rule, self.urls)
         return list(matching_rule_array)
 
     def _create_matching_rule(self, url):
         obj = UrlParser(url)
 
-        matching_rule = MatchingRule(
-            model_rule=self.model_rule, description=self.description
-        )
+        matching_rule = MatchingRule(model_rule=self.model_rule, description=self.description)
         matching_rule.save()
 
         domain_rule = self._create_domain_matching_rule(matching_rule, obj)
 
-        path_rule = self._create_path_matching_rule(
-            matching_rule, obj, bool(obj.url.query_params())
-        )
+        path_rule = self._create_path_matching_rule(matching_rule, obj, bool(obj.url.query_params()))
 
         query_rules = self._create_query_matching_rule(matching_rule, obj)
 
         if self.priority_func is not None:
             self.priority = self.priority_func(domain_rule, path_rule, query_rules)
 
         return matching_rule
 
     def _create_domain_matching_rule(self, matching_rule, url):
-        if url.domain() != "":
+        if url.domain() != '':
 
-            parser_method = ParserMethod.objects.get(name="domain")
+            parser_method = ParserMethod.objects.get(name='domain')
             return RegexRule.objects.create(
                 matching_rule=matching_rule,
                 parser_method=parser_method,
-                regex=self.regex_template_domain.format(
-                    url.domain().replace(".", "[.]").replace("+", "[+]")
-                ),
+                regex=self.regex_template_domain.format(url.domain().replace('.', '[.]'))
             )
 
     def _create_path_matching_rule(self, matching_rule, url, has_params):
-        if url.path() != "":
+        if url.path() != '':
             regex_template = self.regex_template_path
-            parser_method = ParserMethod.objects.get(name="path")
+            parser_method = ParserMethod.objects.get(name='path')
             return RegexRule.objects.create(
                 matching_rule=matching_rule,
                 parser_method=parser_method,
-                regex=regex_template.format(
-                    url.path().replace(".", "[.]").replace("+", "[+]")
-                ),
+                regex=regex_template.format(url.path().replace('.', '[.]'))
             )
 
     def _create_query_matching_rule(self, matching_rule, url):
         result = list()
         query_params = url.url.query_params()
         for k in query_params:
-            parser_method = ParserMethod.objects.get(name="query")
+            parser_method = ParserMethod.objects.get(name='query')
             rule = RegexRule.objects.create(
                 matching_rule=matching_rule,
                 parser_method=parser_method,
-                regex=self.regex_template_query.format(
-                    k, url.query_param(k).replace(".", "[.]").replace("+", "[+]")
-                ),
+                regex=self.regex_template_query.format(k, url.query_param(k).replace('.', '[.]'))
             )
             result.append(rule)
         return result
```

### Comparing `django_regex_match-0.2.5/setup.py` & `django_regex_match-0.2.6/setup.py`

 * *Files identical despite different names*

