# Comparing `tmp/aisp-0.1.31.tar.gz` & `tmp/aisp-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisp-0.1.31.tar", last modified: Mon Apr 29 17:09:12 2024, max compression
+gzip compressed data, was "aisp-0.1.32.tar", last modified: Sun May  5 15:32:35 2024, max compression
```

## Comparing `aisp-0.1.31.tar` & `aisp-0.1.32.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:09:12.300963 aisp-0.1.31/
--rw-rw-rw-   0        0        0     7817 2023-05-19 21:21:29.000000 aisp-0.1.31/LICENSE
--rw-rw-rw-   0        0        0     7996 2024-04-29 17:09:12.298966 aisp-0.1.31/PKG-INFO
--rw-rw-rw-   0        0        0     6854 2023-06-08 16:13:42.000000 aisp-0.1.31/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 17:09:12.256024 aisp-0.1.31/aisp/
-drwxrwxrwx   0        0        0        0 2024-04-29 17:09:12.292024 aisp-0.1.31/aisp/NSA/
--rw-rw-rw-   0        0        0      141 2024-04-27 01:38:31.000000 aisp-0.1.31/aisp/NSA/__init__.py
--rw-rw-rw-   0        0        0     9557 2024-04-29 15:58:05.000000 aisp-0.1.31/aisp/NSA/_base.py
--rw-rw-rw-   0        0        0    54974 2024-04-29 16:34:10.000000 aisp-0.1.31/aisp/NSA/_negative_selection.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:09:12.295965 aisp-0.1.31/aisp.egg-info/
--rw-rw-rw-   0        0        0     7996 2024-04-29 17:09:12.000000 aisp-0.1.31/aisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-29 17:09:12.000000 aisp-0.1.31/aisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:09:12.000000 aisp-0.1.31/aisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-29 17:09:12.000000 aisp-0.1.31/aisp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-29 17:09:12.000000 aisp-0.1.31/aisp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1443 2024-04-29 16:40:40.000000 aisp-0.1.31/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 17:09:12.300963 aisp-0.1.31/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 15:32:35.517609 aisp-0.1.32/
+-rw-rw-rw-   0        0        0     7817 2023-05-19 21:21:29.000000 aisp-0.1.32/LICENSE
+-rw-rw-rw-   0        0        0     7996 2024-05-05 15:32:35.515400 aisp-0.1.32/PKG-INFO
+-rw-rw-rw-   0        0        0     6854 2023-06-08 16:13:42.000000 aisp-0.1.32/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 15:32:35.483120 aisp-0.1.32/aisp/
+drwxrwxrwx   0        0        0        0 2024-05-05 15:32:35.508750 aisp-0.1.32/aisp/NSA/
+-rw-rw-rw-   0        0        0      141 2024-04-27 01:38:31.000000 aisp-0.1.32/aisp/NSA/__init__.py
+-rw-rw-rw-   0        0        0     9557 2024-04-29 15:58:05.000000 aisp-0.1.32/aisp/NSA/_base.py
+-rw-rw-rw-   0        0        0    55330 2024-05-05 15:19:16.000000 aisp-0.1.32/aisp/NSA/_negative_selection.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:32:35.514441 aisp-0.1.32/aisp.egg-info/
+-rw-rw-rw-   0        0        0     7996 2024-05-05 15:32:35.000000 aisp-0.1.32/aisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-05 15:32:35.000000 aisp-0.1.32/aisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:32:35.000000 aisp-0.1.32/aisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-05 15:32:35.000000 aisp-0.1.32/aisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-05 15:32:35.000000 aisp-0.1.32/aisp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1443 2024-05-04 15:42:51.000000 aisp-0.1.32/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:32:35.518619 aisp-0.1.32/setup.cfg
```

### Comparing `aisp-0.1.31/LICENSE` & `aisp-0.1.32/LICENSE`

 * *Files identical despite different names*

### Comparing `aisp-0.1.31/PKG-INFO` & `aisp-0.1.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisp
-Version: 0.1.31
+Version: 0.1.32
 Summary: Package with techniques of artificial immune systems.
 Author-email: João Paulo da Silva Barros <jpsilvabarr@gmail.com>
 Maintainer-email: Alison Zille Lopes <alisonzille@gmail.com>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://ais-package.github.io/
 Project-URL: Documentation, https://ais-package.github.io/docs/intro
 Project-URL: Source Code, https://github.com/AIS-Package/aisp
```

### Comparing `aisp-0.1.31/README.md` & `aisp-0.1.32/README.md`

 * *Files identical despite different names*

### Comparing `aisp-0.1.31/aisp/NSA/_base.py` & `aisp-0.1.32/aisp/NSA/_base.py`

 * *Files identical despite different names*

### Comparing `aisp-0.1.31/aisp/NSA/_negative_selection.py` & `aisp-0.1.32/aisp/NSA/_negative_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import numpy.typing as npt
 from tqdm import tqdm
 from typing import Dict, Literal, Optional, Union
 from collections import namedtuple
-from scipy.spatial.distance import hamming
+from scipy.spatial.distance import cdist
 
 from ._base import Base
 
 
 class RNSA(Base):
     """
     The ``RNSA`` (Real-Valued Negative Selection Algorithm) class is for classification and \
@@ -417,16 +417,15 @@
                     detectores = list(
                         map(lambda x: x.position, self.detectors[_class_])
                     )
                     average_distance[_class_] = np.average(
                         [self.__distance(detector, line)
                          for detector in detectores]
                     )
-                C = np.append(
-                    C, [max(average_distance, key=average_distance.get)])
+                C = np.append(C, [max(average_distance, key=average_distance.get)])
         return C
 
     def __checks_valid_detector(self, X: npt.NDArray = None, vector_x: npt.NDArray = None,
                                     samples_index_class: npt.NDArray = None):
         """
         Function to check if the detector has a valid non-proper ``r`` radius for the class.
 
