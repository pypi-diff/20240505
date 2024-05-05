# Comparing `tmp/bypass_url_parser-0.4.1.tar.gz` & `tmp/bypass_url_parser-0.4.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bypass_url_parser-0.4.1.tar", last modified: Sat Mar  2 19:44:21 2024, max compression
+gzip compressed data, was "bypass_url_parser-0.4.2a0.tar", last modified: Sun May  5 16:40:05 2024, max compression
```

## Comparing `bypass_url_parser-0.4.1.tar` & `bypass_url_parser-0.4.2a0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    34523 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/LICENSE
--rw-r--r--   0        0        0    24583 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/README.md
--rw-r--r--   0        0        0     2232 2024-03-02 19:44:21.606186 bypass_url_parser-0.4.1/pyproject.toml
--rwxr-xr-x   0        0        0    98403 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/__init__.py
--rw-r--r--   0        0        0       22 2024-03-02 19:44:21.606186 bypass_url_parser-0.4.1/src/bypass_url_parser/_version.py
--rw-r--r--   0        0        0       55 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/header_http_methods.lst
--rw-r--r--   0        0        0     1917 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/header_ip_hosts.lst
--rw-r--r--   0        0        0       89 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/header_ports.lst
--rw-r--r--   0        0        0      172 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/header_proto_schemes.lst
--rw-r--r--   0        0        0      514 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/header_urls.lst
--rw-r--r--   0        0        0      192 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/internal_endpaths.lst
--rw-r--r--   0        0        0      259 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/internal_http_methods.lst
--rw-r--r--   0        0        0      105 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/internal_ip_hosts.lst
--rw-r--r--   0        0        0     3559 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/internal_midpaths.lst
--rw-r--r--   0        0        0       63 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/internal_ports.lst
--rw-r--r--   0        0        0       26 2024-03-02 19:43:58.457952 bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/internal_proto_schemes.lst
--rw-r--r--   0        0        0    25855 1970-01-01 00:00:00.000000 bypass_url_parser-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/LICENSE
+-rw-r--r--   0        0        0    23486 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/README.md
+-rw-r--r--   0        0        0     2500 2024-05-05 16:40:05.606028 bypass_url_parser-0.4.2a0/pyproject.toml
+-rwxr-xr-x   0        0        0   102735 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-05 16:40:05.606028 bypass_url_parser-0.4.2a0/src/bypass_url_parser/_version.py
+-rw-r--r--   0        0        0       55 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/header_http_methods.lst
+-rw-r--r--   0        0        0     1917 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/header_ip_hosts.lst
+-rw-r--r--   0        0        0       89 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/header_ports.lst
+-rw-r--r--   0        0        0      172 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/header_proto_schemes.lst
+-rw-r--r--   0        0        0      514 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/header_urls.lst
+-rw-r--r--   0        0        0      223 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/internal_endpaths.lst
+-rw-r--r--   0        0        0      259 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/internal_http_methods.lst
+-rw-r--r--   0        0        0      105 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/internal_ip_hosts.lst
+-rw-r--r--   0        0        0     3561 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/internal_midpaths.lst
+-rw-r--r--   0        0        0       63 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/internal_ports.lst
+-rw-r--r--   0        0        0       26 2024-05-05 16:39:39.822068 bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/internal_proto_schemes.lst
+-rw-r--r--   0        0        0        0 2024-05-05 16:39:39.830068 bypass_url_parser-0.4.2a0/tests/__init__.py
+-rw-r--r--   0        0        0     1042 2024-05-05 16:39:39.830068 bypass_url_parser-0.4.2a0/tests/test_smoke_tests.py
+-rw-r--r--   0        0        0    24760 1970-01-01 00:00:00.000000 bypass_url_parser-0.4.2a0/PKG-INFO
```

### Comparing `bypass_url_parser-0.4.1/LICENSE` & `bypass_url_parser-0.4.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `bypass_url_parser-0.4.1/README.md` & `bypass_url_parser-0.4.2a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1
+Name: bypass-url-parser
+Version: 0.4.2a0
+Summary: Default template for PDM package
+Keywords: security
+Author-Email: Laluka <loukajc@gmail.com>, jtof_fap <jtof_fap@insecurity.fr>, Gabriel Dugny <pypi@dugny.me>
+License: AGPL-3.0-or-later
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Classifier: Typing :: Typed
+Classifier: Topic :: Security
+Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Project-URL: Repository, https://github.com/laluka/bypass-url-parser
+Project-URL: Changelog, https://github.com/laluka/bypass-url-parser/releases
+Requires-Python: >=3.8
+Requires-Dist: coloredlogs==15.0.1
+Requires-Dist: docopt==0.6.2
+Description-Content-Type: text/markdown
+
 # Bypass Url Parser
 
 [![PyPI - Version](https://img.shields.io/pypi/v/bypass-url-parser)](https://pypi.org/project/bypass-url-parser/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bypass-url-parser)](https://pypi.org/project/bypass-url-parser/) [![PyPI - License](https://img.shields.io/pypi/l/bypass-url-parser)](https://github.com/laluka/bypass-url-parser/blob/main/LICENSE) [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 Tool that tests `MANY` url bypasses to reach a `40X protected page`.
 
 If you wonder why this code is `nothing but a dirty curl wrapper`, here's why:
@@ -35,28 +64,28 @@
 
 ```
 Bypass Url Parser, made with love by @TheLaluka
 A tool that tests MANY url bypasses to reach a 40X protected page.
 
 Usage:
     bypass-url-parser (-u <URL> | -R <file>) [-m <mode>] [-o <outdir>] [-S <level>] [ (-H <header>)...] [-r <num>]
-                           [-s <ip>] [--spoofip-replace] [-p <port>] [--spoofport-replace] [--request-tls]
-                           [--dump-payloads] [-t <threads>] [-T <timeout>] [-x <proxy_url>] [-v | -d | -dd]
+                      [-s <ip>] [--spoofip-replace] [-p <port>] [--spoofport-replace] [-t <threads>] [-T <timeout>]
+                      [--request-tls] [--jsonl] [--dump-payloads] [-x <proxy_url>] [-v | -d | -dd]
 
 Program options:
     -u, --url <URL>           URL (path is optional) to run bypasses against
     -R, --request <file>      Load HTTP raw request from a file
     -H, --header <header>     Header(s) to use, format: "Cookie: can_i_haz=fire"
     -m, --mode <mode>         Bypass modes. See 'Bypasser.BYPASS_MODES' in code [Default: all]
     -o, --outdir <outdir>     Output directory for results
     -x, --proxy <proxy_url>   Set a proxy in the format http://proxy_ip:port.
