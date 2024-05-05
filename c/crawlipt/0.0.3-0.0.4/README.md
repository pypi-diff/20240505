# Comparing `tmp/crawlipt-0.0.3.tar.gz` & `tmp/crawlipt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlipt-0.0.3.tar", last modified: Fri Apr 26 06:38:04 2024, max compression
+gzip compressed data, was "crawlipt-0.0.4.tar", last modified: Sun May  5 08:52:18 2024, max compression
```

## Comparing `crawlipt-0.0.3.tar` & `crawlipt-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:04.193247 crawlipt-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-26 06:37:55.000000 crawlipt-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 06:37:55.000000 crawlipt-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-26 06:38:04.193247 crawlipt-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-26 06:37:55.000000 crawlipt-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:04.189247 crawlipt-0.0.3/crawlipt/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:04.193247 crawlipt-0.0.3/crawlipt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/input.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/slide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/actions/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-26 06:37:55.000000 crawlipt-0.0.3/crawlipt/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 06:38:04.193247 crawlipt-0.0.3/crawlipt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-26 06:38:04.000000 crawlipt-0.0.3/crawlipt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-26 06:38:04.000000 crawlipt-0.0.3/crawlipt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 06:38:04.000000 crawlipt-0.0.3/crawlipt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 06:38:04.000000 crawlipt-0.0.3/crawlipt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 06:38:04.000000 crawlipt-0.0.3/crawlipt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 06:38:04.193247 crawlipt-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-26 06:37:55.000000 crawlipt-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:52:18.430924 crawlipt-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-05 08:52:14.000000 crawlipt-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-05 08:52:14.000000 crawlipt-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-05 08:52:18.430924 crawlipt-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-05 08:52:14.000000 crawlipt-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:52:18.426924 crawlipt-0.0.4/crawlipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:52:18.430924 crawlipt-0.0.4/crawlipt/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/actions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:52:18.430924 crawlipt-0.0.4/crawlipt/conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/conditions/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-05-05 08:52:14.000000 crawlipt-0.0.4/crawlipt/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:52:18.430924 crawlipt-0.0.4/crawlipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-05 08:52:18.000000 crawlipt-0.0.4/crawlipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-05 08:52:18.000000 crawlipt-0.0.4/crawlipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:52:18.000000 crawlipt-0.0.4/crawlipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 08:52:18.000000 crawlipt-0.0.4/crawlipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 08:52:18.000000 crawlipt-0.0.4/crawlipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 08:52:18.430924 crawlipt-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-05 08:52:14.000000 crawlipt-0.0.4/setup.py
```

### Comparing `crawlipt-0.0.3/LICENSE` & `crawlipt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.3/PKG-INFO` & `crawlipt-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.3
+Version: 0.0.4
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -83,12 +83,13 @@
 # Execute script
 cpt.Script(script, interval=2)(webdriver)
 
 ```
 
 
 ## Documenting
-If you are interested and would like to see more detailed documentation, please click on the picture below.\
- <a href="https://wwydev.gitbook.io/crawlipt/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:287px; height:123px" ></a>
+If you are interested and would like to see more detailed documentation, please click on the link below.
+
+[中文](https://wwydev.gitbook.io/crawlipt-zh "中文文档")|[English](https://wwydev.gitbook.io/crawlipt "English Document")
 
 ## Contributing
 Please submit pull requests to the develop branch
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.3 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.4 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
@@ -23,9 +23,10 @@
 (agent) webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()),
 options=option) # Define scripts # You can also deserialize JSON strings into a
 dictionary script = { "method": "redirect", "url": "https://www.baidu.com/",
 "next": { "method": "input", "xpath": "//*[@id=\"kw\"]", "keyword":
 "åæ³é¾çº±", "next": { "method": "click", "xpath": "//*[@id=\"su\"]" } } } #
 Execute script cpt.Script(script, interval=2)(webdriver) ``` ## Documenting If
 you are interested and would like to see more detailed documentation, please
