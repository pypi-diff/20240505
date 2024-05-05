# Comparing `tmp/web-ui-helper-0.0.1.tar.gz` & `tmp/web-ui-helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-0.0.1.tar", last modified: Sun May  5 15:11:16 2024, max compression
+gzip compressed data, was "web-ui-helper-0.0.2.tar", last modified: Sun May  5 15:42:38 2024, max compression
```

## Comparing `web-ui-helper-0.0.1.tar` & `web-ui-helper-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:16.638958 web-ui-helper-0.0.1/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      715 2024-05-05 15:11:16.636962 web-ui-helper-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 15:11:16.638958 web-ui-helper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1297 2024-05-05 15:10:54.000000 web-ui-helper-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:16.342572 web-ui-helper-0.0.1/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.0.1/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:16.366483 web-ui-helper-0.0.1/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.0.1/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:16.373465 web-ui-helper-0.0.1/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-05 14:29:04.000000 web-ui-helper-0.0.1/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:16.375489 web-ui-helper-0.0.1/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.0.1/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:16.379482 web-ui-helper-0.0.1/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.0.1/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    27135 2024-05-05 14:29:36.000000 web-ui-helper-0.0.1/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:16.384437 web-ui-helper-0.0.1/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.0.1/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0     4728 2024-05-05 14:31:59.000000 web-ui-helper-0.0.1/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:16.388429 web-ui-helper-0.0.1/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     1615 2024-05-05 14:07:18.000000 web-ui-helper-0.0.1/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:16.632946 web-ui-helper-0.0.1/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.0.1/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:16.635939 web-ui-helper-0.0.1/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      715 2024-05-05 15:11:16.000000 web-ui-helper-0.0.1/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      936 2024-05-05 15:11:16.000000 web-ui-helper-0.0.1/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 15:11:16.000000 web-ui-helper-0.0.1/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2024-05-05 15:11:16.000000 web-ui-helper-0.0.1/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-05 15:11:16.000000 web-ui-helper-0.0.1/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:38.617895 web-ui-helper-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      715 2024-05-05 15:42:38.616910 web-ui-helper-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:42:38.617895 web-ui-helper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2024-05-05 15:41:59.000000 web-ui-helper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:38.564023 web-ui-helper-0.0.2/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-0.0.2/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:38.587961 web-ui-helper-0.0.2/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-0.0.2/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:38.592948 web-ui-helper-0.0.2/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-05 14:29:04.000000 web-ui-helper-0.0.2/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:38.594946 web-ui-helper-0.0.2/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-0.0.2/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:38.598950 web-ui-helper-0.0.2/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-0.0.2/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    27064 2024-05-05 15:41:22.000000 web-ui-helper-0.0.2/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:38.602923 web-ui-helper-0.0.2/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-0.0.2/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0     4728 2024-05-05 14:31:59.000000 web-ui-helper-0.0.2/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:38.607934 web-ui-helper-0.0.2/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     1615 2024-05-05 14:07:18.000000 web-ui-helper-0.0.2/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:38.611899 web-ui-helper-0.0.2/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-0.0.2/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:42:38.614890 web-ui-helper-0.0.2/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      715 2024-05-05 15:42:38.000000 web-ui-helper-0.0.2/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2024-05-05 15:42:38.000000 web-ui-helper-0.0.2/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:42:38.000000 web-ui-helper-0.0.2/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-05 15:42:38.000000 web-ui-helper-0.0.2/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-05 15:42:38.000000 web-ui-helper-0.0.2/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-0.0.1/LICENSE` & `web-ui-helper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/PKG-INFO` & `web-ui-helper-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.0.1/setup.py` & `web-ui-helper-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='0.0.1',
+    version='0.0.2',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-0.0.1/web_ui_helper/common/date_extend.py` & `web-ui-helper-0.0.2/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper/common/dir.py` & `web-ui-helper-0.0.2/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper/common/log.py` & `web-ui-helper-0.0.2/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper/common/metaclass.py` & `web-ui-helper-0.0.2/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper/common/platforms.py` & `web-ui-helper-0.0.2/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper/common/webdriver.py` & `web-ui-helper-0.0.2/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-0.0.2/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-0.0.2/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-0.0.2/web_ui_helper/selenium/frame/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,137 +257,136 @@
                                                 proxy_address=proxy_address)
             if self.browser_proxy.is_running() is True:
                 raise ValueError("Firefox browser is already running.")
             self.browser, self.wait, self.browser_name = self.browser_proxy.get_browser()
         else:
             raise ValueError("Browser name must be Chrome or Firefox.")
 
-    def input_text(self, selector: str, regx: str, value: str) -> bool:
+    def input_text(self, locator: str, regx: str, value: str) -> bool:
         """
-        selector 选择器
+        locator 选择器
         regx 选择器所要匹配的表达式
         value 文本框输入值
         """
         flag = False
         try:
             input_1 = self.wait.until(
-                ec.presence_of_element_located((Locator.get(selector), regx))
+                ec.presence_of_element_located((Locator.get(locator), regx))
             )
             # 模拟键盘操作清空输入框内容
             input_1.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
             input_1.send_keys(Keys.BACKSPACE)  # 删除选中的内容
             # 判断输入框是否有数据
             # if input_1.get_attribute("value"):
             # 清除存在的值
             # input_1.clear()
             # 使用 JavaScript 清除输入框的内容
             # self.browser.execute_script("arguments[0].setAttribute('value', '')", input_1)
             input_1.send_keys('{}'.format(value))
             flag = True
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，捕获输入框设置文本<{}>失败，error：{}".format(selector, regx, value, e)
+            err_str = "通过选择器：{}，表达式: {}，捕获输入框设置文本<{}>失败，error：{}".format(locator, regx, value, e)
             logger.error(err_str)
         return flag
 
