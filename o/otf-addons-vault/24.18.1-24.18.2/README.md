# Comparing `tmp/otf_addons_vault-24.18.1.tar.gz` & `tmp/otf_addons_vault-24.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otf_addons_vault-24.18.1.tar", last modified: Sun May  5 14:22:33 2024, max compression
+gzip compressed data, was "otf_addons_vault-24.18.2.tar", last modified: Sun May  5 15:53:12 2024, max compression
```

## Comparing `otf_addons_vault-24.18.1.tar` & `otf_addons_vault-24.18.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.760862 otf_addons_vault-24.18.1/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/AUTHORS
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/LICENSE
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3705 2024-05-05 14:22:33.756862 otf_addons_vault-24.18.1/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2107 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14429 2024-05-05 14:21:41.000000 otf_addons_vault-24.18.1/pyproject.toml
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-05-05 14:22:33.760862 otf_addons_vault-24.18.1/setup.cfg
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.752863 otf_addons_vault-24.18.1/src/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.752863 otf_addons_vault-24.18.1/src/opentaskpy/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.752863 otf_addons_vault-24.18.1/src/opentaskpy/plugins/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.752863 otf_addons_vault-24.18.1/src/opentaskpy/plugins/lookup/
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.752863 otf_addons_vault-24.18.1/src/opentaskpy/plugins/lookup/hashicorp/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3654 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/src/opentaskpy/plugins/lookup/hashicorp/vault.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.756862 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3705 2024-05-05 14:22:33.000000 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      347 2024-05-05 14:22:33.000000 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-05-05 14:22:33.000000 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      208 2024-05-05 14:22:33.000000 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2024-05-05 14:22:33.000000 otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/top_level.txt
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 14:22:33.756862 otf_addons_vault-24.18.1/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3984 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.1/tests/test_plugin_vault.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 15:53:12.796828 otf_addons_vault-24.18.2/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       72 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.2/AUTHORS
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    35149 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.2/LICENSE
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-05-05 14:07:00.000000 otf_addons_vault-24.18.2/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3889 2024-05-05 15:53:12.796828 otf_addons_vault-24.18.2/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2291 2024-05-05 15:50:50.000000 otf_addons_vault-24.18.2/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    14429 2024-05-05 15:53:05.000000 otf_addons_vault-24.18.2/pyproject.toml
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-05-05 15:53:12.796828 otf_addons_vault-24.18.2/setup.cfg
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 15:53:12.776828 otf_addons_vault-24.18.2/src/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 15:53:12.776828 otf_addons_vault-24.18.2/src/opentaskpy/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 15:53:12.776828 otf_addons_vault-24.18.2/src/opentaskpy/plugins/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 15:53:12.776828 otf_addons_vault-24.18.2/src/opentaskpy/plugins/lookup/
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 15:53:12.784828 otf_addons_vault-24.18.2/src/opentaskpy/plugins/lookup/hashicorp/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3920 2024-05-05 15:45:38.000000 otf_addons_vault-24.18.2/src/opentaskpy/plugins/lookup/hashicorp/vault.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 15:53:12.792828 otf_addons_vault-24.18.2/src/otf_addons_vault.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3889 2024-05-05 15:53:12.000000 otf_addons_vault-24.18.2/src/otf_addons_vault.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      347 2024-05-05 15:53:12.000000 otf_addons_vault-24.18.2/src/otf_addons_vault.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-05-05 15:53:12.000000 otf_addons_vault-24.18.2/src/otf_addons_vault.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      208 2024-05-05 15:53:12.000000 otf_addons_vault-24.18.2/src/otf_addons_vault.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       11 2024-05-05 15:53:12.000000 otf_addons_vault-24.18.2/src/otf_addons_vault.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-05 15:53:12.788828 otf_addons_vault-24.18.2/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4899 2024-05-05 15:37:32.000000 otf_addons_vault-24.18.2/tests/test_plugin_vault.py
```

### Comparing `otf_addons_vault-24.18.1/LICENSE` & `otf_addons_vault-24.18.2/LICENSE`

 * *Files identical despite different names*

### Comparing `otf_addons_vault-24.18.1/PKG-INFO` & `otf_addons_vault-24.18.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otf-addons-vault
-Version: 24.18.1
+Version: 24.18.2
 Summary: Addons for opentaskpy, giving it the ability to read variables from Hashicorp Vault
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/otf-addons-vault
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/otf-addons-vault/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/otf-addons-vault/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,hashicorp,vault,secrets,otf
@@ -59,14 +59,18 @@
     "VAULT_ADDR": "https://vault.example.com:8200",
     "VAULT_TOKEN": "some_token"
 }
 ```
 
 If these variables are set in the environment, then these will be used if not set elsewhere.
 
+# Vault KV Secrets Engine Version
+
+The default version is v1. This can be overridden by setting the environment variable `VAULT_API_VER` to `v2` (or specifying the variable manually)
+
 # Variable Lookup
 
 Variables can be looked up using the `vault` plugin. This is done using standard Jinja2 syntax e.g;
 
 ```json
 {
   "name": "my_task",
```

### Comparing `otf_addons_vault-24.18.1/README.md` & `otf_addons_vault-24.18.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     "VAULT_ADDR": "https://vault.example.com:8200",
     "VAULT_TOKEN": "some_token"
 }
 ```
 
 If these variables are set in the environment, then these will be used if not set elsewhere.
 
+# Vault KV Secrets Engine Version
+
+The default version is v1. This can be overridden by setting the environment variable `VAULT_API_VER` to `v2` (or specifying the variable manually)
+
 # Variable Lookup
 
 Variables can be looked up using the `vault` plugin. This is done using standard Jinja2 syntax e.g;
 
 ```json
 {
   "name": "my_task",
```

### Comparing `otf_addons_vault-24.18.1/pyproject.toml` & `otf_addons_vault-24.18.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otf-addons-vault"
-version = "v24.18.1"
+version = "v24.18.2"
 authors = [{ name = "Adam McDonagh", email = "adam@elitemonkey.net" }]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX",
 ]