-    -S, --save-level <level>  Save results level. From 0 (DISABLE) to 3 (FULL) [Default: 1]
+    -S, --save-level <level>  Save results level. From 0 (DISABLE) to 3 (FULL) [Default: 2]
     -s, --spoofip <ip>        IP(s) to inject in ip-specific headers
     -p, --spoofport <port>    Port(s) to inject in port-specific headers
-    -r, --retry <num>         Retry attempts of failed requests. Set 0 to disable all retry tentatives [Default: 3]
+    -r, --retry <num>         Retry attempts of failed requests. Set 0 to disable all retry tentatives [Default: 1]
     -t, --threads <threads>   Scan with N parallel threads [Default: 1]
     -T, --timeout <timeout>   Request times out after N seconds [Default: 5]
 
 General options:
     -h, --help                Show help, you are here :)
     -v, --verbose             Verbose output
     -d, --debug               Show more details like curl commands generated by this tool
@@ -64,14 +93,15 @@
     -V, --version             Show version info
 
 Misc options:
     --spoofip-replace         Disable list of default internal IPs in 'http_headers_ip' bypass mode
     --spoofport-replace       Disable list of default internal ports in 'http_headers_port' bypass mode
     --request-tls             Force usage of TLS/HTTPS for the request load with the '-R, --request' option
     --dump-payloads           Print all payloads (curls) generated by this tool.
+    --jsonl                   Print results in JSON lines format (pipe command output)
 
 Examples:
     bypass-url-parser -u "http://127.0.0.1/juicy_403_endpoint/" -s 8.8.8.8 -d
     bypass-url-parser -u /path/urls -t 30 -T 5 -H "Cookie: me_iz=admin" -H "User-agent: test"
     bypass-url-parser -R /path/request_file --request-tls -m "mid_paths, end_paths"
 ```
 
@@ -109,22 +139,20 @@
 ```bash
 # Deps
 sudo apt install -y bat curl virtualenv python3
 # Tool
 virtualenv -p python3 .py3
 source .py3/bin/activate
 PDM_BUILD_SCM_VERSION="$(git describe --abbrev=0)-dev" pip install .
+# If bup installed globally, use
+python src/bypass_url_parser/__init__.py -u https://thinkloveshare.com/juicy_403_endpoint/
+# Else this should work
 bypass-url-parser -u https://thinkloveshare.com/juicy_403_endpoint/
 cat /tmp/tmpRANDOM-bypass-url-parser/triaged-bypass.json  | jq -r '.results[].request_curl_cmd'
 cat /tmp/tmpRANDOM-bypass-url-parser/triaged-bypass.json  | jq -r '.results[].response_data'
-
-# To test that all supported versions can boot
-for version in {8..13}; do
-  docker run --rm -it -v "$PWD":/host -w /host "python:3.$version" bash -c 'git config --global --add safe.directory /host && PDM_BUILD_SCM_VERSION="$(git describe --abbrev=0)-dev" pip install . && bup -u https://thinkloveshare.com/ -t 50 -m http_headers_scheme'
-done
 ```
 
 ### DOCKER
 
 ```bash
 docker run --rm -it -v "$PWD:/host" -w /host ghcr.io/laluka/bypass-url-parser:latest bash -il
 # Then bup -h, keep the docker open as the output is saved by default in /tmp
@@ -185,14 +213,24 @@
 Example:
 
 ```bash
 bypass-url-parser -u /path/urls -s /path/custom_ip --spoofip-replace
 bypass-url-parser -u /path/urls -p "3000, 9443, 10443"
 ```
 
+### JSON-Lines output and command piping
+
+With the `--jsonl` option, it's possible to print the results on `stdout` in `JSON-Lines` format. The standard tool's output and results are displayed with a logger on `stderr`, so it is possible to pipe the `JSON-Line` output format with other tools:
+
+```bash
+bypass-url-parser -u "https://thinkloveshare.com/juicy_403_endpoint/" -t 20 -S 0 -m case_substitution,char_encode --jsonl | jq
+```
+
+***Notes:** With `-S 2` ou `-S 3`, the JSON-Lines output also includes the path and the name of saved html files.*
+
 ### Results saving
 
 By default, if target url is unique, the tool saves a copy of the results in `/tmp/tmpXXX-bypass-url-parser/` directory.
 
 ***Notes:** If multiple target urls are passed to `-u`, results are prefixed with the url as directory (`/tmp/tmpXXX-bypass-url-parser/http-target-com-8080-api-users/`).*
 
 There are two arguments to customize this behavior:
@@ -374,55 +412,14 @@
   24   │     <meta http-equiv="Content-type" content="text/html; charset=utf-8">
   25   │     <meta http-equiv="Content-Security-Policy" content="default-src 'none'; style-src 'unsafe-inline'; img-src data:; connect-src 'self'">
   26   │     <title>Bad request &middot; GitHub Pages</title>
   27   │     <style type="text/css" media="screen">
 [...SNIP...]
 ```
 
-## Non-Regression tests & Code Cleanup
-
-```bash
-# Code Cleanup
-pre-commit run --all-files
-# Ensure no regression is pushed
-bypass-url-parser -S 0 -v -u http://127.0.0.1:8000/foo/bar --dump-payloads > "tests-history/bup-payloads-$(date +'%Y-%m-%d').lst"
-# Compare /tmp/bup-payloads-YYYY-MM-DD.lst and the latest tests-history/bup-payloads-YYYY-MM-DD.lst
-git diff --no-index $(find tests-history -type f | sort -n | tail -n 2)
-# Push your changes
-git add .
-git commit -m "My cool feature or bugfix"
-git tag -a vX.Y.Z "$COMMIT_HASH" -m "New release: vX.Y.Z"
-git push --tags
-# If X or Y is bumped, create new release on github
-```
-
-## Github Action Release
-
-- Visit https://github.com/laluka/bypass-url-parser/actions/workflows/release.yml
-- Run Workflow with a version such as `0.4.1` or `0.4.1-a` for alpha tests
-- Test the alpha version with the below script, once done, repeat without `-a`
-
-```bash
-cd /tmp
-export TESTED_VERSION=0.4.1a
-pipx install "bypass-url-parser==$TESTED_VERSION"
-bup --version && bup -u https://thinkloveshare.com/ -t 50 -m http_headers_scheme
-pipx uninstall bypass-url-parser
-bup --version # Should fail
-
-pip install "bypass-url-parser==$TESTED_VERSION"
-bup --version && bup -u https://thinkloveshare.com/ -t 50 -m http_headers_scheme
-pip uninstall bypass-url-parser
-bup --version # Should fail
-
-for version in {8..13}; do
-  docker run --rm -it "python:3.$version" bash -c "pip install bypass-url-parser==$TESTED_VERSION && bup --version && bup -u https://thinkloveshare.com/ -t 50 -m http_headers_scheme"
-done
-```
-
 ## Contributors
 
 - Initial release by [@TheLaluka](https://twitter.com/TheLaluka)
 - Huge refactoring & lib-mode with thanks to [@jtop_fap](https://twitter.com/jtop_fap)
 - Support for `Docker` & `Pypi` builds with the kind work of [@DugnyG](https://twitter.com/DugnyG)
 
 ## License
```

