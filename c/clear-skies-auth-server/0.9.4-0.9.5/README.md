# Comparing `tmp/clear_skies_auth_server-0.9.4.tar.gz` & `tmp/clear_skies_auth_server-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_auth_server-0.9.4.tar", max compression
+gzip compressed data, was "clear_skies_auth_server-0.9.5.tar", max compression
```

## Comparing `clear_skies_auth_server-0.9.4.tar` & `clear_skies_auth_server-0.9.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1065 2023-04-03 23:13:07.715639 clear_skies_auth_server-0.9.4/LICENSE
--rw-r--r--   0        0        0     2070 2023-08-01 20:10:15.789699 clear_skies_auth_server-0.9.4/README.md
--rw-r--r--   0        0        0     1110 2023-08-27 13:45:36.459545 clear_skies_auth_server-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      152 2023-07-28 10:30:32.385807 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/__init__.py
--rw-r--r--   0        0        0       64 2023-06-11 11:04:47.143650 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/applications/__init__.py
--rw-r--r--   0        0        0     2024 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/applications/key_manager.py
--rw-r--r--   0        0        0      264 2023-07-23 12:00:28.807356 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/authentication/__init__.py
--rw-r--r--   0        0        0     2042 2023-07-29 19:48:46.333491 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/authentication/jwks_direct.py
--rw-r--r--   0        0        0      379 2023-07-20 20:45:09.680453 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/column_types/__init__.py
--rw-r--r--   0        0        0    12265 2023-07-20 01:48:22.054909 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/column_types/multi_tenant_configuration.py
--rw-r--r--   0        0        0     5011 2023-07-22 14:20:33.055474 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/column_types/password.py
--rw-r--r--   0        0        0     1904 2023-07-22 15:02:01.773222 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/column_types/tenant_id.py
--rw-r--r--   0        0        0      780 2023-07-28 21:35:59.261167 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/__init__.py
--rw-r--r--   0        0        0     1493 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/create_key.py
--rw-r--r--   0        0        0     1166 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/delete_key.py
--rw-r--r--   0        0        0     1090 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/delete_oldest_key.py
--rw-r--r--   0        0        0      597 2023-08-27 13:43:35.940926 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/jwks.py
--rw-r--r--   0        0        0     5263 2023-08-27 13:41:02.597253 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/key_base.py
--rw-r--r--   0        0        0      683 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/list_keys.py
--rw-r--r--   0        0        0        0 2023-04-04 23:17:41.819609 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/password_less_email_request_login.py
--rw-r--r--   0        0        0        0 2023-04-04 23:17:51.235652 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/password_less_validate_login.py
--rw-r--r--   0        0        0    19960 2023-08-27 13:44:19.517897 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/password_login.py
--rw-r--r--   0        0        0     5990 2023-07-29 19:48:46.457492 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/password_reset.py
--rw-r--r--   0        0        0     8588 2023-08-13 19:22:03.455029 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/password_reset_request.py
--rw-r--r--   0        0        0     1415 2023-07-28 17:15:08.379602 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/profile.py
--rw-r--r--   0        0        0    12749 2023-08-27 13:41:46.174342 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/switch_tenant.py
--rw-r--r--   0        0        0      793 2023-07-28 11:08:13.445657 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/input_requirements/__init__.py
--rw-r--r--   0        0        0      604 2023-07-18 11:19:05.147085 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/input_requirements/letters_digits.py
--rw-r--r--   0        0        0     1066 2023-07-18 11:19:05.147085 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/input_requirements/letters_digits_special_characters.py
--rw-r--r--   0        0        0     1654 2023-07-29 19:48:46.485492 clear_skies_auth_server-0.9.4/src/clearskies_auth_server/input_requirements/password_validation.py
--rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 clear_skies_auth_server-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-03 23:13:07.715639 clear_skies_auth_server-0.9.5/LICENSE
+-rw-r--r--   0        0        0     2070 2023-08-01 20:10:15.789699 clear_skies_auth_server-0.9.5/README.md
+-rw-r--r--   0        0        0     1110 2023-08-29 11:42:44.891153 clear_skies_auth_server-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      152 2023-07-28 10:30:32.385807 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-11 11:04:47.143650 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/applications/__init__.py
+-rw-r--r--   0        0        0     2024 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/applications/key_manager.py
+-rw-r--r--   0        0        0      264 2023-07-23 12:00:28.807356 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/authentication/__init__.py
+-rw-r--r--   0        0        0     2042 2023-07-29 19:48:46.333491 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/authentication/jwks_direct.py
+-rw-r--r--   0        0        0      379 2023-07-20 20:45:09.680453 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/column_types/__init__.py
+-rw-r--r--   0        0        0    12265 2023-07-20 01:48:22.054909 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/column_types/multi_tenant_configuration.py
+-rw-r--r--   0        0        0     5011 2023-07-22 14:20:33.055474 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/column_types/password.py
+-rw-r--r--   0        0        0     1904 2023-07-22 15:02:01.773222 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/column_types/tenant_id.py
+-rw-r--r--   0        0        0      780 2023-07-28 21:35:59.261167 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/__init__.py
+-rw-r--r--   0        0        0     1493 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/create_key.py
+-rw-r--r--   0        0        0     1166 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/delete_key.py
+-rw-r--r--   0        0        0     1090 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/delete_oldest_key.py
+-rw-r--r--   0        0        0      597 2023-08-27 13:43:35.940926 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/jwks.py
+-rw-r--r--   0        0        0     5263 2023-08-27 13:41:02.597253 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/key_base.py
+-rw-r--r--   0        0        0      683 2023-07-18 11:19:05.143086 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/list_keys.py
+-rw-r--r--   0        0        0        0 2023-04-04 23:17:41.819609 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/password_less_email_request_login.py
+-rw-r--r--   0        0        0        0 2023-04-04 23:17:51.235652 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/password_less_validate_login.py
+-rw-r--r--   0        0        0    20190 2023-08-29 11:43:04.407237 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/password_login.py
+-rw-r--r--   0        0        0     5990 2023-07-29 19:48:46.457492 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/password_reset.py
+-rw-r--r--   0        0        0     8588 2023-08-13 19:22:03.455029 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/password_reset_request.py
+-rw-r--r--   0        0        0     1415 2023-07-28 17:15:08.379602 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/profile.py
+-rw-r--r--   0        0        0    12749 2023-08-27 13:41:46.174342 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/switch_tenant.py
+-rw-r--r--   0        0        0      793 2023-07-28 11:08:13.445657 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/input_requirements/__init__.py
+-rw-r--r--   0        0        0      604 2023-07-18 11:19:05.147085 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/input_requirements/letters_digits.py
+-rw-r--r--   0        0        0     1066 2023-07-18 11:19:05.147085 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/input_requirements/letters_digits_special_characters.py
+-rw-r--r--   0        0        0     1654 2023-07-29 19:48:46.485492 clear_skies_auth_server-0.9.5/src/clearskies_auth_server/input_requirements/password_validation.py
+-rw-r--r--   0        0        0     3101 1970-01-01 00:00:00.000000 clear_skies_auth_server-0.9.5/PKG-INFO
```

### Comparing `clear_skies_auth_server-0.9.4/LICENSE` & `clear_skies_auth_server-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/README.md` & `clear_skies_auth_server-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/pyproject.toml` & `clear_skies_auth_server-0.9.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-auth-server"
-version = "0.9.4"
+version = "0.9.5"
 description = "clearskies bindings for managing an authentication server that issues JWTs"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
 ]
 repository = "https://github.com/cmancone/clearskies-auth-server"
 license = "MIT"
 readme = "./README.md"
