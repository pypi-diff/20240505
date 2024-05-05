# Comparing `tmp/tasksflow-0.2.1.tar.gz` & `tmp/tasksflow-0.2.2.tar.gz`

## Comparing `tasksflow-0.2.1.tar` & `tasksflow-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tasksflow-0.2.1/.python-version
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 tasksflow-0.2.1/Dockerfile.ci
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 tasksflow-0.2.1/README_zh_CN.md
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 tasksflow-0.2.1/requirements-dev.lock
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tasksflow-0.2.1/requirements.lock
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 tasksflow-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 tasksflow-0.2.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 tasksflow-0.2.1/docs/dev.md
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tasksflow-0.2.1/docs/demo/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tasksflow-0.2.1/docs/demo/demo1.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tasksflow-0.2.1/docs/demo/requirements.txt
--rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 tasksflow-0.2.1/scripts/entrypoint
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/__init__.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/cache.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/common.py
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/executer.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/pool.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 tasksflow-0.2.1/src/tasksflow/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tasksflow-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tasksflow-0.2.1/tests/cache_test.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 tasksflow-0.2.1/tests/cpu_intensive_test.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 tasksflow-0.2.1/tests/http_test.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 tasksflow-0.2.1/tests/normal_test.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tasksflow-0.2.1/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 tasksflow-0.2.1/LICENSE
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tasksflow-0.2.1/README.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 tasksflow-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 tasksflow-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 tasksflow-0.2.2/.python-version
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 tasksflow-0.2.2/Dockerfile.ci
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 tasksflow-0.2.2/README_zh_CN.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 tasksflow-0.2.2/requirements-dev.lock
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 tasksflow-0.2.2/requirements.lock
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 tasksflow-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 tasksflow-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 tasksflow-0.2.2/docs/dev.md
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 tasksflow-0.2.2/docs/demo/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 tasksflow-0.2.2/docs/demo/demo1.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 tasksflow-0.2.2/docs/demo/requirements.txt
+-rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 tasksflow-0.2.2/scripts/entrypoint
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 tasksflow-0.2.2/src/tasksflow/__init__.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 tasksflow-0.2.2/src/tasksflow/cache.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tasksflow-0.2.2/src/tasksflow/common.py
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tasksflow-0.2.2/src/tasksflow/executer.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 tasksflow-0.2.2/src/tasksflow/pool.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 tasksflow-0.2.2/src/tasksflow/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tasksflow-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tasksflow-0.2.2/tests/cache_test.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 tasksflow-0.2.2/tests/cpu_intensive_test.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 tasksflow-0.2.2/tests/http_test.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 tasksflow-0.2.2/tests/normal_test.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tasksflow-0.2.2/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 tasksflow-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 tasksflow-0.2.2/README.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 tasksflow-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 tasksflow-0.2.2/PKG-INFO
```

### Comparing `tasksflow-0.2.1/README_zh_CN.md` & `tasksflow-0.2.2/README_zh_CN.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 
 > 通过 tasks 处理复杂流程
 
 在处理复杂流程时，我们通常需要将流程分解为多个任务，然后将这些任务组合在一起。这个库提供了一种简单的方法来定义和执行这些任务。
 
 ## 快速开始
 
-安装 tasksflow：
+安装 tasksflow
 
 ```bash
 pip install tasksflow
 ```
 
 创建一些简单的任务
 
 ```python
+import tasksflow.pool
 import tasksflow.task
+import tasksflow.cache
+import tasksflow.executer
+from pathlib import Path
 
 class Task1(tasksflow.task.Task):
     def run(self):
         return {"a": 1, "b": 2}
 
 
 class Task2(tasksflow.task.Task):
@@ -78,21 +82,22 @@
 其中 Task2 传入了 `enable_cache = False`，将不再自动进行缓存。
 
 #### 缓存实现
 
 `pool` 默认会在 `cache.db` 创建 Sqlite 数据库并缓存任务代码和输入。如果要自定义储存路径，可以
 
 ```python