@@ -44,15 +44,15 @@
 "Bug Tracker" = "https://github.com/adammcdonagh/otf-addons-vault/issues"
 "Changelog" = "https://github.com/adammcdonagh/otf-addons-vault/blob/main/CHANGELOG.md"
 
 [tool.isort]
 profile = 'black'
 
 [tool.bumpver]
-current_version = "v24.18.1"
+current_version = "v24.18.2"
 version_pattern = "vYY.WW.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `otf_addons_vault-24.18.1/src/opentaskpy/plugins/lookup/hashicorp/vault.py` & `otf_addons_vault-24.18.2/src/opentaskpy/plugins/lookup/hashicorp/vault.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,32 +51,45 @@
     )
     vault_addr = (
         globals_["VAULT_ADDR"]
         if globals_ and "VAULT_ADDR" in globals_
         else os.environ.get("VAULT_ADDR")
     )
 
+    vault_api_version = (
+        globals_["VAULT_API_VER"]
+        if globals_ and "VAULT_API_VER" in globals_
+        else os.environ.get("VAULT_API_VER", "v1")
+    )
+
     result = None
     try:
         client = hvac.Client(
             url=vault_addr,
             token=vault_token,
         )
 
-        result = client.secrets.kv.v2.read_secret_version(
-            path=kwargs["key"],
-        )
-
         # Result will be some JSON, so parse it and if an attribute name is provided
         # return that value, else return the value attribute (if it exists, otherwise
         # raise an error)
         value_attribute = kwargs.get("attribute", "value")
-        result = result["data"]
-        if "data" in result and value_attribute in result["data"]:
-            result = result["data"][value_attribute]
+
+        if vault_api_version == "v1":
+            result = client.secrets.kv.v1.read_secret(
+                path=kwargs["key"],
+            )
+            result = result["data"]
+        else:
+            result = client.secrets.kv.v2.read_secret_version(
+                path=kwargs["key"],
+            )
+            result = result["data"]["data"]
+
+        if value_attribute in result:
+            result = result[value_attribute]
         else:
             raise FileNotFoundError(f"Secret not found: {kwargs['key']}")
 
         logger.log(12, f"Read '{result}' from secret {kwargs['key']}")
 
     except requests.exceptions.ConnectionError as e:
         logger.error(f"Error connecting to Hashicorp Vault: {e}")
@@ -93,14 +106,12 @@
 
     except Exception as e:
         logger.error(f"Error reading secret {kwargs['key']}: {e}")
         raise LookupPluginError("Error connecting to Hashicorp Vault")
 
     # Escape any escape characters so they can be stored in JSON as a string
     if result:
-        # Escape any newline characters
-        result = result.replace("\n", "\\n")
         result = json.dumps(result)
         # Remove the leading and trailing quotes
         result = result[1:-1]
 
     return result
```

### Comparing `otf_addons_vault-24.18.1/src/otf_addons_vault.egg-info/PKG-INFO` & `otf_addons_vault-24.18.2/src/otf_addons_vault.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otf-addons-vault
-Version: 24.18.1
+Version: 24.18.2
 Summary: Addons for opentaskpy, giving it the ability to read variables from Hashicorp Vault
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/otf-addons-vault
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/otf-addons-vault/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/otf-addons-vault/blob/main/CHANGELOG.md
 Keywords: automation,task,framework,hashicorp,vault,secrets,otf
