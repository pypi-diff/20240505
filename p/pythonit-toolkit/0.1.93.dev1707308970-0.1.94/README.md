# Comparing `tmp/pythonit_toolkit-0.1.93.dev1707308970.tar.gz` & `tmp/pythonit_toolkit-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonit_toolkit-0.1.93.dev1707308970.tar", max compression
+gzip compressed data, was "pythonit_toolkit-0.1.94.tar", max compression
```

## Comparing `pythonit_toolkit-0.1.93.dev1707308970.tar` & `pythonit_toolkit-0.1.94.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1070 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/LICENSE
--rw-r--r--   0        0        0      763 2024-02-07 12:29:30.862344 pythonit_toolkit-0.1.93.dev1707308970/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/api/__init__.py
--rw-r--r--   0        0        0      854 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/api/builder.py
--rw-r--r--   0        0        0      386 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/api/extensions.py
--rw-r--r--   0        0        0     2472 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/api/graphql_test_client.py
--rw-r--r--   0        0        0     1618 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/api/permissions.py
--rw-r--r--   0        0        0      196 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/api/types.py
--rw-r--r--   0        0        0       70 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/backends/__init__.py
--rw-r--r--   0        0        0      535 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/backends/base.py
--rw-r--r--   0        0        0      866 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/backends/local.py
--rw-r--r--   0        0        0     1371 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/backends/ses.py
--rw-r--r--   0        0        0      917 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/templates.py
--rw-r--r--   0        0        0      893 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/utils.py
--rw-r--r--   0        0        0      127 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/headers/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/pastaporto/__init__.py
--rw-r--r--   0        0        0     1065 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/pastaporto/actions.py
--rw-r--r--   0        0        0     1794 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/pastaporto/entities.py
--rw-r--r--   0        0        0      167 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/pastaporto/exceptions.py
--rw-r--r--   0        0        0     1026 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/pastaporto/test.py
--rw-r--r--   0        0        0     1046 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/pastaporto/tokens.py
--rw-r--r--   0        0        0        0 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/sentry/__init__.py
--rw-r--r--   0        0        0      437 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/sentry/sentry.py
--rw-r--r--   0        0        0      129 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/service_client/__init__.py
--rw-r--r--   0        0        0     1680 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/service_client/client.py
--rw-r--r--   0        0        0        0 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/starlette_backend/__init__.py
--rw-r--r--   0        0        0      422 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/starlette_backend/middleware.py
--rw-r--r--   0        0        0     1471 2024-02-07 12:29:21.250424 pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/starlette_backend/pastaporto_backend.py
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 pythonit_toolkit-0.1.93.dev1707308970/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/LICENSE
+-rw-r--r--   0        0        0      748 2024-05-05 21:17:39.842895 pythonit_toolkit-0.1.94/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/api/__init__.py
+-rw-r--r--   0        0        0      854 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/api/builder.py
+-rw-r--r--   0        0        0      386 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/api/extensions.py
+-rw-r--r--   0        0        0     2472 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/api/graphql_test_client.py
+-rw-r--r--   0        0        0     1618 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/api/permissions.py
+-rw-r--r--   0        0        0      196 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/api/types.py
+-rw-r--r--   0        0        0       70 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/emails/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/emails/backends/__init__.py
+-rw-r--r--   0        0        0      542 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/emails/backends/base.py
+-rw-r--r--   0        0        0      935 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/emails/backends/local.py
+-rw-r--r--   0        0        0     1426 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/emails/backends/ses.py
+-rw-r--r--   0        0        0      917 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/emails/templates.py
+-rw-r--r--   0        0        0      893 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/emails/utils.py
+-rw-r--r--   0        0        0      127 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/headers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/pastaporto/__init__.py
+-rw-r--r--   0        0        0     1065 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/pastaporto/actions.py
+-rw-r--r--   0        0        0     1794 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/pastaporto/entities.py
+-rw-r--r--   0        0        0      167 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/pastaporto/exceptions.py
+-rw-r--r--   0        0        0     1026 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/pastaporto/test.py
+-rw-r--r--   0        0        0     1046 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/pastaporto/tokens.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/sentry/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/sentry/sentry.py
+-rw-r--r--   0        0        0      129 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/service_client/__init__.py
+-rw-r--r--   0        0        0     1680 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/service_client/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/starlette_backend/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/starlette_backend/middleware.py
+-rw-r--r--   0        0        0     1471 2024-05-05 21:17:32.094841 pythonit_toolkit-0.1.94/pythonit_toolkit/starlette_backend/pastaporto_backend.py
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 pythonit_toolkit-0.1.94/PKG-INFO
```

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/LICENSE` & `pythonit_toolkit-0.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pyproject.toml` & `pythonit_toolkit-0.1.94/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythonit-toolkit"
-version = "0.1.93-dev.1707308970"
+version = "0.1.94"
 description = ""
 authors = ["Python Italia"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
 PyJWT = "^2.8.0"
 starlette = { version = "^0.30.0", optional = true }
```

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/api/builder.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/api/builder.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/api/graphql_test_client.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/api/graphql_test_client.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/api/permissions.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/api/permissions.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/backends/base.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/emails/backends/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,9 +14,9 @@
         *,
         template: EmailTemplate,
         subject: str,
         from_: str,
         to: str,
         variables: Optional[Dict[str, str]] = None,
         reply_to: List[str] = None
