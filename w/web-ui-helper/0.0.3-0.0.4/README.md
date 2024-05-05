# Comparing `tmp/web-ui-helper-0.0.3.tar.gz` & `tmp/web-ui-helper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-0.0.3.tar", last modified: Sun May  5 16:51:12 2024, max compression
+gzip compressed data, was "web-ui-helper-0.0.4.tar", last modified: Sun May  5 17:52:13 2024, max compression
```

## Comparing `web-ui-helper-0.0.3.tar` & `web-ui-helper-0.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 16:51:12.843196 web-ui-helper-0.0.3/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      715 2024-05-05 16:51:12.840212 web-ui-helper-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 16:51:12.843196 web-ui-helper-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1297 2024-05-05 16:51:05.000000 web-ui-helper-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:51:12.790335 web-ui-helper-0.0.3/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.0.3/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:51:12.813276 web-ui-helper-0.0.3/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.0.3/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:51:12.819260 web-ui-helper-0.0.3/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-05 14:29:04.000000 web-ui-helper-0.0.3/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:51:12.821255 web-ui-helper-0.0.3/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.0.3/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:51:12.825244 web-ui-helper-0.0.3/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.0.3/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    27064 2024-05-05 15:41:22.000000 web-ui-helper-0.0.3/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:51:12.828236 web-ui-helper-0.0.3/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.0.3/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0     4643 2024-05-05 16:47:53.000000 web-ui-helper-0.0.3/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:51:12.832238 web-ui-helper-0.0.3/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     1615 2024-05-05 16:50:13.000000 web-ui-helper-0.0.3/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:51:12.835216 web-ui-helper-0.0.3/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.0.3/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-05 16:51:12.838208 web-ui-helper-0.0.3/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      715 2024-05-05 16:51:12.000000 web-ui-helper-0.0.3/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-05-05 16:51:12.000000 web-ui-helper-0.0.3/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 16:51:12.000000 web-ui-helper-0.0.3/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-05 16:51:12.000000 web-ui-helper-0.0.3/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-05 16:51:12.000000 web-ui-helper-0.0.3/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.743025 web-ui-helper-0.0.4/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      715 2024-05-05 17:52:13.741031 web-ui-helper-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 17:52:13.743025 web-ui-helper-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2024-05-05 17:52:08.000000 web-ui-helper-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.694156 web-ui-helper-0.0.4/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.0.4/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.716096 web-ui-helper-0.0.4/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.0.4/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.722133 web-ui-helper-0.0.4/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-05 14:29:04.000000 web-ui-helper-0.0.4/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.723102 web-ui-helper-0.0.4/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.727068 web-ui-helper-0.0.4/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    27222 2024-05-05 17:51:54.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.731057 web-ui-helper-0.0.4/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0     4643 2024-05-05 16:47:53.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.734073 web-ui-helper-0.0.4/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     1615 2024-05-05 16:50:13.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.738038 web-ui-helper-0.0.4/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.740052 web-ui-helper-0.0.4/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      715 2024-05-05 17:52:13.000000 web-ui-helper-0.0.4/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-05-05 17:52:13.000000 web-ui-helper-0.0.4/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 17:52:13.000000 web-ui-helper-0.0.4/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-05 17:52:13.000000 web-ui-helper-0.0.4/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-05 17:52:13.000000 web-ui-helper-0.0.4/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-0.0.3/LICENSE` & `web-ui-helper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/PKG-INFO` & `web-ui-helper-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.0.3/setup.py` & `web-ui-helper-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='0.0.3',
+    version='0.0.4',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-0.0.3/web_ui_helper/common/date_extend.py` & `web-ui-helper-0.0.4/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper/common/dir.py` & `web-ui-helper-0.0.4/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper/common/log.py` & `web-ui-helper-0.0.4/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper/common/metaclass.py` & `web-ui-helper-0.0.4/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper/common/platforms.py` & `web-ui-helper-0.0.4/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper/common/webdriver.py` & `web-ui-helper-0.0.4/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-0.0.4/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-0.0.4/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-0.0.4/web_ui_helper/selenium/frame/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -588,7 +588,12 @@
     )
 
 
 @loop_find_element
 def get_sub_element(element: WebElement, locator: str, regx: str, **kwargs) -> WebElement:
     kwargs.clear()
     return element.find_element(Locator.get(locator), regx)
+
+
+def js_click(driver: webdriver, element: WebElement):
+    # 使用 JavaScript 点击操作
+    driver.execute_script("arguments[0].click();", element)
```

### Comparing `web-ui-helper-0.0.3/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-0.0.4/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-0.0.4/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper/terminal/device.py` & `web-ui-helper-0.0.4/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.3/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-0.0.4/web_ui_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.0.3/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-0.0.4/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