@@ -956,19 +955,20 @@
                 progress.set_description_str(
                     f"Generating the detectors for the {_class_} class:")
             while len(valid_detectors_set) < self.N:
 
                 is_valid_detector: bool = True
                 # Gera um vetor candidato a detector aleatoriamente com valores 0 e 1.
                 vector_x = np.random.choice([False, True], size=X.shape[1])
-                for i in sample_index[_class_]:
-                    # Verifica a validade do detector para o não-próprio com relação às amostras da classe.
-                    if hamming(X[i], vector_x) <= self.aff_thresh:
-                        is_valid_detector = False
-                        break
+                # Calcula a distância entre o candidato e as amostras da classe.
+                distances = cdist(np.expand_dims(vector_x, axis=0), 
+                                  X[sample_index[_class_]], metric='hamming')
+                # Verifica se alguma das distâncias está abaixo ou igual ao limiar
+                is_valid_detector = not np.any(distances <= self.aff_thresh)
+
                 # Se o detector for válido, adicione a lista dos válidos.
                 if is_valid_detector:
                     discard_count = 0
                     valid_detectors_set.append(vector_x)
                     if verbose:
                         progress.update(1)
                 else:
@@ -1053,21 +1053,26 @@
             class_found: bool = True
             # Lista para armazenar as possíveis classes às quais a amostra se adequou ao self na
             # comparação com os detectores non-self.
             possible_classes: list = []
             for _class_ in self.classes:
                 # Lista para armazenar as taxas de similaridade entre a amostra e os detectores.
                 similarity_sum: float = 0
-                for detector in self.detectors[_class_]:
-                    similarity = hamming(line, detector)
-                    if similarity <= self.aff_thresh:
-                        class_found = False
-                        break
-                    else:
-                        similarity_sum += similarity
+
+                # Calcula a distância de Hamming entre a linha e todos os detectores
+                distances = cdist(np.expand_dims(line, axis=0),
+                                  self.detectors[_class_], metric='hamming')
+
+                # Verificar se alguma distância está abaixo ou igual ao limiar
+                if np.any(distances <= self.aff_thresh):
+                    class_found = False
+                else:
+                    # Somar todas as distâncias
+                    similarity_sum = np.sum(distances)
+
                 # Se a amostra passar por todos os detectores de uma classe, adiciona a classe como
                 # possível previsão e sua media de similaridade.
                 if class_found:
                     possible_classes.append([_class_, similarity_sum / self.N])
 
             # Se, pertencer a uma ou mais classes, adiciona a classe com a distância média mais distante.
             if len(possible_classes) > 0:
@@ -1082,27 +1087,26 @@
                 C = np.append(C, ["non-self"])
             # Se a classe não puder ser identificada pelos detectores
             elif not class_found:
                 class_differences: dict = {}
                 for _class_ in self.classes:
                     # Atribua-a o rotulo a classe com à maior distância em relação ao detector mais próximo.
                     if self.no_label_sample_selection == 'nearest_difference':
-                        differences: list = []
-                        for detector in self.detectors[_class_]:
-                            differences.append(hamming(line, detector))
-                        class_differences[_class_] = min(differences)
+                        difference_min: float = cdist( np.expand_dims(line, axis=0),
+                                                    self.detectors[_class_], metric='hamming'
+                                                ).min()
+                        class_differences[_class_] = difference_min
                     # Ou com base na maior distância com relação à média da distancias dos detectores
                     else:
-                        difference_sum: float = 0
-                        for detector in self.detectors[_class_]:
-                            difference_sum += hamming(line, detector)
+                        difference_sum: float = cdist( np.expand_dims(line, axis=0),
+                                                    self.detectors[_class_], metric='hamming'
+                                                ).sum()
                         class_differences[_class_] = difference_sum / self.N
 
-                C = np.append(
-                    C, [max(class_differences, key=class_differences.get)])
+                C = np.append(C, [max(class_differences, key=class_differences.get)])
 
         return C
 
     def __slice_index_list_by_class(self, y: npt.NDArray) -> dict:
         """
         The function ``__slice_index_list_by_class(...)``, separates the indices of the lines according \
         to the output class, to loop through the sample array, only in positions where the output is \
```

### Comparing `aisp-0.1.31/aisp.egg-info/PKG-INFO` & `aisp-0.1.32/aisp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisp
-Version: 0.1.31
+Version: 0.1.32
 Summary: Package with techniques of artificial immune systems.
 Author-email: João Paulo da Silva Barros <jpsilvabarr@gmail.com>
 Maintainer-email: Alison Zille Lopes <alisonzille@gmail.com>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://ais-package.github.io/
 Project-URL: Documentation, https://ais-package.github.io/docs/intro
 Project-URL: Source Code, https://github.com/AIS-Package/aisp
```

### Comparing `aisp-0.1.31/pyproject.toml` & `aisp-0.1.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aisp"
-version = "0.1.31"
+version = "0.1.32"
 authors = [
   { name="João Paulo da Silva Barros", email="jpsilvabarr@gmail.com" },
 ]
 
 maintainers = [
   { name="Alison Zille Lopes",  email="alisonzille@gmail.com"},
 ]
```

