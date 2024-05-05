# Comparing `tmp/web-ui-helper-0.0.4.tar.gz` & `tmp/web-ui-helper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-0.0.4.tar", last modified: Sun May  5 17:52:13 2024, max compression
+gzip compressed data, was "web-ui-helper-0.0.5.tar", last modified: Sun May  5 18:20:24 2024, max compression
```

## Comparing `web-ui-helper-0.0.4.tar` & `web-ui-helper-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.743025 web-ui-helper-0.0.4/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      715 2024-05-05 17:52:13.741031 web-ui-helper-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 17:52:13.743025 web-ui-helper-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1297 2024-05-05 17:52:08.000000 web-ui-helper-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.694156 web-ui-helper-0.0.4/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.0.4/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.716096 web-ui-helper-0.0.4/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.0.4/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.722133 web-ui-helper-0.0.4/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-05 14:29:04.000000 web-ui-helper-0.0.4/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.723102 web-ui-helper-0.0.4/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.727068 web-ui-helper-0.0.4/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    27222 2024-05-05 17:51:54.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.731057 web-ui-helper-0.0.4/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0     4643 2024-05-05 16:47:53.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.734073 web-ui-helper-0.0.4/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     1615 2024-05-05 16:50:13.000000 web-ui-helper-0.0.4/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.738038 web-ui-helper-0.0.4/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.0.4/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-05 17:52:13.740052 web-ui-helper-0.0.4/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      715 2024-05-05 17:52:13.000000 web-ui-helper-0.0.4/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-05-05 17:52:13.000000 web-ui-helper-0.0.4/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 17:52:13.000000 web-ui-helper-0.0.4/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-05 17:52:13.000000 web-ui-helper-0.0.4/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-05 17:52:13.000000 web-ui-helper-0.0.4/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 18:20:24.359809 web-ui-helper-0.0.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      715 2024-05-05 18:20:24.357815 web-ui-helper-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:20:24.359809 web-ui-helper-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2024-05-05 18:20:19.000000 web-ui-helper-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:20:24.310941 web-ui-helper-0.0.5/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.0.5/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:20:24.331885 web-ui-helper-0.0.5/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.0.5/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:20:24.338871 web-ui-helper-0.0.5/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-05 14:29:04.000000 web-ui-helper-0.0.5/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:20:24.339863 web-ui-helper-0.0.5/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.0.5/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:20:24.342856 web-ui-helper-0.0.5/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.0.5/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    27222 2024-05-05 17:51:54.000000 web-ui-helper-0.0.5/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:20:24.346845 web-ui-helper-0.0.5/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.0.5/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0     5206 2024-05-05 18:18:39.000000 web-ui-helper-0.0.5/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:20:24.349837 web-ui-helper-0.0.5/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     1615 2024-05-05 16:50:13.000000 web-ui-helper-0.0.5/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:20:24.353852 web-ui-helper-0.0.5/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.0.5/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:20:24.356829 web-ui-helper-0.0.5/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      715 2024-05-05 18:20:24.000000 web-ui-helper-0.0.5/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-05-05 18:20:24.000000 web-ui-helper-0.0.5/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:20:24.000000 web-ui-helper-0.0.5/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-05 18:20:24.000000 web-ui-helper-0.0.5/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-05 18:20:24.000000 web-ui-helper-0.0.5/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-0.0.4/LICENSE` & `web-ui-helper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/PKG-INFO` & `web-ui-helper-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.0.4/setup.py` & `web-ui-helper-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='0.0.4',
+    version='0.0.5',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-0.0.4/web_ui_helper/common/date_extend.py` & `web-ui-helper-0.0.5/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper/common/dir.py` & `web-ui-helper-0.0.5/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper/common/log.py` & `web-ui-helper-0.0.5/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper/common/metaclass.py` & `web-ui-helper-0.0.5/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper/common/platforms.py` & `web-ui-helper-0.0.5/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper/common/webdriver.py` & `web-ui-helper-0.0.5/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-0.0.5/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-0.0.5/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-0.0.5/web_ui_helper/selenium/frame/browser.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-0.0.5/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,42 +50,49 @@
             "index", "plane_no", "airline", "plane_type", "price", "price_uint",
             "depart_time", "depart_airport", "arrive_time", "cross_days", "arrive_airport"
         ]
         df = DataFrame(columns=columns)
         for index, element in elements_data.items():
             element = driver.find_element(Locator.get("xpath"), index_regx.format(index))
             # print(element.get_attribute('outerHTML'))
-            price = get_sub_element(element=element, locator="xpath", regx=price_regx, interval=1, loop=3).text.strip()
-            airline = get_sub_element(
+            price_element = get_sub_element(element=element, locator="xpath", regx=price_regx, interval=1, loop=3)
+            price = price_element.text.strip() if price_element else ""
+            airline_element = get_sub_element(
                 element=element, locator="xpath", regx=airline_regx, interval=1, loop=3
-            ).text.strip()
+            )
+            airline = airline_element.text.strip() if airline_element else ""
             plane_no = get_sub_element(element=element, locator="xpath", regx=plane_no_regx_1, interval=1, loop=3)
             if plane_no:
                 plane_no_slice = plane_no.text.strip().split()
                 plane_no = plane_no_slice[0].strip()
                 plane_type = plane_no_slice[1].strip()
             else:
                 plane_no = element.find_element(Locator.get("xpath"), plane_no_regx_2)
                 plane_no = plane_no.get_attribute('id').split("_")[0].split("-")[1].strip()
                 plane_type = ""
-            depart_time = get_sub_element(
+            depart_time_element = get_sub_element(
                 element=element, locator="xpath", regx=depart_time_regx, interval=1, loop=3
-            ).text.strip()
-            arrive_time_slice = get_sub_element(
+            )
+            depart_time = depart_time_element.text.strip() if depart_time_element else ""
+            arrive_time_element = get_sub_element(
                 element=element, locator="xpath", regx=arrive_time_regx, interval=1, loop=3
-            ).text.strip().split("\n")
-            depart_airport = get_sub_element(
+            )
+            arrive_time_slice = arrive_time_element.text.strip().split("\n") if arrive_time_element else list()
+            depart_airport_element = get_sub_element(
                 element=element, locator="xpath", regx=depart_airport_regx, interval=1, loop=3
-            ).text.strip()
-            arrive_airport = get_sub_element(
+            )
+            depart_airport = depart_airport_element.text.strip() if depart_airport_element else ""
+            arrive_airport_element = get_sub_element(
                 element=element, locator="xpath", regx=arrive_airport_regx, interval=1, loop=3
-            ).text.strip()
+            )
+            arrive_airport = arrive_airport_element.text.strip() if arrive_airport_element else ""
             # 逐行添加数据
             new_row = dict(
                 index=index, airline=airline, plane_no=plane_no, plane_type=plane_type,
-                arrive_time=arrive_time_slice[0], cross_days=arrive_time_slice[1] if len(arrive_time_slice) > 1 else "",
+                arrive_time=arrive_time_slice[0] if len(arrive_time_slice) > 0 else "",
+                cross_days=arrive_time_slice[1] if len(arrive_time_slice) > 1 else "",
                 depart_time=depart_time, price=Decimal(price[1:]), price_uint=price[:1], depart_airport=depart_airport,
                 arrive_airport=arrive_airport
             )
             # 添加新行数据
             df.loc[len(df)] = new_row
         return df
```

### Comparing `web-ui-helper-0.0.4/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-0.0.5/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper/terminal/device.py` & `web-ui-helper-0.0.5/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.4/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-0.0.5/web_ui_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.0.4/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-0.0.5/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