-    ):
+    ) -> str:
         pass
```

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/backends/local.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/emails/backends/local.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Dict, List, Optional
+from uuid import uuid4
 
 from pythonit_toolkit.emails.templates import EmailTemplate
 
 from .base import EmailBackend
 
 
 class LocalEmailBackend(EmailBackend):
@@ -14,18 +15,20 @@
         *,
         template: EmailTemplate,
         subject: str,
         from_: str,
         to: str,
         variables: Optional[Dict[str, str]] = None,
         reply_to: List[str] = None,
-    ):
+    ) -> str:
         reply_to = reply_to or []
 
         print("=== Email sending ===")
         print(f"Template: {template}")
         print(f"From: {from_}")
         print(f"To: {to}")
         print(f"Subject: {subject}")
         print(f"Variables: {str(variables)}")
         print(f"Reply to: {str(reply_to)}")
         print("=== End Email sending ===")
+
+        return f'messageid-{uuid4()}'
```

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/backends/ses.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/emails/backends/ses.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,26 +18,27 @@
         *,
         template: EmailTemplate,
         subject: str,
         from_: str,
         to: str,
         variables: Optional[Dict[str, str]] = None,
         reply_to: List[str] = None,
-    ):
+    ) -> str:
         reply_to = reply_to or []
 
         variables = self.encode_vars({"subject": subject, **(variables or {})})
-        self.ses.send_templated_email(
+        response = self.ses.send_templated_email(
             Source=from_,
             Destination={"ToAddresses": [to]},
             Template=f"pythonit-{self.environment}-{template}",
             TemplateData=json.dumps(variables),
             ReplyToAddresses=reply_to,
             ConfigurationSetName='primary',
         )
+        return response['MessageId']
 
     def encode_vars(self, variables: dict[str, Any]) -> dict[str, Any]:
         vars = dict()
 
         for key, value in variables.items():
             if isinstance(value, str) and not isinstance(value, SafeString):
                 value = html.escape(value)
```

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/templates.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/emails/templates.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/emails/utils.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/emails/utils.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/pastaporto/actions.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/pastaporto/actions.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/pastaporto/entities.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/pastaporto/entities.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/pastaporto/test.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/pastaporto/test.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/pastaporto/tokens.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/pastaporto/tokens.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/service_client/client.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/service_client/client.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/pythonit_toolkit/starlette_backend/pastaporto_backend.py` & `pythonit_toolkit-0.1.94/pythonit_toolkit/starlette_backend/pastaporto_backend.py`

 * *Files identical despite different names*

### Comparing `pythonit_toolkit-0.1.93.dev1707308970/PKG-INFO` & `pythonit_toolkit-0.1.94/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonit-toolkit
-Version: 0.1.93.dev1707308970
+Version: 0.1.94
 Summary: 
 Author: Python Italia
 Requires-Python: >=3.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