### Comparing `bypass_url_parser-0.4.1/pyproject.toml` & `bypass_url_parser-0.4.2a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
     "Typing :: Typed",
     "Topic :: Security",
     "Operating System :: OS Independent",
     "Environment :: Console",
 ]
-version = "0.4.1"
+version = "0.4.2a0"
 
 [project.license]
 text = "AGPL-3.0-or-later"
 
 [project.urls]
 Repository = "https://github.com/laluka/bypass-url-parser"
 Changelog = "https://github.com/laluka/bypass-url-parser/releases"
@@ -55,14 +55,17 @@
 [tool.pdm]
 distribution = true
 plugins = [
     "sync-pre-commit-lock",
     "pdm-autoexport",
 ]
 
+[tool.pdm.scripts]
+lint-ruff = "ruff check ."
+
 [tool.pdm.version]
 source = "scm"
 write_to = "bypass_url_parser/_version.py"
 write_template = "__version__ = \"{}\"\n"
 
 [tool.pdm.dev-dependencies]
 dev = [
@@ -72,14 +75,18 @@
     "ipython>=8.10.0",
     "pre-commit==3.2.2",
     "rich==13.3.4",
     "isort>=5.13.2",
     "mypy>=1.8.0",
     "types-docopt>=0.6.11.4",
     "autopep8>=2.0.4",
+    "ruff>=0.3.0",
+    "tox-pdm>=0.7.2",
+    "tox>=4.13.0",
+    "pytest>=8.0.2",
 ]
 
 [[tool.pdm.autoexport]]
 filename = "requirements.txt"
 groups = [
     "default",
 ]
@@ -91,7 +98,16 @@
 ]
 
 [tool.autopep8]
 max_line_length = 120
 in-place = true
 recursive = true
 aggresive = 1
+
+[tool.mypy]
+files = [
+    "src",
+]
+python_version = "3.8"
+overrides = [
+    { module = "coloredlogs", ignore_missing_imports = true },
+]
```

### Comparing `bypass_url_parser-0.4.1/src/bypass_url_parser/__init__.py` & `bypass_url_parser-0.4.2a0/src/bypass_url_parser/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 """Bypass Url Parser, made with love by @TheLaluka
 A tool that tests MANY url bypasses to reach a 40X protected page.
 
 Usage:
     bypass-url-parser (-u <URL> | -R <file>) [-m <mode>] [-o <outdir>] [-S <level>] [ (-H <header>)...] [-r <num>]
-                           [-s <ip>] [--spoofip-replace] [-p <port>] [--spoofport-replace] [--request-tls]
-                           [--dump-payloads] [-t <threads>] [-T <timeout>] [-x <proxy_url>] [-v | -d | -dd]
+                      [-s <ip>] [--spoofip-replace] [-p <port>] [--spoofport-replace] [-t <threads>] [-T <timeout>]
+                      [--request-tls] [--jsonl] [--dump-payloads] [-x <proxy_url>] [-v | -d | -dd]
 
 Program options:
     -u, --url <URL>           URL (path is optional) to run bypasses against
     -R, --request <file>      Load HTTP raw request from a file
     -H, --header <header>     Header(s) to use, format: "Cookie: can_i_haz=fire"
     -m, --mode <mode>         Bypass modes. See 'Bypasser.BYPASS_MODES' in code [Default: all]
     -o, --outdir <outdir>     Output directory for results
@@ -29,14 +29,15 @@
     -V, --version             Show version info
 
 Misc options:
     --spoofip-replace         Disable list of default internal IPs in 'http_headers_ip' bypass mode
     --spoofport-replace       Disable list of default internal ports in 'http_headers_port' bypass mode
     --request-tls             Force usage of TLS/HTTPS for the request load with the '-R, --request' option
     --dump-payloads           Print all payloads (curls) generated by this tool.
+    --jsonl                   Print results in JSON lines format (pipe command output)
 
 Examples:
     bypass-url-parser -u "http://127.0.0.1/juicy_403_endpoint/" -s 8.8.8.8 -d
     bypass-url-parser -u /path/urls -t 30 -T 5 -H "Cookie: me_iz=admin" -H "User-agent: test"
     bypass-url-parser -R /path/request_file --request-tls -m "mid_paths, end_paths"
 """
 
@@ -195,16 +196,17 @@
         self.save_level = config_dict.get("--save-level")
         self.spoof_ip_replace = config_dict.get("--spoofip-replace")  # If False spoof_ips append to existing list
         self.spoof_ips = config_dict.get("--spoofip")
         self.spoof_port_replace = config_dict.get("--spoofport-replace")  # If False spoof_ports append to existing list
         self.spoof_ports = config_dict.get("--spoofport")
         self.threads = config_dict.get("--threads")
         self.timeout = config_dict.get("--timeout")
-        self.dump_payloads = config_dict.get("--dump-payloads")
         self.retry_number = config_dict.get("--retry")
+        self.dump_payloads = config_dict.get("--dump-payloads")
+        self.jsonl_output = config_dict.get("--jsonl")
         self.request_tls = config_dict.get("--request-tls")
         if config_dict.get("--request"):
             self.request_raw = Tools.load_file_into_memory_list(
                 config_dict.get("--request"), enc_format=self.encoding, clean_filename=False, external_file=True,
                 return_str=True, ext_logger=self.logger, debug=self.debug_class)
         else:
             self.request_raw = None
