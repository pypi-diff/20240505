# Comparing `tmp/miniwdl-omics-run-0.4.0.tar.gz` & `tmp/miniwdl_omics_run-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniwdl-omics-run-0.4.0.tar", last modified: Tue Dec 26 02:02:18 2023, max compression
+gzip compressed data, was "miniwdl_omics_run-0.5.0.tar", last modified: Sun May  5 20:39:15 2024, max compression
```

## Comparing `miniwdl-omics-run-0.4.0.tar` & `miniwdl_omics_run-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-12-26 02:02:18.346618 miniwdl-omics-run-0.4.0/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1830 2023-04-03 05:58:09.000000 miniwdl-omics-run-0.4.0/.gitignore
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      203 2023-04-03 05:53:41.000000 miniwdl-omics-run-0.4.0/.pre-commit-config.yaml
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     1056 2023-04-03 05:55:43.000000 miniwdl-omics-run-0.4.0/LICENSE
--rw-r--r--   0 mlin      (1000) mlin      (1000)     5600 2023-12-26 02:02:18.346618 miniwdl-omics-run-0.4.0/PKG-INFO
--rw-rw-r--   0 mlin      (1000) mlin      (1000)     4971 2023-12-26 02:01:05.000000 miniwdl-omics-run-0.4.0/README.md
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-12-26 02:02:18.346618 miniwdl-omics-run-0.4.0/miniwdl_omics_run/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       47 2023-04-03 05:53:41.000000 miniwdl-omics-run-0.4.0/miniwdl_omics_run/__init__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)    12817 2023-12-26 02:00:17.000000 miniwdl-omics-run-0.4.0/miniwdl_omics_run/__main__.py
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      411 2023-12-26 02:02:18.000000 miniwdl-omics-run-0.4.0/miniwdl_omics_run/_version.py
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-12-26 02:02:18.346618 miniwdl-omics-run-0.4.0/miniwdl_omics_run.egg-info/
--rw-r--r--   0 mlin      (1000) mlin      (1000)     5600 2023-12-26 02:02:18.000000 miniwdl-omics-run-0.4.0/miniwdl_omics_run.egg-info/PKG-INFO
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      446 2023-12-26 02:02:18.000000 miniwdl-omics-run-0.4.0/miniwdl_omics_run.egg-info/SOURCES.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)        1 2023-12-26 02:02:18.000000 miniwdl-omics-run-0.4.0/miniwdl_omics_run.egg-info/dependency_links.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      104 2023-12-26 02:02:18.000000 miniwdl-omics-run-0.4.0/miniwdl_omics_run.egg-info/entry_points.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       85 2023-12-26 02:02:18.000000 miniwdl-omics-run-0.4.0/miniwdl_omics_run.egg-info/requires.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       18 2023-12-26 02:02:18.000000 miniwdl-omics-run-0.4.0/miniwdl_omics_run.egg-info/top_level.txt
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      927 2023-04-04 03:16:29.000000 miniwdl-omics-run-0.4.0/pyproject.toml
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      118 2023-04-03 18:39:13.000000 miniwdl-omics-run-0.4.0/release.sh
--rw-rw-r--   0 mlin      (1000) mlin      (1000)       38 2023-12-26 02:02:18.346618 miniwdl-omics-run-0.4.0/setup.cfg
-drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2023-12-26 02:02:18.346618 miniwdl-omics-run-0.4.0/test/
--rw-rw-r--   0 mlin      (1000) mlin      (1000)      764 2023-09-09 08:36:32.000000 miniwdl-omics-run-0.4.0/test/TestFlow.wdl
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2024-05-05 20:39:15.690054 miniwdl_omics_run-0.5.0/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1830 2023-04-03 05:58:09.000000 miniwdl_omics_run-0.5.0/.gitignore
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      222 2024-05-05 20:35:44.000000 miniwdl_omics_run-0.5.0/.pre-commit-config.yaml
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     1056 2023-04-03 05:55:43.000000 miniwdl_omics_run-0.5.0/LICENSE
+-rw-r--r--   0 mlin      (1000) mlin      (1000)     5583 2024-05-05 20:39:15.690054 miniwdl_omics_run-0.5.0/PKG-INFO
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)     4991 2024-05-05 20:29:11.000000 miniwdl_omics_run-0.5.0/README.md
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2024-05-05 20:39:15.686054 miniwdl_omics_run-0.5.0/miniwdl_omics_run/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       47 2023-04-03 05:53:41.000000 miniwdl_omics_run-0.5.0/miniwdl_omics_run/__init__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)    13059 2024-05-05 20:33:51.000000 miniwdl_omics_run-0.5.0/miniwdl_omics_run/__main__.py
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      411 2024-05-05 20:39:15.000000 miniwdl_omics_run-0.5.0/miniwdl_omics_run/_version.py
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2024-05-05 20:39:15.686054 miniwdl_omics_run-0.5.0/miniwdl_omics_run.egg-info/
+-rw-r--r--   0 mlin      (1000) mlin      (1000)     5583 2024-05-05 20:39:15.000000 miniwdl_omics_run-0.5.0/miniwdl_omics_run.egg-info/PKG-INFO
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      446 2024-05-05 20:39:15.000000 miniwdl_omics_run-0.5.0/miniwdl_omics_run.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)        1 2024-05-05 20:39:15.000000 miniwdl_omics_run-0.5.0/miniwdl_omics_run.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      104 2024-05-05 20:39:15.000000 miniwdl_omics_run-0.5.0/miniwdl_omics_run.egg-info/entry_points.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       79 2024-05-05 20:39:15.000000 miniwdl_omics_run-0.5.0/miniwdl_omics_run.egg-info/requires.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       18 2024-05-05 20:39:15.000000 miniwdl_omics_run-0.5.0/miniwdl_omics_run.egg-info/top_level.txt
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      921 2024-05-05 20:35:23.000000 miniwdl_omics_run-0.5.0/pyproject.toml
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      118 2023-04-03 18:39:13.000000 miniwdl_omics_run-0.5.0/release.sh
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)       38 2024-05-05 20:39:15.690054 miniwdl_omics_run-0.5.0/setup.cfg
+drwxrwxr-x   0 mlin      (1000) mlin      (1000)        0 2024-05-05 20:39:15.686054 miniwdl_omics_run-0.5.0/test/
+-rw-rw-r--   0 mlin      (1000) mlin      (1000)      764 2023-09-09 08:36:32.000000 miniwdl_omics_run-0.5.0/test/TestFlow.wdl
```

### Comparing `miniwdl-omics-run-0.4.0/.gitignore` & `miniwdl_omics_run-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `miniwdl-omics-run-0.4.0/LICENSE` & `miniwdl_omics_run-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miniwdl-omics-run-0.4.0/PKG-INFO` & `miniwdl_omics_run-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: miniwdl-omics-run
-Version: 0.4.0
+Version: 0.5.0
 Summary: WDL launcher for Amazon Omics
 Project-URL: repository, https://github.com/miniwdl-ext/miniwdl-omics-run.git
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: miniwdl<2,>=1.9.1
-Requires-Dist: boto3>=1.26.42
+Requires-Dist: boto3>=1.34.98
 Provides-Extra: dev
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: black; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 
 # miniwdl-omics-run
 
 This command-line tool makes it easier to launch [WDL](https://openwdl.org/) runs on the [AWS HealthOmics](https://docs.aws.amazon.com/omics/latest/dev/workflows.html) workflow service. It uses [miniwdl](https://github.com/chanzuckerberg/miniwdl) locally to register WDL workflows, validate command-line inputs, and start a run.
 
 ```
 pip3 install miniwdl-omics-run
 
 miniwdl-omics-run \
