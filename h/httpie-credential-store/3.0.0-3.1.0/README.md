# Comparing `tmp/httpie-credential-store-3.0.0.tar.gz` & `tmp/httpie_credential_store-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpie-credential-store-3.0.0.tar", max compression
+gzip compressed data, was "httpie_credential_store-3.1.0.tar", max compression
```

## Comparing `httpie-credential-store-3.0.0.tar` & `httpie_credential_store-3.1.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     7701 2022-04-27 22:18:28.907437 httpie-credential-store-3.0.0/README.rst
--rw-r--r--   0        0        0      829 2022-04-27 22:18:28.907437 httpie-credential-store-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      157 2022-04-27 22:18:28.907437 httpie-credential-store-3.0.0/src/httpie_credential_store/__init__.py
--rw-r--r--   0        0        0     4029 2022-04-27 22:18:28.907437 httpie-credential-store-3.0.0/src/httpie_credential_store/_auth.py
--rw-r--r--   0        0        0     1975 2022-04-27 22:18:28.907437 httpie-credential-store-3.0.0/src/httpie_credential_store/_keychain.py
--rw-r--r--   0        0        0     1275 2022-04-27 22:18:28.907437 httpie-credential-store-3.0.0/src/httpie_credential_store/_plugin.py
--rw-r--r--   0        0        0     2440 2022-04-27 22:18:28.907437 httpie-credential-store-3.0.0/src/httpie_credential_store/_store.py
--rw-r--r--   0        0        0     9085 2022-04-27 22:18:36.464909 httpie-credential-store-3.0.0/setup.py
--rw-r--r--   0        0        0     8524 2022-04-27 22:18:36.465360 httpie-credential-store-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7701 2024-05-05 18:56:10.447491 httpie_credential_store-3.1.0/README.rst
+-rw-r--r--   0        0        0      831 2024-05-05 18:56:10.447491 httpie_credential_store-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      157 2024-05-05 18:56:10.447491 httpie_credential_store-3.1.0/src/httpie_credential_store/__init__.py
+-rw-r--r--   0        0        0     4029 2024-05-05 18:56:10.447491 httpie_credential_store-3.1.0/src/httpie_credential_store/_auth.py
+-rw-r--r--   0        0        0     1975 2024-05-05 18:56:10.447491 httpie_credential_store-3.1.0/src/httpie_credential_store/_keychain.py
+-rw-r--r--   0        0        0     1275 2024-05-05 18:56:10.447491 httpie_credential_store-3.1.0/src/httpie_credential_store/_plugin.py
+-rw-r--r--   0        0        0     2440 2024-05-05 18:56:10.447491 httpie_credential_store-3.1.0/src/httpie_credential_store/_store.py
+-rw-r--r--   0        0        0     8570 1970-01-01 00:00:00.000000 httpie_credential_store-3.1.0/PKG-INFO
```

### Comparing `httpie-credential-store-3.0.0/README.rst` & `httpie_credential_store-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `httpie-credential-store-3.0.0/pyproject.toml` & `httpie_credential_store-3.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "httpie-credential-store"
-version = "3.0.0"
+version = "3.1.0"
 description = "HTTPie: one auth to rule them all!"
 authors = ["Ihor Kalnytskyi <ihor@kalnytskyi.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ikalnytskyi/httpie-credential-store"
 repository = "https://github.com/ikalnytskyi/httpie-credential-store"
 keywords = ["httpie", "credential", "store", "keychain", "plugin", "auth"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 httpie = "^3.1"
-keyring = "^23.5"
+keyring = ">= 23.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 responses = "^0.20"
 mock = "^4.0"
 
 [tool.poetry.plugins."httpie.plugins.auth.v1"]
```

### Comparing `httpie-credential-store-3.0.0/src/httpie_credential_store/_auth.py` & `httpie_credential_store-3.1.0/src/httpie_credential_store/_auth.py`

 * *Files identical despite different names*

### Comparing `httpie-credential-store-3.0.0/src/httpie_credential_store/_keychain.py` & `httpie_credential_store-3.1.0/src/httpie_credential_store/_keychain.py`

 * *Files identical despite different names*

### Comparing `httpie-credential-store-3.0.0/src/httpie_credential_store/_plugin.py` & `httpie_credential_store-3.1.0/src/httpie_credential_store/_plugin.py`

 * *Files identical despite different names*

