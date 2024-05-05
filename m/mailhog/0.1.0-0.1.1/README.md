# Comparing `tmp/mailhog-0.1.0.tar.gz` & `tmp/mailhog-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailhog-0.1.0.tar", max compression
+gzip compressed data, was "mailhog-0.1.1.tar", max compression
```

## Comparing `mailhog-0.1.0.tar` & `mailhog-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1061 2022-12-27 15:39:35.705577 mailhog-0.1.0/LICENSE
--rw-r--r--   0        0        0     4391 2022-12-27 15:52:23.050205 mailhog-0.1.0/README.md
--rw-r--r--   0        0        0      120 2022-12-27 15:39:35.705577 mailhog-0.1.0/mailhog/__init__.py
--rw-r--r--   0        0        0        0 2022-12-27 15:39:35.705577 mailhog-0.1.0/mailhog/exceptions.py
--rw-r--r--   0        0        0     2276 2022-12-27 15:39:35.705577 mailhog-0.1.0/mailhog/main.py
--rw-r--r--   0        0        0     2909 2022-12-27 15:39:35.705577 mailhog-0.1.0/mailhog/types.py
--rw-r--r--   0        0        0        0 2022-12-27 15:39:35.705577 mailhog-0.1.0/mailhog/utils.py
--rw-r--r--   0        0        0      619 2022-12-27 15:42:56.677916 mailhog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5274 1970-01-01 00:00:00.000000 mailhog-0.1.0/setup.py
--rw-r--r--   0        0        0     5179 1970-01-01 00:00:00.000000 mailhog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-05 18:07:55.753379 mailhog-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4621 2024-05-05 18:07:55.753379 mailhog-0.1.1/README.md
+-rw-r--r--   0        0        0      120 2024-05-05 18:07:55.753379 mailhog-0.1.1/mailhog/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 18:07:55.753379 mailhog-0.1.1/mailhog/exceptions.py
+-rw-r--r--   0        0        0     2553 2024-05-05 18:07:55.753379 mailhog-0.1.1/mailhog/main.py
+-rw-r--r--   0        0        0     2929 2024-05-05 18:07:55.753379 mailhog-0.1.1/mailhog/types.py
+-rw-r--r--   0        0        0        0 2024-05-05 18:07:55.753379 mailhog-0.1.1/mailhog/utils.py
+-rw-r--r--   0        0        0      619 2024-05-05 18:10:36.233382 mailhog-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5460 1970-01-01 00:00:00.000000 mailhog-0.1.1/PKG-INFO
```

### Comparing `mailhog-0.1.0/LICENSE` & `mailhog-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mailhog-0.1.0/README.md` & `mailhog-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 mailhog.search('test@test.com', 'To')
 
 # Search for messages by sender
 mailhog.search('test@test.com', 'From')
 
 # Delete all messages
 mailhog.delete_all()
+
+# Delete a message
+mailhog.delete(messages.items[0])
 ```
 
 # API
 ##  mailhog.Mailhog
 > Mailhog API client
 #### Parameters
 
@@ -94,14 +97,26 @@
 from mailhog import Mailhog
 
 mailhog = Mailhog()
 
 mailhog.delete_all()
 ```
 
+### `delete()`
+> Delete a message
+
+#### Example
+```python
+from mailhog import Mailhog
+
+mailhog = Mailhog()
+messages = mailhog.messages()
+mailhog.delete(messages.items[0])
+```
+
 # Datatypes
 ##  mailhog.Messages
 > A list of `mailhog.Message` objects
 #### Attributes
 * `total` - The total number of messages
 * `start` - The start index of the messages
 * `count` - The total number of received messages
@@ -178,15 +193,15 @@
 
 ### Roadmap
 
 - [x] Mailhog API v2 Messages Endpoint
 - [x] Mailhog API v2 Search Endpoint
 - [ ] Mailhog API v2 Jim Endpoint
 - [x] Mailhog API v1 Delete Messages Endpoint
-- [ ] Mailhog API v1 Delete Message Endpoint
+- [x] Mailhog API v1 Delete Message Endpoint
 
 
 ### Local Development
 
 To install the package locally, run the following commands:
 
 ```
```

