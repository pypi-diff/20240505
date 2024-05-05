# Comparing `tmp/data_watchtower-0.0.1.tar.gz` & `tmp/data_watchtower-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_watchtower-0.0.1.tar", last modified: Thu May  2 02:39:39 2024, max compression
+gzip compressed data, was "data_watchtower-0.0.2.tar", last modified: Sun May  5 07:24:00 2024, max compression
```

## Comparing `data_watchtower-0.0.1.tar` & `data_watchtower-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 02:39:39.730381 data_watchtower-0.0.1/
--rw-rw-rw-   0        0        0     1090 2024-05-01 02:10:55.000000 data_watchtower-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      291 2024-05-02 02:39:39.730381 data_watchtower-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1549 2024-05-02 02:20:01.000000 data_watchtower-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 02:39:39.715473 data_watchtower-0.0.1/data_watchtower/
--rw-rw-rw-   0        0        0      241 2024-05-02 01:56:04.000000 data_watchtower-0.0.1/data_watchtower/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 02:39:39.724288 data_watchtower-0.0.1/data_watchtower/core/
--rw-rw-rw-   0        0        0       48 2024-04-26 07:27:27.000000 data_watchtower-0.0.1/data_watchtower/core/__init__.py
--rw-rw-rw-   0        0        0     2208 2024-04-28 13:49:28.000000 data_watchtower-0.0.1/data_watchtower/core/base.py
--rw-rw-rw-   0        0        0      609 2024-04-28 13:49:28.000000 data_watchtower-0.0.1/data_watchtower/core/data_loaders.py
--rw-rw-rw-   0        0        0     1551 2024-04-28 13:49:28.000000 data_watchtower-0.0.1/data_watchtower/core/macro.py
--rw-rw-rw-   0        0        0     4841 2024-04-29 13:24:29.000000 data_watchtower-0.0.1/data_watchtower/core/utils.py
--rw-rw-rw-   0        0        0    10439 2024-04-28 03:18:50.000000 data_watchtower-0.0.1/data_watchtower/core/validators.py
--rw-rw-rw-   0        0        0     5291 2024-04-28 07:50:34.000000 data_watchtower-0.0.1/data_watchtower/core/watchtower.py
-drwxrwxrwx   0        0        0        0 2024-05-02 02:39:39.728374 data_watchtower-0.0.1/data_watchtower/model/
--rw-rw-rw-   0        0        0       48 2024-04-26 07:38:23.000000 data_watchtower-0.0.1/data_watchtower/model/__init__.py
--rw-rw-rw-   0        0        0     1763 2024-05-01 05:20:15.000000 data_watchtower-0.0.1/data_watchtower/model/models.py
--rw-rw-rw-   0        0        0     7354 2024-05-02 02:07:49.000000 data_watchtower-0.0.1/data_watchtower/model/services.py
-drwxrwxrwx   0        0        0        0 2024-05-02 02:39:39.728374 data_watchtower-0.0.1/data_watchtower.egg-info/
--rw-rw-rw-   0        0        0      291 2024-05-02 02:39:39.000000 data_watchtower-0.0.1/data_watchtower.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-02 02:39:39.000000 data_watchtower-0.0.1/data_watchtower.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 02:39:39.000000 data_watchtower-0.0.1/data_watchtower.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-02 02:39:39.000000 data_watchtower-0.0.1/data_watchtower.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 02:39:39.730381 data_watchtower-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      391 2024-05-01 07:55:06.000000 data_watchtower-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.348128 data_watchtower-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-05-01 02:10:55.000000 data_watchtower-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      511 2024-05-05 07:24:00.348128 data_watchtower-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2435 2024-05-03 13:56:51.000000 data_watchtower-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.271070 data_watchtower-0.0.2/data_watchtower/
+-rw-rw-rw-   0        0        0      270 2024-05-05 07:21:20.000000 data_watchtower-0.0.2/data_watchtower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.288437 data_watchtower-0.0.2/data_watchtower/api/
+-rw-rw-rw-   0        0        0       48 2024-05-03 02:34:32.000000 data_watchtower-0.0.2/data_watchtower/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.301283 data_watchtower-0.0.2/data_watchtower/api/handlers/
+-rw-rw-rw-   0        0        0       48 2024-05-03 03:21:05.000000 data_watchtower-0.0.2/data_watchtower/api/handlers/__init__.py
+-rw-rw-rw-   0        0        0      845 2024-05-05 04:43:17.000000 data_watchtower-0.0.2/data_watchtower/api/handlers/base.py
+-rw-rw-rw-   0        0        0      553 2024-05-03 12:39:06.000000 data_watchtower-0.0.2/data_watchtower/api/handlers/watchtower.py
+-rw-rw-rw-   0        0        0      835 2024-05-05 04:40:00.000000 data_watchtower-0.0.2/data_watchtower/api/server.py
+-rw-rw-rw-   0        0        0      291 2024-05-05 06:57:58.000000 data_watchtower-0.0.2/data_watchtower/api/url.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.320817 data_watchtower-0.0.2/data_watchtower/core/
+-rw-rw-rw-   0        0        0       48 2024-04-26 07:27:27.000000 data_watchtower-0.0.2/data_watchtower/core/__init__.py
+-rw-rw-rw-   0        0        0     2809 2024-05-05 04:36:42.000000 data_watchtower-0.0.2/data_watchtower/core/base.py
+-rw-rw-rw-   0        0        0     1138 2024-05-03 09:14:39.000000 data_watchtower-0.0.2/data_watchtower/core/data_loaders.py
+-rw-rw-rw-   0        0        0     1546 2024-05-03 04:45:13.000000 data_watchtower-0.0.2/data_watchtower/core/macro.py
+-rw-rw-rw-   0        0        0    10439 2024-04-28 03:18:50.000000 data_watchtower-0.0.2/data_watchtower/core/validators.py
+-rw-rw-rw-   0        0        0     5861 2024-05-03 12:39:06.000000 data_watchtower-0.0.2/data_watchtower/core/watchtower.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.334605 data_watchtower-0.0.2/data_watchtower/model/
+-rw-rw-rw-   0        0        0       48 2024-04-26 07:38:23.000000 data_watchtower-0.0.2/data_watchtower/model/__init__.py
+-rw-rw-rw-   0        0        0     2528 2024-05-03 15:15:42.000000 data_watchtower-0.0.2/data_watchtower/model/models.py
+-rw-rw-rw-   0        0        0     8448 2024-05-03 15:15:42.000000 data_watchtower-0.0.2/data_watchtower/model/services.py
+-rw-rw-rw-   0        0        0     5473 2024-05-03 12:33:46.000000 data_watchtower-0.0.2/data_watchtower/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.346089 data_watchtower-0.0.2/data_watchtower.egg-info/
+-rw-rw-rw-   0        0        0      511 2024-05-05 07:23:59.000000 data_watchtower-0.0.2/data_watchtower.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2024-05-05 07:24:00.000000 data_watchtower-0.0.2/data_watchtower.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 07:24:00.000000 data_watchtower-0.0.2/data_watchtower.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-05-05 07:24:00.000000 data_watchtower-0.0.2/data_watchtower.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-05 07:24:00.000000 data_watchtower-0.0.2/data_watchtower.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 07:24:00.349167 data_watchtower-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      802 2024-05-05 07:22:28.000000 data_watchtower-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.342425 data_watchtower-0.0.2/tests/
+-rw-rw-rw-   0        0        0     7055 2024-05-05 04:20:24.000000 data_watchtower-0.0.2/tests/test_validator.py
```

### Comparing `data_watchtower-0.0.1/LICENSE` & `data_watchtower-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.1/README.md` & `data_watchtower-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,103 @@
 # data_watchtower
 
 数据监控校验工具