### Comparing `httpie-credential-store-3.0.0/src/httpie_credential_store/_store.py` & `httpie_credential_store-3.1.0/src/httpie_credential_store/_store.py`

 * *Files identical despite different names*

### Comparing `httpie-credential-store-3.0.0/setup.py` & `httpie_credential_store-3.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,340 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: httpie-credential-store
+Version: 3.1.0
+Summary: HTTPie: one auth to rule them all!
+Home-page: https://github.com/ikalnytskyi/httpie-credential-store
+License: MIT
+Keywords: httpie,credential,store,keychain,plugin,auth
+Author: Ihor Kalnytskyi
+Author-email: ihor@kalnytskyi.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpie (>=3.1,<4.0)
+Requires-Dist: keyring (>=23.5)
+Project-URL: Repository, https://github.com/ikalnytskyi/httpie-credential-store
+Description-Content-Type: text/x-rst
 
-package_dir = \
-{'': 'src'}
+Credential store plugin for HTTPie
+==================================
 
-packages = \
-['httpie_credential_store']
+HTTPie Credential Store is an `HTTPie`_ authentication plugin that looks
+for credentials using a given URL and attaches them to the ongoing HTTP
+request. That said, you don't need to memorize and/or look for
+tokens/username/passwords anymore. Simply add them to the credential
+store and everything else will be done for you by this plugin. It goes
+without saying that this plugin supports various secured secret storages
+such as system keychains or password managers (see keychain providers).
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['httpie>=3.1,<4.0', 'keyring>=23.5,<24.0']
-
-entry_points = \
-{'httpie.plugins.auth.v1': ['credential-store = '
-                            'httpie_credential_store:CredentialStoreAuthPlugin',
-                            'creds = httpie_credential_store:CredsAuthPlugin']}
-
-setup_kwargs = {
-    'name': 'httpie-credential-store',
-    'version': '3.0.0',
-    'description': 'HTTPie: one auth to rule them all!',
-    'long_description': 'Credential store plugin for HTTPie\n==================================\n\nHTTPie Credential Store is an `HTTPie`_ authentication plugin that looks\nfor credentials using a given URL and attaches them to the ongoing HTTP\nrequest. That said, you don\'t need to memorize and/or look for\ntokens/username/passwords anymore. Simply add them to the credential\nstore and everything else will be done for you by this plugin. It goes\nwithout saying that this plugin supports various secured secret storages\nsuch as system keychains or password managers (see keychain providers).\n\nEager to get started? Just start with installing!\n\n.. code:: bash\n\n   $ python3 -m pip install httpie-credential-store\n\n\nUsage\n-----\n\n.. note:: Please, do not forget to activate the plugin by invoking\n          ``http`` with ``-A creds`` option.\n\nOnce installed, the plugin will look for credentials in the credential\nfile. The credential file is stored in HTTPie configuration directory.\nSo on Linux/macOS, it will look for ``~/.httpie/credentials.json``,\nwhile on Windows - for ``%APPDATA%\\httpie\\credentials.json``. The\ncredential file will not be created for you, you\'re fully responsible\nfor creating one.\n\nBy its nature, the credentials file is a JSON array of credential\nrecords. Each credential record consists of the following properties:\n\n* ``url`` (*required*) is a regular expression pattern that is used to\n  map credential record to the ongoing HTTP request. I.e. if the regular\n  expression matches URL of the ongoing HTTP request, credentials of\n  matched record must be attached.\n\n* ``auth`` (*required*) is an authentication provider to use for a given\n  record. The provider will be used to attach credentials to the ongoing\n  HTTP request if the record is matched.\n\n* ``id`` (*optional*) is unique identifier of the credential record that\n  can be used to solve ambiguousness between two or more matched\n  credential records. By using ``id`` one may achieve support of\n  multiple accounts for the same service.\n\nExample:\n\n.. code:: json\n\n   [\n     {\n       "url": "api.github.com",\n       "auth": {\n         "provider": "token",\n         "token": "your-github-oauth-token",\n         "scheme": "token"\n       }\n     },\n     {\n       "id": "bots",\n       "url": "api.github.com",\n       "auth": {\n         "provider": "token",\n         "token": "bots-github-oauth-token",\n         "scheme": "token"\n       }\n     }\n   ]\n\nThe example above assumes you store your secrets unencrypted in the\ncredential file. Despite enforcing you to set sole access permissions\nfor the credential file, it\'s not secured and, hence, not recommended.\nHTTPie Credential Store plugin can pull secrets and other sensitive\ninformation out from password managers or system keychains. For\ninstance, you can pull your token from the `password store`_ by using\nthe following credential record:\n\n.. code:: json\n\n   [\n     {\n       "url": "api.github.com",\n       "auth": {\n         "provider": "token",\n         "scheme": "token",\n         "token": {\n           "keychain": "password-store",\n           "name": "github.com/ikalnytskyi/token"\n         }\n       }\n     }\n   ]\n\nOnce the credential store is filled, you\'re ready to use the plugin at\nyour will. In order to activate the plugin, you must pass ``-A creds``\nor ``-A credential-store`` to ``http`` executable.\n\n.. code:: bash\n\n   $ http -A creds https://api.github.com\n\nOptionally, you can provide an ID of the credential record to use by\npassing ``-a`` argument.\n\n.. code:: bash\n\n   $ http -A creds -a bots https://api.github.com\n\n\nAuthentication providers\n------------------------\n\nHTTPie Credential Store comes with the following authentication\nproviders out of box.\n\n\n``basic``\n.........\n\nThe \'Basic\' HTTP authentication scheme as defined in :RFC:`7617`.\nTransmits credentials as username/password pairs, encoded using Base64.\n\n.. code:: json\n\n   {\n     "provider": "basic",\n     "username": "ikalnytskyi",\n     "password": "p@ss"\n   }\n\nwhere\n\n* ``username`` is a username to authenticate\n* ``password`` is a password of the authenticating user\n\n\n``digest``\n..........\n\nThe \'Digest\' HTTP authentication scheme as defined in :RFC:`2617`. It\napplies a hash function to the username and password before sending them\nover the network.\n\n.. code:: json\n\n   {\n     "provider": "digest",\n     "username": "ikalnytskyi",\n     "password": "p@ss"\n   }\n\nwhere\n\n* ``username`` is a username to authenticate\n* ``password`` is a password of the authenticating user\n\n\n``token``\n.........\n\nThe \'Token\' HTTP authentication scheme (also called \'Bearer\') transmits\ntoken in the ``Authorization`` HTTP header.\n\n.. code:: json\n\n   {\n     "provider": "token",\n     "token": "t0k3n",\n     "scheme": "JWT"\n   }\n\nwhere\n\n* ``token`` is a token of the authenticating user\n* ``scheme`` (optional, default: "Bearer") is an authenticating scheme\n\n\n``header``\n..........\n\nThe \'Header\' HTTP authentication is not exactly an authentication\nscheme. It\'s rather a way to pass any free-formed HTTP header with\nsecret or not.\n\n.. code:: json\n\n   {\n     "provider": "header",\n     "name": "X-Extra-Key",\n     "value": "k3y"\n   }\n\nwhere\n\n* ``name`` is an HTTP header name to use\n* ``value`` is an HTTP header value to pass\n\n\n``multiple``\n............\n\nThis is a fake authentication scheme even in terms of this plugin. It\ndoes no auth but chains and applies one or more providers\nsimultaneously. It\'s something you will (likely) never use.\n\n.. code:: json\n\n   {\n     "provider": "multiple",\n     "providers": [\n       {\n         "provider": "token",\n         "token": "t0k3n"\n       },\n       {\n         "provider": "header",\n         "name": "X-Extra-Key",\n         "value": "k3y"\n       }\n     ]\n   }\n\nwhere\n\n* ``providers`` is a list of auth providers to use simultaneously\n\n\nKeychain providers\n------------------\n\nThe plugin supports a bunch of keychains that can be used to pull\nsecrets from secured storage.\n\n\n``shell``\n.........\n\nShell provider is nothing more but a mere shell command to execute. The\ncommand must return a secret to the plugin via standard output stream.\nThis is a universal approach that can be used to glue together various\nunsupported password managers and/or keychains.\n\nExample:\n\n.. code:: json\n\n   {\n     "keychain": "shell",\n     "command": "cat ~/path/to/secret | tr -d \'\\n\'"\n   }\n\nwhere\n\n* ``command`` is a shell command to execute\n\n\n\n``system``\n..........\n\nSystem provider, as the name suggests, use your system keychain to pull\nsecrets from. It may be **KWallet**, **GNOME Keyring**, **macOS\nKeychain** or even **Windows Credential Locker**.\n\nExample:\n\n.. code:: json\n\n   {\n     "keychain": "system",\n     "service": "github",\n     "username": "ikalnytskyi"\n   }\n\nwhere\n\n* ``service`` is a service to pull data for\n* ``username`` is a username for that service to pull data for\n\n\n``password-store``\n..................\n\nPassword store provider is a bridge between this plugin and the\n`password store`_. It invokes ``pass`` on your system and pulls the\nsecret from the first line of the stored record (normally password).\n\nExample:\n\n.. code:: json\n\n   {\n     "keychain": "password-store",\n     "name": "github.com/ikalnytskyi"\n   }\n\nwhere\n\n* ``name`` is a pass name in terms of the password store\n\nFAQ\n---\n\n* **Q**: How to learn which credentials have been attached to the request?\n\n  **A**: Unfortunately, due to late credentials binding, it\'s impossible\n  to learn which credentials have been used by running ``http --debug``\n  command. Nevertheless, one can check amends made by auth providers by\n  inspect HTTP headers transmitted within the request by passing ``-v``\n  argument to HTTPie: ``http -v``.\n\n\n.. _HTTPie: https://httpie.org/\n.. _password store: https://www.passwordstore.org/\n',
-    'author': 'Ihor Kalnytskyi',
-    'author_email': 'ihor@kalnytskyi.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ikalnytskyi/httpie-credential-store',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+Eager to get started? Just start with installing!
 
+.. code:: bash
+
+   $ python3 -m pip install httpie-credential-store
+
+
+Usage
+-----
+
+.. note:: Please, do not forget to activate the plugin by invoking
+          ``http`` with ``-A creds`` option.
+
+Once installed, the plugin will look for credentials in the credential
+file. The credential file is stored in HTTPie configuration directory.
+So on Linux/macOS, it will look for ``~/.httpie/credentials.json``,
+while on Windows - for ``%APPDATA%\httpie\credentials.json``. The
+credential file will not be created for you, you're fully responsible
+for creating one.
+
+By its nature, the credentials file is a JSON array of credential
+records. Each credential record consists of the following properties:
+
+* ``url`` (*required*) is a regular expression pattern that is used to
+  map credential record to the ongoing HTTP request. I.e. if the regular
+  expression matches URL of the ongoing HTTP request, credentials of
+  matched record must be attached.
+
+* ``auth`` (*required*) is an authentication provider to use for a given
+  record. The provider will be used to attach credentials to the ongoing
+  HTTP request if the record is matched.
+
+* ``id`` (*optional*) is unique identifier of the credential record that
+  can be used to solve ambiguousness between two or more matched
+  credential records. By using ``id`` one may achieve support of
+  multiple accounts for the same service.
+
+Example:
+
+.. code:: json
+
+   [
+     {
+       "url": "api.github.com",
+       "auth": {
+         "provider": "token",
+         "token": "your-github-oauth-token",
+         "scheme": "token"
+       }
+     },
+     {
+       "id": "bots",
+       "url": "api.github.com",
+       "auth": {
+         "provider": "token",
+         "token": "bots-github-oauth-token",
+         "scheme": "token"
+       }
+     }
+   ]
+
+The example above assumes you store your secrets unencrypted in the
+credential file. Despite enforcing you to set sole access permissions
+for the credential file, it's not secured and, hence, not recommended.
+HTTPie Credential Store plugin can pull secrets and other sensitive
+information out from password managers or system keychains. For
+instance, you can pull your token from the `password store`_ by using
+the following credential record:
+
+.. code:: json
+
+   [
+     {
+       "url": "api.github.com",
+       "auth": {
+         "provider": "token",
+         "scheme": "token",
+         "token": {
+           "keychain": "password-store",
+           "name": "github.com/ikalnytskyi/token"
+         }
+       }
+     }
+   ]
+
+Once the credential store is filled, you're ready to use the plugin at
+your will. In order to activate the plugin, you must pass ``-A creds``
+or ``-A credential-store`` to ``http`` executable.
+
+.. code:: bash
+
+   $ http -A creds https://api.github.com
+
+Optionally, you can provide an ID of the credential record to use by
+passing ``-a`` argument.
+
+.. code:: bash
+
+   $ http -A creds -a bots https://api.github.com
+
+
+Authentication providers
+------------------------
+
+HTTPie Credential Store comes with the following authentication
+providers out of box.
+
+
+``basic``
+.........
+
+The 'Basic' HTTP authentication scheme as defined in :RFC:`7617`.
+Transmits credentials as username/password pairs, encoded using Base64.
+
+.. code:: json
+
+   {
+     "provider": "basic",
+     "username": "ikalnytskyi",
+     "password": "p@ss"
+   }
+
+where
+
+* ``username`` is a username to authenticate
+* ``password`` is a password of the authenticating user
+
+
+``digest``
+..........
+
+The 'Digest' HTTP authentication scheme as defined in :RFC:`2617`. It
+applies a hash function to the username and password before sending them
+over the network.
+
+.. code:: json
+
+   {
+     "provider": "digest",
+     "username": "ikalnytskyi",
+     "password": "p@ss"
+   }
+
+where
+
+* ``username`` is a username to authenticate
+* ``password`` is a password of the authenticating user
+
+
+``token``
+.........
+
+The 'Token' HTTP authentication scheme (also called 'Bearer') transmits
+token in the ``Authorization`` HTTP header.
+
+.. code:: json
+
+   {
+     "provider": "token",
+     "token": "t0k3n",
+     "scheme": "JWT"
+   }
+
+where
+
+* ``token`` is a token of the authenticating user
+* ``scheme`` (optional, default: "Bearer") is an authenticating scheme
+
+
+``header``
+..........
+
+The 'Header' HTTP authentication is not exactly an authentication
+scheme. It's rather a way to pass any free-formed HTTP header with
+secret or not.
+
+.. code:: json
+
+   {
+     "provider": "header",
+     "name": "X-Extra-Key",
+     "value": "k3y"
+   }
+
+where
+
+* ``name`` is an HTTP header name to use
+* ``value`` is an HTTP header value to pass
+
+
+``multiple``
+............
+
+This is a fake authentication scheme even in terms of this plugin. It
+does no auth but chains and applies one or more providers
+simultaneously. It's something you will (likely) never use.
+
+.. code:: json
+
+   {
+     "provider": "multiple",
+     "providers": [
+       {
+         "provider": "token",
+         "token": "t0k3n"
+       },
+       {
+         "provider": "header",
+         "name": "X-Extra-Key",
+         "value": "k3y"
+       }
+     ]
+   }
+
+where
+
+* ``providers`` is a list of auth providers to use simultaneously
+
+
+Keychain providers
+------------------
+
+The plugin supports a bunch of keychains that can be used to pull
+secrets from secured storage.
+
+
+``shell``
+.........
+
+Shell provider is nothing more but a mere shell command to execute. The
+command must return a secret to the plugin via standard output stream.
+This is a universal approach that can be used to glue together various
+unsupported password managers and/or keychains.
+
+Example:
+
+.. code:: json
+
+   {
+     "keychain": "shell",
+     "command": "cat ~/path/to/secret | tr -d '\n'"
+   }
+
+where
+
+* ``command`` is a shell command to execute
+
+
+
+``system``
+..........
+
+System provider, as the name suggests, use your system keychain to pull
+secrets from. It may be **KWallet**, **GNOME Keyring**, **macOS
+Keychain** or even **Windows Credential Locker**.
+
+Example:
+
+.. code:: json
+
+   {
+     "keychain": "system",
+     "service": "github",
+     "username": "ikalnytskyi"
+   }
+
+where
+
+* ``service`` is a service to pull data for
+* ``username`` is a username for that service to pull data for
+
+
+``password-store``
+..................
+
+Password store provider is a bridge between this plugin and the
+`password store`_. It invokes ``pass`` on your system and pulls the
+secret from the first line of the stored record (normally password).
+
+Example:
+
+.. code:: json
+
+   {
+     "keychain": "password-store",
+     "name": "github.com/ikalnytskyi"
+   }
+
+where
+
+* ``name`` is a pass name in terms of the password store
+
+FAQ
+---
+
+* **Q**: How to learn which credentials have been attached to the request?
+
+  **A**: Unfortunately, due to late credentials binding, it's impossible
+  to learn which credentials have been used by running ``http --debug``
+  command. Nevertheless, one can check amends made by auth providers by
+  inspect HTTP headers transmitted within the request by passing ``-v``
+  argument to HTTPie: ``http -v``.
+
+
+.. _HTTPie: https://httpie.org/
+.. _password store: https://www.passwordstore.org/
 
-setup(**setup_kwargs)
```

