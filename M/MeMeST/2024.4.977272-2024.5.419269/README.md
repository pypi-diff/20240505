# Comparing `tmp/MeMeST-2024.4.977272-py3-none-any.whl.zip` & `tmp/MeMeST-2024.5.419269-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 33742 bytes, number of entries: 16
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-10 04:45 MeMeST-2024.4.977272.data/data/LICENSE
+Zip file size: 33846 bytes, number of entries: 16
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-10 04:45 MeMeST-2024.5.419269.data/data/LICENSE
 -rw-rw-r--  2.0 unx       76 b- defN 24-Apr-10 04:45 git_tools/__init__.py
 -rw-rw-r--  2.0 unx     1139 b- defN 24-Apr-18 09:30 git_tools/base_dtypes.py
--rw-rw-r--  2.0 unx     9002 b- defN 24-Apr-29 13:49 git_tools/git_api.py
+-rw-rw-r--  2.0 unx     9287 b- defN 24-May-05 13:38 git_tools/git_api.py
 -rw-rw-r--  2.0 unx      143 b- defN 24-Apr-10 04:45 git_tools/rep_task.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-10 04:45 mest/__init__.py
 -rw-rw-r--  2.0 unx     4518 b- defN 24-Apr-29 10:15 mest/config.py
--rw-rw-r--  2.0 unx     3400 b- defN 24-Apr-29 13:52 mest/main.py
+-rw-rw-r--  2.0 unx     3405 b- defN 24-May-05 13:37 mest/main.py
 -rw-rw-r--  2.0 unx     2717 b- defN 24-Apr-29 13:50 mest/rep_mana.py
 -rw-rw-r--  2.0 unx      569 b- defN 24-Apr-10 04:45 mest/test_git.py
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-29 13:54 MeMeST-2024.4.977272.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1797 b- defN 24-Apr-29 13:54 MeMeST-2024.4.977272.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-29 13:54 MeMeST-2024.4.977272.dist-info/WHEEL
--rw-rw-r--  2.0 unx       42 b- defN 24-Apr-29 13:54 MeMeST-2024.4.977272.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-29 13:54 MeMeST-2024.4.977272.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1286 b- defN 24-Apr-29 13:54 MeMeST-2024.4.977272.dist-info/RECORD
-16 files, 95094 bytes uncompressed, 31626 bytes compressed:  66.7%
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1797 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       42 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       15 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1286 b- defN 24-May-05 13:39 MeMeST-2024.5.419269.dist-info/RECORD
+16 files, 95384 bytes uncompressed, 31730 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: MeMeST-2024.4.977272.data/data/LICENSE
+Filename: MeMeST-2024.5.419269.data/data/LICENSE
 Comment: 
 
 Filename: git_tools/__init__.py
 Comment: 
 
 Filename: git_tools/base_dtypes.py
 Comment: 
@@ -24,26 +24,26 @@
 
 Filename: mest/rep_mana.py
 Comment: 
 
 Filename: mest/test_git.py
 Comment: 
 
-Filename: MeMeST-2024.4.977272.dist-info/LICENSE
+Filename: MeMeST-2024.5.419269.dist-info/LICENSE
 Comment: 
 
-Filename: MeMeST-2024.4.977272.dist-info/METADATA
+Filename: MeMeST-2024.5.419269.dist-info/METADATA
 Comment: 
 
-Filename: MeMeST-2024.4.977272.dist-info/WHEEL
+Filename: MeMeST-2024.5.419269.dist-info/WHEEL
 Comment: 
 
-Filename: MeMeST-2024.4.977272.dist-info/entry_points.txt
+Filename: MeMeST-2024.5.419269.dist-info/entry_points.txt
 Comment: 
 
-Filename: MeMeST-2024.4.977272.dist-info/top_level.txt
+Filename: MeMeST-2024.5.419269.dist-info/top_level.txt
 Comment: 
 
-Filename: MeMeST-2024.4.977272.dist-info/RECORD
+Filename: MeMeST-2024.5.419269.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## git_tools/git_api.py

```diff
@@ -6,14 +6,23 @@
 ENV = os.environ.copy()
 ENV["LD_LIBRARY_PATH"] = ""
 ENV["PATH"] = "/usr/bin:/bin:/usr/local/bin"
 if "OPENSSL_DIR" in ENV:
     del ENV["OPENSSL_DIR"]
 
 
+def handle_index_lock_error(work_dir, error_msg):
+    if ".git/index.lock" in error_msg:
+        subprocess.run(
+            ["rm", "-f", ".git/index.lock"], env=ENV, cwd=work_dir, check=False
+        )
+        return True
+    return False
+
+
 def mkdir(path):
     if not os.path.exists(path):
         os.makedirs(path)
 
 
 def get_all_remotes(work_dir: str):
     cmd = ["git", "remote", "-v"]
@@ -137,16 +146,20 @@
 
 
 def update_branch_list(rep_data: RepData):
     work_dir = rep_data.work_dir
     git_command = ["git", "branch", "-r"]
     output = subprocess.check_output(git_command, text=True, cwd=work_dir)
     alias = rep_data.alias
-    remote_branches = [line.strip() for line in output.splitlines() if line.strip().startswith(alias)]
-    rep_data.branch_list = [branch_name[len(alias) + 1:] for branch_name in remote_branches]
+    remote_branches = [
+        line.strip() for line in output.splitlines() if line.strip().startswith(alias)
+    ]
+    rep_data.branch_list = [
+        branch_name[len(alias) + 1 :] for branch_name in remote_branches
+    ]
     # logger.info("remote_branches {}", rep_data.branch_list)
 
 
 @logger.catch
 def push(rep_data: RepData):
     if not good_rep_data(rep_data):
         return
@@ -160,19 +173,17 @@
             checkout_command,
             cwd=work_dir,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.PIPE,
             check=False,
         )
         if result.returncode != 0:
-            logger.error(
-                "fail, code:{} reason:{}",
-                result.returncode,
-                result.stderr.decode("utf-8"),
-            )
+            error_msg = result.stderr.decode("utf-8")
+            if not handle_index_lock_error(work_dir, error_msg):
+                logger.error("fail, code:{} reason:{}", result.returncode, error_msg)
             continue
 
         push_command = []
         pull_command = []
         if rep_data.key_file:
             git_ssh_command = f'ssh -i "{rep_data.key_file}"'
             push_command.append(git_ssh_command)
@@ -228,31 +239,29 @@
             cwd=work_dir,
             env=ENV,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.PIPE,
             check=False,
         )
         subprocess.run(
-            ["git", "merge", "--no-commit"
-             f"{alias}/{branch}"],
+            ["git", "merge", "--no-commit" f"{alias}/{branch}"],
             cwd=work_dir,
             check=False,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL,
         )
         subprocess.run(
             ["git", "add", "."],
             cwd=work_dir,
             check=False,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL,
         )
         subprocess.run(
-            ["git", "commit"
-             "-m", "Force merged with conflicts"],
+            ["git", "commit" "-m", "Force merged with conflicts"],
             cwd=work_dir,
             check=False,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.DEVNULL,
         )
```