-p = tasksflow.pool.Pool(tasks, CacheProvider=tasksflow.cache.SqliteCacheProvider("mycache.db"))
+from pathlib import Path
+p = tasksflow.pool.Pool(tasks, cache_provider=tasksflow.cache.SqliteCacheProvider(Path("mycache.db")))
 ```
 
 也可以使用 `MemoryCacheProvider` 代替 `SqliteCacheProvider`，将缓存保存在内存中，常用于测试。
 
 ```python
-p = tasksflow.pool.Pool(tasks, CacheProvider=tasksflow.cache.MemoryCacheProvider())
+p = tasksflow.pool.Pool(tasks, cache_provider=tasksflow.cache.MemoryCacheProvider())
 ```
 
 或者自定义 `CacheProvider`，继承 `tasksflow.cache.CacheProvider` 并实现 `get` 和 `set` 方法。然后将自定义的 `CacheProvider` 传入 `Pool`。
 
 ### executer
 
 `pool` 默认使用 `tasksflow.executer.multiprocess_run`，即为每个任务创建单独的进程。当一个任务被完成后，会根据此任务的输出，自动调用依赖此任务的后置任务。
@@ -102,11 +107,12 @@
 ```python
 p = tasksflow.pool.Pool(tasks, executer=tasksflow.executer.serial_run)
 ```
 
 也可以自定义执行器
 
 ```python
-def my_executer(tasks: list[Task]) -> Dict[str, Any]:
+from typing import Any
+def my_executer(tasks: list[tasksflow.task.Task]) -> dict[str, Any]:
     pass
 p = tasksflow.pool.Pool(tasks, executer=my_executer)
 ```
```

### Comparing `tasksflow-0.2.1/requirements-dev.lock` & `tasksflow-0.2.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.1/.github/workflows/publish.yml` & `tasksflow-0.2.2/.github/workflows/publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -29,9 +29,10 @@
 
       - run: docker exec tasksflow-ci rye sync
 
       - run: docker exec tasksflow-ci rye test -- -s
 
       - run: docker exec tasksflow-ci rye build
 
+      # https://github.com/pypa/gh-action-pypi-publish
       - name: Publish distribution 📦 to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `tasksflow-0.2.1/.github/workflows/test.yml` & `tasksflow-0.2.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.1/docs/demo/demo1.py` & `tasksflow-0.2.2/docs/demo/demo1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import tasksflow.pool
 import tasksflow.task
 
 
 class Task1(tasksflow.task.Task):
     def run(self):
         return {"a": 1, "b": 2}
 
@@ -19,15 +20,15 @@
 class Task4(tasksflow.task.Task):
     def run(self, c: int):
         pass
 
 
 def test_case1():
     tasks = [Task1(), Task2(), Task3()]
-    p = tasksflow.task.Pool(tasks)
+    p = tasksflow.pool.Pool(tasks)
     result = p.run()
     print(f"result: {result}")
 
 
 def main():
     test_case1()
```

### Comparing `tasksflow-0.2.1/src/tasksflow/cache.py` & `tasksflow-0.2.2/src/tasksflow/cache.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.1/src/tasksflow/executer.py` & `tasksflow-0.2.2/src/tasksflow/executer.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.1/src/tasksflow/pool.py` & `tasksflow-0.2.2/src/tasksflow/pool.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.1/src/tasksflow/task.py` & `tasksflow-0.2.2/src/tasksflow/task.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.1/tests/cpu_intensive_test.py` & `tasksflow-0.2.2/tests/cpu_intensive_test.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.1/tests/http_test.py` & `tasksflow-0.2.2/tests/http_test.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.1/tests/normal_test.py` & `tasksflow-0.2.2/tests/normal_test.py`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.1/LICENSE` & `tasksflow-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tasksflow-0.2.1/pyproject.toml` & `tasksflow-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "tasksflow"
-version = "0.2.1"
-description = "Supporting complex processes through tasks"
+version = "0.2.2"
+description = "Handling Complex Workflows with Tasks"
 authors = [{ name = "117503445", email = "t117503445@gmail.com" }]
 dependencies = ["loguru>=0.7.2"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [build-system]
 requires = ["hatchling"]
```

