# Comparing `tmp/FFEM-0.3.2.tar.gz` & `tmp/FFEM-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FFEM-0.3.2.tar", last modified: Mon Nov  6 13:35:07 2023, max compression
+gzip compressed data, was "FFEM-0.4.1.tar", last modified: Sun May  5 05:04:49 2024, max compression
```

## Comparing `FFEM-0.3.2.tar` & `FFEM-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-06 13:35:07.218635 FFEM-0.3.2/
-drwxrwxrwx   0        0        0        0 2023-11-06 13:35:07.182933 FFEM-0.3.2/FFEM/
--rw-rw-rw-   0        0        0    12134 2023-11-03 20:52:43.000000 FFEM-0.3.2/FFEM/FFEM.py
--rw-rw-rw-   0        0        0        0 2023-11-02 20:15:27.000000 FFEM-0.3.2/FFEM/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-06 13:35:07.199024 FFEM-0.3.2/FFEM.egg-info/
--rw-rw-rw-   0        0        0     1590 2023-11-06 13:35:06.000000 FFEM-0.3.2/FFEM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-11-06 13:35:07.000000 FFEM-0.3.2/FFEM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-06 13:35:06.000000 FFEM-0.3.2/FFEM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-11-06 13:35:06.000000 FFEM-0.3.2/FFEM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-11-06 13:35:06.000000 FFEM-0.3.2/FFEM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-11-01 15:13:47.000000 FFEM-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     1590 2023-11-06 13:35:07.201025 FFEM-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1083 2023-11-06 13:05:47.000000 FFEM-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-11-06 13:35:07.219988 FFEM-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1243 2023-11-06 13:35:02.000000 FFEM-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 05:04:49.264097 FFEM-0.4.1/
+drwxrwxrwx   0        0        0        0 2024-05-05 05:04:49.254285 FFEM-0.4.1/FFEM/
+-rw-rw-rw-   0        0        0    12134 2023-11-03 20:52:43.000000 FFEM-0.4.1/FFEM/FFEM.py
+-rw-rw-rw-   0        0        0        0 2023-11-02 20:15:27.000000 FFEM-0.4.1/FFEM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 05:04:49.262616 FFEM-0.4.1/FFEM.egg-info/
+-rw-rw-rw-   0        0        0     1644 2024-05-05 05:04:49.000000 FFEM-0.4.1/FFEM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-05 05:04:49.000000 FFEM-0.4.1/FFEM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 05:04:49.000000 FFEM-0.4.1/FFEM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2024-05-05 05:04:49.000000 FFEM-0.4.1/FFEM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-05 05:04:49.000000 FFEM-0.4.1/FFEM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-11-01 15:13:47.000000 FFEM-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1644 2024-05-05 05:04:49.264097 FFEM-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1130 2024-05-05 04:30:04.000000 FFEM-0.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 05:04:49.264097 FFEM-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1285 2024-05-05 05:01:04.000000 FFEM-0.4.1/setup.py
```

### Comparing `FFEM-0.3.2/FFEM/FFEM.py` & `FFEM-0.4.1/FFEM/FFEM.py`

 * *Files identical despite different names*

### Comparing `FFEM-0.3.2/FFEM.egg-info/PKG-INFO` & `FFEM-0.4.1/FFEM.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFEM
-Version: 0.3.2
+Version: 0.4.1
 Summary: Easy and Fast Facial Emotion Monitoring
 Home-page: https://github.com/WiseGeorge/Fast-Facial-Emotion-Monitoring-FFEM-Package
 Author: Jorge Felix Martinez
 Author-email: jorgito16040@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,21 +12,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Fast Facial Emotion Monitoring (FFEM)
 
 This package provides a simple and efficient way to perform Facial Emotion Recognition (FER). It leverages advanced techniques and algorithms to detect and classify emotions from facial expressions.
 
