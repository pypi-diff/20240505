# Comparing `tmp/beancount_parser-1.0.0.tar.gz` & `tmp/beancount_parser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_parser-1.0.0.tar", max compression
+gzip compressed data, was "beancount_parser-1.0.1.tar", max compression
```

## Comparing `beancount_parser-1.0.0.tar` & `beancount_parser-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1076 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/LICENSE
--rw-r--r--   0        0        0     2434 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/__init__.py
--rw-r--r--   0        0        0      335 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/account.lark
--rw-r--r--   0        0        0     3464 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/beancount.lark
--rw-r--r--   0        0        0       26 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/boolean.lark
--rw-r--r--   0        0        0       22 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/comment.lark
--rw-r--r--   0        0        0      162 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/currency.lark
--rw-r--r--   0        0        0      404 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/date.lark
--rw-r--r--   0        0        0      397 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/escaped_string.lark
--rw-r--r--   0        0        0      208 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/flag.lark
--rw-r--r--   0        0        0      223 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/link.lark
--rw-r--r--   0        0        0      162 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/numbers.lark
--rw-r--r--   0        0        0       29 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/section_header.lark
--rw-r--r--   0        0        0      289 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/grammar/tag.lark
--rw-r--r--   0        0        0      403 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/beancount_parser/parser.py
--rw-r--r--   0        0        0      529 2024-03-17 01:01:37.029895 beancount_parser-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 beancount_parser-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2434 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/__init__.py
+-rw-r--r--   0        0        0      335 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/account.lark
+-rw-r--r--   0        0        0     3467 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/beancount.lark
+-rw-r--r--   0        0        0       26 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/boolean.lark
+-rw-r--r--   0        0        0       22 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/comment.lark
+-rw-r--r--   0        0        0      162 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/currency.lark
+-rw-r--r--   0        0        0      404 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/date.lark
+-rw-r--r--   0        0        0      397 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/escaped_string.lark
+-rw-r--r--   0        0        0      208 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/flag.lark
+-rw-r--r--   0        0        0      223 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/link.lark
+-rw-r--r--   0        0        0      162 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/numbers.lark
+-rw-r--r--   0        0        0       29 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/section_header.lark
+-rw-r--r--   0        0        0      289 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/grammar/tag.lark
+-rw-r--r--   0        0        0      403 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/beancount_parser/parser.py
+-rw-r--r--   0        0        0      529 2024-05-05 17:12:00.749791 beancount_parser-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 beancount_parser-1.0.1/PKG-INFO
```

### Comparing `beancount_parser-1.0.0/LICENSE` & `beancount_parser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_parser-1.0.0/README.md` & `beancount_parser-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `beancount_parser-1.0.0/beancount_parser/grammar/beancount.lark` & `beancount_parser-1.0.1/beancount_parser/grammar/beancount.lark`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 simple_directive: option
                  | include
                  | plugin
 
 // Posting
 total_cost: "{{" amount "}}"
 both_cost: "{" number_expr  "#" amount "}"
-cost_spec: "{" cost_item ["," cost_item]* "}"
+cost_spec: "{" (cost_item ("," cost_item)*)? "}"
 cost_item: amount | DATE | ESCAPED_STRING | ASTERISK
 ?cost: total_cost | both_cost | cost_spec
 
 per_unit_price: "@" amount
 total_price: "@@" amount
 ?posting_price: per_unit_price | total_price
```

### Comparing `beancount_parser-1.0.0/pyproject.toml` & `beancount_parser-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beancount-parser"
-version = "1.0.0"
+version = "1.0.1"
 description = "Standalone Lark based Beancount syntax parser (not relying on Beancount library), MIT license"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/beancount-parser"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `beancount_parser-1.0.0/PKG-INFO` & `beancount_parser-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-parser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Standalone Lark based Beancount syntax parser (not relying on Beancount library), MIT license
 Home-page: https://github.com/LaunchPlatform/beancount-parser
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: beancount-parser Version: 1.0.0 Summary: Standalone
+Metadata-Version: 2.1 Name: beancount-parser Version: 1.0.1 Summary: Standalone
 Lark based Beancount syntax parser (not relying on Beancount library), MIT
 license Home-page: https://github.com/LaunchPlatform/beancount-parser License:
 MIT Author: Fang-Pen Lin Author-email: fangpen@launchplatform.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: lark
```

