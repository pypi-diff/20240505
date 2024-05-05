# Comparing `tmp/pytest-pyreport-1.5.0.tar.gz` & `tmp/pytest_pyreport-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-pyreport-1.5.0.tar", last modified: Sat Feb  3 23:44:43 2024, max compression
+gzip compressed data, was "pytest_pyreport-1.6.0.tar", last modified: Sun May  5 19:59:58 2024, max compression
```

## Comparing `pytest-pyreport-1.5.0.tar` & `pytest_pyreport-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 23:44:43.359257 pytest-pyreport-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-03 23:44:33.000000 pytest-pyreport-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-02-03 23:44:43.359257 pytest-pyreport-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-02-03 23:44:33.000000 pytest-pyreport-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 23:44:43.359257 pytest-pyreport-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-02-03 23:44:33.000000 pytest-pyreport-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 23:44:43.355257 pytest-pyreport-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 23:44:43.359257 pytest-pyreport-1.5.0/src/pytest_pyreport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 23:44:33.000000 pytest-pyreport-1.5.0/src/pytest_pyreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-02-03 23:44:33.000000 pytest-pyreport-1.5.0/src/pytest_pyreport/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 23:44:43.359257 pytest-pyreport-1.5.0/src/pytest_pyreport/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9420 2024-02-03 23:44:33.000000 pytest-pyreport-1.5.0/src/pytest_pyreport/templates/template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 23:44:43.359257 pytest-pyreport-1.5.0/src/pytest_pyreport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-02-03 23:44:43.000000 pytest-pyreport-1.5.0/src/pytest_pyreport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-03 23:44:43.000000 pytest-pyreport-1.5.0/src/pytest_pyreport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 23:44:43.000000 pytest-pyreport-1.5.0/src/pytest_pyreport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-03 23:44:43.000000 pytest-pyreport-1.5.0/src/pytest_pyreport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-03 23:44:43.000000 pytest-pyreport-1.5.0/src/pytest_pyreport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-03 23:44:43.000000 pytest-pyreport-1.5.0/src/pytest_pyreport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:59:58.901582 pytest_pyreport-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 19:59:53.000000 pytest_pyreport-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-05-05 19:59:58.901582 pytest_pyreport-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-05 19:59:53.000000 pytest_pyreport-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 19:59:58.901582 pytest_pyreport-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-05 19:59:53.000000 pytest_pyreport-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:59:58.897582 pytest_pyreport-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:59:58.901582 pytest_pyreport-1.6.0/src/pytest_pyreport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 19:59:53.000000 pytest_pyreport-1.6.0/src/pytest_pyreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-05-05 19:59:53.000000 pytest_pyreport-1.6.0/src/pytest_pyreport/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:59:58.901582 pytest_pyreport-1.6.0/src/pytest_pyreport/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9420 2024-05-05 19:59:53.000000 pytest_pyreport-1.6.0/src/pytest_pyreport/templates/template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 19:59:58.901582 pytest_pyreport-1.6.0/src/pytest_pyreport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-05-05 19:59:58.000000 pytest_pyreport-1.6.0/src/pytest_pyreport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-05 19:59:58.000000 pytest_pyreport-1.6.0/src/pytest_pyreport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 19:59:58.000000 pytest_pyreport-1.6.0/src/pytest_pyreport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-05 19:59:58.000000 pytest_pyreport-1.6.0/src/pytest_pyreport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 19:59:58.000000 pytest_pyreport-1.6.0/src/pytest_pyreport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 19:59:58.000000 pytest_pyreport-1.6.0/src/pytest_pyreport.egg-info/top_level.txt
```

### Comparing `pytest-pyreport-1.5.0/LICENSE` & `pytest_pyreport-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-pyreport-1.5.0/PKG-INFO` & `pytest_pyreport-1.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-pyreport
-Version: 1.5.0
+Version: 1.6.0
 Summary: PyReport is a lightweight reporting plugin for Pytest that provides concise HTML report
 Home-page: https://github.com/ToghrulMirzayev/pytest-pyreport
 Author: Toghrul Mirzayev
 Author-email: togrul.mirzoev@gmail.com
 License: MIT
 Keywords: pytest_pyreport,python,pytest,report,slack,telegram,messenger,pyreport
 Classifier: Framework :: Pytest