-click on the picture below.\ _[_c_r_a_w_l_i_s_t_]## Contributing Please submit pull
-requests to the develop branch
+click on the link below. [ä¸­æ](https://wwydev.gitbook.io/crawlipt-zh
+"ä¸­æææ¡£")|[English](https://wwydev.gitbook.io/crawlipt "English
+Document") ## Contributing Please submit pull requests to the develop branch
```

### Comparing `crawlipt-0.0.3/README.md` & `crawlipt-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,12 +63,13 @@
 # Execute script
 cpt.Script(script, interval=2)(webdriver)
 
 ```
 
 
 ## Documenting
-If you are interested and would like to see more detailed documentation, please click on the picture below.\
- <a href="https://wwydev.gitbook.io/crawlipt/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:287px; height:123px" ></a>
+If you are interested and would like to see more detailed documentation, please click on the link below.
+
+[中文](https://wwydev.gitbook.io/crawlipt-zh "中文文档")|[English](https://wwydev.gitbook.io/crawlipt "English Document")
 
 ## Contributing
 Please submit pull requests to the develop branch
```

#### html2text {}

```diff
@@ -14,9 +14,10 @@
 (agent) webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()),
 options=option) # Define scripts # You can also deserialize JSON strings into a
 dictionary script = { "method": "redirect", "url": "https://www.baidu.com/",
 "next": { "method": "input", "xpath": "//*[@id=\"kw\"]", "keyword":
 "åæ³é¾çº±", "next": { "method": "click", "xpath": "//*[@id=\"su\"]" } } } #
 Execute script cpt.Script(script, interval=2)(webdriver) ``` ## Documenting If
 you are interested and would like to see more detailed documentation, please
-click on the picture below.\ _[_c_r_a_w_l_i_s_t_]## Contributing Please submit pull
-requests to the develop branch
+click on the link below. [ä¸­æ](https://wwydev.gitbook.io/crawlipt-zh
+"ä¸­æææ¡£")|[English](https://wwydev.gitbook.io/crawlipt "English
+Document") ## Contributing Please submit pull requests to the develop branch
```

### Comparing `crawlipt-0.0.3/crawlipt/actions/click.py` & `crawlipt-0.0.4/crawlipt/actions/click.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import random
 import time
 
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 
-from crawlipt.annotation import check
+from crawlipt.annotation import check, alias
 
 
 class Click:
     @staticmethod
     @check(exclude="driver")
+    @alias("C")
     def click(driver: WebDriver, xpath: str) -> None:
         """
         Handling click events
         :param driver: selenium webdriver
         :param xpath: click on the xpath path of the button
         """
         element = driver.find_element(By.XPATH, xpath)
-        driver.execute_script("arguments[0].click();", element)
+        element.click()
 
     @staticmethod
     @check(exclude="driver")
     def clickMulti(driver: WebDriver, xpath: str, cnt: str | int, frequency: int = 0.1) -> None:
         """
         Handling click events multiple times
         :param driver: selenium webdriver
@@ -30,11 +31,21 @@
         :param frequency: click frequency of the button
         """
         if isinstance(cnt, str):
             cnt = int(cnt)
         element = driver.find_element(By.XPATH, xpath)
         while cnt:
             cnt -= 1
-            driver.execute_script("arguments[0].click();", element)
+            element.click()
             time.sleep(random.uniform(frequency/2, frequency))
 
+    @staticmethod
+    @check(exclude="driver")
+    def clickByJs(driver: WebDriver, xpath: str) -> None:
+        """
+        Handling click events by js 'arguments[0].click();'
+        :param driver: selenium webdriver
+        :param xpath: click on the xpath path of the button
+        """
+        element = driver.find_element(By.XPATH, xpath)
+        driver.execute_script("arguments[0].click();", element)
```

### Comparing `crawlipt-0.0.3/crawlipt/actions/get.py` & `crawlipt-0.0.4/crawlipt/actions/get.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.3/crawlipt/actions/input.py` & `crawlipt-0.0.4/crawlipt/actions/input.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from selenium.webdriver import Keys
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 
-from crawlipt.annotation import check
+from crawlipt.annotation import check, alias
 
 
 class Input:
     @staticmethod
     @check(exclude="driver")
+    @alias("I")
     def input(driver: WebDriver, xpath: str, text: str) -> None:
         """
         Handling keyboard input events
         :param driver: selenium webdriver
         :param xpath: The xpath path of the input box
         :param text: text needs to be passed in
         """
         element = driver.find_element(By.XPATH, xpath)
         element.send_keys(text)
 
     @staticmethod
     @check(exclude="driver")
+    @alias("E")
     def enter(driver: WebDriver, xpath: str) -> None:
         """
         Press the enter key once
         :param driver: selenium webdriver
         :param xpath: The xpath path of the input box
         :return: Whether successful
         """
```

### Comparing `crawlipt-0.0.3/crawlipt/actions/redirect.py` & `crawlipt-0.0.4/crawlipt/actions/redirect.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from selenium.webdriver.remote.webdriver import WebDriver
+from selenium.webdriver.support.wait import WebDriverWait
 
-from crawlipt.annotation import check
+from crawlipt.annotation import check, alias
 
 
 class Redirect:
     @staticmethod
     @check(exclude="driver")
     def searchRedirect(driver: WebDriver, url: str, keyword: str) -> None:
         """
@@ -14,14 +15,26 @@
         :param keyword: keyword needs to be passed in
         """
         url = url.replace(r"%s", keyword)
         driver.get(url)
 
     @staticmethod
     @check(exclude="driver")
+    @alias("R")
     def redirect(driver: WebDriver, url: str) -> None:
         """
         Direct redirection
         :param driver:  selenium webdriver
         :param url: Links that require redirection
         """
         driver.get(url)
+
+    @staticmethod
+    @check(exclude="driver")
+    def redirectNewTab(driver: WebDriver, url: str) -> None:
+        """
+        redirect to a new tab
+        :param driver:  selenium webdriver
+        :param url: Links that require redirection
+        """
+        js = f'window.open("{url}")'
+        driver.execute_script(js)
```

### Comparing `crawlipt-0.0.3/crawlipt/actions/select.py` & `crawlipt-0.0.4/crawlipt/actions/select.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.3/crawlipt/actions/slide.py` & `crawlipt-0.0.4/crawlipt/actions/slide.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.3/crawlipt/actions/switch.py` & `crawlipt-0.0.4/crawlipt/actions/switch.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         if isinstance(index, str):
             index = int(index)
         window_handles = driver.window_handles
         driver.switch_to.window(window_handles[index])
 
     @staticmethod
     @check(exclude="driver")
-    def switchToframe(driver: WebDriver, xpath: str) -> None:
+    def switchToFrame(driver: WebDriver, xpath: str) -> None:
         """
         Switch to the inner frame
         :param driver: selenium webdriver
         :param xpath: The xpath of frame
         """
         frame = driver.find_element(By.XPATH, xpath)
         driver.switch_to.frame(frame)
```

### Comparing `crawlipt-0.0.3/crawlipt/annotation.py` & `crawlipt-0.0.4/crawlipt/annotation.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,7 +61,32 @@
             return func(*args, **kwargs)
 
         return inner_wrapper
 
     if callable(exclude):
         return wrapper(exclude)
     return wrapper
+
+
+def alias(name: str = ""):
+    """
+    Add an alias to your newly added action or condition so that the script can resolve to this function through the alias
+    :param name: The name of func
+    :return: Decorator
+    """
+    if not callable(name):
+        assert isinstance(name, str)
+
+    def wrapper(func):
+        @wraps(func)
+        def inner_wrapper(*args, **kwargs):
+            if callable(name) or not name:
+                return func(*args, **kwargs)
+            func.__crawlipt_func_name__ = name
+            return func(*args, **kwargs)
+
+        inner_wrapper.__crawlipt_func_name__ = name
+        return inner_wrapper
+
+    if callable(name):
+        return wrapper(name)
+    return wrapper
```

### Comparing `crawlipt-0.0.3/crawlipt.egg-info/PKG-INFO` & `crawlipt-0.0.4/crawlipt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.3
+Version: 0.0.4
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -83,12 +83,13 @@
 # Execute script
 cpt.Script(script, interval=2)(webdriver)
 
 ```
 
 
 ## Documenting
-If you are interested and would like to see more detailed documentation, please click on the picture below.\
- <a href="https://wwydev.gitbook.io/crawlipt/"><img src="https://s2.loli.net/2024/04/12/5gOBimSY4oklGys.png" alt="crawlist" style="width:287px; height:123px" ></a>
+If you are interested and would like to see more detailed documentation, please click on the link below.
+
+[中文](https://wwydev.gitbook.io/crawlipt-zh "中文文档")|[English](https://wwydev.gitbook.io/crawlipt "English Document")
 
 ## Contributing
 Please submit pull requests to the develop branch
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.3 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.4 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
@@ -23,9 +23,10 @@
 (agent) webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()),
 options=option) # Define scripts # You can also deserialize JSON strings into a
 dictionary script = { "method": "redirect", "url": "https://www.baidu.com/",
 "next": { "method": "input", "xpath": "//*[@id=\"kw\"]", "keyword":
 "åæ³é¾çº±", "next": { "method": "click", "xpath": "//*[@id=\"su\"]" } } } #
 Execute script cpt.Script(script, interval=2)(webdriver) ``` ## Documenting If
 you are interested and would like to see more detailed documentation, please
-click on the picture below.\ _[_c_r_a_w_l_i_s_t_]## Contributing Please submit pull
-requests to the develop branch
+click on the link below. [ä¸­æ](https://wwydev.gitbook.io/crawlipt-zh
+"ä¸­æææ¡£")|[English](https://wwydev.gitbook.io/crawlipt "English
+Document") ## Contributing Please submit pull requests to the develop branch
```

### Comparing `crawlipt-0.0.3/setup.py` & `crawlipt-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlipt'
 DESCRIPTION = 'The script for selenium in python'
 URL = 'https://github.com/WwwwwyDev/crawlipt'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwwwwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "selenium>=4.0.0"
 ]
 
 # What packages are optional?
@@ -99,15 +99,15 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*", "test"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
```