### Comparing `mailhog-0.1.0/mailhog/types.py` & `mailhog-0.1.1/mailhog/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Dict, List, Union
+from typing import Dict, List, Union, Optional
 
 from dataclass_wizard import JSONWizard, json_field
 
 
 @dataclass
 class Path:
     """A path
@@ -110,15 +110,15 @@
     def get_recipients(self) -> List[str]:
         """Get the recipients of the message.
 
         :return: The list of recipients of the message.
         """
         return [f"{path.mailbox}@{path.domain}" for path in self.to]
 
-    def get_subject(self) -> str:
+    def get_subject(self) -> Optional[str]:
         """Get the subject of the message.
 
         :return: The subject.
 
         """
 
         if "Subject" in self.content.headers:
```

### Comparing `mailhog-0.1.0/pyproject.toml` & `mailhog-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mailhog"
-version = "0.1.0"
+version = "0.1.1"
 description = "A python client for the Mailhog API"
 keywords = ["mailhog", "client", "wrapper", "api"]
 authors = ["nklsw"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/nklsw/mailhog-python"
 repository = "https://github.com/nklsw/mailhog-python"
```

### Comparing `mailhog-0.1.0/setup.py` & `mailhog-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,249 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mailhog
+Version: 0.1.1
+Summary: A python client for the Mailhog API
+Home-page: https://github.com/nklsw/mailhog-python
+License: MIT
+Keywords: mailhog,client,wrapper,api
+Author: nklsw
+Requires-Python: >=3.7,<4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dataclass-wizard (>=0.22.2,<0.23.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Repository, https://github.com/nklsw/mailhog-python
+Description-Content-Type: text/markdown
 
-packages = \
-['mailhog']
+# mailhog-python
 
-package_data = \
-{'': ['*']}
+A python client for the [Mailhog](https://github.com/mailhog/MailHog) API
 
-install_requires = \
-['dataclass-wizard>=0.22.2,<0.23.0', 'requests>=2.28.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'mailhog',
-    'version': '0.1.0',
-    'description': 'A python client for the Mailhog API',
-    'long_description': "# mailhog-python\n\nA python client for the [Mailhog](https://github.com/mailhog/MailHog) API\n\n\n## Installation\n\nInstall from PyPI \n\n```\npip install mailhog\n```\n\n## Get Started\n\n```python\nfrom mailhog import Mailhog\n\nmailhog = Mailhog() # Defaults to http://localhost:8025\n\n# Get all messages\nmailhog.messages()\n\n# Get all messages with start and limit parameters\nmailhog.messages(start=0, limit=10)\n\n# Search for messages\nmailhog.search('Text contained in the message')\n\n# Search for messages by recipient\nmailhog.search('test@test.com', 'To')\n\n# Search for messages by sender\nmailhog.search('test@test.com', 'From')\n\n# Delete all messages\nmailhog.delete_all()\n```\n\n# API\n##  mailhog.Mailhog\n> Mailhog API client\n#### Parameters\n\n* `host` - The host of the Mailhog API, defaults to `localhost`\n* `port` - The port of the Mailhog API, defaults to `8025`\n\n### Methods\n### `messages(start=0, limit=10)`\n> Get all messages\n\n#### Parameters\n* `start` - The start index of the messages to return, defaults to `0`\n* `limit` - The number of messages to return, defaults to `10`\n\n#### Returns\n* `list` - A list of `mailhog.Message` objects\n\n#### Example\n```python\nfrom mailhog import Mailhog\n\nmailhog = Mailhog()\n\nmessages = mailhog.messages()\n```\n\n### `search(query, kind='containing', start=0, limit=10)`\n> Search for messages\n\n#### Parameters\n* `query` - The query to search for\n* `kind` - The kind of search to perform, defaults to `containing`\n* `start` - The start index of the messages to return, defaults to `0`\n* `limit` - The number of messages to return, defaults to `10`\n\n#### Returns\n* `list` - A list of `mailhog.Message` objects\n\n#### Example\n```python\nfrom mailhog import Mailhog\n\nmailhog = Mailhog()\n\nmessages = mailhog.search('Some Text')\n```\n\n### `delete_all()`\n> Delete all messages\n\n#### Example\n```python\nfrom mailhog import Mailhog\n\nmailhog = Mailhog()\n\nmailhog.delete_all()\n```\n\n# Datatypes\n##  mailhog.Messages\n> A list of `mailhog.Message` objects\n#### Attributes\n* `total` - The total number of messages\n* `start` - The start index of the messages\n* `count` - The total number of received messages\n* `items` - A list of `mailhog.Message` objects\n\n##  mailhog.Message\n> A message from Mailhog\n#### Attributes\n* `id` - The ID of the message\n* `from_` - A mailhog.Path object containing the sender\n* `to` - A List of mailhog.Path objects containing the recipients\n* `created` - The date the message was created\n* `content` - A mailhog.Content object containing the content of the message\n* `raw`: - The raw message\n* `mime` - A mailhog.MIME object containing the MIME data of the message\n\n#### Methods\n### `get_sender()`\n> Get the sender of the message\n\n#### Returns\n* `str` - The sender of the message\n\n### `get_recipients()`\n> Get the recipients of the message\n\n#### Returns\n* `list` - A list of recipients\n\n### `get_subject()`\n> Get the subject of the message\n\n#### Returns\n* `str` - The subject of the message\n\n##  mailhog.Path\n> A path object\n#### Attributes\n* `relays` - A list of relays\n* `mailbox` - The mailbox\n* `domain` - The domain\n* `params` - The parameters\n\n##  mailhog.Content\n> The content of a message\n#### Attributes\n* `headers` - A Dict of headers of the message\n* `body` - The body of the message\n* `size` - The size of the message\n* `mime` - The MIME type of the message\n\n\n##  mailhog.MIMEBody\n> The body of a MIME message\n#### Attributes\n* `parts` - A list of mailhog.MIMEContent objects\n\n\n##  mailhog.MIMEContent\n> The content of a MIME message\n#### Attributes\n* `headers` - A Dict of headers of the message\n* `body` - The body of the message\n* `size` - The size of the message\n* `mime` - The MIME type of the message\n\n___\n\n## About the Package\n\n### WIP\n\nThis package is still a work in progress. If you find any bugs or have any suggestions, please open an issue on the [GitHub repository](https://github.com/nklsw/mailhog-python)\n\n### Roadmap\n\n- [x] Mailhog API v2 Messages Endpoint\n- [x] Mailhog API v2 Search Endpoint\n- [ ] Mailhog API v2 Jim Endpoint\n- [x] Mailhog API v1 Delete Messages Endpoint\n- [ ] Mailhog API v1 Delete Message Endpoint\n\n\n### Local Development\n\nTo install the package locally, run the following commands:\n\n```\ngit clone\ncd mailhog-python\n\npoetry install\n```\n\nTo run a mailhog instance locally, run the following command:\n\n```\ndocker-compose up -d\n```\n\n\n\nTo run the tests, run the following command:\n\n```\npoetry run pytest\n```\n",
-    'author': 'nklsw',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nklsw/mailhog-python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4',
-}
 
+## Installation
+
+Install from PyPI 
+
+```
+pip install mailhog
+```
+
+## Get Started
+
+```python
+from mailhog import Mailhog
+
+mailhog = Mailhog() # Defaults to http://localhost:8025
+
+# Get all messages
+mailhog.messages()
+
+# Get all messages with start and limit parameters
+mailhog.messages(start=0, limit=10)
+
+# Search for messages
+mailhog.search('Text contained in the message')
+
+# Search for messages by recipient
+mailhog.search('test@test.com', 'To')
+
+# Search for messages by sender
+mailhog.search('test@test.com', 'From')
+
+# Delete all messages
+mailhog.delete_all()
+
+# Delete a message
+mailhog.delete(messages.items[0])
+```
+
+# API
+##  mailhog.Mailhog
+> Mailhog API client
+#### Parameters
+
+* `host` - The host of the Mailhog API, defaults to `localhost`
+* `port` - The port of the Mailhog API, defaults to `8025`
+
+### Methods
+### `messages(start=0, limit=10)`
+> Get all messages
+
+#### Parameters
+* `start` - The start index of the messages to return, defaults to `0`
+* `limit` - The number of messages to return, defaults to `10`
+
+#### Returns
+* `list` - A list of `mailhog.Message` objects
+
+#### Example
+```python
+from mailhog import Mailhog
+
+mailhog = Mailhog()
+
+messages = mailhog.messages()
+```
+
+### `search(query, kind='containing', start=0, limit=10)`
+> Search for messages
+
+#### Parameters
+* `query` - The query to search for
+* `kind` - The kind of search to perform, defaults to `containing`
+* `start` - The start index of the messages to return, defaults to `0`
+* `limit` - The number of messages to return, defaults to `10`
+
+#### Returns
+* `list` - A list of `mailhog.Message` objects
+
+#### Example
+```python
+from mailhog import Mailhog
+
+mailhog = Mailhog()
+
+messages = mailhog.search('Some Text')
+```
+
+### `delete_all()`
+> Delete all messages
+
+#### Example
+```python
+from mailhog import Mailhog
+
+mailhog = Mailhog()
+
+mailhog.delete_all()
+```
+
+### `delete()`
+> Delete a message
+
+#### Example
+```python
+from mailhog import Mailhog
+
+mailhog = Mailhog()
+messages = mailhog.messages()
+mailhog.delete(messages.items[0])
+```
+
+# Datatypes
+##  mailhog.Messages
+> A list of `mailhog.Message` objects
+#### Attributes
+* `total` - The total number of messages
+* `start` - The start index of the messages
+* `count` - The total number of received messages
+* `items` - A list of `mailhog.Message` objects
+
+##  mailhog.Message
+> A message from Mailhog
+#### Attributes
+* `id` - The ID of the message
+* `from_` - A mailhog.Path object containing the sender
+* `to` - A List of mailhog.Path objects containing the recipients
+* `created` - The date the message was created
+* `content` - A mailhog.Content object containing the content of the message
+* `raw`: - The raw message
+* `mime` - A mailhog.MIME object containing the MIME data of the message
+
+#### Methods
+### `get_sender()`
+> Get the sender of the message
+
+#### Returns
+* `str` - The sender of the message
+
+### `get_recipients()`
+> Get the recipients of the message
+
+#### Returns
+* `list` - A list of recipients
+
+### `get_subject()`
+> Get the subject of the message
+
+#### Returns
+* `str` - The subject of the message
+
+##  mailhog.Path
+> A path object
+#### Attributes
+* `relays` - A list of relays
+* `mailbox` - The mailbox
+* `domain` - The domain
+* `params` - The parameters
+
+##  mailhog.Content
+> The content of a message
+#### Attributes
+* `headers` - A Dict of headers of the message
+* `body` - The body of the message
+* `size` - The size of the message
+* `mime` - The MIME type of the message
+
+
+##  mailhog.MIMEBody
+> The body of a MIME message
+#### Attributes
+* `parts` - A list of mailhog.MIMEContent objects
+
+
+##  mailhog.MIMEContent
+> The content of a MIME message
+#### Attributes
+* `headers` - A Dict of headers of the message
+* `body` - The body of the message
+* `size` - The size of the message
+* `mime` - The MIME type of the message
+
+___
+
+## About the Package
+
+### WIP
+
+This package is still a work in progress. If you find any bugs or have any suggestions, please open an issue on the [GitHub repository](https://github.com/nklsw/mailhog-python)
+
+### Roadmap
+
+- [x] Mailhog API v2 Messages Endpoint
+- [x] Mailhog API v2 Search Endpoint
+- [ ] Mailhog API v2 Jim Endpoint
+- [x] Mailhog API v1 Delete Messages Endpoint
+- [x] Mailhog API v1 Delete Message Endpoint
+
+
+### Local Development
+
+To install the package locally, run the following commands:
+
+```
+git clone
+cd mailhog-python
+
+poetry install
+```
+
+To run a mailhog instance locally, run the following command:
+
+```
+docker-compose up -d
+```
+
+
+
+To run the tests, run the following command:
+
+```
+poetry run pytest
+```
 
-setup(**setup_kwargs)
```

