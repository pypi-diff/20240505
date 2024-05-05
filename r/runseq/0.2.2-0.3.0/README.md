# Comparing `tmp/runseq-0.2.2.tar.gz` & `tmp/runseq-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runseq-0.2.2.tar", last modified: Wed May  1 14:21:50 2024, max compression
+gzip compressed data, was "runseq-0.3.0.tar", last modified: Sun May  5 21:41:01 2024, max compression
```

## Comparing `runseq-0.2.2.tar` & `runseq-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-05-01 14:21:50.729229 runseq-0.2.2/
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    35149 2024-04-23 13:58:13.000000 runseq-0.2.2/LICENSE
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43180 2024-05-01 14:21:50.729229 runseq-0.2.2/PKG-INFO
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)     2309 2024-05-01 13:43:31.000000 runseq-0.2.2/README.md
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      469 2024-05-01 14:21:19.000000 runseq-0.2.2/pyproject.toml
-drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-05-01 14:21:50.729229 runseq-0.2.2/runseq.egg-info/
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43180 2024-05-01 14:21:50.000000 runseq-0.2.2/runseq.egg-info/PKG-INFO
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      216 2024-05-01 14:21:50.000000 runseq-0.2.2/runseq.egg-info/SOURCES.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)        1 2024-05-01 14:21:50.000000 runseq-0.2.2/runseq.egg-info/dependency_links.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       39 2024-05-01 14:21:50.000000 runseq-0.2.2/runseq.egg-info/entry_points.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)        7 2024-05-01 14:21:50.000000 runseq-0.2.2/runseq.egg-info/top_level.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)     5932 2024-05-01 14:20:51.000000 runseq-0.2.2/runseq.py
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-05-01 14:21:50.729229 runseq-0.2.2/setup.cfg
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:30:44.000000 runseq-0.2.2/setup.py
+drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-05-05 21:41:01.397174 runseq-0.3.0/
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    35149 2024-04-23 13:58:13.000000 runseq-0.3.0/LICENSE
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43180 2024-05-05 21:41:01.397174 runseq-0.3.0/PKG-INFO
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)     2309 2024-05-01 13:43:31.000000 runseq-0.3.0/README.md
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)      469 2024-05-05 21:40:35.000000 runseq-0.3.0/pyproject.toml
+drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-05-05 21:41:01.397174 runseq-0.3.0/runseq.egg-info/
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43180 2024-05-05 21:41:01.000000 runseq-0.3.0/runseq.egg-info/PKG-INFO
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)      216 2024-05-05 21:41:01.000000 runseq-0.3.0/runseq.egg-info/SOURCES.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)        1 2024-05-05 21:41:01.000000 runseq-0.3.0/runseq.egg-info/dependency_links.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       39 2024-05-05 21:41:01.000000 runseq-0.3.0/runseq.egg-info/entry_points.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)        7 2024-05-05 21:41:01.000000 runseq-0.3.0/runseq.egg-info/top_level.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)     5927 2024-05-05 21:40:07.000000 runseq-0.3.0/runseq.py
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-05-05 21:41:01.397174 runseq-0.3.0/setup.cfg
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:30:44.000000 runseq-0.3.0/setup.py
```

### Comparing `runseq-0.2.2/LICENSE` & `runseq-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runseq-0.2.2/PKG-INFO` & `runseq-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runseq
-Version: 0.2.2
+Version: 0.3.0
 Summary: Simple job manager to run jobs sequentially in a Linux machine.
 Author-email: Luís Gomes <luismsgomes@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `runseq-0.2.2/README.md` & `runseq-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `runseq-0.2.2/runseq.egg-info/PKG-INFO` & `runseq-0.3.0/runseq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runseq
-Version: 0.2.2
+Version: 0.3.0
 Summary: Simple job manager to run jobs sequentially in a Linux machine.
 Author-email: Luís Gomes <luismsgomes@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `runseq-0.2.2/runseq.py` & `runseq-0.3.0/runseq.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,32 +164,33 @@
     parser_add.add_argument("command", type=str, help="the command to be executed")
     parser_add.add_argument("args", type=str, nargs="*", help="command arguments")
     subparsers.add_parser("list", aliases=["ls"], help="list jobs in the queue")
     parser_rm = subparsers.add_parser(
         "remove", aliases=["rm"], help="remove a job from the queue"
     )
     parser_rm.add_argument("job_id", type=int, help="the id of the job to be removed")
-    parser_clear = subparsers.add_parser(
+    parser_clear = subparsers.add_parser(  # noqa: F841
         "clear", aliases=["cl"], help="remove all finished jobs from the queue"
     )
-    parser_clear.add_argument("job_id", type=int, help="the id of the job to be removed")
     return parser.parse_args()
 
 
 def main():
     args = parse_commandline()
     if args.action == "run":
         run_jobs()
     elif args.action == "add":
         command = " ".join([args.command] + args.args)
         add_job(priority=args.priority, command=command)
     elif args.action in ["list", "ls"]:
         list_jobs()
     elif args.action in ["remove", "rm"]:
         remove_job(args.job_id)
+    elif args.action in ["clear", "cl"]:
+        clear_finished_jobs()
     else:
         print("invalid action:", args.action, file=sys.stderr)
         sys.exit(2)
 
 
 if __name__ == "__main__":
     main()
```