@@ -51,39 +51,56 @@
 ```
 
 ## Report generation
 * Run tests using below command to generate pyreport.html file with test results:
     ```
     pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport
     ```
-
+---
 * Run tests using below command if you want to send Telegram notification <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/83/Telegram_2019_Logo.svg/512px-Telegram_2019_Logo.svg.png?20231105064641" alt="Telegram" width="30" height="30">
     ```
     pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport --telegram-pyreport <chat id> <bot token>
     ```
   * Prerequisites:
     * You need your own Telegram bot, which can be easily created using Telegram instructions.
   You can take the “chat ID” and “bot token” from there.
-
+---
 * Run tests using below command if you want to send Slack notification <img src="https://raw.githubusercontent.com/devicons/devicon/55609aa5bd817ff167afce0d965585c92040787a/icons/slack/slack-original.svg" alt="Slack" width="30" height="30">
     ```
     pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport --slack-pyreport <webhook url> <channel id> <bot token>
     ```
   * Prerequisites:
     * You need your own Slack bot, which can be easily created using Slack instructions.
   You can take the “webhook url”, "channel id" and “bot token” from there.
-
+---
 * Run tests using below command if you want to check generated report on the server if it is available:
   ```
   pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport --telegram-pyreport <chat id> <bot token> --server <URL>
   pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport --slack-pyreport <webhook url> <channel id> <bot token> --server <URL>
   ```
   * Prerequisites:
     * You need to run server beforehand. As an example using CI/CD tools like Jenkins or GitHub Actions
 
+---
+* Run tests with failed tests counter. By running below command you will get JSON file with percentage of failed tests:
+  ```
+   pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport --failed-tests-count
+  ```
+  * Fail percentage formula:
+  ```text
+  Failed Tests Percentage = (Number of Failed Tests / Total Number of Tests) * 100
+                          = (10 / 100) * 100
+                          = 10%
+  ```
+  * Example `fail_percentage.json`:
+  ```json
+  {"fail_count": 10, "fail_percentage": 10.0}
+  ```
+ 
+
 ## Test results
 * Once test run completed you should see `pyreport.html` file that auto generated by using above commands. \
 Open it and check the test results as shown in below presentation
 
 
 
 ## Presentation
```

### Comparing `pytest-pyreport-1.5.0/README.md` & `pytest_pyreport-1.6.0/src/pytest_pyreport.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pytest-pyreport
+Version: 1.6.0
+Summary: PyReport is a lightweight reporting plugin for Pytest that provides concise HTML report
+Home-page: https://github.com/ToghrulMirzayev/pytest-pyreport
+Author: Toghrul Mirzayev
+Author-email: togrul.mirzoev@gmail.com
+License: MIT
+Keywords: pytest_pyreport,python,pytest,report,slack,telegram,messenger,pyreport
+Classifier: Framework :: Pytest
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Jinja2
+Requires-Dist: pytest
+Requires-Dist: matplotlib
+Requires-Dist: requests
+Requires-Dist: logstyle
+
 # PyReport
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pytest-pyreport)
 
 # Quick overview
 PyReport is a lightweight reporting plugin for Pytest that provides concise HTML reports by parsing JunitXML test results
 