+
 在你的CTO发现问题前, 发现问题
 
+## 安装
+
+```
+pip install data-watchtower
+```
+
+## 数据加载器
+
+加载数据到内存中,供校验器使用
+
+## 校验器
+
+校验加载器加载的数据是否符合预期
+
+### 内置加载器
+
+* ExpectColumnValuesToNotBeNull
+* ExpectColumnRecentlyUpdated
+* ExpectColumnStdToBeBetween
+* ExpectColumnMeanToBeBetween
+* ExpectColumnNullRatioToBeBetween
+* ExpectRowCountToBeBetween
+* ExpectColumnDistinctValuesToContainSet
+* ExpectColumnDistinctValuesToEqualSet
+* ExpectColumnValuesToNotBeNull
+* ExpectColumnDistinctValuesToBeInSet
+
+### 自定义加载器
+
+。。。
+
+## 宏
+
+通过自定义宏, 可以在监控项中引用一些自定义的变量, 比如日期, 配置文件等
+
+### 生效范围
+
+* Watchtower的名称
+* 校验器的参数
+* 数据加载器的参数
+
+### 自定义宏
+
+。。。
+
+## 支持的数据库
+
+* MySQL
+* Postgresql
+* SQLite
+* ...
+
 ## 示例
+
 ```python
 import datetime
 from data_watchtower import (DbServices, Watchtower, DatabaseLoader,
                              ExpectRowCountToBeBetween, ExpectColumnValuesToNotBeNull)
 
+dw_test_data_db_url = "sqlite:///test.db"
+dw_backend_db_url = "sqlite:///data.db"
+
 # 自定义宏模板
 custom_macro_map = {
     'today': {'impl': lambda: datetime.datetime.today().strftime("%Y-%m-%d")},
     'start_date': '2024-04-01',
+    'column': 'name',
 }
 # 设置数据加载器,用来加载需要校验的数据
-connection = 'sqlite://test.db'
 query = "SELECT * FROM score where date='${today}'"
-data_loader = DatabaseLoader(query=query, connection=connection)
-
+data_loader = DatabaseLoader(query=query, connection=dw_test_data_db_url)
+data_loader.load()
 # 创建监控项
 wt = Watchtower(name='score of ${today}', data_loader=data_loader, custom_macro_map=custom_macro_map)
 # 添加校验器
 params = ExpectRowCountToBeBetween.Params(min_value=20, max_value=None)
 wt.add_validator(ExpectRowCountToBeBetween(params))
 
-params = ExpectColumnValuesToNotBeNull.Params(column='name')
+params = ExpectColumnValuesToNotBeNull.Params(column='${column}')
 wt.add_validator(ExpectColumnValuesToNotBeNull(params))
 
 result = wt.run()
 print(result['success'])
 
 # 保存监控配置以及监控结果
-db_svr = DbServices("sqlite:///data.db")
+db_svr = DbServices(dw_backend_db_url)
 # 创建表
 db_svr.create_tables()
 # 保存监控配置
 db_svr.add_watchtower(wt)
 # 保存监控结果
 db_svr.save_result(wt, result)
 # 重新计算监控项的成功状态
-db_svr.compute_watchtower_success_status(wt)
-
-```
-
-## 支持的数据库
-* MySQL
-* Postgresql
-* SQLite
-
-## 自定义校验器
+db_svr.update_watchtower_success_status(wt)
 
