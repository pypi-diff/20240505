# Comparing `tmp/FFEM-0.4.2.tar.gz` & `tmp/FFEM-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFEM-0.4.2.tar", last modified: Sun May  5 05:22:01 2024, max compression
+gzip compressed data, was "FFEM-0.4.3.tar", last modified: Sun May  5 05:28:03 2024, max compression
```

## Comparing `FFEM-0.4.2.tar` & `FFEM-0.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 05:22:01.978551 FFEM-0.4.2/
-drwxrwxrwx   0        0        0        0 2024-05-05 05:22:01.962142 FFEM-0.4.2/FFEM/
--rw-rw-rw-   0        0        0    12134 2023-11-03 20:52:43.000000 FFEM-0.4.2/FFEM/FFEM.py
--rw-rw-rw-   0        0        0        0 2023-11-02 20:15:27.000000 FFEM-0.4.2/FFEM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 05:22:01.968094 FFEM-0.4.2/FFEM.egg-info/
--rw-rw-rw-   0        0        0     1644 2024-05-05 05:22:01.000000 FFEM-0.4.2/FFEM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-05-05 05:22:01.000000 FFEM-0.4.2/FFEM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 05:22:01.000000 FFEM-0.4.2/FFEM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2024-05-05 05:22:01.000000 FFEM-0.4.2/FFEM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-05 05:22:01.000000 FFEM-0.4.2/FFEM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-11-01 15:13:47.000000 FFEM-0.4.2/LICENSE
--rw-rw-rw-   0        0        0     1644 2024-05-05 05:22:01.968094 FFEM-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1130 2024-05-05 04:30:04.000000 FFEM-0.4.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 05:22:01.978551 FFEM-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1256 2024-05-05 05:21:59.000000 FFEM-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 05:28:03.442266 FFEM-0.4.3/
+drwxrwxrwx   0        0        0        0 2024-05-05 05:28:03.428346 FFEM-0.4.3/FFEM/
+-rw-rw-rw-   0        0        0    12134 2023-11-03 20:52:43.000000 FFEM-0.4.3/FFEM/FFEM.py
+-rw-rw-rw-   0        0        0        0 2023-11-02 20:15:27.000000 FFEM-0.4.3/FFEM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 05:28:03.431348 FFEM-0.4.3/FFEM.egg-info/
+-rw-rw-rw-   0        0        0     1644 2024-05-05 05:28:03.000000 FFEM-0.4.3/FFEM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-05 05:28:03.000000 FFEM-0.4.3/FFEM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 05:28:03.000000 FFEM-0.4.3/FFEM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2024-05-05 05:28:03.000000 FFEM-0.4.3/FFEM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-05 05:28:03.000000 FFEM-0.4.3/FFEM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-11-01 15:13:47.000000 FFEM-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0     1644 2024-05-05 05:28:03.432349 FFEM-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1130 2024-05-05 04:30:04.000000 FFEM-0.4.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 05:28:03.442266 FFEM-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2024-05-05 05:27:36.000000 FFEM-0.4.3/setup.py
```

### Comparing `FFEM-0.4.2/FFEM/FFEM.py` & `FFEM-0.4.3/FFEM/FFEM.py`

 * *Files identical despite different names*

### Comparing `FFEM-0.4.2/FFEM.egg-info/PKG-INFO` & `FFEM-0.4.3/FFEM.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFEM
-Version: 0.4.2
+Version: 0.4.3
 Summary: Easy and Fast Facial Emotion Monitoring
 Home-page: https://github.com/WiseGeorge/Fast-Facial-Emotion-Monitoring-FFEM-Package
 Author: Jorge Felix Martinez
 Author-email: jorgito16040@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FFEM-0.4.2/LICENSE` & `FFEM-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FFEM-0.4.2/PKG-INFO` & `FFEM-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFEM
-Version: 0.4.2
+Version: 0.4.3
 Summary: Easy and Fast Facial Emotion Monitoring
 Home-page: https://github.com/WiseGeorge/Fast-Facial-Emotion-Monitoring-FFEM-Package
 Author: Jorge Felix Martinez
 Author-email: jorgito16040@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FFEM-0.4.2/README.md` & `FFEM-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `FFEM-0.4.2/setup.py` & `FFEM-0.4.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #Si tienes un readme
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='FFEM',  #nombre del paquete
-     version='0.4.2', #versión
+     version='0.4.3', #versión
      scripts=['FFEM/FFEM.py'] , #nombre del ejecutable
      author="Jorge Felix Martinez", #autor
      author_email="jorgito16040@gmail.com", #email
      description="Easy and Fast Facial Emotion Monitoring", #Breve descripción
      long_description=long_description,
      long_description_content_type="text/markdown", #Incluir el README.md si lo has creado
      url="https://github.com/WiseGeorge/Fast-Facial-Emotion-Monitoring-FFEM-Package", #url donde se encuentra tu paquete en Github
@@ -21,12 +21,13 @@
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent", ],
     
     install_requires=[
         'deepface==0.0.79',
         'tensorflow==2.10',
         'keras==2.10.0',
+        'mediapipe==0.10.0',
         'opencv-contrib-python==4.8.1.78',
         'opencv-python==4.6.0.66',
         ],
     license='MIT'
 )
```

