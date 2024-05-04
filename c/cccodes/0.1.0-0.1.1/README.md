# Comparing `tmp/cccodes-0.1.0.tar.gz` & `tmp/cccodes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cccodes-0.1.0.tar", max compression
+gzip compressed data, was "cccodes-0.1.1.tar", max compression
```

## Comparing `cccodes-0.1.0.tar` & `cccodes-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1296 2024-05-04 18:04:42.667504 cccodes-0.1.0/LICENSE
--rw-r--r--   0        0        0     1821 2024-05-04 18:15:41.851253 cccodes-0.1.0/README.md
--rw-r--r--   0        0        0       71 2024-05-04 13:21:11.318859 cccodes-0.1.0/cccodes/__init__.py
--rw-r--r--   0        0        0      518 2024-05-04 13:21:11.317585 cccodes-0.1.0/cccodes/badwords.py
--rw-r--r--   0        0        0     2182 2024-05-04 13:21:11.318468 cccodes-0.1.0/cccodes/coupon.py
--rw-r--r--   0        0        0      270 2024-05-04 13:21:11.318029 cccodes-0.1.0/cccodes/couponcode_test.py
--rw-r--r--   0        0        0      498 2024-05-04 19:45:38.186194 cccodes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 cccodes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1296 2024-05-04 18:04:42.667504 cccodes-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1821 2024-05-04 18:15:41.851253 cccodes-0.1.1/README.md
+-rw-r--r--   0        0        0       71 2024-05-04 13:21:11.318859 cccodes-0.1.1/cccodes/__init__.py
+-rw-r--r--   0        0        0      715 2024-05-04 21:53:30.894408 cccodes-0.1.1/cccodes/badwords.py
+-rw-r--r--   0        0        0     2174 2024-05-04 21:51:17.022476 cccodes-0.1.1/cccodes/coupon.py
+-rw-r--r--   0        0        0      314 2024-05-04 21:51:56.673249 cccodes-0.1.1/cccodes/couponcode_test.py
+-rw-r--r--   0        0        0      498 2024-05-04 21:57:26.799054 cccodes-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 cccodes-0.1.1/PKG-INFO
```

### Comparing `cccodes-0.1.0/LICENSE` & `cccodes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cccodes-0.1.0/README.md` & `cccodes-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cccodes-0.1.0/cccodes/coupon.py` & `cccodes-0.1.1/cccodes/coupon.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 https://www.mclean.net.nz/cpan/couponcode/
 Coupon Codes from https://github.com/grantm/Algorithm-CouponCode?tab=readme-ov-file
 
 # quick runs:
-python3 -c "import couponcodes.coupon as c; print(c.generate())"
+python3 -c "import cccodes.coupon as c; print(c.generate())"
 
-python3 -c "import couponcodes.coupon as c; print(c.validate('T13P-2LMP-E0B5'))"
+python3 -c "import cccodes.coupon as c; print(c.validate('T13P-2LMP-E0B5'))"
 
 """
 
 import secrets
 import string
 
 from .badwords import bad_words
```

### Comparing `cccodes-0.1.0/PKG-INFO` & `cccodes-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: cccodes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Coupon codes algorithm
 License: BSD 2-Clause License
 Author: birlorg
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Description-Content-Type: text/markdown
 
 # couponcodes
 
 Implements the Coupon Codes Algorithm from Dan Mclean:
 
 - https://www.mclean.net.nz/cpan/couponcode/
```