-## 自定义数据加载器
 
-## 自定义宏
+```
```

### Comparing `data_watchtower-0.0.1/data_watchtower/core/base.py` & `data_watchtower-0.0.2/data_watchtower/core/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import datetime
+import polars as pl
+import pandas as pd
 from attrs import define, field
-from .utils import to_dict, from_dict, to_snake
+from ..utils import to_dict, from_dict, to_snake
 
 
 class BaseBean:
     def to_dict(self):
         result = to_dict(self)
         result['__class__'] = "%s:%s" % (self.__class__.__module__, self.__class__.__name__)
         return result
@@ -49,38 +51,50 @@
         pass
 
     def __init__(self, params: Params):
         self._data = None
         self.result = None
         self.params = params
 
+    def params_to_dict(self):
+        return to_dict(self.params)
+
     def _validation(self):
         raise NotImplementedError
 
     def validation(self):
         result = self._validation()
         return result
 
     def set_data(self, data):
-        self._data = data
+        if isinstance(data, pl.DataFrame):
+            self._data = data
+        elif isinstance(data, pd.DataFrame):
+            self._data = pl.from_pandas(data)
+        else:
+            self._data = pl.DataFrame(data)
 
     def get_data(self):
-        return self._data
+        if isinstance(self._data, pl.DataFrame):
+            return self._data
+        else:
+            raise TypeError("data type error, must be pl.DataFrame. type:%s" % type(self._data))
 
     @classmethod
     def get_validator_name(cls):
         return to_snake(cls.__name__)
 
     @classmethod
     def module_path(cls):
         return "%s:%s" % (cls.__module__, cls.__name__)
 
     def to_dict(self):
         result = dict()
         result['params'] = to_dict(self.params)
