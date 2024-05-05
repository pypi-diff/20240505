# Comparing `tmp/asynctnt-2.1.0a1.tar.gz` & `tmp/asynctnt-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynctnt-2.1.0a1.tar", last modified: Wed Dec 27 06:22:23 2023, max compression
+gzip compressed data, was "asynctnt-2.2.0.tar", last modified: Sun May  5 20:10:37 2024, max compression
```

## Comparing `asynctnt-2.1.0a1.tar` & `asynctnt-2.2.0.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.425199 asynctnt-2.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2023-12-27 06:22:23.425199 asynctnt-2.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.397199 asynctnt-2.1.0a1/asynctnt/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13956 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20512 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25943 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.409199 asynctnt-2.1.0a1/asynctnt/iproto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/bit.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    13423 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/buffer.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/cmsgpuck.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/const.pxi
--rw-r--r--   0 runner    (1001) docker     (127)      836 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/coreproto.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/coreproto.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/db.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/db.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/ext.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/ext.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  4468334 2023-12-27 06:22:22.000000 asynctnt-2.1.0a1/asynctnt/iproto/protocol.c
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-12-27 06:22:22.000000 asynctnt-2.1.0a1/asynctnt/iproto/protocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/protocol.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/protocol.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17426 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/protocol.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/push.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/push.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/python.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/rbuffer.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/rbuffer.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.413199 asynctnt-2.1.0a1/asynctnt/iproto/requests/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/auth.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/auth.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/base.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/base.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/call.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/call.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/delete.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/delete.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/eval.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/eval.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/execute.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/execute.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/id.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/id.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/insert.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/insert.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/ping.pxd
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/ping.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/prepare.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/prepare.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/select.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/select.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/streams.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/streams.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/update.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     7690 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/update.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/upsert.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/requests/upsert.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/response.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    20118 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/response.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/schema.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    11887 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/schema.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/tarantool.pxd
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/ttuple.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.413199 asynctnt-2.1.0a1/asynctnt/iproto/tupleobj/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/tupleobj/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    27202 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/tupleobj/tupleobj.c
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/tupleobj/tupleobj.h
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/unicodeutil.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/unicodeutil.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/iproto/xd.pxd
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/prepared.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/asynctnt/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.421199 asynctnt-2.1.0a1/asynctnt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2023-12-27 06:22:23.000000 asynctnt-2.1.0a1/asynctnt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2023-12-27 06:22:23.000000 asynctnt-2.1.0a1/asynctnt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 06:22:23.000000 asynctnt-2.1.0a1/asynctnt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 06:22:20.000000 asynctnt-2.1.0a1/asynctnt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-12-27 06:22:23.000000 asynctnt-2.1.0a1/asynctnt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 06:22:23.000000 asynctnt-2.1.0a1/asynctnt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 06:22:23.425199 asynctnt-2.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.417199 asynctnt-2.1.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/_testbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    27068 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10133 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_mp_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_sql_execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_sql_prepared.py
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_op_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/test_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.417199 asynctnt-2.1.0a1/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/tests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.417199 asynctnt-2.1.0a1/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.421199 asynctnt-2.1.0a1/third_party/msgpuck/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/.build.mk
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/.git
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    75166 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/Jenkinsfile
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.421199 asynctnt-2.1.0a1/third_party/msgpuck/debian/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/debian/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (127)        2 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/debian/compat
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/debian/control
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/debian/docs
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/debian/libmsgpuck-dev.manpages
--rwxr-xr-x   0 runner    (1001) docker     (127)      569 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.421199 asynctnt-2.1.0a1/third_party/msgpuck/debian/source/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/hints.c
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/msgpuck.c
--rw-r--r--   0 runner    (1001) docker     (127)    67074 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/msgpuck.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.421199 asynctnt-2.1.0a1/third_party/msgpuck/rpm/
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/rpm/msgpuck.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 06:22:23.421199 asynctnt-2.1.0a1/third_party/msgpuck/test/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/test/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38846 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/test/msgpuck.c
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/test/test.c
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2023-12-27 06:21:58.000000 asynctnt-2.1.0a1/third_party/msgpuck/test/test.h
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2023-12-27 06:21:57.000000 asynctnt-2.1.0a1/third_party/xd.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.609443 asynctnt-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 20:10:21.000000 asynctnt-2.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-05 20:10:21.000000 asynctnt-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-05 20:10:21.000000 asynctnt-2.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-05-05 20:10:37.609443 asynctnt-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-05 20:10:21.000000 asynctnt-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.581443 asynctnt-2.2.0/asynctnt/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20512 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25943 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.593443 asynctnt-2.2.0/asynctnt/iproto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/bit.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/buffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    13423 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/buffer.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/cmsgpuck.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/const.pxi
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/coreproto.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/coreproto.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/db.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/db.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/ext.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/ext.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  4467918 2024-05-05 20:10:37.000000 asynctnt-2.2.0/asynctnt/iproto/protocol.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-05 20:10:37.000000 asynctnt-2.2.0/asynctnt/iproto/protocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/protocol.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/protocol.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17426 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/protocol.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/push.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/push.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/python.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/rbuffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/rbuffer.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.597443 asynctnt-2.2.0/asynctnt/iproto/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/auth.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/auth.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/base.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/base.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/call.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/call.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/delete.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/delete.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/eval.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/eval.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/execute.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/execute.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/id.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/id.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/insert.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/insert.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/ping.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/ping.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/prepare.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/prepare.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/select.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/select.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/streams.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/streams.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/update.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/update.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/upsert.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/requests/upsert.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/response.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    20118 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/response.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/schema.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/schema.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/tarantool.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/ttuple.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.597443 asynctnt-2.2.0/asynctnt/iproto/tupleobj/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/tupleobj/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    27202 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/tupleobj/tupleobj.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/tupleobj/tupleobj.h
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/unicodeutil.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/unicodeutil.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/iproto/xd.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-05 20:10:21.000000 asynctnt-2.2.0/asynctnt/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.605443 asynctnt-2.2.0/asynctnt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-05-05 20:10:37.000000 asynctnt-2.2.0/asynctnt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-05 20:10:37.000000 asynctnt-2.2.0/asynctnt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:10:37.000000 asynctnt-2.2.0/asynctnt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:10:34.000000 asynctnt-2.2.0/asynctnt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-05 20:10:37.000000 asynctnt-2.2.0/asynctnt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 20:10:37.000000 asynctnt-2.2.0/asynctnt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-05 20:10:21.000000 asynctnt-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 20:10:37.609443 asynctnt-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-05 20:10:21.000000 asynctnt-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.601443 asynctnt-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/_testbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27068 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_mp_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_sql_execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_sql_prepared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15150 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_op_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.601443 asynctnt-2.2.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-05 20:10:21.000000 asynctnt-2.2.0/tests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.601443 asynctnt-2.2.0/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.605443 asynctnt-2.2.0/third_party/msgpuck/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/.build.mk
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-05 20:10:21.000000 asynctnt-2.2.0/third_party/msgpuck/.git
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    75166 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/Jenkinsfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.605443 asynctnt-2.2.0/third_party/msgpuck/debian/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/debian/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/debian/control
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/debian/docs
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/debian/libmsgpuck-dev.manpages
+-rwxr-xr-x   0 runner    (1001) docker     (127)      569 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.605443 asynctnt-2.2.0/third_party/msgpuck/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/hints.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/msgpuck.c
+-rw-r--r--   0 runner    (1001) docker     (127)    67074 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/msgpuck.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.605443 asynctnt-2.2.0/third_party/msgpuck/rpm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/rpm/msgpuck.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:10:37.605443 asynctnt-2.2.0/third_party/msgpuck/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/test/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38846 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/test/msgpuck.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/test/test.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-05 20:10:22.000000 asynctnt-2.2.0/third_party/msgpuck/test/test.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-05 20:10:21.000000 asynctnt-2.2.0/third_party/xd.h
```

### Comparing `asynctnt-2.1.0a1/LICENSE.txt` & `asynctnt-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/Makefile` & `asynctnt-2.2.0/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 	$(PYTHON) -m black .
 	$(PYTHON) -m isort .
 
 mypy:
 	$(PYTHON) -m mypy --enable-error-code ignore-without-code .
 
 ruff:
-	$(PYTHON) -m ruff .
+	$(PYTHON) -m ruff check .
 
 style-check:
 	$(PYTHON) -m black --check --diff .
 	$(PYTHON) -m isort --check --diff .
 
 lint: style-check ruff
```

### Comparing `asynctnt-2.1.0a1/PKG-INFO` & `asynctnt-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asynctnt
-Version: 2.1.0a1
+Version: 2.2.0
 Summary: A fast Tarantool Database connector for Python/asyncio.
 Author-email: igorcoding <igorcoding@gmail.com>
 License: Apache License, Version 2.0
 Project-URL: github, https://github.com/igorcoding/asynctnt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: POSIX
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asynctnt Version: 2.1.0a1 Summary: A fast Tarantool
+Metadata-Version: 2.1 Name: asynctnt Version: 2.2.0 Summary: A fast Tarantool
 Database connector for Python/asyncio. Author-email: igorcoding
 gmail.com> License: Apache License, Version 2.0 Project-URL: github, https://
 github.com/igorcoding/asynctnt Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: AsyncIO Classifier: Operating System
 :: POSIX Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
```

### Comparing `asynctnt-2.1.0a1/README.md` & `asynctnt-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/api.py` & `asynctnt-2.2.0/asynctnt/api.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/connection.py` & `asynctnt-2.2.0/asynctnt/connection.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/exceptions.py` & `asynctnt-2.2.0/asynctnt/exceptions.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/instance.py` & `asynctnt-2.2.0/asynctnt/instance.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/bit.pxd` & `asynctnt-2.2.0/asynctnt/iproto/bit.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/buffer.pxd` & `asynctnt-2.2.0/asynctnt/iproto/buffer.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/buffer.pyx` & `asynctnt-2.2.0/asynctnt/iproto/buffer.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/cmsgpuck.pxd` & `asynctnt-2.2.0/asynctnt/iproto/cmsgpuck.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/const.pxi` & `asynctnt-2.2.0/asynctnt/iproto/const.pxi`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/coreproto.pxd` & `asynctnt-2.2.0/asynctnt/iproto/coreproto.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/coreproto.pyx` & `asynctnt-2.2.0/asynctnt/iproto/coreproto.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/db.pxd` & `asynctnt-2.2.0/asynctnt/iproto/db.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/db.pyx` & `asynctnt-2.2.0/asynctnt/iproto/db.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/ext.pxd` & `asynctnt-2.2.0/asynctnt/iproto/ext.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/ext.pyx` & `asynctnt-2.2.0/asynctnt/iproto/ext.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/protocol.c` & `asynctnt-2.2.0/asynctnt/iproto/protocol.c`

 * *Files 0% similar despite different names*

```diff
@@ -1996,15 +1996,15 @@
   __pyx_e_8asynctnt_6iproto_8protocol_POST_CONNECTION_NONE = 0,
   __pyx_e_8asynctnt_6iproto_8protocol_POST_CONNECTION_ID = 10,
   __pyx_e_8asynctnt_6iproto_8protocol_POST_CONNECTION_AUTH = 20,
   __pyx_e_8asynctnt_6iproto_8protocol_POST_CONNECTION_SCHEMA = 30,
   __pyx_e_8asynctnt_6iproto_8protocol_POST_CONNECTION_DONE = 0x64
 };
 
-/* "asynctnt/iproto/schema.pxd":53
+/* "asynctnt/iproto/schema.pxd":54
  * 
  *     cdef void add_index(self, SchemaIndex idx)
  *     cdef SchemaIndex get_index(self, index, create_dummy=*)             # <<<<<<<<<<<<<<
  * 
  * 
  */
 struct __pyx_opt_args_8asynctnt_6iproto_8protocol_11SchemaSpace_get_index {
@@ -2092,15 +2092,15 @@
   PyObject *fields;
   PyObject *name_id_map;
   PyObject *names;
 };
 
 __PYX_EXTERN_C DL_EXPORT(PyTypeObject) C_Metadata_Type;
 
-/* "asynctnt/iproto/schema.pxd":26
+/* "asynctnt/iproto/schema.pxd":27
  * 
  * 
  * cdef class SchemaIndex:             # <<<<<<<<<<<<<<
  *     cdef:
  *         readonly int sid
  */
 struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex {
@@ -2110,27 +2110,27 @@
   PyObject *name;
   PyObject *index_type;
   PyObject *unique;
   struct C_Metadata *metadata;
 };
 
 
-/* "asynctnt/iproto/schema.pxd":36
+/* "asynctnt/iproto/schema.pxd":37
  * 
  * 
  * cdef class SchemaDummyIndex(SchemaIndex):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaDummyIndex {
   struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex __pyx_base;
 };
 
 
-/* "asynctnt/iproto/schema.pxd":40
+/* "asynctnt/iproto/schema.pxd":41
  * 
  * 
  * cdef class SchemaSpace:             # <<<<<<<<<<<<<<
  *     cdef:
  *         readonly int sid
  */
 struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace {
@@ -2143,27 +2143,27 @@
   int field_count;
   PyObject *flags;
   struct C_Metadata *metadata;
   PyObject *indexes;
 };
 
 
-/* "asynctnt/iproto/schema.pxd":56
+/* "asynctnt/iproto/schema.pxd":57
  * 
  * 
  * cdef class SchemaDummySpace(SchemaSpace):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaDummySpace {
   struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace __pyx_base;
 };
 
 
-/* "asynctnt/iproto/schema.pxd":60
+/* "asynctnt/iproto/schema.pxd":61
  * 
  * 
  * cdef class Schema:             # <<<<<<<<<<<<<<
  *     cdef:
  *         readonly dict spaces
  */
 struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema {
@@ -2663,23 +2663,25 @@
  */
 
 struct __pyx_vtabstruct_8asynctnt_6iproto_8protocol_Metadata {
   int (*len)(struct C_Metadata *);
   void (*add)(struct C_Metadata *, int, struct __pyx_obj_8asynctnt_6iproto_8protocol_Field *);
   PyObject *(*name_by_id)(struct C_Metadata *, int);
   int (*id_by_name)(struct C_Metadata *, PyObject *);
+  int (*id_by_name_safe)(struct C_Metadata *, PyObject *);
 };
 static struct __pyx_vtabstruct_8asynctnt_6iproto_8protocol_Metadata *__pyx_vtabptr_8asynctnt_6iproto_8protocol_Metadata;
 static CYTHON_INLINE int __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(struct C_Metadata *);
 static CYTHON_INLINE void __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_add(struct C_Metadata *, int, struct __pyx_obj_8asynctnt_6iproto_8protocol_Field *);
 static CYTHON_INLINE PyObject *__pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id(struct C_Metadata *, int);
 static CYTHON_INLINE int __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_id_by_name(struct C_Metadata *, PyObject *);
+static CYTHON_INLINE int __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_id_by_name_safe(struct C_Metadata *, PyObject *);
 
 
-/* "asynctnt/iproto/schema.pyx":79
+/* "asynctnt/iproto/schema.pyx":88
  * 
  * @cython.final
  * cdef class SchemaSpace:             # <<<<<<<<<<<<<<
  *     def __cinit__(self):
  *         self.sid = -1
  */
 
@@ -2688,29 +2690,29 @@
   struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *(*get_index)(struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *, PyObject *, struct __pyx_opt_args_8asynctnt_6iproto_8protocol_11SchemaSpace_get_index *__pyx_optional_args);
 };
 static struct __pyx_vtabstruct_8asynctnt_6iproto_8protocol_SchemaSpace *__pyx_vtabptr_8asynctnt_6iproto_8protocol_SchemaSpace;
 static void __pyx_f_8asynctnt_6iproto_8protocol_11SchemaSpace_add_index(struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *, struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *);
 static struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *__pyx_f_8asynctnt_6iproto_8protocol_11SchemaSpace_get_index(struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *, PyObject *, struct __pyx_opt_args_8asynctnt_6iproto_8protocol_11SchemaSpace_get_index *__pyx_optional_args);
 
 
-/* "asynctnt/iproto/schema.pxd":56
+/* "asynctnt/iproto/schema.pxd":57
  * 
  * 
  * cdef class SchemaDummySpace(SchemaSpace):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 
 struct __pyx_vtabstruct_8asynctnt_6iproto_8protocol_SchemaDummySpace {
   struct __pyx_vtabstruct_8asynctnt_6iproto_8protocol_SchemaSpace __pyx_base;
 };
 static struct __pyx_vtabstruct_8asynctnt_6iproto_8protocol_SchemaDummySpace *__pyx_vtabptr_8asynctnt_6iproto_8protocol_SchemaDummySpace;
 
 
-/* "asynctnt/iproto/schema.pyx":136
+/* "asynctnt/iproto/schema.pyx":145
  * 
  * @cython.final
  * cdef class Schema:             # <<<<<<<<<<<<<<
  *     def __cinit__(self, int schema_id):
  *         self.id = schema_id
  */
 
@@ -4376,14 +4378,15 @@
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_9timedelta_3day_day(PyDateTime_Delta *__pyx_v_self); /* proto*/
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_9timedelta_6second_second(PyDateTime_Delta *__pyx_v_self); /* proto*/
 static CYTHON_INLINE int __pyx_f_7cpython_8datetime_9timedelta_11microsecond_microsecond(PyDateTime_Delta *__pyx_v_self); /* proto*/
 static CYTHON_INLINE struct C_Metadata *__pyx_f_8asynctnt_6iproto_8protocol_11BaseRequest_metadata(struct __pyx_obj_8asynctnt_6iproto_8protocol_BaseRequest *__pyx_v_self); /* proto*/
 static CYTHON_INLINE void __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_add(struct C_Metadata *__pyx_v_self, int __pyx_v_id, struct __pyx_obj_8asynctnt_6iproto_8protocol_Field *__pyx_v_field); /* proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id(struct C_Metadata *__pyx_v_self, int __pyx_v_id); /* proto*/
 static CYTHON_INLINE int __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_id_by_name(struct C_Metadata *__pyx_v_self, PyObject *__pyx_v_name); /* proto*/
+static CYTHON_INLINE int __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_id_by_name_safe(struct C_Metadata *__pyx_v_self, PyObject *__pyx_v_name); /* proto*/
 static CYTHON_INLINE int __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(struct C_Metadata *__pyx_v_self); /* proto*/
 static void __pyx_f_8asynctnt_6iproto_8protocol_11SchemaSpace_add_index(struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *__pyx_v_self, struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *__pyx_v_idx); /* proto*/
 static struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *__pyx_f_8asynctnt_6iproto_8protocol_11SchemaSpace_get_index(struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *__pyx_v_self, PyObject *__pyx_v_index, struct __pyx_opt_args_8asynctnt_6iproto_8protocol_11SchemaSpace_get_index *__pyx_optional_args); /* proto*/
 static struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *__pyx_f_8asynctnt_6iproto_8protocol_6Schema_get_space(struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *__pyx_v_self, PyObject *__pyx_v_space); /* proto*/
 static struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *__pyx_f_8asynctnt_6iproto_8protocol_6Schema_get_or_create_space(struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *__pyx_v_self, PyObject *__pyx_v_space); /* proto*/
 static struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *__pyx_f_8asynctnt_6iproto_8protocol_6Schema_create_dummy_space(struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *__pyx_v_self, int __pyx_v_space_id); /* proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8asynctnt_6iproto_8protocol_6Schema_clear(struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *__pyx_v_self); /* proto*/
@@ -4690,33 +4693,33 @@
 static const char __pyx_k__3[] = "";
 static const char __pyx_k__5[] = ":";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_re[] = "re";
 static const char __pyx_k_02x[] = "{:02x}";
 static const char __pyx_k_ALL[] = "ALL";
 static const char __pyx_k_REQ[] = "REQ";
-static const char __pyx_k__15[] = ", ";
-static const char __pyx_k__18[] = " ... ";
-static const char __pyx_k__19[] = "[";
-static const char __pyx_k__20[] = "]";
-static const char __pyx_k__66[] = "*";
+static const char __pyx_k__14[] = ", ";
+static const char __pyx_k__17[] = " ... ";
+static const char __pyx_k__18[] = "[";
+static const char __pyx_k__19[] = "]";
+static const char __pyx_k__65[] = "*";
 static const char __pyx_k_doc[] = "__doc__";
 static const char __pyx_k_exc[] = "exc";
 static const char __pyx_k_fut[] = "fut";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_got[] = "{}, got: {}";
 static const char __pyx_k_hex[] = "hex";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_map[] = "map";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_req[] = "req";
 static const char __pyx_k_set[] = "set";
 static const char __pyx_k_ver[] = "ver";
 static const char __pyx_k_UUID[] = "UUID";
-static const char __pyx_k__212[] = "?";
+static const char __pyx_k__211[] = "?";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_call[] = "call";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_done[] = "done";
 static const char __pyx_k_enum[] = "enum";
 static const char __pyx_k_eval[] = "eval";
@@ -5159,15 +5162,14 @@
 static const char __pyx_k_IPROTO_FIELD_SPAN_must_be_either[] = "IPROTO_FIELD_SPAN must be either STR or NIL";
 static const char __pyx_k_IPROTO_STMT_ID_type_must_be_a_MP[] = "IPROTO_STMT_ID type must be a MP_UINT, but got ";
 static const char __pyx_k_IProtoErrorStackFrame___reduce_c[] = "IProtoErrorStackFrame.__reduce_cython__";
 static const char __pyx_k_IProtoErrorStackFrame___setstate[] = "IProtoErrorStackFrame.__setstate_cython__";
 static const char __pyx_k_Impossible_condition_happened_Pl[] = "Impossible condition happened. Please file a bug to https://github.com/igorcoding/asynctnt";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x9001016, 0xc05ea8e, 0xfe5f18a) = (check_schema_change, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))";
 static const char __pyx_k_Index_s_not_found_in_space_s_s_C[] = "Index %s not found in space %s/%s. Creating dummy.";
-static const char __pyx_k_Operation_field_no_must_be_int_a[] = "Operation field_no must be int as there is no format declaration in space {}";
 static const char __pyx_k_Operation_field_no_must_be_of_ei[] = "Operation field_no must be of either int or str type";
 static const char __pyx_k_Operation_length_must_be_at_leas[] = "Operation length must be at least 3";
 static const char __pyx_k_PrepareRequest___setstate_cython[] = "PrepareRequest.__setstate_cython__";
 static const char __pyx_k_Response_header_must_be_a_MP_MAP[] = "Response header must be a MP_MAP";
 static const char __pyx_k_RollbackRequest___setstate_cytho[] = "RollbackRequest.__setstate_cython__";
 static const char __pyx_k_Single_operation_must_be_a_tuple[] = "Single operation must be a tuple or list";
 static const char __pyx_k_Space_s_not_found_Creating_dummy[] = "Space %s not found. Creating dummy.";
@@ -5180,15 +5182,14 @@
 static const char __pyx_k_Tarantool_s_s_identified_success[] = "Tarantool[%s:%s] identified successfully";
 static const char __pyx_k_Time_zones_are_not_available_fro[] = "Time zones are not available from the C-API.";
 static const char __pyx_k_Tuple_must_be_an_array_when_deco[] = "Tuple must be an array when decoding as TarantoolTuple";
 static const char __pyx_k_Type_is_not_supported_for_encodi[] = "Type `{}` is not supported for encoding";
 static const char __pyx_k_Unknown_key_with_code_d_in_heade[] = "Unknown key with code '%d' in header. Skipping.";
 static const char __pyx_k_body_data_type_must_be_a_MP_ARRA[] = "body data type must be a MP_ARRAY";
 static const char __pyx_k_encoding_must_be_either_str_or_b[] = "encoding must be either str or bytes";
-static const char __pyx_k_int_argument_required_for_Arithm[] = "int argument required for Arithmetic and Delete operations";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_schema_id_type_must_be_a_MP_UINT[] = "schema_id type must be a MP_UINT";
 static const char __pyx_k_self_execute_cannot_be_converted[] = "self.execute cannot be converted to a Python object for pickling";
 static const char __pyx_k_sequence_must_be_either_list_tup[] = "sequence must be either list, tuple or dict";
 static const char __pyx_k_unknown_iproto_error_map_field_w[] = "unknown iproto_error map field with key ";
 static const char __pyx_k_unknown_iproto_error_stack_eleme[] = "unknown iproto_error stack element with key ";
 static const char __pyx_k_unknown_key_in_metadata_decoding[] = "unknown key in metadata decoding: %d";
@@ -5819,15 +5820,14 @@
   PyObject *__pyx_n_s_Metadata;
   PyObject *__pyx_n_s_Metadata___reduce_cython;
   PyObject *__pyx_n_s_Metadata___setstate_cython;
   PyObject *__pyx_kp_u_Metadata_fields_count;
   PyObject *__pyx_n_s_NEIGHBOR;
   PyObject *__pyx_n_s_OVERLAPS;
   PyObject *__pyx_kp_u_Offset_incorrect_Got_use_len;
-  PyObject *__pyx_kp_u_Operation_field_no_must_be_int_a;
   PyObject *__pyx_kp_u_Operation_field_no_must_be_of_ei;
   PyObject *__pyx_kp_u_Operation_length_must_be_at_leas;
   PyObject *__pyx_kp_u_Operation_type_must_of_a_str_or;
   PyObject *__pyx_n_s_Optional;
   PyObject *__pyx_kp_u_Part_len_must_be_2;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_PingRequest;
@@ -5914,23 +5914,23 @@
   PyObject *__pyx_n_s_UpsertRequest___setstate_cython;
   PyObject *__pyx_n_s_VERSION_STRING_REGEX;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_WriteBuffer;
   PyObject *__pyx_n_s_WriteBuffer___reduce_cython;
   PyObject *__pyx_n_s_WriteBuffer___setstate_cython;
   PyObject *__pyx_n_s_WriteBuffer_hex;
-  PyObject *__pyx_kp_u__15;
+  PyObject *__pyx_kp_u__14;
+  PyObject *__pyx_kp_u__17;
   PyObject *__pyx_kp_u__18;
   PyObject *__pyx_kp_u__19;
   PyObject *__pyx_kp_u__2;
-  PyObject *__pyx_kp_u__20;
-  PyObject *__pyx_n_s__212;
+  PyObject *__pyx_n_s__211;
   PyObject *__pyx_kp_u__3;
   PyObject *__pyx_kp_u__5;
-  PyObject *__pyx_n_s__66;
+  PyObject *__pyx_n_s__65;
   PyObject *__pyx_n_s_add_done_callback;
   PyObject *__pyx_n_s_anext;
   PyObject *__pyx_n_s_append;
   PyObject *__pyx_n_s_args;
   PyObject *__pyx_n_s_as_tuple;
   PyObject *__pyx_n_u_ascii;
   PyObject *__pyx_n_s_asyncio;
@@ -6034,15 +6034,14 @@
   PyObject *__pyx_n_s_indexes;
   PyObject *__pyx_n_s_init;
   PyObject *__pyx_n_s_init_subclass;
   PyObject *__pyx_n_s_initial_read_buffer_size;
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_insert;
   PyObject *__pyx_n_s_inspect;
-  PyObject *__pyx_kp_u_int_argument_required_for_Arithm;
   PyObject *__pyx_kp_u_invalid_datetime_size_got_extra;
   PyObject *__pyx_kp_u_iproto_error_stack_frame_fields;
   PyObject *__pyx_n_s_is_connected;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_n_s_is_fully_connected;
   PyObject *__pyx_n_u_is_nullable;
   PyObject *__pyx_kp_u_isenabled;
@@ -6269,22 +6268,22 @@
   PyObject *__pyx_int_neg_2;
   PyObject *__pyx_tuple_;
   PyObject *__pyx_tuple__4;
   PyObject *__pyx_tuple__6;
   PyObject *__pyx_tuple__7;
   PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__9;
+  PyObject *__pyx_slice__15;
   PyObject *__pyx_slice__16;
-  PyObject *__pyx_slice__17;
-  PyObject *__pyx_slice__40;
+  PyObject *__pyx_slice__39;
   PyObject *__pyx_tuple__10;
   PyObject *__pyx_tuple__11;
   PyObject *__pyx_tuple__12;
   PyObject *__pyx_tuple__13;
-  PyObject *__pyx_tuple__14;
+  PyObject *__pyx_tuple__20;
   PyObject *__pyx_tuple__21;
   PyObject *__pyx_tuple__22;
   PyObject *__pyx_tuple__23;
   PyObject *__pyx_tuple__24;
   PyObject *__pyx_tuple__25;
   PyObject *__pyx_tuple__26;
   PyObject *__pyx_tuple__27;
@@ -6295,18 +6294,18 @@
   PyObject *__pyx_tuple__32;
   PyObject *__pyx_tuple__33;
   PyObject *__pyx_tuple__34;
   PyObject *__pyx_tuple__35;
   PyObject *__pyx_tuple__36;
   PyObject *__pyx_tuple__37;
   PyObject *__pyx_tuple__38;
-  PyObject *__pyx_tuple__39;
+  PyObject *__pyx_tuple__40;
   PyObject *__pyx_tuple__41;
-  PyObject *__pyx_tuple__42;
-  PyObject *__pyx_tuple__45;
+  PyObject *__pyx_tuple__44;
+  PyObject *__pyx_tuple__46;
   PyObject *__pyx_tuple__47;
   PyObject *__pyx_tuple__48;
   PyObject *__pyx_tuple__49;
   PyObject *__pyx_tuple__50;
   PyObject *__pyx_tuple__51;
   PyObject *__pyx_tuple__52;
   PyObject *__pyx_tuple__53;
@@ -6317,67 +6316,67 @@
   PyObject *__pyx_tuple__58;
   PyObject *__pyx_tuple__59;
   PyObject *__pyx_tuple__60;
   PyObject *__pyx_tuple__61;
   PyObject *__pyx_tuple__62;
   PyObject *__pyx_tuple__63;
   PyObject *__pyx_tuple__64;
-  PyObject *__pyx_tuple__65;
-  PyObject *__pyx_tuple__67;
-  PyObject *__pyx_tuple__69;
-  PyObject *__pyx_tuple__79;
-  PyObject *__pyx_tuple__85;
-  PyObject *__pyx_tuple__125;
-  PyObject *__pyx_tuple__127;
+  PyObject *__pyx_tuple__66;
+  PyObject *__pyx_tuple__68;
+  PyObject *__pyx_tuple__78;
+  PyObject *__pyx_tuple__84;
+  PyObject *__pyx_tuple__124;
+  PyObject *__pyx_tuple__126;
+  PyObject *__pyx_tuple__128;
   PyObject *__pyx_tuple__129;
-  PyObject *__pyx_tuple__130;
-  PyObject *__pyx_tuple__132;
-  PyObject *__pyx_tuple__134;
-  PyObject *__pyx_tuple__136;
+  PyObject *__pyx_tuple__131;
+  PyObject *__pyx_tuple__133;
+  PyObject *__pyx_tuple__135;
+  PyObject *__pyx_tuple__137;
   PyObject *__pyx_tuple__138;
-  PyObject *__pyx_tuple__139;
+  PyObject *__pyx_tuple__140;
   PyObject *__pyx_tuple__141;
-  PyObject *__pyx_tuple__142;
-  PyObject *__pyx_tuple__144;
+  PyObject *__pyx_tuple__143;
+  PyObject *__pyx_tuple__145;
   PyObject *__pyx_tuple__146;
-  PyObject *__pyx_tuple__147;
-  PyObject *__pyx_tuple__149;
-  PyObject *__pyx_tuple__151;
+  PyObject *__pyx_tuple__148;
+  PyObject *__pyx_tuple__150;
+  PyObject *__pyx_tuple__152;
   PyObject *__pyx_tuple__153;
-  PyObject *__pyx_tuple__154;
-  PyObject *__pyx_tuple__156;
-  PyObject *__pyx_tuple__158;
-  PyObject *__pyx_tuple__165;
-  PyObject *__pyx_tuple__169;
-  PyObject *__pyx_tuple__171;
-  PyObject *__pyx_tuple__173;
-  PyObject *__pyx_tuple__175;
-  PyObject *__pyx_tuple__180;
-  PyObject *__pyx_tuple__182;
-  PyObject *__pyx_tuple__184;
-  PyObject *__pyx_tuple__186;
-  PyObject *__pyx_tuple__191;
+  PyObject *__pyx_tuple__155;
+  PyObject *__pyx_tuple__157;
+  PyObject *__pyx_tuple__164;
+  PyObject *__pyx_tuple__168;
+  PyObject *__pyx_tuple__170;
+  PyObject *__pyx_tuple__172;
+  PyObject *__pyx_tuple__174;
+  PyObject *__pyx_tuple__179;
+  PyObject *__pyx_tuple__181;
+  PyObject *__pyx_tuple__183;
+  PyObject *__pyx_tuple__185;
+  PyObject *__pyx_tuple__190;
+  PyObject *__pyx_codeobj__42;
   PyObject *__pyx_codeobj__43;
-  PyObject *__pyx_codeobj__44;
-  PyObject *__pyx_codeobj__46;
-  PyObject *__pyx_codeobj__68;
+  PyObject *__pyx_codeobj__45;
+  PyObject *__pyx_codeobj__67;
+  PyObject *__pyx_codeobj__69;
   PyObject *__pyx_codeobj__70;
   PyObject *__pyx_codeobj__71;
   PyObject *__pyx_codeobj__72;
   PyObject *__pyx_codeobj__73;
   PyObject *__pyx_codeobj__74;
   PyObject *__pyx_codeobj__75;
   PyObject *__pyx_codeobj__76;
   PyObject *__pyx_codeobj__77;
-  PyObject *__pyx_codeobj__78;
+  PyObject *__pyx_codeobj__79;
   PyObject *__pyx_codeobj__80;
   PyObject *__pyx_codeobj__81;
   PyObject *__pyx_codeobj__82;
   PyObject *__pyx_codeobj__83;
-  PyObject *__pyx_codeobj__84;
+  PyObject *__pyx_codeobj__85;
   PyObject *__pyx_codeobj__86;
   PyObject *__pyx_codeobj__87;
   PyObject *__pyx_codeobj__88;
   PyObject *__pyx_codeobj__89;
   PyObject *__pyx_codeobj__90;
   PyObject *__pyx_codeobj__91;
   PyObject *__pyx_codeobj__92;
@@ -6408,52 +6407,52 @@
   PyObject *__pyx_codeobj__117;
   PyObject *__pyx_codeobj__118;
   PyObject *__pyx_codeobj__119;
   PyObject *__pyx_codeobj__120;
   PyObject *__pyx_codeobj__121;
   PyObject *__pyx_codeobj__122;
   PyObject *__pyx_codeobj__123;
-  PyObject *__pyx_codeobj__124;
-  PyObject *__pyx_codeobj__126;
-  PyObject *__pyx_codeobj__128;
-  PyObject *__pyx_codeobj__131;
-  PyObject *__pyx_codeobj__133;
-  PyObject *__pyx_codeobj__135;
-  PyObject *__pyx_codeobj__137;
-  PyObject *__pyx_codeobj__140;
-  PyObject *__pyx_codeobj__143;
-  PyObject *__pyx_codeobj__145;
-  PyObject *__pyx_codeobj__148;
-  PyObject *__pyx_codeobj__150;
-  PyObject *__pyx_codeobj__152;
-  PyObject *__pyx_codeobj__155;
-  PyObject *__pyx_codeobj__157;
+  PyObject *__pyx_codeobj__125;
+  PyObject *__pyx_codeobj__127;
+  PyObject *__pyx_codeobj__130;
+  PyObject *__pyx_codeobj__132;
+  PyObject *__pyx_codeobj__134;
+  PyObject *__pyx_codeobj__136;
+  PyObject *__pyx_codeobj__139;
+  PyObject *__pyx_codeobj__142;
+  PyObject *__pyx_codeobj__144;
+  PyObject *__pyx_codeobj__147;
+  PyObject *__pyx_codeobj__149;
+  PyObject *__pyx_codeobj__151;
+  PyObject *__pyx_codeobj__154;
+  PyObject *__pyx_codeobj__156;
+  PyObject *__pyx_codeobj__158;
   PyObject *__pyx_codeobj__159;
   PyObject *__pyx_codeobj__160;
   PyObject *__pyx_codeobj__161;
   PyObject *__pyx_codeobj__162;
   PyObject *__pyx_codeobj__163;
-  PyObject *__pyx_codeobj__164;
+  PyObject *__pyx_codeobj__165;
   PyObject *__pyx_codeobj__166;
   PyObject *__pyx_codeobj__167;
-  PyObject *__pyx_codeobj__168;
-  PyObject *__pyx_codeobj__170;
-  PyObject *__pyx_codeobj__172;
-  PyObject *__pyx_codeobj__174;
+  PyObject *__pyx_codeobj__169;
+  PyObject *__pyx_codeobj__171;
+  PyObject *__pyx_codeobj__173;
+  PyObject *__pyx_codeobj__175;
   PyObject *__pyx_codeobj__176;
   PyObject *__pyx_codeobj__177;
   PyObject *__pyx_codeobj__178;
-  PyObject *__pyx_codeobj__179;
-  PyObject *__pyx_codeobj__181;
-  PyObject *__pyx_codeobj__183;
-  PyObject *__pyx_codeobj__185;
+  PyObject *__pyx_codeobj__180;
+  PyObject *__pyx_codeobj__182;
+  PyObject *__pyx_codeobj__184;
+  PyObject *__pyx_codeobj__186;
   PyObject *__pyx_codeobj__187;
   PyObject *__pyx_codeobj__188;
   PyObject *__pyx_codeobj__189;
-  PyObject *__pyx_codeobj__190;
+  PyObject *__pyx_codeobj__191;
   PyObject *__pyx_codeobj__192;
   PyObject *__pyx_codeobj__193;
   PyObject *__pyx_codeobj__194;
   PyObject *__pyx_codeobj__195;
   PyObject *__pyx_codeobj__196;
   PyObject *__pyx_codeobj__197;
   PyObject *__pyx_codeobj__198;
@@ -6465,15 +6464,14 @@
   PyObject *__pyx_codeobj__204;
   PyObject *__pyx_codeobj__205;
   PyObject *__pyx_codeobj__206;
   PyObject *__pyx_codeobj__207;
   PyObject *__pyx_codeobj__208;
   PyObject *__pyx_codeobj__209;
   PyObject *__pyx_codeobj__210;
-  PyObject *__pyx_codeobj__211;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -6752,15 +6750,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Metadata);
   Py_CLEAR(clear_module_state->__pyx_n_s_Metadata___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Metadata___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Metadata_fields_count);
   Py_CLEAR(clear_module_state->__pyx_n_s_NEIGHBOR);
   Py_CLEAR(clear_module_state->__pyx_n_s_OVERLAPS);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Offset_incorrect_Got_use_len);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_Operation_field_no_must_be_int_a);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Operation_field_no_must_be_of_ei);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Operation_length_must_be_at_leas);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Operation_type_must_of_a_str_or);
   Py_CLEAR(clear_module_state->__pyx_n_s_Optional);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Part_len_must_be_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_PingRequest);
@@ -6847,23 +6844,23 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_UpsertRequest___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_VERSION_STRING_REGEX);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_WriteBuffer);
   Py_CLEAR(clear_module_state->__pyx_n_s_WriteBuffer___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_WriteBuffer___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_WriteBuffer_hex);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__15);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__14);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__17);
   Py_CLEAR(clear_module_state->__pyx_kp_u__18);
   Py_CLEAR(clear_module_state->__pyx_kp_u__19);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__20);
-  Py_CLEAR(clear_module_state->__pyx_n_s__212);
+  Py_CLEAR(clear_module_state->__pyx_n_s__211);
   Py_CLEAR(clear_module_state->__pyx_kp_u__3);
   Py_CLEAR(clear_module_state->__pyx_kp_u__5);
-  Py_CLEAR(clear_module_state->__pyx_n_s__66);
+  Py_CLEAR(clear_module_state->__pyx_n_s__65);
   Py_CLEAR(clear_module_state->__pyx_n_s_add_done_callback);
   Py_CLEAR(clear_module_state->__pyx_n_s_anext);
   Py_CLEAR(clear_module_state->__pyx_n_s_append);
   Py_CLEAR(clear_module_state->__pyx_n_s_args);
   Py_CLEAR(clear_module_state->__pyx_n_s_as_tuple);
   Py_CLEAR(clear_module_state->__pyx_n_u_ascii);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio);
@@ -6967,15 +6964,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_indexes);
   Py_CLEAR(clear_module_state->__pyx_n_s_init);
   Py_CLEAR(clear_module_state->__pyx_n_s_init_subclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_initial_read_buffer_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_insert);
   Py_CLEAR(clear_module_state->__pyx_n_s_inspect);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_int_argument_required_for_Arithm);
   Py_CLEAR(clear_module_state->__pyx_kp_u_invalid_datetime_size_got_extra);
   Py_CLEAR(clear_module_state->__pyx_kp_u_iproto_error_stack_frame_fields);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_connected);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_fully_connected);
   Py_CLEAR(clear_module_state->__pyx_n_u_is_nullable);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
@@ -7202,22 +7198,22 @@
   Py_CLEAR(clear_module_state->__pyx_int_neg_2);
   Py_CLEAR(clear_module_state->__pyx_tuple_);
   Py_CLEAR(clear_module_state->__pyx_tuple__4);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
   Py_CLEAR(clear_module_state->__pyx_tuple__7);
   Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__9);
+  Py_CLEAR(clear_module_state->__pyx_slice__15);
   Py_CLEAR(clear_module_state->__pyx_slice__16);
-  Py_CLEAR(clear_module_state->__pyx_slice__17);
-  Py_CLEAR(clear_module_state->__pyx_slice__40);
+  Py_CLEAR(clear_module_state->__pyx_slice__39);
   Py_CLEAR(clear_module_state->__pyx_tuple__10);
   Py_CLEAR(clear_module_state->__pyx_tuple__11);
   Py_CLEAR(clear_module_state->__pyx_tuple__12);
   Py_CLEAR(clear_module_state->__pyx_tuple__13);
-  Py_CLEAR(clear_module_state->__pyx_tuple__14);
+  Py_CLEAR(clear_module_state->__pyx_tuple__20);
   Py_CLEAR(clear_module_state->__pyx_tuple__21);
   Py_CLEAR(clear_module_state->__pyx_tuple__22);
   Py_CLEAR(clear_module_state->__pyx_tuple__23);
   Py_CLEAR(clear_module_state->__pyx_tuple__24);
   Py_CLEAR(clear_module_state->__pyx_tuple__25);
   Py_CLEAR(clear_module_state->__pyx_tuple__26);
   Py_CLEAR(clear_module_state->__pyx_tuple__27);
@@ -7228,18 +7224,18 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__32);
   Py_CLEAR(clear_module_state->__pyx_tuple__33);
   Py_CLEAR(clear_module_state->__pyx_tuple__34);
   Py_CLEAR(clear_module_state->__pyx_tuple__35);
   Py_CLEAR(clear_module_state->__pyx_tuple__36);
   Py_CLEAR(clear_module_state->__pyx_tuple__37);
   Py_CLEAR(clear_module_state->__pyx_tuple__38);
-  Py_CLEAR(clear_module_state->__pyx_tuple__39);
+  Py_CLEAR(clear_module_state->__pyx_tuple__40);
   Py_CLEAR(clear_module_state->__pyx_tuple__41);
-  Py_CLEAR(clear_module_state->__pyx_tuple__42);
-  Py_CLEAR(clear_module_state->__pyx_tuple__45);
+  Py_CLEAR(clear_module_state->__pyx_tuple__44);
+  Py_CLEAR(clear_module_state->__pyx_tuple__46);
   Py_CLEAR(clear_module_state->__pyx_tuple__47);
   Py_CLEAR(clear_module_state->__pyx_tuple__48);
   Py_CLEAR(clear_module_state->__pyx_tuple__49);
   Py_CLEAR(clear_module_state->__pyx_tuple__50);
   Py_CLEAR(clear_module_state->__pyx_tuple__51);
   Py_CLEAR(clear_module_state->__pyx_tuple__52);
   Py_CLEAR(clear_module_state->__pyx_tuple__53);
@@ -7250,67 +7246,67 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__58);
   Py_CLEAR(clear_module_state->__pyx_tuple__59);
   Py_CLEAR(clear_module_state->__pyx_tuple__60);
   Py_CLEAR(clear_module_state->__pyx_tuple__61);
   Py_CLEAR(clear_module_state->__pyx_tuple__62);
   Py_CLEAR(clear_module_state->__pyx_tuple__63);
   Py_CLEAR(clear_module_state->__pyx_tuple__64);
-  Py_CLEAR(clear_module_state->__pyx_tuple__65);
-  Py_CLEAR(clear_module_state->__pyx_tuple__67);
-  Py_CLEAR(clear_module_state->__pyx_tuple__69);
-  Py_CLEAR(clear_module_state->__pyx_tuple__79);
-  Py_CLEAR(clear_module_state->__pyx_tuple__85);
-  Py_CLEAR(clear_module_state->__pyx_tuple__125);
-  Py_CLEAR(clear_module_state->__pyx_tuple__127);
+  Py_CLEAR(clear_module_state->__pyx_tuple__66);
+  Py_CLEAR(clear_module_state->__pyx_tuple__68);
+  Py_CLEAR(clear_module_state->__pyx_tuple__78);
+  Py_CLEAR(clear_module_state->__pyx_tuple__84);
+  Py_CLEAR(clear_module_state->__pyx_tuple__124);
+  Py_CLEAR(clear_module_state->__pyx_tuple__126);
+  Py_CLEAR(clear_module_state->__pyx_tuple__128);
   Py_CLEAR(clear_module_state->__pyx_tuple__129);
-  Py_CLEAR(clear_module_state->__pyx_tuple__130);
-  Py_CLEAR(clear_module_state->__pyx_tuple__132);
-  Py_CLEAR(clear_module_state->__pyx_tuple__134);
-  Py_CLEAR(clear_module_state->__pyx_tuple__136);
+  Py_CLEAR(clear_module_state->__pyx_tuple__131);
+  Py_CLEAR(clear_module_state->__pyx_tuple__133);
+  Py_CLEAR(clear_module_state->__pyx_tuple__135);
+  Py_CLEAR(clear_module_state->__pyx_tuple__137);
   Py_CLEAR(clear_module_state->__pyx_tuple__138);
-  Py_CLEAR(clear_module_state->__pyx_tuple__139);
+  Py_CLEAR(clear_module_state->__pyx_tuple__140);
   Py_CLEAR(clear_module_state->__pyx_tuple__141);
-  Py_CLEAR(clear_module_state->__pyx_tuple__142);
-  Py_CLEAR(clear_module_state->__pyx_tuple__144);
+  Py_CLEAR(clear_module_state->__pyx_tuple__143);
+  Py_CLEAR(clear_module_state->__pyx_tuple__145);
   Py_CLEAR(clear_module_state->__pyx_tuple__146);
-  Py_CLEAR(clear_module_state->__pyx_tuple__147);
-  Py_CLEAR(clear_module_state->__pyx_tuple__149);
-  Py_CLEAR(clear_module_state->__pyx_tuple__151);
+  Py_CLEAR(clear_module_state->__pyx_tuple__148);
+  Py_CLEAR(clear_module_state->__pyx_tuple__150);
+  Py_CLEAR(clear_module_state->__pyx_tuple__152);
   Py_CLEAR(clear_module_state->__pyx_tuple__153);
-  Py_CLEAR(clear_module_state->__pyx_tuple__154);
-  Py_CLEAR(clear_module_state->__pyx_tuple__156);
-  Py_CLEAR(clear_module_state->__pyx_tuple__158);
-  Py_CLEAR(clear_module_state->__pyx_tuple__165);
-  Py_CLEAR(clear_module_state->__pyx_tuple__169);
-  Py_CLEAR(clear_module_state->__pyx_tuple__171);
-  Py_CLEAR(clear_module_state->__pyx_tuple__173);
-  Py_CLEAR(clear_module_state->__pyx_tuple__175);
-  Py_CLEAR(clear_module_state->__pyx_tuple__180);
-  Py_CLEAR(clear_module_state->__pyx_tuple__182);
-  Py_CLEAR(clear_module_state->__pyx_tuple__184);
-  Py_CLEAR(clear_module_state->__pyx_tuple__186);
-  Py_CLEAR(clear_module_state->__pyx_tuple__191);
+  Py_CLEAR(clear_module_state->__pyx_tuple__155);
+  Py_CLEAR(clear_module_state->__pyx_tuple__157);
+  Py_CLEAR(clear_module_state->__pyx_tuple__164);
+  Py_CLEAR(clear_module_state->__pyx_tuple__168);
+  Py_CLEAR(clear_module_state->__pyx_tuple__170);
+  Py_CLEAR(clear_module_state->__pyx_tuple__172);
+  Py_CLEAR(clear_module_state->__pyx_tuple__174);
+  Py_CLEAR(clear_module_state->__pyx_tuple__179);
+  Py_CLEAR(clear_module_state->__pyx_tuple__181);
+  Py_CLEAR(clear_module_state->__pyx_tuple__183);
+  Py_CLEAR(clear_module_state->__pyx_tuple__185);
+  Py_CLEAR(clear_module_state->__pyx_tuple__190);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__42);
   Py_CLEAR(clear_module_state->__pyx_codeobj__43);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__44);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__46);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__68);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__45);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__67);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__69);
   Py_CLEAR(clear_module_state->__pyx_codeobj__70);
   Py_CLEAR(clear_module_state->__pyx_codeobj__71);
   Py_CLEAR(clear_module_state->__pyx_codeobj__72);
   Py_CLEAR(clear_module_state->__pyx_codeobj__73);
   Py_CLEAR(clear_module_state->__pyx_codeobj__74);
   Py_CLEAR(clear_module_state->__pyx_codeobj__75);
   Py_CLEAR(clear_module_state->__pyx_codeobj__76);
   Py_CLEAR(clear_module_state->__pyx_codeobj__77);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__78);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__79);
   Py_CLEAR(clear_module_state->__pyx_codeobj__80);
   Py_CLEAR(clear_module_state->__pyx_codeobj__81);
   Py_CLEAR(clear_module_state->__pyx_codeobj__82);
   Py_CLEAR(clear_module_state->__pyx_codeobj__83);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__84);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__85);
   Py_CLEAR(clear_module_state->__pyx_codeobj__86);
   Py_CLEAR(clear_module_state->__pyx_codeobj__87);
   Py_CLEAR(clear_module_state->__pyx_codeobj__88);
   Py_CLEAR(clear_module_state->__pyx_codeobj__89);
   Py_CLEAR(clear_module_state->__pyx_codeobj__90);
   Py_CLEAR(clear_module_state->__pyx_codeobj__91);
   Py_CLEAR(clear_module_state->__pyx_codeobj__92);
@@ -7341,52 +7337,52 @@
   Py_CLEAR(clear_module_state->__pyx_codeobj__117);
   Py_CLEAR(clear_module_state->__pyx_codeobj__118);
   Py_CLEAR(clear_module_state->__pyx_codeobj__119);
   Py_CLEAR(clear_module_state->__pyx_codeobj__120);
   Py_CLEAR(clear_module_state->__pyx_codeobj__121);
   Py_CLEAR(clear_module_state->__pyx_codeobj__122);
   Py_CLEAR(clear_module_state->__pyx_codeobj__123);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__124);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__126);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__128);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__131);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__133);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__135);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__137);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__140);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__143);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__145);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__148);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__150);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__152);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__155);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__157);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__125);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__127);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__130);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__132);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__134);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__136);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__139);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__142);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__144);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__147);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__149);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__151);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__154);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__156);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__158);
   Py_CLEAR(clear_module_state->__pyx_codeobj__159);
   Py_CLEAR(clear_module_state->__pyx_codeobj__160);
   Py_CLEAR(clear_module_state->__pyx_codeobj__161);
   Py_CLEAR(clear_module_state->__pyx_codeobj__162);
   Py_CLEAR(clear_module_state->__pyx_codeobj__163);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__164);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__165);
   Py_CLEAR(clear_module_state->__pyx_codeobj__166);
   Py_CLEAR(clear_module_state->__pyx_codeobj__167);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__168);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__170);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__172);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__174);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__169);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__171);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__173);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__175);
   Py_CLEAR(clear_module_state->__pyx_codeobj__176);
   Py_CLEAR(clear_module_state->__pyx_codeobj__177);
   Py_CLEAR(clear_module_state->__pyx_codeobj__178);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__179);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__181);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__183);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__185);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__180);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__182);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__184);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__186);
   Py_CLEAR(clear_module_state->__pyx_codeobj__187);
   Py_CLEAR(clear_module_state->__pyx_codeobj__188);
   Py_CLEAR(clear_module_state->__pyx_codeobj__189);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__190);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__191);
   Py_CLEAR(clear_module_state->__pyx_codeobj__192);
   Py_CLEAR(clear_module_state->__pyx_codeobj__193);
   Py_CLEAR(clear_module_state->__pyx_codeobj__194);
   Py_CLEAR(clear_module_state->__pyx_codeobj__195);
   Py_CLEAR(clear_module_state->__pyx_codeobj__196);
   Py_CLEAR(clear_module_state->__pyx_codeobj__197);
   Py_CLEAR(clear_module_state->__pyx_codeobj__198);
@@ -7398,15 +7394,14 @@
   Py_CLEAR(clear_module_state->__pyx_codeobj__204);
   Py_CLEAR(clear_module_state->__pyx_codeobj__205);
   Py_CLEAR(clear_module_state->__pyx_codeobj__206);
   Py_CLEAR(clear_module_state->__pyx_codeobj__207);
   Py_CLEAR(clear_module_state->__pyx_codeobj__208);
   Py_CLEAR(clear_module_state->__pyx_codeobj__209);
   Py_CLEAR(clear_module_state->__pyx_codeobj__210);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__211);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -7663,15 +7658,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Metadata);
   Py_VISIT(traverse_module_state->__pyx_n_s_Metadata___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Metadata___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Metadata_fields_count);
   Py_VISIT(traverse_module_state->__pyx_n_s_NEIGHBOR);
   Py_VISIT(traverse_module_state->__pyx_n_s_OVERLAPS);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Offset_incorrect_Got_use_len);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_Operation_field_no_must_be_int_a);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Operation_field_no_must_be_of_ei);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Operation_length_must_be_at_leas);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Operation_type_must_of_a_str_or);
   Py_VISIT(traverse_module_state->__pyx_n_s_Optional);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Part_len_must_be_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_PingRequest);
@@ -7758,23 +7752,23 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_UpsertRequest___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_VERSION_STRING_REGEX);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_WriteBuffer);
   Py_VISIT(traverse_module_state->__pyx_n_s_WriteBuffer___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_WriteBuffer___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_WriteBuffer_hex);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__15);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__14);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__17);
   Py_VISIT(traverse_module_state->__pyx_kp_u__18);
   Py_VISIT(traverse_module_state->__pyx_kp_u__19);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__20);
-  Py_VISIT(traverse_module_state->__pyx_n_s__212);
+  Py_VISIT(traverse_module_state->__pyx_n_s__211);
   Py_VISIT(traverse_module_state->__pyx_kp_u__3);
   Py_VISIT(traverse_module_state->__pyx_kp_u__5);
-  Py_VISIT(traverse_module_state->__pyx_n_s__66);
+  Py_VISIT(traverse_module_state->__pyx_n_s__65);
   Py_VISIT(traverse_module_state->__pyx_n_s_add_done_callback);
   Py_VISIT(traverse_module_state->__pyx_n_s_anext);
   Py_VISIT(traverse_module_state->__pyx_n_s_append);
   Py_VISIT(traverse_module_state->__pyx_n_s_args);
   Py_VISIT(traverse_module_state->__pyx_n_s_as_tuple);
   Py_VISIT(traverse_module_state->__pyx_n_u_ascii);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio);
@@ -7878,15 +7872,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_indexes);
   Py_VISIT(traverse_module_state->__pyx_n_s_init);
   Py_VISIT(traverse_module_state->__pyx_n_s_init_subclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_initial_read_buffer_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_insert);
   Py_VISIT(traverse_module_state->__pyx_n_s_inspect);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_int_argument_required_for_Arithm);
   Py_VISIT(traverse_module_state->__pyx_kp_u_invalid_datetime_size_got_extra);
   Py_VISIT(traverse_module_state->__pyx_kp_u_iproto_error_stack_frame_fields);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_connected);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_fully_connected);
   Py_VISIT(traverse_module_state->__pyx_n_u_is_nullable);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
@@ -8113,22 +8106,22 @@
   Py_VISIT(traverse_module_state->__pyx_int_neg_2);
   Py_VISIT(traverse_module_state->__pyx_tuple_);
   Py_VISIT(traverse_module_state->__pyx_tuple__4);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
   Py_VISIT(traverse_module_state->__pyx_tuple__7);
   Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__9);
+  Py_VISIT(traverse_module_state->__pyx_slice__15);
   Py_VISIT(traverse_module_state->__pyx_slice__16);
-  Py_VISIT(traverse_module_state->__pyx_slice__17);
-  Py_VISIT(traverse_module_state->__pyx_slice__40);
+  Py_VISIT(traverse_module_state->__pyx_slice__39);
   Py_VISIT(traverse_module_state->__pyx_tuple__10);
   Py_VISIT(traverse_module_state->__pyx_tuple__11);
   Py_VISIT(traverse_module_state->__pyx_tuple__12);
   Py_VISIT(traverse_module_state->__pyx_tuple__13);
-  Py_VISIT(traverse_module_state->__pyx_tuple__14);
+  Py_VISIT(traverse_module_state->__pyx_tuple__20);
   Py_VISIT(traverse_module_state->__pyx_tuple__21);
   Py_VISIT(traverse_module_state->__pyx_tuple__22);
   Py_VISIT(traverse_module_state->__pyx_tuple__23);
   Py_VISIT(traverse_module_state->__pyx_tuple__24);
   Py_VISIT(traverse_module_state->__pyx_tuple__25);
   Py_VISIT(traverse_module_state->__pyx_tuple__26);
   Py_VISIT(traverse_module_state->__pyx_tuple__27);
@@ -8139,18 +8132,18 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__32);
   Py_VISIT(traverse_module_state->__pyx_tuple__33);
   Py_VISIT(traverse_module_state->__pyx_tuple__34);
   Py_VISIT(traverse_module_state->__pyx_tuple__35);
   Py_VISIT(traverse_module_state->__pyx_tuple__36);
   Py_VISIT(traverse_module_state->__pyx_tuple__37);
   Py_VISIT(traverse_module_state->__pyx_tuple__38);
-  Py_VISIT(traverse_module_state->__pyx_tuple__39);
+  Py_VISIT(traverse_module_state->__pyx_tuple__40);
   Py_VISIT(traverse_module_state->__pyx_tuple__41);
-  Py_VISIT(traverse_module_state->__pyx_tuple__42);
-  Py_VISIT(traverse_module_state->__pyx_tuple__45);
+  Py_VISIT(traverse_module_state->__pyx_tuple__44);
+  Py_VISIT(traverse_module_state->__pyx_tuple__46);
   Py_VISIT(traverse_module_state->__pyx_tuple__47);
   Py_VISIT(traverse_module_state->__pyx_tuple__48);
   Py_VISIT(traverse_module_state->__pyx_tuple__49);
   Py_VISIT(traverse_module_state->__pyx_tuple__50);
   Py_VISIT(traverse_module_state->__pyx_tuple__51);
   Py_VISIT(traverse_module_state->__pyx_tuple__52);
   Py_VISIT(traverse_module_state->__pyx_tuple__53);
@@ -8161,67 +8154,67 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__58);
   Py_VISIT(traverse_module_state->__pyx_tuple__59);
   Py_VISIT(traverse_module_state->__pyx_tuple__60);
   Py_VISIT(traverse_module_state->__pyx_tuple__61);
   Py_VISIT(traverse_module_state->__pyx_tuple__62);
   Py_VISIT(traverse_module_state->__pyx_tuple__63);
   Py_VISIT(traverse_module_state->__pyx_tuple__64);
-  Py_VISIT(traverse_module_state->__pyx_tuple__65);
-  Py_VISIT(traverse_module_state->__pyx_tuple__67);
-  Py_VISIT(traverse_module_state->__pyx_tuple__69);
-  Py_VISIT(traverse_module_state->__pyx_tuple__79);
-  Py_VISIT(traverse_module_state->__pyx_tuple__85);
-  Py_VISIT(traverse_module_state->__pyx_tuple__125);
-  Py_VISIT(traverse_module_state->__pyx_tuple__127);
+  Py_VISIT(traverse_module_state->__pyx_tuple__66);
+  Py_VISIT(traverse_module_state->__pyx_tuple__68);
+  Py_VISIT(traverse_module_state->__pyx_tuple__78);
+  Py_VISIT(traverse_module_state->__pyx_tuple__84);
+  Py_VISIT(traverse_module_state->__pyx_tuple__124);
+  Py_VISIT(traverse_module_state->__pyx_tuple__126);
+  Py_VISIT(traverse_module_state->__pyx_tuple__128);
   Py_VISIT(traverse_module_state->__pyx_tuple__129);
-  Py_VISIT(traverse_module_state->__pyx_tuple__130);
-  Py_VISIT(traverse_module_state->__pyx_tuple__132);
-  Py_VISIT(traverse_module_state->__pyx_tuple__134);
-  Py_VISIT(traverse_module_state->__pyx_tuple__136);
+  Py_VISIT(traverse_module_state->__pyx_tuple__131);
+  Py_VISIT(traverse_module_state->__pyx_tuple__133);
+  Py_VISIT(traverse_module_state->__pyx_tuple__135);
+  Py_VISIT(traverse_module_state->__pyx_tuple__137);
   Py_VISIT(traverse_module_state->__pyx_tuple__138);
-  Py_VISIT(traverse_module_state->__pyx_tuple__139);
+  Py_VISIT(traverse_module_state->__pyx_tuple__140);
   Py_VISIT(traverse_module_state->__pyx_tuple__141);
-  Py_VISIT(traverse_module_state->__pyx_tuple__142);
-  Py_VISIT(traverse_module_state->__pyx_tuple__144);
+  Py_VISIT(traverse_module_state->__pyx_tuple__143);
+  Py_VISIT(traverse_module_state->__pyx_tuple__145);
   Py_VISIT(traverse_module_state->__pyx_tuple__146);
-  Py_VISIT(traverse_module_state->__pyx_tuple__147);
-  Py_VISIT(traverse_module_state->__pyx_tuple__149);
-  Py_VISIT(traverse_module_state->__pyx_tuple__151);
+  Py_VISIT(traverse_module_state->__pyx_tuple__148);
+  Py_VISIT(traverse_module_state->__pyx_tuple__150);
+  Py_VISIT(traverse_module_state->__pyx_tuple__152);
   Py_VISIT(traverse_module_state->__pyx_tuple__153);
-  Py_VISIT(traverse_module_state->__pyx_tuple__154);
-  Py_VISIT(traverse_module_state->__pyx_tuple__156);
-  Py_VISIT(traverse_module_state->__pyx_tuple__158);
-  Py_VISIT(traverse_module_state->__pyx_tuple__165);
-  Py_VISIT(traverse_module_state->__pyx_tuple__169);
-  Py_VISIT(traverse_module_state->__pyx_tuple__171);
-  Py_VISIT(traverse_module_state->__pyx_tuple__173);
-  Py_VISIT(traverse_module_state->__pyx_tuple__175);
-  Py_VISIT(traverse_module_state->__pyx_tuple__180);
-  Py_VISIT(traverse_module_state->__pyx_tuple__182);
-  Py_VISIT(traverse_module_state->__pyx_tuple__184);
-  Py_VISIT(traverse_module_state->__pyx_tuple__186);
-  Py_VISIT(traverse_module_state->__pyx_tuple__191);
+  Py_VISIT(traverse_module_state->__pyx_tuple__155);
+  Py_VISIT(traverse_module_state->__pyx_tuple__157);
+  Py_VISIT(traverse_module_state->__pyx_tuple__164);
+  Py_VISIT(traverse_module_state->__pyx_tuple__168);
+  Py_VISIT(traverse_module_state->__pyx_tuple__170);
+  Py_VISIT(traverse_module_state->__pyx_tuple__172);
+  Py_VISIT(traverse_module_state->__pyx_tuple__174);
+  Py_VISIT(traverse_module_state->__pyx_tuple__179);
+  Py_VISIT(traverse_module_state->__pyx_tuple__181);
+  Py_VISIT(traverse_module_state->__pyx_tuple__183);
+  Py_VISIT(traverse_module_state->__pyx_tuple__185);
+  Py_VISIT(traverse_module_state->__pyx_tuple__190);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__42);
   Py_VISIT(traverse_module_state->__pyx_codeobj__43);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__44);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__46);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__68);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__45);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__67);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__69);
   Py_VISIT(traverse_module_state->__pyx_codeobj__70);
   Py_VISIT(traverse_module_state->__pyx_codeobj__71);
   Py_VISIT(traverse_module_state->__pyx_codeobj__72);
   Py_VISIT(traverse_module_state->__pyx_codeobj__73);
   Py_VISIT(traverse_module_state->__pyx_codeobj__74);
   Py_VISIT(traverse_module_state->__pyx_codeobj__75);
   Py_VISIT(traverse_module_state->__pyx_codeobj__76);
   Py_VISIT(traverse_module_state->__pyx_codeobj__77);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__78);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__79);
   Py_VISIT(traverse_module_state->__pyx_codeobj__80);
   Py_VISIT(traverse_module_state->__pyx_codeobj__81);
   Py_VISIT(traverse_module_state->__pyx_codeobj__82);
   Py_VISIT(traverse_module_state->__pyx_codeobj__83);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__84);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__85);
   Py_VISIT(traverse_module_state->__pyx_codeobj__86);
   Py_VISIT(traverse_module_state->__pyx_codeobj__87);
   Py_VISIT(traverse_module_state->__pyx_codeobj__88);
   Py_VISIT(traverse_module_state->__pyx_codeobj__89);
   Py_VISIT(traverse_module_state->__pyx_codeobj__90);
   Py_VISIT(traverse_module_state->__pyx_codeobj__91);
   Py_VISIT(traverse_module_state->__pyx_codeobj__92);
@@ -8252,52 +8245,52 @@
   Py_VISIT(traverse_module_state->__pyx_codeobj__117);
   Py_VISIT(traverse_module_state->__pyx_codeobj__118);
   Py_VISIT(traverse_module_state->__pyx_codeobj__119);
   Py_VISIT(traverse_module_state->__pyx_codeobj__120);
   Py_VISIT(traverse_module_state->__pyx_codeobj__121);
   Py_VISIT(traverse_module_state->__pyx_codeobj__122);
   Py_VISIT(traverse_module_state->__pyx_codeobj__123);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__124);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__126);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__128);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__131);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__133);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__135);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__137);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__140);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__143);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__145);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__148);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__150);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__152);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__155);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__157);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__125);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__127);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__130);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__132);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__134);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__136);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__139);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__142);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__144);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__147);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__149);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__151);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__154);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__156);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__158);
   Py_VISIT(traverse_module_state->__pyx_codeobj__159);
   Py_VISIT(traverse_module_state->__pyx_codeobj__160);
   Py_VISIT(traverse_module_state->__pyx_codeobj__161);
   Py_VISIT(traverse_module_state->__pyx_codeobj__162);
   Py_VISIT(traverse_module_state->__pyx_codeobj__163);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__164);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__165);
   Py_VISIT(traverse_module_state->__pyx_codeobj__166);
   Py_VISIT(traverse_module_state->__pyx_codeobj__167);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__168);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__170);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__172);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__174);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__169);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__171);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__173);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__175);
   Py_VISIT(traverse_module_state->__pyx_codeobj__176);
   Py_VISIT(traverse_module_state->__pyx_codeobj__177);
   Py_VISIT(traverse_module_state->__pyx_codeobj__178);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__179);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__181);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__183);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__185);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__180);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__182);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__184);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__186);
   Py_VISIT(traverse_module_state->__pyx_codeobj__187);
   Py_VISIT(traverse_module_state->__pyx_codeobj__188);
   Py_VISIT(traverse_module_state->__pyx_codeobj__189);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__190);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__191);
   Py_VISIT(traverse_module_state->__pyx_codeobj__192);
   Py_VISIT(traverse_module_state->__pyx_codeobj__193);
   Py_VISIT(traverse_module_state->__pyx_codeobj__194);
   Py_VISIT(traverse_module_state->__pyx_codeobj__195);
   Py_VISIT(traverse_module_state->__pyx_codeobj__196);
   Py_VISIT(traverse_module_state->__pyx_codeobj__197);
   Py_VISIT(traverse_module_state->__pyx_codeobj__198);
@@ -8309,15 +8302,14 @@
   Py_VISIT(traverse_module_state->__pyx_codeobj__204);
   Py_VISIT(traverse_module_state->__pyx_codeobj__205);
   Py_VISIT(traverse_module_state->__pyx_codeobj__206);
   Py_VISIT(traverse_module_state->__pyx_codeobj__207);
   Py_VISIT(traverse_module_state->__pyx_codeobj__208);
   Py_VISIT(traverse_module_state->__pyx_codeobj__209);
   Py_VISIT(traverse_module_state->__pyx_codeobj__210);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__211);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -8688,15 +8680,14 @@
 #define __pyx_n_s_Metadata __pyx_mstate_global->__pyx_n_s_Metadata
 #define __pyx_n_s_Metadata___reduce_cython __pyx_mstate_global->__pyx_n_s_Metadata___reduce_cython
 #define __pyx_n_s_Metadata___setstate_cython __pyx_mstate_global->__pyx_n_s_Metadata___setstate_cython
 #define __pyx_kp_u_Metadata_fields_count __pyx_mstate_global->__pyx_kp_u_Metadata_fields_count
 #define __pyx_n_s_NEIGHBOR __pyx_mstate_global->__pyx_n_s_NEIGHBOR
 #define __pyx_n_s_OVERLAPS __pyx_mstate_global->__pyx_n_s_OVERLAPS
 #define __pyx_kp_u_Offset_incorrect_Got_use_len __pyx_mstate_global->__pyx_kp_u_Offset_incorrect_Got_use_len
-#define __pyx_kp_u_Operation_field_no_must_be_int_a __pyx_mstate_global->__pyx_kp_u_Operation_field_no_must_be_int_a
 #define __pyx_kp_u_Operation_field_no_must_be_of_ei __pyx_mstate_global->__pyx_kp_u_Operation_field_no_must_be_of_ei
 #define __pyx_kp_u_Operation_length_must_be_at_leas __pyx_mstate_global->__pyx_kp_u_Operation_length_must_be_at_leas
 #define __pyx_kp_u_Operation_type_must_of_a_str_or __pyx_mstate_global->__pyx_kp_u_Operation_type_must_of_a_str_or
 #define __pyx_n_s_Optional __pyx_mstate_global->__pyx_n_s_Optional
 #define __pyx_kp_u_Part_len_must_be_2 __pyx_mstate_global->__pyx_kp_u_Part_len_must_be_2
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_PingRequest __pyx_mstate_global->__pyx_n_s_PingRequest
@@ -8783,23 +8774,23 @@
 #define __pyx_n_s_UpsertRequest___setstate_cython __pyx_mstate_global->__pyx_n_s_UpsertRequest___setstate_cython
 #define __pyx_n_s_VERSION_STRING_REGEX __pyx_mstate_global->__pyx_n_s_VERSION_STRING_REGEX
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_WriteBuffer __pyx_mstate_global->__pyx_n_s_WriteBuffer
 #define __pyx_n_s_WriteBuffer___reduce_cython __pyx_mstate_global->__pyx_n_s_WriteBuffer___reduce_cython
 #define __pyx_n_s_WriteBuffer___setstate_cython __pyx_mstate_global->__pyx_n_s_WriteBuffer___setstate_cython
 #define __pyx_n_s_WriteBuffer_hex __pyx_mstate_global->__pyx_n_s_WriteBuffer_hex
-#define __pyx_kp_u__15 __pyx_mstate_global->__pyx_kp_u__15
+#define __pyx_kp_u__14 __pyx_mstate_global->__pyx_kp_u__14
+#define __pyx_kp_u__17 __pyx_mstate_global->__pyx_kp_u__17
 #define __pyx_kp_u__18 __pyx_mstate_global->__pyx_kp_u__18
 #define __pyx_kp_u__19 __pyx_mstate_global->__pyx_kp_u__19
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
-#define __pyx_kp_u__20 __pyx_mstate_global->__pyx_kp_u__20
-#define __pyx_n_s__212 __pyx_mstate_global->__pyx_n_s__212
+#define __pyx_n_s__211 __pyx_mstate_global->__pyx_n_s__211
 #define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
 #define __pyx_kp_u__5 __pyx_mstate_global->__pyx_kp_u__5
-#define __pyx_n_s__66 __pyx_mstate_global->__pyx_n_s__66
+#define __pyx_n_s__65 __pyx_mstate_global->__pyx_n_s__65
 #define __pyx_n_s_add_done_callback __pyx_mstate_global->__pyx_n_s_add_done_callback
 #define __pyx_n_s_anext __pyx_mstate_global->__pyx_n_s_anext
 #define __pyx_n_s_append __pyx_mstate_global->__pyx_n_s_append
 #define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
 #define __pyx_n_s_as_tuple __pyx_mstate_global->__pyx_n_s_as_tuple
 #define __pyx_n_u_ascii __pyx_mstate_global->__pyx_n_u_ascii
 #define __pyx_n_s_asyncio __pyx_mstate_global->__pyx_n_s_asyncio
@@ -8903,15 +8894,14 @@
 #define __pyx_n_s_indexes __pyx_mstate_global->__pyx_n_s_indexes
 #define __pyx_n_s_init __pyx_mstate_global->__pyx_n_s_init
 #define __pyx_n_s_init_subclass __pyx_mstate_global->__pyx_n_s_init_subclass
 #define __pyx_n_s_initial_read_buffer_size __pyx_mstate_global->__pyx_n_s_initial_read_buffer_size
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_insert __pyx_mstate_global->__pyx_n_s_insert
 #define __pyx_n_s_inspect __pyx_mstate_global->__pyx_n_s_inspect
-#define __pyx_kp_u_int_argument_required_for_Arithm __pyx_mstate_global->__pyx_kp_u_int_argument_required_for_Arithm
 #define __pyx_kp_u_invalid_datetime_size_got_extra __pyx_mstate_global->__pyx_kp_u_invalid_datetime_size_got_extra
 #define __pyx_kp_u_iproto_error_stack_frame_fields __pyx_mstate_global->__pyx_kp_u_iproto_error_stack_frame_fields
 #define __pyx_n_s_is_connected __pyx_mstate_global->__pyx_n_s_is_connected
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_n_s_is_fully_connected __pyx_mstate_global->__pyx_n_s_is_fully_connected
 #define __pyx_n_u_is_nullable __pyx_mstate_global->__pyx_n_u_is_nullable
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
@@ -9138,22 +9128,22 @@
 #define __pyx_int_neg_2 __pyx_mstate_global->__pyx_int_neg_2
 #define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
+#define __pyx_slice__15 __pyx_mstate_global->__pyx_slice__15
 #define __pyx_slice__16 __pyx_mstate_global->__pyx_slice__16
-#define __pyx_slice__17 __pyx_mstate_global->__pyx_slice__17
-#define __pyx_slice__40 __pyx_mstate_global->__pyx_slice__40
+#define __pyx_slice__39 __pyx_mstate_global->__pyx_slice__39
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
 #define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
 #define __pyx_tuple__12 __pyx_mstate_global->__pyx_tuple__12
 #define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
-#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
+#define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
 #define __pyx_tuple__21 __pyx_mstate_global->__pyx_tuple__21
 #define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
 #define __pyx_tuple__23 __pyx_mstate_global->__pyx_tuple__23
 #define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
 #define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
 #define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
 #define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
@@ -9164,18 +9154,18 @@
 #define __pyx_tuple__32 __pyx_mstate_global->__pyx_tuple__32
 #define __pyx_tuple__33 __pyx_mstate_global->__pyx_tuple__33
 #define __pyx_tuple__34 __pyx_mstate_global->__pyx_tuple__34
 #define __pyx_tuple__35 __pyx_mstate_global->__pyx_tuple__35
 #define __pyx_tuple__36 __pyx_mstate_global->__pyx_tuple__36
 #define __pyx_tuple__37 __pyx_mstate_global->__pyx_tuple__37
 #define __pyx_tuple__38 __pyx_mstate_global->__pyx_tuple__38
-#define __pyx_tuple__39 __pyx_mstate_global->__pyx_tuple__39
+#define __pyx_tuple__40 __pyx_mstate_global->__pyx_tuple__40
 #define __pyx_tuple__41 __pyx_mstate_global->__pyx_tuple__41
-#define __pyx_tuple__42 __pyx_mstate_global->__pyx_tuple__42
-#define __pyx_tuple__45 __pyx_mstate_global->__pyx_tuple__45
+#define __pyx_tuple__44 __pyx_mstate_global->__pyx_tuple__44
+#define __pyx_tuple__46 __pyx_mstate_global->__pyx_tuple__46
 #define __pyx_tuple__47 __pyx_mstate_global->__pyx_tuple__47
 #define __pyx_tuple__48 __pyx_mstate_global->__pyx_tuple__48
 #define __pyx_tuple__49 __pyx_mstate_global->__pyx_tuple__49
 #define __pyx_tuple__50 __pyx_mstate_global->__pyx_tuple__50
 #define __pyx_tuple__51 __pyx_mstate_global->__pyx_tuple__51
 #define __pyx_tuple__52 __pyx_mstate_global->__pyx_tuple__52
 #define __pyx_tuple__53 __pyx_mstate_global->__pyx_tuple__53
@@ -9186,67 +9176,67 @@
 #define __pyx_tuple__58 __pyx_mstate_global->__pyx_tuple__58
 #define __pyx_tuple__59 __pyx_mstate_global->__pyx_tuple__59
 #define __pyx_tuple__60 __pyx_mstate_global->__pyx_tuple__60
 #define __pyx_tuple__61 __pyx_mstate_global->__pyx_tuple__61
 #define __pyx_tuple__62 __pyx_mstate_global->__pyx_tuple__62
 #define __pyx_tuple__63 __pyx_mstate_global->__pyx_tuple__63
 #define __pyx_tuple__64 __pyx_mstate_global->__pyx_tuple__64
-#define __pyx_tuple__65 __pyx_mstate_global->__pyx_tuple__65
-#define __pyx_tuple__67 __pyx_mstate_global->__pyx_tuple__67
-#define __pyx_tuple__69 __pyx_mstate_global->__pyx_tuple__69
-#define __pyx_tuple__79 __pyx_mstate_global->__pyx_tuple__79
-#define __pyx_tuple__85 __pyx_mstate_global->__pyx_tuple__85
-#define __pyx_tuple__125 __pyx_mstate_global->__pyx_tuple__125
-#define __pyx_tuple__127 __pyx_mstate_global->__pyx_tuple__127
+#define __pyx_tuple__66 __pyx_mstate_global->__pyx_tuple__66
+#define __pyx_tuple__68 __pyx_mstate_global->__pyx_tuple__68
+#define __pyx_tuple__78 __pyx_mstate_global->__pyx_tuple__78
+#define __pyx_tuple__84 __pyx_mstate_global->__pyx_tuple__84
+#define __pyx_tuple__124 __pyx_mstate_global->__pyx_tuple__124
+#define __pyx_tuple__126 __pyx_mstate_global->__pyx_tuple__126
+#define __pyx_tuple__128 __pyx_mstate_global->__pyx_tuple__128
 #define __pyx_tuple__129 __pyx_mstate_global->__pyx_tuple__129
-#define __pyx_tuple__130 __pyx_mstate_global->__pyx_tuple__130
-#define __pyx_tuple__132 __pyx_mstate_global->__pyx_tuple__132
-#define __pyx_tuple__134 __pyx_mstate_global->__pyx_tuple__134
-#define __pyx_tuple__136 __pyx_mstate_global->__pyx_tuple__136
+#define __pyx_tuple__131 __pyx_mstate_global->__pyx_tuple__131
+#define __pyx_tuple__133 __pyx_mstate_global->__pyx_tuple__133
+#define __pyx_tuple__135 __pyx_mstate_global->__pyx_tuple__135
+#define __pyx_tuple__137 __pyx_mstate_global->__pyx_tuple__137
 #define __pyx_tuple__138 __pyx_mstate_global->__pyx_tuple__138
-#define __pyx_tuple__139 __pyx_mstate_global->__pyx_tuple__139
+#define __pyx_tuple__140 __pyx_mstate_global->__pyx_tuple__140
 #define __pyx_tuple__141 __pyx_mstate_global->__pyx_tuple__141
-#define __pyx_tuple__142 __pyx_mstate_global->__pyx_tuple__142
-#define __pyx_tuple__144 __pyx_mstate_global->__pyx_tuple__144
+#define __pyx_tuple__143 __pyx_mstate_global->__pyx_tuple__143
+#define __pyx_tuple__145 __pyx_mstate_global->__pyx_tuple__145
 #define __pyx_tuple__146 __pyx_mstate_global->__pyx_tuple__146
-#define __pyx_tuple__147 __pyx_mstate_global->__pyx_tuple__147
-#define __pyx_tuple__149 __pyx_mstate_global->__pyx_tuple__149
-#define __pyx_tuple__151 __pyx_mstate_global->__pyx_tuple__151
+#define __pyx_tuple__148 __pyx_mstate_global->__pyx_tuple__148
+#define __pyx_tuple__150 __pyx_mstate_global->__pyx_tuple__150
+#define __pyx_tuple__152 __pyx_mstate_global->__pyx_tuple__152
 #define __pyx_tuple__153 __pyx_mstate_global->__pyx_tuple__153
-#define __pyx_tuple__154 __pyx_mstate_global->__pyx_tuple__154
-#define __pyx_tuple__156 __pyx_mstate_global->__pyx_tuple__156
-#define __pyx_tuple__158 __pyx_mstate_global->__pyx_tuple__158
-#define __pyx_tuple__165 __pyx_mstate_global->__pyx_tuple__165
-#define __pyx_tuple__169 __pyx_mstate_global->__pyx_tuple__169
-#define __pyx_tuple__171 __pyx_mstate_global->__pyx_tuple__171
-#define __pyx_tuple__173 __pyx_mstate_global->__pyx_tuple__173
-#define __pyx_tuple__175 __pyx_mstate_global->__pyx_tuple__175
-#define __pyx_tuple__180 __pyx_mstate_global->__pyx_tuple__180
-#define __pyx_tuple__182 __pyx_mstate_global->__pyx_tuple__182
-#define __pyx_tuple__184 __pyx_mstate_global->__pyx_tuple__184
-#define __pyx_tuple__186 __pyx_mstate_global->__pyx_tuple__186
-#define __pyx_tuple__191 __pyx_mstate_global->__pyx_tuple__191
+#define __pyx_tuple__155 __pyx_mstate_global->__pyx_tuple__155
+#define __pyx_tuple__157 __pyx_mstate_global->__pyx_tuple__157
+#define __pyx_tuple__164 __pyx_mstate_global->__pyx_tuple__164
+#define __pyx_tuple__168 __pyx_mstate_global->__pyx_tuple__168
+#define __pyx_tuple__170 __pyx_mstate_global->__pyx_tuple__170
+#define __pyx_tuple__172 __pyx_mstate_global->__pyx_tuple__172
+#define __pyx_tuple__174 __pyx_mstate_global->__pyx_tuple__174
+#define __pyx_tuple__179 __pyx_mstate_global->__pyx_tuple__179
+#define __pyx_tuple__181 __pyx_mstate_global->__pyx_tuple__181
+#define __pyx_tuple__183 __pyx_mstate_global->__pyx_tuple__183
+#define __pyx_tuple__185 __pyx_mstate_global->__pyx_tuple__185
+#define __pyx_tuple__190 __pyx_mstate_global->__pyx_tuple__190
+#define __pyx_codeobj__42 __pyx_mstate_global->__pyx_codeobj__42
 #define __pyx_codeobj__43 __pyx_mstate_global->__pyx_codeobj__43
-#define __pyx_codeobj__44 __pyx_mstate_global->__pyx_codeobj__44
-#define __pyx_codeobj__46 __pyx_mstate_global->__pyx_codeobj__46
-#define __pyx_codeobj__68 __pyx_mstate_global->__pyx_codeobj__68
+#define __pyx_codeobj__45 __pyx_mstate_global->__pyx_codeobj__45
+#define __pyx_codeobj__67 __pyx_mstate_global->__pyx_codeobj__67
+#define __pyx_codeobj__69 __pyx_mstate_global->__pyx_codeobj__69
 #define __pyx_codeobj__70 __pyx_mstate_global->__pyx_codeobj__70
 #define __pyx_codeobj__71 __pyx_mstate_global->__pyx_codeobj__71
 #define __pyx_codeobj__72 __pyx_mstate_global->__pyx_codeobj__72
 #define __pyx_codeobj__73 __pyx_mstate_global->__pyx_codeobj__73
 #define __pyx_codeobj__74 __pyx_mstate_global->__pyx_codeobj__74
 #define __pyx_codeobj__75 __pyx_mstate_global->__pyx_codeobj__75
 #define __pyx_codeobj__76 __pyx_mstate_global->__pyx_codeobj__76
 #define __pyx_codeobj__77 __pyx_mstate_global->__pyx_codeobj__77
-#define __pyx_codeobj__78 __pyx_mstate_global->__pyx_codeobj__78
+#define __pyx_codeobj__79 __pyx_mstate_global->__pyx_codeobj__79
 #define __pyx_codeobj__80 __pyx_mstate_global->__pyx_codeobj__80
 #define __pyx_codeobj__81 __pyx_mstate_global->__pyx_codeobj__81
 #define __pyx_codeobj__82 __pyx_mstate_global->__pyx_codeobj__82
 #define __pyx_codeobj__83 __pyx_mstate_global->__pyx_codeobj__83
-#define __pyx_codeobj__84 __pyx_mstate_global->__pyx_codeobj__84
+#define __pyx_codeobj__85 __pyx_mstate_global->__pyx_codeobj__85
 #define __pyx_codeobj__86 __pyx_mstate_global->__pyx_codeobj__86
 #define __pyx_codeobj__87 __pyx_mstate_global->__pyx_codeobj__87
 #define __pyx_codeobj__88 __pyx_mstate_global->__pyx_codeobj__88
 #define __pyx_codeobj__89 __pyx_mstate_global->__pyx_codeobj__89
 #define __pyx_codeobj__90 __pyx_mstate_global->__pyx_codeobj__90
 #define __pyx_codeobj__91 __pyx_mstate_global->__pyx_codeobj__91
 #define __pyx_codeobj__92 __pyx_mstate_global->__pyx_codeobj__92
@@ -9277,52 +9267,52 @@
 #define __pyx_codeobj__117 __pyx_mstate_global->__pyx_codeobj__117
 #define __pyx_codeobj__118 __pyx_mstate_global->__pyx_codeobj__118
 #define __pyx_codeobj__119 __pyx_mstate_global->__pyx_codeobj__119
 #define __pyx_codeobj__120 __pyx_mstate_global->__pyx_codeobj__120
 #define __pyx_codeobj__121 __pyx_mstate_global->__pyx_codeobj__121
 #define __pyx_codeobj__122 __pyx_mstate_global->__pyx_codeobj__122
 #define __pyx_codeobj__123 __pyx_mstate_global->__pyx_codeobj__123
-#define __pyx_codeobj__124 __pyx_mstate_global->__pyx_codeobj__124
-#define __pyx_codeobj__126 __pyx_mstate_global->__pyx_codeobj__126
-#define __pyx_codeobj__128 __pyx_mstate_global->__pyx_codeobj__128
-#define __pyx_codeobj__131 __pyx_mstate_global->__pyx_codeobj__131
-#define __pyx_codeobj__133 __pyx_mstate_global->__pyx_codeobj__133
-#define __pyx_codeobj__135 __pyx_mstate_global->__pyx_codeobj__135
-#define __pyx_codeobj__137 __pyx_mstate_global->__pyx_codeobj__137
-#define __pyx_codeobj__140 __pyx_mstate_global->__pyx_codeobj__140
-#define __pyx_codeobj__143 __pyx_mstate_global->__pyx_codeobj__143
-#define __pyx_codeobj__145 __pyx_mstate_global->__pyx_codeobj__145
-#define __pyx_codeobj__148 __pyx_mstate_global->__pyx_codeobj__148
-#define __pyx_codeobj__150 __pyx_mstate_global->__pyx_codeobj__150
-#define __pyx_codeobj__152 __pyx_mstate_global->__pyx_codeobj__152
-#define __pyx_codeobj__155 __pyx_mstate_global->__pyx_codeobj__155
-#define __pyx_codeobj__157 __pyx_mstate_global->__pyx_codeobj__157
+#define __pyx_codeobj__125 __pyx_mstate_global->__pyx_codeobj__125
+#define __pyx_codeobj__127 __pyx_mstate_global->__pyx_codeobj__127
+#define __pyx_codeobj__130 __pyx_mstate_global->__pyx_codeobj__130
+#define __pyx_codeobj__132 __pyx_mstate_global->__pyx_codeobj__132
+#define __pyx_codeobj__134 __pyx_mstate_global->__pyx_codeobj__134
+#define __pyx_codeobj__136 __pyx_mstate_global->__pyx_codeobj__136
+#define __pyx_codeobj__139 __pyx_mstate_global->__pyx_codeobj__139
+#define __pyx_codeobj__142 __pyx_mstate_global->__pyx_codeobj__142
+#define __pyx_codeobj__144 __pyx_mstate_global->__pyx_codeobj__144
+#define __pyx_codeobj__147 __pyx_mstate_global->__pyx_codeobj__147
+#define __pyx_codeobj__149 __pyx_mstate_global->__pyx_codeobj__149
+#define __pyx_codeobj__151 __pyx_mstate_global->__pyx_codeobj__151
+#define __pyx_codeobj__154 __pyx_mstate_global->__pyx_codeobj__154
+#define __pyx_codeobj__156 __pyx_mstate_global->__pyx_codeobj__156
+#define __pyx_codeobj__158 __pyx_mstate_global->__pyx_codeobj__158
 #define __pyx_codeobj__159 __pyx_mstate_global->__pyx_codeobj__159
 #define __pyx_codeobj__160 __pyx_mstate_global->__pyx_codeobj__160
 #define __pyx_codeobj__161 __pyx_mstate_global->__pyx_codeobj__161
 #define __pyx_codeobj__162 __pyx_mstate_global->__pyx_codeobj__162
 #define __pyx_codeobj__163 __pyx_mstate_global->__pyx_codeobj__163
-#define __pyx_codeobj__164 __pyx_mstate_global->__pyx_codeobj__164
+#define __pyx_codeobj__165 __pyx_mstate_global->__pyx_codeobj__165
 #define __pyx_codeobj__166 __pyx_mstate_global->__pyx_codeobj__166
 #define __pyx_codeobj__167 __pyx_mstate_global->__pyx_codeobj__167
-#define __pyx_codeobj__168 __pyx_mstate_global->__pyx_codeobj__168
-#define __pyx_codeobj__170 __pyx_mstate_global->__pyx_codeobj__170
-#define __pyx_codeobj__172 __pyx_mstate_global->__pyx_codeobj__172
-#define __pyx_codeobj__174 __pyx_mstate_global->__pyx_codeobj__174
+#define __pyx_codeobj__169 __pyx_mstate_global->__pyx_codeobj__169
+#define __pyx_codeobj__171 __pyx_mstate_global->__pyx_codeobj__171
+#define __pyx_codeobj__173 __pyx_mstate_global->__pyx_codeobj__173
+#define __pyx_codeobj__175 __pyx_mstate_global->__pyx_codeobj__175
 #define __pyx_codeobj__176 __pyx_mstate_global->__pyx_codeobj__176
 #define __pyx_codeobj__177 __pyx_mstate_global->__pyx_codeobj__177
 #define __pyx_codeobj__178 __pyx_mstate_global->__pyx_codeobj__178
-#define __pyx_codeobj__179 __pyx_mstate_global->__pyx_codeobj__179
-#define __pyx_codeobj__181 __pyx_mstate_global->__pyx_codeobj__181
-#define __pyx_codeobj__183 __pyx_mstate_global->__pyx_codeobj__183
-#define __pyx_codeobj__185 __pyx_mstate_global->__pyx_codeobj__185
+#define __pyx_codeobj__180 __pyx_mstate_global->__pyx_codeobj__180
+#define __pyx_codeobj__182 __pyx_mstate_global->__pyx_codeobj__182
+#define __pyx_codeobj__184 __pyx_mstate_global->__pyx_codeobj__184
+#define __pyx_codeobj__186 __pyx_mstate_global->__pyx_codeobj__186
 #define __pyx_codeobj__187 __pyx_mstate_global->__pyx_codeobj__187
 #define __pyx_codeobj__188 __pyx_mstate_global->__pyx_codeobj__188
 #define __pyx_codeobj__189 __pyx_mstate_global->__pyx_codeobj__189
-#define __pyx_codeobj__190 __pyx_mstate_global->__pyx_codeobj__190
+#define __pyx_codeobj__191 __pyx_mstate_global->__pyx_codeobj__191
 #define __pyx_codeobj__192 __pyx_mstate_global->__pyx_codeobj__192
 #define __pyx_codeobj__193 __pyx_mstate_global->__pyx_codeobj__193
 #define __pyx_codeobj__194 __pyx_mstate_global->__pyx_codeobj__194
 #define __pyx_codeobj__195 __pyx_mstate_global->__pyx_codeobj__195
 #define __pyx_codeobj__196 __pyx_mstate_global->__pyx_codeobj__196
 #define __pyx_codeobj__197 __pyx_mstate_global->__pyx_codeobj__197
 #define __pyx_codeobj__198 __pyx_mstate_global->__pyx_codeobj__198
@@ -9334,15 +9324,14 @@
 #define __pyx_codeobj__204 __pyx_mstate_global->__pyx_codeobj__204
 #define __pyx_codeobj__205 __pyx_mstate_global->__pyx_codeobj__205
 #define __pyx_codeobj__206 __pyx_mstate_global->__pyx_codeobj__206
 #define __pyx_codeobj__207 __pyx_mstate_global->__pyx_codeobj__207
 #define __pyx_codeobj__208 __pyx_mstate_global->__pyx_codeobj__208
 #define __pyx_codeobj__209 __pyx_mstate_global->__pyx_codeobj__209
 #define __pyx_codeobj__210 __pyx_mstate_global->__pyx_codeobj__210
-#define __pyx_codeobj__211 __pyx_mstate_global->__pyx_codeobj__211
 /* #### Code section: module_code ### */
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
  *         cdef inline double real(self):             # <<<<<<<<<<<<<<
  *             return self.cval.real
@@ -13550,15 +13539,15 @@
   }
 
   /* "asynctnt/iproto/schema.pyx":52
  *         if fld == NULL:
  *             raise KeyError('Field \'{}\' not found'.format(name))
  *         return <int> <object> fld             # <<<<<<<<<<<<<<
  * 
- *     cdef inline int len(self):
+ *     cdef inline int id_by_name_safe(self, str name) except *:
  */
   __pyx_t_5 = __Pyx_PyInt_As_int(((PyObject *)__pyx_v_fld)); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 52, __pyx_L1_error)
   __pyx_r = ((int)__pyx_t_5);
   goto __pyx_L0;
 
   /* "asynctnt/iproto/schema.pyx":45
  *         return field.name
@@ -13579,53 +13568,143 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "asynctnt/iproto/schema.pyx":54
  *         return <int> <object> fld
  * 
+ *     cdef inline int id_by_name_safe(self, str name) except *:             # <<<<<<<<<<<<<<
+ *         cdef:
+ *             PyObject *fld
+ */
+
+static CYTHON_INLINE int __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_id_by_name_safe(struct C_Metadata *__pyx_v_self, PyObject *__pyx_v_name) {
+  PyObject *__pyx_v_fld;
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("id_by_name_safe", 1);
+
+  /* "asynctnt/iproto/schema.pyx":58
+ *             PyObject *fld
+ * 
+ *         fld = cpython.dict.PyDict_GetItem(self.name_id_map, name)             # <<<<<<<<<<<<<<
+ *         if fld == NULL:
+ *             return -1
+ */
+  __pyx_t_1 = __pyx_v_self->name_id_map;
+  __Pyx_INCREF(__pyx_t_1);
+  __pyx_v_fld = PyDict_GetItem(__pyx_t_1, __pyx_v_name);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "asynctnt/iproto/schema.pyx":59
+ * 
+ *         fld = cpython.dict.PyDict_GetItem(self.name_id_map, name)
+ *         if fld == NULL:             # <<<<<<<<<<<<<<
+ *             return -1
+ *         return <int> <object> fld
+ */
+  __pyx_t_2 = (__pyx_v_fld == NULL);
+  if (__pyx_t_2) {
+
+    /* "asynctnt/iproto/schema.pyx":60
+ *         fld = cpython.dict.PyDict_GetItem(self.name_id_map, name)
+ *         if fld == NULL:
+ *             return -1             # <<<<<<<<<<<<<<
+ *         return <int> <object> fld
+ * 
+ */
+    __pyx_r = -1;
+    goto __pyx_L0;
+
+    /* "asynctnt/iproto/schema.pyx":59
+ * 
+ *         fld = cpython.dict.PyDict_GetItem(self.name_id_map, name)
+ *         if fld == NULL:             # <<<<<<<<<<<<<<
+ *             return -1
+ *         return <int> <object> fld
+ */
+  }
+
+  /* "asynctnt/iproto/schema.pyx":61
+ *         if fld == NULL:
+ *             return -1
+ *         return <int> <object> fld             # <<<<<<<<<<<<<<
+ * 
+ *     cdef inline int len(self):
+ */
+  __pyx_t_3 = __Pyx_PyInt_As_int(((PyObject *)__pyx_v_fld)); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 61, __pyx_L1_error)
+  __pyx_r = ((int)__pyx_t_3);
+  goto __pyx_L0;
+
+  /* "asynctnt/iproto/schema.pyx":54
+ *         return <int> <object> fld
+ * 
+ *     cdef inline int id_by_name_safe(self, str name) except *:             # <<<<<<<<<<<<<<
+ *         cdef:
+ *             PyObject *fld
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("asynctnt.iproto.protocol.Metadata.id_by_name_safe", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "asynctnt/iproto/schema.pyx":63
+ *         return <int> <object> fld
+ * 
  *     cdef inline int len(self):             # <<<<<<<<<<<<<<
  *         return <int> cpython.list.PyList_GET_SIZE(self.fields)
  * 
  */
 
 static CYTHON_INLINE int __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(struct C_Metadata *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("len", 1);
 
-  /* "asynctnt/iproto/schema.pyx":55
+  /* "asynctnt/iproto/schema.pyx":64
  * 
  *     cdef inline int len(self):
  *         return <int> cpython.list.PyList_GET_SIZE(self.fields)             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):  # pragma: nocover
  */
   __pyx_t_1 = __pyx_v_self->fields;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_r = ((int)PyList_GET_SIZE(__pyx_t_1));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":54
+  /* "asynctnt/iproto/schema.pyx":63
  *         return <int> <object> fld
  * 
  *     cdef inline int len(self):             # <<<<<<<<<<<<<<
  *         return <int> cpython.list.PyList_GET_SIZE(self.fields)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":57
+/* "asynctnt/iproto/schema.pyx":66
  *         return <int> cpython.list.PyList_GET_SIZE(self.fields)
  * 
  *     def __repr__(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return '<Metadata [fields_count={}]>'.format(self.len())
  * 
  */
 
@@ -13653,26 +13732,26 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 1);
 
-  /* "asynctnt/iproto/schema.pyx":58
+  /* "asynctnt/iproto/schema.pyx":67
  * 
  *     def __repr__(self):  # pragma: nocover
  *         return '<Metadata [fields_count={}]>'.format(self.len())             # <<<<<<<<<<<<<<
  * 
  * @cython.final
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Metadata_fields_count, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 58, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Metadata_fields_count, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 58, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 58, __pyx_L1_error)
+  __pyx_t_3 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(__pyx_v_self); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 67, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_3 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
@@ -13685,23 +13764,23 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_4};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_3, 1+__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 58, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 67, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":57
+  /* "asynctnt/iproto/schema.pyx":66
  *         return <int> cpython.list.PyList_GET_SIZE(self.fields)
  * 
  *     def __repr__(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return '<Metadata [fields_count={}]>'.format(self.len())
  * 
  */
 
@@ -14007,15 +14086,15 @@
   __Pyx_AddTraceback("asynctnt.iproto.protocol.Metadata.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":62
+/* "asynctnt/iproto/schema.pyx":71
  * @cython.final
  * cdef class SchemaIndex:
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.iid = -1
  *         self.sid = -1
  */
 
@@ -14044,99 +14123,99 @@
 }
 
 static int __pyx_pf_8asynctnt_6iproto_8protocol_11SchemaIndex___cinit__(struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 1);
 
-  /* "asynctnt/iproto/schema.pyx":63
+  /* "asynctnt/iproto/schema.pyx":72
  * cdef class SchemaIndex:
  *     def __cinit__(self):
  *         self.iid = -1             # <<<<<<<<<<<<<<
  *         self.sid = -1
  *         self.name = None
  */
   __pyx_v_self->iid = -1;
 
-  /* "asynctnt/iproto/schema.pyx":64
+  /* "asynctnt/iproto/schema.pyx":73
  *     def __cinit__(self):
  *         self.iid = -1
  *         self.sid = -1             # <<<<<<<<<<<<<<
  *         self.name = None
  *         self.index_type = None
  */
   __pyx_v_self->sid = -1;
 
-  /* "asynctnt/iproto/schema.pyx":65
+  /* "asynctnt/iproto/schema.pyx":74
  *         self.iid = -1
  *         self.sid = -1
  *         self.name = None             # <<<<<<<<<<<<<<
  *         self.index_type = None
  *         self.unique = None
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = ((PyObject*)Py_None);
 
-  /* "asynctnt/iproto/schema.pyx":66
+  /* "asynctnt/iproto/schema.pyx":75
  *         self.sid = -1
  *         self.name = None
  *         self.index_type = None             # <<<<<<<<<<<<<<
  *         self.unique = None
  *         self.metadata = None
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->index_type);
   __Pyx_DECREF(__pyx_v_self->index_type);
   __pyx_v_self->index_type = ((PyObject*)Py_None);
 
-  /* "asynctnt/iproto/schema.pyx":67
+  /* "asynctnt/iproto/schema.pyx":76
  *         self.name = None
  *         self.index_type = None
  *         self.unique = None             # <<<<<<<<<<<<<<
  *         self.metadata = None
  * 
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->unique);
   __Pyx_DECREF(__pyx_v_self->unique);
   __pyx_v_self->unique = Py_None;
 
-  /* "asynctnt/iproto/schema.pyx":68
+  /* "asynctnt/iproto/schema.pyx":77
  *         self.index_type = None
  *         self.unique = None
  *         self.metadata = None             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):  # pragma: nocover
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF((PyObject *)__pyx_v_self->metadata);
   __Pyx_DECREF((PyObject *)__pyx_v_self->metadata);
   __pyx_v_self->metadata = ((struct C_Metadata *)Py_None);
 
-  /* "asynctnt/iproto/schema.pyx":62
+  /* "asynctnt/iproto/schema.pyx":71
  * @cython.final
  * cdef class SchemaIndex:
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.iid = -1
  *         self.sid = -1
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":70
+/* "asynctnt/iproto/schema.pyx":79
  *         self.metadata = None
  * 
  *     def __repr__(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return \
  *             '<{} sid={}, id={}, name={}, ' \
  */
 
@@ -14166,56 +14245,56 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 1);
 
-  /* "asynctnt/iproto/schema.pyx":71
+  /* "asynctnt/iproto/schema.pyx":80
  * 
  *     def __repr__(self):  # pragma: nocover
  *         return \             # <<<<<<<<<<<<<<
  *             '<{} sid={}, id={}, name={}, ' \
  *             'type={}, unique={}>'.format(
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "asynctnt/iproto/schema.pyx":73
+  /* "asynctnt/iproto/schema.pyx":82
  *         return \
  *             '<{} sid={}, id={}, name={}, ' \
  *             'type={}, unique={}>'.format(             # <<<<<<<<<<<<<<
  *                 self.__class__.__name__,
  *                 self.sid, self.iid, self.name, self.index_type, self.unique
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_sid_id_name_type_unique, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 73, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_sid_id_name_type_unique, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "asynctnt/iproto/schema.pyx":74
+  /* "asynctnt/iproto/schema.pyx":83
  *             '<{} sid={}, id={}, name={}, ' \
  *             'type={}, unique={}>'.format(
  *                 self.__class__.__name__,             # <<<<<<<<<<<<<<
  *                 self.sid, self.iid, self.name, self.index_type, self.unique
  *             )
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 74, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 74, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 83, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":75
+  /* "asynctnt/iproto/schema.pyx":84
  *             'type={}, unique={}>'.format(
  *                 self.__class__.__name__,
  *                 self.sid, self.iid, self.name, self.index_type, self.unique             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 75, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->iid); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 75, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_self->iid); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 84, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
@@ -14230,23 +14309,23 @@
   {
     PyObject *__pyx_callargs[7] = {__pyx_t_6, __pyx_t_4, __pyx_t_3, __pyx_t_5, __pyx_v_self->name, __pyx_v_self->index_type, __pyx_v_self->unique};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 6+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 73, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":70
+  /* "asynctnt/iproto/schema.pyx":79
  *         self.metadata = None
  * 
  *     def __repr__(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return \
  *             '<{} sid={}, id={}, name={}, ' \
  */
 
@@ -14262,15 +14341,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":28
+/* "asynctnt/iproto/schema.pxd":29
  * cdef class SchemaIndex:
  *     cdef:
  *         readonly int sid             # <<<<<<<<<<<<<<
  *         readonly int iid
  *         readonly str name
  */
 
@@ -14294,15 +14373,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14311,15 +14390,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":29
+/* "asynctnt/iproto/schema.pxd":30
  *     cdef:
  *         readonly int sid
  *         readonly int iid             # <<<<<<<<<<<<<<
  *         readonly str name
  *         readonly str index_type
  */
 
@@ -14343,15 +14422,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->iid); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 29, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->iid); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -14360,15 +14439,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":30
+/* "asynctnt/iproto/schema.pxd":31
  *         readonly int sid
  *         readonly int iid
  *         readonly str name             # <<<<<<<<<<<<<<
  *         readonly str index_type
  *         readonly object unique
  */
 
@@ -14399,15 +14478,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":31
+/* "asynctnt/iproto/schema.pxd":32
  *         readonly int iid
  *         readonly str name
  *         readonly str index_type             # <<<<<<<<<<<<<<
  *         readonly object unique
  *         readonly Metadata metadata
  */
 
@@ -14438,15 +14517,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":32
+/* "asynctnt/iproto/schema.pxd":33
  *         readonly str name
  *         readonly str index_type
  *         readonly object unique             # <<<<<<<<<<<<<<
  *         readonly Metadata metadata
  * 
  */
 
@@ -14477,15 +14556,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":33
+/* "asynctnt/iproto/schema.pxd":34
  *         readonly str index_type
  *         readonly object unique
  *         readonly Metadata metadata             # <<<<<<<<<<<<<<
  * 
  * 
  */
 
@@ -14730,15 +14809,15 @@
   __Pyx_AddTraceback("asynctnt.iproto.protocol.SchemaIndex.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":80
+/* "asynctnt/iproto/schema.pyx":89
  * @cython.final
  * cdef class SchemaSpace:
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.sid = -1
  *         self.owner = -1
  */
 
@@ -14771,109 +14850,109 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 1);
 
-  /* "asynctnt/iproto/schema.pyx":81
+  /* "asynctnt/iproto/schema.pyx":90
  * cdef class SchemaSpace:
  *     def __cinit__(self):
  *         self.sid = -1             # <<<<<<<<<<<<<<
  *         self.owner = -1
  *         self.name = None
  */
   __pyx_v_self->sid = -1;
 
-  /* "asynctnt/iproto/schema.pyx":82
+  /* "asynctnt/iproto/schema.pyx":91
  *     def __cinit__(self):
  *         self.sid = -1
  *         self.owner = -1             # <<<<<<<<<<<<<<
  *         self.name = None
  *         self.engine = None
  */
   __pyx_v_self->owner = -1;
 
-  /* "asynctnt/iproto/schema.pyx":83
+  /* "asynctnt/iproto/schema.pyx":92
  *         self.sid = -1
  *         self.owner = -1
  *         self.name = None             # <<<<<<<<<<<<<<
  *         self.engine = None
  *         self.field_count = 0
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = ((PyObject*)Py_None);
 
-  /* "asynctnt/iproto/schema.pyx":84
+  /* "asynctnt/iproto/schema.pyx":93
  *         self.owner = -1
  *         self.name = None
  *         self.engine = None             # <<<<<<<<<<<<<<
  *         self.field_count = 0
  *         self.flags = None
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->engine);
   __Pyx_DECREF(__pyx_v_self->engine);
   __pyx_v_self->engine = ((PyObject*)Py_None);
 
-  /* "asynctnt/iproto/schema.pyx":85
+  /* "asynctnt/iproto/schema.pyx":94
  *         self.name = None
  *         self.engine = None
  *         self.field_count = 0             # <<<<<<<<<<<<<<
  *         self.flags = None
  * 
  */
   __pyx_v_self->field_count = 0;
 
-  /* "asynctnt/iproto/schema.pyx":86
+  /* "asynctnt/iproto/schema.pyx":95
  *         self.engine = None
  *         self.field_count = 0
  *         self.flags = None             # <<<<<<<<<<<<<<
  * 
  *         self.metadata = None
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->flags);
   __Pyx_DECREF(__pyx_v_self->flags);
   __pyx_v_self->flags = Py_None;
 
-  /* "asynctnt/iproto/schema.pyx":88
+  /* "asynctnt/iproto/schema.pyx":97
  *         self.flags = None
  * 
  *         self.metadata = None             # <<<<<<<<<<<<<<
  *         self.indexes = {}
  * 
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF((PyObject *)__pyx_v_self->metadata);
   __Pyx_DECREF((PyObject *)__pyx_v_self->metadata);
   __pyx_v_self->metadata = ((struct C_Metadata *)Py_None);
 
-  /* "asynctnt/iproto/schema.pyx":89
+  /* "asynctnt/iproto/schema.pyx":98
  * 
  *         self.metadata = None
  *         self.indexes = {}             # <<<<<<<<<<<<<<
  * 
  *     cdef void add_index(self, SchemaIndex idx):
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 89, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->indexes);
   __Pyx_DECREF(__pyx_v_self->indexes);
   __pyx_v_self->indexes = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":80
+  /* "asynctnt/iproto/schema.pyx":89
  * @cython.final
  * cdef class SchemaSpace:
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
  *         self.sid = -1
  *         self.owner = -1
  */
 
@@ -14885,15 +14964,15 @@
   __Pyx_AddTraceback("asynctnt.iproto.protocol.SchemaSpace.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":91
+/* "asynctnt/iproto/schema.pyx":100
  *         self.indexes = {}
  * 
  *     cdef void add_index(self, SchemaIndex idx):             # <<<<<<<<<<<<<<
  *         cpython.dict.PyDict_SetItem(self.indexes, idx.iid, idx)
  *         if idx.name:
  */
 
@@ -14904,64 +14983,64 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_index", 1);
 
-  /* "asynctnt/iproto/schema.pyx":92
+  /* "asynctnt/iproto/schema.pyx":101
  * 
  *     cdef void add_index(self, SchemaIndex idx):
  *         cpython.dict.PyDict_SetItem(self.indexes, idx.iid, idx)             # <<<<<<<<<<<<<<
  *         if idx.name:
  *             cpython.dict.PyDict_SetItem(self.indexes, idx.name, idx)
  */
   __pyx_t_1 = __pyx_v_self->indexes;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_idx->iid); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 92, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_idx->iid); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyDict_SetItem(__pyx_t_1, __pyx_t_2, ((PyObject *)__pyx_v_idx)); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 92, __pyx_L1_error)
+  __pyx_t_3 = PyDict_SetItem(__pyx_t_1, __pyx_t_2, ((PyObject *)__pyx_v_idx)); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":93
+  /* "asynctnt/iproto/schema.pyx":102
  *     cdef void add_index(self, SchemaIndex idx):
  *         cpython.dict.PyDict_SetItem(self.indexes, idx.iid, idx)
  *         if idx.name:             # <<<<<<<<<<<<<<
  *             cpython.dict.PyDict_SetItem(self.indexes, idx.name, idx)
  * 
  */
   __pyx_t_4 = (__pyx_v_idx->name != Py_None)&&(__Pyx_PyUnicode_IS_TRUE(__pyx_v_idx->name) != 0);
   if (__pyx_t_4) {
 
-    /* "asynctnt/iproto/schema.pyx":94
+    /* "asynctnt/iproto/schema.pyx":103
  *         cpython.dict.PyDict_SetItem(self.indexes, idx.iid, idx)
  *         if idx.name:
  *             cpython.dict.PyDict_SetItem(self.indexes, idx.name, idx)             # <<<<<<<<<<<<<<
  * 
  *     cdef SchemaIndex get_index(self, index, create_dummy=True):
  */
     __pyx_t_2 = __pyx_v_self->indexes;
     __Pyx_INCREF(__pyx_t_2);
     __pyx_t_1 = __pyx_v_idx->name;
     __Pyx_INCREF(__pyx_t_1);
-    __pyx_t_3 = PyDict_SetItem(__pyx_t_2, __pyx_t_1, ((PyObject *)__pyx_v_idx)); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 94, __pyx_L1_error)
+    __pyx_t_3 = PyDict_SetItem(__pyx_t_2, __pyx_t_1, ((PyObject *)__pyx_v_idx)); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(1, 103, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":93
+    /* "asynctnt/iproto/schema.pyx":102
  *     cdef void add_index(self, SchemaIndex idx):
  *         cpython.dict.PyDict_SetItem(self.indexes, idx.iid, idx)
  *         if idx.name:             # <<<<<<<<<<<<<<
  *             cpython.dict.PyDict_SetItem(self.indexes, idx.name, idx)
  * 
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":91
+  /* "asynctnt/iproto/schema.pyx":100
  *         self.indexes = {}
  * 
  *     cdef void add_index(self, SchemaIndex idx):             # <<<<<<<<<<<<<<
  *         cpython.dict.PyDict_SetItem(self.indexes, idx.iid, idx)
  *         if idx.name:
  */
 
@@ -14971,15 +15050,15 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("asynctnt.iproto.protocol.SchemaSpace.add_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "asynctnt/iproto/schema.pyx":96
+/* "asynctnt/iproto/schema.pyx":105
  *             cpython.dict.PyDict_SetItem(self.indexes, idx.name, idx)
  * 
  *     cdef SchemaIndex get_index(self, index, create_dummy=True):             # <<<<<<<<<<<<<<
  *         cdef:
  *             SchemaIndex idx
  */
 
@@ -15006,35 +15085,35 @@
   __Pyx_RefNannySetupContext("get_index", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_create_dummy = __pyx_optional_args->create_dummy;
     }
   }
 
-  /* "asynctnt/iproto/schema.pyx":101
+  /* "asynctnt/iproto/schema.pyx":110
  *             bint is_str, is_int
  *             PyObject *obj_p
  *         is_str = isinstance(index, str)             # <<<<<<<<<<<<<<
  *         is_int = isinstance(index, int)
  *         if not is_str and not is_int:
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_index); 
   __pyx_v_is_str = __pyx_t_1;
 
-  /* "asynctnt/iproto/schema.pyx":102
+  /* "asynctnt/iproto/schema.pyx":111
  *             PyObject *obj_p
  *         is_str = isinstance(index, str)
  *         is_int = isinstance(index, int)             # <<<<<<<<<<<<<<
  *         if not is_str and not is_int:
  *             raise TypeError(
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_index); 
   __pyx_v_is_int = __pyx_t_1;
 
-  /* "asynctnt/iproto/schema.pyx":103
+  /* "asynctnt/iproto/schema.pyx":112
  *         is_str = isinstance(index, str)
  *         is_int = isinstance(index, int)
  *         if not is_str and not is_int:             # <<<<<<<<<<<<<<
  *             raise TypeError(
  *                 'Index must be either str or int, got: {}'.format(type(index)))
  */
   __pyx_t_2 = (!__pyx_v_is_str);
@@ -15044,22 +15123,22 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (!__pyx_v_is_int);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "asynctnt/iproto/schema.pyx":105
+    /* "asynctnt/iproto/schema.pyx":114
  *         if not is_str and not is_int:
  *             raise TypeError(
  *                 'Index must be either str or int, got: {}'.format(type(index)))             # <<<<<<<<<<<<<<
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(self.indexes, index)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Index_must_be_either_str_or_int, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 105, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Index_must_be_either_str_or_int, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 114, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
@@ -15071,124 +15150,124 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, ((PyObject *)Py_TYPE(__pyx_v_index))};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 105, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 114, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
 
-    /* "asynctnt/iproto/schema.pyx":104
+    /* "asynctnt/iproto/schema.pyx":113
  *         is_int = isinstance(index, int)
  *         if not is_str and not is_int:
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 'Index must be either str or int, got: {}'.format(type(index)))
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 104, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 113, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(1, 104, __pyx_L1_error)
+    __PYX_ERR(1, 113, __pyx_L1_error)
 
-    /* "asynctnt/iproto/schema.pyx":103
+    /* "asynctnt/iproto/schema.pyx":112
  *         is_str = isinstance(index, str)
  *         is_int = isinstance(index, int)
  *         if not is_str and not is_int:             # <<<<<<<<<<<<<<
  *             raise TypeError(
  *                 'Index must be either str or int, got: {}'.format(type(index)))
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":107
+  /* "asynctnt/iproto/schema.pyx":116
  *                 'Index must be either str or int, got: {}'.format(type(index)))
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(self.indexes, index)             # <<<<<<<<<<<<<<
  *         if obj_p is not NULL:
  *             return <SchemaIndex> obj_p
  */
   __pyx_t_4 = __pyx_v_self->indexes;
   __Pyx_INCREF(__pyx_t_4);
   __pyx_v_obj_p = PyDict_GetItem(__pyx_t_4, __pyx_v_index);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":108
+  /* "asynctnt/iproto/schema.pyx":117
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(self.indexes, index)
  *         if obj_p is not NULL:             # <<<<<<<<<<<<<<
  *             return <SchemaIndex> obj_p
  *         else:
  */
   __pyx_t_1 = (__pyx_v_obj_p != NULL);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/schema.pyx":109
+    /* "asynctnt/iproto/schema.pyx":118
  *         obj_p = cpython.dict.PyDict_GetItem(self.indexes, index)
  *         if obj_p is not NULL:
  *             return <SchemaIndex> obj_p             # <<<<<<<<<<<<<<
  *         else:
  *             if is_int and create_dummy:
  */
     __Pyx_XDECREF((PyObject *)__pyx_r);
     __Pyx_INCREF((PyObject *)((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *)__pyx_v_obj_p));
     __pyx_r = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *)__pyx_v_obj_p);
     goto __pyx_L0;
 
-    /* "asynctnt/iproto/schema.pyx":108
+    /* "asynctnt/iproto/schema.pyx":117
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(self.indexes, index)
  *         if obj_p is not NULL:             # <<<<<<<<<<<<<<
  *             return <SchemaIndex> obj_p
  *         else:
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":111
+  /* "asynctnt/iproto/schema.pyx":120
  *             return <SchemaIndex> obj_p
  *         else:
  *             if is_int and create_dummy:             # <<<<<<<<<<<<<<
  *                 logger.debug(
  *                     'Index %s not found in space %s/%s. Creating dummy.',
  */
   /*else*/ {
     if (__pyx_v_is_int) {
     } else {
       __pyx_t_1 = __pyx_v_is_int;
       goto __pyx_L8_bool_binop_done;
     }
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_create_dummy); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 111, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_create_dummy); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 120, __pyx_L1_error)
     __pyx_t_1 = __pyx_t_2;
     __pyx_L8_bool_binop_done:;
     if (likely(__pyx_t_1)) {
 
-      /* "asynctnt/iproto/schema.pyx":112
+      /* "asynctnt/iproto/schema.pyx":121
  *         else:
  *             if is_int and create_dummy:
  *                 logger.debug(             # <<<<<<<<<<<<<<
  *                     'Index %s not found in space %s/%s. Creating dummy.',
  *                     index, self.sid, self.name
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 112, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logger); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 121, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 112, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_debug); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 121, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":114
+      /* "asynctnt/iproto/schema.pyx":123
  *                 logger.debug(
  *                     'Index %s not found in space %s/%s. Creating dummy.',
  *                     index, self.sid, self.name             # <<<<<<<<<<<<<<
  *                 )
  *                 idx = <SchemaIndex> SchemaIndex.__new__(SchemaIndex)
  */
-      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 114, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_7 = NULL;
       __pyx_t_6 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_7)) {
@@ -15201,132 +15280,132 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[5] = {__pyx_t_7, __pyx_kp_u_Index_s_not_found_in_space_s_s_C, __pyx_v_index, __pyx_t_3, __pyx_v_self->name};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 4+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 112, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 121, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":116
+      /* "asynctnt/iproto/schema.pyx":125
  *                     index, self.sid, self.name
  *                 )
  *                 idx = <SchemaIndex> SchemaIndex.__new__(SchemaIndex)             # <<<<<<<<<<<<<<
  *                 idx.iid = index
  *                 idx.sid = self.sid
  */
-      __pyx_t_4 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_SchemaIndex(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 116, __pyx_L1_error)
+      __pyx_t_4 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_SchemaIndex(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 125, __pyx_L1_error)
       __Pyx_GOTREF((PyObject *)__pyx_t_4);
       __pyx_t_5 = ((PyObject *)__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_DECREF((PyObject *)__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v_idx = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *)__pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":117
+      /* "asynctnt/iproto/schema.pyx":126
  *                 )
  *                 idx = <SchemaIndex> SchemaIndex.__new__(SchemaIndex)
  *                 idx.iid = index             # <<<<<<<<<<<<<<
  *                 idx.sid = self.sid
  *                 idx.name = str(index)
  */
-      __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 117, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 126, __pyx_L1_error)
       __pyx_v_idx->iid = __pyx_t_6;
 
-      /* "asynctnt/iproto/schema.pyx":118
+      /* "asynctnt/iproto/schema.pyx":127
  *                 idx = <SchemaIndex> SchemaIndex.__new__(SchemaIndex)
  *                 idx.iid = index
  *                 idx.sid = self.sid             # <<<<<<<<<<<<<<
  *                 idx.name = str(index)
  *                 cpython.dict.PyDict_SetItem(self.indexes, index, idx)
  */
       __pyx_t_6 = __pyx_v_self->sid;
       __pyx_v_idx->sid = __pyx_t_6;
 
-      /* "asynctnt/iproto/schema.pyx":119
+      /* "asynctnt/iproto/schema.pyx":128
  *                 idx.iid = index
  *                 idx.sid = self.sid
  *                 idx.name = str(index)             # <<<<<<<<<<<<<<
  *                 cpython.dict.PyDict_SetItem(self.indexes, index, idx)
  *                 return idx
  */
-      __pyx_t_5 = __Pyx_PyObject_Str(__pyx_v_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 119, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Str(__pyx_v_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_v_idx->name);
       __Pyx_DECREF(__pyx_v_idx->name);
       __pyx_v_idx->name = ((PyObject*)__pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":120
+      /* "asynctnt/iproto/schema.pyx":129
  *                 idx.sid = self.sid
  *                 idx.name = str(index)
  *                 cpython.dict.PyDict_SetItem(self.indexes, index, idx)             # <<<<<<<<<<<<<<
  *                 return idx
  *             else:
  */
       __pyx_t_5 = __pyx_v_self->indexes;
       __Pyx_INCREF(__pyx_t_5);
-      __pyx_t_6 = PyDict_SetItem(__pyx_t_5, __pyx_v_index, ((PyObject *)__pyx_v_idx)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 120, __pyx_L1_error)
+      __pyx_t_6 = PyDict_SetItem(__pyx_t_5, __pyx_v_index, ((PyObject *)__pyx_v_idx)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 129, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":121
+      /* "asynctnt/iproto/schema.pyx":130
  *                 idx.name = str(index)
  *                 cpython.dict.PyDict_SetItem(self.indexes, index, idx)
  *                 return idx             # <<<<<<<<<<<<<<
  *             else:
  *                 raise TarantoolSchemaError(
  */
       __Pyx_XDECREF((PyObject *)__pyx_r);
       __Pyx_INCREF((PyObject *)__pyx_v_idx);
       __pyx_r = __pyx_v_idx;
       goto __pyx_L0;
 
-      /* "asynctnt/iproto/schema.pyx":111
+      /* "asynctnt/iproto/schema.pyx":120
  *             return <SchemaIndex> obj_p
  *         else:
  *             if is_int and create_dummy:             # <<<<<<<<<<<<<<
  *                 logger.debug(
  *                     'Index %s not found in space %s/%s. Creating dummy.',
  */
     }
 
-    /* "asynctnt/iproto/schema.pyx":123
+    /* "asynctnt/iproto/schema.pyx":132
  *                 return idx
  *             else:
  *                 raise TarantoolSchemaError(             # <<<<<<<<<<<<<<
  *                     'Index {} not found in space {}/{}'.format(
  *                         index, self.sid, self.name
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_TarantoolSchemaError); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 123, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_TarantoolSchemaError); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 132, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
 
-      /* "asynctnt/iproto/schema.pyx":124
+      /* "asynctnt/iproto/schema.pyx":133
  *             else:
  *                 raise TarantoolSchemaError(
  *                     'Index {} not found in space {}/{}'.format(             # <<<<<<<<<<<<<<
  *                         index, self.sid, self.name
  *                     )
  */
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Index_not_found_in_space, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 124, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Index_not_found_in_space, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 133, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "asynctnt/iproto/schema.pyx":125
+      /* "asynctnt/iproto/schema.pyx":134
  *                 raise TarantoolSchemaError(
  *                     'Index {} not found in space {}/{}'.format(
  *                         index, self.sid, self.name             # <<<<<<<<<<<<<<
  *                     )
  *                 )
  */
-      __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 125, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 134, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_9 = NULL;
       __pyx_t_6 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_9)) {
@@ -15339,15 +15418,15 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[4] = {__pyx_t_9, __pyx_v_index, __pyx_t_8, __pyx_v_self->name};
         __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_6, 3+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 124, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 133, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __pyx_t_7 = NULL;
       __pyx_t_6 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_4))) {
@@ -15362,25 +15441,25 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_3};
         __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 123, __pyx_L1_error)
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 132, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       }
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(1, 123, __pyx_L1_error)
+      __PYX_ERR(1, 132, __pyx_L1_error)
     }
   }
 
-  /* "asynctnt/iproto/schema.pyx":96
+  /* "asynctnt/iproto/schema.pyx":105
  *             cpython.dict.PyDict_SetItem(self.indexes, idx.name, idx)
  * 
  *     cdef SchemaIndex get_index(self, index, create_dummy=True):             # <<<<<<<<<<<<<<
  *         cdef:
  *             SchemaIndex idx
  */
 
@@ -15397,15 +15476,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_idx);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":129
+/* "asynctnt/iproto/schema.pyx":138
  *                 )
  * 
  *     def __repr__(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return '<{} id={} name={} engine={}>'.format(
  *             self.__class__.__name__,
  */
 
@@ -15434,46 +15513,46 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 1);
 
-  /* "asynctnt/iproto/schema.pyx":130
+  /* "asynctnt/iproto/schema.pyx":139
  * 
  *     def __repr__(self):  # pragma: nocover
  *         return '<{} id={} name={} engine={}>'.format(             # <<<<<<<<<<<<<<
  *             self.__class__.__name__,
  *             self.sid, self.name, self.engine
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_id_name_engine, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 130, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_id_name_engine, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "asynctnt/iproto/schema.pyx":131
+  /* "asynctnt/iproto/schema.pyx":140
  *     def __repr__(self):  # pragma: nocover
  *         return '<{} id={} name={} engine={}>'.format(
  *             self.__class__.__name__,             # <<<<<<<<<<<<<<
  *             self.sid, self.name, self.engine
  *         )
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 131, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 131, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":132
+  /* "asynctnt/iproto/schema.pyx":141
  *         return '<{} id={} name={} engine={}>'.format(
  *             self.__class__.__name__,
  *             self.sid, self.name, self.engine             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 132, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
@@ -15487,23 +15566,23 @@
   #endif
   {
     PyObject *__pyx_callargs[5] = {__pyx_t_5, __pyx_t_4, __pyx_t_3, __pyx_v_self->name, __pyx_v_self->engine};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 4+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 130, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":129
+  /* "asynctnt/iproto/schema.pyx":138
  *                 )
  * 
  *     def __repr__(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return '<{} id={} name={} engine={}>'.format(
  *             self.__class__.__name__,
  */
 
@@ -15518,15 +15597,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":42
+/* "asynctnt/iproto/schema.pxd":43
  * cdef class SchemaSpace:
  *     cdef:
  *         readonly int sid             # <<<<<<<<<<<<<<
  *         readonly int owner
  *         readonly str name
  */
 
@@ -15550,15 +15629,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 42, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->sid); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 43, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15567,15 +15646,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":43
+/* "asynctnt/iproto/schema.pxd":44
  *     cdef:
  *         readonly int sid
  *         readonly int owner             # <<<<<<<<<<<<<<
  *         readonly str name
  *         readonly str engine
  */
 
@@ -15599,15 +15678,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->owner); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 43, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->owner); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15616,15 +15695,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":44
+/* "asynctnt/iproto/schema.pxd":45
  *         readonly int sid
  *         readonly int owner
  *         readonly str name             # <<<<<<<<<<<<<<
  *         readonly str engine
  *         readonly int field_count
  */
 
@@ -15655,15 +15734,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":45
+/* "asynctnt/iproto/schema.pxd":46
  *         readonly int owner
  *         readonly str name
  *         readonly str engine             # <<<<<<<<<<<<<<
  *         readonly int field_count
  *         readonly object flags
  */
 
@@ -15694,15 +15773,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":46
+/* "asynctnt/iproto/schema.pxd":47
  *         readonly str name
  *         readonly str engine
  *         readonly int field_count             # <<<<<<<<<<<<<<
  *         readonly object flags
  * 
  */
 
@@ -15726,15 +15805,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->field_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 46, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->field_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 47, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -15743,15 +15822,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":47
+/* "asynctnt/iproto/schema.pxd":48
  *         readonly str engine
  *         readonly int field_count
  *         readonly object flags             # <<<<<<<<<<<<<<
  * 
  *         readonly Metadata metadata
  */
 
@@ -15782,15 +15861,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":49
+/* "asynctnt/iproto/schema.pxd":50
  *         readonly object flags
  * 
  *         readonly Metadata metadata             # <<<<<<<<<<<<<<
  *         readonly dict indexes
  * 
  */
 
@@ -15821,15 +15900,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":50
+/* "asynctnt/iproto/schema.pxd":51
  * 
  *         readonly Metadata metadata
  *         readonly dict indexes             # <<<<<<<<<<<<<<
  * 
  *     cdef void add_index(self, SchemaIndex idx)
  */
 
@@ -16074,15 +16153,15 @@
   __Pyx_AddTraceback("asynctnt.iproto.protocol.SchemaSpace.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":137
+/* "asynctnt/iproto/schema.pyx":146
  * @cython.final
  * cdef class Schema:
  *     def __cinit__(self, int schema_id):             # <<<<<<<<<<<<<<
  *         self.id = schema_id
  *         self.spaces = {}
  */
 
@@ -16118,31 +16197,31 @@
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_schema_id)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 137, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 146, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 137, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 146, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
-    __pyx_v_schema_id = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_schema_id == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 137, __pyx_L3_error)
+    __pyx_v_schema_id = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_schema_id == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 146, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 137, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 146, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
@@ -16170,39 +16249,39 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 1);
 
-  /* "asynctnt/iproto/schema.pyx":138
+  /* "asynctnt/iproto/schema.pyx":147
  * cdef class Schema:
  *     def __cinit__(self, int schema_id):
  *         self.id = schema_id             # <<<<<<<<<<<<<<
  *         self.spaces = {}
  * 
  */
   __pyx_v_self->id = __pyx_v_schema_id;
 
-  /* "asynctnt/iproto/schema.pyx":139
+  /* "asynctnt/iproto/schema.pyx":148
  *     def __cinit__(self, int schema_id):
  *         self.id = schema_id
  *         self.spaces = {}             # <<<<<<<<<<<<<<
  * 
  *     cdef SchemaSpace get_space(self, space):
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 139, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->spaces);
   __Pyx_DECREF(__pyx_v_self->spaces);
   __pyx_v_self->spaces = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":137
+  /* "asynctnt/iproto/schema.pyx":146
  * @cython.final
  * cdef class Schema:
  *     def __cinit__(self, int schema_id):             # <<<<<<<<<<<<<<
  *         self.id = schema_id
  *         self.spaces = {}
  */
 
@@ -16214,15 +16293,15 @@
   __Pyx_AddTraceback("asynctnt.iproto.protocol.Schema.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":141
+/* "asynctnt/iproto/schema.pyx":150
  *         self.spaces = {}
  * 
  *     cdef SchemaSpace get_space(self, space):             # <<<<<<<<<<<<<<
  *         cdef PyObject *obj_p = \
  *             cpython.dict.PyDict_GetItem(self.spaces, space)
  */
 
@@ -16230,84 +16309,84 @@
   PyObject *__pyx_v_obj_p;
   struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("get_space", 1);
 
-  /* "asynctnt/iproto/schema.pyx":143
+  /* "asynctnt/iproto/schema.pyx":152
  *     cdef SchemaSpace get_space(self, space):
  *         cdef PyObject *obj_p = \
  *             cpython.dict.PyDict_GetItem(self.spaces, space)             # <<<<<<<<<<<<<<
  *         if obj_p is NULL:
  *             return None
  */
   __pyx_t_1 = __pyx_v_self->spaces;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_obj_p = PyDict_GetItem(__pyx_t_1, __pyx_v_space);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":144
+  /* "asynctnt/iproto/schema.pyx":153
  *         cdef PyObject *obj_p = \
  *             cpython.dict.PyDict_GetItem(self.spaces, space)
  *         if obj_p is NULL:             # <<<<<<<<<<<<<<
  *             return None
  *         return <SchemaSpace> obj_p
  */
   __pyx_t_2 = (__pyx_v_obj_p == NULL);
   if (__pyx_t_2) {
 
-    /* "asynctnt/iproto/schema.pyx":145
+    /* "asynctnt/iproto/schema.pyx":154
  *             cpython.dict.PyDict_GetItem(self.spaces, space)
  *         if obj_p is NULL:
  *             return None             # <<<<<<<<<<<<<<
  *         return <SchemaSpace> obj_p
  * 
  */
     __Pyx_XDECREF((PyObject *)__pyx_r);
     __pyx_r = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)Py_None); __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "asynctnt/iproto/schema.pyx":144
+    /* "asynctnt/iproto/schema.pyx":153
  *         cdef PyObject *obj_p = \
  *             cpython.dict.PyDict_GetItem(self.spaces, space)
  *         if obj_p is NULL:             # <<<<<<<<<<<<<<
  *             return None
  *         return <SchemaSpace> obj_p
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":146
+  /* "asynctnt/iproto/schema.pyx":155
  *         if obj_p is NULL:
  *             return None
  *         return <SchemaSpace> obj_p             # <<<<<<<<<<<<<<
  * 
  *     cdef SchemaSpace get_or_create_space(self, space):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)__pyx_v_obj_p));
   __pyx_r = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)__pyx_v_obj_p);
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":141
+  /* "asynctnt/iproto/schema.pyx":150
  *         self.spaces = {}
  * 
  *     cdef SchemaSpace get_space(self, space):             # <<<<<<<<<<<<<<
  *         cdef PyObject *obj_p = \
  *             cpython.dict.PyDict_GetItem(self.spaces, space)
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":148
+/* "asynctnt/iproto/schema.pyx":157
  *         return <SchemaSpace> obj_p
  * 
  *     cdef SchemaSpace get_or_create_space(self, space):             # <<<<<<<<<<<<<<
  *         cdef:
  *             bint is_str, is_int
  */
 
@@ -16326,35 +16405,35 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_or_create_space", 1);
 
-  /* "asynctnt/iproto/schema.pyx":152
+  /* "asynctnt/iproto/schema.pyx":161
  *             bint is_str, is_int
  *             PyObject *obj_p
  *         is_str = isinstance(space, str)             # <<<<<<<<<<<<<<
  *         is_int = isinstance(space, int)
  *         if not is_str and not is_int:
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_space); 
   __pyx_v_is_str = __pyx_t_1;
 
-  /* "asynctnt/iproto/schema.pyx":153
+  /* "asynctnt/iproto/schema.pyx":162
  *             PyObject *obj_p
  *         is_str = isinstance(space, str)
  *         is_int = isinstance(space, int)             # <<<<<<<<<<<<<<
  *         if not is_str and not is_int:
  *             raise TypeError(
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_space); 
   __pyx_v_is_int = __pyx_t_1;
 
-  /* "asynctnt/iproto/schema.pyx":154
+  /* "asynctnt/iproto/schema.pyx":163
  *         is_str = isinstance(space, str)
  *         is_int = isinstance(space, int)
  *         if not is_str and not is_int:             # <<<<<<<<<<<<<<
  *             raise TypeError(
  *                 'Space must be either str or int, got: {}'.format(type(space)))
  */
   __pyx_t_2 = (!__pyx_v_is_str);
@@ -16364,22 +16443,22 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (!__pyx_v_is_int);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "asynctnt/iproto/schema.pyx":156
+    /* "asynctnt/iproto/schema.pyx":165
  *         if not is_str and not is_int:
  *             raise TypeError(
  *                 'Space must be either str or int, got: {}'.format(type(space)))             # <<<<<<<<<<<<<<
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(self.spaces, space)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Space_must_be_either_str_or_int, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 156, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Space_must_be_either_str_or_int, __pyx_n_s_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 165, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
@@ -16391,91 +16470,91 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_5, ((PyObject *)Py_TYPE(__pyx_v_space))};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 156, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 165, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
 
-    /* "asynctnt/iproto/schema.pyx":155
+    /* "asynctnt/iproto/schema.pyx":164
  *         is_int = isinstance(space, int)
  *         if not is_str and not is_int:
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 'Space must be either str or int, got: {}'.format(type(space)))
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 155, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(1, 155, __pyx_L1_error)
+    __PYX_ERR(1, 164, __pyx_L1_error)
 
-    /* "asynctnt/iproto/schema.pyx":154
+    /* "asynctnt/iproto/schema.pyx":163
  *         is_str = isinstance(space, str)
  *         is_int = isinstance(space, int)
  *         if not is_str and not is_int:             # <<<<<<<<<<<<<<
  *             raise TypeError(
  *                 'Space must be either str or int, got: {}'.format(type(space)))
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":158
+  /* "asynctnt/iproto/schema.pyx":167
  *                 'Space must be either str or int, got: {}'.format(type(space)))
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(self.spaces, space)             # <<<<<<<<<<<<<<
  *         if obj_p is NULL:
  *             if is_str:
  */
   __pyx_t_4 = __pyx_v_self->spaces;
   __Pyx_INCREF(__pyx_t_4);
   __pyx_v_obj_p = PyDict_GetItem(__pyx_t_4, __pyx_v_space);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":159
+  /* "asynctnt/iproto/schema.pyx":168
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(self.spaces, space)
  *         if obj_p is NULL:             # <<<<<<<<<<<<<<
  *             if is_str:
  *                 raise TarantoolSchemaError(
  */
   __pyx_t_1 = (__pyx_v_obj_p == NULL);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/schema.pyx":160
+    /* "asynctnt/iproto/schema.pyx":169
  *         obj_p = cpython.dict.PyDict_GetItem(self.spaces, space)
  *         if obj_p is NULL:
  *             if is_str:             # <<<<<<<<<<<<<<
  *                 raise TarantoolSchemaError(
  *                     'Space {} not found'.format(space)
  */
     if (unlikely(__pyx_v_is_str)) {
 
-      /* "asynctnt/iproto/schema.pyx":161
+      /* "asynctnt/iproto/schema.pyx":170
  *         if obj_p is NULL:
  *             if is_str:
  *                 raise TarantoolSchemaError(             # <<<<<<<<<<<<<<
  *                     'Space {} not found'.format(space)
  *                 )
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_TarantoolSchemaError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 161, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_TarantoolSchemaError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 170, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
 
-      /* "asynctnt/iproto/schema.pyx":162
+      /* "asynctnt/iproto/schema.pyx":171
  *             if is_str:
  *                 raise TarantoolSchemaError(
  *                     'Space {} not found'.format(space)             # <<<<<<<<<<<<<<
  *                 )
  *             else:
  */
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Space_not_found, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 162, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Space_not_found, __pyx_n_s_format); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 171, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       __pyx_t_6 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_8)) {
@@ -16487,15 +16566,15 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_v_space};
         __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 162, __pyx_L1_error)
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 171, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __pyx_t_7 = NULL;
       __pyx_t_6 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_3))) {
@@ -16510,70 +16589,70 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 161, __pyx_L1_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 170, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(1, 161, __pyx_L1_error)
+      __PYX_ERR(1, 170, __pyx_L1_error)
 
-      /* "asynctnt/iproto/schema.pyx":160
+      /* "asynctnt/iproto/schema.pyx":169
  *         obj_p = cpython.dict.PyDict_GetItem(self.spaces, space)
  *         if obj_p is NULL:
  *             if is_str:             # <<<<<<<<<<<<<<
  *                 raise TarantoolSchemaError(
  *                     'Space {} not found'.format(space)
  */
     }
 
-    /* "asynctnt/iproto/schema.pyx":165
+    /* "asynctnt/iproto/schema.pyx":174
  *                 )
  *             else:
  *                 return self.create_dummy_space(space)             # <<<<<<<<<<<<<<
  *         return <SchemaSpace> obj_p
  * 
  */
     /*else*/ {
       __Pyx_XDECREF((PyObject *)__pyx_r);
-      __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_space); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 165, __pyx_L1_error)
-      __pyx_t_4 = ((PyObject *)__pyx_f_8asynctnt_6iproto_8protocol_6Schema_create_dummy_space(__pyx_v_self, __pyx_t_6)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 165, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_space); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 174, __pyx_L1_error)
+      __pyx_t_4 = ((PyObject *)__pyx_f_8asynctnt_6iproto_8protocol_6Schema_create_dummy_space(__pyx_v_self, __pyx_t_6)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 174, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_r = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)__pyx_t_4);
       __pyx_t_4 = 0;
       goto __pyx_L0;
     }
 
-    /* "asynctnt/iproto/schema.pyx":159
+    /* "asynctnt/iproto/schema.pyx":168
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(self.spaces, space)
  *         if obj_p is NULL:             # <<<<<<<<<<<<<<
  *             if is_str:
  *                 raise TarantoolSchemaError(
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":166
+  /* "asynctnt/iproto/schema.pyx":175
  *             else:
  *                 return self.create_dummy_space(space)
  *         return <SchemaSpace> obj_p             # <<<<<<<<<<<<<<
  * 
  *     cdef SchemaSpace create_dummy_space(self, int space_id):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)__pyx_v_obj_p));
   __pyx_r = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)__pyx_v_obj_p);
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":148
+  /* "asynctnt/iproto/schema.pyx":157
  *         return <SchemaSpace> obj_p
  * 
  *     cdef SchemaSpace get_or_create_space(self, space):             # <<<<<<<<<<<<<<
  *         cdef:
  *             bint is_str, is_int
  */
 
@@ -16588,15 +16667,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":168
+/* "asynctnt/iproto/schema.pyx":177
  *         return <SchemaSpace> obj_p
  * 
  *     cdef SchemaSpace create_dummy_space(self, int space_id):             # <<<<<<<<<<<<<<
  *         cdef SchemaSpace s
  *         logger.debug('Space %s not found. Creating dummy.', space_id)
  */
 
@@ -16610,27 +16689,27 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("create_dummy_space", 1);
 
-  /* "asynctnt/iproto/schema.pyx":170
+  /* "asynctnt/iproto/schema.pyx":179
  *     cdef SchemaSpace create_dummy_space(self, int space_id):
  *         cdef SchemaSpace s
  *         logger.debug('Space %s not found. Creating dummy.', space_id)             # <<<<<<<<<<<<<<
  *         s = <SchemaSpace> SchemaSpace.__new__(SchemaSpace)
  *         s.sid = space_id
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_space_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_space_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -16643,90 +16722,90 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_kp_u_Space_s_not_found_Creating_dummy, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 170, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 179, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":171
+  /* "asynctnt/iproto/schema.pyx":180
  *         cdef SchemaSpace s
  *         logger.debug('Space %s not found. Creating dummy.', space_id)
  *         s = <SchemaSpace> SchemaSpace.__new__(SchemaSpace)             # <<<<<<<<<<<<<<
  *         s.sid = space_id
  *         s.name = str(space_id)
  */
-  __pyx_t_1 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_SchemaSpace(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 171, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_SchemaSpace(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 180, __pyx_L1_error)
   __Pyx_GOTREF((PyObject *)__pyx_t_1);
   __pyx_t_3 = ((PyObject *)__pyx_t_1);
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_DECREF((PyObject *)__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_s = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":172
+  /* "asynctnt/iproto/schema.pyx":181
  *         logger.debug('Space %s not found. Creating dummy.', space_id)
  *         s = <SchemaSpace> SchemaSpace.__new__(SchemaSpace)
  *         s.sid = space_id             # <<<<<<<<<<<<<<
  *         s.name = str(space_id)
  *         cpython.dict.PyDict_SetItem(self.spaces, space_id, s)
  */
   __pyx_v_s->sid = __pyx_v_space_id;
 
-  /* "asynctnt/iproto/schema.pyx":173
+  /* "asynctnt/iproto/schema.pyx":182
  *         s = <SchemaSpace> SchemaSpace.__new__(SchemaSpace)
  *         s.sid = space_id
  *         s.name = str(space_id)             # <<<<<<<<<<<<<<
  *         cpython.dict.PyDict_SetItem(self.spaces, space_id, s)
  *         return s
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_space_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 173, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_space_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_Str(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 173, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Str(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_s->name);
   __Pyx_DECREF(__pyx_v_s->name);
   __pyx_v_s->name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":174
+  /* "asynctnt/iproto/schema.pyx":183
  *         s.sid = space_id
  *         s.name = str(space_id)
  *         cpython.dict.PyDict_SetItem(self.spaces, space_id, s)             # <<<<<<<<<<<<<<
  *         return s
  * 
  */
   __pyx_t_1 = __pyx_v_self->spaces;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_space_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 174, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_space_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyDict_SetItem(__pyx_t_1, __pyx_t_3, ((PyObject *)__pyx_v_s)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(1, 174, __pyx_L1_error)
+  __pyx_t_5 = PyDict_SetItem(__pyx_t_1, __pyx_t_3, ((PyObject *)__pyx_v_s)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":175
+  /* "asynctnt/iproto/schema.pyx":184
  *         s.name = str(space_id)
  *         cpython.dict.PyDict_SetItem(self.spaces, space_id, s)
  *         return s             # <<<<<<<<<<<<<<
  * 
  *     cdef inline clear(self):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_s);
   __pyx_r = __pyx_v_s;
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":168
+  /* "asynctnt/iproto/schema.pyx":177
  *         return <SchemaSpace> obj_p
  * 
  *     cdef SchemaSpace create_dummy_space(self, int space_id):             # <<<<<<<<<<<<<<
  *         cdef SchemaSpace s
  *         logger.debug('Space %s not found. Creating dummy.', space_id)
  */
 
@@ -16741,15 +16820,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_s);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":177
+/* "asynctnt/iproto/schema.pyx":186
  *         return s
  * 
  *     cdef inline clear(self):             # <<<<<<<<<<<<<<
  *         self.spaces.clear()
  * 
  */
 
@@ -16758,28 +16837,28 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 1);
 
-  /* "asynctnt/iproto/schema.pyx":178
+  /* "asynctnt/iproto/schema.pyx":187
  * 
  *     cdef inline clear(self):
  *         self.spaces.clear()             # <<<<<<<<<<<<<<
  * 
  *     cdef SchemaSpace parse_space(self, space_row):
  */
   if (unlikely(__pyx_v_self->spaces == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "clear");
-    __PYX_ERR(1, 178, __pyx_L1_error)
+    __PYX_ERR(1, 187, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyDict_Clear(__pyx_v_self->spaces); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 178, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_Clear(__pyx_v_self->spaces); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 187, __pyx_L1_error)
 
-  /* "asynctnt/iproto/schema.pyx":177
+  /* "asynctnt/iproto/schema.pyx":186
  *         return s
  * 
  *     cdef inline clear(self):             # <<<<<<<<<<<<<<
  *         self.spaces.clear()
  * 
  */
 
@@ -16791,15 +16870,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":180
+/* "asynctnt/iproto/schema.pyx":189
  *         self.spaces.clear()
  * 
  *     cdef SchemaSpace parse_space(self, space_row):             # <<<<<<<<<<<<<<
  *         cdef:
  *             SchemaSpace sp
  */
 
@@ -16822,464 +16901,464 @@
   Py_ssize_t __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse_space", 1);
 
-  /* "asynctnt/iproto/schema.pyx":187
+  /* "asynctnt/iproto/schema.pyx":196
  *             list format_list
  * 
  *         assert space_row is not None             # <<<<<<<<<<<<<<
  * 
  *         sp = <SchemaSpace> SchemaSpace.__new__(SchemaSpace)
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = (__pyx_v_space_row != Py_None);
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(1, 187, __pyx_L1_error)
+      __PYX_ERR(1, 196, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(1, 187, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(1, 196, __pyx_L1_error)
   #endif
 
-  /* "asynctnt/iproto/schema.pyx":189
+  /* "asynctnt/iproto/schema.pyx":198
  *         assert space_row is not None
  * 
  *         sp = <SchemaSpace> SchemaSpace.__new__(SchemaSpace)             # <<<<<<<<<<<<<<
  *         row_len = <size_t> len(space_row)
  * 
  */
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_SchemaSpace(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 189, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_SchemaSpace(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 198, __pyx_L1_error)
   __Pyx_GOTREF((PyObject *)__pyx_t_2);
   __pyx_t_3 = ((PyObject *)__pyx_t_2);
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_DECREF((PyObject *)__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_sp = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":190
+  /* "asynctnt/iproto/schema.pyx":199
  * 
  *         sp = <SchemaSpace> SchemaSpace.__new__(SchemaSpace)
  *         row_len = <size_t> len(space_row)             # <<<<<<<<<<<<<<
  * 
  *         k = 0
  */
-  __pyx_t_4 = PyObject_Length(__pyx_v_space_row); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 190, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(__pyx_v_space_row); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_v_row_len = ((size_t)__pyx_t_4);
 
-  /* "asynctnt/iproto/schema.pyx":192
+  /* "asynctnt/iproto/schema.pyx":201
  *         row_len = <size_t> len(space_row)
  * 
  *         k = 0             # <<<<<<<<<<<<<<
  *         sp.sid = <int> space_row[k]
  *         k += 1
  */
   __pyx_v_k = 0;
 
-  /* "asynctnt/iproto/schema.pyx":193
+  /* "asynctnt/iproto/schema.pyx":202
  * 
  *         k = 0
  *         sp.sid = <int> space_row[k]             # <<<<<<<<<<<<<<
  *         k += 1
  *         if k < row_len:
  */
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 193, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_sp->sid = ((int)__pyx_t_5);
 
-  /* "asynctnt/iproto/schema.pyx":194
+  /* "asynctnt/iproto/schema.pyx":203
  *         k = 0
  *         sp.sid = <int> space_row[k]
  *         k += 1             # <<<<<<<<<<<<<<
  *         if k < row_len:
  *             sp.owner = <int> space_row[k]
  */
   __pyx_v_k = (__pyx_v_k + 1);
 
-  /* "asynctnt/iproto/schema.pyx":195
+  /* "asynctnt/iproto/schema.pyx":204
  *         sp.sid = <int> space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             sp.owner = <int> space_row[k]
  *         k += 1
  */
   __pyx_t_1 = (__pyx_v_k < __pyx_v_row_len);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/schema.pyx":196
+    /* "asynctnt/iproto/schema.pyx":205
  *         k += 1
  *         if k < row_len:
  *             sp.owner = <int> space_row[k]             # <<<<<<<<<<<<<<
  *         k += 1
  *         if k < row_len:
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 196, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 196, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 205, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_sp->owner = ((int)__pyx_t_5);
 
-    /* "asynctnt/iproto/schema.pyx":195
+    /* "asynctnt/iproto/schema.pyx":204
  *         sp.sid = <int> space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             sp.owner = <int> space_row[k]
  *         k += 1
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":197
+  /* "asynctnt/iproto/schema.pyx":206
  *         if k < row_len:
  *             sp.owner = <int> space_row[k]
  *         k += 1             # <<<<<<<<<<<<<<
  *         if k < row_len:
  *             sp.name = <str> space_row[k]
  */
   __pyx_v_k = (__pyx_v_k + 1);
 
-  /* "asynctnt/iproto/schema.pyx":198
+  /* "asynctnt/iproto/schema.pyx":207
  *             sp.owner = <int> space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             sp.name = <str> space_row[k]
  *         k += 1
  */
   __pyx_t_1 = (__pyx_v_k < __pyx_v_row_len);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/schema.pyx":199
+    /* "asynctnt/iproto/schema.pyx":208
  *         k += 1
  *         if k < row_len:
  *             sp.name = <str> space_row[k]             # <<<<<<<<<<<<<<
  *         k += 1
  *         if k < row_len:
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 199, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = __pyx_t_3;
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_sp->name);
     __Pyx_DECREF(__pyx_v_sp->name);
     __pyx_v_sp->name = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":198
+    /* "asynctnt/iproto/schema.pyx":207
  *             sp.owner = <int> space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             sp.name = <str> space_row[k]
  *         k += 1
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":200
+  /* "asynctnt/iproto/schema.pyx":209
  *         if k < row_len:
  *             sp.name = <str> space_row[k]
  *         k += 1             # <<<<<<<<<<<<<<
  *         if k < row_len:
  *             sp.engine = <str> space_row[k]
  */
   __pyx_v_k = (__pyx_v_k + 1);
 
-  /* "asynctnt/iproto/schema.pyx":201
+  /* "asynctnt/iproto/schema.pyx":210
  *             sp.name = <str> space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             sp.engine = <str> space_row[k]
  *         k += 1
  */
   __pyx_t_1 = (__pyx_v_k < __pyx_v_row_len);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/schema.pyx":202
+    /* "asynctnt/iproto/schema.pyx":211
  *         k += 1
  *         if k < row_len:
  *             sp.engine = <str> space_row[k]             # <<<<<<<<<<<<<<
  *         k += 1
  *         if k < row_len:
  */
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 202, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __pyx_t_2;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GIVEREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_v_sp->engine);
     __Pyx_DECREF(__pyx_v_sp->engine);
     __pyx_v_sp->engine = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":201
+    /* "asynctnt/iproto/schema.pyx":210
  *             sp.name = <str> space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             sp.engine = <str> space_row[k]
  *         k += 1
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":203
+  /* "asynctnt/iproto/schema.pyx":212
  *         if k < row_len:
  *             sp.engine = <str> space_row[k]
  *         k += 1             # <<<<<<<<<<<<<<
  *         if k < row_len:
  *             sp.field_count = <int> space_row[k]
  */
   __pyx_v_k = (__pyx_v_k + 1);
 
-  /* "asynctnt/iproto/schema.pyx":204
+  /* "asynctnt/iproto/schema.pyx":213
  *             sp.engine = <str> space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             sp.field_count = <int> space_row[k]
  *         k += 1
  */
   __pyx_t_1 = (__pyx_v_k < __pyx_v_row_len);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/schema.pyx":205
+    /* "asynctnt/iproto/schema.pyx":214
  *         k += 1
  *         if k < row_len:
  *             sp.field_count = <int> space_row[k]             # <<<<<<<<<<<<<<
  *         k += 1
  *         if k < row_len:
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 205, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 214, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 205, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 214, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_sp->field_count = ((int)__pyx_t_5);
 
-    /* "asynctnt/iproto/schema.pyx":204
+    /* "asynctnt/iproto/schema.pyx":213
  *             sp.engine = <str> space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             sp.field_count = <int> space_row[k]
  *         k += 1
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":206
+  /* "asynctnt/iproto/schema.pyx":215
  *         if k < row_len:
  *             sp.field_count = <int> space_row[k]
  *         k += 1             # <<<<<<<<<<<<<<
  *         if k < row_len:
  *             sp.flags = space_row[k]
  */
   __pyx_v_k = (__pyx_v_k + 1);
 
-  /* "asynctnt/iproto/schema.pyx":207
+  /* "asynctnt/iproto/schema.pyx":216
  *             sp.field_count = <int> space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             sp.flags = space_row[k]
  *         k += 1
  */
   __pyx_t_1 = (__pyx_v_k < __pyx_v_row_len);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/schema.pyx":208
+    /* "asynctnt/iproto/schema.pyx":217
  *         k += 1
  *         if k < row_len:
  *             sp.flags = space_row[k]             # <<<<<<<<<<<<<<
  *         k += 1
  *         if k < row_len:
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 208, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 217, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_v_sp->flags);
     __Pyx_DECREF(__pyx_v_sp->flags);
     __pyx_v_sp->flags = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":207
+    /* "asynctnt/iproto/schema.pyx":216
  *             sp.field_count = <int> space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             sp.flags = space_row[k]
  *         k += 1
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":209
+  /* "asynctnt/iproto/schema.pyx":218
  *         if k < row_len:
  *             sp.flags = space_row[k]
  *         k += 1             # <<<<<<<<<<<<<<
  *         if k < row_len:
  *             # format
  */
   __pyx_v_k = (__pyx_v_k + 1);
 
-  /* "asynctnt/iproto/schema.pyx":210
+  /* "asynctnt/iproto/schema.pyx":219
  *             sp.flags = space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             # format
  *             format_list = <list> space_row[k]
  */
   __pyx_t_1 = (__pyx_v_k < __pyx_v_row_len);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/schema.pyx":212
+    /* "asynctnt/iproto/schema.pyx":221
  *         if k < row_len:
  *             # format
  *             format_list = <list> space_row[k]             # <<<<<<<<<<<<<<
  *             if len(format_list) > 0:
  *                 sp.metadata = <Metadata> Metadata.__new__(Metadata)
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 212, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_space_row, __pyx_v_k, size_t, 0, __Pyx_PyInt_FromSize_t, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = __pyx_t_3;
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_format_list = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":213
+    /* "asynctnt/iproto/schema.pyx":222
  *             # format
  *             format_list = <list> space_row[k]
  *             if len(format_list) > 0:             # <<<<<<<<<<<<<<
  *                 sp.metadata = <Metadata> Metadata.__new__(Metadata)
  *                 for i in range(len(format_list)):
  */
     if (unlikely(__pyx_v_format_list == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(1, 213, __pyx_L1_error)
+      __PYX_ERR(1, 222, __pyx_L1_error)
     }
-    __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_v_format_list); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 213, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_v_format_list); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 222, __pyx_L1_error)
     __pyx_t_1 = (__pyx_t_4 > 0);
     if (__pyx_t_1) {
 
-      /* "asynctnt/iproto/schema.pyx":214
+      /* "asynctnt/iproto/schema.pyx":223
  *             format_list = <list> space_row[k]
  *             if len(format_list) > 0:
  *                 sp.metadata = <Metadata> Metadata.__new__(Metadata)             # <<<<<<<<<<<<<<
  *                 for i in range(len(format_list)):
  *                     field_id = i
  */
-      __pyx_t_2 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Metadata(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Metadata), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 214, __pyx_L1_error)
+      __pyx_t_2 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Metadata(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Metadata), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 223, __pyx_L1_error)
       __Pyx_GOTREF((PyObject *)__pyx_t_2);
       __pyx_t_3 = ((PyObject *)__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_DECREF((PyObject *)__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_GIVEREF(__pyx_t_3);
       __Pyx_GOTREF((PyObject *)__pyx_v_sp->metadata);
       __Pyx_DECREF((PyObject *)__pyx_v_sp->metadata);
       __pyx_v_sp->metadata = ((struct C_Metadata *)__pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":215
+      /* "asynctnt/iproto/schema.pyx":224
  *             if len(format_list) > 0:
  *                 sp.metadata = <Metadata> Metadata.__new__(Metadata)
  *                 for i in range(len(format_list)):             # <<<<<<<<<<<<<<
  *                     field_id = i
  *                     field = <Field> Field.__new__(Field)
  */
       if (unlikely(__pyx_v_format_list == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(1, 215, __pyx_L1_error)
+        __PYX_ERR(1, 224, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_v_format_list); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 215, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_v_format_list); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 224, __pyx_L1_error)
       __pyx_t_6 = __pyx_t_4;
       for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
         __pyx_v_i = __pyx_t_7;
 
-        /* "asynctnt/iproto/schema.pyx":216
+        /* "asynctnt/iproto/schema.pyx":225
  *                 sp.metadata = <Metadata> Metadata.__new__(Metadata)
  *                 for i in range(len(format_list)):
  *                     field_id = i             # <<<<<<<<<<<<<<
  *                     field = <Field> Field.__new__(Field)
  * 
  */
         __pyx_v_field_id = __pyx_v_i;
 
-        /* "asynctnt/iproto/schema.pyx":217
+        /* "asynctnt/iproto/schema.pyx":226
  *                 for i in range(len(format_list)):
  *                     field_id = i
  *                     field = <Field> Field.__new__(Field)             # <<<<<<<<<<<<<<
  * 
  *                     field.name = format_list[i]['name']
  */
-        __pyx_t_3 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Field(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Field), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 217, __pyx_L1_error)
+        __pyx_t_3 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Field(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Field), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 226, __pyx_L1_error)
         __Pyx_GOTREF((PyObject *)__pyx_t_3);
         __pyx_t_2 = ((PyObject *)__pyx_t_3);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_DECREF((PyObject *)__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF_SET(__pyx_v_field, ((struct __pyx_obj_8asynctnt_6iproto_8protocol_Field *)__pyx_t_2));
         __pyx_t_2 = 0;
 
-        /* "asynctnt/iproto/schema.pyx":219
+        /* "asynctnt/iproto/schema.pyx":228
  *                     field = <Field> Field.__new__(Field)
  * 
  *                     field.name = format_list[i]['name']             # <<<<<<<<<<<<<<
  *                     field.type = format_list[i]['type']
  *                     field.is_nullable = format_list[i].get('is_nullable')
  */
         if (unlikely(__pyx_v_format_list == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(1, 219, __pyx_L1_error)
+          __PYX_ERR(1, 228, __pyx_L1_error)
         }
-        __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_format_list, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 219, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_format_list, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 228, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_name_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 219, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_name_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 228, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-        if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_3))) __PYX_ERR(1, 219, __pyx_L1_error)
+        if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_3))) __PYX_ERR(1, 228, __pyx_L1_error)
         __Pyx_GIVEREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_v_field->name);
         __Pyx_DECREF(__pyx_v_field->name);
         __pyx_v_field->name = ((PyObject*)__pyx_t_3);
         __pyx_t_3 = 0;
 
-        /* "asynctnt/iproto/schema.pyx":220
+        /* "asynctnt/iproto/schema.pyx":229
  * 
  *                     field.name = format_list[i]['name']
  *                     field.type = format_list[i]['type']             # <<<<<<<<<<<<<<
  *                     field.is_nullable = format_list[i].get('is_nullable')
  * 
  */
         if (unlikely(__pyx_v_format_list == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(1, 220, __pyx_L1_error)
+          __PYX_ERR(1, 229, __pyx_L1_error)
         }
-        __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_format_list, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 220, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_format_list, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 229, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 220, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_Dict_GetItem(__pyx_t_3, __pyx_n_u_type); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 229, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(1, 220, __pyx_L1_error)
+        if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(1, 229, __pyx_L1_error)
         __Pyx_GIVEREF(__pyx_t_2);
         __Pyx_GOTREF(__pyx_v_field->type);
         __Pyx_DECREF(__pyx_v_field->type);
         __pyx_v_field->type = ((PyObject*)__pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "asynctnt/iproto/schema.pyx":221
+        /* "asynctnt/iproto/schema.pyx":230
  *                     field.name = format_list[i]['name']
  *                     field.type = format_list[i]['type']
  *                     field.is_nullable = format_list[i].get('is_nullable')             # <<<<<<<<<<<<<<
  * 
  *                     sp.metadata.add(field_id, field)
  */
         if (unlikely(__pyx_v_format_list == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(1, 221, __pyx_L1_error)
+          __PYX_ERR(1, 230, __pyx_L1_error)
         }
-        __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_format_list, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 221, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_GetItemInt_List(__pyx_v_format_list, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 230, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 221, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 230, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_3 = NULL;
         __pyx_t_5 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_8))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
@@ -17292,65 +17371,65 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_n_u_is_nullable};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 221, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 230, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __Pyx_GIVEREF(__pyx_t_2);
         __Pyx_GOTREF(__pyx_v_field->is_nullable);
         __Pyx_DECREF(__pyx_v_field->is_nullable);
         __pyx_v_field->is_nullable = __pyx_t_2;
         __pyx_t_2 = 0;
 
-        /* "asynctnt/iproto/schema.pyx":223
+        /* "asynctnt/iproto/schema.pyx":232
  *                     field.is_nullable = format_list[i].get('is_nullable')
  * 
  *                     sp.metadata.add(field_id, field)             # <<<<<<<<<<<<<<
  * 
  *         return sp
  */
-        __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_add(__pyx_v_sp->metadata, __pyx_v_field_id, __pyx_v_field); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 223, __pyx_L1_error)
+        __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_add(__pyx_v_sp->metadata, __pyx_v_field_id, __pyx_v_field); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 232, __pyx_L1_error)
       }
 
-      /* "asynctnt/iproto/schema.pyx":213
+      /* "asynctnt/iproto/schema.pyx":222
  *             # format
  *             format_list = <list> space_row[k]
  *             if len(format_list) > 0:             # <<<<<<<<<<<<<<
  *                 sp.metadata = <Metadata> Metadata.__new__(Metadata)
  *                 for i in range(len(format_list)):
  */
     }
 
-    /* "asynctnt/iproto/schema.pyx":210
+    /* "asynctnt/iproto/schema.pyx":219
  *             sp.flags = space_row[k]
  *         k += 1
  *         if k < row_len:             # <<<<<<<<<<<<<<
  *             # format
  *             format_list = <list> space_row[k]
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":225
+  /* "asynctnt/iproto/schema.pyx":234
  *                     sp.metadata.add(field_id, field)
  * 
  *         return sp             # <<<<<<<<<<<<<<
  * 
  *     cdef SchemaIndex parse_index(self, index_row):
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_sp);
   __pyx_r = __pyx_v_sp;
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":180
+  /* "asynctnt/iproto/schema.pyx":189
  *         self.spaces.clear()
  * 
  *     cdef SchemaSpace parse_space(self, space_row):             # <<<<<<<<<<<<<<
  *         cdef:
  *             SchemaSpace sp
  */
 
@@ -17366,15 +17445,15 @@
   __Pyx_XDECREF(__pyx_v_format_list);
   __Pyx_XDECREF((PyObject *)__pyx_v_field);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":227
+/* "asynctnt/iproto/schema.pyx":236
  *         return sp
  * 
  *     cdef SchemaIndex parse_index(self, index_row):             # <<<<<<<<<<<<<<
  *         cdef:
  *             SchemaIndex idx
  */
 
@@ -17405,195 +17484,195 @@
   uint32_t __pyx_t_15;
   long __pyx_t_16;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse_index", 1);
 
-  /* "asynctnt/iproto/schema.pyx":232
+  /* "asynctnt/iproto/schema.pyx":241
  *             SchemaSpace sp
  *             uint32_t i
  *             int field_id = -1             # <<<<<<<<<<<<<<
  *             str field_type
  * 
  */
   __pyx_v_field_id = -1;
 
-  /* "asynctnt/iproto/schema.pyx":235
+  /* "asynctnt/iproto/schema.pyx":244
  *             str field_type
  * 
  *         assert index_row is not None             # <<<<<<<<<<<<<<
  * 
  *         idx = <SchemaIndex> SchemaIndex.__new__(SchemaIndex)
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = (__pyx_v_index_row != Py_None);
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(1, 235, __pyx_L1_error)
+      __PYX_ERR(1, 244, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(1, 235, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(1, 244, __pyx_L1_error)
   #endif
 
-  /* "asynctnt/iproto/schema.pyx":237
+  /* "asynctnt/iproto/schema.pyx":246
  *         assert index_row is not None
  * 
  *         idx = <SchemaIndex> SchemaIndex.__new__(SchemaIndex)             # <<<<<<<<<<<<<<
  *         idx.sid = <int> index_row[0]
  *         idx.iid = <int> index_row[1]
  */
-  __pyx_t_2 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_SchemaIndex(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 237, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_SchemaIndex(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 246, __pyx_L1_error)
   __Pyx_GOTREF((PyObject *)__pyx_t_2);
   __pyx_t_3 = ((PyObject *)__pyx_t_2);
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_DECREF((PyObject *)__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_idx = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":238
+  /* "asynctnt/iproto/schema.pyx":247
  * 
  *         idx = <SchemaIndex> SchemaIndex.__new__(SchemaIndex)
  *         idx.sid = <int> index_row[0]             # <<<<<<<<<<<<<<
  *         idx.iid = <int> index_row[1]
  *         idx.name = <str> index_row[2]
  */
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 247, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_idx->sid = ((int)__pyx_t_4);
 
-  /* "asynctnt/iproto/schema.pyx":239
+  /* "asynctnt/iproto/schema.pyx":248
  *         idx = <SchemaIndex> SchemaIndex.__new__(SchemaIndex)
  *         idx.sid = <int> index_row[0]
  *         idx.iid = <int> index_row[1]             # <<<<<<<<<<<<<<
  *         idx.name = <str> index_row[2]
  *         idx.index_type = <str> index_row[3]
  */
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 239, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 248, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_idx->iid = ((int)__pyx_t_4);
 
-  /* "asynctnt/iproto/schema.pyx":240
+  /* "asynctnt/iproto/schema.pyx":249
  *         idx.sid = <int> index_row[0]
  *         idx.iid = <int> index_row[1]
  *         idx.name = <str> index_row[2]             # <<<<<<<<<<<<<<
  *         idx.index_type = <str> index_row[3]
  *         idx.unique = <object> index_row[4]
  */
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 240, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 249, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __pyx_t_3;
   __Pyx_INCREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_idx->name);
   __Pyx_DECREF(__pyx_v_idx->name);
   __pyx_v_idx->name = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":241
+  /* "asynctnt/iproto/schema.pyx":250
  *         idx.iid = <int> index_row[1]
  *         idx.name = <str> index_row[2]
  *         idx.index_type = <str> index_row[3]             # <<<<<<<<<<<<<<
  *         idx.unique = <object> index_row[4]
  *         idx.metadata = None
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_index_row, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 241, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_index_row, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __pyx_t_2;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_idx->index_type);
   __Pyx_DECREF(__pyx_v_idx->index_type);
   __pyx_v_idx->index_type = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":242
+  /* "asynctnt/iproto/schema.pyx":251
  *         idx.name = <str> index_row[2]
  *         idx.index_type = <str> index_row[3]
  *         idx.unique = <object> index_row[4]             # <<<<<<<<<<<<<<
  *         idx.metadata = None
  * 
  */
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, 4, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 242, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, 4, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __pyx_t_3;
   __Pyx_INCREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_idx->unique);
   __Pyx_DECREF(__pyx_v_idx->unique);
   __pyx_v_idx->unique = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":243
+  /* "asynctnt/iproto/schema.pyx":252
  *         idx.index_type = <str> index_row[3]
  *         idx.unique = <object> index_row[4]
  *         idx.metadata = None             # <<<<<<<<<<<<<<
  * 
  *         sp = self.get_space(idx.sid)
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF((PyObject *)__pyx_v_idx->metadata);
   __Pyx_DECREF((PyObject *)__pyx_v_idx->metadata);
   __pyx_v_idx->metadata = ((struct C_Metadata *)Py_None);
 
-  /* "asynctnt/iproto/schema.pyx":245
+  /* "asynctnt/iproto/schema.pyx":254
  *         idx.metadata = None
  * 
  *         sp = self.get_space(idx.sid)             # <<<<<<<<<<<<<<
  *         if sp is None:
  *             raise TarantoolSchemaError(
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_idx->sid); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 245, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_idx->sid); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = ((PyObject *)__pyx_f_8asynctnt_6iproto_8protocol_6Schema_get_space(__pyx_v_self, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 245, __pyx_L1_error)
+  __pyx_t_3 = ((PyObject *)__pyx_f_8asynctnt_6iproto_8protocol_6Schema_get_space(__pyx_v_self, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_sp = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":246
+  /* "asynctnt/iproto/schema.pyx":255
  * 
  *         sp = self.get_space(idx.sid)
  *         if sp is None:             # <<<<<<<<<<<<<<
  *             raise TarantoolSchemaError(
  *                 'Space with id {} not found'.format(idx.sid))
  */
   __pyx_t_1 = (((PyObject *)__pyx_v_sp) == Py_None);
   if (unlikely(__pyx_t_1)) {
 
-    /* "asynctnt/iproto/schema.pyx":247
+    /* "asynctnt/iproto/schema.pyx":256
  *         sp = self.get_space(idx.sid)
  *         if sp is None:
  *             raise TarantoolSchemaError(             # <<<<<<<<<<<<<<
  *                 'Space with id {} not found'.format(idx.sid))
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_TarantoolSchemaError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 247, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_TarantoolSchemaError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 256, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "asynctnt/iproto/schema.pyx":248
+    /* "asynctnt/iproto/schema.pyx":257
  *         if sp is None:
  *             raise TarantoolSchemaError(
  *                 'Space with id {} not found'.format(idx.sid))             # <<<<<<<<<<<<<<
  * 
  *         if sp.metadata is not None:
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Space_with_id_not_found, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 248, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Space_with_id_not_found, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 257, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_idx->sid); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 248, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_int(__pyx_v_idx->sid); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 257, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_8 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_8)) {
@@ -17606,15 +17685,15 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_t_7};
       __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 248, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 257, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __pyx_t_6 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_2))) {
@@ -17629,72 +17708,72 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 247, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 256, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 247, __pyx_L1_error)
+    __PYX_ERR(1, 256, __pyx_L1_error)
 
-    /* "asynctnt/iproto/schema.pyx":246
+    /* "asynctnt/iproto/schema.pyx":255
  * 
  *         sp = self.get_space(idx.sid)
  *         if sp is None:             # <<<<<<<<<<<<<<
  *             raise TarantoolSchemaError(
  *                 'Space with id {} not found'.format(idx.sid))
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":250
+  /* "asynctnt/iproto/schema.pyx":259
  *                 'Space with id {} not found'.format(idx.sid))
  * 
  *         if sp.metadata is not None:             # <<<<<<<<<<<<<<
  *             parts = index_row[5]
  *             idx.metadata = <Metadata> Metadata.__new__(Metadata)
  */
   __pyx_t_1 = (((PyObject *)__pyx_v_sp->metadata) != Py_None);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/schema.pyx":251
+    /* "asynctnt/iproto/schema.pyx":260
  * 
  *         if sp.metadata is not None:
  *             parts = index_row[5]             # <<<<<<<<<<<<<<
  *             idx.metadata = <Metadata> Metadata.__new__(Metadata)
  * 
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, 5, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 251, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, 5, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_parts = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":252
+    /* "asynctnt/iproto/schema.pyx":261
  *         if sp.metadata is not None:
  *             parts = index_row[5]
  *             idx.metadata = <Metadata> Metadata.__new__(Metadata)             # <<<<<<<<<<<<<<
  * 
  *             if isinstance(parts, (list, tuple)):
  */
-    __pyx_t_3 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Metadata(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Metadata), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 252, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Metadata(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Metadata), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 261, __pyx_L1_error)
     __Pyx_GOTREF((PyObject *)__pyx_t_3);
     __pyx_t_2 = ((PyObject *)__pyx_t_3);
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_DECREF((PyObject *)__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF((PyObject *)__pyx_v_idx->metadata);
     __Pyx_DECREF((PyObject *)__pyx_v_idx->metadata);
     __pyx_v_idx->metadata = ((struct C_Metadata *)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":254
+    /* "asynctnt/iproto/schema.pyx":263
  *             idx.metadata = <Metadata> Metadata.__new__(Metadata)
  * 
  *             if isinstance(parts, (list, tuple)):             # <<<<<<<<<<<<<<
  *                 for part in parts:
  *                     field = <Field> Field.__new__(Field)
  */
     __pyx_t_9 = PyList_Check(__pyx_v_parts); 
@@ -17704,105 +17783,105 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_9 = PyTuple_Check(__pyx_v_parts); 
     __pyx_t_1 = __pyx_t_9;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_1) {
 
-      /* "asynctnt/iproto/schema.pyx":255
+      /* "asynctnt/iproto/schema.pyx":264
  * 
  *             if isinstance(parts, (list, tuple)):
  *                 for part in parts:             # <<<<<<<<<<<<<<
  *                     field = <Field> Field.__new__(Field)
  *                     field.name = ''
  */
       if (likely(PyList_CheckExact(__pyx_v_parts)) || PyTuple_CheckExact(__pyx_v_parts)) {
         __pyx_t_2 = __pyx_v_parts; __Pyx_INCREF(__pyx_t_2);
         __pyx_t_10 = 0;
         __pyx_t_11 = NULL;
       } else {
-        __pyx_t_10 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_parts); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 255, __pyx_L1_error)
+        __pyx_t_10 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_parts); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 264, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 255, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 264, __pyx_L1_error)
       }
       for (;;) {
         if (likely(!__pyx_t_11)) {
           if (likely(PyList_CheckExact(__pyx_t_2))) {
             {
               Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 255, __pyx_L1_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 264, __pyx_L1_error)
               #endif
               if (__pyx_t_10 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_3); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(1, 255, __pyx_L1_error)
+            __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_3); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(1, 264, __pyx_L1_error)
             #else
-            __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 255, __pyx_L1_error)
+            __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 264, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_3);
             #endif
           } else {
             {
               Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 255, __pyx_L1_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 264, __pyx_L1_error)
               #endif
               if (__pyx_t_10 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_3); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(1, 255, __pyx_L1_error)
+            __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_10); __Pyx_INCREF(__pyx_t_3); __pyx_t_10++; if (unlikely((0 < 0))) __PYX_ERR(1, 264, __pyx_L1_error)
             #else
-            __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 255, __pyx_L1_error)
+            __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_10); __pyx_t_10++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 264, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_3);
             #endif
           }
         } else {
           __pyx_t_3 = __pyx_t_11(__pyx_t_2);
           if (unlikely(!__pyx_t_3)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(1, 255, __pyx_L1_error)
+              else __PYX_ERR(1, 264, __pyx_L1_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_3);
         }
         __Pyx_XDECREF_SET(__pyx_v_part, __pyx_t_3);
         __pyx_t_3 = 0;
 
-        /* "asynctnt/iproto/schema.pyx":256
+        /* "asynctnt/iproto/schema.pyx":265
  *             if isinstance(parts, (list, tuple)):
  *                 for part in parts:
  *                     field = <Field> Field.__new__(Field)             # <<<<<<<<<<<<<<
  *                     field.name = ''
  * 
  */
-        __pyx_t_3 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Field(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Field), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 256, __pyx_L1_error)
+        __pyx_t_3 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Field(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Field), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 265, __pyx_L1_error)
         __Pyx_GOTREF((PyObject *)__pyx_t_3);
         __pyx_t_5 = ((PyObject *)__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_DECREF((PyObject *)__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF_SET(__pyx_v_field, ((struct __pyx_obj_8asynctnt_6iproto_8protocol_Field *)__pyx_t_5));
         __pyx_t_5 = 0;
 
-        /* "asynctnt/iproto/schema.pyx":257
+        /* "asynctnt/iproto/schema.pyx":266
  *                 for part in parts:
  *                     field = <Field> Field.__new__(Field)
  *                     field.name = ''             # <<<<<<<<<<<<<<
  * 
  *                     if isinstance(part, (list, tuple)):
  */
         __Pyx_INCREF(__pyx_kp_u__3);
         __Pyx_GIVEREF(__pyx_kp_u__3);
         __Pyx_GOTREF(__pyx_v_field->name);
         __Pyx_DECREF(__pyx_v_field->name);
         __pyx_v_field->name = __pyx_kp_u__3;
 
-        /* "asynctnt/iproto/schema.pyx":259
+        /* "asynctnt/iproto/schema.pyx":268
  *                     field.name = ''
  * 
  *                     if isinstance(part, (list, tuple)):             # <<<<<<<<<<<<<<
  *                         assert len(part) == 2, 'Part len must be 2'
  *                         field_id = part[0]
  */
         __pyx_t_9 = PyList_Check(__pyx_v_part); 
@@ -17812,142 +17891,142 @@
           goto __pyx_L11_bool_binop_done;
         }
         __pyx_t_9 = PyTuple_Check(__pyx_v_part); 
         __pyx_t_1 = __pyx_t_9;
         __pyx_L11_bool_binop_done:;
         if (__pyx_t_1) {
 
-          /* "asynctnt/iproto/schema.pyx":260
+          /* "asynctnt/iproto/schema.pyx":269
  * 
  *                     if isinstance(part, (list, tuple)):
  *                         assert len(part) == 2, 'Part len must be 2'             # <<<<<<<<<<<<<<
  *                         field_id = part[0]
  *                         field.type = part[1]
  */
           #ifndef CYTHON_WITHOUT_ASSERTIONS
           if (unlikely(__pyx_assertions_enabled())) {
-            __pyx_t_12 = PyObject_Length(__pyx_v_part); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(1, 260, __pyx_L1_error)
+            __pyx_t_12 = PyObject_Length(__pyx_v_part); if (unlikely(__pyx_t_12 == ((Py_ssize_t)-1))) __PYX_ERR(1, 269, __pyx_L1_error)
             __pyx_t_1 = (__pyx_t_12 == 2);
             if (unlikely(!__pyx_t_1)) {
               __Pyx_Raise(__pyx_builtin_AssertionError, __pyx_kp_u_Part_len_must_be_2, 0, 0);
-              __PYX_ERR(1, 260, __pyx_L1_error)
+              __PYX_ERR(1, 269, __pyx_L1_error)
             }
           }
           #else
-          if ((1)); else __PYX_ERR(1, 260, __pyx_L1_error)
+          if ((1)); else __PYX_ERR(1, 269, __pyx_L1_error)
           #endif
 
-          /* "asynctnt/iproto/schema.pyx":261
+          /* "asynctnt/iproto/schema.pyx":270
  *                     if isinstance(part, (list, tuple)):
  *                         assert len(part) == 2, 'Part len must be 2'
  *                         field_id = part[0]             # <<<<<<<<<<<<<<
  *                         field.type = part[1]
  *                     elif isinstance(part, dict):
  */
-          __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_part, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 261, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_part, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 270, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_5); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 261, __pyx_L1_error)
+          __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_5); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 270, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __pyx_v_field_id = __pyx_t_4;
 
-          /* "asynctnt/iproto/schema.pyx":262
+          /* "asynctnt/iproto/schema.pyx":271
  *                         assert len(part) == 2, 'Part len must be 2'
  *                         field_id = part[0]
  *                         field.type = part[1]             # <<<<<<<<<<<<<<
  *                     elif isinstance(part, dict):
  *                         field_id = part['field']
  */
-          __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_part, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 262, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_part, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 271, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
-          if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_5))) __PYX_ERR(1, 262, __pyx_L1_error)
+          if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_5))) __PYX_ERR(1, 271, __pyx_L1_error)
           __Pyx_GIVEREF(__pyx_t_5);
           __Pyx_GOTREF(__pyx_v_field->type);
           __Pyx_DECREF(__pyx_v_field->type);
           __pyx_v_field->type = ((PyObject*)__pyx_t_5);
           __pyx_t_5 = 0;
 
-          /* "asynctnt/iproto/schema.pyx":259
+          /* "asynctnt/iproto/schema.pyx":268
  *                     field.name = ''
  * 
  *                     if isinstance(part, (list, tuple)):             # <<<<<<<<<<<<<<
  *                         assert len(part) == 2, 'Part len must be 2'
  *                         field_id = part[0]
  */
           goto __pyx_L10;
         }
 
-        /* "asynctnt/iproto/schema.pyx":263
+        /* "asynctnt/iproto/schema.pyx":272
  *                         field_id = part[0]
  *                         field.type = part[1]
  *                     elif isinstance(part, dict):             # <<<<<<<<<<<<<<
  *                         field_id = part['field']
  *                         field.type = part['type']
  */
         __pyx_t_1 = PyDict_Check(__pyx_v_part); 
         if (likely(__pyx_t_1)) {
 
-          /* "asynctnt/iproto/schema.pyx":264
+          /* "asynctnt/iproto/schema.pyx":273
  *                         field.type = part[1]
  *                     elif isinstance(part, dict):
  *                         field_id = part['field']             # <<<<<<<<<<<<<<
  *                         field.type = part['type']
  *                         # TODO: add is_nullable and collation if we really need
  */
-          __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_part, __pyx_n_u_field); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 264, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_part, __pyx_n_u_field); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 273, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_5); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 264, __pyx_L1_error)
+          __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_5); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 273, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __pyx_v_field_id = __pyx_t_4;
 
-          /* "asynctnt/iproto/schema.pyx":265
+          /* "asynctnt/iproto/schema.pyx":274
  *                     elif isinstance(part, dict):
  *                         field_id = part['field']
  *                         field.type = part['type']             # <<<<<<<<<<<<<<
  *                         # TODO: add is_nullable and collation if we really need
  *                         # TODO: it in a python driver
  */
-          __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_part, __pyx_n_u_type); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 265, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyObject_Dict_GetItem(__pyx_v_part, __pyx_n_u_type); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 274, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
-          if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_5))) __PYX_ERR(1, 265, __pyx_L1_error)
+          if (!(likely(PyUnicode_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_5))) __PYX_ERR(1, 274, __pyx_L1_error)
           __Pyx_GIVEREF(__pyx_t_5);
           __Pyx_GOTREF(__pyx_v_field->type);
           __Pyx_DECREF(__pyx_v_field->type);
           __pyx_v_field->type = ((PyObject*)__pyx_t_5);
           __pyx_t_5 = 0;
 
-          /* "asynctnt/iproto/schema.pyx":263
+          /* "asynctnt/iproto/schema.pyx":272
  *                         field_id = part[0]
  *                         field.type = part[1]
  *                     elif isinstance(part, dict):             # <<<<<<<<<<<<<<
  *                         field_id = part['field']
  *                         field.type = part['type']
  */
           goto __pyx_L10;
         }
 
-        /* "asynctnt/iproto/schema.pyx":269
+        /* "asynctnt/iproto/schema.pyx":278
  *                         # TODO: it in a python driver
  *                     else:
  *                         raise TypeError(             # <<<<<<<<<<<<<<
  *                             "unexpected type of part: {}. "
  *                             "must be either dict or list/tuple".format(
  */
         /*else*/ {
 
-          /* "asynctnt/iproto/schema.pyx":271
+          /* "asynctnt/iproto/schema.pyx":280
  *                         raise TypeError(
  *                             "unexpected type of part: {}. "
  *                             "must be either dict or list/tuple".format(             # <<<<<<<<<<<<<<
  *                                 type(part)
  *                             )
  */
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_unexpected_type_of_part_must_be, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 271, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_unexpected_type_of_part_must_be, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 280, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
 
-          /* "asynctnt/iproto/schema.pyx":272
+          /* "asynctnt/iproto/schema.pyx":281
  *                             "unexpected type of part: {}. "
  *                             "must be either dict or list/tuple".format(
  *                                 type(part)             # <<<<<<<<<<<<<<
  *                             )
  *                         )
  */
           __pyx_t_6 = NULL;
@@ -17964,93 +18043,93 @@
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_6, ((PyObject *)Py_TYPE(__pyx_v_part))};
             __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-            if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 271, __pyx_L1_error)
+            if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 280, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_5);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           }
 
-          /* "asynctnt/iproto/schema.pyx":269
+          /* "asynctnt/iproto/schema.pyx":278
  *                         # TODO: it in a python driver
  *                     else:
  *                         raise TypeError(             # <<<<<<<<<<<<<<
  *                             "unexpected type of part: {}. "
  *                             "must be either dict or list/tuple".format(
  */
-          __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 269, __pyx_L1_error)
+          __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 278, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
           __Pyx_Raise(__pyx_t_3, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __PYX_ERR(1, 269, __pyx_L1_error)
+          __PYX_ERR(1, 278, __pyx_L1_error)
         }
         __pyx_L10:;
 
-        /* "asynctnt/iproto/schema.pyx":276
+        /* "asynctnt/iproto/schema.pyx":285
  *                         )
  * 
  *                     if field_id < sp.metadata.len():             # <<<<<<<<<<<<<<
  *                         field.name = sp.metadata.name_by_id(field_id)
  *                     else:
  */
-        __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(__pyx_v_sp->metadata); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 276, __pyx_L1_error)
+        __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(__pyx_v_sp->metadata); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 285, __pyx_L1_error)
         __pyx_t_1 = (__pyx_v_field_id < __pyx_t_4);
         if (__pyx_t_1) {
 
-          /* "asynctnt/iproto/schema.pyx":277
+          /* "asynctnt/iproto/schema.pyx":286
  * 
  *                     if field_id < sp.metadata.len():
  *                         field.name = sp.metadata.name_by_id(field_id)             # <<<<<<<<<<<<<<
  *                     else:
  *                         logger.debug(
  */
-          __pyx_t_3 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id(__pyx_v_sp->metadata, __pyx_v_field_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 277, __pyx_L1_error)
+          __pyx_t_3 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id(__pyx_v_sp->metadata, __pyx_v_field_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 286, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_v_field->name);
           __Pyx_DECREF(__pyx_v_field->name);
           __pyx_v_field->name = ((PyObject*)__pyx_t_3);
           __pyx_t_3 = 0;
 
-          /* "asynctnt/iproto/schema.pyx":276
+          /* "asynctnt/iproto/schema.pyx":285
  *                         )
  * 
  *                     if field_id < sp.metadata.len():             # <<<<<<<<<<<<<<
  *                         field.name = sp.metadata.name_by_id(field_id)
  *                     else:
  */
           goto __pyx_L13;
         }
 
-        /* "asynctnt/iproto/schema.pyx":279
+        /* "asynctnt/iproto/schema.pyx":288
  *                         field.name = sp.metadata.name_by_id(field_id)
  *                     else:
  *                         logger.debug(             # <<<<<<<<<<<<<<
  *                             'Field #%d of space %s is not '
  *                             'in space format definition', field_id, sp.name)
  */
         /*else*/ {
-          __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logger); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 279, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_logger); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 288, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_debug); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 279, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_debug); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 288, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-          /* "asynctnt/iproto/schema.pyx":281
+          /* "asynctnt/iproto/schema.pyx":290
  *                         logger.debug(
  *                             'Field #%d of space %s is not '
  *                             'in space format definition', field_id, sp.name)             # <<<<<<<<<<<<<<
  * 
  *                     idx.metadata.add(field_id, field)
  */
-          __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_field_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 281, __pyx_L1_error)
+          __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_field_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 290, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           __pyx_t_7 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
           if (unlikely(PyMethod_Check(__pyx_t_6))) {
             __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
             if (likely(__pyx_t_7)) {
@@ -18063,181 +18142,181 @@
           }
           #endif
           {
             PyObject *__pyx_callargs[4] = {__pyx_t_7, __pyx_kp_u_Field_d_of_space_s_is_not_in_spa, __pyx_t_5, __pyx_v_sp->name};
             __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_4, 3+__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
             __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-            if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 279, __pyx_L1_error)
+            if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 288, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           }
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_L13:;
 
-        /* "asynctnt/iproto/schema.pyx":283
+        /* "asynctnt/iproto/schema.pyx":292
  *                             'in space format definition', field_id, sp.name)
  * 
  *                     idx.metadata.add(field_id, field)             # <<<<<<<<<<<<<<
  *             else:
  *                 for i in range(parts):
  */
-        __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_add(__pyx_v_idx->metadata, __pyx_v_field_id, __pyx_v_field); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 283, __pyx_L1_error)
+        __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_add(__pyx_v_idx->metadata, __pyx_v_field_id, __pyx_v_field); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 292, __pyx_L1_error)
 
-        /* "asynctnt/iproto/schema.pyx":255
+        /* "asynctnt/iproto/schema.pyx":264
  * 
  *             if isinstance(parts, (list, tuple)):
  *                 for part in parts:             # <<<<<<<<<<<<<<
  *                     field = <Field> Field.__new__(Field)
  *                     field.name = ''
  */
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":254
+      /* "asynctnt/iproto/schema.pyx":263
  *             idx.metadata = <Metadata> Metadata.__new__(Metadata)
  * 
  *             if isinstance(parts, (list, tuple)):             # <<<<<<<<<<<<<<
  *                 for part in parts:
  *                     field = <Field> Field.__new__(Field)
  */
       goto __pyx_L5;
     }
 
-    /* "asynctnt/iproto/schema.pyx":285
+    /* "asynctnt/iproto/schema.pyx":294
  *                     idx.metadata.add(field_id, field)
  *             else:
  *                 for i in range(parts):             # <<<<<<<<<<<<<<
  *                     field = <Field> Field.__new__(Field)
  * 
  */
     /*else*/ {
-      __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_parts); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 285, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyInt_As_long(__pyx_v_parts); if (unlikely((__pyx_t_13 == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 294, __pyx_L1_error)
       __pyx_t_14 = __pyx_t_13;
       for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
         __pyx_v_i = __pyx_t_15;
 
-        /* "asynctnt/iproto/schema.pyx":286
+        /* "asynctnt/iproto/schema.pyx":295
  *             else:
  *                 for i in range(parts):
  *                     field = <Field> Field.__new__(Field)             # <<<<<<<<<<<<<<
  * 
  *                     field_id = index_row[5 + 1 + i * 2]
  */
-        __pyx_t_2 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Field(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Field), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 286, __pyx_L1_error)
+        __pyx_t_2 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Field(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Field), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 295, __pyx_L1_error)
         __Pyx_GOTREF((PyObject *)__pyx_t_2);
         __pyx_t_3 = ((PyObject *)__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_DECREF((PyObject *)__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF_SET(__pyx_v_field, ((struct __pyx_obj_8asynctnt_6iproto_8protocol_Field *)__pyx_t_3));
         __pyx_t_3 = 0;
 
-        /* "asynctnt/iproto/schema.pyx":288
+        /* "asynctnt/iproto/schema.pyx":297
  *                     field = <Field> Field.__new__(Field)
  * 
  *                     field_id = index_row[5 + 1 + i * 2]             # <<<<<<<<<<<<<<
  *                     field.type = index_row[5 + 2 + i * 2]
  *                     field.name = ''
  */
         __pyx_t_16 = (0x6 + (__pyx_v_i * 2));
-        __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, __pyx_t_16, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 288, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, __pyx_t_16, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 297, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 288, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 297, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_v_field_id = __pyx_t_4;
 
-        /* "asynctnt/iproto/schema.pyx":289
+        /* "asynctnt/iproto/schema.pyx":298
  * 
  *                     field_id = index_row[5 + 1 + i * 2]
  *                     field.type = index_row[5 + 2 + i * 2]             # <<<<<<<<<<<<<<
  *                     field.name = ''
  * 
  */
         __pyx_t_16 = (0x7 + (__pyx_v_i * 2));
-        __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, __pyx_t_16, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 289, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_index_row, __pyx_t_16, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 298, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_3))) __PYX_ERR(1, 289, __pyx_L1_error)
+        if (!(likely(PyUnicode_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_3))) __PYX_ERR(1, 298, __pyx_L1_error)
         __Pyx_GIVEREF(__pyx_t_3);
         __Pyx_GOTREF(__pyx_v_field->type);
         __Pyx_DECREF(__pyx_v_field->type);
         __pyx_v_field->type = ((PyObject*)__pyx_t_3);
         __pyx_t_3 = 0;
 
-        /* "asynctnt/iproto/schema.pyx":290
+        /* "asynctnt/iproto/schema.pyx":299
  *                     field_id = index_row[5 + 1 + i * 2]
  *                     field.type = index_row[5 + 2 + i * 2]
  *                     field.name = ''             # <<<<<<<<<<<<<<
  * 
  *                     if field_id < sp.metadata.len():
  */
         __Pyx_INCREF(__pyx_kp_u__3);
         __Pyx_GIVEREF(__pyx_kp_u__3);
         __Pyx_GOTREF(__pyx_v_field->name);
         __Pyx_DECREF(__pyx_v_field->name);
         __pyx_v_field->name = __pyx_kp_u__3;
 
-        /* "asynctnt/iproto/schema.pyx":292
+        /* "asynctnt/iproto/schema.pyx":301
  *                     field.name = ''
  * 
  *                     if field_id < sp.metadata.len():             # <<<<<<<<<<<<<<
  *                         field.name = sp.metadata.name_by_id(field_id)
  *                     else:
  */
-        __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(__pyx_v_sp->metadata); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 292, __pyx_L1_error)
+        __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(__pyx_v_sp->metadata); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 301, __pyx_L1_error)
         __pyx_t_1 = (__pyx_v_field_id < __pyx_t_4);
         if (__pyx_t_1) {
 
-          /* "asynctnt/iproto/schema.pyx":293
+          /* "asynctnt/iproto/schema.pyx":302
  * 
  *                     if field_id < sp.metadata.len():
  *                         field.name = sp.metadata.name_by_id(field_id)             # <<<<<<<<<<<<<<
  *                     else:
  *                         logger.debug(
  */
-          __pyx_t_3 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id(__pyx_v_sp->metadata, __pyx_v_field_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 293, __pyx_L1_error)
+          __pyx_t_3 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id(__pyx_v_sp->metadata, __pyx_v_field_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 302, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           __Pyx_GIVEREF(__pyx_t_3);
           __Pyx_GOTREF(__pyx_v_field->name);
           __Pyx_DECREF(__pyx_v_field->name);
           __pyx_v_field->name = ((PyObject*)__pyx_t_3);
           __pyx_t_3 = 0;
 
-          /* "asynctnt/iproto/schema.pyx":292
+          /* "asynctnt/iproto/schema.pyx":301
  *                     field.name = ''
  * 
  *                     if field_id < sp.metadata.len():             # <<<<<<<<<<<<<<
  *                         field.name = sp.metadata.name_by_id(field_id)
  *                     else:
  */
           goto __pyx_L17;
         }
 
-        /* "asynctnt/iproto/schema.pyx":295
+        /* "asynctnt/iproto/schema.pyx":304
  *                         field.name = sp.metadata.name_by_id(field_id)
  *                     else:
  *                         logger.debug(             # <<<<<<<<<<<<<<
  *                             'Field #%d of space %s is not '
  *                             'in space format definition', field_id, sp.name)
  */
         /*else*/ {
-          __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 295, __pyx_L1_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_logger); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 304, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
-          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 295, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_debug); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 304, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-          /* "asynctnt/iproto/schema.pyx":297
+          /* "asynctnt/iproto/schema.pyx":306
  *                         logger.debug(
  *                             'Field #%d of space %s is not '
  *                             'in space format definition', field_id, sp.name)             # <<<<<<<<<<<<<<
  * 
  *                     idx.metadata.add(field_id, field)
  */
-          __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_field_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 297, __pyx_L1_error)
+          __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_field_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 306, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __pyx_t_5 = NULL;
           __pyx_t_4 = 0;
           #if CYTHON_UNPACK_METHODS
           if (unlikely(PyMethod_Check(__pyx_t_6))) {
             __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
             if (likely(__pyx_t_5)) {
@@ -18250,56 +18329,56 @@
           }
           #endif
           {
             PyObject *__pyx_callargs[4] = {__pyx_t_5, __pyx_kp_u_Field_d_of_space_s_is_not_in_spa, __pyx_t_2, __pyx_v_sp->name};
             __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_4, 3+__pyx_t_4);
             __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-            if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 295, __pyx_L1_error)
+            if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 304, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           }
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __pyx_L17:;
 
-        /* "asynctnt/iproto/schema.pyx":299
+        /* "asynctnt/iproto/schema.pyx":308
  *                             'in space format definition', field_id, sp.name)
  * 
  *                     idx.metadata.add(field_id, field)             # <<<<<<<<<<<<<<
  * 
  *         return idx
  */
-        __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_add(__pyx_v_idx->metadata, __pyx_v_field_id, __pyx_v_field); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 299, __pyx_L1_error)
+        __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_add(__pyx_v_idx->metadata, __pyx_v_field_id, __pyx_v_field); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L1_error)
       }
     }
     __pyx_L5:;
 
-    /* "asynctnt/iproto/schema.pyx":250
+    /* "asynctnt/iproto/schema.pyx":259
  *                 'Space with id {} not found'.format(idx.sid))
  * 
  *         if sp.metadata is not None:             # <<<<<<<<<<<<<<
  *             parts = index_row[5]
  *             idx.metadata = <Metadata> Metadata.__new__(Metadata)
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":301
+  /* "asynctnt/iproto/schema.pyx":310
  *                     idx.metadata.add(field_id, field)
  * 
  *         return idx             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_idx);
   __pyx_r = __pyx_v_idx;
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":227
+  /* "asynctnt/iproto/schema.pyx":236
  *         return sp
  * 
  *     cdef SchemaIndex parse_index(self, index_row):             # <<<<<<<<<<<<<<
  *         cdef:
  *             SchemaIndex idx
  */
 
@@ -18320,15 +18399,15 @@
   __Pyx_XDECREF(__pyx_v_part);
   __Pyx_XDECREF((PyObject *)__pyx_v_field);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":304
+/* "asynctnt/iproto/schema.pyx":313
  * 
  *     @staticmethod
  *     cdef Schema parse(int64_t schema_id, spaces, indexes):             # <<<<<<<<<<<<<<
  *         cdef:
  *             Schema s
  */
 
@@ -18348,296 +18427,296 @@
   int __pyx_t_6;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse", 1);
 
-  /* "asynctnt/iproto/schema.pyx":310
+  /* "asynctnt/iproto/schema.pyx":319
  *             SchemaIndex idx
  * 
  *         s = <Schema> Schema.__new__(Schema, <int> schema_id)             # <<<<<<<<<<<<<<
  *         for space_row in spaces:
  *             sp = s.parse_space(space_row)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(((int)__pyx_v_schema_id)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 310, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(((int)__pyx_v_schema_id)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 310, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 319, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(1, 310, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(1, 319, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_1 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Schema(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Schema), __pyx_t_2, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 310, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_tp_new_8asynctnt_6iproto_8protocol_Schema(((PyTypeObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Schema), __pyx_t_2, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 319, __pyx_L1_error)
   __Pyx_GOTREF((PyObject *)__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = ((PyObject *)__pyx_t_1);
   __Pyx_INCREF(__pyx_t_2);
   __Pyx_DECREF((PyObject *)__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_s = ((struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":311
+  /* "asynctnt/iproto/schema.pyx":320
  * 
  *         s = <Schema> Schema.__new__(Schema, <int> schema_id)
  *         for space_row in spaces:             # <<<<<<<<<<<<<<
  *             sp = s.parse_space(space_row)
  *             cpython.dict.PyDict_SetItem(s.spaces, sp.sid, sp)
  */
   if (likely(PyList_CheckExact(__pyx_v_spaces)) || PyTuple_CheckExact(__pyx_v_spaces)) {
     __pyx_t_2 = __pyx_v_spaces; __Pyx_INCREF(__pyx_t_2);
     __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_spaces); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 311, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_spaces); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 320, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 311, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 320, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 311, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 320, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 311, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 320, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 311, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 320, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 311, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 320, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 311, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 320, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 311, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 320, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 311, __pyx_L1_error)
+          else __PYX_ERR(1, 320, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_space_row, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":312
+    /* "asynctnt/iproto/schema.pyx":321
  *         s = <Schema> Schema.__new__(Schema, <int> schema_id)
  *         for space_row in spaces:
  *             sp = s.parse_space(space_row)             # <<<<<<<<<<<<<<
  *             cpython.dict.PyDict_SetItem(s.spaces, sp.sid, sp)
  *             if sp.name:
  */
-    __pyx_t_1 = ((PyObject *)__pyx_f_8asynctnt_6iproto_8protocol_6Schema_parse_space(__pyx_v_s, __pyx_v_space_row)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 312, __pyx_L1_error)
+    __pyx_t_1 = ((PyObject *)__pyx_f_8asynctnt_6iproto_8protocol_6Schema_parse_space(__pyx_v_s, __pyx_v_space_row)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 321, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_sp, ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":313
+    /* "asynctnt/iproto/schema.pyx":322
  *         for space_row in spaces:
  *             sp = s.parse_space(space_row)
  *             cpython.dict.PyDict_SetItem(s.spaces, sp.sid, sp)             # <<<<<<<<<<<<<<
  *             if sp.name:
  *                 cpython.dict.PyDict_SetItem(s.spaces, sp.name, sp)
  */
     __pyx_t_1 = __pyx_v_s->spaces;
     __Pyx_INCREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_sp->sid); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 313, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_sp->sid); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 322, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyDict_SetItem(__pyx_t_1, __pyx_t_5, ((PyObject *)__pyx_v_sp)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 313, __pyx_L1_error)
+    __pyx_t_6 = PyDict_SetItem(__pyx_t_1, __pyx_t_5, ((PyObject *)__pyx_v_sp)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 322, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":314
+    /* "asynctnt/iproto/schema.pyx":323
  *             sp = s.parse_space(space_row)
  *             cpython.dict.PyDict_SetItem(s.spaces, sp.sid, sp)
  *             if sp.name:             # <<<<<<<<<<<<<<
  *                 cpython.dict.PyDict_SetItem(s.spaces, sp.name, sp)
  * 
  */
     __pyx_t_7 = (__pyx_v_sp->name != Py_None)&&(__Pyx_PyUnicode_IS_TRUE(__pyx_v_sp->name) != 0);
     if (__pyx_t_7) {
 
-      /* "asynctnt/iproto/schema.pyx":315
+      /* "asynctnt/iproto/schema.pyx":324
  *             cpython.dict.PyDict_SetItem(s.spaces, sp.sid, sp)
  *             if sp.name:
  *                 cpython.dict.PyDict_SetItem(s.spaces, sp.name, sp)             # <<<<<<<<<<<<<<
  * 
  *         for index_row in indexes:
  */
       __pyx_t_5 = __pyx_v_s->spaces;
       __Pyx_INCREF(__pyx_t_5);
       __pyx_t_1 = __pyx_v_sp->name;
       __Pyx_INCREF(__pyx_t_1);
-      __pyx_t_6 = PyDict_SetItem(__pyx_t_5, __pyx_t_1, ((PyObject *)__pyx_v_sp)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 315, __pyx_L1_error)
+      __pyx_t_6 = PyDict_SetItem(__pyx_t_5, __pyx_t_1, ((PyObject *)__pyx_v_sp)); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 324, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":314
+      /* "asynctnt/iproto/schema.pyx":323
  *             sp = s.parse_space(space_row)
  *             cpython.dict.PyDict_SetItem(s.spaces, sp.sid, sp)
  *             if sp.name:             # <<<<<<<<<<<<<<
  *                 cpython.dict.PyDict_SetItem(s.spaces, sp.name, sp)
  * 
  */
     }
 
-    /* "asynctnt/iproto/schema.pyx":311
+    /* "asynctnt/iproto/schema.pyx":320
  * 
  *         s = <Schema> Schema.__new__(Schema, <int> schema_id)
  *         for space_row in spaces:             # <<<<<<<<<<<<<<
  *             sp = s.parse_space(space_row)
  *             cpython.dict.PyDict_SetItem(s.spaces, sp.sid, sp)
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":317
+  /* "asynctnt/iproto/schema.pyx":326
  *                 cpython.dict.PyDict_SetItem(s.spaces, sp.name, sp)
  * 
  *         for index_row in indexes:             # <<<<<<<<<<<<<<
  *             idx = s.parse_index(index_row)
  *             sp = s.spaces[idx.sid]
  */
   if (likely(PyList_CheckExact(__pyx_v_indexes)) || PyTuple_CheckExact(__pyx_v_indexes)) {
     __pyx_t_2 = __pyx_v_indexes; __Pyx_INCREF(__pyx_t_2);
     __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_indexes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 317, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_indexes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 326, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 317, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 326, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 317, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 326, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 317, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 326, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 317, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 326, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 317, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 326, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 317, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 326, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 317, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 326, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 317, __pyx_L1_error)
+          else __PYX_ERR(1, 326, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_index_row, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":318
+    /* "asynctnt/iproto/schema.pyx":327
  * 
  *         for index_row in indexes:
  *             idx = s.parse_index(index_row)             # <<<<<<<<<<<<<<
  *             sp = s.spaces[idx.sid]
  *             sp.add_index(idx)
  */
-    __pyx_t_1 = ((PyObject *)__pyx_f_8asynctnt_6iproto_8protocol_6Schema_parse_index(__pyx_v_s, __pyx_v_index_row)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 318, __pyx_L1_error)
+    __pyx_t_1 = ((PyObject *)__pyx_f_8asynctnt_6iproto_8protocol_6Schema_parse_index(__pyx_v_s, __pyx_v_index_row)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 327, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_idx, ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":319
+    /* "asynctnt/iproto/schema.pyx":328
  *         for index_row in indexes:
  *             idx = s.parse_index(index_row)
  *             sp = s.spaces[idx.sid]             # <<<<<<<<<<<<<<
  *             sp.add_index(idx)
  * 
  */
     if (unlikely(__pyx_v_s->spaces == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(1, 319, __pyx_L1_error)
+      __PYX_ERR(1, 328, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_idx->sid); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 319, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_idx->sid); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_s->spaces, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 319, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_GetItem(__pyx_v_s->spaces, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace))))) __PYX_ERR(1, 319, __pyx_L1_error)
+    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace))))) __PYX_ERR(1, 328, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_sp, ((struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":320
+    /* "asynctnt/iproto/schema.pyx":329
  *             idx = s.parse_index(index_row)
  *             sp = s.spaces[idx.sid]
  *             sp.add_index(idx)             # <<<<<<<<<<<<<<
  * 
  *         return s
  */
-    __pyx_f_8asynctnt_6iproto_8protocol_11SchemaSpace_add_index(__pyx_v_sp, __pyx_v_idx); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 320, __pyx_L1_error)
+    __pyx_f_8asynctnt_6iproto_8protocol_11SchemaSpace_add_index(__pyx_v_sp, __pyx_v_idx); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 329, __pyx_L1_error)
 
-    /* "asynctnt/iproto/schema.pyx":317
+    /* "asynctnt/iproto/schema.pyx":326
  *                 cpython.dict.PyDict_SetItem(s.spaces, sp.name, sp)
  * 
  *         for index_row in indexes:             # <<<<<<<<<<<<<<
  *             idx = s.parse_index(index_row)
  *             sp = s.spaces[idx.sid]
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":322
+  /* "asynctnt/iproto/schema.pyx":331
  *             sp.add_index(idx)
  * 
  *         return s             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):  # pragma: nocover
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_s);
   __pyx_r = __pyx_v_s;
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":304
+  /* "asynctnt/iproto/schema.pyx":313
  * 
  *     @staticmethod
  *     cdef Schema parse(int64_t schema_id, spaces, indexes):             # <<<<<<<<<<<<<<
  *         cdef:
  *             Schema s
  */
 
@@ -18655,15 +18734,15 @@
   __Pyx_XDECREF(__pyx_v_space_row);
   __Pyx_XDECREF(__pyx_v_index_row);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":324
+/* "asynctnt/iproto/schema.pyx":333
  *         return s
  * 
  *     def __repr__(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return '<Schema spaces={}>'.format(len(self.spaces))
  * 
  */
 
@@ -18692,33 +18771,33 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 1);
 
-  /* "asynctnt/iproto/schema.pyx":325
+  /* "asynctnt/iproto/schema.pyx":334
  * 
  *     def __repr__(self):  # pragma: nocover
  *         return '<Schema spaces={}>'.format(len(self.spaces))             # <<<<<<<<<<<<<<
  * 
  * cdef list dict_to_list_fields(dict d, Metadata metadata, bint default_none):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Schema_spaces, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 325, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Schema_spaces, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __pyx_v_self->spaces;
   __Pyx_INCREF(__pyx_t_3);
   if (unlikely(__pyx_t_3 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(1, 325, __pyx_L1_error)
+    __PYX_ERR(1, 334, __pyx_L1_error)
   }
-  __pyx_t_4 = PyDict_Size(__pyx_t_3); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 325, __pyx_L1_error)
+  __pyx_t_4 = PyDict_Size(__pyx_t_3); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 334, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 325, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
@@ -18731,23 +18810,23 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 325, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 334, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":324
+  /* "asynctnt/iproto/schema.pyx":333
  *         return s
  * 
  *     def __repr__(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return '<Schema spaces={}>'.format(len(self.spaces))
  * 
  */
 
@@ -18761,15 +18840,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":62
+/* "asynctnt/iproto/schema.pxd":63
  * cdef class Schema:
  *     cdef:
  *         readonly dict spaces             # <<<<<<<<<<<<<<
  *         readonly int id
  * 
  */
 
@@ -18800,15 +18879,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pxd":63
+/* "asynctnt/iproto/schema.pxd":64
  *     cdef:
  *         readonly dict spaces
  *         readonly int id             # <<<<<<<<<<<<<<
  * 
  *     cdef SchemaSpace get_space(self, space)
  */
 
@@ -18832,15 +18911,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->id); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 63, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->id); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -19063,15 +19142,15 @@
   __Pyx_AddTraceback("asynctnt.iproto.protocol.Schema.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/schema.pyx":327
+/* "asynctnt/iproto/schema.pyx":336
  *         return '<Schema spaces={}>'.format(len(self.spaces))
  * 
  * cdef list dict_to_list_fields(dict d, Metadata metadata, bint default_none):             # <<<<<<<<<<<<<<
  *     cdef:
  *         list tpl
  */
 
@@ -19099,342 +19178,342 @@
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dict_to_list_fields", 1);
 
-  /* "asynctnt/iproto/schema.pyx":337
+  /* "asynctnt/iproto/schema.pyx":346
  *         PyObject *obj_p
  * 
  *     assert metadata is not None             # <<<<<<<<<<<<<<
  *     assert d is not None
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = (((PyObject *)__pyx_v_metadata) != Py_None);
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(1, 337, __pyx_L1_error)
+      __PYX_ERR(1, 346, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(1, 337, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(1, 346, __pyx_L1_error)
   #endif
 
-  /* "asynctnt/iproto/schema.pyx":338
+  /* "asynctnt/iproto/schema.pyx":347
  * 
  *     assert metadata is not None
  *     assert d is not None             # <<<<<<<<<<<<<<
  * 
  *     tpl = []
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = (__pyx_v_d != ((PyObject*)Py_None));
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(1, 338, __pyx_L1_error)
+      __PYX_ERR(1, 347, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(1, 338, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(1, 347, __pyx_L1_error)
   #endif
 
-  /* "asynctnt/iproto/schema.pyx":340
+  /* "asynctnt/iproto/schema.pyx":349
  *     assert d is not None
  * 
  *     tpl = []             # <<<<<<<<<<<<<<
  *     used_count = <int32_t> cpython.dict.PyDict_Size(d)
  * 
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 340, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 349, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_tpl = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "asynctnt/iproto/schema.pyx":341
+  /* "asynctnt/iproto/schema.pyx":350
  * 
  *     tpl = []
  *     used_count = <int32_t> cpython.dict.PyDict_Size(d)             # <<<<<<<<<<<<<<
  * 
  *     for field_id in range(metadata.len()):
  */
-  __pyx_t_3 = PyDict_Size(__pyx_v_d); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 341, __pyx_L1_error)
+  __pyx_t_3 = PyDict_Size(__pyx_v_d); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1L))) __PYX_ERR(1, 350, __pyx_L1_error)
   __pyx_v_used_count = ((int32_t)__pyx_t_3);
 
-  /* "asynctnt/iproto/schema.pyx":343
+  /* "asynctnt/iproto/schema.pyx":352
  *     used_count = <int32_t> cpython.dict.PyDict_Size(d)
  * 
  *     for field_id in range(metadata.len()):             # <<<<<<<<<<<<<<
  *         field_name = metadata.name_by_id(field_id)
  * 
  */
-  __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(__pyx_v_metadata); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(__pyx_v_metadata); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 352, __pyx_L1_error)
   __pyx_t_5 = __pyx_t_4;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_field_id = __pyx_t_6;
 
-    /* "asynctnt/iproto/schema.pyx":344
+    /* "asynctnt/iproto/schema.pyx":353
  * 
  *     for field_id in range(metadata.len()):
  *         field_name = metadata.name_by_id(field_id)             # <<<<<<<<<<<<<<
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(d, field_name)
  */
-    __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id(__pyx_v_metadata, __pyx_v_field_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 344, __pyx_L1_error)
+    __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id(__pyx_v_metadata, __pyx_v_field_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 353, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_field_name, ((PyObject*)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":346
+    /* "asynctnt/iproto/schema.pyx":355
  *         field_name = metadata.name_by_id(field_id)
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(d, field_name)             # <<<<<<<<<<<<<<
  *         if obj_p is not NULL:
  *             value = <object> obj_p
  */
     __pyx_v_obj_p = PyDict_GetItem(__pyx_v_d, __pyx_v_field_name);
 
-    /* "asynctnt/iproto/schema.pyx":347
+    /* "asynctnt/iproto/schema.pyx":356
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(d, field_name)
  *         if obj_p is not NULL:             # <<<<<<<<<<<<<<
  *             value = <object> obj_p
  *             used_count -= 1
  */
     __pyx_t_1 = (__pyx_v_obj_p != NULL);
     if (__pyx_t_1) {
 
-      /* "asynctnt/iproto/schema.pyx":348
+      /* "asynctnt/iproto/schema.pyx":357
  *         obj_p = cpython.dict.PyDict_GetItem(d, field_name)
  *         if obj_p is not NULL:
  *             value = <object> obj_p             # <<<<<<<<<<<<<<
  *             used_count -= 1
  *             tpl.append(value)
  */
       __pyx_t_2 = ((PyObject *)__pyx_v_obj_p);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":349
+      /* "asynctnt/iproto/schema.pyx":358
  *         if obj_p is not NULL:
  *             value = <object> obj_p
  *             used_count -= 1             # <<<<<<<<<<<<<<
  *             tpl.append(value)
  *         else:
  */
       __pyx_v_used_count = (__pyx_v_used_count - 1);
 
-      /* "asynctnt/iproto/schema.pyx":350
+      /* "asynctnt/iproto/schema.pyx":359
  *             value = <object> obj_p
  *             used_count -= 1
  *             tpl.append(value)             # <<<<<<<<<<<<<<
  *         else:
  *             if default_none:
  */
-      __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_tpl, __pyx_v_value); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(1, 350, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_tpl, __pyx_v_value); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(1, 359, __pyx_L1_error)
 
-      /* "asynctnt/iproto/schema.pyx":347
+      /* "asynctnt/iproto/schema.pyx":356
  * 
  *         obj_p = cpython.dict.PyDict_GetItem(d, field_name)
  *         if obj_p is not NULL:             # <<<<<<<<<<<<<<
  *             value = <object> obj_p
  *             used_count -= 1
  */
       goto __pyx_L5;
     }
 
-    /* "asynctnt/iproto/schema.pyx":352
+    /* "asynctnt/iproto/schema.pyx":361
  *             tpl.append(value)
  *         else:
  *             if default_none:             # <<<<<<<<<<<<<<
  *                 tpl.append(None)
  * 
  */
     /*else*/ {
       if (__pyx_v_default_none) {
 
-        /* "asynctnt/iproto/schema.pyx":353
+        /* "asynctnt/iproto/schema.pyx":362
  *         else:
  *             if default_none:
  *                 tpl.append(None)             # <<<<<<<<<<<<<<
  * 
  *     # Warn user if he used any of unknown fields
  */
-        __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_tpl, Py_None); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(1, 353, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_tpl, Py_None); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(1, 362, __pyx_L1_error)
 
-        /* "asynctnt/iproto/schema.pyx":352
+        /* "asynctnt/iproto/schema.pyx":361
  *             tpl.append(value)
  *         else:
  *             if default_none:             # <<<<<<<<<<<<<<
  *                 tpl.append(None)
  * 
  */
       }
     }
     __pyx_L5:;
   }
 
-  /* "asynctnt/iproto/schema.pyx":356
+  /* "asynctnt/iproto/schema.pyx":365
  * 
  *     # Warn user if he used any of unknown fields
  *     if used_count != 0:             # <<<<<<<<<<<<<<
  *         used = {}
  *         for field_id in range(metadata.len()):
  */
   __pyx_t_1 = (__pyx_v_used_count != 0);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/schema.pyx":357
+    /* "asynctnt/iproto/schema.pyx":366
  *     # Warn user if he used any of unknown fields
  *     if used_count != 0:
  *         used = {}             # <<<<<<<<<<<<<<
  *         for field_id in range(metadata.len()):
  *             field_name = metadata.name_by_id(field_id)
  */
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 357, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 366, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_used = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":358
+    /* "asynctnt/iproto/schema.pyx":367
  *     if used_count != 0:
  *         used = {}
  *         for field_id in range(metadata.len()):             # <<<<<<<<<<<<<<
  *             field_name = metadata.name_by_id(field_id)
  * 
  */
-    __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(__pyx_v_metadata); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 358, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len(__pyx_v_metadata); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 367, __pyx_L1_error)
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_field_id = __pyx_t_6;
 
-      /* "asynctnt/iproto/schema.pyx":359
+      /* "asynctnt/iproto/schema.pyx":368
  *         used = {}
  *         for field_id in range(metadata.len()):
  *             field_name = metadata.name_by_id(field_id)             # <<<<<<<<<<<<<<
  * 
  *             if <bint> cpython.dict.PyDict_Contains(d, field_name):
  */
-      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id(__pyx_v_metadata, __pyx_v_field_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 359, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id(__pyx_v_metadata, __pyx_v_field_id); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 368, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_v_field_name, ((PyObject*)__pyx_t_2));
       __pyx_t_2 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":361
+      /* "asynctnt/iproto/schema.pyx":370
  *             field_name = metadata.name_by_id(field_id)
  * 
  *             if <bint> cpython.dict.PyDict_Contains(d, field_name):             # <<<<<<<<<<<<<<
  *                 used[field_name] = None
  *         if <bint> cpython.dict.PyDict_Contains(d, ''):
  */
-      __pyx_t_8 = PyDict_Contains(__pyx_v_d, __pyx_v_field_name); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(1, 361, __pyx_L1_error)
+      __pyx_t_8 = PyDict_Contains(__pyx_v_d, __pyx_v_field_name); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(1, 370, __pyx_L1_error)
       __pyx_t_1 = (__pyx_t_8 != 0);
       if (__pyx_t_1) {
 
-        /* "asynctnt/iproto/schema.pyx":362
+        /* "asynctnt/iproto/schema.pyx":371
  * 
  *             if <bint> cpython.dict.PyDict_Contains(d, field_name):
  *                 used[field_name] = None             # <<<<<<<<<<<<<<
  *         if <bint> cpython.dict.PyDict_Contains(d, ''):
  *             used[''] = None
  */
-        if (unlikely((PyDict_SetItem(__pyx_v_used, __pyx_v_field_name, Py_None) < 0))) __PYX_ERR(1, 362, __pyx_L1_error)
+        if (unlikely((PyDict_SetItem(__pyx_v_used, __pyx_v_field_name, Py_None) < 0))) __PYX_ERR(1, 371, __pyx_L1_error)
 
-        /* "asynctnt/iproto/schema.pyx":361
+        /* "asynctnt/iproto/schema.pyx":370
  *             field_name = metadata.name_by_id(field_id)
  * 
  *             if <bint> cpython.dict.PyDict_Contains(d, field_name):             # <<<<<<<<<<<<<<
  *                 used[field_name] = None
  *         if <bint> cpython.dict.PyDict_Contains(d, ''):
  */
       }
     }
 
-    /* "asynctnt/iproto/schema.pyx":363
+    /* "asynctnt/iproto/schema.pyx":372
  *             if <bint> cpython.dict.PyDict_Contains(d, field_name):
  *                 used[field_name] = None
  *         if <bint> cpython.dict.PyDict_Contains(d, ''):             # <<<<<<<<<<<<<<
  *             used[''] = None
  * 
  */
-    __pyx_t_4 = PyDict_Contains(__pyx_v_d, __pyx_kp_u__3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 363, __pyx_L1_error)
+    __pyx_t_4 = PyDict_Contains(__pyx_v_d, __pyx_kp_u__3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 372, __pyx_L1_error)
     __pyx_t_1 = (__pyx_t_4 != 0);
     if (__pyx_t_1) {
 
-      /* "asynctnt/iproto/schema.pyx":364
+      /* "asynctnt/iproto/schema.pyx":373
  *                 used[field_name] = None
  *         if <bint> cpython.dict.PyDict_Contains(d, ''):
  *             used[''] = None             # <<<<<<<<<<<<<<
  * 
  *         for f in d:
  */
-      if (unlikely((PyDict_SetItem(__pyx_v_used, __pyx_kp_u__3, Py_None) < 0))) __PYX_ERR(1, 364, __pyx_L1_error)
+      if (unlikely((PyDict_SetItem(__pyx_v_used, __pyx_kp_u__3, Py_None) < 0))) __PYX_ERR(1, 373, __pyx_L1_error)
 
-      /* "asynctnt/iproto/schema.pyx":363
+      /* "asynctnt/iproto/schema.pyx":372
  *             if <bint> cpython.dict.PyDict_Contains(d, field_name):
  *                 used[field_name] = None
  *         if <bint> cpython.dict.PyDict_Contains(d, ''):             # <<<<<<<<<<<<<<
  *             used[''] = None
  * 
  */
     }
 
-    /* "asynctnt/iproto/schema.pyx":366
+    /* "asynctnt/iproto/schema.pyx":375
  *             used[''] = None
  * 
  *         for f in d:             # <<<<<<<<<<<<<<
  *             if f not in used:
  *                 logger.warning(
  */
     __pyx_t_3 = 0;
     if (unlikely(__pyx_v_d == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(1, 366, __pyx_L1_error)
+      __PYX_ERR(1, 375, __pyx_L1_error)
     }
-    __pyx_t_10 = __Pyx_dict_iterator(__pyx_v_d, 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_4)); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 366, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_dict_iterator(__pyx_v_d, 1, ((PyObject *)NULL), (&__pyx_t_9), (&__pyx_t_4)); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 375, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_XDECREF(__pyx_t_2);
     __pyx_t_2 = __pyx_t_10;
     __pyx_t_10 = 0;
     while (1) {
       __pyx_t_5 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_9, &__pyx_t_3, &__pyx_t_10, NULL, NULL, __pyx_t_4);
       if (unlikely(__pyx_t_5 == 0)) break;
-      if (unlikely(__pyx_t_5 == -1)) __PYX_ERR(1, 366, __pyx_L1_error)
+      if (unlikely(__pyx_t_5 == -1)) __PYX_ERR(1, 375, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_XDECREF_SET(__pyx_v_f, __pyx_t_10);
       __pyx_t_10 = 0;
 
-      /* "asynctnt/iproto/schema.pyx":367
+      /* "asynctnt/iproto/schema.pyx":376
  * 
  *         for f in d:
  *             if f not in used:             # <<<<<<<<<<<<<<
  *                 logger.warning(
  *                     'Field \'%s\' in supplied dict is unknown as '
  */
-      __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_f, __pyx_v_used, Py_NE)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 367, __pyx_L1_error)
+      __pyx_t_1 = (__Pyx_PyDict_ContainsTF(__pyx_v_f, __pyx_v_used, Py_NE)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 376, __pyx_L1_error)
       if (__pyx_t_1) {
 
-        /* "asynctnt/iproto/schema.pyx":368
+        /* "asynctnt/iproto/schema.pyx":377
  *         for f in d:
  *             if f not in used:
  *                 logger.warning(             # <<<<<<<<<<<<<<
  *                     'Field \'%s\' in supplied dict is unknown as '
  *                     'a tuple field for selected index. Skipping.',
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_logger); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 368, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_logger); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 377, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
-        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_warning); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 368, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_warning); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 377, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-        /* "asynctnt/iproto/schema.pyx":371
+        /* "asynctnt/iproto/schema.pyx":380
  *                     'Field \'%s\' in supplied dict is unknown as '
  *                     'a tuple field for selected index. Skipping.',
  *                     f             # <<<<<<<<<<<<<<
  *                 )
  *     return tpl
  */
         __pyx_t_11 = NULL;
@@ -19451,51 +19530,51 @@
           }
         }
         #endif
         {
           PyObject *__pyx_callargs[3] = {__pyx_t_11, __pyx_kp_u_Field_s_in_supplied_dict_is_unkn, __pyx_v_f};
           __pyx_t_10 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-          if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 368, __pyx_L1_error)
+          if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 377, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_10);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         }
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-        /* "asynctnt/iproto/schema.pyx":367
+        /* "asynctnt/iproto/schema.pyx":376
  * 
  *         for f in d:
  *             if f not in used:             # <<<<<<<<<<<<<<
  *                 logger.warning(
  *                     'Field \'%s\' in supplied dict is unknown as '
  */
       }
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "asynctnt/iproto/schema.pyx":356
+    /* "asynctnt/iproto/schema.pyx":365
  * 
  *     # Warn user if he used any of unknown fields
  *     if used_count != 0:             # <<<<<<<<<<<<<<
  *         used = {}
  *         for field_id in range(metadata.len()):
  */
   }
 
-  /* "asynctnt/iproto/schema.pyx":373
+  /* "asynctnt/iproto/schema.pyx":382
  *                     f
  *                 )
  *     return tpl             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_tpl);
   __pyx_r = __pyx_v_tpl;
   goto __pyx_L0;
 
-  /* "asynctnt/iproto/schema.pyx":327
+  /* "asynctnt/iproto/schema.pyx":336
  *         return '<Schema spaces={}>'.format(len(self.spaces))
  * 
  * cdef list dict_to_list_fields(dict d, Metadata metadata, bint default_none):             # <<<<<<<<<<<<<<
  *     cdef:
  *         list tpl
  */
 
@@ -32557,15 +32636,18 @@
   uint32_t __pyx_v_ops_len;
   uint32_t __pyx_v_op_len;
   PyObject *__pyx_v_str_temp = 0;
   char *__pyx_v_op_str_c;
   Py_ssize_t __pyx_v_op_str_len;
   char __pyx_v_op;
   uint32_t __pyx_v_extra_length;
+  int __pyx_v_field_encode_as_str;
   uint64_t __pyx_v_field_no;
+  char *__pyx_v_field_str_c;
+  Py_ssize_t __pyx_v_field_str_len;
   PyObject *__pyx_v_field_no_obj = 0;
   uint32_t __pyx_v_splice_position;
   uint32_t __pyx_v_splice_offset;
   PyObject *__pyx_v_operation = NULL;
   PyObject *__pyx_v_op_type_str = NULL;
   PyObject *__pyx_v_op_argument = NULL;
   PyObject *__pyx_v_splice_position_obj = NULL;
@@ -32584,834 +32666,794 @@
   int __pyx_t_10;
   uint32_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode_update_ops", 1);
 
-  /* "asynctnt/iproto/requests/update.pyx":31
+  /* "asynctnt/iproto/requests/update.pyx":34
  *         uint32_t splice_position, splice_offset
  * 
+ *     field_encode_as_str = 0             # <<<<<<<<<<<<<<
+ *     field_str_c = NULL
+ * 
+ */
+  __pyx_v_field_encode_as_str = 0;
+
+  /* "asynctnt/iproto/requests/update.pyx":35
+ * 
+ *     field_encode_as_str = 0
+ *     field_str_c = NULL             # <<<<<<<<<<<<<<
+ * 
+ *     begin = NULL
+ */
+  __pyx_v_field_str_c = NULL;
+
+  /* "asynctnt/iproto/requests/update.pyx":37
+ *     field_str_c = NULL
+ * 
  *     begin = NULL             # <<<<<<<<<<<<<<
  * 
  *     if operations is not None:
  */
   __pyx_v_begin = NULL;
 
-  /* "asynctnt/iproto/requests/update.pyx":33
+  /* "asynctnt/iproto/requests/update.pyx":39
  *     begin = NULL
  * 
  *     if operations is not None:             # <<<<<<<<<<<<<<
  *         ops_len = <uint32_t> cpython.list.PyList_GET_SIZE(operations)
  *     else:
  */
   __pyx_t_1 = (__pyx_v_operations != ((PyObject*)Py_None));
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/requests/update.pyx":34
+    /* "asynctnt/iproto/requests/update.pyx":40
  * 
  *     if operations is not None:
  *         ops_len = <uint32_t> cpython.list.PyList_GET_SIZE(operations)             # <<<<<<<<<<<<<<
  *     else:
  *         ops_len = 0
  */
     __pyx_v_ops_len = ((uint32_t)PyList_GET_SIZE(__pyx_v_operations));
 
-    /* "asynctnt/iproto/requests/update.pyx":33
+    /* "asynctnt/iproto/requests/update.pyx":39
  *     begin = NULL
  * 
  *     if operations is not None:             # <<<<<<<<<<<<<<
  *         ops_len = <uint32_t> cpython.list.PyList_GET_SIZE(operations)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "asynctnt/iproto/requests/update.pyx":36
+  /* "asynctnt/iproto/requests/update.pyx":42
  *         ops_len = <uint32_t> cpython.list.PyList_GET_SIZE(operations)
  *     else:
  *         ops_len = 0             # <<<<<<<<<<<<<<
  * 
  *     p = buffer.mp_encode_array(p, ops_len)
  */
   /*else*/ {
     __pyx_v_ops_len = 0;
   }
   __pyx_L3:;
 
-  /* "asynctnt/iproto/requests/update.pyx":38
+  /* "asynctnt/iproto/requests/update.pyx":44
  *         ops_len = 0
  * 
  *     p = buffer.mp_encode_array(p, ops_len)             # <<<<<<<<<<<<<<
  *     if ops_len == 0:
  *         return p
  */
-  __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_array(__pyx_v_buffer, __pyx_v_p, __pyx_v_ops_len); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 38, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_array(__pyx_v_buffer, __pyx_v_p, __pyx_v_ops_len); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 44, __pyx_L1_error)
   __pyx_v_p = __pyx_t_2;
 
-  /* "asynctnt/iproto/requests/update.pyx":39
+  /* "asynctnt/iproto/requests/update.pyx":45
  * 
  *     p = buffer.mp_encode_array(p, ops_len)
  *     if ops_len == 0:             # <<<<<<<<<<<<<<
  *         return p
  * 
  */
   __pyx_t_1 = (__pyx_v_ops_len == 0);
   if (__pyx_t_1) {
 
-    /* "asynctnt/iproto/requests/update.pyx":40
+    /* "asynctnt/iproto/requests/update.pyx":46
  *     p = buffer.mp_encode_array(p, ops_len)
  *     if ops_len == 0:
  *         return p             # <<<<<<<<<<<<<<
  * 
  *     for operation in operations:
  */
     __pyx_r = __pyx_v_p;
     goto __pyx_L0;
 
-    /* "asynctnt/iproto/requests/update.pyx":39
+    /* "asynctnt/iproto/requests/update.pyx":45
  * 
  *     p = buffer.mp_encode_array(p, ops_len)
  *     if ops_len == 0:             # <<<<<<<<<<<<<<
  *         return p
  * 
  */
   }
 
-  /* "asynctnt/iproto/requests/update.pyx":42
+  /* "asynctnt/iproto/requests/update.pyx":48
  *         return p
  * 
  *     for operation in operations:             # <<<<<<<<<<<<<<
  *         if isinstance(operation, tuple):
  *             op_len = cpython.tuple.PyTuple_GET_SIZE(operation)
  */
   if (unlikely(__pyx_v_operations == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(4, 42, __pyx_L1_error)
+    __PYX_ERR(4, 48, __pyx_L1_error)
   }
   __pyx_t_3 = __pyx_v_operations; __Pyx_INCREF(__pyx_t_3);
   __pyx_t_4 = 0;
   for (;;) {
     {
       Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
       #if !CYTHON_ASSUME_SAFE_MACROS
-      if (unlikely((__pyx_temp < 0))) __PYX_ERR(4, 42, __pyx_L1_error)
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(4, 48, __pyx_L1_error)
       #endif
       if (__pyx_t_4 >= __pyx_temp) break;
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_5); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(4, 42, __pyx_L1_error)
+    __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_5); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(4, 48, __pyx_L1_error)
     #else
-    __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 42, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 48, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_operation, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "asynctnt/iproto/requests/update.pyx":43
+    /* "asynctnt/iproto/requests/update.pyx":49
  * 
  *     for operation in operations:
  *         if isinstance(operation, tuple):             # <<<<<<<<<<<<<<
  *             op_len = cpython.tuple.PyTuple_GET_SIZE(operation)
  *         elif isinstance(operation, list):
  */
     __pyx_t_1 = PyTuple_Check(__pyx_v_operation); 
     if (__pyx_t_1) {
 
-      /* "asynctnt/iproto/requests/update.pyx":44
+      /* "asynctnt/iproto/requests/update.pyx":50
  *     for operation in operations:
  *         if isinstance(operation, tuple):
  *             op_len = cpython.tuple.PyTuple_GET_SIZE(operation)             # <<<<<<<<<<<<<<
  *         elif isinstance(operation, list):
  *             op_len = cpython.list.PyList_GET_SIZE(operation)
  */
       __pyx_v_op_len = PyTuple_GET_SIZE(__pyx_v_operation);
 
-      /* "asynctnt/iproto/requests/update.pyx":43
+      /* "asynctnt/iproto/requests/update.pyx":49
  * 
  *     for operation in operations:
  *         if isinstance(operation, tuple):             # <<<<<<<<<<<<<<
  *             op_len = cpython.tuple.PyTuple_GET_SIZE(operation)
  *         elif isinstance(operation, list):
  */
       goto __pyx_L7;
     }
 
-    /* "asynctnt/iproto/requests/update.pyx":45
+    /* "asynctnt/iproto/requests/update.pyx":51
  *         if isinstance(operation, tuple):
  *             op_len = cpython.tuple.PyTuple_GET_SIZE(operation)
  *         elif isinstance(operation, list):             # <<<<<<<<<<<<<<
  *             op_len = cpython.list.PyList_GET_SIZE(operation)
  *         else:
  */
     __pyx_t_1 = PyList_Check(__pyx_v_operation); 
     if (likely(__pyx_t_1)) {
 
-      /* "asynctnt/iproto/requests/update.pyx":46
+      /* "asynctnt/iproto/requests/update.pyx":52
  *             op_len = cpython.tuple.PyTuple_GET_SIZE(operation)
  *         elif isinstance(operation, list):
  *             op_len = cpython.list.PyList_GET_SIZE(operation)             # <<<<<<<<<<<<<<
  *         else:
  *             raise TypeError(
  */
       __pyx_v_op_len = PyList_GET_SIZE(__pyx_v_operation);
 
-      /* "asynctnt/iproto/requests/update.pyx":45
+      /* "asynctnt/iproto/requests/update.pyx":51
  *         if isinstance(operation, tuple):
  *             op_len = cpython.tuple.PyTuple_GET_SIZE(operation)
  *         elif isinstance(operation, list):             # <<<<<<<<<<<<<<
  *             op_len = cpython.list.PyList_GET_SIZE(operation)
  *         else:
  */
       goto __pyx_L7;
     }
 
-    /* "asynctnt/iproto/requests/update.pyx":48
+    /* "asynctnt/iproto/requests/update.pyx":54
  *             op_len = cpython.list.PyList_GET_SIZE(operation)
  *         else:
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 'Single operation must be a tuple or list')
  *         if op_len < 3:
  */
     /*else*/ {
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 48, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 54, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(4, 48, __pyx_L1_error)
+      __PYX_ERR(4, 54, __pyx_L1_error)
     }
     __pyx_L7:;
 
-    /* "asynctnt/iproto/requests/update.pyx":50
+    /* "asynctnt/iproto/requests/update.pyx":56
  *             raise TypeError(
  *                 'Single operation must be a tuple or list')
  *         if op_len < 3:             # <<<<<<<<<<<<<<
  *             raise IndexError(
  *                 'Operation length must be at least 3')
  */
     __pyx_t_1 = (__pyx_v_op_len < 3);
     if (unlikely(__pyx_t_1)) {
 
-      /* "asynctnt/iproto/requests/update.pyx":51
+      /* "asynctnt/iproto/requests/update.pyx":57
  *                 'Single operation must be a tuple or list')
  *         if op_len < 3:
  *             raise IndexError(             # <<<<<<<<<<<<<<
  *                 'Operation length must be at least 3')
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 51, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 57, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(4, 51, __pyx_L1_error)
+      __PYX_ERR(4, 57, __pyx_L1_error)
 
-      /* "asynctnt/iproto/requests/update.pyx":50
+      /* "asynctnt/iproto/requests/update.pyx":56
  *             raise TypeError(
  *                 'Single operation must be a tuple or list')
  *         if op_len < 3:             # <<<<<<<<<<<<<<
  *             raise IndexError(
  *                 'Operation length must be at least 3')
  */
     }
 
-    /* "asynctnt/iproto/requests/update.pyx":54
+    /* "asynctnt/iproto/requests/update.pyx":60
  *                 'Operation length must be at least 3')
  * 
  *         op_type_str = operation[0]             # <<<<<<<<<<<<<<
  *         if isinstance(op_type_str, str):
  *             str_temp = encode_unicode_string(op_type_str, buffer._encoding)
  */
-    __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_operation, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 54, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_operation, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_XDECREF_SET(__pyx_v_op_type_str, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "asynctnt/iproto/requests/update.pyx":55
+    /* "asynctnt/iproto/requests/update.pyx":61
  * 
  *         op_type_str = operation[0]
  *         if isinstance(op_type_str, str):             # <<<<<<<<<<<<<<
  *             str_temp = encode_unicode_string(op_type_str, buffer._encoding)
  *         elif isinstance(op_type_str, bytes):
  */
     __pyx_t_1 = PyUnicode_Check(__pyx_v_op_type_str); 
     if (__pyx_t_1) {
 
-      /* "asynctnt/iproto/requests/update.pyx":56
+      /* "asynctnt/iproto/requests/update.pyx":62
  *         op_type_str = operation[0]
  *         if isinstance(op_type_str, str):
  *             str_temp = encode_unicode_string(op_type_str, buffer._encoding)             # <<<<<<<<<<<<<<
  *         elif isinstance(op_type_str, bytes):
  *             str_temp = <bytes> op_type_str
  */
       __pyx_t_5 = __pyx_v_buffer->_encoding;
       __Pyx_INCREF(__pyx_t_5);
-      __pyx_t_6 = __pyx_f_8asynctnt_6iproto_8protocol_encode_unicode_string(__pyx_v_op_type_str, ((PyObject*)__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 56, __pyx_L1_error)
+      __pyx_t_6 = __pyx_f_8asynctnt_6iproto_8protocol_encode_unicode_string(__pyx_v_op_type_str, ((PyObject*)__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 62, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF_SET(__pyx_v_str_temp, ((PyObject*)__pyx_t_6));
       __pyx_t_6 = 0;
 
-      /* "asynctnt/iproto/requests/update.pyx":55
+      /* "asynctnt/iproto/requests/update.pyx":61
  * 
  *         op_type_str = operation[0]
  *         if isinstance(op_type_str, str):             # <<<<<<<<<<<<<<
  *             str_temp = encode_unicode_string(op_type_str, buffer._encoding)
  *         elif isinstance(op_type_str, bytes):
  */
       goto __pyx_L9;
     }
 
-    /* "asynctnt/iproto/requests/update.pyx":57
+    /* "asynctnt/iproto/requests/update.pyx":63
  *         if isinstance(op_type_str, str):
  *             str_temp = encode_unicode_string(op_type_str, buffer._encoding)
  *         elif isinstance(op_type_str, bytes):             # <<<<<<<<<<<<<<
  *             str_temp = <bytes> op_type_str
  *         else:
  */
     __pyx_t_1 = PyBytes_Check(__pyx_v_op_type_str); 
     if (likely(__pyx_t_1)) {
 
-      /* "asynctnt/iproto/requests/update.pyx":58
+      /* "asynctnt/iproto/requests/update.pyx":64
  *             str_temp = encode_unicode_string(op_type_str, buffer._encoding)
  *         elif isinstance(op_type_str, bytes):
  *             str_temp = <bytes> op_type_str             # <<<<<<<<<<<<<<
  *         else:
  *             raise TypeError(
  */
       __pyx_t_6 = __pyx_v_op_type_str;
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_str_temp, ((PyObject*)__pyx_t_6));
       __pyx_t_6 = 0;
 
-      /* "asynctnt/iproto/requests/update.pyx":57
+      /* "asynctnt/iproto/requests/update.pyx":63
  *         if isinstance(op_type_str, str):
  *             str_temp = encode_unicode_string(op_type_str, buffer._encoding)
  *         elif isinstance(op_type_str, bytes):             # <<<<<<<<<<<<<<
  *             str_temp = <bytes> op_type_str
  *         else:
  */
       goto __pyx_L9;
     }
 
-    /* "asynctnt/iproto/requests/update.pyx":60
+    /* "asynctnt/iproto/requests/update.pyx":66
  *             str_temp = <bytes> op_type_str
  *         else:
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 'Operation type must of a str or bytes type')
  * 
  */
     /*else*/ {
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 60, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 66, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(4, 60, __pyx_L1_error)
+      __PYX_ERR(4, 66, __pyx_L1_error)
     }
     __pyx_L9:;
 
-    /* "asynctnt/iproto/requests/update.pyx":63
+    /* "asynctnt/iproto/requests/update.pyx":69
  *                 'Operation type must of a str or bytes type')
  * 
+ *         cpython.bytes.PyBytes_AsStringAndSize(str_temp, &op_str_c,             # <<<<<<<<<<<<<<
+ *                                               &op_str_len)
+ * 
+ */
+    __pyx_t_7 = PyBytes_AsStringAndSize(__pyx_v_str_temp, (&__pyx_v_op_str_c), ((Py_ssize_t *)(&__pyx_v_op_str_len))); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(4, 69, __pyx_L1_error)
+
+    /* "asynctnt/iproto/requests/update.pyx":72
+ *                                               &op_str_len)
+ * 
  *         field_no_obj = operation[1]             # <<<<<<<<<<<<<<
  *         if isinstance(field_no_obj, int):
  *             field_no = <int> field_no_obj
  */
-    __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_operation, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 63, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_operation, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_XDECREF_SET(__pyx_v_field_no_obj, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "asynctnt/iproto/requests/update.pyx":64
+    /* "asynctnt/iproto/requests/update.pyx":73
  * 
  *         field_no_obj = operation[1]
  *         if isinstance(field_no_obj, int):             # <<<<<<<<<<<<<<
  *             field_no = <int> field_no_obj
  *         elif isinstance(field_no_obj, str):
  */
     __pyx_t_1 = PyInt_Check(__pyx_v_field_no_obj); 
     if (__pyx_t_1) {
 
-      /* "asynctnt/iproto/requests/update.pyx":65
+      /* "asynctnt/iproto/requests/update.pyx":74
  *         field_no_obj = operation[1]
  *         if isinstance(field_no_obj, int):
  *             field_no = <int> field_no_obj             # <<<<<<<<<<<<<<
  *         elif isinstance(field_no_obj, str):
  *             if space.metadata is not None:
  */
-      __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_field_no_obj); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(4, 65, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_field_no_obj); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(4, 74, __pyx_L1_error)
       __pyx_v_field_no = ((int)__pyx_t_7);
 
-      /* "asynctnt/iproto/requests/update.pyx":64
+      /* "asynctnt/iproto/requests/update.pyx":73
  * 
  *         field_no_obj = operation[1]
  *         if isinstance(field_no_obj, int):             # <<<<<<<<<<<<<<
  *             field_no = <int> field_no_obj
  *         elif isinstance(field_no_obj, str):
  */
       goto __pyx_L10;
     }
 
-    /* "asynctnt/iproto/requests/update.pyx":66
+    /* "asynctnt/iproto/requests/update.pyx":75
  *         if isinstance(field_no_obj, int):
  *             field_no = <int> field_no_obj
  *         elif isinstance(field_no_obj, str):             # <<<<<<<<<<<<<<
  *             if space.metadata is not None:
- *                 field_no = <int> space.metadata.id_by_name(field_no_obj)
+ *                 field_no = <int> space.metadata.id_by_name_safe(field_no_obj)
  */
     __pyx_t_1 = PyUnicode_Check(__pyx_v_field_no_obj); 
     if (likely(__pyx_t_1)) {
 
-      /* "asynctnt/iproto/requests/update.pyx":67
+      /* "asynctnt/iproto/requests/update.pyx":76
  *             field_no = <int> field_no_obj
  *         elif isinstance(field_no_obj, str):
  *             if space.metadata is not None:             # <<<<<<<<<<<<<<
- *                 field_no = <int> space.metadata.id_by_name(field_no_obj)
- *             else:
+ *                 field_no = <int> space.metadata.id_by_name_safe(field_no_obj)
+ *                 if field_no == -1:
  */
       __pyx_t_1 = (((PyObject *)__pyx_v_space->metadata) != Py_None);
-      if (likely(__pyx_t_1)) {
+      if (__pyx_t_1) {
 
-        /* "asynctnt/iproto/requests/update.pyx":68
+        /* "asynctnt/iproto/requests/update.pyx":77
  *         elif isinstance(field_no_obj, str):
  *             if space.metadata is not None:
- *                 field_no = <int> space.metadata.id_by_name(field_no_obj)             # <<<<<<<<<<<<<<
- *             else:
- *                 raise TypeError(
+ *                 field_no = <int> space.metadata.id_by_name_safe(field_no_obj)             # <<<<<<<<<<<<<<
+ *                 if field_no == -1:
+ *                     field_encode_as_str = 1
  */
-        if (!(likely(PyUnicode_CheckExact(__pyx_v_field_no_obj))||((__pyx_v_field_no_obj) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_field_no_obj))) __PYX_ERR(4, 68, __pyx_L1_error)
-        __pyx_t_7 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_id_by_name(__pyx_v_space->metadata, ((PyObject*)__pyx_v_field_no_obj)); if (unlikely(PyErr_Occurred())) __PYX_ERR(4, 68, __pyx_L1_error)
+        if (!(likely(PyUnicode_CheckExact(__pyx_v_field_no_obj))||((__pyx_v_field_no_obj) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_field_no_obj))) __PYX_ERR(4, 77, __pyx_L1_error)
+        __pyx_t_7 = __pyx_f_8asynctnt_6iproto_8protocol_8Metadata_id_by_name_safe(__pyx_v_space->metadata, ((PyObject*)__pyx_v_field_no_obj)); if (unlikely(PyErr_Occurred())) __PYX_ERR(4, 77, __pyx_L1_error)
         __pyx_v_field_no = ((int)__pyx_t_7);
 
-        /* "asynctnt/iproto/requests/update.pyx":67
+        /* "asynctnt/iproto/requests/update.pyx":78
+ *             if space.metadata is not None:
+ *                 field_no = <int> space.metadata.id_by_name_safe(field_no_obj)
+ *                 if field_no == -1:             # <<<<<<<<<<<<<<
+ *                     field_encode_as_str = 1
+ *             else:
+ */
+        __pyx_t_1 = (__pyx_v_field_no == -1LL);
+        if (__pyx_t_1) {
+
+          /* "asynctnt/iproto/requests/update.pyx":79
+ *                 field_no = <int> space.metadata.id_by_name_safe(field_no_obj)
+ *                 if field_no == -1:
+ *                     field_encode_as_str = 1             # <<<<<<<<<<<<<<
+ *             else:
+ *                 field_encode_as_str = 1
+ */
+          __pyx_v_field_encode_as_str = 1;
+
+          /* "asynctnt/iproto/requests/update.pyx":78
+ *             if space.metadata is not None:
+ *                 field_no = <int> space.metadata.id_by_name_safe(field_no_obj)
+ *                 if field_no == -1:             # <<<<<<<<<<<<<<
+ *                     field_encode_as_str = 1
+ *             else:
+ */
+        }
+
+        /* "asynctnt/iproto/requests/update.pyx":76
  *             field_no = <int> field_no_obj
  *         elif isinstance(field_no_obj, str):
  *             if space.metadata is not None:             # <<<<<<<<<<<<<<
- *                 field_no = <int> space.metadata.id_by_name(field_no_obj)
- *             else:
+ *                 field_no = <int> space.metadata.id_by_name_safe(field_no_obj)
+ *                 if field_no == -1:
  */
         goto __pyx_L11;
       }
 
-      /* "asynctnt/iproto/requests/update.pyx":70
- *                 field_no = <int> space.metadata.id_by_name(field_no_obj)
+      /* "asynctnt/iproto/requests/update.pyx":81
+ *                     field_encode_as_str = 1
  *             else:
- *                 raise TypeError(             # <<<<<<<<<<<<<<
- *                     'Operation field_no must be int as there is '
- *                     'no format declaration in space {}'.format(space.sid))
+ *                 field_encode_as_str = 1             # <<<<<<<<<<<<<<
+ * 
+ *             if field_encode_as_str:
  */
       /*else*/ {
+        __pyx_v_field_encode_as_str = 1;
+      }
+      __pyx_L11:;
 
-        /* "asynctnt/iproto/requests/update.pyx":72
- *                 raise TypeError(
- *                     'Operation field_no must be int as there is '
- *                     'no format declaration in space {}'.format(space.sid))             # <<<<<<<<<<<<<<
- *         else:
- *             raise TypeError(
+      /* "asynctnt/iproto/requests/update.pyx":83
+ *                 field_encode_as_str = 1
+ * 
+ *             if field_encode_as_str:             # <<<<<<<<<<<<<<
+ *                 str_temp = encode_unicode_string(field_no_obj, buffer._encoding)
+ *                 cpython.bytes.PyBytes_AsStringAndSize(str_temp, &field_str_c, &field_str_len)
  */
-        __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Operation_field_no_must_be_int_a, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 72, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_space->sid); if (unlikely(!__pyx_t_8)) __PYX_ERR(4, 72, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_9 = NULL;
-        __pyx_t_7 = 0;
-        #if CYTHON_UNPACK_METHODS
-        if (likely(PyMethod_Check(__pyx_t_5))) {
-          __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
-          if (likely(__pyx_t_9)) {
-            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-            __Pyx_INCREF(__pyx_t_9);
-            __Pyx_INCREF(function);
-            __Pyx_DECREF_SET(__pyx_t_5, function);
-            __pyx_t_7 = 1;
-          }
-        }
-        #endif
-        {
-          PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_8};
-          __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
-          __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 72, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_6);
-          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        }
+      if (__pyx_v_field_encode_as_str) {
 
-        /* "asynctnt/iproto/requests/update.pyx":70
- *                 field_no = <int> space.metadata.id_by_name(field_no_obj)
- *             else:
- *                 raise TypeError(             # <<<<<<<<<<<<<<
- *                     'Operation field_no must be int as there is '
- *                     'no format declaration in space {}'.format(space.sid))
+        /* "asynctnt/iproto/requests/update.pyx":84
+ * 
+ *             if field_encode_as_str:
+ *                 str_temp = encode_unicode_string(field_no_obj, buffer._encoding)             # <<<<<<<<<<<<<<
+ *                 cpython.bytes.PyBytes_AsStringAndSize(str_temp, &field_str_c, &field_str_len)
+ *         else:
  */
-        __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 70, __pyx_L1_error)
+        __pyx_t_6 = __pyx_v_buffer->_encoding;
+        __Pyx_INCREF(__pyx_t_6);
+        __pyx_t_5 = __pyx_f_8asynctnt_6iproto_8protocol_encode_unicode_string(__pyx_v_field_no_obj, ((PyObject*)__pyx_t_6)); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 84, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __Pyx_Raise(__pyx_t_5, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __PYX_ERR(4, 70, __pyx_L1_error)
+        __Pyx_DECREF_SET(__pyx_v_str_temp, ((PyObject*)__pyx_t_5));
+        __pyx_t_5 = 0;
+
+        /* "asynctnt/iproto/requests/update.pyx":85
+ *             if field_encode_as_str:
+ *                 str_temp = encode_unicode_string(field_no_obj, buffer._encoding)
+ *                 cpython.bytes.PyBytes_AsStringAndSize(str_temp, &field_str_c, &field_str_len)             # <<<<<<<<<<<<<<
+ *         else:
+ *             raise TypeError(
+ */
+        __pyx_t_7 = PyBytes_AsStringAndSize(__pyx_v_str_temp, (&__pyx_v_field_str_c), ((Py_ssize_t *)(&__pyx_v_field_str_len))); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(4, 85, __pyx_L1_error)
+
+        /* "asynctnt/iproto/requests/update.pyx":83
+ *                 field_encode_as_str = 1
+ * 
+ *             if field_encode_as_str:             # <<<<<<<<<<<<<<
+ *                 str_temp = encode_unicode_string(field_no_obj, buffer._encoding)
+ *                 cpython.bytes.PyBytes_AsStringAndSize(str_temp, &field_str_c, &field_str_len)
+ */
       }
-      __pyx_L11:;
 
-      /* "asynctnt/iproto/requests/update.pyx":66
+      /* "asynctnt/iproto/requests/update.pyx":75
  *         if isinstance(field_no_obj, int):
  *             field_no = <int> field_no_obj
  *         elif isinstance(field_no_obj, str):             # <<<<<<<<<<<<<<
  *             if space.metadata is not None:
- *                 field_no = <int> space.metadata.id_by_name(field_no_obj)
+ *                 field_no = <int> space.metadata.id_by_name_safe(field_no_obj)
  */
       goto __pyx_L10;
     }
 
-    /* "asynctnt/iproto/requests/update.pyx":74
- *                     'no format declaration in space {}'.format(space.sid))
+    /* "asynctnt/iproto/requests/update.pyx":87
+ *                 cpython.bytes.PyBytes_AsStringAndSize(str_temp, &field_str_c, &field_str_len)
  *         else:
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 'Operation field_no must be of either int or str type')
  * 
  */
     /*else*/ {
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 74, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 87, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(4, 74, __pyx_L1_error)
+      __PYX_ERR(4, 87, __pyx_L1_error)
     }
     __pyx_L10:;
 
-    /* "asynctnt/iproto/requests/update.pyx":77
+    /* "asynctnt/iproto/requests/update.pyx":90
  *                 'Operation field_no must be of either int or str type')
  * 
- *         cpython.bytes.PyBytes_AsStringAndSize(str_temp, &op_str_c,             # <<<<<<<<<<<<<<
- *                                               &op_str_len)
- *         op = <char> 0
- */
-    __pyx_t_7 = PyBytes_AsStringAndSize(__pyx_v_str_temp, (&__pyx_v_op_str_c), ((Py_ssize_t *)(&__pyx_v_op_str_len))); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(4, 77, __pyx_L1_error)
-
-    /* "asynctnt/iproto/requests/update.pyx":79
- *         cpython.bytes.PyBytes_AsStringAndSize(str_temp, &op_str_c,
- *                                               &op_str_len)
  *         op = <char> 0             # <<<<<<<<<<<<<<
  *         if op_str_len == 1:
  *             op = op_str_c[0]
  */
     __pyx_v_op = ((char)0);
 
-    /* "asynctnt/iproto/requests/update.pyx":80
- *                                               &op_str_len)
+    /* "asynctnt/iproto/requests/update.pyx":91
+ * 
  *         op = <char> 0
  *         if op_str_len == 1:             # <<<<<<<<<<<<<<
  *             op = op_str_c[0]
  * 
  */
     __pyx_t_1 = (__pyx_v_op_str_len == 1);
     if (__pyx_t_1) {
 
-      /* "asynctnt/iproto/requests/update.pyx":81
+      /* "asynctnt/iproto/requests/update.pyx":92
  *         op = <char> 0
  *         if op_str_len == 1:
  *             op = op_str_c[0]             # <<<<<<<<<<<<<<
  * 
  *         if op == tarantool.IPROTO_OP_ADD \
  */
       __pyx_v_op = (__pyx_v_op_str_c[0]);
 
-      /* "asynctnt/iproto/requests/update.pyx":80
- *                                               &op_str_len)
+      /* "asynctnt/iproto/requests/update.pyx":91
+ * 
  *         op = <char> 0
  *         if op_str_len == 1:             # <<<<<<<<<<<<<<
  *             op = op_str_c[0]
  * 
  */
     }
 
-    /* "asynctnt/iproto/requests/update.pyx":83
+    /* "asynctnt/iproto/requests/update.pyx":94
  *             op = op_str_c[0]
  * 
  *         if op == tarantool.IPROTO_OP_ADD \             # <<<<<<<<<<<<<<
  *                 or op == tarantool.IPROTO_OP_SUB \
  *                 or op == tarantool.IPROTO_OP_AND \
  */
     switch (__pyx_v_op) {
       case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_ADD:
       case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_SUB:
 
-      /* "asynctnt/iproto/requests/update.pyx":84
+      /* "asynctnt/iproto/requests/update.pyx":95
  * 
  *         if op == tarantool.IPROTO_OP_ADD \
  *                 or op == tarantool.IPROTO_OP_SUB \             # <<<<<<<<<<<<<<
  *                 or op == tarantool.IPROTO_OP_AND \
  *                 or op == tarantool.IPROTO_OP_XOR \
  */
       case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_AND:
 
-      /* "asynctnt/iproto/requests/update.pyx":85
+      /* "asynctnt/iproto/requests/update.pyx":96
  *         if op == tarantool.IPROTO_OP_ADD \
  *                 or op == tarantool.IPROTO_OP_SUB \
  *                 or op == tarantool.IPROTO_OP_AND \             # <<<<<<<<<<<<<<
  *                 or op == tarantool.IPROTO_OP_XOR \
  *                 or op == tarantool.IPROTO_OP_OR \
  */
       case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_XOR:
 
-      /* "asynctnt/iproto/requests/update.pyx":86
+      /* "asynctnt/iproto/requests/update.pyx":97
  *                 or op == tarantool.IPROTO_OP_SUB \
  *                 or op == tarantool.IPROTO_OP_AND \
  *                 or op == tarantool.IPROTO_OP_XOR \             # <<<<<<<<<<<<<<
  *                 or op == tarantool.IPROTO_OP_OR \
- *                 or op == tarantool.IPROTO_OP_DELETE:
+ *                 or op == tarantool.IPROTO_OP_DELETE \
  */
       case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_OR:
 
-      /* "asynctnt/iproto/requests/update.pyx":87
+      /* "asynctnt/iproto/requests/update.pyx":98
  *                 or op == tarantool.IPROTO_OP_AND \
  *                 or op == tarantool.IPROTO_OP_XOR \
  *                 or op == tarantool.IPROTO_OP_OR \             # <<<<<<<<<<<<<<
- *                 or op == tarantool.IPROTO_OP_DELETE:
- *             op_argument = operation[2]
+ *                 or op == tarantool.IPROTO_OP_DELETE \
+ *                 or op == tarantool.IPROTO_OP_INSERT \
  */
       case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_DELETE:
 
-      /* "asynctnt/iproto/requests/update.pyx":89
+      /* "asynctnt/iproto/requests/update.pyx":99
+ *                 or op == tarantool.IPROTO_OP_XOR \
  *                 or op == tarantool.IPROTO_OP_OR \
- *                 or op == tarantool.IPROTO_OP_DELETE:
- *             op_argument = operation[2]             # <<<<<<<<<<<<<<
- *             if not isinstance(op_argument, int):
- *                 raise TypeError(
- */
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_operation, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 89, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_XDECREF_SET(__pyx_v_op_argument, __pyx_t_5);
-      __pyx_t_5 = 0;
-
-      /* "asynctnt/iproto/requests/update.pyx":90
- *                 or op == tarantool.IPROTO_OP_DELETE:
- *             op_argument = operation[2]
- *             if not isinstance(op_argument, int):             # <<<<<<<<<<<<<<
- *                 raise TypeError(
- *                     'int argument required for '
- */
-      __pyx_t_1 = PyInt_Check(__pyx_v_op_argument); 
-      __pyx_t_10 = (!__pyx_t_1);
-      if (unlikely(__pyx_t_10)) {
-
-        /* "asynctnt/iproto/requests/update.pyx":91
- *             op_argument = operation[2]
- *             if not isinstance(op_argument, int):
- *                 raise TypeError(             # <<<<<<<<<<<<<<
- *                     'int argument required for '
- *                     'Arithmetic and Delete operations'
+ *                 or op == tarantool.IPROTO_OP_DELETE \             # <<<<<<<<<<<<<<
+ *                 or op == tarantool.IPROTO_OP_INSERT \
+ *                 or op == tarantool.IPROTO_OP_ASSIGN:
  */
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 91, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_5);
-        __Pyx_Raise(__pyx_t_5, 0, 0, 0);
-        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-        __PYX_ERR(4, 91, __pyx_L1_error)
+      case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_INSERT:
 
-        /* "asynctnt/iproto/requests/update.pyx":90
- *                 or op == tarantool.IPROTO_OP_DELETE:
- *             op_argument = operation[2]
- *             if not isinstance(op_argument, int):             # <<<<<<<<<<<<<<
- *                 raise TypeError(
- *                     'int argument required for '
+      /* "asynctnt/iproto/requests/update.pyx":100
+ *                 or op == tarantool.IPROTO_OP_OR \
+ *                 or op == tarantool.IPROTO_OP_DELETE \
+ *                 or op == tarantool.IPROTO_OP_INSERT \             # <<<<<<<<<<<<<<
+ *                 or op == tarantool.IPROTO_OP_ASSIGN:
+ *             # mp_sizeof_array(3)
  */
-      }
+      case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_ASSIGN:
 
-      /* "asynctnt/iproto/requests/update.pyx":98
+      /* "asynctnt/iproto/requests/update.pyx":105
  *             # + mp_sizeof_str(1)
  *             # + mp_sizeof_uint(field_no)
  *             extra_length = 1 + 2 + mp_sizeof_uint(field_no)             # <<<<<<<<<<<<<<
  *             p = begin = buffer._ensure_allocated(p, extra_length)
  * 
  */
       __pyx_v_extra_length = (0x3 + mp_sizeof_uint(__pyx_v_field_no));
 
-      /* "asynctnt/iproto/requests/update.pyx":99
+      /* "asynctnt/iproto/requests/update.pyx":106
  *             # + mp_sizeof_uint(field_no)
  *             extra_length = 1 + 2 + mp_sizeof_uint(field_no)
  *             p = begin = buffer._ensure_allocated(p, extra_length)             # <<<<<<<<<<<<<<
  * 
  *             p = mp_encode_array(p, 3)
  */
-      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer__ensure_allocated(__pyx_v_buffer, __pyx_v_p, __pyx_v_extra_length); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 99, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer__ensure_allocated(__pyx_v_buffer, __pyx_v_p, __pyx_v_extra_length); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 106, __pyx_L1_error)
       __pyx_v_p = __pyx_t_2;
       __pyx_v_begin = __pyx_t_2;
 
-      /* "asynctnt/iproto/requests/update.pyx":101
+      /* "asynctnt/iproto/requests/update.pyx":108
  *             p = begin = buffer._ensure_allocated(p, extra_length)
  * 
  *             p = mp_encode_array(p, 3)             # <<<<<<<<<<<<<<
  *             p = mp_encode_str(p, op_str_c, 1)
- *             p = mp_encode_uint(p, field_no)
+ *             if field_str_c == NULL:
  */
       __pyx_v_p = mp_encode_array(__pyx_v_p, 3);
 
-      /* "asynctnt/iproto/requests/update.pyx":102
+      /* "asynctnt/iproto/requests/update.pyx":109
  * 
  *             p = mp_encode_array(p, 3)
  *             p = mp_encode_str(p, op_str_c, 1)             # <<<<<<<<<<<<<<
- *             p = mp_encode_uint(p, field_no)
- *             buffer._length += (p - begin)
+ *             if field_str_c == NULL:
+ *                 p = mp_encode_uint(p, field_no)
  */
       __pyx_v_p = mp_encode_str(__pyx_v_p, __pyx_v_op_str_c, 1);
 
-      /* "asynctnt/iproto/requests/update.pyx":103
+      /* "asynctnt/iproto/requests/update.pyx":110
  *             p = mp_encode_array(p, 3)
  *             p = mp_encode_str(p, op_str_c, 1)
- *             p = mp_encode_uint(p, field_no)             # <<<<<<<<<<<<<<
- *             buffer._length += (p - begin)
- *             p = buffer.mp_encode_obj(p, op_argument)
+ *             if field_str_c == NULL:             # <<<<<<<<<<<<<<
+ *                 p = mp_encode_uint(p, field_no)
+ *             else:
  */
-      __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_v_field_no);
+      __pyx_t_1 = (__pyx_v_field_str_c == NULL);
+      if (__pyx_t_1) {
 
-      /* "asynctnt/iproto/requests/update.pyx":104
+        /* "asynctnt/iproto/requests/update.pyx":111
  *             p = mp_encode_str(p, op_str_c, 1)
- *             p = mp_encode_uint(p, field_no)
- *             buffer._length += (p - begin)             # <<<<<<<<<<<<<<
- *             p = buffer.mp_encode_obj(p, op_argument)
- *         elif op == tarantool.IPROTO_OP_INSERT \
+ *             if field_str_c == NULL:
+ *                 p = mp_encode_uint(p, field_no)             # <<<<<<<<<<<<<<
+ *             else:
+ *                 p = mp_encode_str(p, field_str_c, field_str_len)
  */
-      __pyx_v_buffer->_length = (__pyx_v_buffer->_length + (__pyx_v_p - __pyx_v_begin));
+        __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_v_field_no);
 
-      /* "asynctnt/iproto/requests/update.pyx":105
- *             p = mp_encode_uint(p, field_no)
- *             buffer._length += (p - begin)
- *             p = buffer.mp_encode_obj(p, op_argument)             # <<<<<<<<<<<<<<
- *         elif op == tarantool.IPROTO_OP_INSERT \
- *                 or op == tarantool.IPROTO_OP_ASSIGN:
+        /* "asynctnt/iproto/requests/update.pyx":110
+ *             p = mp_encode_array(p, 3)
+ *             p = mp_encode_str(p, op_str_c, 1)
+ *             if field_str_c == NULL:             # <<<<<<<<<<<<<<
+ *                 p = mp_encode_uint(p, field_no)
+ *             else:
  */
-      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_obj(__pyx_v_buffer, __pyx_v_p, __pyx_v_op_argument); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 105, __pyx_L1_error)
-      __pyx_v_p = __pyx_t_2;
+        goto __pyx_L15;
+      }
 
-      /* "asynctnt/iproto/requests/update.pyx":83
- *             op = op_str_c[0]
+      /* "asynctnt/iproto/requests/update.pyx":113
+ *                 p = mp_encode_uint(p, field_no)
+ *             else:
+ *                 p = mp_encode_str(p, field_str_c, field_str_len)             # <<<<<<<<<<<<<<
  * 
- *         if op == tarantool.IPROTO_OP_ADD \             # <<<<<<<<<<<<<<
- *                 or op == tarantool.IPROTO_OP_SUB \
- *                 or op == tarantool.IPROTO_OP_AND \
+ *             buffer._length += (p - begin)
  */
-      break;
-      case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_INSERT:
+      /*else*/ {
+        __pyx_v_p = mp_encode_str(__pyx_v_p, __pyx_v_field_str_c, __pyx_v_field_str_len);
+      }
+      __pyx_L15:;
 
-      /* "asynctnt/iproto/requests/update.pyx":106
- *             buffer._length += (p - begin)
- *             p = buffer.mp_encode_obj(p, op_argument)
- *         elif op == tarantool.IPROTO_OP_INSERT \             # <<<<<<<<<<<<<<
- *                 or op == tarantool.IPROTO_OP_ASSIGN:
+      /* "asynctnt/iproto/requests/update.pyx":115
+ *                 p = mp_encode_str(p, field_str_c, field_str_len)
+ * 
+ *             buffer._length += (p - begin)             # <<<<<<<<<<<<<<
+ * 
  *             op_argument = operation[2]
  */
-      case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_ASSIGN:
+      __pyx_v_buffer->_length = (__pyx_v_buffer->_length + (__pyx_v_p - __pyx_v_begin));
 
-      /* "asynctnt/iproto/requests/update.pyx":108
- *         elif op == tarantool.IPROTO_OP_INSERT \
- *                 or op == tarantool.IPROTO_OP_ASSIGN:
+      /* "asynctnt/iproto/requests/update.pyx":117
+ *             buffer._length += (p - begin)
+ * 
  *             op_argument = operation[2]             # <<<<<<<<<<<<<<
+ *             p = buffer.mp_encode_obj(p, op_argument)
  * 
- *             # mp_sizeof_array(3)
  */
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_operation, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 108, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_operation, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 117, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_XDECREF_SET(__pyx_v_op_argument, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "asynctnt/iproto/requests/update.pyx":113
- *             # + mp_sizeof_str(1)
- *             # + mp_sizeof_uint(field_no)
- *             extra_length = 1 + 2 + mp_sizeof_uint(field_no)             # <<<<<<<<<<<<<<
- *             p = begin = buffer._ensure_allocated(p, extra_length)
- * 
- */
-      __pyx_v_extra_length = (0x3 + mp_sizeof_uint(__pyx_v_field_no));
-
-      /* "asynctnt/iproto/requests/update.pyx":114
- *             # + mp_sizeof_uint(field_no)
- *             extra_length = 1 + 2 + mp_sizeof_uint(field_no)
- *             p = begin = buffer._ensure_allocated(p, extra_length)             # <<<<<<<<<<<<<<
- * 
- *             p = mp_encode_array(p, 3)
- */
-      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer__ensure_allocated(__pyx_v_buffer, __pyx_v_p, __pyx_v_extra_length); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 114, __pyx_L1_error)
-      __pyx_v_p = __pyx_t_2;
-      __pyx_v_begin = __pyx_t_2;
-
-      /* "asynctnt/iproto/requests/update.pyx":116
- *             p = begin = buffer._ensure_allocated(p, extra_length)
- * 
- *             p = mp_encode_array(p, 3)             # <<<<<<<<<<<<<<
- *             p = mp_encode_str(p, op_str_c, 1)
- *             p = mp_encode_uint(p, field_no)
- */
-      __pyx_v_p = mp_encode_array(__pyx_v_p, 3);
-
-      /* "asynctnt/iproto/requests/update.pyx":117
- * 
- *             p = mp_encode_array(p, 3)
- *             p = mp_encode_str(p, op_str_c, 1)             # <<<<<<<<<<<<<<
- *             p = mp_encode_uint(p, field_no)
- *             buffer._length += (p - begin)
- */
-      __pyx_v_p = mp_encode_str(__pyx_v_p, __pyx_v_op_str_c, 1);
-
       /* "asynctnt/iproto/requests/update.pyx":118
- *             p = mp_encode_array(p, 3)
- *             p = mp_encode_str(p, op_str_c, 1)
- *             p = mp_encode_uint(p, field_no)             # <<<<<<<<<<<<<<
- *             buffer._length += (p - begin)
- *             p = buffer.mp_encode_obj(p, op_argument)
- */
-      __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_v_field_no);
-
-      /* "asynctnt/iproto/requests/update.pyx":119
- *             p = mp_encode_str(p, op_str_c, 1)
- *             p = mp_encode_uint(p, field_no)
- *             buffer._length += (p - begin)             # <<<<<<<<<<<<<<
- *             p = buffer.mp_encode_obj(p, op_argument)
  * 
- */
-      __pyx_v_buffer->_length = (__pyx_v_buffer->_length + (__pyx_v_p - __pyx_v_begin));
-
-      /* "asynctnt/iproto/requests/update.pyx":120
- *             p = mp_encode_uint(p, field_no)
- *             buffer._length += (p - begin)
+ *             op_argument = operation[2]
  *             p = buffer.mp_encode_obj(p, op_argument)             # <<<<<<<<<<<<<<
  * 
  *         elif op == tarantool.IPROTO_OP_SPLICE:
  */
-      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_obj(__pyx_v_buffer, __pyx_v_p, __pyx_v_op_argument); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 120, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_obj(__pyx_v_buffer, __pyx_v_p, __pyx_v_op_argument); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 118, __pyx_L1_error)
       __pyx_v_p = __pyx_t_2;
 
-      /* "asynctnt/iproto/requests/update.pyx":106
- *             buffer._length += (p - begin)
- *             p = buffer.mp_encode_obj(p, op_argument)
- *         elif op == tarantool.IPROTO_OP_INSERT \             # <<<<<<<<<<<<<<
- *                 or op == tarantool.IPROTO_OP_ASSIGN:
- *             op_argument = operation[2]
+      /* "asynctnt/iproto/requests/update.pyx":94
+ *             op = op_str_c[0]
+ * 
+ *         if op == tarantool.IPROTO_OP_ADD \             # <<<<<<<<<<<<<<
+ *                 or op == tarantool.IPROTO_OP_SUB \
+ *                 or op == tarantool.IPROTO_OP_AND \
  */
       break;
       case __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OP_SPLICE:
 
-      /* "asynctnt/iproto/requests/update.pyx":123
+      /* "asynctnt/iproto/requests/update.pyx":121
  * 
  *         elif op == tarantool.IPROTO_OP_SPLICE:
  *             if op_len < 5:             # <<<<<<<<<<<<<<
- *                 raise IndexError(
+ *                 raise ValueError(
  *                     'Splice operation must have length of 5, '
  */
-      __pyx_t_10 = (__pyx_v_op_len < 5);
-      if (unlikely(__pyx_t_10)) {
+      __pyx_t_1 = (__pyx_v_op_len < 5);
+      if (unlikely(__pyx_t_1)) {
 
-        /* "asynctnt/iproto/requests/update.pyx":126
- *                 raise IndexError(
+        /* "asynctnt/iproto/requests/update.pyx":124
+ *                 raise ValueError(
  *                     'Splice operation must have length of 5, '
  *                     'but got: {}'.format(op_len)             # <<<<<<<<<<<<<<
  *                 )
  * 
  */
-        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Splice_operation_must_have_lengt, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 126, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Splice_operation_must_have_lengt, __pyx_n_s_format); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 124, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_op_len); if (unlikely(!__pyx_t_8)) __PYX_ERR(4, 126, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyInt_From_uint32_t(__pyx_v_op_len); if (unlikely(!__pyx_t_8)) __PYX_ERR(4, 124, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __pyx_t_9 = NULL;
         __pyx_t_7 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_6))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_6);
           if (likely(__pyx_t_9)) {
@@ -33424,266 +33466,298 @@
         }
         #endif
         {
           PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_8};
           __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
           __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 126, __pyx_L1_error)
+          if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 124, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_5);
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         }
 
-        /* "asynctnt/iproto/requests/update.pyx":124
+        /* "asynctnt/iproto/requests/update.pyx":122
  *         elif op == tarantool.IPROTO_OP_SPLICE:
  *             if op_len < 5:
- *                 raise IndexError(             # <<<<<<<<<<<<<<
+ *                 raise ValueError(             # <<<<<<<<<<<<<<
  *                     'Splice operation must have length of 5, '
  *                     'but got: {}'.format(op_len)
  */
-        __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 124, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 122, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_Raise(__pyx_t_6, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __PYX_ERR(4, 124, __pyx_L1_error)
+        __PYX_ERR(4, 122, __pyx_L1_error)
 
-        /* "asynctnt/iproto/requests/update.pyx":123
+        /* "asynctnt/iproto/requests/update.pyx":121
  * 
  *         elif op == tarantool.IPROTO_OP_SPLICE:
  *             if op_len < 5:             # <<<<<<<<<<<<<<
- *                 raise IndexError(
+ *                 raise ValueError(
  *                     'Splice operation must have length of 5, '
  */
       }
 
-      /* "asynctnt/iproto/requests/update.pyx":129
+      /* "asynctnt/iproto/requests/update.pyx":127
  *                 )
  * 
  *             splice_position_obj = operation[2]             # <<<<<<<<<<<<<<
  *             splice_offset_obj = operation[3]
  *             op_argument = operation[4]
  */
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_operation, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 129, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_operation, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 127, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_splice_position_obj, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "asynctnt/iproto/requests/update.pyx":130
+      /* "asynctnt/iproto/requests/update.pyx":128
  * 
  *             splice_position_obj = operation[2]
  *             splice_offset_obj = operation[3]             # <<<<<<<<<<<<<<
  *             op_argument = operation[4]
  *             if not isinstance(splice_position_obj, int):
  */
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_operation, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 130, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_operation, 3, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 128, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_splice_offset_obj, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "asynctnt/iproto/requests/update.pyx":131
+      /* "asynctnt/iproto/requests/update.pyx":129
  *             splice_position_obj = operation[2]
  *             splice_offset_obj = operation[3]
  *             op_argument = operation[4]             # <<<<<<<<<<<<<<
  *             if not isinstance(splice_position_obj, int):
  *                 raise TypeError('Splice position must be int')
  */
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_operation, 4, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 131, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_operation, 4, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 129, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_op_argument, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "asynctnt/iproto/requests/update.pyx":132
+      /* "asynctnt/iproto/requests/update.pyx":130
  *             splice_offset_obj = operation[3]
  *             op_argument = operation[4]
  *             if not isinstance(splice_position_obj, int):             # <<<<<<<<<<<<<<
  *                 raise TypeError('Splice position must be int')
  *             if not isinstance(splice_offset_obj, int):
  */
-      __pyx_t_10 = PyInt_Check(__pyx_v_splice_position_obj); 
-      __pyx_t_1 = (!__pyx_t_10);
-      if (unlikely(__pyx_t_1)) {
+      __pyx_t_1 = PyInt_Check(__pyx_v_splice_position_obj); 
+      __pyx_t_10 = (!__pyx_t_1);
+      if (unlikely(__pyx_t_10)) {
 
-        /* "asynctnt/iproto/requests/update.pyx":133
+        /* "asynctnt/iproto/requests/update.pyx":131
  *             op_argument = operation[4]
  *             if not isinstance(splice_position_obj, int):
  *                 raise TypeError('Splice position must be int')             # <<<<<<<<<<<<<<
  *             if not isinstance(splice_offset_obj, int):
  *                 raise TypeError('Splice offset must be int')
  */
-        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 133, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 131, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_Raise(__pyx_t_6, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __PYX_ERR(4, 133, __pyx_L1_error)
+        __PYX_ERR(4, 131, __pyx_L1_error)
 
-        /* "asynctnt/iproto/requests/update.pyx":132
+        /* "asynctnt/iproto/requests/update.pyx":130
  *             splice_offset_obj = operation[3]
  *             op_argument = operation[4]
  *             if not isinstance(splice_position_obj, int):             # <<<<<<<<<<<<<<
  *                 raise TypeError('Splice position must be int')
  *             if not isinstance(splice_offset_obj, int):
  */
       }
 
-      /* "asynctnt/iproto/requests/update.pyx":134
+      /* "asynctnt/iproto/requests/update.pyx":132
  *             if not isinstance(splice_position_obj, int):
  *                 raise TypeError('Splice position must be int')
  *             if not isinstance(splice_offset_obj, int):             # <<<<<<<<<<<<<<
  *                 raise TypeError('Splice offset must be int')
  * 
  */
-      __pyx_t_1 = PyInt_Check(__pyx_v_splice_offset_obj); 
-      __pyx_t_10 = (!__pyx_t_1);
-      if (unlikely(__pyx_t_10)) {
+      __pyx_t_10 = PyInt_Check(__pyx_v_splice_offset_obj); 
+      __pyx_t_1 = (!__pyx_t_10);
+      if (unlikely(__pyx_t_1)) {
 
-        /* "asynctnt/iproto/requests/update.pyx":135
+        /* "asynctnt/iproto/requests/update.pyx":133
  *                 raise TypeError('Splice position must be int')
  *             if not isinstance(splice_offset_obj, int):
  *                 raise TypeError('Splice offset must be int')             # <<<<<<<<<<<<<<
  * 
  *             splice_position = <uint32_t> splice_position_obj
  */
-        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 135, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 133, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_Raise(__pyx_t_6, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        __PYX_ERR(4, 135, __pyx_L1_error)
+        __PYX_ERR(4, 133, __pyx_L1_error)
 
-        /* "asynctnt/iproto/requests/update.pyx":134
+        /* "asynctnt/iproto/requests/update.pyx":132
  *             if not isinstance(splice_position_obj, int):
  *                 raise TypeError('Splice position must be int')
  *             if not isinstance(splice_offset_obj, int):             # <<<<<<<<<<<<<<
  *                 raise TypeError('Splice offset must be int')
  * 
  */
       }
 
-      /* "asynctnt/iproto/requests/update.pyx":137
+      /* "asynctnt/iproto/requests/update.pyx":135
  *                 raise TypeError('Splice offset must be int')
  * 
  *             splice_position = <uint32_t> splice_position_obj             # <<<<<<<<<<<<<<
  *             splice_offset = <uint32_t> splice_offset_obj
  * 
  */
-      __pyx_t_11 = __Pyx_PyInt_As_uint32_t(__pyx_v_splice_position_obj); if (unlikely((__pyx_t_11 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(4, 137, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_As_uint32_t(__pyx_v_splice_position_obj); if (unlikely((__pyx_t_11 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(4, 135, __pyx_L1_error)
       __pyx_v_splice_position = ((uint32_t)__pyx_t_11);
 
-      /* "asynctnt/iproto/requests/update.pyx":138
+      /* "asynctnt/iproto/requests/update.pyx":136
  * 
  *             splice_position = <uint32_t> splice_position_obj
  *             splice_offset = <uint32_t> splice_offset_obj             # <<<<<<<<<<<<<<
  * 
  *             # mp_sizeof_array(5) + mp_sizeof_str(1) + ...
  */
-      __pyx_t_11 = __Pyx_PyInt_As_uint32_t(__pyx_v_splice_offset_obj); if (unlikely((__pyx_t_11 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(4, 138, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_As_uint32_t(__pyx_v_splice_offset_obj); if (unlikely((__pyx_t_11 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(4, 136, __pyx_L1_error)
       __pyx_v_splice_offset = ((uint32_t)__pyx_t_11);
 
-      /* "asynctnt/iproto/requests/update.pyx":144
+      /* "asynctnt/iproto/requests/update.pyx":142
  *                            + mp_sizeof_uint(field_no) \
  *                            + mp_sizeof_uint(splice_position) \
  *                            + mp_sizeof_uint(splice_offset)             # <<<<<<<<<<<<<<
  *             p = begin = buffer._ensure_allocated(p, extra_length)
  * 
  */
       __pyx_v_extra_length = (((0x3 + mp_sizeof_uint(__pyx_v_field_no)) + mp_sizeof_uint(__pyx_v_splice_position)) + mp_sizeof_uint(__pyx_v_splice_offset));
 
-      /* "asynctnt/iproto/requests/update.pyx":145
+      /* "asynctnt/iproto/requests/update.pyx":143
  *                            + mp_sizeof_uint(splice_position) \
  *                            + mp_sizeof_uint(splice_offset)
  *             p = begin = buffer._ensure_allocated(p, extra_length)             # <<<<<<<<<<<<<<
  * 
  *             p = mp_encode_array(p, 5)
  */
-      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer__ensure_allocated(__pyx_v_buffer, __pyx_v_p, __pyx_v_extra_length); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 145, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer__ensure_allocated(__pyx_v_buffer, __pyx_v_p, __pyx_v_extra_length); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 143, __pyx_L1_error)
       __pyx_v_p = __pyx_t_2;
       __pyx_v_begin = __pyx_t_2;
 
-      /* "asynctnt/iproto/requests/update.pyx":147
+      /* "asynctnt/iproto/requests/update.pyx":145
  *             p = begin = buffer._ensure_allocated(p, extra_length)
  * 
  *             p = mp_encode_array(p, 5)             # <<<<<<<<<<<<<<
  *             p = mp_encode_str(p, op_str_c, 1)
- *             p = mp_encode_uint(p, field_no)
+ *             if field_str_c == NULL:
  */
       __pyx_v_p = mp_encode_array(__pyx_v_p, 5);
 
-      /* "asynctnt/iproto/requests/update.pyx":148
+      /* "asynctnt/iproto/requests/update.pyx":146
  * 
  *             p = mp_encode_array(p, 5)
  *             p = mp_encode_str(p, op_str_c, 1)             # <<<<<<<<<<<<<<
- *             p = mp_encode_uint(p, field_no)
- *             p = mp_encode_uint(p, splice_position)
+ *             if field_str_c == NULL:
+ *                 p = mp_encode_uint(p, field_no)
  */
       __pyx_v_p = mp_encode_str(__pyx_v_p, __pyx_v_op_str_c, 1);
 
-      /* "asynctnt/iproto/requests/update.pyx":149
+      /* "asynctnt/iproto/requests/update.pyx":147
+ *             p = mp_encode_array(p, 5)
+ *             p = mp_encode_str(p, op_str_c, 1)
+ *             if field_str_c == NULL:             # <<<<<<<<<<<<<<
+ *                 p = mp_encode_uint(p, field_no)
+ *             else:
+ */
+      __pyx_t_1 = (__pyx_v_field_str_c == NULL);
+      if (__pyx_t_1) {
+
+        /* "asynctnt/iproto/requests/update.pyx":148
+ *             p = mp_encode_str(p, op_str_c, 1)
+ *             if field_str_c == NULL:
+ *                 p = mp_encode_uint(p, field_no)             # <<<<<<<<<<<<<<
+ *             else:
+ *                 p = mp_encode_str(p, field_str_c, field_str_len)
+ */
+        __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_v_field_no);
+
+        /* "asynctnt/iproto/requests/update.pyx":147
  *             p = mp_encode_array(p, 5)
  *             p = mp_encode_str(p, op_str_c, 1)
- *             p = mp_encode_uint(p, field_no)             # <<<<<<<<<<<<<<
+ *             if field_str_c == NULL:             # <<<<<<<<<<<<<<
+ *                 p = mp_encode_uint(p, field_no)
+ *             else:
+ */
+        goto __pyx_L19;
+      }
+
+      /* "asynctnt/iproto/requests/update.pyx":150
+ *                 p = mp_encode_uint(p, field_no)
+ *             else:
+ *                 p = mp_encode_str(p, field_str_c, field_str_len)             # <<<<<<<<<<<<<<
  *             p = mp_encode_uint(p, splice_position)
  *             p = mp_encode_uint(p, splice_offset)
  */
-      __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_v_field_no);
+      /*else*/ {
+        __pyx_v_p = mp_encode_str(__pyx_v_p, __pyx_v_field_str_c, __pyx_v_field_str_len);
+      }
+      __pyx_L19:;
 
-      /* "asynctnt/iproto/requests/update.pyx":150
- *             p = mp_encode_str(p, op_str_c, 1)
- *             p = mp_encode_uint(p, field_no)
+      /* "asynctnt/iproto/requests/update.pyx":151
+ *             else:
+ *                 p = mp_encode_str(p, field_str_c, field_str_len)
  *             p = mp_encode_uint(p, splice_position)             # <<<<<<<<<<<<<<
  *             p = mp_encode_uint(p, splice_offset)
  *             buffer._length += (p - begin)
  */
       __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_v_splice_position);
 
-      /* "asynctnt/iproto/requests/update.pyx":151
- *             p = mp_encode_uint(p, field_no)
+      /* "asynctnt/iproto/requests/update.pyx":152
+ *                 p = mp_encode_str(p, field_str_c, field_str_len)
  *             p = mp_encode_uint(p, splice_position)
  *             p = mp_encode_uint(p, splice_offset)             # <<<<<<<<<<<<<<
  *             buffer._length += (p - begin)
  *             p = buffer.mp_encode_obj(p, op_argument)
  */
       __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_v_splice_offset);
 
-      /* "asynctnt/iproto/requests/update.pyx":152
+      /* "asynctnt/iproto/requests/update.pyx":153
  *             p = mp_encode_uint(p, splice_position)
  *             p = mp_encode_uint(p, splice_offset)
  *             buffer._length += (p - begin)             # <<<<<<<<<<<<<<
  *             p = buffer.mp_encode_obj(p, op_argument)
  *         else:
  */
       __pyx_v_buffer->_length = (__pyx_v_buffer->_length + (__pyx_v_p - __pyx_v_begin));
 
-      /* "asynctnt/iproto/requests/update.pyx":153
+      /* "asynctnt/iproto/requests/update.pyx":154
  *             p = mp_encode_uint(p, splice_offset)
  *             buffer._length += (p - begin)
  *             p = buffer.mp_encode_obj(p, op_argument)             # <<<<<<<<<<<<<<
  *         else:
  *             raise TypeError(
  */
-      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_obj(__pyx_v_buffer, __pyx_v_p, __pyx_v_op_argument); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 153, __pyx_L1_error)
+      __pyx_t_2 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_obj(__pyx_v_buffer, __pyx_v_p, __pyx_v_op_argument); if (unlikely(__pyx_t_2 == ((char *)NULL))) __PYX_ERR(4, 154, __pyx_L1_error)
       __pyx_v_p = __pyx_t_2;
 
-      /* "asynctnt/iproto/requests/update.pyx":122
+      /* "asynctnt/iproto/requests/update.pyx":120
  *             p = buffer.mp_encode_obj(p, op_argument)
  * 
  *         elif op == tarantool.IPROTO_OP_SPLICE:             # <<<<<<<<<<<<<<
  *             if op_len < 5:
- *                 raise IndexError(
+ *                 raise ValueError(
  */
       break;
       default:
 
-      /* "asynctnt/iproto/requests/update.pyx":156
+      /* "asynctnt/iproto/requests/update.pyx":157
  *         else:
  *             raise TypeError(
  *                 'Unknown update operation type `{}`'.format(op_type_str))             # <<<<<<<<<<<<<<
  *     return p
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Unknown_update_operation_type, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 156, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Unknown_update_operation_type, __pyx_n_s_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 157, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_8 = NULL;
       __pyx_t_7 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_8)) {
@@ -33695,46 +33769,46 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_v_op_type_str};
         __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-        if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 156, __pyx_L1_error)
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(4, 157, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       }
 
-      /* "asynctnt/iproto/requests/update.pyx":155
+      /* "asynctnt/iproto/requests/update.pyx":156
  *             p = buffer.mp_encode_obj(p, op_argument)
  *         else:
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 'Unknown update operation type `{}`'.format(op_type_str))
  *     return p
  */
-      __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 155, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(4, 156, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(4, 155, __pyx_L1_error)
+      __PYX_ERR(4, 156, __pyx_L1_error)
       break;
     }
 
-    /* "asynctnt/iproto/requests/update.pyx":42
+    /* "asynctnt/iproto/requests/update.pyx":48
  *         return p
  * 
  *     for operation in operations:             # <<<<<<<<<<<<<<
  *         if isinstance(operation, tuple):
  *             op_len = cpython.tuple.PyTuple_GET_SIZE(operation)
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "asynctnt/iproto/requests/update.pyx":157
+  /* "asynctnt/iproto/requests/update.pyx":158
  *             raise TypeError(
  *                 'Unknown update operation type `{}`'.format(op_type_str))
  *     return p             # <<<<<<<<<<<<<<
  * 
  * cdef int encode_request_update(WriteBuffer buffer,
  */
   __pyx_r = __pyx_v_p;
@@ -33765,15 +33839,15 @@
   __Pyx_XDECREF(__pyx_v_op_argument);
   __Pyx_XDECREF(__pyx_v_splice_position_obj);
   __Pyx_XDECREF(__pyx_v_splice_offset_obj);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "asynctnt/iproto/requests/update.pyx":159
+/* "asynctnt/iproto/requests/update.pyx":160
  *     return p
  * 
  * cdef int encode_request_update(WriteBuffer buffer,             # <<<<<<<<<<<<<<
  *                                SchemaSpace space, SchemaIndex index,
  *                                key_tuple, list operations,
  */
 
@@ -33795,330 +33869,330 @@
   PyObject *__pyx_t_3 = NULL;
   char *__pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("encode_request_update", 1);
 
-  /* "asynctnt/iproto/requests/update.pyx":173
+  /* "asynctnt/iproto/requests/update.pyx":174
  *         bint default_fields_none
  * 
  *     space_id = space.sid             # <<<<<<<<<<<<<<
  *     index_id = index.iid
  * 
  */
   __pyx_t_1 = __pyx_v_space->sid;
   __pyx_v_space_id = __pyx_t_1;
 
-  /* "asynctnt/iproto/requests/update.pyx":174
+  /* "asynctnt/iproto/requests/update.pyx":175
  * 
  *     space_id = space.sid
  *     index_id = index.iid             # <<<<<<<<<<<<<<
  * 
  *     if not is_upsert:
  */
   __pyx_t_1 = __pyx_v_index->iid;
   __pyx_v_index_id = __pyx_t_1;
 
-  /* "asynctnt/iproto/requests/update.pyx":176
+  /* "asynctnt/iproto/requests/update.pyx":177
  *     index_id = index.iid
  * 
  *     if not is_upsert:             # <<<<<<<<<<<<<<
  *         key_of_tuple = tarantool.IPROTO_KEY
  *         key_of_operations = tarantool.IPROTO_TUPLE
  */
   __pyx_t_2 = (!__pyx_v_is_upsert);
   if (__pyx_t_2) {
 
-    /* "asynctnt/iproto/requests/update.pyx":177
+    /* "asynctnt/iproto/requests/update.pyx":178
  * 
  *     if not is_upsert:
  *         key_of_tuple = tarantool.IPROTO_KEY             # <<<<<<<<<<<<<<
  *         key_of_operations = tarantool.IPROTO_TUPLE
  *         metadata = index.metadata
  */
     __pyx_v_key_of_tuple = __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_KEY;
 
-    /* "asynctnt/iproto/requests/update.pyx":178
+    /* "asynctnt/iproto/requests/update.pyx":179
  *     if not is_upsert:
  *         key_of_tuple = tarantool.IPROTO_KEY
  *         key_of_operations = tarantool.IPROTO_TUPLE             # <<<<<<<<<<<<<<
  *         metadata = index.metadata
  *         default_fields_none = False
  */
     __pyx_v_key_of_operations = __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_TUPLE;
 
-    /* "asynctnt/iproto/requests/update.pyx":179
+    /* "asynctnt/iproto/requests/update.pyx":180
  *         key_of_tuple = tarantool.IPROTO_KEY
  *         key_of_operations = tarantool.IPROTO_TUPLE
  *         metadata = index.metadata             # <<<<<<<<<<<<<<
  *         default_fields_none = False
  *     else:
  */
     __pyx_t_3 = ((PyObject *)__pyx_v_index->metadata);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_metadata = ((struct C_Metadata *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "asynctnt/iproto/requests/update.pyx":180
+    /* "asynctnt/iproto/requests/update.pyx":181
  *         key_of_operations = tarantool.IPROTO_TUPLE
  *         metadata = index.metadata
  *         default_fields_none = False             # <<<<<<<<<<<<<<
  *     else:
  *         key_of_tuple = tarantool.IPROTO_TUPLE
  */
     __pyx_v_default_fields_none = 0;
 
-    /* "asynctnt/iproto/requests/update.pyx":176
+    /* "asynctnt/iproto/requests/update.pyx":177
  *     index_id = index.iid
  * 
  *     if not is_upsert:             # <<<<<<<<<<<<<<
  *         key_of_tuple = tarantool.IPROTO_KEY
  *         key_of_operations = tarantool.IPROTO_TUPLE
  */
     goto __pyx_L3;
   }
 
-  /* "asynctnt/iproto/requests/update.pyx":182
+  /* "asynctnt/iproto/requests/update.pyx":183
  *         default_fields_none = False
  *     else:
  *         key_of_tuple = tarantool.IPROTO_TUPLE             # <<<<<<<<<<<<<<
  *         key_of_operations = tarantool.IPROTO_OPS
  *         metadata = space.metadata
  */
   /*else*/ {
     __pyx_v_key_of_tuple = __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_TUPLE;
 
-    /* "asynctnt/iproto/requests/update.pyx":183
+    /* "asynctnt/iproto/requests/update.pyx":184
  *     else:
  *         key_of_tuple = tarantool.IPROTO_TUPLE
  *         key_of_operations = tarantool.IPROTO_OPS             # <<<<<<<<<<<<<<
  *         metadata = space.metadata
  *         default_fields_none = True
  */
     __pyx_v_key_of_operations = __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_OPS;
 
-    /* "asynctnt/iproto/requests/update.pyx":184
+    /* "asynctnt/iproto/requests/update.pyx":185
  *         key_of_tuple = tarantool.IPROTO_TUPLE
  *         key_of_operations = tarantool.IPROTO_OPS
  *         metadata = space.metadata             # <<<<<<<<<<<<<<
  *         default_fields_none = True
  * 
  */
     __pyx_t_3 = ((PyObject *)__pyx_v_space->metadata);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_metadata = ((struct C_Metadata *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "asynctnt/iproto/requests/update.pyx":185
+    /* "asynctnt/iproto/requests/update.pyx":186
  *         key_of_operations = tarantool.IPROTO_OPS
  *         metadata = space.metadata
  *         default_fields_none = True             # <<<<<<<<<<<<<<
  * 
  *     body_map_sz = 3 + <uint32_t> (index_id > 0)
  */
     __pyx_v_default_fields_none = 1;
   }
   __pyx_L3:;
 
-  /* "asynctnt/iproto/requests/update.pyx":187
+  /* "asynctnt/iproto/requests/update.pyx":188
  *         default_fields_none = True
  * 
  *     body_map_sz = 3 + <uint32_t> (index_id > 0)             # <<<<<<<<<<<<<<
  *     # Size description:
  *     # mp_sizeof_map(body_map_sz)
  */
   __pyx_v_body_map_sz = (3 + ((uint32_t)(__pyx_v_index_id > 0)));
 
-  /* "asynctnt/iproto/requests/update.pyx":194
+  /* "asynctnt/iproto/requests/update.pyx":195
  *     max_body_len = 1 \
  *                    + 1 \
  *                    + 9             # <<<<<<<<<<<<<<
  * 
  *     if index_id > 0:
  */
   __pyx_v_max_body_len = 0xb;
 
-  /* "asynctnt/iproto/requests/update.pyx":196
+  /* "asynctnt/iproto/requests/update.pyx":197
  *                    + 9
  * 
  *     if index_id > 0:             # <<<<<<<<<<<<<<
  *         # + mp_sizeof_uint(TP_INDEX)
  *         # + mp_sizeof_uint(index)
  */
   __pyx_t_2 = (__pyx_v_index_id > 0);
   if (__pyx_t_2) {
 
-    /* "asynctnt/iproto/requests/update.pyx":199
+    /* "asynctnt/iproto/requests/update.pyx":200
  *         # + mp_sizeof_uint(TP_INDEX)
  *         # + mp_sizeof_uint(index)
  *         max_body_len += 1 + 9             # <<<<<<<<<<<<<<
  * 
  *     max_body_len += 1  # + mp_sizeof_uint(TP_KEY)
  */
     __pyx_v_max_body_len = (__pyx_v_max_body_len + 0xa);
 
-    /* "asynctnt/iproto/requests/update.pyx":196
+    /* "asynctnt/iproto/requests/update.pyx":197
  *                    + 9
  * 
  *     if index_id > 0:             # <<<<<<<<<<<<<<
  *         # + mp_sizeof_uint(TP_INDEX)
  *         # + mp_sizeof_uint(index)
  */
   }
 
-  /* "asynctnt/iproto/requests/update.pyx":201
+  /* "asynctnt/iproto/requests/update.pyx":202
  *         max_body_len += 1 + 9
  * 
  *     max_body_len += 1  # + mp_sizeof_uint(TP_KEY)             # <<<<<<<<<<<<<<
  *     max_body_len += 1  # + mp_sizeof_uint(TP_TUPLE)
  * 
  */
   __pyx_v_max_body_len = (__pyx_v_max_body_len + 1);
 
-  /* "asynctnt/iproto/requests/update.pyx":202
+  /* "asynctnt/iproto/requests/update.pyx":203
  * 
  *     max_body_len += 1  # + mp_sizeof_uint(TP_KEY)
  *     max_body_len += 1  # + mp_sizeof_uint(TP_TUPLE)             # <<<<<<<<<<<<<<
  * 
  *     buffer.ensure_allocated(max_body_len)
  */
   __pyx_v_max_body_len = (__pyx_v_max_body_len + 1);
 
-  /* "asynctnt/iproto/requests/update.pyx":204
+  /* "asynctnt/iproto/requests/update.pyx":205
  *     max_body_len += 1  # + mp_sizeof_uint(TP_TUPLE)
  * 
  *     buffer.ensure_allocated(max_body_len)             # <<<<<<<<<<<<<<
  * 
  *     p = begin = &buffer._buf[buffer._length]
  */
-  __pyx_t_1 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_ensure_allocated(__pyx_v_buffer, __pyx_v_max_body_len); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(4, 204, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_ensure_allocated(__pyx_v_buffer, __pyx_v_max_body_len); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(4, 205, __pyx_L1_error)
 
-  /* "asynctnt/iproto/requests/update.pyx":206
+  /* "asynctnt/iproto/requests/update.pyx":207
  *     buffer.ensure_allocated(max_body_len)
  * 
  *     p = begin = &buffer._buf[buffer._length]             # <<<<<<<<<<<<<<
  *     p = mp_encode_map(p, body_map_sz)
  *     p = mp_encode_uint(p, tarantool.IPROTO_SPACE_ID)
  */
   __pyx_t_4 = (&(__pyx_v_buffer->_buf[__pyx_v_buffer->_length]));
   __pyx_v_p = __pyx_t_4;
   __pyx_v_begin = __pyx_t_4;
 
-  /* "asynctnt/iproto/requests/update.pyx":207
+  /* "asynctnt/iproto/requests/update.pyx":208
  * 
  *     p = begin = &buffer._buf[buffer._length]
  *     p = mp_encode_map(p, body_map_sz)             # <<<<<<<<<<<<<<
  *     p = mp_encode_uint(p, tarantool.IPROTO_SPACE_ID)
  *     p = mp_encode_uint(p, space_id)
  */
   __pyx_v_p = mp_encode_map(__pyx_v_p, __pyx_v_body_map_sz);
 
-  /* "asynctnt/iproto/requests/update.pyx":208
+  /* "asynctnt/iproto/requests/update.pyx":209
  *     p = begin = &buffer._buf[buffer._length]
  *     p = mp_encode_map(p, body_map_sz)
  *     p = mp_encode_uint(p, tarantool.IPROTO_SPACE_ID)             # <<<<<<<<<<<<<<
  *     p = mp_encode_uint(p, space_id)
  * 
  */
   __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_SPACE_ID);
 
-  /* "asynctnt/iproto/requests/update.pyx":209
+  /* "asynctnt/iproto/requests/update.pyx":210
  *     p = mp_encode_map(p, body_map_sz)
  *     p = mp_encode_uint(p, tarantool.IPROTO_SPACE_ID)
  *     p = mp_encode_uint(p, space_id)             # <<<<<<<<<<<<<<
  * 
  *     if index_id > 0:
  */
   __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_v_space_id);
 
-  /* "asynctnt/iproto/requests/update.pyx":211
+  /* "asynctnt/iproto/requests/update.pyx":212
  *     p = mp_encode_uint(p, space_id)
  * 
  *     if index_id > 0:             # <<<<<<<<<<<<<<
  *         p = mp_encode_uint(p, tarantool.IPROTO_INDEX_ID)
  *         p = mp_encode_uint(p, index_id)
  */
   __pyx_t_2 = (__pyx_v_index_id > 0);
   if (__pyx_t_2) {
 
-    /* "asynctnt/iproto/requests/update.pyx":212
+    /* "asynctnt/iproto/requests/update.pyx":213
  * 
  *     if index_id > 0:
  *         p = mp_encode_uint(p, tarantool.IPROTO_INDEX_ID)             # <<<<<<<<<<<<<<
  *         p = mp_encode_uint(p, index_id)
  *     buffer._length += (p - begin)
  */
     __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_e_8asynctnt_6iproto_9tarantool_IPROTO_INDEX_ID);
 
-    /* "asynctnt/iproto/requests/update.pyx":213
+    /* "asynctnt/iproto/requests/update.pyx":214
  *     if index_id > 0:
  *         p = mp_encode_uint(p, tarantool.IPROTO_INDEX_ID)
  *         p = mp_encode_uint(p, index_id)             # <<<<<<<<<<<<<<
  *     buffer._length += (p - begin)
  * 
  */
     __pyx_v_p = mp_encode_uint(__pyx_v_p, __pyx_v_index_id);
 
-    /* "asynctnt/iproto/requests/update.pyx":211
+    /* "asynctnt/iproto/requests/update.pyx":212
  *     p = mp_encode_uint(p, space_id)
  * 
  *     if index_id > 0:             # <<<<<<<<<<<<<<
  *         p = mp_encode_uint(p, tarantool.IPROTO_INDEX_ID)
  *         p = mp_encode_uint(p, index_id)
  */
   }
 
-  /* "asynctnt/iproto/requests/update.pyx":214
+  /* "asynctnt/iproto/requests/update.pyx":215
  *         p = mp_encode_uint(p, tarantool.IPROTO_INDEX_ID)
  *         p = mp_encode_uint(p, index_id)
  *     buffer._length += (p - begin)             # <<<<<<<<<<<<<<
  * 
  *     p = buffer.mp_encode_uint(p, key_of_tuple)
  */
   __pyx_v_buffer->_length = (__pyx_v_buffer->_length + (__pyx_v_p - __pyx_v_begin));
 
-  /* "asynctnt/iproto/requests/update.pyx":216
+  /* "asynctnt/iproto/requests/update.pyx":217
  *     buffer._length += (p - begin)
  * 
  *     p = buffer.mp_encode_uint(p, key_of_tuple)             # <<<<<<<<<<<<<<
  *     p = encode_key_sequence(buffer, p, key_tuple, metadata, default_fields_none)
  * 
  */
-  __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_uint(__pyx_v_buffer, __pyx_v_p, __pyx_v_key_of_tuple); if (unlikely(__pyx_t_4 == ((char *)NULL))) __PYX_ERR(4, 216, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_uint(__pyx_v_buffer, __pyx_v_p, __pyx_v_key_of_tuple); if (unlikely(__pyx_t_4 == ((char *)NULL))) __PYX_ERR(4, 217, __pyx_L1_error)
   __pyx_v_p = __pyx_t_4;
 
-  /* "asynctnt/iproto/requests/update.pyx":217
+  /* "asynctnt/iproto/requests/update.pyx":218
  * 
  *     p = buffer.mp_encode_uint(p, key_of_tuple)
  *     p = encode_key_sequence(buffer, p, key_tuple, metadata, default_fields_none)             # <<<<<<<<<<<<<<
  * 
  *     p = buffer.mp_encode_uint(p, key_of_operations)
  */
-  __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_encode_key_sequence(__pyx_v_buffer, __pyx_v_p, __pyx_v_key_tuple, __pyx_v_metadata, __pyx_v_default_fields_none); if (unlikely(__pyx_t_4 == ((char *)NULL))) __PYX_ERR(4, 217, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_encode_key_sequence(__pyx_v_buffer, __pyx_v_p, __pyx_v_key_tuple, __pyx_v_metadata, __pyx_v_default_fields_none); if (unlikely(__pyx_t_4 == ((char *)NULL))) __PYX_ERR(4, 218, __pyx_L1_error)
   __pyx_v_p = __pyx_t_4;
 
-  /* "asynctnt/iproto/requests/update.pyx":219
+  /* "asynctnt/iproto/requests/update.pyx":220
  *     p = encode_key_sequence(buffer, p, key_tuple, metadata, default_fields_none)
  * 
  *     p = buffer.mp_encode_uint(p, key_of_operations)             # <<<<<<<<<<<<<<
  *     p = encode_update_ops(buffer, p, operations, space)
  */
-  __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_uint(__pyx_v_buffer, __pyx_v_p, __pyx_v_key_of_operations); if (unlikely(__pyx_t_4 == ((char *)NULL))) __PYX_ERR(4, 219, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_mp_encode_uint(__pyx_v_buffer, __pyx_v_p, __pyx_v_key_of_operations); if (unlikely(__pyx_t_4 == ((char *)NULL))) __PYX_ERR(4, 220, __pyx_L1_error)
   __pyx_v_p = __pyx_t_4;
 
-  /* "asynctnt/iproto/requests/update.pyx":220
+  /* "asynctnt/iproto/requests/update.pyx":221
  * 
  *     p = buffer.mp_encode_uint(p, key_of_operations)
  *     p = encode_update_ops(buffer, p, operations, space)             # <<<<<<<<<<<<<<
  */
-  __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_encode_update_ops(__pyx_v_buffer, __pyx_v_p, __pyx_v_operations, __pyx_v_space); if (unlikely(__pyx_t_4 == ((char *)NULL))) __PYX_ERR(4, 220, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_8asynctnt_6iproto_8protocol_encode_update_ops(__pyx_v_buffer, __pyx_v_p, __pyx_v_operations, __pyx_v_space); if (unlikely(__pyx_t_4 == ((char *)NULL))) __PYX_ERR(4, 221, __pyx_L1_error)
   __pyx_v_p = __pyx_t_4;
 
-  /* "asynctnt/iproto/requests/update.pyx":159
+  /* "asynctnt/iproto/requests/update.pyx":160
  *     return p
  * 
  * cdef int encode_request_update(WriteBuffer buffer,             # <<<<<<<<<<<<<<
  *                                SchemaSpace space, SchemaIndex index,
  *                                key_tuple, list operations,
  */
 
@@ -41573,15 +41647,15 @@
     /* "asynctnt/iproto/response.pyx":86
  *     cdef inline object pop_push(self):
  *         if not self._push_subscribe:
  *             raise RuntimeError('Cannot pop push from a non-async response')             # <<<<<<<<<<<<<<
  * 
  *         push = self._q_popleft()
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 86, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(5, 86, __pyx_L1_error)
 
     /* "asynctnt/iproto/response.pyx":85
  * 
@@ -42094,15 +42168,15 @@
   __Pyx_INCREF(__pyx_v_x);
   __Pyx_GIVEREF(__pyx_v_x);
   if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_x)) __PYX_ERR(5, 112, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_map, __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyUnicode_Join(__pyx_kp_u__15, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 112, __pyx_L1_error)
+  __pyx_t_2 = PyUnicode_Join(__pyx_kp_u__14, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
@@ -42190,25 +42264,25 @@
       /* "asynctnt/iproto/response.pyx":113
  *             if len(data) > 10:
  *                 parts = map(lambda x: ', '.join(map(repr, x)), [
  *                     data[:5],             # <<<<<<<<<<<<<<
  *                     data[-2:]
  *                 ])
  */
-      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_data, 0, 5, NULL, NULL, &__pyx_slice__16, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(5, 113, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetSlice(__pyx_v_data, 0, 5, NULL, NULL, &__pyx_slice__15, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(5, 113, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
 
       /* "asynctnt/iproto/response.pyx":114
  *                 parts = map(lambda x: ', '.join(map(repr, x)), [
  *                     data[:5],
  *                     data[-2:]             # <<<<<<<<<<<<<<
  *                 ])
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_v_data, -2L, 0, NULL, NULL, &__pyx_slice__17, 1, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 114, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetSlice(__pyx_v_data, -2L, 0, NULL, NULL, &__pyx_slice__16, 1, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 114, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
 
       /* "asynctnt/iproto/response.pyx":112
  *         if data is not None:
  *             if len(data) > 10:
  *                 parts = map(lambda x: ', '.join(map(repr, x)), [             # <<<<<<<<<<<<<<
  *                     data[:5],
@@ -42239,29 +42313,29 @@
       /* "asynctnt/iproto/response.pyx":117
  *                 ])
  * 
  *                 data = ' ... '.join(parts)             # <<<<<<<<<<<<<<
  *                 data = '[' + data + ']'
  * 
  */
-      __pyx_t_6 = PyUnicode_Join(__pyx_kp_u__18, __pyx_v_parts); if (unlikely(!__pyx_t_6)) __PYX_ERR(5, 117, __pyx_L1_error)
+      __pyx_t_6 = PyUnicode_Join(__pyx_kp_u__17, __pyx_v_parts); if (unlikely(!__pyx_t_6)) __PYX_ERR(5, 117, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_6);
       __pyx_t_6 = 0;
 
       /* "asynctnt/iproto/response.pyx":118
  * 
  *                 data = ' ... '.join(parts)
  *                 data = '[' + data + ']'             # <<<<<<<<<<<<<<
  * 
  *         return '<{} sync={} rowcount={} data={}>'.format(
  */
-      __pyx_t_6 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u__19, __pyx_v_data); if (unlikely(!__pyx_t_6)) __PYX_ERR(5, 118, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyUnicode_ConcatSafe(__pyx_kp_u__18, __pyx_v_data); if (unlikely(!__pyx_t_6)) __PYX_ERR(5, 118, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_6, __pyx_kp_u__20); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 118, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyUnicode_ConcatInPlace(__pyx_t_6, __pyx_kp_u__19); if (unlikely(!__pyx_t_5)) __PYX_ERR(5, 118, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_5);
       __pyx_t_5 = 0;
 
       /* "asynctnt/iproto/response.pyx":111
  *         data = self.body
@@ -45032,15 +45106,15 @@
         /* "asynctnt/iproto/response.pyx":306
  *         for i in range(size):
  *             if mp_typeof(b[0][0]) != MP_ARRAY:  # pragma: nocover
  *                 raise TypeError(             # <<<<<<<<<<<<<<
  *                     'Tuple must be an array when decoding as TarantoolTuple'
  *                 )
  */
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 306, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 306, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_Raise(__pyx_t_1, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __PYX_ERR(5, 306, __pyx_L1_error)
 
         /* "asynctnt/iproto/response.pyx":305
  * 
@@ -45256,15 +45330,15 @@
     /* "asynctnt/iproto/response.pyx":337
  * 
  *     if mp_typeof(b[0]) != MP_MAP:  # pragma: nocover
  *         raise TypeError('Response header must be a MP_MAP')             # <<<<<<<<<<<<<<
  * 
  *     # parsing header
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 337, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 337, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(5, 337, __pyx_L1_error)
 
     /* "asynctnt/iproto/response.pyx":336
  *     # stdio.fprintf(stdio.stdout, "\n")
@@ -45309,15 +45383,15 @@
       /* "asynctnt/iproto/response.pyx":343
  *     for _ in range(size):
  *         if mp_typeof(b[0]) != MP_UINT:  # pragma: nocover
  *             raise TypeError('Header key must be a MP_UINT')             # <<<<<<<<<<<<<<
  * 
  *         key = mp_decode_uint(&b)
  */
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 343, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 343, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __PYX_ERR(5, 343, __pyx_L1_error)
 
       /* "asynctnt/iproto/response.pyx":342
  *     size = mp_decode_map(&b)
@@ -45360,15 +45434,15 @@
         /* "asynctnt/iproto/response.pyx":348
  *         if key == tarantool.IPROTO_REQUEST_TYPE:
  *             if mp_typeof(b[0]) != MP_UINT:  # pragma: nocover
  *                 raise TypeError('code type must be a MP_UINT')             # <<<<<<<<<<<<<<
  * 
  *             hdr.code = <uint32_t> mp_decode_uint(&b)
  */
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 348, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 348, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_Raise(__pyx_t_2, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __PYX_ERR(5, 348, __pyx_L1_error)
 
         /* "asynctnt/iproto/response.pyx":347
  *         key = mp_decode_uint(&b)
@@ -45420,15 +45494,15 @@
         /* "asynctnt/iproto/response.pyx":354
  *         elif key == tarantool.IPROTO_SYNC:
  *             if mp_typeof(b[0]) != MP_UINT:  # pragma: nocover
  *                 raise TypeError('sync type must be a MP_UINT')             # <<<<<<<<<<<<<<
  * 
  *             hdr.sync = mp_decode_uint(&b)
  */
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 354, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 354, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_Raise(__pyx_t_2, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __PYX_ERR(5, 354, __pyx_L1_error)
 
         /* "asynctnt/iproto/response.pyx":353
  *             hdr.return_code = hdr.code & 0x7FFF
@@ -45471,15 +45545,15 @@
         /* "asynctnt/iproto/response.pyx":359
  *         elif key == tarantool.IPROTO_SCHEMA_VERSION:
  *             if mp_typeof(b[0]) != MP_UINT:  # pragma: nocover
  *                 raise TypeError('schema_id type must be a MP_UINT')             # <<<<<<<<<<<<<<
  * 
  *             hdr.schema_id = mp_decode_uint(&b)
  */
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 359, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 359, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_Raise(__pyx_t_2, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __PYX_ERR(5, 359, __pyx_L1_error)
 
         /* "asynctnt/iproto/response.pyx":358
  *             hdr.sync = mp_decode_uint(&b)
@@ -45695,15 +45769,15 @@
       /* "asynctnt/iproto/response.pyx":385
  *         field_map_size = mp_decode_map(b)
  *         if field_map_size == 0:  # pragma: nocover
  *             raise RuntimeError('Field map must contain at least '             # <<<<<<<<<<<<<<
  *                                '1 element - field_name')
  * 
  */
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 385, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 385, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __PYX_ERR(5, 385, __pyx_L1_error)
 
       /* "asynctnt/iproto/response.pyx":384
  *     for i in range(arr_size):
@@ -46127,15 +46201,15 @@
  * 
  *                 else:  # pragma: nocover
  *                     raise TypeError(             # <<<<<<<<<<<<<<
  *                         "IPROTO_FIELD_SPAN must be either STR or NIL"
  *                     )
  */
         /*else*/ {
-          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 432, __pyx_L1_error)
+          __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 432, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_1);
           __Pyx_Raise(__pyx_t_1, 0, 0, 0);
           __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
           __PYX_ERR(5, 432, __pyx_L1_error)
         }
         __pyx_L8:;
 
@@ -46221,15 +46295,15 @@
       /* "asynctnt/iproto/response.pyx":441
  * 
  *         if field.name is None:  # pragma: nocover
  *             raise RuntimeError('field.name must not be None')             # <<<<<<<<<<<<<<
  * 
  *         metadata.add(<int> field_id, field)
  */
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 441, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 441, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __PYX_ERR(5, 441, __pyx_L1_error)
 
       /* "asynctnt/iproto/response.pyx":440
  *                 mp_next(b)
@@ -47132,15 +47206,15 @@
     /* "asynctnt/iproto/response.pyx":557
  * 
  *     if mp_typeof(b[0]) != MP_MAP:  # pragma: nocover
  *         raise TypeError('Response body must be a MP_MAP')             # <<<<<<<<<<<<<<
  * 
  *     size = mp_decode_map(&b)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 557, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 557, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(5, 557, __pyx_L1_error)
 
     /* "asynctnt/iproto/response.pyx":556
  *     # parsing body
@@ -47185,15 +47259,15 @@
       /* "asynctnt/iproto/response.pyx":562
  *     for _ in range(size):
  *         if mp_typeof(b[0]) != MP_UINT:  # pragma: nocover
  *             raise TypeError('Header key must be a MP_UINT')             # <<<<<<<<<<<<<<
  * 
  *         key = mp_decode_uint(&b)
  */
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 562, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 562, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __PYX_ERR(5, 562, __pyx_L1_error)
 
       /* "asynctnt/iproto/response.pyx":561
  *     size = mp_decode_map(&b)
@@ -47236,15 +47310,15 @@
         /* "asynctnt/iproto/response.pyx":567
  *         if key == tarantool.IPROTO_ERROR_24:
  *             if mp_typeof(b[0]) != MP_STR:  # pragma: nocover
  *                 raise TypeError('errstr type must be a MP_STR')             # <<<<<<<<<<<<<<
  * 
  *             s = NULL
  */
-        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 567, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(5, 567, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_Raise(__pyx_t_2, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __PYX_ERR(5, 567, __pyx_L1_error)
 
         /* "asynctnt/iproto/response.pyx":566
  *         key = mp_decode_uint(&b)
@@ -47326,15 +47400,15 @@
         /* "asynctnt/iproto/response.pyx":576
  *         elif key == tarantool.IPROTO_ERROR:
  *             if mp_typeof(b[0]) != MP_MAP:  # pragma: nocover
  *                 raise TypeError('IPROTO_ERROR type must be a MP_MAP')             # <<<<<<<<<<<<<<
  * 
  *             resp.error = parse_iproto_error(&b, resp.encoding)
  */
-        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(5, 576, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(5, 576, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_Raise(__pyx_t_7, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __PYX_ERR(5, 576, __pyx_L1_error)
 
         /* "asynctnt/iproto/response.pyx":575
  * 
@@ -47601,15 +47675,15 @@
         /* "asynctnt/iproto/response.pyx":606
  *             field_map_size = mp_decode_map(&b)
  *             if field_map_size == 0:
  *                 raise RuntimeError('Field map must contain at least '             # <<<<<<<<<<<<<<
  *                                    '1 element - rowcount')
  * 
  */
-        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(5, 606, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(5, 606, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_Raise(__pyx_t_6, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __PYX_ERR(5, 606, __pyx_L1_error)
 
         /* "asynctnt/iproto/response.pyx":605
  *         elif key == tarantool.IPROTO_SQL_INFO:
@@ -47834,15 +47908,15 @@
         /* "asynctnt/iproto/response.pyx":627
  *         elif key == tarantool.IPROTO_DATA:
  *             if mp_typeof(b[0]) != MP_ARRAY:  # pragma: nocover
  *                 raise TypeError('body data type must be a MP_ARRAY')             # <<<<<<<<<<<<<<
  *             data = _response_parse_body_data(&b, resp, req)
  *             if is_chunk:
  */
-        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(5, 627, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(5, 627, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_Raise(__pyx_t_7, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __PYX_ERR(5, 627, __pyx_L1_error)
 
         /* "asynctnt/iproto/response.pyx":626
  * 
@@ -50267,15 +50341,15 @@
  *             req.statement_id = <uint64_t> query
  *         else:
  *             raise TypeError('query must be either str or int')             # <<<<<<<<<<<<<<
  * 
  *         req.args = args
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(26, 252, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(26, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(26, 252, __pyx_L1_error)
   }
   __pyx_L3:;
 
@@ -50520,15 +50594,15 @@
  *             req.statement_id = <uint64_t> query
  *         else:
  *             raise TypeError('query must be either str or int')             # <<<<<<<<<<<<<<
  * 
  *         req.push_subscribe = False
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(26, 281, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(26, 281, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(26, 281, __pyx_L1_error)
   }
   __pyx_L3:;
 
@@ -54532,15 +54606,15 @@
     /* "asynctnt/iproto/push.pyx":37
  *             BaseRequest request
  *         if not hasattr(fut, '_response'):
  *             raise ValueError('Future is invalid. Make sure to call with '             # <<<<<<<<<<<<<<
  *                              'a future returned from a method with '
  *                              'push_subscribe=True flag')
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(27, 37, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(27, 37, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(27, 37, __pyx_L1_error)
 
     /* "asynctnt/iproto/push.pyx":36
  *             Response response
@@ -54591,15 +54665,15 @@
     /* "asynctnt/iproto/push.pyx":45
  * 
  *         if not request.push_subscribe:
  *             raise ValueError('Future is invalid. Make sure to call with '             # <<<<<<<<<<<<<<
  *                              'a future returned from a method with '
  *                              'push_subscribe=True flag')
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(27, 45, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(27, 45, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(27, 45, __pyx_L1_error)
 
     /* "asynctnt/iproto/push.pyx":44
  *         request = response.request_
@@ -54707,15 +54781,15 @@
   /* "asynctnt/iproto/push.pyx":54
  * 
  *     def __iter__(self):
  *         raise RuntimeError('Cannot use iter with PushIterator - use aiter')             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(27, 54, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(27, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(27, 54, __pyx_L1_error)
 
   /* "asynctnt/iproto/push.pyx":53
  *         self._response = response
@@ -54770,15 +54844,15 @@
   /* "asynctnt/iproto/push.pyx":57
  * 
  *     def __next__(self):
  *         raise RuntimeError('Cannot use next with PushIterator - use anext')             # <<<<<<<<<<<<<<
  * 
  *     def __aiter__(self):
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(27, 57, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(27, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(27, 57, __pyx_L1_error)
 
   /* "asynctnt/iproto/push.pyx":56
  *         raise RuntimeError('Cannot use iter with PushIterator - use aiter')
@@ -56094,15 +56168,15 @@
  *             self.encoding = encoding
  *         else:
  *             raise TypeError('encoding must be either str or bytes')             # <<<<<<<<<<<<<<
  * 
  *         initial_read_buffer_size = initial_read_buffer_size or 0x20000
  */
   /*else*/ {
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(28, 32, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(28, 32, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(28, 32, __pyx_L1_error)
   }
   __pyx_L5:;
 
@@ -57308,15 +57382,15 @@
   /* "asynctnt/iproto/coreproto.pyx":139
  *             self.rbuf.get_slice(ver_length,
  *                                 ver_length + SALT_LENGTH)
  *         )[:SCRAMBLE_SIZE]             # <<<<<<<<<<<<<<
  *         self.state = PROTOCOL_NORMAL
  *         self._on_greeting_received()
  */
-  __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 20, NULL, NULL, &__pyx_slice__40, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 139, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetSlice(__pyx_t_1, 0, 20, NULL, NULL, &__pyx_slice__39, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_3))) __PYX_ERR(28, 139, __pyx_L1_error)
 
   /* "asynctnt/iproto/coreproto.pyx":136
  *         rbuf = self.rbuf
  *         self.version = self._parse_version(self.rbuf.get_slice_end(ver_length))
@@ -60232,15 +60306,15 @@
     /* "asynctnt/iproto/protocol.pyx":139
  *         if self.post_con_state == POST_CONNECTION_ID:
  *             assert self.version is not None
  *             if self.version >= (2, 10, 0):             # <<<<<<<<<<<<<<
  *                 # send <id> request
  *                 self._do_id()
  */
-    __pyx_t_2 = PyObject_RichCompare(__pyx_v_self->__pyx_base.version, __pyx_tuple__41, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 139, __pyx_L1_error)
+    __pyx_t_2 = PyObject_RichCompare(__pyx_v_self->__pyx_base.version, __pyx_tuple__40, Py_GE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 139, __pyx_L1_error)
     __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(6, 139, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_1) {
 
       /* "asynctnt/iproto/protocol.pyx":141
  *             if self.version >= (2, 10, 0):
  *                 # send <id> request
@@ -61855,15 +61929,15 @@
   /* "asynctnt/iproto/protocol.pyx":250
  *         fut = self._db._id(0.0)
  * 
  *         def on_id(f):             # <<<<<<<<<<<<<<
  *             if f.cancelled():
  *                 self._set_connection_error(asyncio.futures.CancelledError())
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_6_do_id_1on_id, 0, __pyx_n_s_BaseProtocol__do_id_locals_on_id, ((PyObject*)__pyx_cur_scope), __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 250, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_6_do_id_1on_id, 0, __pyx_n_s_BaseProtocol__do_id_locals_on_id, ((PyObject*)__pyx_cur_scope), __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_on_id = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "asynctnt/iproto/protocol.pyx":266
  *                 self._set_connection_error(e)
  * 
@@ -62398,15 +62472,15 @@
   /* "asynctnt/iproto/protocol.pyx":272
  *         fut = self._db._auth(self.salt, username, password, 0)
  * 
  *         def on_authorized(f):             # <<<<<<<<<<<<<<
  *             if f.cancelled():
  *                 self._set_connection_error(asyncio.futures.CancelledError())
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_8_do_auth_1on_authorized, 0, __pyx_n_s_BaseProtocol__do_auth_locals_on, ((PyObject*)__pyx_cur_scope), __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 272, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_8_do_auth_1on_authorized, 0, __pyx_n_s_BaseProtocol__do_auth_locals_on, ((PyObject*)__pyx_cur_scope), __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__43)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 272, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_on_authorized = __pyx_t_2;
   __pyx_t_2 = 0;
 
   /* "asynctnt/iproto/protocol.pyx":288
  *                 self._set_connection_error(e)
  * 
@@ -63872,15 +63946,15 @@
   /* "asynctnt/iproto/protocol.pyx":296
  *         self._schema_fetch_in_progress = True
  * 
  *         def on_fetch(f):             # <<<<<<<<<<<<<<
  *             self._schema_fetch_in_progress = False
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_16_do_fetch_schema_1on_fetch, 0, __pyx_n_s_BaseProtocol__do_fetch_schema_lo, ((PyObject*)__pyx_cur_scope), __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 296, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_16_do_fetch_schema_1on_fetch, 0, __pyx_n_s_BaseProtocol__do_fetch_schema_lo, ((PyObject*)__pyx_cur_scope), __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 296, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_on_fetch = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "asynctnt/iproto/protocol.pyx":349
  *                     fut.set_exception(e)
  * 
@@ -63906,15 +63980,15 @@
   /* "asynctnt/iproto/protocol.pyx":349
  *                     fut.set_exception(e)
  * 
  *         fut_vspace = self._db.select(SPACE_VSPACE, timeout=0,             # <<<<<<<<<<<<<<
  *                                      check_schema_change=False)
  *         fut_vindex = self._db.select(SPACE_VINDEX, timeout=0,
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__47, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(6, 349, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__46, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(6, 349, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_fut_vspace = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "asynctnt/iproto/protocol.pyx":351
@@ -63942,15 +64016,15 @@
   /* "asynctnt/iproto/protocol.pyx":351
  *         fut_vspace = self._db.select(SPACE_VSPACE, timeout=0,
  *                                      check_schema_change=False)
  *         fut_vindex = self._db.select(SPACE_VINDEX, timeout=0,             # <<<<<<<<<<<<<<
  *                                      check_schema_change=False)
  *         gather_fut = asyncio.gather(fut_vspace, fut_vindex,
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__48, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 351, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__47, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 351, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_fut_vindex = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "asynctnt/iproto/protocol.pyx":353
@@ -66577,15 +66651,15 @@
  *             return Iterator[iterator]
  *         else:
  *             raise TypeError('Iterator is of unsupported type '             # <<<<<<<<<<<<<<
  *                             '(asynctnt.Iterator, int, str)')
  * 
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__49, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(6, 502, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__48, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(6, 502, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_ERR(6, 502, __pyx_L1_error)
   }
 
   /* "asynctnt/iproto/protocol.pyx":494
@@ -67263,15 +67337,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9001016, 0xc05ea8e, 0xfe5f18a) = (check_schema_change, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__50, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__49, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -67804,15 +67878,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9001016, 0xc05ea8e, 0xfe5f18a) = (check_schema_change, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__50, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__49, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -68345,15 +68419,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x2d5a81d, 0xac90343, 0xcd9f35b):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x2d5a81d, 0xac90343, 0xcd9f35b) = (args, check_schema_change, func_name, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__51, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__50, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x2d5a81d, 0xac90343, 0xcd9f35b):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -68909,15 +68983,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xafafa67, 0x3c16c97, 0x904102b):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0xafafa67, 0x3c16c97, 0x904102b) = (args, check_schema_change, expression, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__52, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__51, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xafafa67, 0x3c16c97, 0x904102b):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -69473,15 +69547,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x8e2dc2b, 0x62f76f3, 0x57fe0b4):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x8e2dc2b, 0x62f76f3, 0x57fe0b4) = (check_schema_change, index, iterator, key, limit, offset, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__53, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__52, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x8e2dc2b, 0x62f76f3, 0x57fe0b4):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -70065,15 +70139,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb91d1f2, 0xff182e4, 0x15f8d7d):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0xb91d1f2, 0xff182e4, 0x15f8d7d) = (check_schema_change, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, t, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__54, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__53, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb91d1f2, 0xff182e4, 0x15f8d7d):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -70617,15 +70691,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xf383ff7, 0x8ac4f18, 0xe9836c0):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0xf383ff7, 0x8ac4f18, 0xe9836c0) = (check_schema_change, index, key, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__55, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__54, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xf383ff7, 0x8ac4f18, 0xe9836c0):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -71181,15 +71255,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x815e48a, 0x8a9c73b, 0x180001a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x815e48a, 0x8a9c73b, 0x180001a) = (check_schema_change, index, key, op, operations, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__56, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__55, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x815e48a, 0x8a9c73b, 0x180001a):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -71757,15 +71831,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xc823323, 0xea6e875, 0x0493034):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0xc823323, 0xea6e875, 0x0493034) = (check_schema_change, op, operations, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, t, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__57, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__56, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xc823323, 0xea6e875, 0x0493034):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -72321,15 +72395,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd0934a3, 0xcc899a0, 0x7b3178d):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0xd0934a3, 0xcc899a0, 0x7b3178d) = (check_schema_change, op, parse_as_tuples, parse_metadata, push_subscribe, query, schema_id, space, statement_id, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__58, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__57, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xd0934a3, 0xcc899a0, 0x7b3178d):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -72883,15 +72957,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x314ca88, 0x64ec1ad, 0xd228fa0):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x314ca88, 0x64ec1ad, 0xd228fa0) = (args, check_schema_change, op, parse_as_tuples, parse_metadata, push_subscribe, query, schema_id, space, statement_id, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__59, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__58, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x314ca88, 0x64ec1ad, 0xd228fa0):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -73456,15 +73530,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9001016, 0xc05ea8e, 0xfe5f18a) = (check_schema_change, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__50, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__49, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -73997,15 +74071,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x335e105, 0xf5a1799, 0xa2d5d5d):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x335e105, 0xf5a1799, 0xa2d5d5d) = (check_schema_change, op, parse_as_tuples, parse_metadata, password, push_subscribe, salt, schema_id, space, stream_id, sync, timeout_handle, username, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__60, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__59, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x335e105, 0xf5a1799, 0xa2d5d5d):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -74574,15 +74648,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x30f95df, 0xa4f125c, 0xfc952a6):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x30f95df, 0xa4f125c, 0xfc952a6) = (check_schema_change, isolation, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, tx_timeout, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__61, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__60, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x30f95df, 0xa4f125c, 0xfc952a6):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -75135,15 +75209,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9001016, 0xc05ea8e, 0xfe5f18a) = (check_schema_change, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__50, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__49, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -75676,15 +75750,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9001016, 0xc05ea8e, 0xfe5f18a) = (check_schema_change, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__50, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__49, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -76217,15 +76291,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xab276bf, 0xb7ed9c7, 0x6438658):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0xab276bf, 0xb7ed9c7, 0x6438658) = (code, err_no, error_type, fields, file, line, message))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__62, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__61, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xab276bf, 0xb7ed9c7, 0x6438658):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -76724,15 +76798,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xeafe895, 0xd0fa554, 0x04a7503):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0xeafe895, 0xd0fa554, 0x04a7503) = (trace))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__63, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__62, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xeafe895, 0xd0fa554, 0x04a7503):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -77168,15 +77242,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x98137af, 0xbb11453, 0xd6d3964):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x98137af, 0xbb11453, 0xd6d3964) = (_fut, _request, _response))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__64, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__63, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x98137af, 0xbb11453, 0xd6d3964):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -77635,15 +77709,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x89d360e, 0xe0a6eac, 0xf188771):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x89d360e, 0xe0a6eac, 0xf188771) = (con_state, encoding, host, port, rbuf, salt, state, version))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__65, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__64, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x89d360e, 0xe0a6eac, 0xf188771):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -84707,15 +84781,14 @@
     {&__pyx_n_s_Metadata, __pyx_k_Metadata, sizeof(__pyx_k_Metadata), 0, 0, 1, 1},
     {&__pyx_n_s_Metadata___reduce_cython, __pyx_k_Metadata___reduce_cython, sizeof(__pyx_k_Metadata___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Metadata___setstate_cython, __pyx_k_Metadata___setstate_cython, sizeof(__pyx_k_Metadata___setstate_cython), 0, 0, 1, 1},
     {&__pyx_kp_u_Metadata_fields_count, __pyx_k_Metadata_fields_count, sizeof(__pyx_k_Metadata_fields_count), 0, 1, 0, 0},
     {&__pyx_n_s_NEIGHBOR, __pyx_k_NEIGHBOR, sizeof(__pyx_k_NEIGHBOR), 0, 0, 1, 1},
     {&__pyx_n_s_OVERLAPS, __pyx_k_OVERLAPS, sizeof(__pyx_k_OVERLAPS), 0, 0, 1, 1},
     {&__pyx_kp_u_Offset_incorrect_Got_use_len, __pyx_k_Offset_incorrect_Got_use_len, sizeof(__pyx_k_Offset_incorrect_Got_use_len), 0, 1, 0, 0},
-    {&__pyx_kp_u_Operation_field_no_must_be_int_a, __pyx_k_Operation_field_no_must_be_int_a, sizeof(__pyx_k_Operation_field_no_must_be_int_a), 0, 1, 0, 0},
     {&__pyx_kp_u_Operation_field_no_must_be_of_ei, __pyx_k_Operation_field_no_must_be_of_ei, sizeof(__pyx_k_Operation_field_no_must_be_of_ei), 0, 1, 0, 0},
     {&__pyx_kp_u_Operation_length_must_be_at_leas, __pyx_k_Operation_length_must_be_at_leas, sizeof(__pyx_k_Operation_length_must_be_at_leas), 0, 1, 0, 0},
     {&__pyx_kp_u_Operation_type_must_of_a_str_or, __pyx_k_Operation_type_must_of_a_str_or, sizeof(__pyx_k_Operation_type_must_of_a_str_or), 0, 1, 0, 0},
     {&__pyx_n_s_Optional, __pyx_k_Optional, sizeof(__pyx_k_Optional), 0, 0, 1, 1},
     {&__pyx_kp_u_Part_len_must_be_2, __pyx_k_Part_len_must_be_2, sizeof(__pyx_k_Part_len_must_be_2), 0, 1, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_PingRequest, __pyx_k_PingRequest, sizeof(__pyx_k_PingRequest), 0, 0, 1, 1},
@@ -84802,23 +84875,23 @@
     {&__pyx_n_s_UpsertRequest___setstate_cython, __pyx_k_UpsertRequest___setstate_cython, sizeof(__pyx_k_UpsertRequest___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_VERSION_STRING_REGEX, __pyx_k_VERSION_STRING_REGEX, sizeof(__pyx_k_VERSION_STRING_REGEX), 0, 0, 1, 1},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_WriteBuffer, __pyx_k_WriteBuffer, sizeof(__pyx_k_WriteBuffer), 0, 0, 1, 1},
     {&__pyx_n_s_WriteBuffer___reduce_cython, __pyx_k_WriteBuffer___reduce_cython, sizeof(__pyx_k_WriteBuffer___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_WriteBuffer___setstate_cython, __pyx_k_WriteBuffer___setstate_cython, sizeof(__pyx_k_WriteBuffer___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_WriteBuffer_hex, __pyx_k_WriteBuffer_hex, sizeof(__pyx_k_WriteBuffer_hex), 0, 0, 1, 1},
-    {&__pyx_kp_u__15, __pyx_k__15, sizeof(__pyx_k__15), 0, 1, 0, 0},
+    {&__pyx_kp_u__14, __pyx_k__14, sizeof(__pyx_k__14), 0, 1, 0, 0},
+    {&__pyx_kp_u__17, __pyx_k__17, sizeof(__pyx_k__17), 0, 1, 0, 0},
     {&__pyx_kp_u__18, __pyx_k__18, sizeof(__pyx_k__18), 0, 1, 0, 0},
     {&__pyx_kp_u__19, __pyx_k__19, sizeof(__pyx_k__19), 0, 1, 0, 0},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-    {&__pyx_kp_u__20, __pyx_k__20, sizeof(__pyx_k__20), 0, 1, 0, 0},
-    {&__pyx_n_s__212, __pyx_k__212, sizeof(__pyx_k__212), 0, 0, 1, 1},
+    {&__pyx_n_s__211, __pyx_k__211, sizeof(__pyx_k__211), 0, 0, 1, 1},
     {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
     {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
-    {&__pyx_n_s__66, __pyx_k__66, sizeof(__pyx_k__66), 0, 0, 1, 1},
+    {&__pyx_n_s__65, __pyx_k__65, sizeof(__pyx_k__65), 0, 0, 1, 1},
     {&__pyx_n_s_add_done_callback, __pyx_k_add_done_callback, sizeof(__pyx_k_add_done_callback), 0, 0, 1, 1},
     {&__pyx_n_s_anext, __pyx_k_anext, sizeof(__pyx_k_anext), 0, 0, 1, 1},
     {&__pyx_n_s_append, __pyx_k_append, sizeof(__pyx_k_append), 0, 0, 1, 1},
     {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
     {&__pyx_n_s_as_tuple, __pyx_k_as_tuple, sizeof(__pyx_k_as_tuple), 0, 0, 1, 1},
     {&__pyx_n_u_ascii, __pyx_k_ascii, sizeof(__pyx_k_ascii), 0, 1, 0, 1},
     {&__pyx_n_s_asyncio, __pyx_k_asyncio, sizeof(__pyx_k_asyncio), 0, 0, 1, 1},
@@ -84922,15 +84995,14 @@
     {&__pyx_n_s_indexes, __pyx_k_indexes, sizeof(__pyx_k_indexes), 0, 0, 1, 1},
     {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
     {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
     {&__pyx_n_s_initial_read_buffer_size, __pyx_k_initial_read_buffer_size, sizeof(__pyx_k_initial_read_buffer_size), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
     {&__pyx_n_s_insert, __pyx_k_insert, sizeof(__pyx_k_insert), 0, 0, 1, 1},
     {&__pyx_n_s_inspect, __pyx_k_inspect, sizeof(__pyx_k_inspect), 0, 0, 1, 1},
-    {&__pyx_kp_u_int_argument_required_for_Arithm, __pyx_k_int_argument_required_for_Arithm, sizeof(__pyx_k_int_argument_required_for_Arithm), 0, 1, 0, 0},
     {&__pyx_kp_u_invalid_datetime_size_got_extra, __pyx_k_invalid_datetime_size_got_extra, sizeof(__pyx_k_invalid_datetime_size_got_extra), 0, 1, 0, 0},
     {&__pyx_kp_u_iproto_error_stack_frame_fields, __pyx_k_iproto_error_stack_frame_fields, sizeof(__pyx_k_iproto_error_stack_frame_fields), 0, 1, 0, 0},
     {&__pyx_n_s_is_connected, __pyx_k_is_connected, sizeof(__pyx_k_is_connected), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_n_s_is_fully_connected, __pyx_k_is_fully_connected, sizeof(__pyx_k_is_fully_connected), 0, 0, 1, 1},
     {&__pyx_n_u_is_nullable, __pyx_k_is_nullable, sizeof(__pyx_k_is_nullable), 0, 1, 0, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
@@ -85092,21 +85164,21 @@
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(1, 51, __pyx_L1_error)
-  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(1, 187, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 215, __pyx_L1_error)
+  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(1, 196, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 224, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 173, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(3, 39, __pyx_L1_error)
   __pyx_builtin_BufferError = __Pyx_GetBuiltinName(__pyx_n_s_BufferError); if (!__pyx_builtin_BufferError) __PYX_ERR(3, 67, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(3, 106, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(4, 51, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(4, 57, __pyx_L1_error)
   __pyx_builtin_map = __Pyx_GetBuiltinName(__pyx_n_s_map); if (!__pyx_builtin_map) __PYX_ERR(5, 112, __pyx_L1_error)
   __pyx_builtin_UnicodeDecodeError = __Pyx_GetBuiltinName(__pyx_n_s_UnicodeDecodeError); if (!__pyx_builtin_UnicodeDecodeError) __PYX_ERR(5, 209, __pyx_L1_error)
   __pyx_builtin_hex = __Pyx_GetBuiltinName(__pyx_n_s_hex); if (!__pyx_builtin_hex) __PYX_ERR(5, 644, __pyx_L1_error)
   __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(6, 105, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
@@ -85146,1340 +85218,1329 @@
  * 
  *     cdef inline len(self):
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_the_buffer_is_in_read_only_mode); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(3, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "asynctnt/iproto/requests/update.pyx":48
+  /* "asynctnt/iproto/requests/update.pyx":54
  *             op_len = cpython.list.PyList_GET_SIZE(operation)
  *         else:
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 'Single operation must be a tuple or list')
  *         if op_len < 3:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Single_operation_must_be_a_tuple); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(4, 48, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_Single_operation_must_be_a_tuple); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(4, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "asynctnt/iproto/requests/update.pyx":51
+  /* "asynctnt/iproto/requests/update.pyx":57
  *                 'Single operation must be a tuple or list')
  *         if op_len < 3:
  *             raise IndexError(             # <<<<<<<<<<<<<<
  *                 'Operation length must be at least 3')
  * 
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Operation_length_must_be_at_leas); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(4, 51, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_Operation_length_must_be_at_leas); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(4, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "asynctnt/iproto/requests/update.pyx":60
+  /* "asynctnt/iproto/requests/update.pyx":66
  *             str_temp = <bytes> op_type_str
  *         else:
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 'Operation type must of a str or bytes type')
  * 
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Operation_type_must_of_a_str_or); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(4, 60, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Operation_type_must_of_a_str_or); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(4, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "asynctnt/iproto/requests/update.pyx":74
- *                     'no format declaration in space {}'.format(space.sid))
+  /* "asynctnt/iproto/requests/update.pyx":87
+ *                 cpython.bytes.PyBytes_AsStringAndSize(str_temp, &field_str_c, &field_str_len)
  *         else:
  *             raise TypeError(             # <<<<<<<<<<<<<<
  *                 'Operation field_no must be of either int or str type')
  * 
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Operation_field_no_must_be_of_ei); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(4, 74, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_Operation_field_no_must_be_of_ei); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(4, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "asynctnt/iproto/requests/update.pyx":91
- *             op_argument = operation[2]
- *             if not isinstance(op_argument, int):
- *                 raise TypeError(             # <<<<<<<<<<<<<<
- *                     'int argument required for '
- *                     'Arithmetic and Delete operations'
- */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_int_argument_required_for_Arithm); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(4, 91, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-
-  /* "asynctnt/iproto/requests/update.pyx":133
+  /* "asynctnt/iproto/requests/update.pyx":131
  *             op_argument = operation[4]
  *             if not isinstance(splice_position_obj, int):
  *                 raise TypeError('Splice position must be int')             # <<<<<<<<<<<<<<
  *             if not isinstance(splice_offset_obj, int):
  *                 raise TypeError('Splice offset must be int')
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_Splice_position_must_be_int); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(4, 133, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_Splice_position_must_be_int); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(4, 131, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "asynctnt/iproto/requests/update.pyx":135
+  /* "asynctnt/iproto/requests/update.pyx":133
  *                 raise TypeError('Splice position must be int')
  *             if not isinstance(splice_offset_obj, int):
  *                 raise TypeError('Splice offset must be int')             # <<<<<<<<<<<<<<
  * 
  *             splice_position = <uint32_t> splice_position_obj
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_Splice_offset_must_be_int); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(4, 135, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_Splice_offset_must_be_int); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(4, 133, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "asynctnt/iproto/response.pyx":86
  *     cdef inline object pop_push(self):
  *         if not self._push_subscribe:
  *             raise RuntimeError('Cannot pop push from a non-async response')             # <<<<<<<<<<<<<<
  * 
  *         push = self._q_popleft()
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_Cannot_pop_push_from_a_non_async); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(5, 86, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_u_Cannot_pop_push_from_a_non_async); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(5, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "asynctnt/iproto/response.pyx":113
  *             if len(data) > 10:
  *                 parts = map(lambda x: ', '.join(map(repr, x)), [
  *                     data[:5],             # <<<<<<<<<<<<<<
  *                     data[-2:]
  *                 ])
  */
-  __pyx_slice__16 = PySlice_New(Py_None, __pyx_int_5, Py_None); if (unlikely(!__pyx_slice__16)) __PYX_ERR(5, 113, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__16);
-  __Pyx_GIVEREF(__pyx_slice__16);
+  __pyx_slice__15 = PySlice_New(Py_None, __pyx_int_5, Py_None); if (unlikely(!__pyx_slice__15)) __PYX_ERR(5, 113, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__15);
+  __Pyx_GIVEREF(__pyx_slice__15);
 
   /* "asynctnt/iproto/response.pyx":114
  *                 parts = map(lambda x: ', '.join(map(repr, x)), [
  *                     data[:5],
  *                     data[-2:]             # <<<<<<<<<<<<<<
  *                 ])
  * 
  */
-  __pyx_slice__17 = PySlice_New(__pyx_int_neg_2, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(5, 114, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__17);
-  __Pyx_GIVEREF(__pyx_slice__17);
+  __pyx_slice__16 = PySlice_New(__pyx_int_neg_2, Py_None, Py_None); if (unlikely(!__pyx_slice__16)) __PYX_ERR(5, 114, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__16);
+  __Pyx_GIVEREF(__pyx_slice__16);
 
   /* "asynctnt/iproto/response.pyx":306
  *         for i in range(size):
  *             if mp_typeof(b[0][0]) != MP_ARRAY:  # pragma: nocover
  *                 raise TypeError(             # <<<<<<<<<<<<<<
  *                     'Tuple must be an array when decoding as TarantoolTuple'
  *                 )
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_u_Tuple_must_be_an_array_when_deco); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(5, 306, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_u_Tuple_must_be_an_array_when_deco); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(5, 306, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "asynctnt/iproto/response.pyx":337
  * 
  *     if mp_typeof(b[0]) != MP_MAP:  # pragma: nocover
  *         raise TypeError('Response header must be a MP_MAP')             # <<<<<<<<<<<<<<
  * 
  *     # parsing header
  */
-  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_u_Response_header_must_be_a_MP_MAP); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(5, 337, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_u_Response_header_must_be_a_MP_MAP); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(5, 337, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "asynctnt/iproto/response.pyx":343
  *     for _ in range(size):
  *         if mp_typeof(b[0]) != MP_UINT:  # pragma: nocover
  *             raise TypeError('Header key must be a MP_UINT')             # <<<<<<<<<<<<<<
  * 
  *         key = mp_decode_uint(&b)
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_u_Header_key_must_be_a_MP_UINT); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(5, 343, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_u_Header_key_must_be_a_MP_UINT); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(5, 343, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "asynctnt/iproto/response.pyx":348
  *         if key == tarantool.IPROTO_REQUEST_TYPE:
  *             if mp_typeof(b[0]) != MP_UINT:  # pragma: nocover
  *                 raise TypeError('code type must be a MP_UINT')             # <<<<<<<<<<<<<<
  * 
  *             hdr.code = <uint32_t> mp_decode_uint(&b)
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_u_code_type_must_be_a_MP_UINT); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(5, 348, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_u_code_type_must_be_a_MP_UINT); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(5, 348, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "asynctnt/iproto/response.pyx":354
  *         elif key == tarantool.IPROTO_SYNC:
  *             if mp_typeof(b[0]) != MP_UINT:  # pragma: nocover
  *                 raise TypeError('sync type must be a MP_UINT')             # <<<<<<<<<<<<<<
  * 
  *             hdr.sync = mp_decode_uint(&b)
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_u_sync_type_must_be_a_MP_UINT); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(5, 354, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_u_sync_type_must_be_a_MP_UINT); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(5, 354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "asynctnt/iproto/response.pyx":359
  *         elif key == tarantool.IPROTO_SCHEMA_VERSION:
  *             if mp_typeof(b[0]) != MP_UINT:  # pragma: nocover
  *                 raise TypeError('schema_id type must be a MP_UINT')             # <<<<<<<<<<<<<<
  * 
  *             hdr.schema_id = mp_decode_uint(&b)
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_u_schema_id_type_must_be_a_MP_UINT); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(5, 359, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_u_schema_id_type_must_be_a_MP_UINT); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(5, 359, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "asynctnt/iproto/response.pyx":385
  *         field_map_size = mp_decode_map(b)
  *         if field_map_size == 0:  # pragma: nocover
  *             raise RuntimeError('Field map must contain at least '             # <<<<<<<<<<<<<<
  *                                '1 element - field_name')
  * 
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_u_Field_map_must_contain_at_least); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(5, 385, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_u_Field_map_must_contain_at_least); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(5, 385, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "asynctnt/iproto/response.pyx":432
  * 
  *                 else:  # pragma: nocover
  *                     raise TypeError(             # <<<<<<<<<<<<<<
  *                         "IPROTO_FIELD_SPAN must be either STR or NIL"
  *                     )
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_u_IPROTO_FIELD_SPAN_must_be_either); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(5, 432, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_u_IPROTO_FIELD_SPAN_must_be_either); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(5, 432, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "asynctnt/iproto/response.pyx":441
  * 
  *         if field.name is None:  # pragma: nocover
  *             raise RuntimeError('field.name must not be None')             # <<<<<<<<<<<<<<
  * 
  *         metadata.add(<int> field_id, field)
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_u_field_name_must_not_be_None); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(5, 441, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_u_field_name_must_not_be_None); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(5, 441, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "asynctnt/iproto/response.pyx":557
  * 
  *     if mp_typeof(b[0]) != MP_MAP:  # pragma: nocover
  *         raise TypeError('Response body must be a MP_MAP')             # <<<<<<<<<<<<<<
  * 
  *     size = mp_decode_map(&b)
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_u_Response_body_must_be_a_MP_MAP); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(5, 557, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_u_Response_body_must_be_a_MP_MAP); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(5, 557, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
 
   /* "asynctnt/iproto/response.pyx":567
  *         if key == tarantool.IPROTO_ERROR_24:
  *             if mp_typeof(b[0]) != MP_STR:  # pragma: nocover
  *                 raise TypeError('errstr type must be a MP_STR')             # <<<<<<<<<<<<<<
  * 
  *             s = NULL
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_u_errstr_type_must_be_a_MP_STR); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(5, 567, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_u_errstr_type_must_be_a_MP_STR); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(5, 567, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
 
   /* "asynctnt/iproto/response.pyx":576
  *         elif key == tarantool.IPROTO_ERROR:
  *             if mp_typeof(b[0]) != MP_MAP:  # pragma: nocover
  *                 raise TypeError('IPROTO_ERROR type must be a MP_MAP')             # <<<<<<<<<<<<<<
  * 
  *             resp.error = parse_iproto_error(&b, resp.encoding)
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_u_IPROTO_ERROR_type_must_be_a_MP_M); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(5, 576, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_u_IPROTO_ERROR_type_must_be_a_MP_M); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(5, 576, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "asynctnt/iproto/response.pyx":606
  *             field_map_size = mp_decode_map(&b)
  *             if field_map_size == 0:
  *                 raise RuntimeError('Field map must contain at least '             # <<<<<<<<<<<<<<
  *                                    '1 element - rowcount')
  * 
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_u_Field_map_must_contain_at_least_2); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(5, 606, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_u_Field_map_must_contain_at_least_2); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(5, 606, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
 
   /* "asynctnt/iproto/response.pyx":627
  *         elif key == tarantool.IPROTO_DATA:
  *             if mp_typeof(b[0]) != MP_ARRAY:  # pragma: nocover
  *                 raise TypeError('body data type must be a MP_ARRAY')             # <<<<<<<<<<<<<<
  *             data = _response_parse_body_data(&b, resp, req)
  *             if is_chunk:
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_u_body_data_type_must_be_a_MP_ARRA); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(5, 627, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_u_body_data_type_must_be_a_MP_ARRA); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(5, 627, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
 
   /* "asynctnt/iproto/db.pyx":252
  *             req.statement_id = <uint64_t> query
  *         else:
  *             raise TypeError('query must be either str or int')             # <<<<<<<<<<<<<<
  * 
  *         req.args = args
  */
-  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_u_query_must_be_either_str_or_int); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(26, 252, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_u_query_must_be_either_str_or_int); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(26, 252, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
 
   /* "asynctnt/iproto/push.pyx":37
  *             BaseRequest request
  *         if not hasattr(fut, '_response'):
  *             raise ValueError('Future is invalid. Make sure to call with '             # <<<<<<<<<<<<<<
  *                              'a future returned from a method with '
  *                              'push_subscribe=True flag')
  */
-  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_u_Future_is_invalid_Make_sure_to_c); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(27, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_u_Future_is_invalid_Make_sure_to_c); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(27, 37, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
 
   /* "asynctnt/iproto/push.pyx":54
  * 
  *     def __iter__(self):
  *         raise RuntimeError('Cannot use iter with PushIterator - use aiter')             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
-  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_u_Cannot_use_iter_with_PushIterato); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(27, 54, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_u_Cannot_use_iter_with_PushIterato); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(27, 54, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
 
   /* "asynctnt/iproto/push.pyx":57
  * 
  *     def __next__(self):
  *         raise RuntimeError('Cannot use next with PushIterator - use anext')             # <<<<<<<<<<<<<<
  * 
  *     def __aiter__(self):
  */
-  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_u_Cannot_use_next_with_PushIterato); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(27, 57, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__38);
-  __Pyx_GIVEREF(__pyx_tuple__38);
+  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_u_Cannot_use_next_with_PushIterato); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(27, 57, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
 
   /* "asynctnt/iproto/coreproto.pyx":32
  *             self.encoding = encoding
  *         else:
  *             raise TypeError('encoding must be either str or bytes')             # <<<<<<<<<<<<<<
  * 
  *         initial_read_buffer_size = initial_read_buffer_size or 0x20000
  */
-  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_u_encoding_must_be_either_str_or_b); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(28, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__39);
-  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_u_encoding_must_be_either_str_or_b); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(28, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__38);
+  __Pyx_GIVEREF(__pyx_tuple__38);
 
   /* "asynctnt/iproto/coreproto.pyx":139
  *             self.rbuf.get_slice(ver_length,
  *                                 ver_length + SALT_LENGTH)
  *         )[:SCRAMBLE_SIZE]             # <<<<<<<<<<<<<<
  *         self.state = PROTOCOL_NORMAL
  *         self._on_greeting_received()
  */
-  __pyx_slice__40 = PySlice_New(Py_None, __pyx_int_20, Py_None); if (unlikely(!__pyx_slice__40)) __PYX_ERR(28, 139, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__40);
-  __Pyx_GIVEREF(__pyx_slice__40);
+  __pyx_slice__39 = PySlice_New(Py_None, __pyx_int_20, Py_None); if (unlikely(!__pyx_slice__39)) __PYX_ERR(28, 139, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__39);
+  __Pyx_GIVEREF(__pyx_slice__39);
 
   /* "asynctnt/iproto/protocol.pyx":139
  *         if self.post_con_state == POST_CONNECTION_ID:
  *             assert self.version is not None
  *             if self.version >= (2, 10, 0):             # <<<<<<<<<<<<<<
  *                 # send <id> request
  *                 self._do_id()
  */
-  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_int_2, __pyx_int_10, __pyx_int_0); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(6, 139, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__41);
-  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_tuple__40 = PyTuple_Pack(3, __pyx_int_2, __pyx_int_10, __pyx_int_0); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(6, 139, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
 
   /* "asynctnt/iproto/protocol.pyx":250
  *         fut = self._db._id(0.0)
  * 
  *         def on_id(f):             # <<<<<<<<<<<<<<
  *             if f.cancelled():
  *                 self._set_connection_error(asyncio.futures.CancelledError())
  */
-  __pyx_tuple__42 = PyTuple_Pack(2, __pyx_n_s_f, __pyx_n_s_e); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(6, 250, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__42);
-  __Pyx_GIVEREF(__pyx_tuple__42);
-  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_on_id, 250, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(6, 250, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(2, __pyx_n_s_f, __pyx_n_s_e); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(6, 250, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_on_id, 250, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(6, 250, __pyx_L1_error)
 
   /* "asynctnt/iproto/protocol.pyx":272
  *         fut = self._db._auth(self.salt, username, password, 0)
  * 
  *         def on_authorized(f):             # <<<<<<<<<<<<<<
  *             if f.cancelled():
  *                 self._set_connection_error(asyncio.futures.CancelledError())
  */
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_on_authorized, 272, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(6, 272, __pyx_L1_error)
+  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_on_authorized, 272, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(6, 272, __pyx_L1_error)
 
   /* "asynctnt/iproto/protocol.pyx":296
  *         self._schema_fetch_in_progress = True
  * 
  *         def on_fetch(f):             # <<<<<<<<<<<<<<
  *             self._schema_fetch_in_progress = False
  * 
  */
-  __pyx_tuple__45 = PyTuple_Pack(4, __pyx_n_s_f, __pyx_n_s_e, __pyx_n_s_spaces, __pyx_n_s_indexes); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(6, 296, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__45);
-  __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_on_fetch, 296, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(6, 296, __pyx_L1_error)
+  __pyx_tuple__44 = PyTuple_Pack(4, __pyx_n_s_f, __pyx_n_s_e, __pyx_n_s_spaces, __pyx_n_s_indexes); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(6, 296, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__44);
+  __Pyx_GIVEREF(__pyx_tuple__44);
+  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_on_fetch, 296, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(6, 296, __pyx_L1_error)
 
   /* "asynctnt/iproto/protocol.pyx":349
  *                     fut.set_exception(e)
  * 
  *         fut_vspace = self._db.select(SPACE_VSPACE, timeout=0,             # <<<<<<<<<<<<<<
  *                                      check_schema_change=False)
  *         fut_vindex = self._db.select(SPACE_VINDEX, timeout=0,
  */
-  __pyx_tuple__47 = PyTuple_Pack(1, __pyx_int_281); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(6, 349, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__47);
-  __Pyx_GIVEREF(__pyx_tuple__47);
+  __pyx_tuple__46 = PyTuple_Pack(1, __pyx_int_281); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(6, 349, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__46);
+  __Pyx_GIVEREF(__pyx_tuple__46);
 
   /* "asynctnt/iproto/protocol.pyx":351
  *         fut_vspace = self._db.select(SPACE_VSPACE, timeout=0,
  *                                      check_schema_change=False)
  *         fut_vindex = self._db.select(SPACE_VINDEX, timeout=0,             # <<<<<<<<<<<<<<
  *                                      check_schema_change=False)
  *         gather_fut = asyncio.gather(fut_vspace, fut_vindex,
  */
-  __pyx_tuple__48 = PyTuple_Pack(1, __pyx_int_289); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(6, 351, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__48);
-  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_tuple__47 = PyTuple_Pack(1, __pyx_int_289); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(6, 351, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__47);
+  __Pyx_GIVEREF(__pyx_tuple__47);
 
   /* "asynctnt/iproto/protocol.pyx":502
  *             return Iterator[iterator]
  *         else:
  *             raise TypeError('Iterator is of unsupported type '             # <<<<<<<<<<<<<<
  *                             '(asynctnt.Iterator, int, str)')
  * 
  */
-  __pyx_tuple__49 = PyTuple_Pack(1, __pyx_kp_u_Iterator_is_of_unsupported_type); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(6, 502, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__49);
-  __Pyx_GIVEREF(__pyx_tuple__49);
+  __pyx_tuple__48 = PyTuple_Pack(1, __pyx_kp_u_Iterator_is_of_unsupported_type); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(6, 502, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__48);
+  __Pyx_GIVEREF(__pyx_tuple__48);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x9001016, 0xc05ea8e, 0xfe5f18a):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9001016, 0xc05ea8e, 0xfe5f18a) = (check_schema_change, op, parse_as_tuples, parse_metadata, push_subscribe, schema_id, space, stream_id, sync, timeout_handle, waiter))" % __pyx_checksum
  */
-  __pyx_tuple__50 = PyTuple_Pack(3, __pyx_int_150999062, __pyx_int_201714318, __pyx_int_266727818); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__49 = PyTuple_Pack(3, __pyx_int_150999062, __pyx_int_201714318, __pyx_int_266727818); if (unlikely(!__pyx_tuple__49)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__49);
+  __Pyx_GIVEREF(__pyx_tuple__49);
+  __pyx_tuple__50 = PyTuple_Pack(3, __pyx_int_47556637, __pyx_int_180945731, __pyx_int_215610203); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__50);
   __Pyx_GIVEREF(__pyx_tuple__50);
-  __pyx_tuple__51 = PyTuple_Pack(3, __pyx_int_47556637, __pyx_int_180945731, __pyx_int_215610203); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__51 = PyTuple_Pack(3, __pyx_int_184220263, __pyx_int_63007895, __pyx_int_151261227); if (unlikely(!__pyx_tuple__51)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__51);
   __Pyx_GIVEREF(__pyx_tuple__51);
-  __pyx_tuple__52 = PyTuple_Pack(3, __pyx_int_184220263, __pyx_int_63007895, __pyx_int_151261227); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(3, __pyx_int_149085227, __pyx_int_103773939, __pyx_int_92266676); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__52);
   __Pyx_GIVEREF(__pyx_tuple__52);
-  __pyx_tuple__53 = PyTuple_Pack(3, __pyx_int_149085227, __pyx_int_103773939, __pyx_int_92266676); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__53 = PyTuple_Pack(3, __pyx_int_194105842, __pyx_int_267485924, __pyx_int_23039357); if (unlikely(!__pyx_tuple__53)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__53);
   __Pyx_GIVEREF(__pyx_tuple__53);
-  __pyx_tuple__54 = PyTuple_Pack(3, __pyx_int_194105842, __pyx_int_267485924, __pyx_int_23039357); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__54 = PyTuple_Pack(3, __pyx_int_255344631, __pyx_int_145510168, __pyx_int_244856512); if (unlikely(!__pyx_tuple__54)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__54);
   __Pyx_GIVEREF(__pyx_tuple__54);
-  __pyx_tuple__55 = PyTuple_Pack(3, __pyx_int_255344631, __pyx_int_145510168, __pyx_int_244856512); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__55 = PyTuple_Pack(3, __pyx_int_135652490, __pyx_int_145344315, __pyx_int_25165850); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__55);
   __Pyx_GIVEREF(__pyx_tuple__55);
-  __pyx_tuple__56 = PyTuple_Pack(3, __pyx_int_135652490, __pyx_int_145344315, __pyx_int_25165850); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__56 = PyTuple_Pack(3, __pyx_int_209859363, __pyx_int_245819509, __pyx_int_4796468); if (unlikely(!__pyx_tuple__56)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__56);
   __Pyx_GIVEREF(__pyx_tuple__56);
-  __pyx_tuple__57 = PyTuple_Pack(3, __pyx_int_209859363, __pyx_int_245819509, __pyx_int_4796468); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__57 = PyTuple_Pack(3, __pyx_int_218707107, __pyx_int_214473120, __pyx_int_129177485); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__57);
   __Pyx_GIVEREF(__pyx_tuple__57);
-  __pyx_tuple__58 = PyTuple_Pack(3, __pyx_int_218707107, __pyx_int_214473120, __pyx_int_129177485); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__58 = PyTuple_Pack(3, __pyx_int_51694216, __pyx_int_105824685, __pyx_int_220368800); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__58);
   __Pyx_GIVEREF(__pyx_tuple__58);
-  __pyx_tuple__59 = PyTuple_Pack(3, __pyx_int_51694216, __pyx_int_105824685, __pyx_int_220368800); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__59 = PyTuple_Pack(3, __pyx_int_53862661, __pyx_int_257562521, __pyx_int_170745181); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__59);
   __Pyx_GIVEREF(__pyx_tuple__59);
-  __pyx_tuple__60 = PyTuple_Pack(3, __pyx_int_53862661, __pyx_int_257562521, __pyx_int_170745181); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__60 = PyTuple_Pack(3, __pyx_int_51353055, __pyx_int_172954204, __pyx_int_264852134); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__60);
   __Pyx_GIVEREF(__pyx_tuple__60);
-  __pyx_tuple__61 = PyTuple_Pack(3, __pyx_int_51353055, __pyx_int_172954204, __pyx_int_264852134); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__61 = PyTuple_Pack(3, __pyx_int_179467967, __pyx_int_192862663, __pyx_int_105088600); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__61);
   __Pyx_GIVEREF(__pyx_tuple__61);
-  __pyx_tuple__62 = PyTuple_Pack(3, __pyx_int_179467967, __pyx_int_192862663, __pyx_int_105088600); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__62 = PyTuple_Pack(3, __pyx_int_246409365, __pyx_int_219129172, __pyx_int_4879619); if (unlikely(!__pyx_tuple__62)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__62);
   __Pyx_GIVEREF(__pyx_tuple__62);
-  __pyx_tuple__63 = PyTuple_Pack(3, __pyx_int_246409365, __pyx_int_219129172, __pyx_int_4879619); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__63 = PyTuple_Pack(3, __pyx_int_159463343, __pyx_int_196154451, __pyx_int_225261924); if (unlikely(!__pyx_tuple__63)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__63);
   __Pyx_GIVEREF(__pyx_tuple__63);
-  __pyx_tuple__64 = PyTuple_Pack(3, __pyx_int_159463343, __pyx_int_196154451, __pyx_int_225261924); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__64 = PyTuple_Pack(3, __pyx_int_144520718, __pyx_int_235564716, __pyx_int_253265777); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__64);
   __Pyx_GIVEREF(__pyx_tuple__64);
-  __pyx_tuple__65 = PyTuple_Pack(3, __pyx_int_144520718, __pyx_int_235564716, __pyx_int_253265777); if (unlikely(!__pyx_tuple__65)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__65);
-  __Pyx_GIVEREF(__pyx_tuple__65);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_tuple__67 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__67)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__67);
-  __Pyx_GIVEREF(__pyx_tuple__67);
-  __pyx_codeobj__68 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__68)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_tuple__66 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__66)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__66);
+  __Pyx_GIVEREF(__pyx_tuple__66);
+  __pyx_codeobj__67 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__67)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_tuple__69 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__69)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__69);
-  __Pyx_GIVEREF(__pyx_tuple__69);
-  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_tuple__68 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__68)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__68);
+  __Pyx_GIVEREF(__pyx_tuple__68);
+  __pyx_codeobj__69 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__69)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__71 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__71)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__70 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__70)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__72 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__72)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__71 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__71)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__73 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__73)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__72 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__72)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__74 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__74)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__73 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__73)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__75 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__75)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__74 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__74)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__75 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__75)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__76 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__76)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__78 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__78)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__77 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__77)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "asynctnt/iproto/buffer.pyx":54
  *         self._view_count -= 1
  * 
  *     def hex(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return ":".join("{:02x}".format(ord(<bytes> (self._buf[i])))
  *                         for i in range(self._length))
  */
-  __pyx_tuple__79 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__79)) __PYX_ERR(3, 54, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__79);
-  __Pyx_GIVEREF(__pyx_tuple__79);
-  __pyx_codeobj__80 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__79, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_buffer_pyx, __pyx_n_s_hex, 54, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__80)) __PYX_ERR(3, 54, __pyx_L1_error)
+  __pyx_tuple__78 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__78)) __PYX_ERR(3, 54, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__78);
+  __Pyx_GIVEREF(__pyx_tuple__78);
+  __pyx_codeobj__79 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__78, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_buffer_pyx, __pyx_n_s_hex, 54, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__79)) __PYX_ERR(3, 54, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__81 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__81)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__80 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__80)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__82 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__82)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__81 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__81)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__83 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__83)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__82 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__82)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__84 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__84)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__83 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__83)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_tuple__85 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__85)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__85);
-  __Pyx_GIVEREF(__pyx_tuple__85);
-  __pyx_codeobj__86 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__86)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_tuple__84 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__84)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__84);
+  __Pyx_GIVEREF(__pyx_tuple__84);
+  __pyx_codeobj__85 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__85)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_BaseRequest, (type(self), 0x9001016, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_BaseRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__87 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__87)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__86 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__86)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__88 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__88)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__87 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__87)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_PingRequest, (type(self), 0x9001016, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_PingRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__88 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__88)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__90 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__90)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_CallRequest, (type(self), 0x2d5a81d, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_CallRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__91 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__91)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__90 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__90)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__92 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__92)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__91 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__91)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_EvalRequest, (type(self), 0xafafa67, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_EvalRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__93 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__93)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__92 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__92)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__94 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__94)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__93 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__93)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_SelectRequest, (type(self), 0x8e2dc2b, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_SelectRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__95 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__95)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__94 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__94)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__96 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__96)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__95 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__95)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_InsertRequest, (type(self), 0xb91d1f2, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_InsertRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__97 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__97)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__96 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__96)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__97 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__97)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_DeleteRequest, (type(self), 0xf383ff7, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_DeleteRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__99 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__99)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__100 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__100)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__99 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__99)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_UpdateRequest, (type(self), 0x815e48a, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_UpdateRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__101 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__101)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__100 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__100)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__102 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__102)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__101 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__101)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_UpsertRequest, (type(self), 0xc823323, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_UpsertRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__103 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__103)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__102 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__102)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__104 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__104)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__103 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__103)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_PrepareRequest, (type(self), 0xd0934a3, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_PrepareRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__105 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__105)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__104 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__104)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__106 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__106)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__105 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__105)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_ExecuteRequest, (type(self), 0x314ca88, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_ExecuteRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__107 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__107)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__106 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__106)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__108 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__108)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__107 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__107)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_IDRequest, (type(self), 0x9001016, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_IDRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__109 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__109)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__108 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__108)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__110 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__110)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__109 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__109)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_AuthRequest, (type(self), 0x335e105, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_AuthRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__111 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__111)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__110 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__110)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__112 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__112)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__111 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__111)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_BeginRequest, (type(self), 0x30f95df, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_BeginRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__113 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__113)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__112 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__112)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__114 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__114)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__113 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__113)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_CommitRequest, (type(self), 0x9001016, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_CommitRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__115 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__115)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__114 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__114)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__116 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__116)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__115 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__115)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_RollbackRequest, (type(self), 0x9001016, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_RollbackRequest__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__117 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__117)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__116 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__116)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__118 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__118)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__117 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__117)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_IProtoErrorStackFrame, (type(self), 0xab276bf, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_IProtoErrorStackFrame__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__119 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__119)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__118 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__118)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__120 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__120)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__119 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__119)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_IProtoError, (type(self), 0xeafe895, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_IProtoError__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__121 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__121)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__120 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__120)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "asynctnt/iproto/response.pyx":160
  *         return self.stmt_id_
  * 
  *     def done(self):             # <<<<<<<<<<<<<<
  *         return self.code_ >= 0
  * 
  */
-  __pyx_codeobj__122 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_response_pyx, __pyx_n_s_done, 160, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__122)) __PYX_ERR(5, 160, __pyx_L1_error)
+  __pyx_codeobj__121 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_response_pyx, __pyx_n_s_done, 160, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__121)) __PYX_ERR(5, 160, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__123 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__123)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__122 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__122)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__124 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__124)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__123 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__123)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "asynctnt/iproto/db.pyx":327
  *         return <int> self._stream_id
  * 
  *     def set_stream_id(self, int stream_id):             # <<<<<<<<<<<<<<
  *         self._stream_id = <uint64_t> stream_id
  * 
  */
-  __pyx_tuple__125 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_stream_id); if (unlikely(!__pyx_tuple__125)) __PYX_ERR(26, 327, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__125);
-  __Pyx_GIVEREF(__pyx_tuple__125);
-  __pyx_codeobj__126 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__125, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_set_stream_id, 327, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__126)) __PYX_ERR(26, 327, __pyx_L1_error)
+  __pyx_tuple__124 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_stream_id); if (unlikely(!__pyx_tuple__124)) __PYX_ERR(26, 327, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__124);
+  __Pyx_GIVEREF(__pyx_tuple__124);
+  __pyx_codeobj__125 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__124, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_set_stream_id, 327, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__125)) __PYX_ERR(26, 327, __pyx_L1_error)
 
   /* "asynctnt/iproto/db.pyx":330
  *         self._stream_id = <uint64_t> stream_id
  * 
  *     def ping(self, float timeout=-1):             # <<<<<<<<<<<<<<
  *         return self._ping(timeout)
  * 
  */
-  __pyx_tuple__127 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__127)) __PYX_ERR(26, 330, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__127);
-  __Pyx_GIVEREF(__pyx_tuple__127);
-  __pyx_codeobj__128 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__127, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_ping, 330, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__128)) __PYX_ERR(26, 330, __pyx_L1_error)
-  __pyx_tuple__129 = PyTuple_Pack(1, __pyx_float_neg_1_0); if (unlikely(!__pyx_tuple__129)) __PYX_ERR(26, 330, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__129);
-  __Pyx_GIVEREF(__pyx_tuple__129);
+  __pyx_tuple__126 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__126)) __PYX_ERR(26, 330, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__126);
+  __Pyx_GIVEREF(__pyx_tuple__126);
+  __pyx_codeobj__127 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__126, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_ping, 330, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__127)) __PYX_ERR(26, 330, __pyx_L1_error)
+  __pyx_tuple__128 = PyTuple_Pack(1, __pyx_float_neg_1_0); if (unlikely(!__pyx_tuple__128)) __PYX_ERR(26, 330, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__128);
+  __Pyx_GIVEREF(__pyx_tuple__128);
 
   /* "asynctnt/iproto/db.pyx":333
  *         return self._ping(timeout)
  * 
  *     def call16(self,             # <<<<<<<<<<<<<<
  *                str func_name,
  *                object args=None,
  */
-  __pyx_tuple__130 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_func_name, __pyx_n_s_args, __pyx_n_s_timeout, __pyx_n_s_push_subscribe); if (unlikely(!__pyx_tuple__130)) __PYX_ERR(26, 333, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__130);
-  __Pyx_GIVEREF(__pyx_tuple__130);
-  __pyx_codeobj__131 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__130, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_call16, 333, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__131)) __PYX_ERR(26, 333, __pyx_L1_error)
-  __pyx_tuple__132 = PyTuple_Pack(3, Py_None, __pyx_float_neg_1_0, Py_False); if (unlikely(!__pyx_tuple__132)) __PYX_ERR(26, 333, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__132);
-  __Pyx_GIVEREF(__pyx_tuple__132);
+  __pyx_tuple__129 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_func_name, __pyx_n_s_args, __pyx_n_s_timeout, __pyx_n_s_push_subscribe); if (unlikely(!__pyx_tuple__129)) __PYX_ERR(26, 333, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__129);
+  __Pyx_GIVEREF(__pyx_tuple__129);
+  __pyx_codeobj__130 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__129, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_call16, 333, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__130)) __PYX_ERR(26, 333, __pyx_L1_error)
+  __pyx_tuple__131 = PyTuple_Pack(3, Py_None, __pyx_float_neg_1_0, Py_False); if (unlikely(!__pyx_tuple__131)) __PYX_ERR(26, 333, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__131);
+  __Pyx_GIVEREF(__pyx_tuple__131);
 
   /* "asynctnt/iproto/db.pyx":344
  *                           <bint> push_subscribe)
  * 
  *     def call(self,             # <<<<<<<<<<<<<<
  *              str func_name,
  *              object args=None,
  */
-  __pyx_codeobj__133 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__130, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_call, 344, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__133)) __PYX_ERR(26, 344, __pyx_L1_error)
+  __pyx_codeobj__132 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__129, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_call, 344, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__132)) __PYX_ERR(26, 344, __pyx_L1_error)
 
   /* "asynctnt/iproto/db.pyx":355
  *                           <bint> push_subscribe)
  * 
  *     def eval(self,             # <<<<<<<<<<<<<<
  *              str expression,
  *              object args=None,
  */
-  __pyx_tuple__134 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_expression, __pyx_n_s_args, __pyx_n_s_timeout, __pyx_n_s_push_subscribe); if (unlikely(!__pyx_tuple__134)) __PYX_ERR(26, 355, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__134);
-  __Pyx_GIVEREF(__pyx_tuple__134);
-  __pyx_codeobj__135 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__134, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_eval, 355, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__135)) __PYX_ERR(26, 355, __pyx_L1_error)
+  __pyx_tuple__133 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_expression, __pyx_n_s_args, __pyx_n_s_timeout, __pyx_n_s_push_subscribe); if (unlikely(!__pyx_tuple__133)) __PYX_ERR(26, 355, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__133);
+  __Pyx_GIVEREF(__pyx_tuple__133);
+  __pyx_codeobj__134 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__133, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_eval, 355, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__134)) __PYX_ERR(26, 355, __pyx_L1_error)
 
   /* "asynctnt/iproto/db.pyx":365
  *                           <bint> push_subscribe)
  * 
  *     def select(self,             # <<<<<<<<<<<<<<
  *                object space,
  *                object key=None,
  */
-  __pyx_tuple__136 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_key, __pyx_n_s_offset, __pyx_n_s_limit, __pyx_n_s_index, __pyx_n_s_iterator, __pyx_n_s_timeout, __pyx_n_s_check_schema_change); if (unlikely(!__pyx_tuple__136)) __PYX_ERR(26, 365, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__136);
-  __Pyx_GIVEREF(__pyx_tuple__136);
-  __pyx_codeobj__137 = (PyObject*)__Pyx_PyCode_New(9, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__136, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_select, 365, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__137)) __PYX_ERR(26, 365, __pyx_L1_error)
-  __pyx_tuple__138 = PyTuple_Pack(7, Py_None, __pyx_int_0, __pyx_int_4294967295, __pyx_int_0, __pyx_int_0, __pyx_float_neg_1_0, Py_True); if (unlikely(!__pyx_tuple__138)) __PYX_ERR(26, 365, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__138);
-  __Pyx_GIVEREF(__pyx_tuple__138);
+  __pyx_tuple__135 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_key, __pyx_n_s_offset, __pyx_n_s_limit, __pyx_n_s_index, __pyx_n_s_iterator, __pyx_n_s_timeout, __pyx_n_s_check_schema_change); if (unlikely(!__pyx_tuple__135)) __PYX_ERR(26, 365, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__135);
+  __Pyx_GIVEREF(__pyx_tuple__135);
+  __pyx_codeobj__136 = (PyObject*)__Pyx_PyCode_New(9, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__135, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_select, 365, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__136)) __PYX_ERR(26, 365, __pyx_L1_error)
+  __pyx_tuple__137 = PyTuple_Pack(7, Py_None, __pyx_int_0, __pyx_int_4294967295, __pyx_int_0, __pyx_int_0, __pyx_float_neg_1_0, Py_True); if (unlikely(!__pyx_tuple__137)) __PYX_ERR(26, 365, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__137);
+  __Pyx_GIVEREF(__pyx_tuple__137);
 
   /* "asynctnt/iproto/db.pyx":377
  *                             timeout, check_schema_change)
  * 
  *     def insert(self,             # <<<<<<<<<<<<<<
  *                object space,
  *                object t,
  */
-  __pyx_tuple__139 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_t, __pyx_n_s_replace, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__139)) __PYX_ERR(26, 377, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__139);
-  __Pyx_GIVEREF(__pyx_tuple__139);
-  __pyx_codeobj__140 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__139, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_insert, 377, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__140)) __PYX_ERR(26, 377, __pyx_L1_error)
-  __pyx_tuple__141 = PyTuple_Pack(2, Py_False, __pyx_float_neg_1_0); if (unlikely(!__pyx_tuple__141)) __PYX_ERR(26, 377, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__141);
-  __Pyx_GIVEREF(__pyx_tuple__141);
+  __pyx_tuple__138 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_t, __pyx_n_s_replace, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__138)) __PYX_ERR(26, 377, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__138);
+  __Pyx_GIVEREF(__pyx_tuple__138);
+  __pyx_codeobj__139 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__138, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_insert, 377, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__139)) __PYX_ERR(26, 377, __pyx_L1_error)
+  __pyx_tuple__140 = PyTuple_Pack(2, Py_False, __pyx_float_neg_1_0); if (unlikely(!__pyx_tuple__140)) __PYX_ERR(26, 377, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__140);
+  __Pyx_GIVEREF(__pyx_tuple__140);
 
   /* "asynctnt/iproto/db.pyx":384
  *         return self._insert(space, t, <bint> replace, timeout)
  * 
  *     def replace(self,             # <<<<<<<<<<<<<<
  *                 object space,
  *                 object t,
  */
-  __pyx_tuple__142 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_t, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__142)) __PYX_ERR(26, 384, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__142);
-  __Pyx_GIVEREF(__pyx_tuple__142);
-  __pyx_codeobj__143 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__142, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_replace, 384, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__143)) __PYX_ERR(26, 384, __pyx_L1_error)
+  __pyx_tuple__141 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_t, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__141)) __PYX_ERR(26, 384, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__141);
+  __Pyx_GIVEREF(__pyx_tuple__141);
+  __pyx_codeobj__142 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__141, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_replace, 384, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__142)) __PYX_ERR(26, 384, __pyx_L1_error)
 
   /* "asynctnt/iproto/db.pyx":390
  *         return self._insert(space, t, <bint> True, timeout)
  * 
  *     def delete(self,             # <<<<<<<<<<<<<<
  *                object space,
  *                object key,
  */
-  __pyx_tuple__144 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_key, __pyx_n_s_index, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__144)) __PYX_ERR(26, 390, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__144);
-  __Pyx_GIVEREF(__pyx_tuple__144);
-  __pyx_codeobj__145 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__144, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_delete, 390, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__145)) __PYX_ERR(26, 390, __pyx_L1_error)
-  __pyx_tuple__146 = PyTuple_Pack(2, __pyx_int_0, __pyx_float_neg_1_0); if (unlikely(!__pyx_tuple__146)) __PYX_ERR(26, 390, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__146);
-  __Pyx_GIVEREF(__pyx_tuple__146);
+  __pyx_tuple__143 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_key, __pyx_n_s_index, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__143)) __PYX_ERR(26, 390, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__143);
+  __Pyx_GIVEREF(__pyx_tuple__143);
+  __pyx_codeobj__144 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__143, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_delete, 390, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__144)) __PYX_ERR(26, 390, __pyx_L1_error)
+  __pyx_tuple__145 = PyTuple_Pack(2, __pyx_int_0, __pyx_float_neg_1_0); if (unlikely(!__pyx_tuple__145)) __PYX_ERR(26, 390, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__145);
+  __Pyx_GIVEREF(__pyx_tuple__145);
 
   /* "asynctnt/iproto/db.pyx":397
  *         return self._delete(space, index, key, timeout)
  * 
  *     def update(self,             # <<<<<<<<<<<<<<
  *                object space,
  *                object key,
  */
-  __pyx_tuple__147 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_key, __pyx_n_s_operations, __pyx_n_s_index, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__147)) __PYX_ERR(26, 397, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__147);
-  __Pyx_GIVEREF(__pyx_tuple__147);
-  __pyx_codeobj__148 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__147, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_update, 397, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__148)) __PYX_ERR(26, 397, __pyx_L1_error)
+  __pyx_tuple__146 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_key, __pyx_n_s_operations, __pyx_n_s_index, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__146)) __PYX_ERR(26, 397, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__146);
+  __Pyx_GIVEREF(__pyx_tuple__146);
+  __pyx_codeobj__147 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__146, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_update, 397, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__147)) __PYX_ERR(26, 397, __pyx_L1_error)
 
   /* "asynctnt/iproto/db.pyx":405
  *         return self._update(space, index, key, operations, timeout)
  * 
  *     def upsert(self,             # <<<<<<<<<<<<<<
  *                object space,
  *                object t,
  */
-  __pyx_tuple__149 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_t, __pyx_n_s_operations, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__149)) __PYX_ERR(26, 405, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__149);
-  __Pyx_GIVEREF(__pyx_tuple__149);
-  __pyx_codeobj__150 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__149, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_upsert, 405, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__150)) __PYX_ERR(26, 405, __pyx_L1_error)
+  __pyx_tuple__148 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_space, __pyx_n_s_t, __pyx_n_s_operations, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__148)) __PYX_ERR(26, 405, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__148);
+  __Pyx_GIVEREF(__pyx_tuple__148);
+  __pyx_codeobj__149 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__148, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_upsert, 405, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__149)) __PYX_ERR(26, 405, __pyx_L1_error)
 
   /* "asynctnt/iproto/db.pyx":412
  *         return self._upsert(space, t, operations, timeout)
  * 
  *     def execute(self,             # <<<<<<<<<<<<<<
  *                 object query,
  *                 object args,
  */
-  __pyx_tuple__151 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_query, __pyx_n_s_args, __pyx_n_s_parse_metadata, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__151)) __PYX_ERR(26, 412, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__151);
-  __Pyx_GIVEREF(__pyx_tuple__151);
-  __pyx_codeobj__152 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__151, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_execute, 412, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__152)) __PYX_ERR(26, 412, __pyx_L1_error)
-  __pyx_tuple__153 = PyTuple_Pack(2, Py_True, __pyx_float_neg_1_0); if (unlikely(!__pyx_tuple__153)) __PYX_ERR(26, 412, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__153);
-  __Pyx_GIVEREF(__pyx_tuple__153);
+  __pyx_tuple__150 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_query, __pyx_n_s_args, __pyx_n_s_parse_metadata, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__150)) __PYX_ERR(26, 412, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__150);
+  __Pyx_GIVEREF(__pyx_tuple__150);
+  __pyx_codeobj__151 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__150, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_execute, 412, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__151)) __PYX_ERR(26, 412, __pyx_L1_error)
+  __pyx_tuple__152 = PyTuple_Pack(2, Py_True, __pyx_float_neg_1_0); if (unlikely(!__pyx_tuple__152)) __PYX_ERR(26, 412, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__152);
+  __Pyx_GIVEREF(__pyx_tuple__152);
 
   /* "asynctnt/iproto/db.pyx":419
  *         return self._execute(query, args, <bint> parse_metadata, timeout)
  * 
  *     def prepare(self,             # <<<<<<<<<<<<<<
  *                 object query,
  *                 bint parse_metadata=True,
  */
-  __pyx_tuple__154 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_query, __pyx_n_s_parse_metadata, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__154)) __PYX_ERR(26, 419, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__154);
-  __Pyx_GIVEREF(__pyx_tuple__154);
-  __pyx_codeobj__155 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__154, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_prepare, 419, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__155)) __PYX_ERR(26, 419, __pyx_L1_error)
+  __pyx_tuple__153 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_query, __pyx_n_s_parse_metadata, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__153)) __PYX_ERR(26, 419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__153);
+  __Pyx_GIVEREF(__pyx_tuple__153);
+  __pyx_codeobj__154 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__153, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_prepare, 419, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__154)) __PYX_ERR(26, 419, __pyx_L1_error)
 
   /* "asynctnt/iproto/db.pyx":425
  *         return self._prepare(query, <bint> parse_metadata, timeout)
  * 
  *     def begin(self,             # <<<<<<<<<<<<<<
  *               uint32_t isolation,
  *               float tx_timeout=0,
  */
-  __pyx_tuple__156 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_isolation, __pyx_n_s_tx_timeout, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__156)) __PYX_ERR(26, 425, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__156);
-  __Pyx_GIVEREF(__pyx_tuple__156);
-  __pyx_codeobj__157 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__156, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_begin, 425, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__157)) __PYX_ERR(26, 425, __pyx_L1_error)
-  __pyx_tuple__158 = PyTuple_Pack(2, __pyx_float_0_0, __pyx_float_neg_1_0); if (unlikely(!__pyx_tuple__158)) __PYX_ERR(26, 425, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__158);
-  __Pyx_GIVEREF(__pyx_tuple__158);
+  __pyx_tuple__155 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_isolation, __pyx_n_s_tx_timeout, __pyx_n_s_timeout); if (unlikely(!__pyx_tuple__155)) __PYX_ERR(26, 425, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__155);
+  __Pyx_GIVEREF(__pyx_tuple__155);
+  __pyx_codeobj__156 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__155, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_begin, 425, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__156)) __PYX_ERR(26, 425, __pyx_L1_error)
+  __pyx_tuple__157 = PyTuple_Pack(2, __pyx_float_0_0, __pyx_float_neg_1_0); if (unlikely(!__pyx_tuple__157)) __PYX_ERR(26, 425, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__157);
+  __Pyx_GIVEREF(__pyx_tuple__157);
 
   /* "asynctnt/iproto/db.pyx":431
  *         return self._begin(isolation, <double> tx_timeout, timeout)
  * 
  *     def commit(self, float timeout=-1):             # <<<<<<<<<<<<<<
  *         return self._commit(timeout)
  * 
  */
-  __pyx_codeobj__159 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__127, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_commit, 431, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__159)) __PYX_ERR(26, 431, __pyx_L1_error)
+  __pyx_codeobj__158 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__126, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_commit, 431, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__158)) __PYX_ERR(26, 431, __pyx_L1_error)
 
   /* "asynctnt/iproto/db.pyx":434
  *         return self._commit(timeout)
  * 
  *     def rollback(self, float timeout=-1):             # <<<<<<<<<<<<<<
  *         return self._rollback(timeout)
  */
-  __pyx_codeobj__160 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__127, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_rollback, 434, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__160)) __PYX_ERR(26, 434, __pyx_L1_error)
+  __pyx_codeobj__159 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__126, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_db_pyx, __pyx_n_s_rollback, 434, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__159)) __PYX_ERR(26, 434, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__161 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__161)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__160 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__160)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__162 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__162)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__161 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__161)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__163 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__163)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__162 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__162)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_PushIterator, (type(self), 0x98137af, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_PushIterator__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__164 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__164)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__163 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__163)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "asynctnt/iproto/coreproto.pyx":15
  * from asynctnt.log import logger
  * 
  * VERSION_STRING_REGEX = re.compile(r'\s*Tarantool\s+([\d.]+)\s+.*')             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__165 = PyTuple_Pack(1, __pyx_kp_u_s_Tarantool_s_d_s); if (unlikely(!__pyx_tuple__165)) __PYX_ERR(28, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__165);
-  __Pyx_GIVEREF(__pyx_tuple__165);
+  __pyx_tuple__164 = PyTuple_Pack(1, __pyx_kp_u_s_Tarantool_s_d_s); if (unlikely(!__pyx_tuple__164)) __PYX_ERR(28, 15, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__164);
+  __Pyx_GIVEREF(__pyx_tuple__164);
 
   /* "asynctnt/iproto/coreproto.pyx":50
  *         return self.con_state == CONNECTION_FULL
  * 
  *     def is_connected(self):             # <<<<<<<<<<<<<<
  *         return self._is_connected()
  * 
  */
-  __pyx_codeobj__166 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_is_connected, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__166)) __PYX_ERR(28, 50, __pyx_L1_error)
+  __pyx_codeobj__165 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_is_connected, 50, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__165)) __PYX_ERR(28, 50, __pyx_L1_error)
 
   /* "asynctnt/iproto/coreproto.pyx":53
  *         return self._is_connected()
  * 
  *     def is_fully_connected(self):             # <<<<<<<<<<<<<<
  *         return self._is_fully_connected()
  * 
  */
-  __pyx_codeobj__167 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_is_fully_connected, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__167)) __PYX_ERR(28, 53, __pyx_L1_error)
+  __pyx_codeobj__166 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_is_fully_connected, 53, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__166)) __PYX_ERR(28, 53, __pyx_L1_error)
 
   /* "asynctnt/iproto/coreproto.pyx":56
  *         return self._is_fully_connected()
  * 
  *     def get_version(self):             # <<<<<<<<<<<<<<
  *         return self.version
  * 
  */
-  __pyx_codeobj__168 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_get_version, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__168)) __PYX_ERR(28, 56, __pyx_L1_error)
+  __pyx_codeobj__167 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_get_version, 56, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__167)) __PYX_ERR(28, 56, __pyx_L1_error)
 
   /* "asynctnt/iproto/coreproto.pyx":143
  *         self._on_greeting_received()
  * 
  *     def _parse_version(self, version):             # <<<<<<<<<<<<<<
  *         m = VERSION_STRING_REGEX.match(version.decode('ascii'))
  *         if m is not None:
  */
-  __pyx_tuple__169 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_version, __pyx_n_s_m, __pyx_n_s_ver); if (unlikely(!__pyx_tuple__169)) __PYX_ERR(28, 143, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__169);
-  __Pyx_GIVEREF(__pyx_tuple__169);
-  __pyx_codeobj__170 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__169, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_parse_version, 143, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__170)) __PYX_ERR(28, 143, __pyx_L1_error)
+  __pyx_tuple__168 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_version, __pyx_n_s_m, __pyx_n_s_ver); if (unlikely(!__pyx_tuple__168)) __PYX_ERR(28, 143, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__168);
+  __Pyx_GIVEREF(__pyx_tuple__168);
+  __pyx_codeobj__169 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__168, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_parse_version, 143, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__169)) __PYX_ERR(28, 143, __pyx_L1_error)
 
   /* "asynctnt/iproto/coreproto.pyx":163
  *     # asyncio callbacks
  * 
  *     def data_received(self, data):             # <<<<<<<<<<<<<<
  *         self._on_data_received(data)
  * 
  */
-  __pyx_tuple__171 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_data); if (unlikely(!__pyx_tuple__171)) __PYX_ERR(28, 163, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__171);
-  __Pyx_GIVEREF(__pyx_tuple__171);
-  __pyx_codeobj__172 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__171, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_data_received, 163, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__172)) __PYX_ERR(28, 163, __pyx_L1_error)
+  __pyx_tuple__170 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_data); if (unlikely(!__pyx_tuple__170)) __PYX_ERR(28, 163, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__170);
+  __Pyx_GIVEREF(__pyx_tuple__170);
+  __pyx_codeobj__171 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__170, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_data_received, 163, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__171)) __PYX_ERR(28, 163, __pyx_L1_error)
 
   /* "asynctnt/iproto/coreproto.pyx":166
  *         self._on_data_received(data)
  * 
  *     def connection_made(self, transport):             # <<<<<<<<<<<<<<
  *         self.transport = transport
  *         self.con_state = CONNECTION_CONNECTED
  */
-  __pyx_tuple__173 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_transport, __pyx_n_s_sock); if (unlikely(!__pyx_tuple__173)) __PYX_ERR(28, 166, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__173);
-  __Pyx_GIVEREF(__pyx_tuple__173);
-  __pyx_codeobj__174 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__173, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_connection_made, 166, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__174)) __PYX_ERR(28, 166, __pyx_L1_error)
+  __pyx_tuple__172 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_transport, __pyx_n_s_sock); if (unlikely(!__pyx_tuple__172)) __PYX_ERR(28, 166, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__172);
+  __Pyx_GIVEREF(__pyx_tuple__172);
+  __pyx_codeobj__173 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__172, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_connection_made, 166, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__173)) __PYX_ERR(28, 166, __pyx_L1_error)
 
   /* "asynctnt/iproto/coreproto.pyx":179
  *         self._on_connection_made()
  * 
  *     def connection_lost(self, exc):             # <<<<<<<<<<<<<<
  *         self.con_state = CONNECTION_BAD
  *         self.version = None
  */
-  __pyx_tuple__175 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_exc); if (unlikely(!__pyx_tuple__175)) __PYX_ERR(28, 179, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__175);
-  __Pyx_GIVEREF(__pyx_tuple__175);
-  __pyx_codeobj__176 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__175, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_connection_lost, 179, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__176)) __PYX_ERR(28, 179, __pyx_L1_error)
+  __pyx_tuple__174 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_exc); if (unlikely(!__pyx_tuple__174)) __PYX_ERR(28, 179, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__174);
+  __Pyx_GIVEREF(__pyx_tuple__174);
+  __pyx_codeobj__175 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__174, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_coreproto_pyx, __pyx_n_s_connection_lost, 179, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__175)) __PYX_ERR(28, 179, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_codeobj__177 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__85, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__177)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__176 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__84, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__176)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_CoreProtocol, (type(self), 0x89d360e, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_CoreProtocol__set_state(self, __pyx_state)
  */
-  __pyx_codeobj__178 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__178)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_codeobj__177 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__177)) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "asynctnt/iproto/protocol.pyx":108
  *             self.create_future = self._create_future_fallback
  * 
  *     def _create_future_fallback(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return asyncio.Future(loop=self.loop)
  * 
  */
-  __pyx_codeobj__179 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_create_future_fallback, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__179)) __PYX_ERR(6, 108, __pyx_L1_error)
+  __pyx_codeobj__178 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_create_future_fallback, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__178)) __PYX_ERR(6, 108, __pyx_L1_error)
 
   /* "asynctnt/iproto/protocol.pyx":425
  *         return self._last_stream_id
  * 
  *     def _on_request_timeout(self, waiter):             # <<<<<<<<<<<<<<
  *         cdef:
  *             BaseRequest req
  */
-  __pyx_tuple__180 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_waiter, __pyx_n_s_req, __pyx_n_s_response_2); if (unlikely(!__pyx_tuple__180)) __PYX_ERR(6, 425, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__180);
-  __Pyx_GIVEREF(__pyx_tuple__180);
-  __pyx_codeobj__181 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__180, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_on_request_timeout, 425, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__181)) __PYX_ERR(6, 425, __pyx_L1_error)
+  __pyx_tuple__179 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_waiter, __pyx_n_s_req, __pyx_n_s_response_2); if (unlikely(!__pyx_tuple__179)) __PYX_ERR(6, 425, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__179);
+  __Pyx_GIVEREF(__pyx_tuple__179);
+  __pyx_codeobj__180 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__179, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_on_request_timeout, 425, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__180)) __PYX_ERR(6, 425, __pyx_L1_error)
 
   /* "asynctnt/iproto/protocol.pyx":442
  *         )
  * 
  *     def _on_request_completed(self, fut):             # <<<<<<<<<<<<<<
  *         cdef BaseRequest req = (<Response> fut._response).request_
  *         fut._response = None
  */
-  __pyx_tuple__182 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_fut, __pyx_n_s_req); if (unlikely(!__pyx_tuple__182)) __PYX_ERR(6, 442, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__182);
-  __Pyx_GIVEREF(__pyx_tuple__182);
-  __pyx_codeobj__183 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__182, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_on_request_completed, 442, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__183)) __PYX_ERR(6, 442, __pyx_L1_error)
+  __pyx_tuple__181 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_fut, __pyx_n_s_req); if (unlikely(!__pyx_tuple__181)) __PYX_ERR(6, 442, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__181);
+  __Pyx_GIVEREF(__pyx_tuple__181);
+  __pyx_codeobj__182 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__181, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_on_request_completed, 442, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__182)) __PYX_ERR(6, 442, __pyx_L1_error)
 
   /* "asynctnt/iproto/protocol.pyx":473
  *         return Db.create(self, stream_id)
  * 
  *     def create_db(self, bint gen_stream_id = False):             # <<<<<<<<<<<<<<
  *         return self._create_db(gen_stream_id)
  * 
  */
-  __pyx_tuple__184 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_gen_stream_id); if (unlikely(!__pyx_tuple__184)) __PYX_ERR(6, 473, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__184);
-  __Pyx_GIVEREF(__pyx_tuple__184);
-  __pyx_codeobj__185 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__184, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_create_db, 473, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__185)) __PYX_ERR(6, 473, __pyx_L1_error)
-  __pyx_tuple__186 = PyTuple_Pack(1, Py_False); if (unlikely(!__pyx_tuple__186)) __PYX_ERR(6, 473, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__186);
-  __Pyx_GIVEREF(__pyx_tuple__186);
+  __pyx_tuple__183 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_gen_stream_id); if (unlikely(!__pyx_tuple__183)) __PYX_ERR(6, 473, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__183);
+  __Pyx_GIVEREF(__pyx_tuple__183);
+  __pyx_codeobj__184 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__183, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_create_db, 473, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__184)) __PYX_ERR(6, 473, __pyx_L1_error)
+  __pyx_tuple__185 = PyTuple_Pack(1, Py_False); if (unlikely(!__pyx_tuple__185)) __PYX_ERR(6, 473, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__185);
+  __Pyx_GIVEREF(__pyx_tuple__185);
 
   /* "asynctnt/iproto/protocol.pyx":476
  *         return self._create_db(gen_stream_id)
  * 
  *     def get_common_db(self):             # <<<<<<<<<<<<<<
  *         return self._db
  * 
  */
-  __pyx_codeobj__187 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_get_common_db, 476, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__187)) __PYX_ERR(6, 476, __pyx_L1_error)
+  __pyx_codeobj__186 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_get_common_db, 476, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__186)) __PYX_ERR(6, 476, __pyx_L1_error)
 
   /* "asynctnt/iproto/protocol.pyx":515
  *         return self._refetch_schema_future
  * 
  *     def refetch_schema(self):             # <<<<<<<<<<<<<<
  *         return self._refetch_schema()
  * 
  */
-  __pyx_codeobj__188 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_refetch_schema, 515, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__188)) __PYX_ERR(6, 515, __pyx_L1_error)
+  __pyx_codeobj__187 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_asynctnt_iproto_protocol_pyx, __pyx_n_s_refetch_schema, 515, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__187)) __PYX_ERR(6, 515, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.execute cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__189 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__67, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__189)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__188 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__66, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__188)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "self.execute cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.execute cannot be converted to a Python object for pickling"
  */
-  __pyx_codeobj__190 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__69, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__190)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__189 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__68, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__189)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_BaseRequest(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__191 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__191)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__191);
-  __Pyx_GIVEREF(__pyx_tuple__191);
-  __pyx_codeobj__192 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BaseRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__192)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__193 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_PingRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__193)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__194 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CallRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__194)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__195 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_EvalRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__195)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__196 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_SelectRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__196)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__197 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_InsertRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__197)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__198 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DeleteRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__198)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__199 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_UpdateRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__199)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__200 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_UpsertRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__200)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__201 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_PrepareRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__201)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__202 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ExecuteRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__202)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__203 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IDRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__203)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__204 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AuthRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__204)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__205 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BeginRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__205)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__206 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CommitRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__206)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__207 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_RollbackRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__207)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__208 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IProtoErrorStackF, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__208)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__209 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IProtoError, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__209)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__210 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_PushIterator, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__210)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_codeobj__211 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__191, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CoreProtocol, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__211)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_tuple__190 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__190)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__190);
+  __Pyx_GIVEREF(__pyx_tuple__190);
+  __pyx_codeobj__191 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BaseRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__191)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__192 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_PingRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__192)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__193 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CallRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__193)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__194 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_EvalRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__194)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__195 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_SelectRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__195)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__196 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_InsertRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__196)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__197 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DeleteRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__197)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__198 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_UpdateRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__198)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__199 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_UpsertRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__199)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__200 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_PrepareRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__200)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__201 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_ExecuteRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__201)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__202 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IDRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__202)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__203 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_AuthRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__203)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__204 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BeginRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__204)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__205 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CommitRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__205)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__206 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_RollbackRequest, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__206)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__207 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IProtoErrorStackF, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__207)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__208 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IProtoError, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__208)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__209 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_PushIterator, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__209)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__210 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__190, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_CoreProtocol, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__210)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -86660,14 +86721,15 @@
   if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_Field) < 0) __PYX_ERR(1, 13, __pyx_L1_error)
   #endif
   __pyx_vtabptr_8asynctnt_6iproto_8protocol_Metadata = &__pyx_vtable_8asynctnt_6iproto_8protocol_Metadata;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Metadata.len = (int (*)(struct C_Metadata *))__pyx_f_8asynctnt_6iproto_8protocol_8Metadata_len;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Metadata.add = (void (*)(struct C_Metadata *, int, struct __pyx_obj_8asynctnt_6iproto_8protocol_Field *))__pyx_f_8asynctnt_6iproto_8protocol_8Metadata_add;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Metadata.name_by_id = (PyObject *(*)(struct C_Metadata *, int))__pyx_f_8asynctnt_6iproto_8protocol_8Metadata_name_by_id;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Metadata.id_by_name = (int (*)(struct C_Metadata *, PyObject *))__pyx_f_8asynctnt_6iproto_8protocol_8Metadata_id_by_name;
+  __pyx_vtable_8asynctnt_6iproto_8protocol_Metadata.id_by_name_safe = (int (*)(struct C_Metadata *, PyObject *))__pyx_f_8asynctnt_6iproto_8protocol_8Metadata_id_by_name_safe;
   #if CYTHON_USE_TYPE_SPECS
   __pyx_ptype_8asynctnt_6iproto_8protocol_Metadata = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &C_Metadata_Type_spec, NULL); if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_Metadata)) __PYX_ERR(1, 29, __pyx_L1_error)
   if (__Pyx_fix_up_extension_type_from_spec(&C_Metadata_Type_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_Metadata) < 0) __PYX_ERR(1, 29, __pyx_L1_error)
   #else
   __pyx_ptype_8asynctnt_6iproto_8protocol_Metadata = &C_Metadata_Type;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
@@ -86688,156 +86750,156 @@
   if (__Pyx_MergeVtables(__pyx_ptype_8asynctnt_6iproto_8protocol_Metadata) < 0) __PYX_ERR(1, 29, __pyx_L1_error)
   #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Metadata, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_Metadata) < 0) __PYX_ERR(1, 29, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_Metadata) < 0) __PYX_ERR(1, 29, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8asynctnt_6iproto_8protocol_SchemaIndex_spec, NULL); if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex)) __PYX_ERR(1, 61, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8asynctnt_6iproto_8protocol_SchemaIndex_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex) < 0) __PYX_ERR(1, 61, __pyx_L1_error)
+  __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8asynctnt_6iproto_8protocol_SchemaIndex_spec, NULL); if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex)) __PYX_ERR(1, 70, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8asynctnt_6iproto_8protocol_SchemaIndex_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   #else
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex = &__pyx_type_8asynctnt_6iproto_8protocol_SchemaIndex;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex) < 0) __PYX_ERR(1, 61, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex->tp_dictoffset && __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SchemaIndex, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex) < 0) __PYX_ERR(1, 61, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SchemaIndex, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex) < 0) __PYX_ERR(1, 61, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 36, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8asynctnt_6iproto_8protocol_SchemaDummyIndex_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex)) __PYX_ERR(11, 36, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8asynctnt_6iproto_8protocol_SchemaDummyIndex_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex) < 0) __PYX_ERR(11, 36, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex)) __PYX_ERR(11, 37, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8asynctnt_6iproto_8protocol_SchemaDummyIndex_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex) < 0) __PYX_ERR(11, 37, __pyx_L1_error)
   #else
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex = &__pyx_type_8asynctnt_6iproto_8protocol_SchemaDummyIndex;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex->tp_base = __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaIndex;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex) < 0) __PYX_ERR(11, 36, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex) < 0) __PYX_ERR(11, 37, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex->tp_dictoffset && __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SchemaDummyIndex, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex) < 0) __PYX_ERR(11, 36, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SchemaDummyIndex, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummyIndex) < 0) __PYX_ERR(11, 37, __pyx_L1_error)
   __pyx_vtabptr_8asynctnt_6iproto_8protocol_SchemaSpace = &__pyx_vtable_8asynctnt_6iproto_8protocol_SchemaSpace;
   __pyx_vtable_8asynctnt_6iproto_8protocol_SchemaSpace.add_index = (void (*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *, struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *))__pyx_f_8asynctnt_6iproto_8protocol_11SchemaSpace_add_index;
   __pyx_vtable_8asynctnt_6iproto_8protocol_SchemaSpace.get_index = (struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *(*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *, PyObject *, struct __pyx_opt_args_8asynctnt_6iproto_8protocol_11SchemaSpace_get_index *__pyx_optional_args))__pyx_f_8asynctnt_6iproto_8protocol_11SchemaSpace_get_index;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8asynctnt_6iproto_8protocol_SchemaSpace_spec, NULL); if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace)) __PYX_ERR(1, 79, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8asynctnt_6iproto_8protocol_SchemaSpace_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
+  __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8asynctnt_6iproto_8protocol_SchemaSpace_spec, NULL); if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace)) __PYX_ERR(1, 88, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8asynctnt_6iproto_8protocol_SchemaSpace_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
   #else
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace = &__pyx_type_8asynctnt_6iproto_8protocol_SchemaSpace;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace->tp_dictoffset && __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace, __pyx_vtabptr_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace, __pyx_vtabptr_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SchemaSpace, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SchemaSpace, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
   #endif
   __pyx_vtabptr_8asynctnt_6iproto_8protocol_SchemaDummySpace = &__pyx_vtable_8asynctnt_6iproto_8protocol_SchemaDummySpace;
   __pyx_vtable_8asynctnt_6iproto_8protocol_SchemaDummySpace.__pyx_base = *__pyx_vtabptr_8asynctnt_6iproto_8protocol_SchemaSpace;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 56, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8asynctnt_6iproto_8protocol_SchemaDummySpace_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace)) __PYX_ERR(11, 56, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8asynctnt_6iproto_8protocol_SchemaDummySpace_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace) < 0) __PYX_ERR(11, 56, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace)) __PYX_ERR(11, 57, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8asynctnt_6iproto_8protocol_SchemaDummySpace_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace) < 0) __PYX_ERR(11, 57, __pyx_L1_error)
   #else
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace = &__pyx_type_8asynctnt_6iproto_8protocol_SchemaDummySpace;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace->tp_base = __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaSpace;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace) < 0) __PYX_ERR(11, 56, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace) < 0) __PYX_ERR(11, 57, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace->tp_dictoffset && __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace, __pyx_vtabptr_8asynctnt_6iproto_8protocol_SchemaDummySpace) < 0) __PYX_ERR(11, 56, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace, __pyx_vtabptr_8asynctnt_6iproto_8protocol_SchemaDummySpace) < 0) __PYX_ERR(11, 57, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace) < 0) __PYX_ERR(11, 56, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace) < 0) __PYX_ERR(11, 57, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SchemaDummySpace, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace) < 0) __PYX_ERR(11, 56, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SchemaDummySpace, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_SchemaDummySpace) < 0) __PYX_ERR(11, 57, __pyx_L1_error)
   __pyx_vtabptr_8asynctnt_6iproto_8protocol_Schema = &__pyx_vtable_8asynctnt_6iproto_8protocol_Schema;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Schema.get_space = (struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *(*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *, PyObject *))__pyx_f_8asynctnt_6iproto_8protocol_6Schema_get_space;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Schema.create_dummy_space = (struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *(*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *, int))__pyx_f_8asynctnt_6iproto_8protocol_6Schema_create_dummy_space;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Schema.get_or_create_space = (struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *(*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *, PyObject *))__pyx_f_8asynctnt_6iproto_8protocol_6Schema_get_or_create_space;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Schema.parse_space = (struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaSpace *(*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *, PyObject *))__pyx_f_8asynctnt_6iproto_8protocol_6Schema_parse_space;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Schema.parse_index = (struct __pyx_obj_8asynctnt_6iproto_8protocol_SchemaIndex *(*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *, PyObject *))__pyx_f_8asynctnt_6iproto_8protocol_6Schema_parse_index;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Schema.clear = (PyObject *(*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *))__pyx_f_8asynctnt_6iproto_8protocol_6Schema_clear;
   __pyx_vtable_8asynctnt_6iproto_8protocol_Schema.parse = (struct __pyx_obj_8asynctnt_6iproto_8protocol_Schema *(*)(int64_t, PyObject *, PyObject *))__pyx_f_8asynctnt_6iproto_8protocol_6Schema_parse;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_8asynctnt_6iproto_8protocol_Schema = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8asynctnt_6iproto_8protocol_Schema_spec, NULL); if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_Schema)) __PYX_ERR(1, 136, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8asynctnt_6iproto_8protocol_Schema_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 136, __pyx_L1_error)
+  __pyx_ptype_8asynctnt_6iproto_8protocol_Schema = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_8asynctnt_6iproto_8protocol_Schema_spec, NULL); if (unlikely(!__pyx_ptype_8asynctnt_6iproto_8protocol_Schema)) __PYX_ERR(1, 145, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_8asynctnt_6iproto_8protocol_Schema_spec, __pyx_ptype_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 145, __pyx_L1_error)
   #else
   __pyx_ptype_8asynctnt_6iproto_8protocol_Schema = &__pyx_type_8asynctnt_6iproto_8protocol_Schema;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 136, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 145, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_8asynctnt_6iproto_8protocol_Schema->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_8asynctnt_6iproto_8protocol_Schema->tp_dictoffset && __pyx_ptype_8asynctnt_6iproto_8protocol_Schema->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_8asynctnt_6iproto_8protocol_Schema->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_8asynctnt_6iproto_8protocol_Schema, __pyx_vtabptr_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 136, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_8asynctnt_6iproto_8protocol_Schema, __pyx_vtabptr_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 145, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 136, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 145, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Schema, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 136, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Schema, (PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 145, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 136, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_8asynctnt_6iproto_8protocol_Schema) < 0) __PYX_ERR(1, 145, __pyx_L1_error)
   #endif
   __pyx_vtabptr_8asynctnt_6iproto_8protocol_WriteBuffer = &__pyx_vtable_8asynctnt_6iproto_8protocol_WriteBuffer;
   __pyx_vtable_8asynctnt_6iproto_8protocol_WriteBuffer.create = (struct __pyx_obj_8asynctnt_6iproto_8protocol_WriteBuffer *(*)(PyObject *))__pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_create;
   __pyx_vtable_8asynctnt_6iproto_8protocol_WriteBuffer._check_readonly = (PyObject *(*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_WriteBuffer *))__pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer__check_readonly;
   __pyx_vtable_8asynctnt_6iproto_8protocol_WriteBuffer.len = (PyObject *(*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_WriteBuffer *))__pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_len;
   __pyx_vtable_8asynctnt_6iproto_8protocol_WriteBuffer.ensure_allocated = (int (*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_WriteBuffer *, Py_ssize_t))__pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer_ensure_allocated;
   __pyx_vtable_8asynctnt_6iproto_8protocol_WriteBuffer._ensure_allocated = (char *(*)(struct __pyx_obj_8asynctnt_6iproto_8protocol_WriteBuffer *, char *, Py_ssize_t))__pyx_f_8asynctnt_6iproto_8protocol_11WriteBuffer__ensure_allocated;
@@ -88298,110 +88360,110 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_5Field_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Field___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__68)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_5Field_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Field___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__67)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_5Field_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Field___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_5Field_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Field___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__69)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_8Metadata_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Metadata___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__71)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_8Metadata_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Metadata___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__70)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_8Metadata_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Metadata___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__72)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_8Metadata_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Metadata___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__71)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11SchemaIndex_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SchemaIndex___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__73)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11SchemaIndex_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SchemaIndex___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__72)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11SchemaIndex_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SchemaIndex___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__74)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11SchemaIndex_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SchemaIndex___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__73)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11SchemaSpace_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SchemaSpace___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__75)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11SchemaSpace_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SchemaSpace___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__74)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11SchemaSpace_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SchemaSpace___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__76)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11SchemaSpace_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SchemaSpace___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__75)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_6Schema_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Schema___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__77)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_6Schema_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Schema___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__76)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_6Schema_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Schema___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__78)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_6Schema_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Schema___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__77)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "asynctnt/iproto/ext.pyx":6
  * from libc.string cimport memcpy
  * 
@@ -88489,333 +88551,333 @@
   /* "asynctnt/iproto/buffer.pyx":54
  *         self._view_count -= 1
  * 
  *     def hex(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return ":".join("{:02x}".format(ord(<bytes> (self._buf[i])))
  *                         for i in range(self._length))
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11WriteBuffer_9hex, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_WriteBuffer_hex, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 54, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11WriteBuffer_9hex, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_WriteBuffer_hex, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__79)); if (unlikely(!__pyx_t_3)) __PYX_ERR(3, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_WriteBuffer, __pyx_n_s_hex, __pyx_t_3) < 0) __PYX_ERR(3, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_WriteBuffer);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11WriteBuffer_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_WriteBuffer___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11WriteBuffer_11__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_WriteBuffer___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__80)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11WriteBuffer_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_WriteBuffer___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11WriteBuffer_13__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_WriteBuffer___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__81)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_10ReadBuffer_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ReadBuffer___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_10ReadBuffer_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ReadBuffer___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__82)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_10ReadBuffer_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ReadBuffer___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__84)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_10ReadBuffer_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ReadBuffer___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__83)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11BaseRequest_3__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__86)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11BaseRequest_3__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__85)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_BaseRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_BaseRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_BaseRequest, (type(self), 0x9001016, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_BaseRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11BaseRequest_5__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11BaseRequest_5__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__86)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_BaseRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_BaseRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11PingRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PingRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__88)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11PingRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PingRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_PingRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_PingRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_PingRequest, (type(self), 0x9001016, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_PingRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11PingRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PingRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__89)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11PingRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PingRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__88)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_PingRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_PingRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11CallRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CallRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__90)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11CallRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CallRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__89)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CallRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CallRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_CallRequest, (type(self), 0x2d5a81d, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_CallRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11CallRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CallRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__91)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11CallRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CallRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__90)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CallRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CallRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11EvalRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_EvalRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11EvalRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_EvalRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__91)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_EvalRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_EvalRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_EvalRequest, (type(self), 0xafafa67, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_EvalRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11EvalRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_EvalRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__93)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11EvalRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_EvalRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_EvalRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_EvalRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13SelectRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SelectRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__94)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13SelectRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SelectRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__93)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SelectRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_SelectRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_SelectRequest, (type(self), 0x8e2dc2b, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_SelectRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13SelectRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SelectRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__95)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13SelectRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SelectRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__94)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_SelectRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_SelectRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13InsertRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_InsertRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13InsertRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_InsertRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__95)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_InsertRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_InsertRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_InsertRequest, (type(self), 0xb91d1f2, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_InsertRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13InsertRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_InsertRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__97)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13InsertRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_InsertRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_InsertRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_InsertRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13DeleteRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_DeleteRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13DeleteRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_DeleteRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__97)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_DeleteRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_DeleteRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_DeleteRequest, (type(self), 0xf383ff7, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_DeleteRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13DeleteRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_DeleteRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__99)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13DeleteRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_DeleteRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_DeleteRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_DeleteRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13UpdateRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_UpdateRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__100)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13UpdateRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_UpdateRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__99)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_UpdateRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_UpdateRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_UpdateRequest, (type(self), 0x815e48a, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_UpdateRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13UpdateRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_UpdateRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__101)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13UpdateRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_UpdateRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__100)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_UpdateRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_UpdateRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13UpsertRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_UpsertRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__102)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13UpsertRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_UpsertRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__101)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_UpsertRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_UpsertRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_UpsertRequest, (type(self), 0xc823323, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_UpsertRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13UpsertRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_UpsertRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__103)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13UpsertRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_UpsertRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__102)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_UpsertRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_UpsertRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_14PrepareRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PrepareRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__104)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_14PrepareRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PrepareRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__103)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_PrepareRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_PrepareRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_PrepareRequest, (type(self), 0xd0934a3, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_PrepareRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_14PrepareRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PrepareRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__105)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_14PrepareRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PrepareRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__104)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_PrepareRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_PrepareRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_14ExecuteRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ExecuteRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__106)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_14ExecuteRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ExecuteRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__105)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_ExecuteRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_ExecuteRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_ExecuteRequest, (type(self), 0x314ca88, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_ExecuteRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_14ExecuteRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ExecuteRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__107)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_14ExecuteRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_ExecuteRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__106)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_ExecuteRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_ExecuteRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_9IDRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IDRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__108)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_9IDRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IDRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__107)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_IDRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_IDRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_IDRequest, (type(self), 0x9001016, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_IDRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_9IDRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IDRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__109)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_9IDRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IDRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__108)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_IDRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_IDRequest);
 
   /* "asynctnt/iproto/requests/auth.pyx":5
  * cimport cython
@@ -88830,96 +88892,96 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11AuthRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_AuthRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__110)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11AuthRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_AuthRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__109)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_AuthRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_AuthRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_AuthRequest, (type(self), 0x335e105, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_AuthRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11AuthRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_AuthRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__111)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11AuthRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_AuthRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__110)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_AuthRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_AuthRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BeginRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BeginRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__112)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BeginRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BeginRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__111)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_BeginRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_BeginRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_BeginRequest, (type(self), 0x30f95df, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_BeginRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BeginRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BeginRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__113)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BeginRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BeginRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__112)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_BeginRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_BeginRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13CommitRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CommitRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__114)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13CommitRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CommitRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__113)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CommitRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CommitRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_CommitRequest, (type(self), 0x9001016, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_CommitRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13CommitRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CommitRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__115)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13CommitRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CommitRequest___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__114)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CommitRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CommitRequest);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_15RollbackRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RollbackRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__116)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_15RollbackRequest_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RollbackRequest___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__115)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_RollbackRequest, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_RollbackRequest);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_RollbackRequest, (type(self), 0x9001016, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_RollbackRequest__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_15RollbackRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RollbackRequest___setstate_cytho, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__117)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_15RollbackRequest_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_RollbackRequest___setstate_cytho, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__116)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_RollbackRequest, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_RollbackRequest);
 
   /* "asynctnt/iproto/ttuple.pyx":1
  * TarantoolTuple = <object> tupleobj.AtntTuple_InitTypes()             # <<<<<<<<<<<<<<
@@ -88994,328 +89056,328 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_21IProtoErrorStackFrame_3__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IProtoErrorStackFrame___reduce_c, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__118)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_21IProtoErrorStackFrame_3__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IProtoErrorStackFrame___reduce_c, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__117)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_IProtoErrorStackFrame, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_IProtoErrorStackFrame);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_IProtoErrorStackFrame, (type(self), 0xab276bf, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_IProtoErrorStackFrame__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_21IProtoErrorStackFrame_5__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IProtoErrorStackFrame___setstate, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__119)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_21IProtoErrorStackFrame_5__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IProtoErrorStackFrame___setstate, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__118)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_IProtoErrorStackFrame, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_IProtoErrorStackFrame);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11IProtoError_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IProtoError___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__120)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11IProtoError_1__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IProtoError___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__119)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_IProtoError, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_IProtoError);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_IProtoError, (type(self), 0xeafe895, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_IProtoError__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11IProtoError_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IProtoError___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__121)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11IProtoError_3__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_IProtoError___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__120)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_IProtoError, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_IProtoError);
 
   /* "asynctnt/iproto/response.pyx":160
  *         return self.stmt_id_
  * 
  *     def done(self):             # <<<<<<<<<<<<<<
  *         return self.code_ >= 0
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_8Response_5done, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Response_done, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__122)); if (unlikely(!__pyx_t_3)) __PYX_ERR(5, 160, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_8Response_5done, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Response_done, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__121)); if (unlikely(!__pyx_t_3)) __PYX_ERR(5, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Response, __pyx_n_s_done, __pyx_t_3) < 0) __PYX_ERR(5, 160, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Response);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_8Response_13__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Response___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__123)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_8Response_13__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Response___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__122)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_8Response_15__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Response___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__124)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_8Response_15__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Response___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__123)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "asynctnt/iproto/db.pyx":327
  *         return <int> self._stream_id
  * 
  *     def set_stream_id(self, int stream_id):             # <<<<<<<<<<<<<<
  *         self._stream_id = <uint64_t> stream_id
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_3set_stream_id, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_set_stream_id, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__126)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 327, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_3set_stream_id, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_set_stream_id, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__125)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_set_stream_id, __pyx_t_3) < 0) __PYX_ERR(26, 327, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":330
  *         self._stream_id = <uint64_t> stream_id
  * 
  *     def ping(self, float timeout=-1):             # <<<<<<<<<<<<<<
  *         return self._ping(timeout)
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_5ping, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_ping, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__128)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 330, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_5ping, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_ping, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__127)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__129);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__128);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_ping, __pyx_t_3) < 0) __PYX_ERR(26, 330, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":333
  *         return self._ping(timeout)
  * 
  *     def call16(self,             # <<<<<<<<<<<<<<
  *                str func_name,
  *                object args=None,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_7call16, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_call16, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__131)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 333, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_7call16, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_call16, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__130)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__132);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__131);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_call16, __pyx_t_3) < 0) __PYX_ERR(26, 333, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":344
  *                           <bint> push_subscribe)
  * 
  *     def call(self,             # <<<<<<<<<<<<<<
  *              str func_name,
  *              object args=None,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_9call, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_call, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__133)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 344, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_9call, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_call, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__132)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 344, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__132);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__131);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_call, __pyx_t_3) < 0) __PYX_ERR(26, 344, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":355
  *                           <bint> push_subscribe)
  * 
  *     def eval(self,             # <<<<<<<<<<<<<<
  *              str expression,
  *              object args=None,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_11eval, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_eval, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__135)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 355, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_11eval, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_eval, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__134)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 355, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__132);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__131);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_eval, __pyx_t_3) < 0) __PYX_ERR(26, 355, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":365
  *                           <bint> push_subscribe)
  * 
  *     def select(self,             # <<<<<<<<<<<<<<
  *                object space,
  *                object key=None,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_13select, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_select, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__137)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 365, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_13select, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_select, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__136)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__138);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__137);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_select, __pyx_t_3) < 0) __PYX_ERR(26, 365, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":377
  *                             timeout, check_schema_change)
  * 
  *     def insert(self,             # <<<<<<<<<<<<<<
  *                object space,
  *                object t,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_15insert, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_insert, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__140)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 377, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_15insert, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_insert, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__139)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 377, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__141);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__140);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_insert, __pyx_t_3) < 0) __PYX_ERR(26, 377, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":384
  *         return self._insert(space, t, <bint> replace, timeout)
  * 
  *     def replace(self,             # <<<<<<<<<<<<<<
  *                 object space,
  *                 object t,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_17replace, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_replace, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__143)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 384, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_17replace, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_replace, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__142)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 384, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__129);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__128);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_replace, __pyx_t_3) < 0) __PYX_ERR(26, 384, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":390
  *         return self._insert(space, t, <bint> True, timeout)
  * 
  *     def delete(self,             # <<<<<<<<<<<<<<
  *                object space,
  *                object key,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_19delete, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_delete, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__145)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 390, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_19delete, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_delete, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__144)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 390, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__146);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__145);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_delete, __pyx_t_3) < 0) __PYX_ERR(26, 390, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":397
  *         return self._delete(space, index, key, timeout)
  * 
  *     def update(self,             # <<<<<<<<<<<<<<
  *                object space,
  *                object key,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_21update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_update, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__148)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 397, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_21update, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_update, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__147)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 397, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__146);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__145);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_update, __pyx_t_3) < 0) __PYX_ERR(26, 397, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":405
  *         return self._update(space, index, key, operations, timeout)
  * 
  *     def upsert(self,             # <<<<<<<<<<<<<<
  *                object space,
  *                object t,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_23upsert, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_upsert, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__150)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 405, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_23upsert, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_upsert, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__149)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__129);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__128);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_upsert, __pyx_t_3) < 0) __PYX_ERR(26, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":412
  *         return self._upsert(space, t, operations, timeout)
  * 
  *     def execute(self,             # <<<<<<<<<<<<<<
  *                 object query,
  *                 object args,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_25execute, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_execute, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__152)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 412, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_25execute, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_execute, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__151)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 412, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__153);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__152);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_execute, __pyx_t_3) < 0) __PYX_ERR(26, 412, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":419
  *         return self._execute(query, args, <bint> parse_metadata, timeout)
  * 
  *     def prepare(self,             # <<<<<<<<<<<<<<
  *                 object query,
  *                 bint parse_metadata=True,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_27prepare, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_prepare, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__155)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 419, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_27prepare, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_prepare, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__154)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__153);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__152);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_prepare, __pyx_t_3) < 0) __PYX_ERR(26, 419, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":425
  *         return self._prepare(query, <bint> parse_metadata, timeout)
  * 
  *     def begin(self,             # <<<<<<<<<<<<<<
  *               uint32_t isolation,
  *               float tx_timeout=0,
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_29begin, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_begin, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__157)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 425, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_29begin, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_begin, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__156)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__158);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__157);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_begin, __pyx_t_3) < 0) __PYX_ERR(26, 425, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":431
  *         return self._begin(isolation, <double> tx_timeout, timeout)
  * 
  *     def commit(self, float timeout=-1):             # <<<<<<<<<<<<<<
  *         return self._commit(timeout)
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_31commit, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_commit, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__159)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 431, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_31commit, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_commit, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__158)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 431, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__129);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__128);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_commit, __pyx_t_3) < 0) __PYX_ERR(26, 431, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "asynctnt/iproto/db.pyx":434
  *         return self._commit(timeout)
  * 
  *     def rollback(self, float timeout=-1):             # <<<<<<<<<<<<<<
  *         return self._rollback(timeout)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_33rollback, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_rollback, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__160)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 434, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_33rollback, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db_rollback, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__159)); if (unlikely(!__pyx_t_3)) __PYX_ERR(26, 434, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__129);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_3, __pyx_tuple__128);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_Db, __pyx_n_s_rollback, __pyx_t_3) < 0) __PYX_ERR(26, 434, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_Db);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_35__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__161)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_35__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__160)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_37__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__162)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_2Db_37__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Db___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__161)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "asynctnt/iproto/push.pyx":1
  * import asyncio             # <<<<<<<<<<<<<<
  * 
@@ -89339,27 +89401,27 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12PushIterator_12__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PushIterator___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__163)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12PushIterator_12__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PushIterator___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__162)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_PushIterator, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_PushIterator);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_PushIterator, (type(self), 0x98137af, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_PushIterator__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12PushIterator_14__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PushIterator___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__164)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12PushIterator_14__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_PushIterator___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__163)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_PushIterator, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_PushIterator);
 
   /* "asynctnt/iproto/coreproto.pyx":8
  * from libc.stdint cimport uint32_t, uint64_t
@@ -89447,129 +89509,129 @@
  * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_re); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_compile); if (unlikely(!__pyx_t_2)) __PYX_ERR(28, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__165, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 15, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__164, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_VERSION_STRING_REGEX, __pyx_t_3) < 0) __PYX_ERR(28, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "asynctnt/iproto/coreproto.pyx":50
  *         return self.con_state == CONNECTION_FULL
  * 
  *     def is_connected(self):             # <<<<<<<<<<<<<<
  *         return self._is_connected()
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_3is_connected, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_is_connected, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__166)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 50, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_3is_connected, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_is_connected, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__165)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol, __pyx_n_s_is_connected, __pyx_t_3) < 0) __PYX_ERR(28, 50, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol);
 
   /* "asynctnt/iproto/coreproto.pyx":53
  *         return self._is_connected()
  * 
  *     def is_fully_connected(self):             # <<<<<<<<<<<<<<
  *         return self._is_fully_connected()
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_5is_fully_connected, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_is_fully_connected, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__167)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 53, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_5is_fully_connected, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_is_fully_connected, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__166)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol, __pyx_n_s_is_fully_connected, __pyx_t_3) < 0) __PYX_ERR(28, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol);
 
   /* "asynctnt/iproto/coreproto.pyx":56
  *         return self._is_fully_connected()
  * 
  *     def get_version(self):             # <<<<<<<<<<<<<<
  *         return self.version
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_7get_version, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_get_version, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__168)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 56, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_7get_version, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_get_version, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__167)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol, __pyx_n_s_get_version, __pyx_t_3) < 0) __PYX_ERR(28, 56, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol);
 
   /* "asynctnt/iproto/coreproto.pyx":143
  *         self._on_greeting_received()
  * 
  *     def _parse_version(self, version):             # <<<<<<<<<<<<<<
  *         m = VERSION_STRING_REGEX.match(version.decode('ascii'))
  *         if m is not None:
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_9_parse_version, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol__parse_version, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__170)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 143, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_9_parse_version, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol__parse_version, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__169)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol, __pyx_n_s_parse_version, __pyx_t_3) < 0) __PYX_ERR(28, 143, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol);
 
   /* "asynctnt/iproto/coreproto.pyx":163
  *     # asyncio callbacks
  * 
  *     def data_received(self, data):             # <<<<<<<<<<<<<<
  *         self._on_data_received(data)
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_11data_received, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_data_received, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__172)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 163, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_11data_received, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_data_received, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__171)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol, __pyx_n_s_data_received, __pyx_t_3) < 0) __PYX_ERR(28, 163, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol);
 
   /* "asynctnt/iproto/coreproto.pyx":166
  *         self._on_data_received(data)
  * 
  *     def connection_made(self, transport):             # <<<<<<<<<<<<<<
  *         self.transport = transport
  *         self.con_state = CONNECTION_CONNECTED
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_13connection_made, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_connection_made, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__174)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 166, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_13connection_made, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_connection_made, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__173)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol, __pyx_n_s_connection_made, __pyx_t_3) < 0) __PYX_ERR(28, 166, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol);
 
   /* "asynctnt/iproto/coreproto.pyx":179
  *         self._on_connection_made()
  * 
  *     def connection_lost(self, exc):             # <<<<<<<<<<<<<<
  *         self.con_state = CONNECTION_BAD
  *         self.version = None
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_15connection_lost, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_connection_lost, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__176)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 179, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_15connection_lost, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol_connection_lost, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__175)); if (unlikely(!__pyx_t_3)) __PYX_ERR(28, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol, __pyx_n_s_connection_lost, __pyx_t_3) < 0) __PYX_ERR(28, 179, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_17__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__177)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_17__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__176)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_CoreProtocol, (type(self), 0x89d360e, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_CoreProtocol__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_19__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__178)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12CoreProtocol_19__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_CoreProtocol___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__177)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_CoreProtocol);
 
   /* "asynctnt/iproto/protocol.pyx":44
  * 
@@ -89725,103 +89787,103 @@
   /* "asynctnt/iproto/protocol.pyx":108
  *             self.create_future = self._create_future_fallback
  * 
  *     def _create_future_fallback(self):  # pragma: nocover             # <<<<<<<<<<<<<<
  *         return asyncio.Future(loop=self.loop)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_3_create_future_fallback, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol__create_future_fall, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__179)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 108, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_3_create_future_fallback, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol__create_future_fall, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__178)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol, __pyx_n_s_create_future_fallback, __pyx_t_2) < 0) __PYX_ERR(6, 108, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol);
 
   /* "asynctnt/iproto/protocol.pyx":425
  *         return self._last_stream_id
  * 
  *     def _on_request_timeout(self, waiter):             # <<<<<<<<<<<<<<
  *         cdef:
  *             BaseRequest req
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_5_on_request_timeout, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol__on_request_timeout, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__181)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 425, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_5_on_request_timeout, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol__on_request_timeout, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__180)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol, __pyx_n_s_on_request_timeout, __pyx_t_2) < 0) __PYX_ERR(6, 425, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol);
 
   /* "asynctnt/iproto/protocol.pyx":442
  *         )
  * 
  *     def _on_request_completed(self, fut):             # <<<<<<<<<<<<<<
  *         cdef BaseRequest req = (<Response> fut._response).request_
  *         fut._response = None
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_7_on_request_completed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol__on_request_complet, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__183)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 442, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_7_on_request_completed, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol__on_request_complet, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__182)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 442, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol, __pyx_n_s_on_request_completed, __pyx_t_2) < 0) __PYX_ERR(6, 442, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol);
 
   /* "asynctnt/iproto/protocol.pyx":473
  *         return Db.create(self, stream_id)
  * 
  *     def create_db(self, bint gen_stream_id = False):             # <<<<<<<<<<<<<<
  *         return self._create_db(gen_stream_id)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_9create_db, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol_create_db, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__185)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 473, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_9create_db, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol_create_db, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__184)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 473, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__186);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__185);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol, __pyx_n_s_create_db, __pyx_t_2) < 0) __PYX_ERR(6, 473, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol);
 
   /* "asynctnt/iproto/protocol.pyx":476
  *         return self._create_db(gen_stream_id)
  * 
  *     def get_common_db(self):             # <<<<<<<<<<<<<<
  *         return self._db
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_11get_common_db, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol_get_common_db, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__187)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 476, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_11get_common_db, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol_get_common_db, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__186)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol, __pyx_n_s_get_common_db, __pyx_t_2) < 0) __PYX_ERR(6, 476, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol);
 
   /* "asynctnt/iproto/protocol.pyx":515
  *         return self._refetch_schema_future
  * 
  *     def refetch_schema(self):             # <<<<<<<<<<<<<<
  *         return self._refetch_schema()
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_13refetch_schema, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol_refetch_schema, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__188)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 515, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_13refetch_schema, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol_refetch_schema, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__187)); if (unlikely(!__pyx_t_2)) __PYX_ERR(6, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol, __pyx_n_s_refetch_schema, __pyx_t_2) < 0) __PYX_ERR(6, 515, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_8asynctnt_6iproto_8protocol_BaseProtocol);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.execute cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_15__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__189)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_15__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol___reduce_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__188)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "self.execute cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.execute cannot be converted to a Python object for pickling"
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_17__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__190)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_12BaseProtocol_17__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseProtocol___setstate_cython, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__189)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "asynctnt/iproto/protocol.pyx":519
  * 
  * 
@@ -89861,225 +89923,225 @@
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_BaseRequest(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_1__pyx_unpickle_BaseRequest, 0, __pyx_n_s_pyx_unpickle_BaseRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__192)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_1__pyx_unpickle_BaseRequest, 0, __pyx_n_s_pyx_unpickle_BaseRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__191)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_BaseRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_BaseRequest__set_state(<BaseRequest> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_BaseRequest__set_state(BaseRequest __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.check_schema_change = __pyx_state[0]; __pyx_result.op = __pyx_state[1]; __pyx_result.parse_as_tuples = __pyx_state[2]; __pyx_result.parse_metadata = __pyx_state[3]; __pyx_result.push_subscribe = __pyx_state[4]; __pyx_result.schema_id = __pyx_state[5]; __pyx_result.space = __pyx_state[6]; __pyx_result.stream_id = __pyx_state[7]; __pyx_result.sync = __pyx_state[8]; __pyx_result.timeout_handle = __pyx_state[9]; __pyx_result.waiter = __pyx_state[10]
  *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_3__pyx_unpickle_PingRequest, 0, __pyx_n_s_pyx_unpickle_PingRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__193)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_3__pyx_unpickle_PingRequest, 0, __pyx_n_s_pyx_unpickle_PingRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__192)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_PingRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_CallRequest(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_5__pyx_unpickle_CallRequest, 0, __pyx_n_s_pyx_unpickle_CallRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__194)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_5__pyx_unpickle_CallRequest, 0, __pyx_n_s_pyx_unpickle_CallRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__193)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_CallRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_CallRequest__set_state(<CallRequest> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_CallRequest__set_state(CallRequest __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.args = __pyx_state[0]; __pyx_result.check_schema_change = __pyx_state[1]; __pyx_result.func_name = __pyx_state[2]; __pyx_result.op = __pyx_state[3]; __pyx_result.parse_as_tuples = __pyx_state[4]; __pyx_result.parse_metadata = __pyx_state[5]; __pyx_result.push_subscribe = __pyx_state[6]; __pyx_result.schema_id = __pyx_state[7]; __pyx_result.space = __pyx_state[8]; __pyx_result.stream_id = __pyx_state[9]; __pyx_result.sync = __pyx_state[10]; __pyx_result.timeout_handle = __pyx_state[11]; __pyx_result.waiter = __pyx_state[12]
  *     if len(__pyx_state) > 13 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_7__pyx_unpickle_EvalRequest, 0, __pyx_n_s_pyx_unpickle_EvalRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__195)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_7__pyx_unpickle_EvalRequest, 0, __pyx_n_s_pyx_unpickle_EvalRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__194)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_EvalRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_SelectRequest(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_9__pyx_unpickle_SelectRequest, 0, __pyx_n_s_pyx_unpickle_SelectRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__196)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_9__pyx_unpickle_SelectRequest, 0, __pyx_n_s_pyx_unpickle_SelectRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__195)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_SelectRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_SelectRequest__set_state(<SelectRequest> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_SelectRequest__set_state(SelectRequest __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.check_schema_change = __pyx_state[0]; __pyx_result.index = __pyx_state[1]; __pyx_result.iterator = __pyx_state[2]; __pyx_result.key = __pyx_state[3]; __pyx_result.limit = __pyx_state[4]; __pyx_result.offset = __pyx_state[5]; __pyx_result.op = __pyx_state[6]; __pyx_result.parse_as_tuples = __pyx_state[7]; __pyx_result.parse_metadata = __pyx_state[8]; __pyx_result.push_subscribe = __pyx_state[9]; __pyx_result.schema_id = __pyx_state[10]; __pyx_result.space = __pyx_state[11]; __pyx_result.stream_id = __pyx_state[12]; __pyx_result.sync = __pyx_state[13]; __pyx_result.timeout_handle = __pyx_state[14]; __pyx_result.waiter = __pyx_state[15]
  *     if len(__pyx_state) > 16 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11__pyx_unpickle_InsertRequest, 0, __pyx_n_s_pyx_unpickle_InsertRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__197)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_11__pyx_unpickle_InsertRequest, 0, __pyx_n_s_pyx_unpickle_InsertRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__196)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_InsertRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_DeleteRequest(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13__pyx_unpickle_DeleteRequest, 0, __pyx_n_s_pyx_unpickle_DeleteRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__198)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_13__pyx_unpickle_DeleteRequest, 0, __pyx_n_s_pyx_unpickle_DeleteRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__197)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_DeleteRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_DeleteRequest__set_state(<DeleteRequest> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_DeleteRequest__set_state(DeleteRequest __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.check_schema_change = __pyx_state[0]; __pyx_result.index = __pyx_state[1]; __pyx_result.key = __pyx_state[2]; __pyx_result.op = __pyx_state[3]; __pyx_result.parse_as_tuples = __pyx_state[4]; __pyx_result.parse_metadata = __pyx_state[5]; __pyx_result.push_subscribe = __pyx_state[6]; __pyx_result.schema_id = __pyx_state[7]; __pyx_result.space = __pyx_state[8]; __pyx_result.stream_id = __pyx_state[9]; __pyx_result.sync = __pyx_state[10]; __pyx_result.timeout_handle = __pyx_state[11]; __pyx_result.waiter = __pyx_state[12]
  *     if len(__pyx_state) > 13 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_15__pyx_unpickle_UpdateRequest, 0, __pyx_n_s_pyx_unpickle_UpdateRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__199)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_15__pyx_unpickle_UpdateRequest, 0, __pyx_n_s_pyx_unpickle_UpdateRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__198)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_UpdateRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_UpsertRequest(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_17__pyx_unpickle_UpsertRequest, 0, __pyx_n_s_pyx_unpickle_UpsertRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__200)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_17__pyx_unpickle_UpsertRequest, 0, __pyx_n_s_pyx_unpickle_UpsertRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__199)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_UpsertRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_UpsertRequest__set_state(<UpsertRequest> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_UpsertRequest__set_state(UpsertRequest __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.check_schema_change = __pyx_state[0]; __pyx_result.op = __pyx_state[1]; __pyx_result.operations = __pyx_state[2]; __pyx_result.parse_as_tuples = __pyx_state[3]; __pyx_result.parse_metadata = __pyx_state[4]; __pyx_result.push_subscribe = __pyx_state[5]; __pyx_result.schema_id = __pyx_state[6]; __pyx_result.space = __pyx_state[7]; __pyx_result.stream_id = __pyx_state[8]; __pyx_result.sync = __pyx_state[9]; __pyx_result.t = __pyx_state[10]; __pyx_result.timeout_handle = __pyx_state[11]; __pyx_result.waiter = __pyx_state[12]
  *     if len(__pyx_state) > 13 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_19__pyx_unpickle_PrepareRequest, 0, __pyx_n_s_pyx_unpickle_PrepareRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__201)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_19__pyx_unpickle_PrepareRequest, 0, __pyx_n_s_pyx_unpickle_PrepareRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__200)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_PrepareRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_ExecuteRequest(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_21__pyx_unpickle_ExecuteRequest, 0, __pyx_n_s_pyx_unpickle_ExecuteRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__202)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_21__pyx_unpickle_ExecuteRequest, 0, __pyx_n_s_pyx_unpickle_ExecuteRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__201)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_ExecuteRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_ExecuteRequest__set_state(<ExecuteRequest> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_ExecuteRequest__set_state(ExecuteRequest __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.args = __pyx_state[0]; __pyx_result.check_schema_change = __pyx_state[1]; __pyx_result.op = __pyx_state[2]; __pyx_result.parse_as_tuples = __pyx_state[3]; __pyx_result.parse_metadata = __pyx_state[4]; __pyx_result.push_subscribe = __pyx_state[5]; __pyx_result.query = __pyx_state[6]; __pyx_result.schema_id = __pyx_state[7]; __pyx_result.space = __pyx_state[8]; __pyx_result.statement_id = __pyx_state[9]; __pyx_result.stream_id = __pyx_state[10]; __pyx_result.sync = __pyx_state[11]; __pyx_result.timeout_handle = __pyx_state[12]; __pyx_result.waiter = __pyx_state[13]
  *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_23__pyx_unpickle_IDRequest, 0, __pyx_n_s_pyx_unpickle_IDRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__203)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_23__pyx_unpickle_IDRequest, 0, __pyx_n_s_pyx_unpickle_IDRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__202)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_IDRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_AuthRequest(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_25__pyx_unpickle_AuthRequest, 0, __pyx_n_s_pyx_unpickle_AuthRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__204)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_25__pyx_unpickle_AuthRequest, 0, __pyx_n_s_pyx_unpickle_AuthRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__203)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_AuthRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_AuthRequest__set_state(<AuthRequest> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_AuthRequest__set_state(AuthRequest __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.check_schema_change = __pyx_state[0]; __pyx_result.op = __pyx_state[1]; __pyx_result.parse_as_tuples = __pyx_state[2]; __pyx_result.parse_metadata = __pyx_state[3]; __pyx_result.password = __pyx_state[4]; __pyx_result.push_subscribe = __pyx_state[5]; __pyx_result.salt = __pyx_state[6]; __pyx_result.schema_id = __pyx_state[7]; __pyx_result.space = __pyx_state[8]; __pyx_result.stream_id = __pyx_state[9]; __pyx_result.sync = __pyx_state[10]; __pyx_result.timeout_handle = __pyx_state[11]; __pyx_result.username = __pyx_state[12]; __pyx_result.waiter = __pyx_state[13]
  *     if len(__pyx_state) > 14 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_27__pyx_unpickle_BeginRequest, 0, __pyx_n_s_pyx_unpickle_BeginRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__205)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_27__pyx_unpickle_BeginRequest, 0, __pyx_n_s_pyx_unpickle_BeginRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__204)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_BeginRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_CommitRequest(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_29__pyx_unpickle_CommitRequest, 0, __pyx_n_s_pyx_unpickle_CommitRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__206)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_29__pyx_unpickle_CommitRequest, 0, __pyx_n_s_pyx_unpickle_CommitRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__205)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_CommitRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_CommitRequest__set_state(<CommitRequest> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_CommitRequest__set_state(CommitRequest __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.check_schema_change = __pyx_state[0]; __pyx_result.op = __pyx_state[1]; __pyx_result.parse_as_tuples = __pyx_state[2]; __pyx_result.parse_metadata = __pyx_state[3]; __pyx_result.push_subscribe = __pyx_state[4]; __pyx_result.schema_id = __pyx_state[5]; __pyx_result.space = __pyx_state[6]; __pyx_result.stream_id = __pyx_state[7]; __pyx_result.sync = __pyx_state[8]; __pyx_result.timeout_handle = __pyx_state[9]; __pyx_result.waiter = __pyx_state[10]
  *     if len(__pyx_state) > 11 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_31__pyx_unpickle_RollbackRequest, 0, __pyx_n_s_pyx_unpickle_RollbackRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__207)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_31__pyx_unpickle_RollbackRequest, 0, __pyx_n_s_pyx_unpickle_RollbackRequest, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__206)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_RollbackRequest, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_IProtoErrorStackFrame(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_33__pyx_unpickle_IProtoErrorStackFrame, 0, __pyx_n_s_pyx_unpickle_IProtoErrorStackF, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__208)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_33__pyx_unpickle_IProtoErrorStackFrame, 0, __pyx_n_s_pyx_unpickle_IProtoErrorStackF, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__207)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_IProtoErrorStackF, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_IProtoErrorStackFrame__set_state(<IProtoErrorStackFrame> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_IProtoErrorStackFrame__set_state(IProtoErrorStackFrame __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.code = __pyx_state[0]; __pyx_result.err_no = __pyx_state[1]; __pyx_result.error_type = __pyx_state[2]; __pyx_result.fields = __pyx_state[3]; __pyx_result.file = __pyx_state[4]; __pyx_result.line = __pyx_state[5]; __pyx_result.message = __pyx_state[6]
  *     if len(__pyx_state) > 7 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_35__pyx_unpickle_IProtoError, 0, __pyx_n_s_pyx_unpickle_IProtoError, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__209)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_35__pyx_unpickle_IProtoError, 0, __pyx_n_s_pyx_unpickle_IProtoError, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__208)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_IProtoError, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_PushIterator(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_37__pyx_unpickle_PushIterator, 0, __pyx_n_s_pyx_unpickle_PushIterator, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__210)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_37__pyx_unpickle_PushIterator, 0, __pyx_n_s_pyx_unpickle_PushIterator, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__209)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_PushIterator, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "(tree fragment)":11
  *         __pyx_unpickle_PushIterator__set_state(<PushIterator> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_PushIterator__set_state(PushIterator __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result._fut = __pyx_state[0]; __pyx_result._request = __pyx_state[1]; __pyx_result._response = __pyx_state[2]
  *     if len(__pyx_state) > 3 and hasattr(__pyx_result, '__dict__'):
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_39__pyx_unpickle_CoreProtocol, 0, __pyx_n_s_pyx_unpickle_CoreProtocol, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__211)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_8asynctnt_6iproto_8protocol_39__pyx_unpickle_CoreProtocol, 0, __pyx_n_s_pyx_unpickle_CoreProtocol, NULL, __pyx_n_s_asynctnt_iproto_protocol, __pyx_d, ((PyObject *)__pyx_codeobj__210)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_CoreProtocol, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "asynctnt/iproto/protocol.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * 
@@ -96341,15 +96403,15 @@
         return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
     }
     return module;
 }
 #endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__66;
+    PyObject *module, *from_list, *star = __pyx_n_s__65;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
@@ -100349,15 +100411,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__212);
+        name = __Pyx_NewRef(__pyx_n_s__211);
     }
     return name;
 }
 #endif
 
 /* FastTypeChecks */
   #if CYTHON_COMPILING_IN_CPYTHON
```

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/protocol.h` & `asynctnt-2.2.0/asynctnt/iproto/protocol.h`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/protocol.pxd` & `asynctnt-2.2.0/asynctnt/iproto/protocol.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/protocol.pyi` & `asynctnt-2.2.0/asynctnt/iproto/protocol.pyi`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/protocol.pyx` & `asynctnt-2.2.0/asynctnt/iproto/protocol.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/push.pyx` & `asynctnt-2.2.0/asynctnt/iproto/push.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/python.pxd` & `asynctnt-2.2.0/asynctnt/iproto/python.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/rbuffer.pxd` & `asynctnt-2.2.0/asynctnt/iproto/rbuffer.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/rbuffer.pyx` & `asynctnt-2.2.0/asynctnt/iproto/rbuffer.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/auth.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/auth.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/base.pxd` & `asynctnt-2.2.0/asynctnt/iproto/requests/base.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/base.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/base.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/call.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/call.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/delete.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/delete.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/eval.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/eval.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/execute.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/execute.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/id.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/id.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/insert.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/insert.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/prepare.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/prepare.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/select.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/select.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/streams.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/streams.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/update.pxd` & `asynctnt-2.2.0/asynctnt/iproto/requests/update.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/requests/update.pyx` & `asynctnt-2.2.0/asynctnt/iproto/requests/update.pyx`

 * *Files 19% similar despite different names*

```diff
@@ -19,19 +19,25 @@
 
         char *op_str_c
         ssize_t op_str_len
         char op
 
         uint32_t extra_length
 
+        bint field_encode_as_str
         uint64_t field_no
+        char *field_str_c
+        ssize_t field_str_len
         object field_no_obj
 
         uint32_t splice_position, splice_offset
 
+    field_encode_as_str = 0
+    field_str_c = NULL
+
     begin = NULL
 
     if operations is not None:
         ops_len = <uint32_t> cpython.list.PyList_GET_SIZE(operations)
     else:
         ops_len = 0
 
@@ -56,76 +62,68 @@
             str_temp = encode_unicode_string(op_type_str, buffer._encoding)
         elif isinstance(op_type_str, bytes):
             str_temp = <bytes> op_type_str
         else:
             raise TypeError(
                 'Operation type must of a str or bytes type')
 
+        cpython.bytes.PyBytes_AsStringAndSize(str_temp, &op_str_c,
+                                              &op_str_len)
+
         field_no_obj = operation[1]
         if isinstance(field_no_obj, int):
             field_no = <int> field_no_obj
         elif isinstance(field_no_obj, str):
             if space.metadata is not None:
-                field_no = <int> space.metadata.id_by_name(field_no_obj)
+                field_no = <int> space.metadata.id_by_name_safe(field_no_obj)
+                if field_no == -1:
+                    field_encode_as_str = 1
             else:
-                raise TypeError(
-                    'Operation field_no must be int as there is '
-                    'no format declaration in space {}'.format(space.sid))
+                field_encode_as_str = 1
+
+            if field_encode_as_str:
+                str_temp = encode_unicode_string(field_no_obj, buffer._encoding)
+                cpython.bytes.PyBytes_AsStringAndSize(str_temp, &field_str_c, &field_str_len)
         else:
             raise TypeError(
                 'Operation field_no must be of either int or str type')
 
-        cpython.bytes.PyBytes_AsStringAndSize(str_temp, &op_str_c,
-                                              &op_str_len)
         op = <char> 0
         if op_str_len == 1:
             op = op_str_c[0]
 
         if op == tarantool.IPROTO_OP_ADD \
                 or op == tarantool.IPROTO_OP_SUB \
                 or op == tarantool.IPROTO_OP_AND \
                 or op == tarantool.IPROTO_OP_XOR \
                 or op == tarantool.IPROTO_OP_OR \
-                or op == tarantool.IPROTO_OP_DELETE:
-            op_argument = operation[2]
-            if not isinstance(op_argument, int):
-                raise TypeError(
-                    'int argument required for '
-                    'Arithmetic and Delete operations'
-                )
-            # mp_sizeof_array(3)
-            # + mp_sizeof_str(1)
-            # + mp_sizeof_uint(field_no)
-            extra_length = 1 + 2 + mp_sizeof_uint(field_no)
-            p = begin = buffer._ensure_allocated(p, extra_length)
-
-            p = mp_encode_array(p, 3)
-            p = mp_encode_str(p, op_str_c, 1)
-            p = mp_encode_uint(p, field_no)
-            buffer._length += (p - begin)
-            p = buffer.mp_encode_obj(p, op_argument)
-        elif op == tarantool.IPROTO_OP_INSERT \
+                or op == tarantool.IPROTO_OP_DELETE \
+                or op == tarantool.IPROTO_OP_INSERT \
                 or op == tarantool.IPROTO_OP_ASSIGN:
-            op_argument = operation[2]
-
             # mp_sizeof_array(3)
             # + mp_sizeof_str(1)
             # + mp_sizeof_uint(field_no)
             extra_length = 1 + 2 + mp_sizeof_uint(field_no)
             p = begin = buffer._ensure_allocated(p, extra_length)
 
             p = mp_encode_array(p, 3)
             p = mp_encode_str(p, op_str_c, 1)
-            p = mp_encode_uint(p, field_no)
+            if field_str_c == NULL:
+                p = mp_encode_uint(p, field_no)
+            else:
+                p = mp_encode_str(p, field_str_c, field_str_len)
+
             buffer._length += (p - begin)
+
+            op_argument = operation[2]
             p = buffer.mp_encode_obj(p, op_argument)
 
         elif op == tarantool.IPROTO_OP_SPLICE:
             if op_len < 5:
-                raise IndexError(
+                raise ValueError(
                     'Splice operation must have length of 5, '
                     'but got: {}'.format(op_len)
                 )
 
             splice_position_obj = operation[2]
             splice_offset_obj = operation[3]
             op_argument = operation[4]
@@ -142,15 +140,18 @@
                            + mp_sizeof_uint(field_no) \
                            + mp_sizeof_uint(splice_position) \
                            + mp_sizeof_uint(splice_offset)
             p = begin = buffer._ensure_allocated(p, extra_length)
 
             p = mp_encode_array(p, 5)
             p = mp_encode_str(p, op_str_c, 1)
-            p = mp_encode_uint(p, field_no)
+            if field_str_c == NULL:
+                p = mp_encode_uint(p, field_no)
+            else:
+                p = mp_encode_str(p, field_str_c, field_str_len)
             p = mp_encode_uint(p, splice_position)
             p = mp_encode_uint(p, splice_offset)
             buffer._length += (p - begin)
             p = buffer.mp_encode_obj(p, op_argument)
         else:
             raise TypeError(
                 'Unknown update operation type `{}`'.format(op_type_str))
```

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/response.pxd` & `asynctnt-2.2.0/asynctnt/iproto/response.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/response.pyx` & `asynctnt-2.2.0/asynctnt/iproto/response.pyx`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/schema.pxd` & `asynctnt-2.2.0/asynctnt/iproto/schema.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         readonly dict name_id_map
         list names
 
     cdef inline int len(self)
     cdef inline void add(self, int id, Field field)
     cdef inline str name_by_id(self, int i)
     cdef inline int id_by_name(self, str name) except *
+    cdef inline int id_by_name_safe(self, str name) except*
 
 
 cdef class SchemaIndex:
     cdef:
         readonly int sid
         readonly int iid
         readonly str name
```

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/schema.pyx` & `asynctnt-2.2.0/asynctnt/iproto/schema.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,23 @@
             PyObject *fld
 
         fld = cpython.dict.PyDict_GetItem(self.name_id_map, name)
         if fld == NULL:
             raise KeyError('Field \'{}\' not found'.format(name))
         return <int> <object> fld
 
+    cdef inline int id_by_name_safe(self, str name) except *:
+        cdef:
+            PyObject *fld
+
+        fld = cpython.dict.PyDict_GetItem(self.name_id_map, name)
+        if fld == NULL:
+            return -1
+        return <int> <object> fld
+
     cdef inline int len(self):
         return <int> cpython.list.PyList_GET_SIZE(self.fields)
 
     def __repr__(self):  # pragma: nocover
         return '<Metadata [fields_count={}]>'.format(self.len())
 
 @cython.final
```

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/tarantool.pxd` & `asynctnt-2.2.0/asynctnt/iproto/tarantool.pxd`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/tupleobj/tupleobj.c` & `asynctnt-2.2.0/asynctnt/iproto/tupleobj/tupleobj.c`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/iproto/tupleobj/tupleobj.h` & `asynctnt-2.2.0/asynctnt/iproto/tupleobj/tupleobj.h`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/prepared.py` & `asynctnt-2.2.0/asynctnt/prepared.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt/stream.py` & `asynctnt-2.2.0/asynctnt/stream.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/asynctnt.egg-info/PKG-INFO` & `asynctnt-2.2.0/asynctnt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asynctnt
-Version: 2.1.0a1
+Version: 2.2.0
 Summary: A fast Tarantool Database connector for Python/asyncio.
 Author-email: igorcoding <igorcoding@gmail.com>
 License: Apache License, Version 2.0
 Project-URL: github, https://github.com/igorcoding/asynctnt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: POSIX
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asynctnt Version: 2.1.0a1 Summary: A fast Tarantool
+Metadata-Version: 2.1 Name: asynctnt Version: 2.2.0 Summary: A fast Tarantool
 Database connector for Python/asyncio. Author-email: igorcoding
 gmail.com> License: Apache License, Version 2.0 Project-URL: github, https://
 github.com/igorcoding/asynctnt Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: AsyncIO Classifier: Operating System
 :: POSIX Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
```

### Comparing `asynctnt-2.1.0a1/asynctnt.egg-info/SOURCES.txt` & `asynctnt-2.2.0/asynctnt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/pyproject.toml` & `asynctnt-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -116,23 +116,23 @@
 skip_glob = [
     "env*",
     "venv*",
 ]
 
 
 [tool.ruff]
-select = [
+lint.select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     # "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
-ignore = [
+lint.ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "C901",  # too complex
 ]
 
 extend-exclude = [
     "app/store/migrations",
```

### Comparing `asynctnt-2.1.0a1/setup.py` & `asynctnt-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/__init__.py` & `asynctnt-2.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/_testbase.py` & `asynctnt-2.2.0/tests/_testbase.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_common.py` & `asynctnt-2.2.0/tests/test_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,17 @@
         d = {1: 1, 2: 2, "hello": 3, "world": 4, -3: 5, 4.5: 6}
 
         self.assertDictEqual(res[0], d, "Numeric keys parsed ok")
 
     async def test__read_buffer_reallocate_ok(self):
         await self.tnt_reconnect(initial_read_buffer_size=1)
 
-        p, cmp = get_complex_param(encoding=self.conn.encoding)
+        p, cmp = get_complex_param(
+            encoding=self.conn.encoding, replace_bin=self.conn.version < (3, 0)
+        )
         try:
             res = await self.conn.call("func_param", [p])
         except Exception as e:
             self.fail(e)
 
         self.assertDictEqual(res[0][0], cmp, "Body ok")
```

### Comparing `asynctnt-2.1.0a1/tests/test_connect.py` & `asynctnt-2.2.0/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_mp_ext.py` & `asynctnt-2.2.0/tests/test_mp_ext.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_op_call.py` & `asynctnt-2.2.0/tests/test_op_call.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,20 +75,24 @@
     async def test__call_args_tuple(self):
         try:
             await self.conn.call("func_param", (1, 2))
         except Exception as e:
             self.fail(e)
 
     async def test__call_complex_param(self):
-        p, cmp = get_complex_param(encoding=self.conn.encoding)
+        p, cmp = get_complex_param(
+            encoding=self.conn.encoding, replace_bin=self.conn.version < (3, 0)
+        )
         res = await self.conn.call("func_param", [p])
         self.assertDictEqual(res[0][0], cmp, "Body ok")
 
     async def test__call_complex_param_bare(self):
-        p, cmp = get_complex_param(encoding=self.conn.encoding)
+        p, cmp = get_complex_param(
+            encoding=self.conn.encoding, replace_bin=self.conn.version < (3, 0)
+        )
         cmp = [cmp]
         res = await self.conn.call("func_param_bare", [p])
         if not self.has_new_call():
             cmp = [cmp]
         self.assertResponseEqual(res, cmp, "Body ok")
 
     async def test__call_timeout_in_time(self):
@@ -173,20 +177,24 @@
     async def test__call16_args_tuple(self):
         try:
             await self.conn.call16("func_param", (1, 2))
         except Exception as e:
             self.fail(e)
 
     async def test__call16_complex_param(self):
-        p, cmp = get_complex_param(encoding=self.conn.encoding)
+        p, cmp = get_complex_param(
+            encoding=self.conn.encoding, replace_bin=self.conn.version < (3, 0)
+        )
         res = await self.conn.call("func_param", [p])
         self.assertDictEqual(res[0][0], cmp, "Body ok")
 
     async def test__call16_complex_param_bare(self):
-        p, cmp = get_complex_param(encoding=self.conn.encoding)
+        p, cmp = get_complex_param(
+            encoding=self.conn.encoding, replace_bin=self.conn.version < (3, 0)
+        )
         res = await self.conn.call16("func_param_bare", [p])
         self.assertDictEqual(res[0][0], cmp, "Body ok")
 
     async def test__call16_timeout_in_time(self):
         try:
             await self.conn.call16("func_long", [0.1], timeout=1)
         except Exception as e:
```

### Comparing `asynctnt-2.1.0a1/tests/test_op_delete.py` & `asynctnt-2.2.0/tests/test_op_delete.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_op_eval.py` & `asynctnt-2.2.0/tests/test_op_eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,17 @@
     async def test__eval_args_tuple(self):
         try:
             await self.conn.eval("return {...}", (1, 2))
         except Exception as e:
             self.fail(e)
 
     async def test__eval_complex_param(self):
-        p, cmp = get_complex_param(encoding=self.conn.encoding)
+        p, cmp = get_complex_param(
+            encoding=self.conn.encoding, replace_bin=self.conn.version < (3, 0)
+        )
         res = await self.conn.eval("return {...}", [p])
         self.assertDictEqual(res[0][0], cmp, "Body ok")
 
     async def test__eval_timeout_in_time(self):
         try:
             cmd = """
             local args = {...}
```

### Comparing `asynctnt-2.1.0a1/tests/test_op_insert.py` & `asynctnt-2.2.0/tests/test_op_insert.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_op_ping.py` & `asynctnt-2.2.0/tests/test_op_ping.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_op_push.py` & `asynctnt-2.2.0/tests/test_op_push.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_op_select.py` & `asynctnt-2.2.0/tests/test_op_select.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_op_sql_execute.py` & `asynctnt-2.2.0/tests/test_op_sql_execute.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+import asynctnt
 from asynctnt import Response
 from tests import BaseTarantoolTestCase
 from tests._testbase import ensure_version
 
 
 class SQLExecuteTestCase(BaseTarantoolTestCase):
+    def _compat_field_name(self, field_name: str) -> str:
+        if self.conn.version >= (3, 0):
+            return field_name
+        return field_name.upper()
+
     @ensure_version(min=(2, 0))
     async def test__sql_basic(self):
         res = await self.conn.execute("select 1, 2")
 
         self.assertIsInstance(res, Response, "Got response")
         self.assertEqual(res.code, 0, "success")
         self.assertGreater(res.sync, 0, "sync > 0")
@@ -19,44 +25,80 @@
 
         self.assertResponseEqual(res, [[1, 2]], "Body ok")
 
     @ensure_version(min=(2, 0))
     async def test__sql_with_param_cols(self):
         res = await self.conn.execute("select 1 as a, 2 as b where 1 = ?", [1])
 
-        self.assertResponseEqualKV(res, [{"A": 1, "B": 2}], "Body ok")
+        self.assertResponseEqualKV(
+            res,
+            [
+                {
+                    self._compat_field_name("a"): 1,
+                    self._compat_field_name("b"): 2,
+                }
+            ],
+            "Body ok",
+        )
 
     @ensure_version(min=(2, 0))
     async def test__sql_with_param_cols2(self):
         res = await self.conn.execute(
             "select 1 as a, 2 as b where 1 = ? and 2 = ?", [1, 2]
         )
 
-        self.assertResponseEqualKV(res, [{"A": 1, "B": 2}], "Body ok")
+        self.assertResponseEqualKV(
+            res,
+            [
+                {
+                    self._compat_field_name("a"): 1,
+                    self._compat_field_name("b"): 2,
+                }
+            ],
+            "Body ok",
+        )
 
     @ensure_version(min=(2, 0))
     async def test__sql_with_param_cols_maps(self):
         res = await self.conn.execute(
             "select 1 as a, 2 as b where 1 = :p1 and 2 = :p2",
             [
                 {":p1": 1},
                 {":p2": 2},
             ],
         )
 
-        self.assertResponseEqualKV(res, [{"A": 1, "B": 2}], "Body ok")
+        self.assertResponseEqualKV(
+            res,
+            [
+                {
+                    self._compat_field_name("a"): 1,
+                    self._compat_field_name("b"): 2,
+                }
+            ],
+            "Body ok",
+        )
 
     @ensure_version(min=(2, 0))
     async def test__sql_with_param_cols_maps_and_positional(self):
         res = await self.conn.execute(
-            "select 1 as a, 2 as b " "where 1 = :p1 and 2 = :p2 and 3 = ? and 4 = ?",
+            "select 1 as a, 2 as b where 1 = :p1 and 2 = :p2 and 3 = ? and 4 = ?",
             [{":p1": 1}, {":p2": 2}, 3, 4],
         )
 
-        self.assertResponseEqualKV(res, [{"A": 1, "B": 2}], "Body ok")
+        self.assertResponseEqualKV(
+            res,
+            [
+                {
+                    self._compat_field_name("a"): 1,
+                    self._compat_field_name("b"): 2,
+                }
+            ],
+            "Body ok",
+        )
 
     @ensure_version(min=(2, 0))
     async def test__sql_insert(self):
         res = await self.conn.execute(
             "insert into sql_space (id, name) values (1, 'one')"
         )
         self.assertEqual(1, res.rowcount, "rowcount ok")
@@ -107,32 +149,38 @@
 
         res = await self.conn.execute("update sql_space set name = 'uno'")
 
         self.assertEqual(2, res.rowcount, "rowcount ok")
 
     @ensure_version(min=(2, 0))
     async def test__sql_delete(self):
+        await self._compat(self.conn)
+
         await self.conn.execute("insert into sql_space values (1, 'one')")
         res = await self.conn.execute("delete from sql_space where name = 'one'")
         self.assertEqual(1, res.rowcount, "rowcount ok")
 
     @ensure_version(min=(2, 0))
     async def test__sql_select(self):
+        await self._compat(self.conn)
+
         await self.conn.execute("insert into sql_space values (1, 'one')")
         await self.conn.execute("insert into sql_space values (2, 'two')")
 
         res = await self.conn.execute("select * from sql_space")
         self.assertEqual(2, res.rowcount, "rowcount is surely ok")
-        self.assertEqual(1, res.body[0]["ID"])
-        self.assertEqual("one", res.body[0]["NAME"])
-        self.assertEqual(2, res.body[1]["ID"])
-        self.assertEqual("two", res.body[1]["NAME"])
+        self.assertEqual(1, res.body[0][self._compat_field_name("id")])
+        self.assertEqual("one", res.body[0][self._compat_field_name("name")])
+        self.assertEqual(2, res.body[1][self._compat_field_name("id")])
+        self.assertEqual("two", res.body[1][self._compat_field_name("name")])
 
     @ensure_version(min=(2, 0))
     async def test__sql_delete_multiple(self):
+        await self._compat(self.conn)
+
         await self.conn.execute("insert into sql_space values (1, 'one')")
         await self.conn.execute("insert into sql_space values (2, 'two')")
 
         res = await self.conn.execute("delete from sql_space")
         self.assertEqual(2, res.rowcount, "rowcount ok")
 
         res = await self.conn.execute("select * from sql_space")
@@ -148,64 +196,76 @@
         self.assertEqual("COLUMN_1", res.metadata.fields[0].name)
         self.assertEqual("integer", res.metadata.fields[0].type)
         self.assertEqual("COLUMN_2", res.metadata.fields[1].name)
         self.assertEqual("integer", res.metadata.fields[1].type)
 
     @ensure_version(min=(2, 0))
     async def test__metadata_names(self):
+        await self._compat(self.conn)
+
         res = await self.conn.execute("select 1 as a, 2 as b")
         self.assertIsNotNone(res.metadata)
         self.assertIsNotNone(res.metadata.fields)
         self.assertEqual(2, len(res.metadata.fields))
 
-        self.assertEqual("A", res.metadata.fields[0].name)
+        self.assertEqual(self._compat_field_name("a"), res.metadata.fields[0].name)
         self.assertEqual("integer", res.metadata.fields[0].type)
-        self.assertEqual("B", res.metadata.fields[1].name)
+        self.assertEqual(self._compat_field_name("b"), res.metadata.fields[1].name)
         self.assertEqual("integer", res.metadata.fields[1].type)
 
     @ensure_version(min=(2, 0))
     async def test__metadata_actual_space(self):
+        await self._compat(self.conn)
+
         await self.conn.execute("insert into sql_space values (1, 'one')")
         await self.conn.execute("insert into sql_space values (2, 'two')")
 
         res = await self.conn.execute("select * from sql_space")
         self.assertEqual(2, res.rowcount, "rowcount is ok")
         self.assertEqual(2, len(res.metadata.fields))
-        self.assertEqual("ID", res.metadata.fields[0].name)
+        self.assertEqual(self._compat_field_name("id"), res.metadata.fields[0].name)
         self.assertEqual("integer", res.metadata.fields[0].type)
         self.assertIsNone(res.metadata.fields[0].is_nullable)
         self.assertIsNone(res.metadata.fields[0].is_autoincrement)
         self.assertIsNone(res.metadata.fields[0].collation)
 
-        self.assertEqual("NAME", res.metadata.fields[1].name)
+        self.assertEqual(self._compat_field_name("name"), res.metadata.fields[1].name)
         self.assertEqual("string", res.metadata.fields[1].type)
         self.assertIsNone(res.metadata.fields[1].is_nullable)
         self.assertIsNone(res.metadata.fields[1].is_autoincrement)
         self.assertIsNone(res.metadata.fields[1].collation)
 
     @ensure_version(min=(2, 0))
     async def test__sql_select_full_metadata(self):
+        await self._compat(self.conn)
+
         await self.conn.execute("insert into sql_space values (1, 'one')")
         await self.conn.execute("insert into sql_space values (2, 'two')")
 
         await self.conn.update(
             "_session_settings", ["sql_full_metadata"], [("=", "value", True)]
         )
 
         try:
             res = await self.conn.execute("select * from sql_space")
             self.assertEqual(2, len(res.metadata.fields))
-            self.assertEqual("ID", res.metadata.fields[0].name)
+            self.assertEqual(self._compat_field_name("id"), res.metadata.fields[0].name)
             self.assertEqual("integer", res.metadata.fields[0].type)
             self.assertEqual(False, res.metadata.fields[0].is_nullable)
             self.assertEqual(None, res.metadata.fields[1].is_autoincrement)
             self.assertIsNone(res.metadata.fields[0].collation)
 
-            self.assertEqual("NAME", res.metadata.fields[1].name)
+            self.assertEqual(
+                self._compat_field_name("name"), res.metadata.fields[1].name
+            )
             self.assertEqual("string", res.metadata.fields[1].type)
             self.assertEqual(True, res.metadata.fields[1].is_nullable)
             self.assertEqual(None, res.metadata.fields[1].is_autoincrement)
             self.assertEqual("unicode", res.metadata.fields[1].collation)
         finally:
             await self.conn.update(
                 "_session_settings", ["sql_full_metadata"], [("=", "value", False)]
             )
+
+    async def _compat(self, conn: asynctnt.Connection):
+        if conn.version >= (2, 11):
+            await conn.execute('SET SESSION "sql_seq_scan" = true;')
```

### Comparing `asynctnt-2.1.0a1/tests/test_op_sql_prepared.py` & `asynctnt-2.2.0/tests/test_op_sql_prepared.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_op_update.py` & `asynctnt-2.2.0/tests/test_op_update.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,35 @@
+from decimal import Decimal
+
 from asynctnt import Response
 from asynctnt.exceptions import ErrorCode, TarantoolDatabaseError, TarantoolSchemaError
 from tests import BaseTarantoolTestCase
+from tests._testbase import ensure_version
 
 
 class UpdateTestCase(BaseTarantoolTestCase):
     async def _fill_data(self):
         data = [
             [0, "a", 1, 5, "data1"],
             [1, "b", 8, 6, "data2"],
             [2, "c", 10, 12, "data3", "extra_field"],
+            [3, "d", 14, 16, "data4", Decimal("12.3"), 12.5],
+            [
+                4,
+                "e",
+                18,
+                20,
+                {
+                    "tree1": {
+                        "tree11": {
+                            "key1": "value1",
+                        }
+                    }
+                },
+            ],
         ]
         for t in data:
             await self.conn.insert(self.TESTER_SPACE_ID, t)
 
         return data
 
     async def test__update_one_assign(self):
@@ -22,14 +39,34 @@
         self.assertIsInstance(res, Response, "Got response")
         self.assertEqual(res.code, 0, "success")
         self.assertGreater(res.sync, 0, "sync > 0")
 
         data[1][2] = 2
         self.assertResponseEqual(res, [data[1]], "Body ok")
 
+    @ensure_version(min=(2, 3))
+    async def test__update_one_assign_by_field_name_with_no_schema(self):
+        data = await self._fill_data()
+
+        await self.tnt_reconnect(fetch_schema=False)
+
+        res = await self.conn.update(self.TESTER_SPACE_ID, [4], [["=", "f4", 100]])
+        data[4][3] = 100
+        self.assertResponseEqual(res, [data[4]], "Body ok")
+
+    @ensure_version(min=(2, 3))
+    async def test__update_one_assign_by_json(self):
+        data = await self._fill_data()
+
+        res = await self.conn.update(
+            self.TESTER_SPACE_ID, [4], [["=", "f5.tree1.tree11.key1", "value2"]]
+        )
+        data[4][4]["tree1"]["tree11"]["key1"] = "value2"
+        self.assertResponseEqual(res, [data[4]], "Body ok")
+
     async def test__update_one_insert(self):
         data = await self._fill_data()
 
         res = await self.conn.update(self.TESTER_SPACE_ID, [1], [["!", 2, 14]])
         data[1].insert(2, 14)
         self.assertResponseEqual(res, [data[1]], "Body ok")
 
@@ -43,25 +80,46 @@
     async def test__update_one_plus(self):
         data = await self._fill_data()
 
         res = await self.conn.update(self.TESTER_SPACE_ID, [1], [["+", 2, 3]])
         data[1][2] += 3
         self.assertResponseEqual(res, [data[1]], "Body ok")
 
+    @ensure_version(min=(2, 3))
+    async def test__update_one_plus_decimal(self):
+        data = await self._fill_data()
+
+        add = Decimal("1.1")
+        res = await self.conn.update(self.TESTER_SPACE_ID, [3], [["+", 5, add]])
+        data[3][5] += add
+        self.assertResponseEqual(res, [data[3]], "Body ok")
+
+    @ensure_version(min=(2, 3))
+    async def test__update_one_plus_float(self):
+        data = await self._fill_data()
+
+        add = 1.5
+        res = await self.conn.update(self.TESTER_SPACE_ID, [3], [["+", 6, add]])
+        data[3][6] += add
+        self.assertResponseEqual(res, [data[3]], "Body ok")
+
     async def test__update_one_plus_str_field(self):
         data = await self._fill_data()
 
         res = await self.conn.update(self.TESTER_SPACE_ID, [1], [["+", "f3", 3]])
         data[1][2] += 3
         self.assertResponseEqual(res, [data[1]], "Body ok")
 
+    @ensure_version(min=(2, 3))
     async def test__update_one_plus_str_field_unknown(self):
         await self._fill_data()
 
-        with self.assertRaisesRegex(KeyError, "Field 'f10' not found"):
+        with self.assertRaisesRegex(
+            TarantoolDatabaseError, "Field 'f10' was not found in the tuple"
+        ):
             await self.conn.update(self.TESTER_SPACE_ID, [1], [["+", "f10", 3]])
 
     async def test__update_one_plus_negative(self):
         data = await self._fill_data()
 
         res = await self.conn.update(self.TESTER_SPACE_ID, [1], [["+", 2, -3]])
         data[1][2] += -3
@@ -134,26 +192,24 @@
         data[1][2] ^= 1
         self.assertResponseEqual(res, [data[1]], "Body ok")
 
         res = await self.conn.update(self.TESTER_SPACE_ID, [1], [["^", 2, 0]])
         data[1][2] ^= 0
         self.assertResponseEqual(res, [data[1]], "Body ok")
 
+    @ensure_version(min=(2, 3))
     async def test__update_operations_not_int_without_schema(self):
         await self.tnt_reconnect(fetch_schema=False)
 
         data = [1, "hello2", 1, 4, "what is up"]
         await self.conn.insert(self.TESTER_SPACE_ID, data)
 
-        msg = (
-            "Operation field_no must be int as there is "
-            "no format declaration in space {}".format(self.TESTER_SPACE_ID)
-        )
-        with self.assertRaisesRegex(TypeError, msg):
-            await self.conn.update(self.TESTER_SPACE_ID, [1], [["+", "f3", 1]])
+        res = await self.conn.update(self.TESTER_SPACE_ID, [1], [["+", "f3", 1]])
+        data[2] += 1
+        self.assertResponseEqual(res, [data], "Body ok")
 
     async def test__update_splice(self):
         data = [1, "hello2", 1, 4, "what is up"]
         await self.conn.insert(self.TESTER_SPACE_ID, data)
 
         res = await self.conn.update(self.TESTER_SPACE_ID, [1], [[":", 1, 1, 3, "!!!"]])
 
@@ -175,20 +231,20 @@
         data = [1, "hello2", 1, 4, "what is up"]
         await self.conn.insert(self.TESTER_SPACE_ID, data)
 
         with self.assertRaisesRegex(IndexError, r"Operation length must be at least 3"):
             await self.conn.update(self.TESTER_SPACE_ID, [1], [[":", 2]])
 
         with self.assertRaisesRegex(
-            IndexError, r"Splice operation must have length of 5"
+            ValueError, r"Splice operation must have length of 5"
         ):
             await self.conn.update(self.TESTER_SPACE_ID, [1], [[":", 2, 1]])
 
         with self.assertRaisesRegex(
-            IndexError, r"Splice operation must have length of 5"
+            ValueError, r"Splice operation must have length of 5"
         ):
             await self.conn.update(self.TESTER_SPACE_ID, [1], [[":", 2, 1, 3]])
 
         with self.assertRaisesRegex(TypeError, r"Splice offset must be int"):
             await self.conn.update(self.TESTER_SPACE_ID, [1], [[":", 2, 1, {}, ":::"]])
 
         with self.assertRaisesRegex(TypeError, r"Splice position must be int"):
@@ -210,18 +266,20 @@
             await self.conn.update(self.TESTER_SPACE_ID, [1], [[{}, 1, 2, 3]])
 
         with self.assertRaisesRegex(
             TypeError, r"Single operation must be a tuple or list"
         ):
             await self.conn.update(self.TESTER_SPACE_ID, [1], [{}])
 
-        with self.assertRaisesRegex(
-            TypeError, r"int argument required for " r"Arithmetic and Delete operations"
-        ):
+        with self.assertRaises(TarantoolDatabaseError) as exc:
             await self.conn.update(self.TESTER_SPACE_ID, [1], [("+", 2, {})])
+        self.assertRegex(
+            exc.exception.message,
+            r"Argument type in operation '\+' on field \d does not match field type: expected a number",
+        )
 
     async def test__update_multiple_operations(self):
         t = [1, "1", 1, 5, "hello", 3, 4, 8]
         await self.conn.insert(self.TESTER_SPACE_ID, t)
 
         t[2] += 1
         t[3] -= 4
```

### Comparing `asynctnt-2.1.0a1/tests/test_op_upsert.py` & `asynctnt-2.2.0/tests/test_op_upsert.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_response.py` & `asynctnt-2.2.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/test_stream.py` & `asynctnt-2.2.0/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/tests/util/__init__.py` & `asynctnt-2.2.0/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/.build.mk` & `asynctnt-2.2.0/third_party/msgpuck/.build.mk`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/.travis.yml` & `asynctnt-2.2.0/third_party/msgpuck/.travis.yml`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/CMakeLists.txt` & `asynctnt-2.2.0/third_party/msgpuck/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/Doxyfile.in` & `asynctnt-2.2.0/third_party/msgpuck/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/LICENSE` & `asynctnt-2.2.0/third_party/msgpuck/LICENSE`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/README.md` & `asynctnt-2.2.0/third_party/msgpuck/README.md`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/debian/changelog` & `asynctnt-2.2.0/third_party/msgpuck/debian/changelog`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/debian/control` & `asynctnt-2.2.0/third_party/msgpuck/debian/control`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/debian/copyright` & `asynctnt-2.2.0/third_party/msgpuck/debian/copyright`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/debian/rules` & `asynctnt-2.2.0/third_party/msgpuck/debian/rules`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/hints.c` & `asynctnt-2.2.0/third_party/msgpuck/hints.c`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/msgpuck.c` & `asynctnt-2.2.0/third_party/msgpuck/msgpuck.c`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/msgpuck.h` & `asynctnt-2.2.0/third_party/msgpuck/msgpuck.h`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/rpm/msgpuck.spec` & `asynctnt-2.2.0/third_party/msgpuck/rpm/msgpuck.spec`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/test/CMakeLists.txt` & `asynctnt-2.2.0/third_party/msgpuck/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/test/msgpuck.c` & `asynctnt-2.2.0/third_party/msgpuck/test/msgpuck.c`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/test/test.c` & `asynctnt-2.2.0/third_party/msgpuck/test/test.c`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/msgpuck/test/test.h` & `asynctnt-2.2.0/third_party/msgpuck/test/test.h`

 * *Files identical despite different names*

### Comparing `asynctnt-2.1.0a1/third_party/xd.h` & `asynctnt-2.2.0/third_party/xd.h`

 * *Files identical despite different names*