@@ -495,15 +497,15 @@
 
         :param CurlItem item: Item object
         """
         if self.debug:
             self.logger.info(f"Current: {shlex_join(item.request_curl_cmd)}")
         try:
             process = subprocess.Popen(item.request_curl_cmd, text=True, shell=False, stderr=subprocess.STDOUT,
-                                       stdout=subprocess.PIPE, encoding='utf-8')
+                                       stdout=subprocess.PIPE, encoding=self.encoding)
 
             # Get command results
             result = process.communicate(timeout=self.timeout)[0]
             # Successful execution, parse result
             if process.returncode == 0:
                 if result:
                     # Apply xxx2unix. Mandatory under Windows/macOS to save curl responses headers in html file
@@ -549,27 +551,28 @@
         except subprocess.TimeoutExpired as e:
             if self.debug:
                 self.logger.warning(f'Command "{shlex_join(e.cmd)}" timed out: {e.output}')
             self.to_retry_items.add(item)
 
     def _save_results(self, url_obj):
         if self.save_level != self.SaveLevel.NONE:
+            results_path = Tools.get_path_with_url(self.output_dir, url_obj) if len(self.urls) > 1 else self.output_dir
             json_items = {
                 "url": url_obj.geturl(),
                 "bypass_modes": ', '.join(self.current_bypass_modes),
+                "results_path": results_path,
                 "results": []
             }
             # Output_directory definition and creation
             outdir = self.output_dir
             try:
                 # If multiple URLs, add one subdirectory by url
                 if len(self.urls) > 1:
                     # Format: output_dir / https - www.tld.com[-port -] - path - endpoint
-                    subdir_name = f"{url_obj.scheme}-{url_obj.netloc.replace(':', '-')}{url_obj.path.replace('/', '-')}"
-                    outdir = f"{self.output_dir}{Tools.SEPARATOR}{subdir_name}"
+                    outdir = Tools.get_path_with_url(self.output_dir, url_obj)
                 # Create directory
                 if Tools.is_exist_directory(outdir, force_create=True):
                     if self.debug_class:
                         self.logger.debug(f"Output directory '{outdir}{Tools.SEPARATOR}' exists on system")
             except Exception as e:
                 error_msg = f"Error while creating output directory '{outdir}{Tools.SEPARATOR}': {e}"
                 self.logger.error(error_msg)
@@ -580,29 +583,29 @@
                 for item in self.curl_items:
                     # Save only completed requests
                     if item not in self.to_retry_items:
                         if not item.save(outdir, force_output_dir_creation=False):
                             self.logger.warning(f"Error when saving {outdir}{Tools.SEPARATOR}{item.filename} file.")
                         else:
                             # Add curl item json representation
-                            json_items["results"].append(json.loads(item.to_json()))
+                            json_items["results"].append(json.loads(item.to_json(with_html_filename=True)))
                 if self.verbose:
                     self.logger.info(f"All curl responses were saved in the '{outdir}{Tools.SEPARATOR}' directory")
 
             # SaveLevel.PERTINENT - Save only results items (single and first element of each group)
             elif self.save_level >= self.SaveLevel.PERTINENT:
                 if self.bypass_results[url_obj]:
                     for url, item_lst in self.bypass_results[url_obj].items():
                         # Save pertinent curl items as individual HTML file
                         if not item_lst[0].save(outdir, force_output_dir_creation=False):
                             self.logger.warning(
                                 f"Error when saving {outdir}{Tools.SEPARATOR}{item_lst[0].filename} file.")
                         else:
                             # Add curl item json representation
-                            json_items["results"].append(json.loads(item_lst[0].to_json()))
+                            json_items["results"].append(json.loads(item_lst[0].to_json(with_html_filename=True)))
                     if self.verbose:
                         self.logger.info(f"Only relevant curl responses (results) were saved in the "
                                          f"'{outdir}{Tools.SEPARATOR}' directory")
                 else:
                     self.logger.warning("No output to save")
 
             # Batcat - Starting at SaveLevel.PERTINENT, IOW no html files, no batcat command
@@ -639,15 +642,15 @@
                 with open(json_file, mode="w", encoding=self.encoding) as file:
                     logger.info(f"Save JSON results for '{url_obj.geturl()}' in {json_file}")
                     file.write(json.dumps(json_items, indent=2))
         else:
             if self.debug_class:
                 self.logger.debug("No saving any output: SaveLevel.NONE")
 
-    def _output_results(self, url_obj, silent_mode=False) -> defaultdict[list]:
+    def _output_results(self, url_obj, jsonl_output=False, silent_mode=False) -> defaultdict[list]:
         # Create a new defaultdict(list) of aggregated items and reset output
         grouped_curl_items = defaultdict(list)
         self.clean_output = ""
 
         # Parse all completed curl items
         for item in self.curl_items:
             # Results aggregating
@@ -655,22 +658,29 @@
                 key_for_unicity = item.get_formatted_response(with_content_length=False, trunk_redirect_url=True)
                 if item not in grouped_curl_items[key_for_unicity]:
                     grouped_curl_items[key_for_unicity].append(item)
 
         # Output program result
         if grouped_curl_items:
             # Get results and store (for the program log file) program output.
+            multiple_urls = True if len(self.urls) > 1 else False
             with_filename = True if self.save_level >= self.SaveLevel.PERTINENT else False
             self.clean_output = \
-                Bypasser.get_results_from_grouped_items(url_obj, grouped_curl_items, header_line=True,
-                                                        with_filename=with_filename, ext_logger=self.logger,
-                                                        verbose=self.verbose)
+                Bypasser.get_results_from_grouped_items(
+                    url_obj, grouped_curl_items, header_line=True, with_filename=with_filename,
+                    jsonl_format=jsonl_output, jsonl_output_dir=self.output_dir, jsonl_multiple_urls=multiple_urls,
+                    ext_logger=self.logger, verbose=self.verbose)
             # Print results
             if not silent_mode:
-                self.logger.info(f"\n{self.clean_output}")
+                if self.jsonl_output:
+                    # JSON-lines output (stdout)
+                    print(self.clean_output, flush=True)
+                else:
+                    # Normal output in logger (stderr)
+                    self.logger.info(f"\n{self.clean_output}")
 
         return grouped_curl_items
 
     def _parse_raw_request(self) -> None:
         """ Parse raw request if present to define headers and url.
 
         Called by get_curl_base and keep the prevalence of existing headers. So it's possible to override a raw request
