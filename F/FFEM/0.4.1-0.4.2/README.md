# Comparing `tmp/FFEM-0.4.1.tar.gz` & `tmp/FFEM-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFEM-0.4.1.tar", last modified: Sun May  5 05:04:49 2024, max compression
+gzip compressed data, was "FFEM-0.4.2.tar", last modified: Sun May  5 05:22:01 2024, max compression
```

## Comparing `FFEM-0.4.1.tar` & `FFEM-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 05:04:49.264097 FFEM-0.4.1/
-drwxrwxrwx   0        0        0        0 2024-05-05 05:04:49.254285 FFEM-0.4.1/FFEM/
--rw-rw-rw-   0        0        0    12134 2023-11-03 20:52:43.000000 FFEM-0.4.1/FFEM/FFEM.py
--rw-rw-rw-   0        0        0        0 2023-11-02 20:15:27.000000 FFEM-0.4.1/FFEM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 05:04:49.262616 FFEM-0.4.1/FFEM.egg-info/
--rw-rw-rw-   0        0        0     1644 2024-05-05 05:04:49.000000 FFEM-0.4.1/FFEM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-05-05 05:04:49.000000 FFEM-0.4.1/FFEM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 05:04:49.000000 FFEM-0.4.1/FFEM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2024-05-05 05:04:49.000000 FFEM-0.4.1/FFEM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-05 05:04:49.000000 FFEM-0.4.1/FFEM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-11-01 15:13:47.000000 FFEM-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     1644 2024-05-05 05:04:49.264097 FFEM-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1130 2024-05-05 04:30:04.000000 FFEM-0.4.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 05:04:49.264097 FFEM-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1285 2024-05-05 05:01:04.000000 FFEM-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 05:22:01.978551 FFEM-0.4.2/
+drwxrwxrwx   0        0        0        0 2024-05-05 05:22:01.962142 FFEM-0.4.2/FFEM/
+-rw-rw-rw-   0        0        0    12134 2023-11-03 20:52:43.000000 FFEM-0.4.2/FFEM/FFEM.py
+-rw-rw-rw-   0        0        0        0 2023-11-02 20:15:27.000000 FFEM-0.4.2/FFEM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 05:22:01.968094 FFEM-0.4.2/FFEM.egg-info/
+-rw-rw-rw-   0        0        0     1644 2024-05-05 05:22:01.000000 FFEM-0.4.2/FFEM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-05 05:22:01.000000 FFEM-0.4.2/FFEM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 05:22:01.000000 FFEM-0.4.2/FFEM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2024-05-05 05:22:01.000000 FFEM-0.4.2/FFEM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-05 05:22:01.000000 FFEM-0.4.2/FFEM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-11-01 15:13:47.000000 FFEM-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     1644 2024-05-05 05:22:01.968094 FFEM-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1130 2024-05-05 04:30:04.000000 FFEM-0.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 05:22:01.978551 FFEM-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1256 2024-05-05 05:21:59.000000 FFEM-0.4.2/setup.py
```

### Comparing `FFEM-0.4.1/FFEM/FFEM.py` & `FFEM-0.4.2/FFEM/FFEM.py`

 * *Files identical despite different names*

### Comparing `FFEM-0.4.1/FFEM.egg-info/PKG-INFO` & `FFEM-0.4.2/FFEM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFEM
-Version: 0.4.1
+Version: 0.4.2
 Summary: Easy and Fast Facial Emotion Monitoring
 Home-page: https://github.com/WiseGeorge/Fast-Facial-Emotion-Monitoring-FFEM-Package
 Author: Jorge Felix Martinez
 Author-email: jorgito16040@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FFEM-0.4.1/LICENSE` & `FFEM-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FFEM-0.4.1/PKG-INFO` & `FFEM-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFEM
-Version: 0.4.1
+Version: 0.4.2
 Summary: Easy and Fast Facial Emotion Monitoring
 Home-page: https://github.com/WiseGeorge/Fast-Facial-Emotion-Monitoring-FFEM-Package
 Author: Jorge Felix Martinez
 Author-email: jorgito16040@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FFEM-0.4.1/README.md` & `FFEM-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `FFEM-0.4.1/setup.py` & `FFEM-0.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,30 @@
 #Si tienes un readme
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='FFEM',  #nombre del paquete
-     version='0.4.1', #versión
+     version='0.4.2', #versión
      scripts=['FFEM/FFEM.py'] , #nombre del ejecutable
      author="Jorge Felix Martinez", #autor
      author_email="jorgito16040@gmail.com", #email
      description="Easy and Fast Facial Emotion Monitoring", #Breve descripción
      long_description=long_description,
      long_description_content_type="text/markdown", #Incluir el README.md si lo has creado
      url="https://github.com/WiseGeorge/Fast-Facial-Emotion-Monitoring-FFEM-Package", #url donde se encuentra tu paquete en Github
      packages=setuptools.find_packages(), #buscamos todas las dependecias necesarias para que tu paquete funcione (por ejemplo numpy, scipy, etc.)
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent", ],
     
     install_requires=[
-        'protobuf==3.20.0',
-        'tensorflow==2.10',
         'deepface==0.0.79',
+        'tensorflow==2.10',
         'keras==2.10.0',
         'opencv-contrib-python==4.8.1.78',
         'opencv-python==4.6.0.66',
         ],
     license='MIT'
 )
```