-    def submit_click(self, selector: str, regx: str) -> bool:
+    def submit_click(self, locator: str, regx: str) -> bool:
         """
-        selector 选择器
+        locator 选择器
         regx 选择器所要匹配的表达式
         value 文本框输入值
         """
         flag = False
         try:
             submit = self.wait.until(
-                ec.element_to_be_clickable((Locator.get(selector), regx))
+                ec.element_to_be_clickable((Locator.get(locator), regx))
             )
             submit.click()
             flag = True
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，捕获点击对象并点击失败，error：{}".format(selector, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，捕获点击对象并点击失败，error：{}".format(locator, regx, e)
             logger.error(err_str)
         return flag
 
-    def get_code(self, selector: str, regx: str) -> str:
+    def get_code(self, locator: str, regx: str) -> str:
         logger.warning("开始获取验证码...")
         ocr_result = None
         try:
-            selector = Locator.get(selector)
-            captcha = self.browser.find_element(Locator.get(selector), regx)
+            captcha = self.browser.find_element(Locator.get(locator), regx)
             code_image = Image.open(BytesIO(captcha.screenshot_as_png))
             # 1.初始化一个实例，配置识别模式默认为OCR识别
             ocr = ddddocr.DdddOcr(show_ad=False)
             ocr_result = ocr.classification(code_image)
             logger.warning("识别到的验证码为：", ocr_result)
             return ocr_result
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，识别验证码失败，error：{}".format(selector, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，识别验证码失败，error：{}".format(locator, regx, e)
             logger.error(err_str)
         return ocr_result
 
     def alert_accept(self) -> bool:
         # 等待弹框出现
         try:
             alert = self.wait.until(ec.alert_is_present())
             logger.warning("弹框已出现")
             # 处理弹框，点击确定按钮
             alert.accept()
         except (Exception,):
             logger.warning("未出现弹框，无需处理。")
         return True
 
-    def get_element_text(self, selector: str, regx: str) -> str:
+    def get_element_text(self, locator: str, regx: str) -> str:
         element_text = None
         try:
             # 根据实际情况定位按钮元素
-            element = self.browser.find_element(Locator.get(selector), regx)
+            element = self.browser.find_element(Locator.get(locator), regx)
             # 获取按钮元素的文本信息
             element_text = element.text.strip() if isinstance(element.text, str) else ""
             logger.warning("获取元素的文字信息为: {}".format(element_text))
             return element_text
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，获取元素文本信息失败，error：{}".format(selector, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，获取元素文本信息失败，error：{}".format(locator, regx, e)
             logger.error(err_str)
         return element_text
 
-    def get_element(self, selector: str, regx: str) -> WebElement:
+    def get_element(self, locator: str, regx: str) -> WebElement:
         element = None
         try:
             # 根据实际情况定位按钮元素
-            element = self.browser.find_element(Locator.get(selector), regx)
+            element = self.browser.find_element(Locator.get(locator), regx)
         except (NoSuchElementException,):
-            err_str = "通过选择器：{}，表达式: {}，没有找到对应的元素".format(selector, regx)
+            err_str = "通过选择器：{}，表达式: {}，没有找到对应的元素".format(locator, regx)
             logger.warning(err_str)
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，获取元素失败，error：{}".format(selector, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，获取元素失败，error：{}".format(locator, regx, e)
             logger.error(err_str)
         return element
 
-    def get_elements(self, selector: str, regx: str) -> [WebElement]:
+    def get_elements(self, locator: str, regx: str) -> [WebElement]:
         elements = list()
         try:
             # 根据实际情况定位按钮元素
-            elements = self.browser.find_elements(Locator.get(selector), regx)
+            elements = self.browser.find_elements(Locator.get(locator), regx)
         except (NoSuchElementException,):
-            err_str = "通过选择器：{}，表达式: {}，没有找到对应的元素".format(selector, regx)
+            err_str = "通过选择器：{}，表达式: {}，没有找到对应的元素".format(locator, regx)
             logger.warning(err_str)
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，获取元素失败，error：{}".format(selector, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，获取元素失败，error：{}".format(locator, regx, e)
             logger.error(err_str)
         return elements
 
-    def get_background_color(self, selector: str, regx: str) -> str:
+    def get_background_color(self, locator: str, regx: str) -> str:
         background_color = None
         try:
             # 根据实际情况定位按钮元素
-            element = self.browser.find_element(Locator.get(selector), regx)
+            element = self.browser.find_element(Locator.get(locator), regx)
             # 获取选项的背景颜色
             background_color = element.value_of_css_property("background-color")
             background_color = background_color.strip() if isinstance(background_color, str) else ""
         except Exception as e:
-            err_str = "通过选择器：{}，表达式: {}，获取背景颜色失败，error：{}".format(selector, regx, e)
+            err_str = "通过选择器：{}，表达式: {}，获取背景颜色失败，error：{}".format(locator, regx, e)
             logger.error(err_str)
         return background_color
 
     def quit(self) -> None:
         self.browser.quit()
 
     def get(self, url: str) -> None:
```

### Comparing `web-ui-helper-0.0.1/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-0.0.2/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-0.0.2/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper/terminal/device.py` & `web-ui-helper-0.0.2/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-0.0.1/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-0.0.2/web_ui_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-0.0.1/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-0.0.2/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