+        # result['params']['__class__'] = "%s:%s" % (self.params.__class__.__module__, self.params.__class__.__name__)
         result['__class__'] = "%s:%s" % (self.__class__.__module__, self.__class__.__name__)
         return result
 
     @classmethod
     def from_dict(cls, items: dict):
         # params = cls.Params(**items['params'])
         params = from_dict(cls.Params, items['params'])
```

### Comparing `data_watchtower-0.0.1/data_watchtower/core/macro.py` & `data_watchtower-0.0.2/data_watchtower/core/macro.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import logging
 import datetime
-from data_watchtower.core.utils import load_object
+from data_watchtower.utils import load_object
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_MACRO_CONFIG = {
     'year:1': {'impl': lambda: datetime.datetime.now().strftime("%Y")},
     'today': {
         'impl': lambda: datetime.datetime.now().strftime("%Y%m%d"),
```

### Comparing `data_watchtower-0.0.1/data_watchtower/core/utils.py` & `data_watchtower-0.0.2/data_watchtower/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import re
-import datetime
+import json
 import copy
 import importlib
 from string import Template
 
-from attrs import define, field, asdict
+from attrs import asdict
 
 
 def load_object(path):
     if not isinstance(path, str):
         if callable(path):
             return path
         else:
@@ -59,14 +59,15 @@
 def spawn_validator_from_dict(item):
     cls_path = item.get('__class__')
     cls = load_object(cls_path)
     return cls.from_dict(item)
 
 
 def spawn_data_loader_from_dict(item):
+    item = item.copy()
     cls_path = item.pop('__class__')
     cls = load_object(cls_path)
     return cls.from_dict(item)
 
 
 def get_string_values(data):
     result = []
@@ -163,7 +164,49 @@
                 elif isinstance(v, str):
                     result[k] = self.apply_string(v)
                 else:
                     result[k] = v
             return result
         else:
             return value
+
+
+def json_dumps(obj):
+    def _default_encoder(_obj):
+        return str(_obj)
+
+    if isinstance(obj, str):
+        return obj
+    return json.dumps(obj, default=_default_encoder, ensure_ascii=True)
+
+
+def json_loads(data):
+    if isinstance(data, str):
+        return json.loads(data)
+    else:
+        return data
+
+
+def dump_macro_map(macro_map):
+    """
+    把模板转换成字符串
+    :param macro_map:
+    :return:
+    """
+
+    pass
+
+
+def f2():
+    return 1
+
+
+def main():
+    def add():
+        return 1
+
+    import inspect
+    return
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `data_watchtower-0.0.1/data_watchtower/core/validators.py` & `data_watchtower-0.0.2/data_watchtower/core/validators.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.1/data_watchtower/core/watchtower.py` & `data_watchtower-0.0.2/data_watchtower/core/watchtower.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import copy
 import datetime
 
-from data_watchtower.core.utils import (spawn_data_loader_from_dict, spawn_validator_from_dict,
-                                        get_string_values, MacroTemplate)
+from data_watchtower.utils import (spawn_data_loader_from_dict, spawn_validator_from_dict,
+                                   get_string_values, MacroTemplate, json_loads, json_dumps)
 from data_watchtower.core.macro import DEFAULT_MACRO_CONFIG
 
 
 class Watchtower(object):
 
     def __init__(self, name, data_loader, **params):
-        custom_macro_map = params.get('custom_macro_map')
+        """
+
+        :param name:
+        :param data_loader:
+        :param params:
+        """
+        custom_macro_map = params.get('custom_macro_map')  # 只是运行的时候使用,不会保存
         validator_success_method = params.get('validator_success_method', 'all')
         success_method = params.get('success_method', None)
         extra = params.get('extra', {})
         self.params = params
-        self._data_loader = data_loader
-        self._data_loader_meta = data_loader.to_dict()
+        self._data_loader = data_loader  # 原本的loader,参数可能包含宏
+        self._data_loader_meta = data_loader.to_dict()  # 原本的loader,参数可能包含宏
         self._validators = []
         self._validators_meta = []
         self.name = name
         self.metrics = {}
         custom_macro_map = custom_macro_map or {}
         self.custom_macro_map = custom_macro_map
         self.macro_map = copy.deepcopy(DEFAULT_MACRO_CONFIG)
@@ -37,25 +43,33 @@
                 self.success_method = 'last'
         else:
             self.success_method = success_method
 
     @classmethod
     def from_dict(cls, data):
         data_loader = spawn_data_loader_from_dict(data.get('data_loader', {}))
-        custom_macro_map = data.get('custom_macro_map')
         validator_success_method = data.get('validator_success_method', 'all')
         inst = cls(
             name=data['name'], data_loader=data_loader,
-            custom_macro_map=custom_macro_map,
             validator_success_method=validator_success_method,
         )
         for validator in data.get('validators', []):
             inst.add_validator(spawn_validator_from_dict(validator))
         return inst
 
+    def to_dict(self):
+        result = dict(
+            name=self.name,
+            data_loader=json_dumps(self.get_loader_meta()),
+            validators=json_dumps(self.get_validator_meta()),
+            validator_success_method=self.validator_success_method,
+            success_method=self.success_method,
+        )
+        return result
+
     def add_validator(self, validator):
         item = validator.to_dict()
         self._validators_meta.append(item)
 
     def get_validator_meta(self):
         return self._validators_meta
 
@@ -107,19 +121,21 @@
     def run(self):
         run_time = datetime.datetime.now()
         macro_maps = self.get_macro_maps()
         macro_template = MacroTemplate(macro_maps)
         wt_name = macro_template.apply_string(self.name)
         # self.metrics['raw_name'] = self.name
         # self.metrics['name'] = wt_name
-
+        data_loader_meta = {}
         for k, v in self._data_loader_meta.items():
             if isinstance(v, str):
-                self._data_loader_meta[k] = macro_template.apply_string(v)
-        self._data_loader = spawn_data_loader_from_dict(self._data_loader_meta)
+                data_loader_meta[k] = macro_template.apply_string(v)
+            else:
+                data_loader_meta[k] = v
+        self._data_loader = spawn_data_loader_from_dict(data_loader_meta)
         data = self._data_loader.load()
         validators_result = self.run_validators(data, macro_template)
         self.gen_metrics(data, validators_result)
         success = self.compute_success(validators_result)
         result = dict(
             name=wt_name,
             success=success,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `data_watchtower-0.0.1/data_watchtower/model/services.py` & `data_watchtower-0.0.2/data_watchtower/model/services.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-import json
-from data_watchtower.model.models import *
+import logging
+import datetime
+import shortuuid
 from peewee import fn, JOIN
+from peewee import IntegrityError
 from playhouse.db_url import connect
+from data_watchtower.model.models import ValidationDetail, Watchtower, database_proxy, ValidatorRelation
+from data_watchtower.utils import json_dumps, json_loads
 
-
-def json_dumps(obj):
-    def _default_encoder(obj):
-        return str(obj)
-
-    if isinstance(obj, str):
-        return obj
-    return json.dumps(obj, default=_default_encoder, ensure_ascii=True)
-
-
-def json_loads(data):
-    if isinstance(data, str):
-        return json.loads(data)
-    else:
-        return data
+logger = logging.getLogger(__name__)
 
 
 class DbServices(object):
     def __init__(self, connection):
         """
         可以使用db_url进行数据库连接. 用法: https://docs.peewee-orm.com/en/latest/peewee/playhouse.html#db-url
         或者直接使用peewee的Database对象
@@ -34,60 +24,95 @@
         if isinstance(connection, str):
             self.database = connect(url=connection)
         else:
             self.database = connection
         database_proxy.initialize(self.database)
 
     def create_tables(self):
-        models = [Watchtower, ValidationDetail]
+        models = [Watchtower, ValidationDetail, ValidatorRelation]
         with self.database:
             for model in models:
                 if not self.database.table_exists(model):
                     self.database.create_tables([model])
 
     def get_watchtower(self, name):
         model = Watchtower.get(Watchtower.name == name).get()
         item = model.to_dict()
         if item is not None:
             item['data_loader'] = json_loads(item['data_loader'])
-            item['validators'] = json_loads(item['validators'])
-            item['custom_macro_map'] = json_loads(item['custom_macro_map'])
+            # item['validators'] = json_loads(item['validators'])
+        validators = ValidatorRelation.select().where(ValidatorRelation.wt_name == name)
+        item['validators'] = []
+        for validator_item in validators:
+            validator = dict(
+                params=json_loads(validator_item.params),
+                __class__=validator_item.validator,
+            )
+            item['validators'].append(validator)
         return item
 
+    def get_watchtowers(self):
+        """
+        获取所有的watchtower
+        :return:
+        """
+        result = []
+        query = Watchtower.select(
+            Watchtower.name,
+            Watchtower.success,
+            Watchtower.run_time,
+            Watchtower.data_loader,
+            Watchtower.success_method,
+            Watchtower.validator_success_method,
+        )
+        for item in query:
+            result.append(item.to_dict(fields_from_query=query))
+        return result
+
     def add_watchtower(self, watchtower):
         update_time = datetime.datetime.now()
         try:
             with self.database.atomic():
-                wt = Watchtower(
-                    name=watchtower.name,
-                    data_loader=json_dumps(watchtower.get_loader_meta()),
-                    validators=json_dumps(watchtower.get_validator_meta()),
-                    custom_macro_map=json_dumps(watchtower.custom_macro_map),
-                    validator_success_method=watchtower.validator_success_method,
-                    success_method=watchtower.success_method,
-                    create_time=update_time,
-                    update_time=update_time,
-                )
-                return wt.save(force_insert=True)
+                item = watchtower.to_dict()
+                item['create_time'] = update_time
+                item['update_time'] = update_time
+                wt = Watchtower(**item)
+                wt.save(force_insert=True)
+                validators = []
+                for validator_item in watchtower.get_validator_meta():
+                    inst = ValidatorRelation(
+                        wt_name=watchtower.name,
+                        validator=validator_item['__class__'],
+                        params=json_dumps(validator_item['params']),
+                    )
+                    validators.append(inst)
+                ValidatorRelation.bulk_create(validators, batch_size=100)
         except IntegrityError as e:
-            return None
+            logger.warning('add watchtower error!. msg:%s' % str(e))
+            return
 
     def update_watchtower(self, wt_name, **item):
         if len(item) == 0:
-            return
+            return 0
         update_time = datetime.datetime.now()
         with self.database.atomic():
             wt = Watchtower.select().where(Watchtower.name == wt_name).get()
             if wt:
                 if 'validators' in item:
-                    wt.validators = json_dumps(item.pop('validators'))
+                    validators = []
+                    for validator_item in wt.get_validator_meta():
+                        inst = ValidatorRelation(
+                            wt_name=wt.name,
+                            validator=validator_item['__class__'],
+                            params=json_dumps(validator_item['params']),
+                        )
+                        validators.append(inst)
+                    ValidatorRelation.bulk_create(validators, batch_size=100)
                 if 'data_loader' in item:
                     wt.validators = json_dumps(item.pop('data_loader'))
-                if 'custom_macro_map' in item:
-                    wt.validators = json_dumps(item.pop('custom_macro_map'))
                 for k, v in item.items():
                     setattr(wt, k, v)
                 wt.update_time = update_time
                 return wt.save()
             else:
                 return 0
 
@@ -135,15 +160,14 @@
             )
             records.append(row)
         with self.database.atomic():
             ValidationDetail.insert_many(records).execute()
         return
 
     def compute_watchtower_success_status(self, watchtower):
-        wt_name = "日行情-${last_trading_day}"
         wt_name = watchtower.name
         success_method = watchtower.validator_success_method
         if success_method == 'all':
             DetailAlias = ValidationDetail.alias()
             DetailAliasBase = ValidationDetail.alias('base')
             join_query = DetailAlias.select(
                 DetailAlias.name,
@@ -176,21 +200,14 @@
             raise ValueError('success_method error. value:%s' % success_method)
 
     def update_watchtower_success_status(self, watchtower):
         run_time = datetime.datetime.now()
         success = self.compute_watchtower_success_status(watchtower)
         self.update_watchtower(watchtower.name, success=success, run_time=run_time)
 
-
-def main():
-    from data_watchtower import Watchtower
-    svr = DbServices()
-    # svr.foo()
-    x = svr.get_watchtower('日行情-${last_trading_day}')
-    ww = Watchtower.from_dict(x)
-    r = ww.run()
-    svr.update_watchtower_success_status(ww)
-    return
-
-
-if __name__ == '__main__':
-    main()
+    def add_validator_to_watchtower(self, wt_name, validator, params):
+        inst = ValidatorRelation(
+            wt_name=wt_name,
+            validator=validator,
+            params=params,
+        )
+        return inst.save(force_insert=True)
```

### Comparing `data_watchtower-0.0.1/data_watchtower.egg-info/SOURCES.txt` & `data_watchtower-0.0.2/data_watchtower.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 LICENSE
 README.md
 setup.py
 data_watchtower/__init__.py
+data_watchtower/utils.py
 data_watchtower.egg-info/PKG-INFO
 data_watchtower.egg-info/SOURCES.txt
 data_watchtower.egg-info/dependency_links.txt
+data_watchtower.egg-info/requires.txt
 data_watchtower.egg-info/top_level.txt
+data_watchtower/api/__init__.py
+data_watchtower/api/server.py
+data_watchtower/api/url.py
+data_watchtower/api/handlers/__init__.py
+data_watchtower/api/handlers/base.py
+data_watchtower/api/handlers/watchtower.py
 data_watchtower/core/__init__.py
 data_watchtower/core/base.py
 data_watchtower/core/data_loaders.py
 data_watchtower/core/macro.py
-data_watchtower/core/utils.py
 data_watchtower/core/validators.py
 data_watchtower/core/watchtower.py
 data_watchtower/model/__init__.py
 data_watchtower/model/models.py
-data_watchtower/model/services.py
+data_watchtower/model/services.py
+tests/test_validator.py
```