@@ -883,67 +893,89 @@
                 self.logger.warning(f"Trying to bypass '{url_obj.geturl()}' url ({len(self.curl_items)} payloads)...")
             self._run_curls(self.curl_items)
 
             # Retry failed curl requests
             self._retry_failed_commands()
 
             # Show results
-            current_result = self._output_results(url_obj, silent_mode=silent_mode)
+            if self.jsonl_output and self.save_level >= self.SaveLevel.MINIMAL:
+                self._output_results(url_obj, jsonl_output=self.jsonl_output, silent_mode=silent_mode)
+                # Keep original output for triaged-bypass.log file
+                current_result = self._output_results(url_obj, jsonl_output=False, silent_mode=True)
+            else:
+                current_result = self._output_results(url_obj, jsonl_output=self.jsonl_output, silent_mode=silent_mode)
+
             if url_obj not in self.bypass_results.keys():
                 self.bypass_results[url_obj] = current_result
 
             # Save results (Curl request/responses and program logfile)
             self._save_results(url_obj)
 
         # Return global results dict for library mode
         return self.bypass_results
 
     @staticmethod
     def get_results_from_grouped_items(url_obj: ParseResult, grouped_curl_items: defaultdict[list], header_line=True,
-                                       with_filename=True, filter_sc=None, ext_logger=None, verbose=False) -> str:
+                                       with_filename=True, filter_sc=None, jsonl_format=False, jsonl_output_dir="",
+                                       jsonl_multiple_urls=False, ext_logger=None, verbose=False) -> str:
         """Ungroup and return string from aggregated curl items.
 
         When the Bypasser is used as a library, this method is useful to retrieve the aggregated results in a string,
         as usually returned by the program. See the commented code in the main() function for an example of use.
 
-        :param ParseResult url_obj: Curl command target url object
-        :param defaultdict[list] grouped_curl_items: Aggregation of curls items. Result of _output_results() method
+        :param ParseResult url_obj: The target URL object of the curl command
+        :param defaultdict[list] grouped_curl_items: Aggregated curl items. Result of _output_results() method
         :param bool header_line: If True return result headers: '[#####] [bypass_method] [payload] => [status_code]...'
         :param bool with_filename: If True return (item.filename) as end of output line
-        :param list filter_sc: Filter status codes from results. Ex: [403,405,400]
+        :param list filter_sc: List of status codes to filter from results. Ex: [403,405,400]
+        :param bool jsonl_format: Format and print results as JSON lines. Defaults to True.
+        :param str jsonl_output_dir: Output directory where HTML files are stored (default: "")
+        :param bool jsonl_multiple_urls: Adds URL to 'jsonl_output_dir' (when len(self.url) > 1 in Bypasser).
         :param logger ext_logger: Specify your own logger for verbose output (default: None) (Optional)
         :param bool verbose: Show verbose information for this method
         :return: Aggregated results
         """
         clean_output = ""
         if grouped_curl_items:
             filter_status_codes = filter_sc if filter_sc else []
-            if ext_logger and verbose:
+            if ext_logger and verbose and not jsonl_format:
                 ext_logger.warning(f"Triaged results & distinct pages for '{url_obj.geturl()}' url:")
             # Build output
-            if header_line:
+            if header_line and not jsonl_format:
                 if with_filename:
                     clean_output += f"{CurlItem.get_formatted_item_header()} (filename)\n"
                 else:
                     clean_output += f"{CurlItem.get_formatted_item_header()}\n"
             for out_key, item_lst in grouped_curl_items.items():
                 item_count = len(item_lst)
-                if item_count == 1:
-                    if item_lst[0].response_status_code not in filter_status_codes:
-                        if with_filename:
-                            clean_output += f"[SINGLE] {item_lst[0].get_formatted_item()} ({item_lst[0].filename})\n"
-                        else:
-                            clean_output += f"[SINGLE] {item_lst[0].get_formatted_item()}\n"
+                if not jsonl_format:
+                    if item_count == 1:
+                        if item_lst[0].response_status_code not in filter_status_codes:
+                            if with_filename:
+                                clean_output += \
+                                    f"[SINGLE] {item_lst[0].get_formatted_item()} ({item_lst[0].filename})\n"
+                            else:
+                                clean_output += f"[SINGLE] {item_lst[0].get_formatted_item()}\n"
+                    else:
+                        if item_lst[0].response_status_code not in filter_status_codes:
+                            if with_filename:
+                                clean_output += f"[GROUP ({item_count})] {item_lst[0].get_formatted_item()} " \
+                                                f"({item_lst[0].filename})\n"
+                            else:
+                                clean_output += f"[GROUP ({item_count})] {item_lst[0].get_formatted_item()}\n"
                 else:
                     if item_lst[0].response_status_code not in filter_status_codes:
                         if with_filename:
-                            clean_output += f"[GROUP ({item_count})] {item_lst[0].get_formatted_item()} " \
-                                            f"({item_lst[0].filename})\n"
+                            json_line = item_lst[0].to_json(
+                                result_path=jsonl_output_dir, result_path_with_url=jsonl_multiple_urls,
+                                result_count=item_count, with_url=jsonl_format)
                         else:
-                            clean_output += f"[GROUP ({item_count})] {item_lst[0].get_formatted_item()}\n"
+                            json_line = item_lst[0].to_json(
+                                result_path=None, result_count=item_count, with_url=jsonl_format)
+                        clean_output = f"{clean_output}{json_line}\n"
         else:
             if ext_logger and verbose:
                 ext_logger.warning(f"Failed to find any valid response for '{url_obj.geturl()}' url")
 
         return clean_output.rstrip("\n")
 
     # *** Properties ***#
@@ -1436,16 +1468,17 @@
     REGEX_CONTENT_TYPE = re.compile(r"Content-Type:\s+(\w+/\w+)", re.IGNORECASE)
     REGEX_HTTP_VERSION = re.compile(r"(?!--)http[\w.-]*(?<! )", re.IGNORECASE)
     REGEX_REDIRECT_URL = re.compile(r"Location:\s+(.*)", re.IGNORECASE)
     REGEX_SERVER_TYPE = re.compile(r"Server:\s+(.*)", re.IGNORECASE)
     REGEX_TITLE = re.compile(r"<title>(.*?)</title>", re.IGNORECASE)
     REDIRECT_URL_MAX_SIZE = 25
 