```

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/applications/key_manager.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/applications/key_manager.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/authentication/jwks_direct.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/authentication/jwks_direct.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/column_types/multi_tenant_configuration.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/column_types/multi_tenant_configuration.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/column_types/password.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/column_types/password.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/column_types/tenant_id.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/column_types/tenant_id.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/__init__.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/create_key.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/create_key.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/delete_key.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/delete_key.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/delete_oldest_key.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/delete_oldest_key.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/jwks.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/jwks.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/key_base.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/key_base.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/list_keys.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/list_keys.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/password_login.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/password_login.py`

 * *Files 6% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         users = self.users
         if self.configuration("tenant_id_column_name"):
             tenant_id_column_name = self.configuration("tenant_id_column_name")
             tenant_id_source_key_name = self.configuration("tenant_id_source_key_name")
             if self.configuration("tenant_id_source") == "routing_data":
                 tenant_id_value = input_output.routing_data().get(tenant_id_source_key_name)
             if not tenant_id_value:
-                return self.error(input_output, "Invalid username/password combination", 404)
+                return self.input_errors(input_output, {username_column_name: "Invalid username/password combination"})
             users = users.where(f"{tenant_id_column_name}={tenant_id_value}")
         username = request_data[username_column_name]
         user = users.find(f"{username_column_name}={username}")
         audit_overrides = self.configuration("audit_overrides")
         audit_extra_data_unmapped = {
             "username": username,
             "user_id": user.get(user.id_column_name),
@@ -237,56 +237,58 @@
         }
         audit_extra_data = {}
         for key, value in audit_overrides.items():
             audit_extra_data[value] = audit_extra_data_unmapped[key]
 
         # no user found
         if not user.exists:
