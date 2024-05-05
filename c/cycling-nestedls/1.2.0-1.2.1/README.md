# Comparing `tmp/cycling_nestedls-1.2.0.tar.gz` & `tmp/cycling_nestedls-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycling_nestedls-1.2.0.tar", last modified: Sun Apr 21 13:19:37 2024, max compression
+gzip compressed data, was "cycling_nestedls-1.2.1.tar", last modified: Sun May  5 14:16:02 2024, max compression
```

## Comparing `cycling_nestedls-1.2.0.tar` & `cycling_nestedls-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 13:19:37.042462 cycling_nestedls-1.2.0/
--rw-rw-rw-   0        0        0     2087 2024-04-21 13:19:37.042462 cycling_nestedls-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2024-04-21 13:16:05.000000 cycling_nestedls-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 13:19:37.042462 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/
--rw-rw-rw-   0        0        0     2087 2024-04-21 13:19:36.000000 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-04-21 13:19:36.000000 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 13:19:36.000000 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-21 13:19:36.000000 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 13:19:36.000000 cycling_nestedls-1.2.0/cycling_nestedls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 13:19:37.042462 cycling_nestedls-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3258 2024-04-21 13:17:06.000000 cycling_nestedls-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 14:16:02.855875 cycling_nestedls-1.2.1/
+-rw-rw-rw-   0        0        0      195 2024-05-05 14:16:02.855875 cycling_nestedls-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1448 2024-05-05 14:12:43.000000 cycling_nestedls-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 14:16:02.855875 cycling_nestedls-1.2.1/cycling_nestedls.egg-info/
+-rw-rw-rw-   0        0        0      195 2024-05-05 14:16:02.000000 cycling_nestedls-1.2.1/cycling_nestedls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2024-05-05 14:16:02.000000 cycling_nestedls-1.2.1/cycling_nestedls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 14:16:02.000000 cycling_nestedls-1.2.1/cycling_nestedls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 14:16:02.000000 cycling_nestedls-1.2.1/cycling_nestedls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 14:16:02.855875 cycling_nestedls-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     3612 2024-05-05 14:07:45.000000 cycling_nestedls-1.2.1/setup.py
```

### Comparing `cycling_nestedls-1.2.0/README.md` & `cycling_nestedls-1.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -21,20 +21,16 @@
 
 test_copy=example.cycling_nestedls(a,True)
 
 #def cycling_nestedls(self,the_list,tab_switch=False,tab_levels=0)
 
 ```
 
-## Get help
-
-Github地址（还没写好）
-Get help ➡️ [Github issue](https://github.com/sgys22/picture_url)
-
 ## Update log
+`1.2.1`更新了setup.py文件
 
 `1.2.0`添加了tab缩进功能，且可导出为csv
 
 `1.0.2`修改了readme.md文件
 
 `1.0.1`第一次上传，但是代码不健全
 
@@ -43,22 +39,27 @@
 ## how to upload a new version (for me)
 
 >pypi: https://packaging.python.org/tutorials/packaging-projects/
 >pypi: https://python-packaging-zh.readthedocs.io/zh_CN/latest/minimal.html#id2
 
 ![png](https://raw.githubusercontent.com/cornradio/imgs/main/20230218220613.png)
 
-
-> make sure have twine installed first⭐⭐⭐
+> make sure have twine and setuptools installed first⭐⭐⭐
 1. change `setup.py`
 2. testing `python3 setup.py develop`
 3. `python3 setup.py sdist`
 4. `twine upload dist/*`
 ![png](E:\ForDocument\Code_items\ForPython\cut_up_04-21_21-14-26.png)
 
-> 编译readme.md
-> 一级标题#，二级##
->是高亮块(`xxx`)
-> 一级注释>
+## 最后：Get help
+
+Github地址（还没写好）
+Get help ➡️ [Github issue](https://github.com/sgys22/picture_url)
+
+---------------------------------------------
+ 编译readme.md
+>> 一级标题#，二级##
+>>是高亮块(`xxx`)
+>> 一级注释>
 >> 多级注释>>
->>>代码'''python'''
+>>代码'''python'''
```

### Comparing `cycling_nestedls-1.2.0/setup.py` & `cycling_nestedls-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+
+from setuptools import find_packages,setup
+
+DESCRIPTION = "A tool to resovle the cycling_nested list."
+setup(
+    name = "cycling_nestedls",
+    version = '1.2.1',
+    author = "aiop102",
+    author_email = "3175454707@qq.com",
+    description = DESCRIPTION,
+    keywords = ['cycle','nested','list'],
+    packages = find_packages()
+    )
+
+
+
+
+
+'''
 import codecs  # 导入处理文件编码的模块
 import os  # 导入操作系统相关功能的模块
 
 from setuptools import find_packages, setup  # 从 setuptools 包中导入查找包和设置函数
 
 # 获取当前脚本所在目录的绝对路径
 here = os.path.abspath(os.path.dirname(__file__))
@@ -9,15 +28,17 @@
 # 打开 README.md 文件并读取其中的内容，作为长描述
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # 定义常量：版本号、描述和长描述
 VERSION = '1.2.0'
 DESCRIPTION = 'A light weight command line menu that supports Windows, MacOS, and Linux'
-LONG_DESCRIPTION = 'A light weight command line menu. Supporting Windows, MacOS, and Linux. It has support for hotkeys'
+#LONG_DESCRIPTION = 'A light weight command line menu. Supporting Windows, MacOS, and Linux. It has support for hotkeys'
+
+
 
 # 设置
 setup(
     name="cycling_nestedls",  # 包的名称
     version=VERSION,  # 版本号
     author="aiop102",  # 作者
     author_email="3175454707@qq.com",  # 作者邮箱
@@ -35,15 +56,15 @@
         "Intended Audience :: Developers",  # 预期受众
         "Programming Language :: Python :: 3",  # 使用的编程语言和版本
         "Operating System :: Unix",  # 支持的操作系统 - Unix
         "Operating System :: MacOS :: MacOS X",  # 支持的操作系统 - macOS
         "Operating System :: Microsoft :: Windows",  # 支持的操作系统 - Windows
     ]
 )
-
+'''
 '''
 import codecs
 import os
 
 from setuptools import find_packages, setup
 
 # these things are needed for the README.md show on pypi
```

