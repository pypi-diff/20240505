# Comparing `tmp/shcheck-1.5.9.tar.gz` & `tmp/shcheck-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shcheck-1.5.9.tar", last modified: Fri Apr 14 09:16:11 2023, max compression
+gzip compressed data, was "shcheck-1.6.tar", last modified: Sun May  5 10:44:26 2024, max compression
```

## Comparing `shcheck-1.5.9.tar` & `shcheck-1.6.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:16:11.345353 shcheck-1.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-14 09:16:00.000000 shcheck-1.5.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-14 09:16:11.345353 shcheck-1.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-14 09:16:00.000000 shcheck-1.5.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:16:11.345353 shcheck-1.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-14 09:16:00.000000 shcheck-1.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:16:11.345353 shcheck-1.5.9/shcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-14 09:16:11.000000 shcheck-1.5.9/shcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-14 09:16:11.000000 shcheck-1.5.9/shcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:16:11.000000 shcheck-1.5.9/shcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 09:16:11.000000 shcheck-1.5.9/shcheck.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    14346 2023-04-14 09:16:00.000000 shcheck-1.5.9/shcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:44:26.335228 shcheck-1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-05 10:44:22.000000 shcheck-1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-05 10:44:26.335228 shcheck-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-05 10:44:22.000000 shcheck-1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:44:26.335228 shcheck-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-05 10:44:22.000000 shcheck-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:44:26.331228 shcheck-1.6/shcheck/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:44:22.000000 shcheck-1.6/shcheck/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16301 2024-05-05 10:44:22.000000 shcheck-1.6/shcheck/shcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:44:26.335228 shcheck-1.6/shcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-05 10:44:26.000000 shcheck-1.6/shcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-05 10:44:26.000000 shcheck-1.6/shcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:44:26.000000 shcheck-1.6/shcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 10:44:26.000000 shcheck-1.6/shcheck.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      818 2024-05-05 10:44:22.000000 shcheck-1.6/shcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:44:26.335228 shcheck-1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-05 10:44:22.000000 shcheck-1.6/tests/test_shcheck.py
```

### Comparing `shcheck-1.5.9/LICENSE.txt` & `shcheck-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shcheck-1.5.9/PKG-INFO` & `shcheck-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shcheck
-Version: 1.5.9
+Version: 1.6
 Summary: A basic tool to check security headers of a website
 Home-page: https://github.com/santoru/shcheck
 Author: santoru
 Author-email: santoru@pm.me
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: shcheck Version: 1.5.9 Summary: A basic tool to
-check security headers of a website Home-page: https://github.com/santoru/
-shcheck Author: santoru Author-email: santoru@pm.me Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE.txt # shcheck -
-Security Header Check
+Metadata-Version: 2.1 Name: shcheck Version: 1.6 Summary: A basic tool to check
+security headers of a website Home-page: https://github.com/santoru/shcheck
+Author: santoru Author-email: santoru@pm.me Requires-Python: >=3 Description-
+Content-Type: text/markdown License-File: LICENSE.txt # shcheck - Security
+Header Check
                    _[_P_y_P_I_]_[_P_y_p_i_]_[_U_p_d_a_t_e_d_][Output on Facebook]
 ## Check security headers on a target website I did this tool to help me to
 check which security headers are enabled on certain websites. The tool is very
 simple and it's the result of few minutes of coding. It just check headers and
 print a report about which are enabled and which not I think there is a lot to
 improve, and I will be grateful if somebody wants to help ## How to run: ###
 Pypi ```bash pip3 install shcheck shcheck.py https://insecurity.blog ``` ###
```

### Comparing `shcheck-1.5.9/README.md` & `shcheck-1.6/README.md`

 * *Files identical despite different names*

### Comparing `shcheck-1.5.9/setup.py` & `shcheck-1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import setup
 
 PACKAGE_NAME = "shcheck"
-VERSION = "1.5.9"
+VERSION = "1.6"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def parse_requirements(filename):
     """Load requirements from a pip requirements file."""