-    --role-arn {SERVICE_ROLE_ARN} \
+    --role {SERVICE_ROLE_NAME} \
     --output-uri s3://{BUCKET_NAME}/{PREFIX} \
     {MAIN_WDL_FILE} input1=value1 input2=value2 ...
 ```
 
 ## Quick start
 
 Prerequisites: Unix command line with Python & pip; up-to-date [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) installed locally, and [configured](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html) with full access to your AWS account.
@@ -91,15 +90,15 @@
 
 Push a plain Ubuntu image to the repository.
 
 ```
 ECR_ENDPT="${AWS_ACCOUNT_ID}.dkr.ecr.${AWS_DEFAULT_REGION}.amazonaws.com"
 aws ecr get-login-password | docker login --username AWS --password-stdin "$ECR_ENDPT"
 
-docker pull ubuntu:22.04
+docker pull --platform linux/amd64 ubuntu:22.04
 docker tag ubuntu:22.04 "${ECR_ENDPT}/omics:ubuntu-22.04"
 docker push "${ECR_ENDPT}/omics:ubuntu-22.04"
 ```
 
 ### Run test workflow
 
 ```
```

### Comparing `miniwdl-omics-run-0.4.0/README.md` & `miniwdl_omics_run-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This command-line tool makes it easier to launch [WDL](https://openwdl.org/) runs on the [AWS HealthOmics](https://docs.aws.amazon.com/omics/latest/dev/workflows.html) workflow service. It uses [miniwdl](https://github.com/chanzuckerberg/miniwdl) locally to register WDL workflows, validate command-line inputs, and start a run.
 
 ```
 pip3 install miniwdl-omics-run
 
 miniwdl-omics-run \
-    --role-arn {SERVICE_ROLE_ARN} \
+    --role {SERVICE_ROLE_NAME} \
     --output-uri s3://{BUCKET_NAME}/{PREFIX} \
     {MAIN_WDL_FILE} input1=value1 input2=value2 ...
 ```
 
 ## Quick start
 
 Prerequisites: Unix command line with Python & pip; up-to-date [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) installed locally, and [configured](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html) with full access to your AWS account.
@@ -72,15 +72,15 @@
 
 Push a plain Ubuntu image to the repository.
 
 ```
 ECR_ENDPT="${AWS_ACCOUNT_ID}.dkr.ecr.${AWS_DEFAULT_REGION}.amazonaws.com"
 aws ecr get-login-password | docker login --username AWS --password-stdin "$ECR_ENDPT"
 
-docker pull ubuntu:22.04
+docker pull --platform linux/amd64 ubuntu:22.04
 docker tag ubuntu:22.04 "${ECR_ENDPT}/omics:ubuntu-22.04"
 docker push "${ECR_ENDPT}/omics:ubuntu-22.04"
 ```
 
 ### Run test workflow
 
 ```
```

### Comparing `miniwdl-omics-run-0.4.0/miniwdl_omics_run/__main__.py` & `miniwdl_omics_run-0.5.0/miniwdl_omics_run/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,28 +207,36 @@
     )
     group.add_argument(
         "--storage-capacity",
         type=int,
         help="Storage capacity in gigabytes",
         default=None,
     )