+## How to Install
+
+```
+$ pip install ffem
+```
+
 ## Main Function
 
 * `MonitorEmotion_From_Video(video_path: str | int, output_path:str) -> None`
   This function takes a video file or a webcam feed as input and performs FER. The results are saved to the specified output path.
 
 ## Main Class
 
 * `FaceEmotion_Detection()`
   This class is the backbone of the FER process. It performs face detection and emotion recognition using DeepFace and MediaPipe. The `MonitorEmotion_From_Video` function utilizes this class to carry out its operations.
 
 This package is designed with user-friendliness in mind, making the complex task of FER accessible and straightforward for users. Whether youâ€™re a researcher, a developer, or someone interested in FER, this package can be a valuable tool for your projects.
 
 ## !!About FFEM
-Use only FEEM version >= 0.3, previous versions had requiriments issues. 
+
+Use only FEEM version >= 0.3, previous versions had requiriments issues.
```

### Comparing `FFEM-0.3.2/LICENSE` & `FFEM-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FFEM-0.3.2/PKG-INFO` & `FFEM-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FFEM
-Version: 0.3.2
+Version: 0.4.1
 Summary: Easy and Fast Facial Emotion Monitoring
 Home-page: https://github.com/WiseGeorge/Fast-Facial-Emotion-Monitoring-FFEM-Package
 Author: Jorge Felix Martinez
 Author-email: jorgito16040@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,21 +12,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Fast Facial Emotion Monitoring (FFEM)
 
 This package provides a simple and efficient way to perform Facial Emotion Recognition (FER). It leverages advanced techniques and algorithms to detect and classify emotions from facial expressions.
 
+## How to Install
+
+```
+$ pip install ffem
+```
+
 ## Main Function
 
 * `MonitorEmotion_From_Video(video_path: str | int, output_path:str) -> None`
   This function takes a video file or a webcam feed as input and performs FER. The results are saved to the specified output path.
 
 ## Main Class
 
 * `FaceEmotion_Detection()`
   This class is the backbone of the FER process. It performs face detection and emotion recognition using DeepFace and MediaPipe. The `MonitorEmotion_From_Video` function utilizes this class to carry out its operations.
 
 This package is designed with user-friendliness in mind, making the complex task of FER accessible and straightforward for users. Whether youâ€™re a researcher, a developer, or someone interested in FER, this package can be a valuable tool for your projects.
 
 ## !!About FFEM
-Use only FEEM version >= 0.3, previous versions had requiriments issues. 
+
+Use only FEEM version >= 0.3, previous versions had requiriments issues.
```

### Comparing `FFEM-0.3.2/README.md` & `FFEM-0.4.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 # Fast Facial Emotion Monitoring (FFEM)
 
 This package provides a simple and efficient way to perform Facial Emotion Recognition (FER). It leverages advanced techniques and algorithms to detect and classify emotions from facial expressions.
 
+## How to Install
+
+```
+$ pip install ffem
+```
+
 ## Main Function
 
 * `MonitorEmotion_From_Video(video_path: str | int, output_path:str) -> None`
   This function takes a video file or a webcam feed as input and performs FER. The results are saved to the specified output path.
 
 ## Main Class
 
 * `FaceEmotion_Detection()`
   This class is the backbone of the FER process. It performs face detection and emotion recognition using DeepFace and MediaPipe. The `MonitorEmotion_From_Video` function utilizes this class to carry out its operations.
 
 This package is designed with user-friendliness in mind, making the complex task of FER accessible and straightforward for users. Whether you’re a researcher, a developer, or someone interested in FER, this package can be a valuable tool for your projects.
 
 ## !!About FFEM
-Use only FEEM version >= 0.3, previous versions had requiriments issues. 
+
+Use only FEEM version >= 0.3, previous versions had requiriments issues.
```

### Comparing `FFEM-0.3.2/setup.py` & `FFEM-0.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 #Si tienes un readme
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='FFEM',  #nombre del paquete
-     version='0.3.2', #versión
+     version='0.4.1', #versión
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
+        'protobuf==3.20.0',
+        'tensorflow==2.10',
         'deepface==0.0.79',
-        'keras>=2.10.0',
+        'keras==2.10.0',
         'opencv-contrib-python==4.8.1.78',
         'opencv-python==4.6.0.66',
-        'protobuf==3.20'],
+        ],
     license='MIT'
 )
```