```

### Comparing `shcheck-1.5.9/shcheck.egg-info/PKG-INFO` & `shcheck-1.6/shcheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shcheck
-Version: 1.5.9
+Version: 1.6
 Summary: A basic tool to check security headers of a website
 Home-page: https://github.com/santoru/shcheck
 Author: santoru
 Author-email: santoru@pm.me
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: shcheck Version: 1.5.9 Summary: A basic tool to
-check security headers of a website Home-page: https://github.com/santoru/
-shcheck Author: santoru Author-email: santoru@pm.me Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE.txt # shcheck -
-Security Header Check
+Metadata-Version: 2.1 Name: shcheck Version: 1.6 Summary: A basic tool to check
+security headers of a website Home-page: https://github.com/santoru/shcheck
+Author: santoru Author-email: santoru@pm.me Requires-Python: >=3 Description-
+Content-Type: text/markdown License-File: LICENSE.txt # shcheck - Security
+Header Check
                    _[_P_y_P_I_]_[_P_y_p_i_]_[_U_p_d_a_t_e_d_][Output on Facebook]
 ## Check security headers on a target website I did this tool to help me to
 check which security headers are enabled on certain websites. The tool is very
 simple and it's the result of few minutes of coding. It just check headers and
 print a report about which are enabled and which not I think there is a lot to
 improve, and I will be grateful if somebody wants to help ## How to run: ###
 Pypi ```bash pip3 install shcheck shcheck.py https://insecurity.blog ``` ###