@@ -28,39 +51,56 @@
 ```
 
 ## Report generation
 * Run tests using below command to generate pyreport.html file with test results:
     ```
     pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport
     ```
-
+---
 * Run tests using below command if you want to send Telegram notification <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/83/Telegram_2019_Logo.svg/512px-Telegram_2019_Logo.svg.png?20231105064641" alt="Telegram" width="30" height="30">
     ```
     pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport --telegram-pyreport <chat id> <bot token>
     ```
   * Prerequisites:
     * You need your own Telegram bot, which can be easily created using Telegram instructions.
   You can take the “chat ID” and “bot token” from there.
-
+---
 * Run tests using below command if you want to send Slack notification <img src="https://raw.githubusercontent.com/devicons/devicon/55609aa5bd817ff167afce0d965585c92040787a/icons/slack/slack-original.svg" alt="Slack" width="30" height="30">
     ```
     pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport --slack-pyreport <webhook url> <channel id> <bot token>
     ```
   * Prerequisites:
     * You need your own Slack bot, which can be easily created using Slack instructions.
   You can take the “webhook url”, "channel id" and “bot token” from there.
-
+---
 * Run tests using below command if you want to check generated report on the server if it is available:
   ```
   pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport --telegram-pyreport <chat id> <bot token> --server <URL>
   pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport --slack-pyreport <webhook url> <channel id> <bot token> --server <URL>
   ```
   * Prerequisites:
     * You need to run server beforehand. As an example using CI/CD tools like Jenkins or GitHub Actions
 
+---
+* Run tests with failed tests counter. By running below command you will get JSON file with percentage of failed tests:
+  ```
+   pytest --junitxml=result.xml -o junit_family="xunit1" --pyreport --failed-tests-count
+  ```
+  * Fail percentage formula:
+  ```text
+  Failed Tests Percentage = (Number of Failed Tests / Total Number of Tests) * 100
+                          = (10 / 100) * 100
+                          = 10%
+  ```
+  * Example `fail_percentage.json`:
+  ```json
+  {"fail_count": 10, "fail_percentage": 10.0}
+  ```
+ 
+
 ## Test results
 * Once test run completed you should see `pyreport.html` file that auto generated by using above commands. \
 Open it and check the test results as shown in below presentation
 
 
 
 ## Presentation
```

### Comparing `pytest-pyreport-1.5.0/setup.py` & `pytest_pyreport-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pytest-pyreport',
-    version='1.5.0',
+    version='1.6.0',
     description='PyReport is a lightweight reporting plugin for Pytest that provides concise HTML report',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Toghrul Mirzayev',
     author_email='togrul.mirzoev@gmail.com',
     url='https://github.com/ToghrulMirzayev/pytest-pyreport',
     packages=find_packages("src"),
```

### Comparing `pytest-pyreport-1.5.0/src/pytest_pyreport/plugin.py` & `pytest_pyreport-1.6.0/src/pytest_pyreport/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,19 @@
         metavar=('WEBHOOK_URL', 'CHANNEL', 'BOT_TOKEN'),
         help='Send the report to Slack with the provided Webhook URL, Channel and Bot Token'
     )
     parser.addoption(
         '--server',
         help='URL or server address to include in the report notification'
     )
+    parser.addoption(
+        '--failed-tests-count',
+        action='store_true',
+        help='Output the count of failed tests to JSON file'
+    )
 
 
 def generate_and_save_chart(report_data):
     report_name = "PyReport"
 
     num_tests = len(report_data['test_cases'])
     num_failures = len([test_case for test_case in report_data['test_cases'] if test_case['result'] == 'fail'])
@@ -88,14 +93,15 @@
 
 def pytest_sessionfinish(session):
     config = session.config
     generate_html_report = config.getoption('--pyreport')
     telegram_config = config.getoption('--telegram-pyreport')
     slack_config = config.getoption('--slack-pyreport')
     server = config.getoption('--server')
+    fail_percentage_counter = config.getoption('--failed-tests-count')
 
     if generate_html_report:
         tree = ET.parse('result.xml')
         root = tree.getroot()
 
         testsuite = root.find('testsuite')
         total_time = float(testsuite.get('time'))
@@ -145,14 +151,25 @@
                                           num_skipped=num_skipped, total_time=total_time)
 
             with open('pyreport.html', 'w') as f:
                 f.write(html_output)
 
             custom_logger.box_log("HTML Report generation complete", CustomLog.COLOR_GREEN)
 
+        if fail_percentage_counter:
+            fail_percentage = (num_failures / num_tests) * 100
+
+            fail_percentage_data = {
+                "fail_count": num_failures,
+                "fail_percentage": fail_percentage
+            }
+
+            with open('fail_percentage.json', 'w') as json_file:
+                json.dump(fail_percentage_data, json_file)
+
         if telegram_config and server:
             chat_id, bot_token = telegram_config
             server_url = server
             send_report_to_telegram(chat_id, bot_token, server_url)
         elif telegram_config:
             chat_id, bot_token = telegram_config
             send_report_to_telegram(chat_id, bot_token)
```

### Comparing `pytest-pyreport-1.5.0/src/pytest_pyreport/templates/template.html` & `pytest_pyreport-1.6.0/src/pytest_pyreport/templates/template.html`

 * *Files identical despite different names*