## mest/main.py

```diff
@@ -54,15 +54,15 @@
                 if children is not None:
                     for child in children:
                         pid_list.append(child.pid)
                 if parent.cmdline is not None:
                     cmdline = " ".join(parent.cmdline())
                     print(f"kill {parent.pid} {cmdline}")
                 parent.send_signal(sig)
-        except Exception:
+        except Exception as e:
             print(e)
 
 
 def init_check():
     if not os.path.exists(CONFIG_FILE):
         print(f"please set `{CONFIG_FILE}`")
         exit(1)
```

## Comparing `MeMeST-2024.4.977272.data/data/LICENSE` & `MeMeST-2024.5.419269.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `MeMeST-2024.4.977272.dist-info/LICENSE` & `MeMeST-2024.5.419269.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MeMeST-2024.4.977272.dist-info/METADATA` & `MeMeST-2024.5.419269.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeMeST
-Version: 2024.4.977272
+Version: 2024.5.419269
 Summary: Multi-Repository Sync Tool
 Author: Xin-Xin Ma
 License: GPL
 Project-URL: Source, https://github.com/xxmawhu/memest.git
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
```

## Comparing `MeMeST-2024.4.977272.dist-info/RECORD` & `MeMeST-2024.5.419269.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-MeMeST-2024.4.977272.data/data/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+MeMeST-2024.5.419269.data/data/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
 git_tools/__init__.py,sha256=-M_wTgmk-Pe-gzayRUsldMI8maSAQpgrCrKbiUQFV2o,76
 git_tools/base_dtypes.py,sha256=Y7F6fUoZvETZVV4EKpPnrfS3Qfeudb-Oojh-B93mSPQ,1139
-git_tools/git_api.py,sha256=wg81-9MGQzNznd1grVBMJT_Nsg561dBhlu_QWvkZnDQ,9002
+git_tools/git_api.py,sha256=D9w3gaNY04_Nf7KBBiFgjsVlxRO2SEbTnjSAkjZBUq4,9287
 git_tools/rep_task.py,sha256=vFPW1Z8mTIF0ZGJgaGF8AZM91A4Ogf_Sdo-bKtdo8-c,143
 mest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mest/config.py,sha256=YS4NJNE1fIAz0K3l7SreoqdtpM3nAJCe_oJc4LwREo0,4518
-mest/main.py,sha256=rvyuJhUCVRIm8c3s-zKh3fof8ACHyN4LPX43VBgQqL4,3400
+mest/main.py,sha256=FKTsqOmePiQK80kg0WU95d21fJ7U4AX8M0viQW5e5a8,3405
 mest/rep_mana.py,sha256=ZEhbeopuFBYIr4Eg64GUEQQ7M9bZZn0IFhmf3HJ2Mso,2717
 mest/test_git.py,sha256=BgD4moVzqnxfnhZzoM-EgHklAVFYPbtYu5Ke6qqFHhI,569
-MeMeST-2024.4.977272.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-MeMeST-2024.4.977272.dist-info/METADATA,sha256=29qA-hneEFkgyVL5-4EfK33SE-EdPrAkOAU5vLz4HvQ,1797
-MeMeST-2024.4.977272.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-MeMeST-2024.4.977272.dist-info/entry_points.txt,sha256=OYg2gMfzGJOXcQc_TTGdfCSPRPqlQylNW3LSReX_ta8,42
-MeMeST-2024.4.977272.dist-info/top_level.txt,sha256=iFxJRSyvq4K2f9Wl2wqP84mPUD7Ta4IoyDy9bDHkiYE,15
-MeMeST-2024.4.977272.dist-info/RECORD,,
+MeMeST-2024.5.419269.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+MeMeST-2024.5.419269.dist-info/METADATA,sha256=S1IYpOdkYXjQMKKnlCBswrn5bT9XeT2dThPXlXqJZrM,1797
+MeMeST-2024.5.419269.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+MeMeST-2024.5.419269.dist-info/entry_points.txt,sha256=OYg2gMfzGJOXcQc_TTGdfCSPRPqlQylNW3LSReX_ta8,42
+MeMeST-2024.5.419269.dist-info/top_level.txt,sha256=iFxJRSyvq4K2f9Wl2wqP84mPUD7Ta4IoyDy9bDHkiYE,15
+MeMeST-2024.5.419269.dist-info/RECORD,,
```