@@ -59,14 +59,18 @@
     "VAULT_ADDR": "https://vault.example.com:8200",
     "VAULT_TOKEN": "some_token"
 }
 ```
 
 If these variables are set in the environment, then these will be used if not set elsewhere.
 
+# Vault KV Secrets Engine Version
+
+The default version is v1. This can be overridden by setting the environment variable `VAULT_API_VER` to `v2` (or specifying the variable manually)
+
 # Variable Lookup
 
 Variables can be looked up using the `vault` plugin. This is done using standard Jinja2 syntax e.g;
 
 ```json
 {
   "name": "my_task",
```

### Comparing `otf_addons_vault-24.18.1/tests/test_plugin_vault.py` & `otf_addons_vault-24.18.2/tests/test_plugin_vault.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,51 +42,81 @@
 
     with pytest.raises(FileNotFoundError) as ex:
         run(key="does_not_exist")
 
     assert ex.value.args[0] == f"Secret not found: does_not_exist"
 
 
-def test_vault_plugin(vault_service):
+def test_vault_plugin(vault_service_v1):
+    os.environ["VAULT_API_VER"] = "v1"
     expected = "test1234"
     # Populate the vault with a test value
-    vault_service.secrets.kv.v2.create_or_update_secret(
+    vault_service_v1.secrets.kv.v1.create_or_update_secret(
         path="some-secret",
         secret=dict(value=expected),
     )
 
     result = run(key="some-secret")
 
     assert result == expected
 
     expected = "mySecretPassword"
     # Insert a new secret, but use a different attribute name
-    vault_service.secrets.kv.v2.create_or_update_secret(
+    vault_service_v1.secrets.kv.v1.create_or_update_secret(
         path="some-secret-password",
         secret=dict(password=expected),
     )
 
     result = run(key="some-secret-password", attribute="password")
 
     assert result == expected
 
 
-def test_vault_lookup_attribute_missing(vault_service):
+def test_vault_plugin_v1(vault_service_v1):
+
+    os.environ["VAULT_API_VER"] = "v1"
+    expected = "test1234"
+    # Populate the vault with a test value
+    vault_service_v1.secrets.kv.v1.create_or_update_secret(
+        path="some-secret",
+        secret=dict(value=expected),
+    )
+
+    result = run(key="some-secret")
+
+    assert result == expected
+
+    expected = "mySecretPassword1"
+    # Insert a new secret, but use a different attribute name
+    vault_service_v1.secrets.kv.v1.create_or_update_secret(
+        path="some-secret-password1",
+        secret=dict(password=expected),
+    )
+
+    result = run(key="some-secret-password1", attribute="password")
+
+    del os.environ["VAULT_API_VER"]
+    assert result == expected
+
+
+def test_vault_lookup_attribute_missing(vault_service_v2):
+    os.environ["VAULT_API_VER"] = "v2"
     expected = "test1234"
     # Populate the vault with a test value
-    vault_service.secrets.kv.v2.create_or_update_secret(
+    vault_service_v2.secrets.kv.v2.create_or_update_secret(
         path="some-secret",
         secret=dict(value=expected),
     )
 
     with pytest.raises(FileNotFoundError) as ex:
         run(key="some-secret", attribute="does_not_exist")
 
 
-def test_config_loader_using_vault_plugin(vault_service, tmpdir):
+def test_config_loader_using_vault_plugin(vault_service_v1, tmpdir):
+    os.environ["VAULT_API_VER"] = "v1"
     json_obj = {
         "testLookup": "{{ lookup('hashicorp.vault', key='my_test_secret') }}",
     }
 
     fs.create_files(
         [
             {
@@ -95,28 +125,29 @@
                 }
             },
         ]
     )
     # Test with a multi line string to make sure that it doesn't break the parser
     expected = """config_loader_test_1234\\nanother_line"""
 
-    vault_service.secrets.kv.v2.create_or_update_secret(
+    vault_service_v1.secrets.kv.v1.create_or_update_secret(
         path="my_test_secret",
         secret=dict(value=expected),
     )
 
     # Test that the global variables are loaded correctly
     config_loader = ConfigLoader(tmpdir)
     config_loader._load_global_variables()
     config_loader._resolve_templated_variables()
 
     assert config_loader.get_global_variables()["testLookup"] == expected
 
 
-def test_config_loader_using_vault_plugin_custom_attribute(vault_service, tmpdir):
+def test_config_loader_using_vault_plugin_custom_attribute(vault_service_v1, tmpdir):
+    os.environ["VAULT_API_VER"] = "v1"
     json_obj = {
         "testLookup": "{{ lookup('hashicorp.vault', key='my_test_secret', attribute='password' ) }}",
     }
 
     fs.create_files(
         [
             {
@@ -125,15 +156,15 @@
                 }
             },
         ]
     )
     # Test with a multi line string to make sure that it doesn't break the parser
     expected = """some_random_password"""
 
-    vault_service.secrets.kv.v2.create_or_update_secret(
+    vault_service_v1.secrets.kv.v1.create_or_update_secret(
         path="my_test_secret",
         secret=dict(password=expected),
     )
 
     # Test that the global variables are loaded correctly
     config_loader = ConfigLoader(tmpdir)
     config_loader._load_global_variables()
```

