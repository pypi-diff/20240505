# Comparing `tmp/seldom-3.6.0.tar.gz` & `tmp/seldom-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldom-3.6.0.tar", max compression
+gzip compressed data, was "seldom-3.7.0.tar", max compression
```

## Comparing `seldom-3.6.0.tar` & `seldom-3.7.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0    11565 2022-12-06 15:57:51.673402 seldom-3.6.0/LICENSE
--rw-r--r--   0        0        0     1500 2024-03-04 14:52:00.827511 seldom-3.6.0/pyproject.toml
--rw-r--r--   0        0        0     9490 2024-03-03 16:13:38.480238 seldom-3.6.0/README.md
--rw-r--r--   0        0        0     1307 2024-03-04 14:51:47.449089 seldom-3.6.0/seldom/__init__.py
--rw-r--r--   0        0        0     6413 2023-12-13 16:52:02.087773 seldom-3.6.0/seldom/appdriver.py
--rw-r--r--   0        0        0     1669 2022-12-06 15:57:51.730115 seldom-3.6.0/seldom/appium_lab/__init__.py
--rw-r--r--   0        0        0     3909 2023-03-13 16:12:23.693178 seldom-3.6.0/seldom/appium_lab/action.py
--rw-r--r--   0        0        0     7248 2023-12-13 00:18:29.166651 seldom-3.6.0/seldom/appium_lab/find.py
--rw-r--r--   0        0        0     3122 2023-12-20 00:17:05.579680 seldom-3.6.0/seldom/appium_lab/keyboard.py
--rw-r--r--   0        0        0      424 2023-12-25 15:36:49.142129 seldom-3.6.0/seldom/appium_lab/ocr_plugin.py
--rw-r--r--   0        0        0     1961 2023-12-25 15:34:24.464069 seldom-3.6.0/seldom/appium_lab/switch.py
--rw-r--r--   0        0        0    11736 2023-12-25 15:41:48.053185 seldom-3.6.0/seldom/case.py
--rw-r--r--   0        0        0    12379 2024-02-21 14:54:07.472569 seldom-3.6.0/seldom/cli.py
--rw-r--r--   0        0        0       64 2022-12-06 15:57:51.734123 seldom-3.6.0/seldom/db_operation/__init__.py
--rw-r--r--   0        0        0     1698 2022-12-06 15:57:51.734123 seldom-3.6.0/seldom/db_operation/base_db.py
--rw-r--r--   0        0        0      715 2022-12-06 15:57:51.734123 seldom-3.6.0/seldom/db_operation/mongo_db.py
--rw-r--r--   0        0        0     4084 2023-05-04 15:57:05.737940 seldom-3.6.0/seldom/db_operation/mssql_db.py
--rw-r--r--   0        0        0     4329 2023-05-04 15:55:58.648089 seldom-3.6.0/seldom/db_operation/mysql_db.py
--rw-r--r--   0        0        0     3773 2023-11-28 15:46:07.408523 seldom-3.6.0/seldom/db_operation/postgres_db.py
--rw-r--r--   0        0        0     3206 2023-05-04 15:54:53.581476 seldom-3.6.0/seldom/db_operation/sqlite_db.py
--rw-r--r--   0        0        0     4004 2023-10-12 16:17:04.295880 seldom-3.6.0/seldom/driver.py
--rw-r--r--   0        0        0      271 2024-01-04 17:28:13.391020 seldom-3.6.0/seldom/extend_lib/__init__.py
--rw-r--r--   0        0        0     1179 2023-10-18 16:11:35.953126 seldom-3.6.0/seldom/extend_lib/curlify.py
--rw-r--r--   0        0        0    10519 2023-10-18 16:11:35.948109 seldom-3.6.0/seldom/extend_lib/jsonpath.py
--rw-r--r--   0        0        0    26889 2023-10-18 16:11:35.942112 seldom-3.6.0/seldom/extend_lib/parameterized.py
--rw-r--r--   0        0        0     1607 2023-10-18 16:15:40.944034 seldom-3.6.0/seldom/extend_lib/tomorrow.py
--rw-r--r--   0        0        0        0 2022-12-06 15:57:51.737139 seldom-3.6.0/seldom/har2case/__init__.py
--rw-r--r--   0        0        0     4014 2023-10-18 15:53:26.993547 seldom-3.6.0/seldom/har2case/core.py
--rw-r--r--   0        0        0     3948 2022-12-06 15:57:51.738139 seldom-3.6.0/seldom/har2case/demo.har
--rw-r--r--   0        0        0     1171 2022-12-06 15:57:51.738139 seldom-3.6.0/seldom/har2case/utils.py
--rw-r--r--   0        0        0       48 2022-12-06 15:57:51.739133 seldom-3.6.0/seldom/logging/__init__.py
--rw-r--r--   0        0        0     1201 2024-02-03 10:35:36.064307 seldom-3.6.0/seldom/logging/exceptions.py
--rw-r--r--   0        0        0     2018 2023-07-16 13:48:12.015173 seldom-3.6.0/seldom/logging/log.py
--rw-r--r--   0        0        0    13534 2024-03-04 14:29:21.584809 seldom-3.6.0/seldom/request.py
--rw-r--r--   0        0        0      803 2022-12-06 15:57:51.741121 seldom-3.6.0/seldom/running/__init__.py
--rw-r--r--   0        0        0      730 2023-12-25 15:40:39.273267 seldom-3.6.0/seldom/running/config.py
--rw-r--r--   0        0        0     2477 2023-08-31 14:22:17.854138 seldom-3.6.0/seldom/running/DebugTestRunner.py
--rw-r--r--   0        0        0     7450 2022-12-15 14:14:22.344315 seldom-3.6.0/seldom/running/loader_extend.py
--rw-r--r--   0        0        0     1038 2023-07-16 13:48:12.018172 seldom-3.6.0/seldom/running/loader_hook.py
--rw-r--r--   0        0        0    15467 2024-02-03 10:35:36.066296 seldom-3.6.0/seldom/running/runner.py
--rw-r--r--   0        0        0     3119 2023-10-12 15:27:54.643152 seldom-3.6.0/seldom/skip.py
--rw-r--r--   0        0        0        0 2024-01-29 16:24:55.055502 seldom-3.6.0/seldom/swagger2case/__init__.py
--rw-r--r--   0        0        0     5280 2024-02-21 14:57:41.944522 seldom-3.6.0/seldom/swagger2case/core.py
--rw-r--r--   0        0        0    36088 2024-01-29 16:24:55.056506 seldom-3.6.0/seldom/swagger2case/swagger.json
--rw-r--r--   0        0        0       28 2022-12-06 15:57:51.743682 seldom-3.6.0/seldom/testdata/__init__.py
--rw-r--r--   0        0        0     4164 2023-03-13 16:12:23.702178 seldom-3.6.0/seldom/testdata/conversion.py
--rw-r--r--   0        0        0    11028 2023-09-02 12:21:04.397189 seldom-3.6.0/seldom/testdata/parameterization.py
--rw-r--r--   0        0        0    18847 2022-12-06 15:57:51.745728 seldom-3.6.0/seldom/testdata/random_data.py
--rw-r--r--   0        0        0    12547 2023-09-19 15:35:38.286847 seldom-3.6.0/seldom/testdata/random_func.py
--rw-r--r--   0        0        0      266 2024-01-04 17:28:24.650425 seldom-3.6.0/seldom/utils/__init__.py
--rw-r--r--   0        0        0     5599 2023-10-30 16:48:04.895557 seldom-3.6.0/seldom/utils/cache.py
--rw-r--r--   0        0        0        2 2022-12-06 15:57:51.747723 seldom-3.6.0/seldom/utils/cache_data.json
--rw-r--r--   0        0        0     1556 2023-10-31 03:43:29.067437 seldom-3.6.0/seldom/utils/dependence.py
--rw-r--r--   0        0        0     2817 2023-11-15 15:05:08.550897 seldom-3.6.0/seldom/utils/diff.py
--rw-r--r--   0        0        0     3280 2022-12-06 15:57:51.748714 seldom-3.6.0/seldom/utils/file_extend.py
--rw-r--r--   0        0        0      438 2022-12-06 15:57:51.748714 seldom-3.6.0/seldom/utils/genson.py
--rw-r--r--   0        0        0      243 2022-12-06 15:57:51.749711 seldom-3.6.0/seldom/utils/jmespath.py
--rw-r--r--   0        0        0     1500 2023-03-13 16:12:23.708177 seldom-3.6.0/seldom/utils/send_extend.py
--rw-r--r--   0        0        0     3967 2023-10-26 15:02:35.253349 seldom-3.6.0/seldom/utils/so_and_so.py
--rw-r--r--   0        0        0     1577 2022-12-06 15:57:51.750730 seldom-3.6.0/seldom/utils/thread_lab.py
--rw-r--r--   0        0        0      401 2024-01-04 17:29:14.316525 seldom-3.6.0/seldom/utils/timer.py
--rw-r--r--   0        0        0    33490 2023-11-22 16:26:34.550796 seldom-3.6.0/seldom/webdriver.py
--rw-r--r--   0        0        0    10364 2023-10-31 02:40:43.274505 seldom-3.6.0/seldom/webdriver_chaining.py
--rw-r--r--   0        0        0    11064 1970-01-01 00:00:00.000000 seldom-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11565 2022-12-06 15:57:51.673402 seldom-3.7.0/LICENSE
+-rw-r--r--   0        0        0     1483 2024-05-05 16:38:56.203308 seldom-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0     9999 2024-04-15 11:20:45.995202 seldom-3.7.0/README.md
+-rw-r--r--   0        0        0     1305 2024-05-05 16:38:33.826783 seldom-3.7.0/seldom/__init__.py
+-rw-r--r--   0        0        0     6413 2023-12-13 16:52:02.087773 seldom-3.7.0/seldom/appdriver.py
+-rw-r--r--   0        0        0     1669 2022-12-06 15:57:51.730115 seldom-3.7.0/seldom/appium_lab/__init__.py
+-rw-r--r--   0        0        0     3909 2023-03-13 16:12:23.693178 seldom-3.7.0/seldom/appium_lab/action.py
+-rw-r--r--   0        0        0     7248 2023-12-13 00:18:29.166651 seldom-3.7.0/seldom/appium_lab/find.py
+-rw-r--r--   0        0        0     3122 2023-12-20 00:17:05.579680 seldom-3.7.0/seldom/appium_lab/keyboard.py
+-rw-r--r--   0        0        0      424 2023-12-25 15:36:49.142129 seldom-3.7.0/seldom/appium_lab/ocr_plugin.py
+-rw-r--r--   0        0        0     1961 2023-12-25 15:34:24.464069 seldom-3.7.0/seldom/appium_lab/switch.py
+-rw-r--r--   0        0        0    11736 2023-12-25 15:41:48.053185 seldom-3.7.0/seldom/case.py
+-rw-r--r--   0        0        0    12379 2024-02-21 14:54:07.472569 seldom-3.7.0/seldom/cli.py
+-rw-r--r--   0        0        0       64 2022-12-06 15:57:51.734123 seldom-3.7.0/seldom/db_operation/__init__.py
+-rw-r--r--   0        0        0     1698 2022-12-06 15:57:51.734123 seldom-3.7.0/seldom/db_operation/base_db.py
+-rw-r--r--   0        0        0      715 2022-12-06 15:57:51.734123 seldom-3.7.0/seldom/db_operation/mongo_db.py
+-rw-r--r--   0        0        0     4084 2023-05-04 15:57:05.737940 seldom-3.7.0/seldom/db_operation/mssql_db.py
+-rw-r--r--   0        0        0     4329 2023-05-04 15:55:58.648089 seldom-3.7.0/seldom/db_operation/mysql_db.py
+-rw-r--r--   0        0        0     3773 2023-11-28 15:46:07.408523 seldom-3.7.0/seldom/db_operation/postgres_db.py
+-rw-r--r--   0        0        0     3206 2023-05-04 15:54:53.581476 seldom-3.7.0/seldom/db_operation/sqlite_db.py
+-rw-r--r--   0        0        0     4348 2024-05-05 15:56:27.392733 seldom-3.7.0/seldom/driver.py
+-rw-r--r--   0        0        0      271 2024-01-04 17:28:13.391020 seldom-3.7.0/seldom/extend_lib/__init__.py
+-rw-r--r--   0        0        0     1179 2023-10-18 16:11:35.953126 seldom-3.7.0/seldom/extend_lib/curlify.py
+-rw-r--r--   0        0        0    10519 2023-10-18 16:11:35.948109 seldom-3.7.0/seldom/extend_lib/jsonpath.py
+-rw-r--r--   0        0        0    26889 2023-10-18 16:11:35.942112 seldom-3.7.0/seldom/extend_lib/parameterized.py
+-rw-r--r--   0        0        0     1607 2023-10-18 16:15:40.944034 seldom-3.7.0/seldom/extend_lib/tomorrow.py
+-rw-r--r--   0        0        0        0 2022-12-06 15:57:51.737139 seldom-3.7.0/seldom/har2case/__init__.py
+-rw-r--r--   0        0        0     4014 2023-10-18 15:53:26.993547 seldom-3.7.0/seldom/har2case/core.py
+-rw-r--r--   0        0        0     3948 2022-12-06 15:57:51.738139 seldom-3.7.0/seldom/har2case/demo.har
+-rw-r--r--   0        0        0     1171 2022-12-06 15:57:51.738139 seldom-3.7.0/seldom/har2case/utils.py
+-rw-r--r--   0        0        0       48 2022-12-06 15:57:51.739133 seldom-3.7.0/seldom/logging/__init__.py
+-rw-r--r--   0        0        0     1201 2024-02-03 10:35:36.064307 seldom-3.7.0/seldom/logging/exceptions.py
+-rw-r--r--   0        0        0     2018 2023-07-16 13:48:12.015173 seldom-3.7.0/seldom/logging/log.py
+-rw-r--r--   0        0        0    13534 2024-03-04 14:29:21.584809 seldom-3.7.0/seldom/request.py
+-rw-r--r--   0        0        0      803 2022-12-06 15:57:51.741121 seldom-3.7.0/seldom/running/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-05 15:30:00.257749 seldom-3.7.0/seldom/running/config.py
+-rw-r--r--   0        0        0     2477 2023-08-31 14:22:17.854138 seldom-3.7.0/seldom/running/DebugTestRunner.py
+-rw-r--r--   0        0        0     7450 2022-12-15 14:14:22.344315 seldom-3.7.0/seldom/running/loader_extend.py
+-rw-r--r--   0        0        0     1038 2023-07-16 13:48:12.018172 seldom-3.7.0/seldom/running/loader_hook.py
+-rw-r--r--   0        0        0    15594 2024-05-05 15:40:42.575496 seldom-3.7.0/seldom/running/runner.py
+-rw-r--r--   0        0        0     3119 2023-10-12 15:27:54.643152 seldom-3.7.0/seldom/skip.py
+-rw-r--r--   0        0        0        0 2024-01-29 16:24:55.055502 seldom-3.7.0/seldom/swagger2case/__init__.py
+-rw-r--r--   0        0        0     5280 2024-02-21 14:57:41.944522 seldom-3.7.0/seldom/swagger2case/core.py
+-rw-r--r--   0        0        0    36088 2024-01-29 16:24:55.056506 seldom-3.7.0/seldom/swagger2case/swagger.json
+-rw-r--r--   0        0        0       28 2022-12-06 15:57:51.743682 seldom-3.7.0/seldom/testdata/__init__.py
+-rw-r--r--   0        0        0     4164 2024-04-11 13:52:00.191608 seldom-3.7.0/seldom/testdata/conversion.py
+-rw-r--r--   0        0        0    11342 2024-04-11 13:18:49.359610 seldom-3.7.0/seldom/testdata/parameterization.py
+-rw-r--r--   0        0        0    18847 2022-12-06 15:57:51.745728 seldom-3.7.0/seldom/testdata/random_data.py
+-rw-r--r--   0        0        0    12547 2023-09-19 15:35:38.286847 seldom-3.7.0/seldom/testdata/random_func.py
+-rw-r--r--   0        0        0      266 2024-01-04 17:28:24.650425 seldom-3.7.0/seldom/utils/__init__.py
+-rw-r--r--   0        0        0     5599 2024-04-11 13:51:55.088380 seldom-3.7.0/seldom/utils/cache.py
+-rw-r--r--   0        0        0        2 2022-12-06 15:57:51.747723 seldom-3.7.0/seldom/utils/cache_data.json
+-rw-r--r--   0        0        0     1556 2024-04-11 13:51:55.089380 seldom-3.7.0/seldom/utils/dependence.py
+-rw-r--r--   0        0        0     2817 2024-04-11 13:51:55.089380 seldom-3.7.0/seldom/utils/diff.py
+-rw-r--r--   0        0        0     3280 2022-12-06 15:57:51.748714 seldom-3.7.0/seldom/utils/file_extend.py
+-rw-r--r--   0        0        0      438 2022-12-06 15:57:51.748714 seldom-3.7.0/seldom/utils/genson.py
+-rw-r--r--   0        0        0      243 2022-12-06 15:57:51.749711 seldom-3.7.0/seldom/utils/jmespath.py
+-rw-r--r--   0        0        0     1500 2024-04-11 13:51:55.090367 seldom-3.7.0/seldom/utils/send_extend.py
+-rw-r--r--   0        0        0     3967 2023-10-26 15:02:35.253349 seldom-3.7.0/seldom/utils/so_and_so.py
+-rw-r--r--   0        0        0     1577 2022-12-06 15:57:51.750730 seldom-3.7.0/seldom/utils/thread_lab.py
+-rw-r--r--   0        0        0      401 2024-01-04 17:29:14.316525 seldom-3.7.0/seldom/utils/timer.py
+-rw-r--r--   0        0        0    34272 2024-04-13 15:25:54.214029 seldom-3.7.0/seldom/webdriver.py
+-rw-r--r--   0        0        0    10364 2023-10-31 02:40:43.274505 seldom-3.7.0/seldom/webdriver_chaining.py
+-rw-r--r--   0        0        0     2168 2024-04-11 13:32:22.825914 seldom-3.7.0/seldom/websocket_client.py
+-rw-r--r--   0        0        0    11502 1970-01-01 00:00:00.000000 seldom-3.7.0/PKG-INFO
```

### Comparing `seldom-3.6.0/LICENSE` & `seldom-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/pyproject.toml` & `seldom-3.7.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seldom"
-version = "3.6.0"
+version = "3.7.0"
 description = "Seldom automation testing framework based on unittest."
 authors = ["bugmaster <fnngj@126.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 homepage = "https://seldomqa.github.io"
 repository = "https://github.com/SeldomQA/seldom"
@@ -13,37 +13,37 @@
 keywords = ["sedom", "selenium", "appium", "requests"]
 
 classifiers = [
     'Intended Audience :: Developers',
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: Microsoft :: Windows',
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     'Topic :: Software Development :: Testing',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 Appium-Python-Client = "^3.1.0"
 XTestRunner = "^1.7.0"
 loguru = "~0.6.0"
 openpyxl = "^3.0.3"
 pyyaml = "^6.0"
 requests = "^2.22.0"
 jsonschema = "^4.10.0"
 jmespath = "^0.10.0"
 pymysql = "^1.0.0"
 genson = "~1.2.2"
 click = "^8.1.3"
 python-dateutil = "~2.8.2"
+websocket-client = "~1.7.0"
 
 [tool.poetry.scripts]
 seldom = "seldom.cli:main"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `seldom-3.6.0/README.md` & `seldom-3.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 - [x] 提供丰富的断言
 - [x] 提供强大的`数据驱动`
 - [x] 平台化支持
 
 ### Install
 
 ```shell
-pip install seldom==3.4.0
+pip install seldom==3.6.0
 ```
 
 If you want to keep up with the latest version, you can install with github repository url:
 
 ```shell
 > pip install -U git+https://github.com/SeldomQA/seldom.git@master
 ```
@@ -171,20 +171,22 @@
         self.assertTitle("seldom_百度搜索")
 
     def test_case_two(self):
         """method chaining """
         Steps(url="https://www.baidu.com").open().find("#kw").type("seldom").find("#su").click()
         self.assertTitle("seldom_百度搜索")
 
+
 if __name__ == '__main__':
     seldom.main(browser="chrome")
 ```
 
 __说明：__
-* `seldom.main()` 通过 `browser` 指定运行的浏览器。 
+
+* `seldom.main()` 通过 `browser` 指定运行的浏览器。
 
 ### HTTP 测试
 
 seldom 2.0 支持HTTP测试
 
 ```python
 import seldom
@@ -193,15 +195,15 @@
 class TestRequest(seldom.TestCase):
 
     def test_put_method(self):
         self.put('/put', data={'key': 'value'})
         self.assertStatusCode(200)
 
     def test_post_method(self):
-        self.post('/post', data={'key':'value'})
+        self.post('/post', data={'key': 'value'})
         self.assertStatusCode(200)
 
     def test_get_method(self):
         payload = {'key1': 'value1', 'key2': 'value2'}
         self.get("/get", params=payload)
         self.assertStatusCode(200)
 
@@ -212,80 +214,98 @@
 
 if __name__ == '__main__':
     seldom.main(base_url="http://httpbin.org")
 ```
 
 __说明：__
 
-* `seldom.main()` 通过 `base_url` 指定接口项目基本URL地址。 
+* `seldom.main()` 通过 `base_url` 指定接口项目基本URL地址。
 
 ### App 测试
 
 seldom 3.0 支持App测试
 
 ```python
-import seldom
 from appium.options.android import UiAutomator2Options
 
+import seldom
+from seldom.appium_lab.keyboard import KeyEvent
+
+
+class TestBingApp(seldom.TestCase):
+    """
+    Test Bing APP
+    """
 
-class TestApp(seldom.TestCase):
+    def start(self):
+        self.ke = KeyEvent(self.driver)
 
-    def test_bbs_search(self):
-        self.wait(10)
-        self.click(id_="com.meizu.flyme.flymebbs:id/nw")
-        self.type(id_="com.meizu.flyme.flymebbs:id/nw", text="flyme")
-        self.click(id_="com.meizu.flyme.flymebbs:id/o1")
+    def test_bing_search(self):
+        """
+        test bing bbs search
+        """
         self.sleep(2)
-        elems = self.get_elements(id_="com.meizu.flyme.flymebbs:id/a29")
-        for elem in elems:
-            self.assertIn("flyme", elem.text.lower())
+        self.click(id_="com.microsoft.bing:id/sa_hp_header_search_box")
+        self.type(id_="com.microsoft.bing:id/sapphire_search_header_input", text="seldom")
+        self.ke.press_key("ENTER")
+        self.sleep(1)
+        elem = self.get_element(xpath='//android.widget.TextView[@resource-id="count"]')
+        self.assertIn("个结果", elem.text.lower())
 
 
 if __name__ == '__main__':
     capabilities = {
-        "automationName": "UiAutomator2",
-        "platformName": "Android",
-        "appPackage": "com.meizu.flyme.flymebbs",
-        "appActivity": "com.meizu.myplus.ui.splash.SplashActivity",
-        "noReset": True,
+        'deviceName': 'ELS-AN00',
+        'automationName': 'UiAutomator2',
+        'platformName': 'Android',
+        'appPackage': 'com.microsoft.bing',
+        'appActivity': 'com.microsoft.sapphire.app.main.MainSapphireActivity',
+        'noReset': True,
     }
     options = UiAutomator2Options().load_capabilities(capabilities)
-    seldom.main(app_server="http://127.0.0.1:4723", app_info=options)
+    seldom.main(app_server="http://127.0.0.1:4723", app_info=options, debug=True)
 ```
+
 __说明：__
 
-* `seldom.main()` 通过 `app_info` 指定App信息； `app_server` 指定appium server 地址。 
+* `seldom.main()` 通过 `app_info` 指定App信息； `app_server` 指定appium server 地址。
 
 ### Run the test
 
 ```python
 import seldom
 
 seldom.main()  # 默认运行当前测试文件
 seldom.main(path="./")  # 当前目录下的所有测试文件
 seldom.main(path="./test_dir/")  # 指定目录下的所有测试文件
 seldom.main(path="./test_dir/test_sample.py")  # 指定目录下的测试文件
 ```
 
-
 ## 📖 Document
 
 [中文文档](https://seldomqa.github.io/)
 
-
 ### 项目实例
 
 基于seldom的web UI自动化项目：
 
 https://github.com/SeldomQA/seldom-web-testing
 
 基于seldom的接口自动化项目:
 
 https://github.com/defnngj/seldom-api-testing
 
+## 微信（WeChat）
+
+> 欢迎添加微信，交流和反馈问题。
+
+<div style="display: flex;justify-content: space-between;width: 100%">
+    <p><img alt="微信" src="wechat.jpg" style="width: 200px;height: 100%" ></p>
+</div>
+
 ### Star History
 
 ![Star History Chart](https://api.star-history.com/svg?repos=SeldomQA/seldom&type=Date)
 
 ### 感谢
 
 感谢从以下项目中得到思路和帮助。
```

### Comparing `seldom-3.6.0/seldom/__init__.py` & `seldom-3.7.0/seldom/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,13 +24,12 @@
 from .utils.send_extend import SMTP, DingTalk
 from .webdriver_chaining import Steps
 
 from .skip import *
 from .driver import *
 from .testdata.parameterization import *
 
-
 __author__ = "bugmaster"
 
-__version__ = "3.6.0"
+__version__ = "3.7.0"
 
 __description__ = "Seldom is an automation testing framework based on unittest."
```

### Comparing `seldom-3.6.0/seldom/appdriver.py` & `seldom-3.7.0/seldom/appdriver.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/appium_lab/__init__.py` & `seldom-3.7.0/seldom/appium_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/appium_lab/action.py` & `seldom-3.7.0/seldom/appium_lab/action.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/appium_lab/find.py` & `seldom-3.7.0/seldom/appium_lab/find.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/appium_lab/keyboard.py` & `seldom-3.7.0/seldom/appium_lab/keyboard.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/appium_lab/switch.py` & `seldom-3.7.0/seldom/appium_lab/switch.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/case.py` & `seldom-3.7.0/seldom/case.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/cli.py` & `seldom-3.7.0/seldom/cli.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/db_operation/base_db.py` & `seldom-3.7.0/seldom/db_operation/base_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/db_operation/mongo_db.py` & `seldom-3.7.0/seldom/db_operation/mongo_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/db_operation/mssql_db.py` & `seldom-3.7.0/seldom/db_operation/mssql_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/db_operation/mysql_db.py` & `seldom-3.7.0/seldom/db_operation/mysql_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/db_operation/postgres_db.py` & `seldom-3.7.0/seldom/db_operation/postgres_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/db_operation/sqlite_db.py` & `seldom-3.7.0/seldom/db_operation/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/extend_lib/curlify.py` & `seldom-3.7.0/seldom/extend_lib/curlify.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/extend_lib/jsonpath.py` & `seldom-3.7.0/seldom/extend_lib/jsonpath.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/extend_lib/parameterized.py` & `seldom-3.7.0/seldom/extend_lib/parameterized.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/extend_lib/tomorrow.py` & `seldom-3.7.0/seldom/extend_lib/tomorrow.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/har2case/core.py` & `seldom-3.7.0/seldom/har2case/core.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/har2case/demo.har` & `seldom-3.7.0/seldom/har2case/demo.har`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/har2case/utils.py` & `seldom-3.7.0/seldom/har2case/utils.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/logging/exceptions.py` & `seldom-3.7.0/seldom/logging/exceptions.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/logging/log.py` & `seldom-3.7.0/seldom/logging/log.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/request.py` & `seldom-3.7.0/seldom/request.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/running/__init__.py` & `seldom-3.7.0/seldom/running/__init__.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/running/config.py` & `seldom-3.7.0/seldom/running/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     REPORT_PATH = None
     REPORT_TITLE = "Seldom Test Report"
     LOG_PATH = None
 
     # driver config
     options = None
     command_executor = ""
-    executable_path = ""
+    executable_path = None
 
 
 def base_url():
     """return base url"""
     return Seldom.base_url
```

### Comparing `seldom-3.6.0/seldom/running/DebugTestRunner.py` & `seldom-3.7.0/seldom/running/DebugTestRunner.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/running/loader_extend.py` & `seldom-3.7.0/seldom/running/loader_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/running/loader_hook.py` & `seldom-3.7.0/seldom/running/loader_hook.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/running/runner.py` & `seldom-3.7.0/seldom/running/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 seldom main
 """
-import os
-import re
 import ast
-import json as sys_json
-import inspect
 import builtins
+import inspect
+import json as sys_json
+import os
+import re
 import unittest
 import webbrowser
 from typing import Dict, List, Any, Optional
 
 from XTestRunner import HTMLTestRunner
 from XTestRunner import XMLTestRunner
-from selenium.webdriver.remote.webdriver import WebDriver as SeleniumWebDriver
 from selenium.common.exceptions import InvalidSessionIdException
+from selenium.webdriver.remote.webdriver import WebDriver as SeleniumWebDriver
+
 from seldom.driver import Browser
 from seldom.logging import log
 from seldom.logging import log_cfg
 from seldom.logging.exceptions import SeldomException, RunParamError
 from seldom.running.DebugTestRunner import DebugTestRunner
 from seldom.running.config import Seldom, BrowserConfig
 from seldom.running.config import base_url as base_url_func
@@ -218,20 +219,21 @@
         If you set up a browser, open the browser
         """
         if self.browser is not None:
             if isinstance(self.browser, str):
                 BrowserConfig.NAME = self.browser
             elif isinstance(self.browser, dict):
                 BrowserConfig.NAME = self.browser.get("browser", None)
-                BrowserConfig.command_executor = self.browser.get("command_executor", "")
-                BrowserConfig.executable_path = self.browser.get("executable_path", "")
+                BrowserConfig.executable_path = self.browser.get("executable_path", None)
                 BrowserConfig.options = self.browser.get("options", None)
+                BrowserConfig.command_executor = self.browser.get("command_executor", "")
             else:
                 raise TypeError("browser type error, str or dict.")
-            Seldom.driver = Browser(BrowserConfig.NAME)
+            Seldom.driver = Browser(BrowserConfig.NAME, BrowserConfig.executable_path, BrowserConfig.options,
+                                    BrowserConfig.command_executor)
 
     @staticmethod
     def close_browser() -> None:
         """
         How to open the browser, close the browser
         """
         if isinstance(Seldom.driver, SeleniumWebDriver):
```

### Comparing `seldom-3.6.0/seldom/skip.py` & `seldom-3.7.0/seldom/skip.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/swagger2case/core.py` & `seldom-3.7.0/seldom/swagger2case/core.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/swagger2case/swagger.json` & `seldom-3.7.0/seldom/swagger2case/swagger.json`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/testdata/conversion.py` & `seldom-3.7.0/seldom/testdata/conversion.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/testdata/parameterization.py` & `seldom-3.7.0/seldom/testdata/parameterization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 test data driver function
 """
-import os
 import inspect as sys_inspect
+import itertools
+import os
 import warnings
 from functools import wraps
 
 import requests
+
+from seldom import Seldom
+from seldom.extend_lib import parameterized_class
+from seldom.extend_lib.parameterized import delete_patches_if_need
 from seldom.extend_lib.parameterized import inspect
 from seldom.extend_lib.parameterized import parameterized
-from seldom.extend_lib.parameterized import skip_on_empty_helper
-from seldom.extend_lib.parameterized import reapply_patches_if_need
-from seldom.extend_lib.parameterized import delete_patches_if_need
 from seldom.extend_lib.parameterized import parameterized_argument_value_pairs
+from seldom.extend_lib.parameterized import reapply_patches_if_need
 from seldom.extend_lib.parameterized import short_repr
+from seldom.extend_lib.parameterized import skip_on_empty_helper
 from seldom.extend_lib.parameterized import to_text
-from seldom.extend_lib import parameterized_class
-from seldom.testdata import conversion
-from seldom.logging.exceptions import FileTypeError
 from seldom.logging import log
+from seldom.logging.exceptions import FileTypeError
+from seldom.testdata import conversion
 from seldom.utils import jmespath as utils_jmespath
-from seldom import Seldom
-
 
 __all__ = [
     "file_data", "api_data", "data", "data_class"
 ]
 
 
 def _search_file_path(file_dir: str, file_name: str) -> str:
@@ -92,15 +93,16 @@
                 return ""
         else:
             file = file.replace("\\", "/")
             current_dir = os.path.join(file_dir, file)
             parent_dir = os.path.join(os.path.dirname(file_dir), file)
             parent_dir_dir = os.path.join(os.path.dirname(os.path.dirname(file_dir)), file)
             parent_dir_dir_dir = os.path.join(os.path.dirname(os.path.dirname(os.path.dirname(file_dir))), file)
-            parent_dir_dir_dir_dir = os.path.join(os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(file_dir)))), file)
+            parent_dir_dir_dir_dir = os.path.join(
+                os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(file_dir)))), file)
 
             if os.path.isfile(current_dir) is True:
                 file_path = current_dir
             elif os.path.isfile(parent_dir) is True:
                 file_path = parent_dir
             elif os.path.isfile(parent_dir_dir) is True:
                 file_path = parent_dir_dir
@@ -199,29 +201,32 @@
         return data(data_)
 
     if isinstance(resp, list) is False:
         raise TypeError(f"Error - {resp} is not list")
     return data(resp)
 
 
-def data(input, name_func=None, doc_func=None, skip_on_empty=False, **legacy):
+def data(input, name_func=None, doc_func=None, skip_on_empty=False, cartesian=False, **legacy):
     """ A "brute force" method of parameterizing test cases. Creates new
         test cases and injects them into the namespace that the wrapped
         function is being defined in. Useful for parameterizing tests in
         subclasses of 'UnitTest', where Nose test generators don't work.
 
         >> @data([("foo", 1, 2)])
         ... def test_add1(name, input, expected):
         ...     actual = add1(input)
         ...     assert_equal(actual, expected)
         ...
         >> locals()
         ... 'test_add1_foo_0': <function ...> ...
         >>
         """
+    if cartesian is True:
+        input = cartesian_product(input)
+
     input = conversion.check_data(input)
 
     if "testcase_func_name" in legacy:
         warnings.warn("testcase_func_name= is deprecated; use name_func=",
                       DeprecationWarning, stacklevel=2)
         if not name_func:
             name_func = legacy["testcase_func_name"]
@@ -296,22 +301,32 @@
     if func.__doc__ is None:
         return None
 
     all_args_with_values = parameterized_argument_value_pairs(func, p)
     first_args_with_values = [all_args_with_values[0]]
 
     # Assumes that the function passed is a bound method.
-    descs = ["%s=%s" %(n, short_repr(v)) for n, v in first_args_with_values]
+    descs = ["%s=%s" % (n, short_repr(v)) for n, v in first_args_with_values]
 
     # The documentation might be a multiline string, so split it
     # and just work with the first string, ignoring the period
     # at the end if there is one.
     first, nl, rest = func.__doc__.lstrip().partition("\n")
     suffix = ""
     if first.endswith("."):
         suffix = "."
         first = first[:-1]
-    args = "%s[%s]" %(len(first) and " " or "", ", ".join(descs))
+    args = "%s[%s]" % (len(first) and " " or "", ", ".join(descs))
     return "".join(
         to_text(x)
         for x in [first.rstrip(), args, suffix, nl, rest]
     )
+
+
+def cartesian_product(arr) -> list:
+    """
+    Cartesian product
+    :param arr: Two-dimensional list
+    return:
+    """
+    cp = list(itertools.product(*arr))
+    return cp
```

### Comparing `seldom-3.6.0/seldom/testdata/random_data.py` & `seldom-3.7.0/seldom/testdata/random_data.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/testdata/random_func.py` & `seldom-3.7.0/seldom/testdata/random_func.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/utils/cache.py` & `seldom-3.7.0/seldom/utils/cache.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/utils/dependence.py` & `seldom-3.7.0/seldom/utils/dependence.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/utils/diff.py` & `seldom-3.7.0/seldom/utils/diff.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/utils/file_extend.py` & `seldom-3.7.0/seldom/utils/file_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/utils/send_extend.py` & `seldom-3.7.0/seldom/utils/send_extend.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/utils/so_and_so.py` & `seldom-3.7.0/seldom/utils/so_and_so.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/utils/thread_lab.py` & `seldom-3.7.0/seldom/utils/thread_lab.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/seldom/webdriver.py` & `seldom-3.7.0/seldom/webdriver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """
 selenium WebDriver API
 """
+import base64
 import os
+import platform
 import time
-import base64
 import warnings
-import platform
+
+from appium.webdriver.common.appiumby import AppiumBy
 from selenium.webdriver import Chrome
-from selenium.webdriver.remote.webdriver import WebDriver as SeleniumWebDriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.chrome.service import Service
+from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.remote.webdriver import WebDriver as SeleniumWebDriver
 from selenium.webdriver.support.select import Select
-from selenium.webdriver.common.action_chains import ActionChains
-from appium.webdriver.common.appiumby import AppiumBy
+
 from seldom.logging import log
-from seldom.running.config import Seldom
 from seldom.logging.exceptions import NotFindElementError
+from seldom.running.config import Seldom
 from seldom.testdata import get_timestamp
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.chrome.service import Service
-
 
 __all__ = ["WebDriver", "WebElement"]
 
 LOCATOR_LIST = {
     'css': By.CSS_SELECTOR,
     'id_': By.ID,
     'name': By.NAME,
@@ -35,15 +36,14 @@
     'ios_uiautomation': AppiumBy.IOS_UIAUTOMATION,
     'ios_predicate': AppiumBy.IOS_PREDICATE,
     'ios_class_chain': AppiumBy.IOS_CLASS_CHAIN,
     'android_uiautomator': AppiumBy.ANDROID_UIAUTOMATOR,
     'android_viewtag': AppiumBy.ANDROID_VIEWTAG,
     'android_data_matcher': AppiumBy.ANDROID_DATA_MATCHER,
     'android_view_matcher': AppiumBy.ANDROID_VIEW_MATCHER,
-    'windows_uiautomation': AppiumBy.WINDOWS_UI_AUTOMATION,
     'accessibility_id': AppiumBy.ACCESSIBILITY_ID,
     'image': AppiumBy.IMAGE,
     'custom': AppiumBy.CUSTOM,
 }
 
 
 class WebElement:
@@ -138,75 +138,118 @@
 
         def __init__(self, index: int = 0, **kwargs) -> None:
             self.web_elem = WebElement(**kwargs)
             self.elem = self.web_elem.get_elements(index)
             self.web_elem.show_element(self.elem)
 
         def input(self, text=""):
+            """
+            input text
+            :param text:
+            :return:
+            """
             log.info(f"✅ {self.web_elem.info}, input '{text}'.")
             self.elem.send_keys(text)
             return self
 
         def enter(self):
+            """
+            enter.
+            :return:
+            """
             log.info(f"✅ {self.web_elem.info}, enter.")
             self.elem.send_keys(Keys.ENTER)
             return self
 
         def select_all(self):
+            """
+            select all.
+            :return:
+            """
             log.info(f"✅ {self.web_elem.info}, ctrl+a.")
             if platform.system().lower() == "darwin":
                 self.elem.send_keys(Keys.COMMAND, "a")
             else:
                 self.elem.send_keys(Keys.CONTROL, "a")
             return self
 
         def cut(self):
+            """
+            cut.
+            :return:
+            """
             log.info(f"✅ {self.web_elem.info}, ctrl+x.")
             if platform.system().lower() == "darwin":
                 self.elem.send_keys(Keys.COMMAND, "x")
             else:
                 self.elem.send_keys(Keys.CONTROL, "x")
             return self
 
         def copy(self):
+            """
+            copy.
+            :return:
+            """
             log.info(f"✅ {self.web_elem.info}, ctrl+c.")
             if platform.system().lower() == "darwin":
                 self.elem.send_keys(Keys.COMMAND, "c")
             else:
                 self.elem.send_keys(Keys.CONTROL, "c")
             return self
 
         def paste(self):
+            """
+            paste.
+            :return:
+            """
             log.info(f"✅ {self.web_elem.info}, ctrl+v.")
             if platform.system().lower() == "darwin":
                 self.elem.send_keys(Keys.COMMAND, "v")
             else:
                 self.elem.send_keys(Keys.CONTROL, "v")
             return self
 
         def backspace(self):
+            """
+            Backspace key.
+            :return:
+            """
             log.info(f"✅ {self.web_elem.info}, backspace.")
             self.elem.send_keys(Keys.BACKSPACE)
             return self
 
         def delete(self):
+            """
+            Delete key.
+            :return:
+            """
             log.info(f"✅ {self.web_elem.info}, delete.")
             self.elem.send_keys(Keys.DELETE)
             return self
 
         def tab(self):
+            """
+            Tab key.
+            """
             log.info(f"✅ {self.web_elem.info}, tab.")
             self.elem.send_keys(Keys.TAB)
 
         def space(self):
+            """
+            Space key.
+            :return:
+            """
             log.info(f"✅ {self.web_elem.info}, space.")
             self.elem.send_keys(Keys.SPACE)
             return self
 
     class Alert:
+        """
+        Alert operation.
+        """
 
         @property
         def text(self) -> str:
             """
             Gets the text of the Alert.
             """
             log.info(f"✅ alert text: {Seldom.driver.switch_to.alert.text}.")
```

### Comparing `seldom-3.6.0/seldom/webdriver_chaining.py` & `seldom-3.7.0/seldom/webdriver_chaining.py`

 * *Files identical despite different names*

### Comparing `seldom-3.6.0/PKG-INFO` & `seldom-3.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: seldom
-Version: 3.6.0
+Version: 3.7.0
 Summary: Seldom automation testing framework based on unittest.
 Home-page: https://seldomqa.github.io
 License: Apache-2.0
 Keywords: sedom,selenium,appium,requests
 Author: bugmaster
 Author-email: fnngj@126.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: Appium-Python-Client (>=3.1.0,<4.0.0)
 Requires-Dist: XTestRunner (>=1.7.0,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
@@ -34,14 +32,15 @@
 Requires-Dist: jsonschema (>=4.10.0,<5.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: openpyxl (>=3.0.3,<4.0.0)
 Requires-Dist: pymysql (>=1.0.0,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<2.9.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.22.0,<3.0.0)
+Requires-Dist: websocket-client (>=1.7.0,<1.8.0)
 Project-URL: Documentation, https://seldomqa.github.io
 Project-URL: Repository, https://github.com/SeldomQA/seldom
 Description-Content-Type: text/markdown
 
 [GitHub](https://github.com/SeldomQA/seldom) | [Gitee](https://gitee.com/fnngj/seldom) |
 
 ![](seldom_logo.jpg)
@@ -60,15 +59,15 @@
 - [x] 提供丰富的断言
 - [x] 提供强大的`数据驱动`
 - [x] 平台化支持
 
 ### Install
 
 ```shell
-pip install seldom==3.4.0
+pip install seldom==3.6.0
 ```
 
 If you want to keep up with the latest version, you can install with github repository url:
 
 ```shell
 > pip install -U git+https://github.com/SeldomQA/seldom.git@master
 ```
@@ -215,20 +214,22 @@
         self.assertTitle("seldom_百度搜索")
 
     def test_case_two(self):
         """method chaining """
         Steps(url="https://www.baidu.com").open().find("#kw").type("seldom").find("#su").click()
         self.assertTitle("seldom_百度搜索")
 
+
 if __name__ == '__main__':
     seldom.main(browser="chrome")
 ```
 
 __说明：__
-* `seldom.main()` 通过 `browser` 指定运行的浏览器。 
+
+* `seldom.main()` 通过 `browser` 指定运行的浏览器。
 
 ### HTTP 测试
 
 seldom 2.0 支持HTTP测试
 
 ```python
 import seldom
@@ -237,15 +238,15 @@
 class TestRequest(seldom.TestCase):
 
     def test_put_method(self):
         self.put('/put', data={'key': 'value'})
         self.assertStatusCode(200)
 
     def test_post_method(self):
-        self.post('/post', data={'key':'value'})
+        self.post('/post', data={'key': 'value'})
         self.assertStatusCode(200)
 
     def test_get_method(self):
         payload = {'key1': 'value1', 'key2': 'value2'}
         self.get("/get", params=payload)
         self.assertStatusCode(200)
 
@@ -256,80 +257,98 @@
 
 if __name__ == '__main__':
     seldom.main(base_url="http://httpbin.org")
 ```
 
 __说明：__
 
-* `seldom.main()` 通过 `base_url` 指定接口项目基本URL地址。 
+* `seldom.main()` 通过 `base_url` 指定接口项目基本URL地址。
 
 ### App 测试
 
 seldom 3.0 支持App测试
 
 ```python
-import seldom
 from appium.options.android import UiAutomator2Options
 
+import seldom
+from seldom.appium_lab.keyboard import KeyEvent
+
+
+class TestBingApp(seldom.TestCase):
+    """
+    Test Bing APP
+    """
 
-class TestApp(seldom.TestCase):
+    def start(self):
+        self.ke = KeyEvent(self.driver)
 
-    def test_bbs_search(self):
-        self.wait(10)
-        self.click(id_="com.meizu.flyme.flymebbs:id/nw")
-        self.type(id_="com.meizu.flyme.flymebbs:id/nw", text="flyme")
-        self.click(id_="com.meizu.flyme.flymebbs:id/o1")
+    def test_bing_search(self):
+        """
+        test bing bbs search
+        """
         self.sleep(2)
-        elems = self.get_elements(id_="com.meizu.flyme.flymebbs:id/a29")
-        for elem in elems:
-            self.assertIn("flyme", elem.text.lower())
+        self.click(id_="com.microsoft.bing:id/sa_hp_header_search_box")
+        self.type(id_="com.microsoft.bing:id/sapphire_search_header_input", text="seldom")
+        self.ke.press_key("ENTER")
+        self.sleep(1)
+        elem = self.get_element(xpath='//android.widget.TextView[@resource-id="count"]')
+        self.assertIn("个结果", elem.text.lower())
 
 
 if __name__ == '__main__':
     capabilities = {
-        "automationName": "UiAutomator2",
-        "platformName": "Android",
-        "appPackage": "com.meizu.flyme.flymebbs",
-        "appActivity": "com.meizu.myplus.ui.splash.SplashActivity",
-        "noReset": True,
+        'deviceName': 'ELS-AN00',
+        'automationName': 'UiAutomator2',
+        'platformName': 'Android',
+        'appPackage': 'com.microsoft.bing',
+        'appActivity': 'com.microsoft.sapphire.app.main.MainSapphireActivity',
+        'noReset': True,
     }
     options = UiAutomator2Options().load_capabilities(capabilities)
-    seldom.main(app_server="http://127.0.0.1:4723", app_info=options)
+    seldom.main(app_server="http://127.0.0.1:4723", app_info=options, debug=True)
 ```
+
 __说明：__
 
-* `seldom.main()` 通过 `app_info` 指定App信息； `app_server` 指定appium server 地址。 
+* `seldom.main()` 通过 `app_info` 指定App信息； `app_server` 指定appium server 地址。
 
 ### Run the test
 
 ```python
 import seldom
 
 seldom.main()  # 默认运行当前测试文件
 seldom.main(path="./")  # 当前目录下的所有测试文件
 seldom.main(path="./test_dir/")  # 指定目录下的所有测试文件
 seldom.main(path="./test_dir/test_sample.py")  # 指定目录下的测试文件
 ```
 
-
 ## 📖 Document
 
 [中文文档](https://seldomqa.github.io/)
 
-
 ### 项目实例
 
 基于seldom的web UI自动化项目：
 
 https://github.com/SeldomQA/seldom-web-testing
 
 基于seldom的接口自动化项目:
 
 https://github.com/defnngj/seldom-api-testing
 
+## 微信（WeChat）
+
+> 欢迎添加微信，交流和反馈问题。
+
+<div style="display: flex;justify-content: space-between;width: 100%">
+    <p><img alt="微信" src="wechat.jpg" style="width: 200px;height: 100%" ></p>
+</div>
+
 ### Star History
 
 ![Star History Chart](https://api.star-history.com/svg?repos=SeldomQA/seldom&type=Date)
 
 ### 感谢
 
 感谢从以下项目中得到思路和帮助。
```