-    def __init__(self, target_url: ParseResult, curl_base: list[str], curl_cmd: list[str], bypass_mode: str | None = None, target_ip: str | None = None,
-                 encoding=None, debug=False, ext_logger=None):
+    def __init__(self, target_url: ParseResult, curl_base: list[str], curl_cmd: list[str],
+                 bypass_mode: str | None = None, target_ip: str | None = None, encoding=None, debug=False,
+                 ext_logger=None):
         """CurlItem object init method
 
         :param ParseResult target_url: Curl command target url object
         :param list[str] curl_base: Curl base command. Ex: curl -sS -kgi --path-as-is
         :param list[str] curl_cmd: Curl full command. Ex: curl -sS -kgi --path-as-is -H 'xxx' https://target.com/path
         :param str bypass_mode:  Payload description (Optional)
         :param str target_ip: IP address of target url (Optional)
@@ -1551,32 +1584,59 @@
             self.logger.debug(f"Saving html pages and short output in: '{output_dir}{Tools.SEPARATOR}'")
             with open(f"{out_filename}", mode="w", encoding=self.encoding) as file:
                 file.write(f"{shlex_join(self.request_curl_cmd)}\n\n{self.response_headers}\n\n{self.response_data}")
             return True
         else:
             return False
 
-    def to_json(self) -> str:
-        # Return json representation of curl item
-        return json.dumps(
-            {
-                "request_curl_cmd": shlex_join(self.request_curl_cmd),
-                "request_curl_payload": self.request_curl_payload,
-                "response_headers": self.response_headers,
-                "response_data": self.response_data,
-                "response_status_code": self.response_status_code,
-                "response_content_type": self.response_content_type,
-                "response_content_length": self.response_content_length,
-                "response_lines_count": self.response_lines_count,
-                "response_words_count": self.response_words_count,
-                "response_title": self.response_title,
-                "response_server_type": self.response_server_type,
-                "response_redirect_url": self.response_redirect_url,
-                "response_html_filename": self.filename
-            })
+    def to_json(self, result_path="", result_path_with_url=False, result_count=0, with_html_filename=False,
+                with_url=False) -> str:
+        """ Converts a curl item object into a JSON representation.
+
+        :param str result_path: Add 'response_html_path' to json if present
+        :param bool result_path_with_url: Adds URL to 'result_path' (when len(self.url) > 1 in Bypasser)
+        :param int result_count: If greater than or equal to 1, adds 'result_count' and 'results_tag' to json
+        :param bool with_html_filename: Includes 'response_html_filename' to json if True or if result_path is present
+        :param bool with_url: Includes 'request_url' to json if True
+        :return: JSON representation of the object
+        """
+        json_repr = {
+            "request_curl_cmd": shlex_join(self.request_curl_cmd),
+            "request_curl_payload": self.request_curl_payload,
+            "response_headers": self.response_headers,
+            "response_data": self.response_data,
+            "response_status_code": self.response_status_code,
+            "response_content_type": self.response_content_type,
+            "response_content_length": self.response_content_length,
+            "response_lines_count": self.response_lines_count,
+            "response_words_count": self.response_words_count,
+            "response_title": self.response_title,
+            "response_server_type": self.response_server_type,
+            "response_redirect_url": self.response_redirect_url
+            # "response_html_filename": self.filename
+        }
+        # Add response HTML path and filename based on options
+        if result_path:
+            json_repr["response_html_filename"] = self.filename
+            json_repr["response_html_path"] = Tools.get_path_with_url(result_path, self.target_url) \
+                if result_path_with_url else result_path
+        else:
+            if with_html_filename:
+                json_repr["response_html_filename"] = self.filename
+
+        # Add result count and result tag
+        if isinstance(result_count, int) and result_count:
+            json_repr["results_count"] = result_count
+            json_repr["results_tag"] = "SINGLE" if result_count == 1 else "GROUP"
+
+        # Add request URL if specified
+        if with_url:
+            json_repr["request_url"] = self.target_url.geturl()
+
+        return json.dumps(json_repr, sort_keys=False)
 
     # *** Properties *** #
 
     @property
     def filename(self) -> str:
         return f"bypass-{hashlib.md5(' '.join(map(str, self._curl_cmd)).encode()).hexdigest()}.html"
 
@@ -1650,15 +1710,15 @@
             raise ValueError(error_msg)
 
     @property
     def response_content_length(self) -> int:
         if self.response_raw_output:
             try:
                 match_content_length = CurlItem.REGEX_CONTENT_LENGTH.search(self.response_headers)
-                return int(match_content_length.group(1).rstrip()) if match_content_length else ""
+                return int(match_content_length.group(1).rstrip()) if match_content_length else len(self.response_data)
             except Exception as e:
                 error_msg = f"Unable to return response content_length, please check the format and " \
                             f"redefine the 'response_raw_output' property {e}"
                 self.logger.error(error_msg)
                 self.logger.error(repr(self.response_raw_output))
                 raise ValueError(error_msg)
         else:
@@ -1921,28 +1981,29 @@
             error_msg = f"The '{arg_name}' argument type is not supported"
             if ext_logger:
                 ext_logger.error(error_msg)
             raise ValueError(error_msg)
 
     @overload
     @staticmethod
-    def load_file_into_memory_list(filename: str, enc_format: str | None = None, clean_filename=False, external_file=False,
-                                   return_str=False, debug=False, ext_logger=None) -> list[str]:
+    def load_file_into_memory_list(filename: str, enc_format: str | None = None, clean_filename=False,
+                                   external_file=False, return_str=False, debug=False, ext_logger=None) -> list[str]:
         ...
 
     @overload
     @staticmethod
-    def load_file_into_memory_list(filename: str, enc_format: str | None = None, clean_filename=False, external_file=False,
-                                   return_str=True, debug=False, ext_logger=None) -> str:
+    def load_file_into_memory_list(filename: str, enc_format: str | None = None, clean_filename=False,
+                                   external_file=False, return_str=True, debug=False, ext_logger=None) -> str:
         ...
 
     @staticmethod
-    def load_file_into_memory_list(filename: str, enc_format: str | None = None, clean_filename=False, external_file=False,
-                                   return_str=False, debug=False, ext_logger=None) -> list[str] | str:
-        r"""Load whole file into a list (or a string) in memory.
+    def load_file_into_memory_list(filename: str, enc_format: str | None = None, clean_filename=False,
+                                   external_file=False, return_str=False, debug=False,
+                                   ext_logger=None) -> list[str] | str:
+        """Load whole file into a list (or a string) in memory.
 
         Note: Fast for small files, do not use with huge file...
 
         :param str filename: Fast filename from args example: .\test.txt or "../../test.txt"
         :param str enc_format: Encoding format to read file. Default (locale.getpreferredencoding) (Optional)
         :param bool clean_filename: Is filename previously cleaned (transform_relative_filename) ? Default (False)
         :param bool external_file: If not clean_filename, don't use project root dir for absolute file name resolution
@@ -2000,14 +2061,26 @@
         res = os.path.isdir(directory)
         if not res and force_create:
             path = Path(directory)
             path.mkdir(mode=create_mode, parents=True, exist_ok=True)
             return True
         return res
 
+    @staticmethod
+    def get_path_with_url(base_path, url_obj) -> str:
+        """ Generate a path combining the base path and URL components.
+
+        :param str base_path: The base path to modify
+        :param ParseResult url_obj: The parsed URL components
+        :return: The combined path
+        """
+        # Format: output_dir / https - www.tld.com[-port -] - path - endpoint
+        subdir_name = f"{url_obj.scheme}-{url_obj.netloc.replace(':', '-')}{url_obj.path.replace('/', '-')}"
+        return f"{base_path}{Tools.SEPARATOR}{subdir_name.rstrip('-')}"
+
 
 def main():
     # Show all options by Default
     if len(sys.argv) == 1:
         sys.argv.append("-h")
     arguments = docopt(__doc__, version=f"bypass_url_parser {__version__}")
```

### Comparing `bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/header_ip_hosts.lst` & `bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/header_ip_hosts.lst`

 * *Files identical despite different names*

### Comparing `bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/header_urls.lst` & `bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/header_urls.lst`

 * *Files identical despite different names*

### Comparing `bypass_url_parser-0.4.1/src/bypass_url_parser/payloads/internal_midpaths.lst` & `bypass_url_parser-0.4.2a0/src/bypass_url_parser/payloads/internal_midpaths.lst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+,
 ;
 ;?
 ;/
 ;/.;.
 ;/..
 ;/..;
 ;/../
```

### Comparing `bypass_url_parser-0.4.1/PKG-INFO` & `bypass_url_parser-0.4.2a0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: bypass-url-parser
-Version: 0.4.1
-Summary: Default template for PDM package
-Keywords: security
-Author-Email: Laluka <loukajc@gmail.com>, jtof_fap <jtof_fap@insecurity.fr>, Gabriel Dugny <pypi@dugny.me>
-License: AGPL-3.0-or-later
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Classifier: Typing :: Typed
-Classifier: Topic :: Security
-Classifier: Operating System :: OS Independent
-Classifier: Environment :: Console
-Project-URL: Repository, https://github.com/laluka/bypass-url-parser
-Project-URL: Changelog, https://github.com/laluka/bypass-url-parser/releases
-Requires-Python: >=3.8
-Requires-Dist: coloredlogs==15.0.1
-Requires-Dist: docopt==0.6.2
-Description-Content-Type: text/markdown
-
 # Bypass Url Parser
 
 [![PyPI - Version](https://img.shields.io/pypi/v/bypass-url-parser)](https://pypi.org/project/bypass-url-parser/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bypass-url-parser)](https://pypi.org/project/bypass-url-parser/) [![PyPI - License](https://img.shields.io/pypi/l/bypass-url-parser)](https://github.com/laluka/bypass-url-parser/blob/main/LICENSE) [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
 Tool that tests `MANY` url bypasses to reach a `40X protected page`.
 
 If you wonder why this code is `nothing but a dirty curl wrapper`, here's why:
@@ -64,28 +35,28 @@
 
 ```
 Bypass Url Parser, made with love by @TheLaluka
 A tool that tests MANY url bypasses to reach a 40X protected page.
 
 Usage:
     bypass-url-parser (-u <URL> | -R <file>) [-m <mode>] [-o <outdir>] [-S <level>] [ (-H <header>)...] [-r <num>]
-                           [-s <ip>] [--spoofip-replace] [-p <port>] [--spoofport-replace] [--request-tls]
-                           [--dump-payloads] [-t <threads>] [-T <timeout>] [-x <proxy_url>] [-v | -d | -dd]
+                      [-s <ip>] [--spoofip-replace] [-p <port>] [--spoofport-replace] [-t <threads>] [-T <timeout>]
+                      [--request-tls] [--jsonl] [--dump-payloads] [-x <proxy_url>] [-v | -d | -dd]
 
 Program options:
     -u, --url <URL>           URL (path is optional) to run bypasses against
     -R, --request <file>      Load HTTP raw request from a file
     -H, --header <header>     Header(s) to use, format: "Cookie: can_i_haz=fire"
     -m, --mode <mode>         Bypass modes. See 'Bypasser.BYPASS_MODES' in code [Default: all]
     -o, --outdir <outdir>     Output directory for results
     -x, --proxy <proxy_url>   Set a proxy in the format http://proxy_ip:port.
-    -S, --save-level <level>  Save results level. From 0 (DISABLE) to 3 (FULL) [Default: 1]
+    -S, --save-level <level>  Save results level. From 0 (DISABLE) to 3 (FULL) [Default: 2]
     -s, --spoofip <ip>        IP(s) to inject in ip-specific headers
     -p, --spoofport <port>    Port(s) to inject in port-specific headers
-    -r, --retry <num>         Retry attempts of failed requests. Set 0 to disable all retry tentatives [Default: 3]
+    -r, --retry <num>         Retry attempts of failed requests. Set 0 to disable all retry tentatives [Default: 1]
     -t, --threads <threads>   Scan with N parallel threads [Default: 1]
     -T, --timeout <timeout>   Request times out after N seconds [Default: 5]
 
 General options:
     -h, --help                Show help, you are here :)
     -v, --verbose             Verbose output
     -d, --debug               Show more details like curl commands generated by this tool
@@ -93,14 +64,15 @@
     -V, --version             Show version info
 
 Misc options:
     --spoofip-replace         Disable list of default internal IPs in 'http_headers_ip' bypass mode
     --spoofport-replace       Disable list of default internal ports in 'http_headers_port' bypass mode
     --request-tls             Force usage of TLS/HTTPS for the request load with the '-R, --request' option
     --dump-payloads           Print all payloads (curls) generated by this tool.
+    --jsonl                   Print results in JSON lines format (pipe command output)
 
 Examples:
     bypass-url-parser -u "http://127.0.0.1/juicy_403_endpoint/" -s 8.8.8.8 -d
     bypass-url-parser -u /path/urls -t 30 -T 5 -H "Cookie: me_iz=admin" -H "User-agent: test"
     bypass-url-parser -R /path/request_file --request-tls -m "mid_paths, end_paths"
 ```
 
@@ -138,22 +110,20 @@
 ```bash
 # Deps
 sudo apt install -y bat curl virtualenv python3
 # Tool
 virtualenv -p python3 .py3
 source .py3/bin/activate
 PDM_BUILD_SCM_VERSION="$(git describe --abbrev=0)-dev" pip install .
+# If bup installed globally, use
+python src/bypass_url_parser/__init__.py -u https://thinkloveshare.com/juicy_403_endpoint/
+# Else this should work
 bypass-url-parser -u https://thinkloveshare.com/juicy_403_endpoint/
 cat /tmp/tmpRANDOM-bypass-url-parser/triaged-bypass.json  | jq -r '.results[].request_curl_cmd'
 cat /tmp/tmpRANDOM-bypass-url-parser/triaged-bypass.json  | jq -r '.results[].response_data'
-
-# To test that all supported versions can boot
-for version in {8..13}; do
-  docker run --rm -it -v "$PWD":/host -w /host "python:3.$version" bash -c 'git config --global --add safe.directory /host && PDM_BUILD_SCM_VERSION="$(git describe --abbrev=0)-dev" pip install . && bup -u https://thinkloveshare.com/ -t 50 -m http_headers_scheme'
-done
 ```
 
 ### DOCKER
 
 ```bash
 docker run --rm -it -v "$PWD:/host" -w /host ghcr.io/laluka/bypass-url-parser:latest bash -il
 # Then bup -h, keep the docker open as the output is saved by default in /tmp
@@ -214,14 +184,24 @@
 Example:
 
 ```bash
 bypass-url-parser -u /path/urls -s /path/custom_ip --spoofip-replace
 bypass-url-parser -u /path/urls -p "3000, 9443, 10443"
 ```
 
+### JSON-Lines output and command piping
+
+With the `--jsonl` option, it's possible to print the results on `stdout` in `JSON-Lines` format. The standard tool's output and results are displayed with a logger on `stderr`, so it is possible to pipe the `JSON-Line` output format with other tools:
+
+```bash
+bypass-url-parser -u "https://thinkloveshare.com/juicy_403_endpoint/" -t 20 -S 0 -m case_substitution,char_encode --jsonl | jq
+```
+
+***Notes:** With `-S 2` ou `-S 3`, the JSON-Lines output also includes the path and the name of saved html files.*
+
 ### Results saving
 
 By default, if target url is unique, the tool saves a copy of the results in `/tmp/tmpXXX-bypass-url-parser/` directory.
 
 ***Notes:** If multiple target urls are passed to `-u`, results are prefixed with the url as directory (`/tmp/tmpXXX-bypass-url-parser/http-target-com-8080-api-users/`).*
 
 There are two arguments to customize this behavior:
@@ -403,55 +383,14 @@
   24   │     <meta http-equiv="Content-type" content="text/html; charset=utf-8">
   25   │     <meta http-equiv="Content-Security-Policy" content="default-src 'none'; style-src 'unsafe-inline'; img-src data:; connect-src 'self'">
   26   │     <title>Bad request &middot; GitHub Pages</title>
   27   │     <style type="text/css" media="screen">
 [...SNIP...]
 ```
 
-## Non-Regression tests & Code Cleanup
-
-```bash
-# Code Cleanup
-pre-commit run --all-files
-# Ensure no regression is pushed
-bypass-url-parser -S 0 -v -u http://127.0.0.1:8000/foo/bar --dump-payloads > "tests-history/bup-payloads-$(date +'%Y-%m-%d').lst"
-# Compare /tmp/bup-payloads-YYYY-MM-DD.lst and the latest tests-history/bup-payloads-YYYY-MM-DD.lst
-git diff --no-index $(find tests-history -type f | sort -n | tail -n 2)
-# Push your changes
-git add .
-git commit -m "My cool feature or bugfix"
-git tag -a vX.Y.Z "$COMMIT_HASH" -m "New release: vX.Y.Z"
-git push --tags
-# If X or Y is bumped, create new release on github
-```
-
-## Github Action Release
-
-- Visit https://github.com/laluka/bypass-url-parser/actions/workflows/release.yml
-- Run Workflow with a version such as `0.4.1` or `0.4.1-a` for alpha tests
-- Test the alpha version with the below script, once done, repeat without `-a`
-
-```bash
-cd /tmp
-export TESTED_VERSION=0.4.1a
-pipx install "bypass-url-parser==$TESTED_VERSION"
-bup --version && bup -u https://thinkloveshare.com/ -t 50 -m http_headers_scheme
-pipx uninstall bypass-url-parser
-bup --version # Should fail
-
-pip install "bypass-url-parser==$TESTED_VERSION"
-bup --version && bup -u https://thinkloveshare.com/ -t 50 -m http_headers_scheme
-pip uninstall bypass-url-parser
-bup --version # Should fail
-
-for version in {8..13}; do
-  docker run --rm -it "python:3.$version" bash -c "pip install bypass-url-parser==$TESTED_VERSION && bup --version && bup -u https://thinkloveshare.com/ -t 50 -m http_headers_scheme"
-done
-```
-
 ## Contributors
 
 - Initial release by [@TheLaluka](https://twitter.com/TheLaluka)
 - Huge refactoring & lib-mode with thanks to [@jtop_fap](https://twitter.com/jtop_fap)
 - Support for `Docker` & `Pypi` builds with the kind work of [@DugnyG](https://twitter.com/DugnyG)
 
 ## License
```