+    group.add_argument(
+        "--storage-type",
+        type=str,
+        choices=["STATIC", "DYNAMIC"],
+        default=None,
+    )
 
     return parser
 
 
 def start_run_options(args):
     ans = {}
     if args.name is not None:
         ans["name"] = args.name
     if args.priority is not None:
         ans["priority"] = args.priority
     if args.run_group_id is not None:
         ans["runGroupId"] = args.run_group_id
     if args.storage_capacity is not None:
         ans["storageCapacity"] = args.storage_capacity
+    if args.storage_type is not None:
+        ans["storageType"] = args.storage_type
     return ans
 
 
 class VersionAction(argparse.Action):
     def __init__(self, option_strings, dest, nargs=None, **kwargs):
         super().__init__(option_strings, dest, nargs=0, **kwargs)
 
@@ -250,15 +258,17 @@
     if not is_s3_uri(x):
         raise argparse.ArgumentTypeError("OUTPUT_S3_URI must be a s3:// URI")
     return x
 
 
 def check_uri_input(path, _is_directory):
     if not (is_s3_uri(path) or is_omics_uri(path)):
-        raise WDL.Error.InputError("File/Directory input is not a s3:// nor an omics:// URI: " + path)
+        raise WDL.Error.InputError(
+            "File/Directory input is not a s3:// nor an omics:// URI: " + path
+        )
     return path
 
 
 def ensure_omics_workflow(logger, cleanup, omics, wdl_doc, wdl_exe):
     """
     Get an Omics workflow id suitable for running the given WDL -- reusing an existing
     one if found, otherwise creating it.
```

### Comparing `miniwdl-omics-run-0.4.0/miniwdl_omics_run.egg-info/PKG-INFO` & `miniwdl_omics_run-0.5.0/miniwdl_omics_run.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: miniwdl-omics-run
-Version: 0.4.0
+Version: 0.5.0
 Summary: WDL launcher for Amazon Omics
 Project-URL: repository, https://github.com/miniwdl-ext/miniwdl-omics-run.git
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: miniwdl<2,>=1.9.1
-Requires-Dist: boto3>=1.26.42
+Requires-Dist: boto3>=1.34.98
 Provides-Extra: dev
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: black; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 
 # miniwdl-omics-run
 
 This command-line tool makes it easier to launch [WDL](https://openwdl.org/) runs on the [AWS HealthOmics](https://docs.aws.amazon.com/omics/latest/dev/workflows.html) workflow service. It uses [miniwdl](https://github.com/chanzuckerberg/miniwdl) locally to register WDL workflows, validate command-line inputs, and start a run.
 
 ```
 pip3 install miniwdl-omics-run
 
 miniwdl-omics-run \
-    --role-arn {SERVICE_ROLE_ARN} \
+    --role {SERVICE_ROLE_NAME} \
     --output-uri s3://{BUCKET_NAME}/{PREFIX} \
     {MAIN_WDL_FILE} input1=value1 input2=value2 ...
 ```
 
 ## Quick start
 
 Prerequisites: Unix command line with Python & pip; up-to-date [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) installed locally, and [configured](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html) with full access to your AWS account.
@@ -91,15 +90,15 @@
 
 Push a plain Ubuntu image to the repository.
 
 ```
 ECR_ENDPT="${AWS_ACCOUNT_ID}.dkr.ecr.${AWS_DEFAULT_REGION}.amazonaws.com"
 aws ecr get-login-password | docker login --username AWS --password-stdin "$ECR_ENDPT"
 
-docker pull ubuntu:22.04
+docker pull --platform linux/amd64 ubuntu:22.04
 docker tag ubuntu:22.04 "${ECR_ENDPT}/omics:ubuntu-22.04"
 docker push "${ECR_ENDPT}/omics:ubuntu-22.04"
 ```
 
 ### Run test workflow
 
 ```
```

### Comparing `miniwdl-omics-run-0.4.0/pyproject.toml` & `miniwdl_omics_run-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [project]
 name = "miniwdl-omics-run"
 description = "WDL launcher for Amazon Omics"
 dynamic = ["version"]
 readme = "./README.md"
 dependencies = [
   "miniwdl>=1.9.1,<2",
-  "boto3>=1.26.42",
+  "boto3>=1.34.98",
 ]
 requires-python = "~=3.8"
 urls = { repository = "https://github.com/miniwdl-ext/miniwdl-omics-run.git" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 
 
 [project.scripts]
@@ -25,23 +25,22 @@
 [project.optional-dependencies]
 # pip install --upgrade -e .[dev]
 dev = [
   "setuptools",
   "build",
   "twine",
   "pre-commit",
-  "black",
   "ruff",
 ]
 
 
 [tool.setuptools_scm]
 write_to = "miniwdl_omics_run/_version.py"
 
 
 [tool.setuptools.dynamic]
 version = {attr = "miniwdl_omics_run._version.__version__"}
 
 
 [tool.ruff]
-select = ["E", "F", "I"]
+lint.select = ["E", "F", "I"]
 line-length = 88
```

### Comparing `miniwdl-omics-run-0.4.0/test/TestFlow.wdl` & `miniwdl_omics_run-0.5.0/test/TestFlow.wdl`

 * *Files identical despite different names*