-            return self.error(input_output, "Invalid username/password combination", 404)
+            return self.input_errors(input_output, {username_column_name: "Invalid username/password combination"})
 
         # account lockout
         if self.account_locked(user):
             self.audit(
                 user,
                 self.configuration("audit_action_name_account_locked"),
                 data={
                     "reason": "Account Locked",
                     **audit_extra_data,
                 },
             )
             minutes = self.configuration("account_lockout_failed_attempts_threshold")
-            return self.error(
+            s = "s" if int(minutes) != 1 else ""
+            return self.input_errors(
                 input_output,
-                f"Your account us under a {minutes} minute lockout due to too many failed login attempts",
-                404,
+                {
+                    username_column_name: f"Your account is under a {minutes}{s} minute lockout due to too many failed login attempts"
+                },
             )
 
         # password not set
         if not user.get(password_column_name):
             self.audit(
                 user,
                 self.configuration("audit_action_name_failed_login"),
                 data={
                     "reason": "Password not set - user is not configured for password login",
                     **audit_extra_data,
                 },
             )
-            return self.error(input_output, "Invalid username/password combination", 404)
+            return self.input_errors(input_output, {username_column_name: "Invalid username/password combination"})
 
         # invalid password
         if not password_column.validate_password(user, request_data[password_column_name]):
             self.audit(
                 user,
                 self.configuration("audit_action_name_failed_login"),
                 data={
                     "reason": "Invalid password",
                     **audit_extra_data,
                 },
             )
-            return self.error(input_output, "Invalid username/password combination", 404)
+            return self.input_errors(input_output, {username_column_name: "Invalid username/password combination"})
 
         # developer-defined checks
         login_check_callables = self.configuration("login_check_callables")
         if login_check_callables:
             for login_check_callable in login_check_callables:
                 response = self._di.call_function(
                     login_check_callable,
@@ -301,15 +303,15 @@
                         user,
                         self.configuration("audit_action_name_failed_login"),
                         data={
                             "reason": response,
                             **audit_extra_data,
                         },
                     )
-                    return self.error(input_output, response, 404)
+                    return self.input_errors(input_output, {username_column_name: response})
 
         self.audit(user, self.configuration("audit_action_name_successful_login"), data=audit_extra_data)
         signing_key = self.get_youngest_private_key(self.configuration("path_to_private_keys"), as_json=False)
         jwt_claims = self.get_jwt_claims(user)
         token = jwt.JWT(header={"alg": "RS256", "typ": "JWT", "kid": signing_key["kid"]}, claims=jwt_claims)
         token.make_signed_token(signing_key)
```

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/password_reset.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/password_reset.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/password_reset_request.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/password_reset_request.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/profile.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/profile.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/handlers/switch_tenant.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/handlers/switch_tenant.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/input_requirements/__init__.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/input_requirements/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/input_requirements/letters_digits.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/input_requirements/letters_digits.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/input_requirements/letters_digits_special_characters.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/input_requirements/letters_digits_special_characters.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/src/clearskies_auth_server/input_requirements/password_validation.py` & `clear_skies_auth_server-0.9.5/src/clearskies_auth_server/input_requirements/password_validation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_auth_server-0.9.4/PKG-INFO` & `clear_skies_auth_server-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-auth-server
-Version: 0.9.4
+Version: 0.9.5
 Summary: clearskies bindings for managing an authentication server that issues JWTs
 Home-page: https://github.com/cmancone/clearskies-auth-server
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