```

### Comparing `shcheck-1.5.9/shcheck.py` & `shcheck-1.6/shcheck/shcheck.py`

 * *Files 16% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         else:
             print("Target host {} seems to be unreachable ({})".format(target, e.reason))
 
     else:
         print("{}".format(str(e)))
 
 
-def check_target(target, options):
+def check_target(target):
     '''
     Just put a protocol to a valid IP and check if connection works,
     returning HEAD response
     '''
     # Recover used options
     ssldisabled = options.ssldisabled
     useget = options.useget
@@ -211,18 +211,18 @@
     try:
         response = urllib.request.urlopen(request, timeout=10)
 
     # Handling issues with HTTP/2
     except http.client.UnknownProtocol as e:
         print("Unknown protocol: {}. Are you using a proxy? Try disabling it".format(e))
     except Exception as e:
-        if hasattr(e, 'code') and e.code == 404:
+        print_error(target, e)
+        if hasattr(e, 'code') and e.code >= 400 and e.code < 500:
             response = e
         else:
-            print_error(target, e)
             return None
 
     if response is not None:
         return response
     print("Couldn't read a response from server.")
     return None
 
@@ -238,18 +238,32 @@
     log("-------------------------------------------------------")
     log("[!] Headers analyzed for {}".format(colorize(target, 'info')))
     log("[+] There are {} security headers".format(colorize(str(safe), 'ok')))
     log("[-] There are not {} security headers".format(
         colorize(str(unsafe), 'error')))
     log("")
 
+def parse_csp(csp):
+    unsafe_operators = ['unsafe-inline', 'unsafe-eval', 'unsafe-hashes', 'wasm-unsafe-eval', 'self']
+    log("Value:")
+    policy_directive = csp.split(";")
+    for policy in policy_directive:
+        elements = policy.lstrip().split(" ", 1)
+
+        values = elements[1].replace("*", colorize("*", 'warning')) if len(elements) > 1 else ""
+        for x in unsafe_operators:
+            values = values.replace(x, colorize(x, 'error'))
+        log("\t" + colorize(elements[0], 'info') + (": " + values if values != "" else ""))
 
-def main(options, targets):
 
+def main():
     # Getting options
+    global options
+    options, targets = parse_options()
+
     port = options.port
     cookie = options.cookie
     custom_headers = options.custom_headers
     information = options.information
     cache_control = options.cache_control
     show_deprecated = options.show_deprecated
     hfile = options.hfile
@@ -287,52 +301,76 @@
         json_headers = {}
         if port is not None:
             target = append_port(target, port)
 
         safe = 0
         unsafe = 0
 
+        log("[*] Analyzing headers of {}".format(colorize(target, 'info')))
+
         # Check if target is valid
-        response = check_target(target, options)
+        response = check_target(target)
         if not response:
             continue
         rUrl = response.geturl()
         json_results = {}
 
-        log("[*] Analyzing headers of {}".format(colorize(target, 'info')))
         log("[*] Effective URL: {}".format(colorize(rUrl, 'info')))
         parse_headers(response.getheaders())
         json_headers[f"{rUrl}"] = json_results
         json_results["present"] = {}
         json_results["missing"] = []
 
+        # Before parsing, remove X-Frame-Options if there's CSP with frame-ancestors directive
+        if "frame-ancestors" in headers.get('Content-Security-Policy'.lower()).lower():
+            sec_headers.pop("X-Frame-Options")
+            headers.pop("X-Frame-Options".lower())
+
         for safeh in sec_headers:
             lsafeh = safeh.lower()
             if lsafeh in headers:
                 safe += 1
                 json_results["present"][safeh] = headers.get(lsafeh)
 
                 # Taking care of special headers that could have bad values
 
+                # Parse CSP headers
+                if lsafeh == 'Content-Security-Policy'.lower():
+                    log("[*] Header {} is present!".format(
+                            colorize(safeh, 'ok')))
+                    parse_csp(headers.get(lsafeh))
+
                 # X-XSS-Protection Should be enabled
-                if safeh == 'X-XSS-Protection' and headers.get(lsafeh) == '0':
+                elif lsafeh == 'X-XSS-Protection'.lower() and headers.get(lsafeh) == '0':
                     log("[*] Header {} is present! (Value: {})".format(
                             colorize(safeh, 'ok'),
                             colorize(headers.get(lsafeh), 'warning')))
 
+                # unsafe-url policy is more insecure compared to the default/unset value
+                elif lsafeh == 'Referrer-Policy'.lower() and headers.get(lsafeh) == 'unsafe-url':
+                    log("[!] Insecure header {} is set! (Value: {})".format(
+                            colorize(safeh, 'warning'),
+                            colorize(headers.get(lsafeh), 'error')))
+
+                # check for max-age=0 in HSTS
+                elif lsafeh == 'Strict-Transport-Security'.lower() and "max-age=0" in headers.get(lsafeh):
+                    log("[!] Insecure header {} is set! (Value: {})".format(
+                            colorize(safeh, 'warning'),
+                            colorize(headers.get(lsafeh), 'error')))
+
                 # Printing generic message if not specified above
                 else:
                     log("[*] Header {} is present! (Value: {})".format(
                             colorize(safeh, 'ok'),
                             headers.get(lsafeh)))
             else:
                 unsafe += 1
                 json_results["missing"].append(safeh)
                 # HSTS works obviously only on HTTPS
-                if safeh == 'Strict-Transport-Security' and not is_https(rUrl):
+                if safeh == 'Strict-Transport-Security'.lower() and not is_https(rUrl):
                     unsafe -= 1
                     json_results["missing"].remove(safeh)
                     continue
                 # Hide deprecated
                 if not show_deprecated and sec_headers.get(safeh) == "deprecated":
                     unsafe -= 1
                     json_results["missing"].remove(safeh)            
@@ -362,30 +400,30 @@
             log("")
             for cacheh in cache_headers:
                 lcacheh = cacheh.lower()
                 if lcacheh in headers:
                     json_headers["caching"][cacheh] = headers.get(lcacheh)
                     c_chk = True
                     log("[!] Cache control header {} is present! \
-Value: {})".format(
+(Value: {})".format(
                             colorize(cacheh, 'info'),
                             headers.get(lcacheh)))
             if not c_chk:
                 log("[*] No caching headers detected")
 
         report(rUrl, safe, unsafe)
         json_out.update(json_headers)
 
     if json_output:
         sys.stdout = sys.__stdout__
         print(json.dumps(json_out))
 
 
-if __name__ == "__main__":
 
+def parse_options():
     parser = OptionParser("Usage: %prog [options] <target>", prog=sys.argv[0])
 
     parser.add_option("-p", "--port", dest="port",
                       help="Set a custom port to connect to",
                       metavar="PORT")
     parser.add_option("-c", "--cookie", dest="cookie",
                       help="Set cookies for the request",
@@ -420,13 +458,17 @@
                       help="Load a list of hosts from a flat file",
                       metavar="PATH_TO_FILE")
     parser.add_option("--colours", dest="colours",
                       help="Set up a colour profile [dark/light/none]",
                       default="dark")
     parser.add_option("--colors", dest="colours",
                       help="Alias for colours for US English")
-    (options, args) = parser.parse_args()
+    (options, targets) = parser.parse_args()
 
-    if len(args) < 1 and options.hfile is None:
+    if len(targets) < 1 and options.hfile is None:
         parser.print_help()
-        sys.exit(1)
-    main(options, args)
+        sys.exit(12)
+
+    return options, targets
+
+if __name__ == "__main__":
+    main(sys.argv[0])
```

