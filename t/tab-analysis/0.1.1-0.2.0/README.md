# Comparing `tmp/tab_analysis-0.1.1.tar.gz` & `tmp/tab_analysis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tab_analysis-0.1.1.tar", last modified: Thu Jan  4 10:09:17 2024, max compression
+gzip compressed data, was "tab_analysis-0.2.0.tar", last modified: Sun May  5 12:38:13 2024, max compression
```

## Comparing `tab_analysis-0.1.1.tar` & `tab_analysis-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-01-04 10:09:17.073433 tab_analysis-0.1.1/
--rw-rw-rw-   0        0        0     5149 2024-01-04 10:09:17.072936 tab_analysis-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4481 2023-12-29 10:06:41.000000 tab_analysis-0.1.1/README.md
--rw-rw-rw-   0        0        0       85 2024-01-04 10:09:17.073932 tab_analysis-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1195 2024-01-04 09:48:33.000000 tab_analysis-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-04 10:09:17.065966 tab_analysis-0.1.1/tab_analysis/
--rw-rw-rw-   0        0        0      961 2023-11-15 21:27:02.000000 tab_analysis-0.1.1/tab_analysis/__init__.py
--rw-rw-rw-   0        0        0    41680 2023-12-26 22:59:14.000000 tab_analysis-0.1.1/tab_analysis/analysis.py
-drwxrwxrwx   0        0        0        0 2024-01-04 10:09:17.071940 tab_analysis-0.1.1/tab_analysis.egg-info/
--rw-rw-rw-   0        0        0     5149 2024-01-04 10:09:17.000000 tab_analysis-0.1.1/tab_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-01-04 10:09:17.000000 tab_analysis-0.1.1/tab_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-04 10:09:17.000000 tab_analysis-0.1.1/tab_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-01-04 10:09:17.000000 tab_analysis-0.1.1/tab_analysis.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-04 10:09:17.070944 tab_analysis-0.1.1/tests/
--rw-rw-rw-   0        0        0    12422 2023-12-26 22:24:25.000000 tab_analysis-0.1.1/tests/tests_analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:38:13.040437 tab_analysis-0.2.0/
+-rw-rw-rw-   0        0        0     5236 2024-05-05 12:38:13.039936 tab_analysis-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4568 2024-05-05 10:12:46.000000 tab_analysis-0.2.0/README.md
+-rw-rw-rw-   0        0        0       85 2024-05-05 12:38:13.040934 tab_analysis-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2024-04-26 19:24:18.000000 tab_analysis-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:38:13.033462 tab_analysis-0.2.0/tab_analysis/
+-rw-rw-rw-   0        0        0      961 2023-11-15 21:27:02.000000 tab_analysis-0.2.0/tab_analysis/__init__.py
+-rw-rw-rw-   0        0        0    45168 2024-05-05 09:44:15.000000 tab_analysis-0.2.0/tab_analysis/analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:38:13.038440 tab_analysis-0.2.0/tab_analysis.egg-info/
+-rw-rw-rw-   0        0        0     5236 2024-05-05 12:38:13.000000 tab_analysis-0.2.0/tab_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2024-05-05 12:38:13.000000 tab_analysis-0.2.0/tab_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 12:38:13.000000 tab_analysis-0.2.0/tab_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-05 12:38:13.000000 tab_analysis-0.2.0/tab_analysis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 12:38:13.037445 tab_analysis-0.2.0/tests/
+-rw-rw-rw-   0        0        0    12578 2024-05-04 21:59:07.000000 tab_analysis-0.2.0/tests/tests_analysis.py
+-rw-rw-rw-   0        0        0     1254 2024-04-15 19:49:55.000000 tab_analysis-0.2.0/tests/tests_mixte.py
```

### Comparing `tab_analysis-0.1.1/PKG-INFO` & `tab_analysis-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tab_analysis
-Version: 0.1.1
-Summary: TAB-analysis : A tool to Analyse tabular and multi-dimensionnal structures
+Version: 0.2.0
+Summary: TAB-analysis : A tool to analyse tabular and multi-dimensionnal structures
 Home-page: https://github.com/loco-philippe/tab-analysis/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: tabular data,open data,environmental data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
-### *TAB-analysis : A tool to Analyse tabular and multi-dimensionnal structures*
+### *TAB-analysis : A tool to Analyse tabular and multi-dimensional structures*
 
 *TAB-analysis analyzes and measures the relationships between Fields in any tabular Dataset.*
 
 *The TAB-analysis tool is part of the [Environmental Sensing Project](https://github.com/loco-philippe/Environmental-Sensing#readme)*
 
 For more information, see the [user guide](https://loco-philippe.github.io/tab-analysis/docs/user_guide.html) or the [github repository](https://github.com/loco-philippe/tab-analysis).
 
@@ -27,15 +27,15 @@
 ## Principles
 
 Each field in a dataset has global properties (e.g. the number of different values).
 The relationships between two fields can also be characterized in a similar way (e.g. number of pairs of values from the two different fields).
 
 Analyzing these properties gives us a measure of the entire dataset.
 
-The TAB-analysis module carries out these measurements and analyzes. It also identifies data that does not respect given relationships.
+The TAB-analysis module carries out these measurements and analyzes. It also identifies data that does not respect given relationships and multidimensional structure.* .
 
 ## Examples
 
 Here is a price list of different foods based on packaging.
 
 | 'plants'    | 'quantity' | 'product' | 'price' |
 |-------------|------------|-----------|---------|
@@ -63,15 +63,15 @@
                    'quantity': ['1 kg' , '10 kg', '1 kg',   '10 kg',  '1 kg',    '10 kg',   '1 kg',     '10 kg'     ], 
                    'product':  ['apple', 'apple', 'orange', 'orange', 'peppers', 'peppers', 'carrot',   'carrot'    ], 
                    'price':    [1,       10,      2,        20,       1.5,       15,        0.5,        5           ]}
         analysis = AnaDataset(Sdataset.ntv(tabular).to_analysis(True))
         # `analysis` is also available from pandas data
         import pandas as pd
         import ntv_pandas as npd
-        analysis = pd.DataFrame(tabular).npd.analysis()
+        analysis = pd.DataFrame(tabular).npd.analysis(distr=True)
 
 In [2]: # each relationship is evaluated and measured 
         analysis.get_relation('plants', 'product').typecoupl
 Out[2]: 'derived'
 
 In [3]: analysis.get_relation('quantity', 'product').typecoupl
 Out[3]: 'crossed'
@@ -85,21 +85,22 @@
 Out[5]: -1: root-derived (8)
            1 : quantity (6 - 2)
            2 : product (4 - 4)
               0 : plants (2 - 2)
            3 : price (0 - 8)
 
 In [6]: # 'partitions' are found (partitions are multi-dimensionnal data)'
-        analysis.partitions(mode='id')
-Out[6]: [['product', 'quantity'], ['price']]
+        analysis.partitions()
+Out[6]: [['quantity', 'product'], ['price']]
 
 In [7]: # the `field_partition` method return the main structure of the dataset
-        analysis.field_partition(mode='id')
+        analysis.field_partition()
 Out[7]: {'primary': ['quantity', 'product'],
          'secondary': ['plants'],
+         'mixte': [],
          'unique': [],
          'variable': ['price']}
 ```
 
 ## Uses
 
 A TAB-analysis object is initialized by a set of properties (a dict with specific keys). It can therefore be used from any tabular data manager (e.g. pandas).
@@ -110,8 +111,9 @@
 - quality indicators of a dataset
 - analysis of datasets
 
 and in connection with the tabular application:
 
 - error detection and correction,
 - generation of optimized data formats
+- conversion to multidimensional data
 - interface to specific applications
```

### Comparing `tab_analysis-0.1.1/README.md` & `tab_analysis-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-### *TAB-analysis : A tool to Analyse tabular and multi-dimensionnal structures*
+### *TAB-analysis : A tool to Analyse tabular and multi-dimensional structures*
 
 *TAB-analysis analyzes and measures the relationships between Fields in any tabular Dataset.*
 
 *The TAB-analysis tool is part of the [Environmental Sensing Project](https://github.com/loco-philippe/Environmental-Sensing#readme)*
 
 For more information, see the [user guide](https://loco-philippe.github.io/tab-analysis/docs/user_guide.html) or the [github repository](https://github.com/loco-philippe/tab-analysis).
 
@@ -11,15 +11,15 @@
 ## Principles
 
 Each field in a dataset has global properties (e.g. the number of different values).
 The relationships between two fields can also be characterized in a similar way (e.g. number of pairs of values from the two different fields).
 
 Analyzing these properties gives us a measure of the entire dataset.
 
-The TAB-analysis module carries out these measurements and analyzes. It also identifies data that does not respect given relationships.
+The TAB-analysis module carries out these measurements and analyzes. It also identifies data that does not respect given relationships and multidimensional structure.* .
 
 ## Examples
 
 Here is a price list of different foods based on packaging.
 
 | 'plants'    | 'quantity' | 'product' | 'price' |
 |-------------|------------|-----------|---------|
@@ -47,15 +47,15 @@
                    'quantity': ['1 kg' , '10 kg', '1 kg',   '10 kg',  '1 kg',    '10 kg',   '1 kg',     '10 kg'     ], 
                    'product':  ['apple', 'apple', 'orange', 'orange', 'peppers', 'peppers', 'carrot',   'carrot'    ], 
                    'price':    [1,       10,      2,        20,       1.5,       15,        0.5,        5           ]}
         analysis = AnaDataset(Sdataset.ntv(tabular).to_analysis(True))
         # `analysis` is also available from pandas data
         import pandas as pd
         import ntv_pandas as npd
-        analysis = pd.DataFrame(tabular).npd.analysis()
+        analysis = pd.DataFrame(tabular).npd.analysis(distr=True)
 
 In [2]: # each relationship is evaluated and measured 
         analysis.get_relation('plants', 'product').typecoupl
 Out[2]: 'derived'
 
 In [3]: analysis.get_relation('quantity', 'product').typecoupl
 Out[3]: 'crossed'
@@ -69,21 +69,22 @@
 Out[5]: -1: root-derived (8)
            1 : quantity (6 - 2)
            2 : product (4 - 4)
               0 : plants (2 - 2)
            3 : price (0 - 8)
 
 In [6]: # 'partitions' are found (partitions are multi-dimensionnal data)'
-        analysis.partitions(mode='id')
-Out[6]: [['product', 'quantity'], ['price']]
+        analysis.partitions()
+Out[6]: [['quantity', 'product'], ['price']]
 
 In [7]: # the `field_partition` method return the main structure of the dataset
-        analysis.field_partition(mode='id')
+        analysis.field_partition()
 Out[7]: {'primary': ['quantity', 'product'],
          'secondary': ['plants'],
+         'mixte': [],
          'unique': [],
          'variable': ['price']}
 ```
 
 ## Uses
 
 A TAB-analysis object is initialized by a set of properties (a dict with specific keys). It can therefore be used from any tabular data manager (e.g. pandas).
@@ -94,8 +95,9 @@
 - quality indicators of a dataset
 - analysis of datasets
 
 and in connection with the tabular application:
 
 - error detection and correction,
 - generation of optimized data formats
+- conversion to multidimensional data
 - interface to specific applications
```

### Comparing `tab_analysis-0.1.1/setup.py` & `tab_analysis-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # -*- coding: utf-8 -*-
 """
-Created on Thu Sep 19 2023
-
-@author: philippe@loco-labs.io
+`tab_analysis` setup
 """
 
 import pathlib
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="tab_analysis",
-    version="0.1.1",
-    description="TAB-analysis : A tool to Analyse tabular and multi-dimensionnal structures",
+    version="0.2.0",
+    description="TAB-analysis : A tool to analyse tabular and multi-dimensionnal structures",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/loco-philippe/tab-analysis/blob/main/README.md",
     author="Philippe Thomy",
     author_email="philippe@loco-labs.io",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `tab_analysis-0.1.1/tab_analysis/__init__.py` & `tab_analysis-0.2.0/tab_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `tab_analysis-0.1.1/tab_analysis/analysis.py` & `tab_analysis-0.2.0/tab_analysis/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,26 +110,26 @@
         *Parameters (multiple attributes)*
 
         - **idfield** : string or integer - Id of the Field
         - **lencodec** : integer (default None) - length of the codec
         - **mincodec** : integer (default None) - number of different values
         - **maxcodec** : integer (default None) - length of the field
         - **hashf** : string (default None) - update identifier
-        
+
         *example*
-        
+
         AnaField is created with a dict
         >>> AnaField(Cfield([1,2,3,3]).to_analysis).to_dict()
         {'lencodec': 4, 'mincodec': 3, 'maxcodec': 4}
         >>> AnaField({'lencodec': 4, 'mincodec': 3, 'maxcodec': 4})
         {'lencodec': 4, 'mincodec': 3, 'maxcodec': 4}
-        
+
         AnaField is created with parameters
         >>> AnaField(lencodec=4, mincodec=3, maxcodec=4).to_dict()
-        {'lencodec': 4, 'mincodec': 3, 'maxcodec': 4}        
+        {'lencodec': 4, 'mincodec': 3, 'maxcodec': 4}
         >>> AnaField(4, 3, 4).to_dict()
         {'lencodec': 4, 'mincodec': 3, 'maxcodec': 4}
         '''
         if isinstance(idfield, dict):
             self.idfield = idfield.get(IDFIELD, None)
             self.lencodec = idfield.get(LENCODEC, None)
             self.mincodec = idfield.get(MINCODEC, None)
@@ -334,15 +334,14 @@
         - **relation** : boolean (default False) - if True, idfield are included
         - **notnone** : boolean (default True) - if True, None values are not included
         - **mode** : str (default 'field') - AnaDfield representation ('field', 'id', 'index')
         '''
         dic = {DIST: self.dist, TYPECOUPL: self.typecoupl, HASHR: self.hashr}
         if relation or full:
             dic[RELATION] = Util.view(self.relation, mode)
-            #dic[TYPECOUPL] = self.typecoupl
             dic[PARENTCHILD] = self.parent_child
         if distances or full:
             dic |= {DISTANCE: self.distance, DISTOMIN: self.distomin,
                     DISTOMAX: self.distomax, DISTRIBUTED: self.distrib,
                     RATECPL: self.ratecpl, RATEDER: self.rateder}
         if misc or full:
             dic |= {DMAX: self.dmax, DMIN: self.dmin,
@@ -359,18 +358,16 @@
         return []
 
     @property
     def parent_child(self):
         '''returns the direction of the relationship (True if parent is first)'''
         rel0 = self.relation[0]
         rel1 = self.relation[1]
-        # if isinstance(rel0, AnaDfield) and isinstance(rel1, AnaDfield):
         return (rel0.lencodec > rel1.lencodec or
                 (rel0.lencodec == rel1.lencodec and rel0.index < rel1.index))
-        # return None
 
     @property
     def index_relation(self):
         '''return a list with the index of the two fields involved'''
         if self.relation:
             return [fld.index for fld in self.relation]
         return []
@@ -586,41 +583,37 @@
     def _p_min_dist(self, distance=True):
         '''return the parent with minimal distance of the AnaDfield'''
         if self.category == UNIQUE:
             return self.dataset.root
         if distance:
             dist_up = [rel.distance for rel in self.list_relations if
                        not rel.parent_child]
-            # not rel.parent_child and rel.relation[1].category != COUPLED]
         else:
             dist_up = [rel.distomin for rel in self.list_relations if
                        not rel.parent_child]
-            # not rel.parent_child and rel.relation[1].category != COUPLED]
         if not dist_up or min(dist_up) == self.dist_root:
             return self.dataset.root
         dist_min = min(dist_up)
         if distance:
             list_dmin = [rel.relation[1] for rel in self.list_relations
                          if rel.distance == dist_min]
-            # if rel.distance == dist_min and not rel.parent_child]
         else:
             list_dmin = [rel.relation[1] for rel in self.list_relations
                          if rel.distomin == dist_min]
-            # if rel.distomin == dist_min and not rel.parent_child]
         max_lencodec = max(fld.lencodec for fld in list_dmin)
         return [fld for fld in list_dmin if fld.lencodec == max_lencodec][0]
 
     def to_dict(self, mode='id'):
         '''return a dict with field attributes.
 
          *Parameters*
 
         - **mode** : str (default 'id') - AnaDfield representation ('field', 'id', 'index')
         '''
-        dic = super().to_dict(full=True, notnone=False)
+        dic = super().to_dict(full=True, idfield=False, notnone=False)
         dic[DISTROOT] = self.dist_root
         dic[NUM] = self.index
         dic[CATEGORY] = self.category
         dic[PDISTANCE] = self.p_distance.view(mode)
         dic[PDISTOMIN] = self.p_distomin.view(mode)
         dic[PDERIVED] = self.p_derived.view(mode)
         return dic
@@ -668,15 +661,15 @@
         - **lname** : integer - maximal length of the names
         - **mode** : string (default 'derived') - kind of tree :
             'derived' : derived tree
             'distance': min distance tree
             'distomin': min distomin tree
 
         *Returns* : dict where key is a AnaDfield and value is the list of
-        the childs.
+        the childs "name ( dist - lencodec)".
         '''
         adding = ''
         if mode == 'distance':
             rel_parent = self.dataset.get_relation(self, self.p_distance)
             adding = str(rel_parent.distance) + ' - '
         elif mode == 'distomin':
             rel_parent = self.dataset.get_relation(self, self.p_distomin)
@@ -685,15 +678,14 @@
             rel_parent = self.dataset.get_relation(self, self.p_derived)
             adding = str(rel_parent.distance) + ' - '
         adding += str(self.lencodec)
         name = str(self.idfield)[:lname] + ' (' + adding + ')'
         lis = [name.replace(' ', '*').replace("'", '*')]
         if mode == 'derived':
             childs = []
-            #if not self.category in (ROOTED, COUPLED):
             if not self.category in (ROOTED, COUPLED, UNIQUE):
                 for rel in self.list_coupled:
                     lis.append(rel.relation[1].dic_inner_node(mode, lname))
             if not self.category in (ROOTED, UNIQUE):
                 childs = [rel.relation[1] for rel in self.list_relations
                           if rel.relation[1].p_derived == self and
                           rel.relation[1].category != COUPLED]
@@ -725,55 +717,74 @@
 
     *field (@property)*
 
     - `root`
     - `primary`
     - `secondary`
     - `unique`
+    - `mixte`
     - `variable`
 
     *global (@property)*
 
     - `category`
     - `complete`
     - `dimension`
 
     *update (instance methods)*
 
     - `set_relations`
 
-
     *access (instance methods)*
 
     - `get_relation`
     - `dfield`
 
     *synthesis (instance methods)*
 
     - `tree`
     - `to_dict`
     - `indicator`
     - `partitions`
     - `field_partition`
+    - `relation_partition`
     '''
 
     def __init__(self, fields=None, relations=None, iddataset=None,
                  leng=None, hashd=None):
         '''Creation mode :
         - single dict attribute where keys are attributes name,
         - single AnaDataset attribute to make a copy
         - multiple attributes
 
-         *Parameters (multiple attributes)*
+        *Parameters (single dict)*
 
-        - **idfield** : string or integer - Id of the Field
-        - **lencodec** : integer (default None) - length of the codec
-        - **mincodec** : integer (default None) - number of different values
-        - **maxcodec** : integer (default None) - length of the field
-        - **hashf** : string (default None) - update identifier
+        - **fields**: {'fields': list_of_dict, 'name': id_dataset,
+                       'length': length, 'relations': dict_of_relations
+            where:
+                list_of_dict : {'id': id_field, 'lencodec': len_codec, 'mincodec': min_codec}
+                id_field: string - name of field
+                other_field: string - name of field
+                len_codec: int - length of the codec
+                min_codec: int - number of different codec values
+                id_dataset : name of the dataset
+                length: int - length of the dataset
+                dict_of_relations: {id_field : {other_field: dist} for all fields}
+                field: name of a field
+                field_other: name of another field
+                dist: integer (distance between the two fields) or
+                array (distance and boolean distributed)
+
+        *Parameters (multiple attributes)*
+
+        - **fields**: list_of_dict
+        - **iddataset** : string (default None) - id_dataset
+        - **relations** : dict (default None) - dict_of_relations
+        - **leng** : int (default None) - length
+        - **hashd** : string (default None) - update identifier
         '''
         if isinstance(fields, AnaDataset):
             self.iddataset = fields.iddataset
             self.fields = fields.fields
             self.relations = fields.relations
             self.hashd = fields.hashd
             return
@@ -830,45 +841,47 @@
         '''return the root AnaDfield'''
         len_self = len(self)
         return AnaDfield(AnaField(ROOT, len_self, len_self, len_self), self)
 
     @property
     def primary(self):
         '''return the first partition of the partitions'''
-        part = self.partitions(distributed=True)
-        return part[0] if part else []
+        return self.field_partition(mode='field')['primary']
+        # part = self.partitions(mode='field', distributed=True)
+        # return part[0] if part else []
 
     @property
     def complete(self):
         '''return True if the dimension is not 0'''
         return self.dimension > 0
 
     @property
     def dimension(self):
         '''return the highest partition lenght'''
         return len(self.primary)
 
     @property
     def secondary(self):
         '''return the derived ou coupled fields from primary'''
-        secondary = []
-        for field in self.primary:
-            self._add_child(field, secondary)
-        return [fld for fld in secondary if not fld in self.primary]
+        return self.field_partition(mode='field')['secondary']
 
     @property
     def unique(self):
         '''return the unique fields'''
         return [fld for fld in self.fields if fld.category == UNIQUE]
 
     @property
     def variable(self):
         '''return the variable fields'''
-        return [fld for fld in self.fields
-                if not fld in self.primary + self.secondary + self.unique]
+        return self.field_partition(mode='field')['variable']
+
+    @property
+    def mixte(self):
+        '''return the variable fields'''
+        return self.field_partition(mode='field')['mixte']
 
     def set_relations(self, field, dic_relations):
         '''Add relations in the AnaDataset from a dict.
 
          *Parameters*
 
         - **field** : AnaDfield, AnaField or str (idfield) - first relation AnaDfield
@@ -902,15 +915,14 @@
         if isinstance(fld, AnaDfield):
             return fld
         if isinstance(fld, int):
             return self.fields[fld]
         if isinstance(fld, str):
             if fld in [dfld.idfield for dfld in self.fields]:
                 return [dfld for dfld in self.fields if dfld.idfield == fld][0]
-            # return self.root
             return None
         return AnaDfield(fld, self)
 
     def tree(self, mode='derived', width=5, lname=20, string=True):
         '''return a string with a tree of derived Field.
 
          *Parameters*
@@ -961,26 +973,25 @@
         leng = len(self.fields)
         if not relations:
             return fields
         return {'fields': fields, 'relations':
                 [self.get_relation(i, j).to_dict(full=True, mode=mode)
                  for i in range(-1, leng) for j in range(i + 1, leng)]}
 
-    def partitions(self, mode='field', distributed=True):
+    def partitions(self, mode='id', distributed=True):
         '''return a list of available partitions (the first is highest).
 
          *Parameters*
 
-        - **mode** : str (default 'field') - AnaDfield representation
+        - **mode** : str (default 'id') - AnaDfield representation
         ('field', 'id', 'index')
         - **distributed** : boolean (default True) - Include only distributed fields
         '''
         partit = [[fld] for fld in self.fields if fld.category == ROOTED]
         crossed = [rel for rel in self.ana_relations if rel.typecoupl == CROSSED
-                   # and rel.relation[1].index > rel.relation[0].index
                    and rel.parent_child
                    and rel.relation[0].category != COUPLED
                    and rel.relation[1].category != COUPLED]
         if distributed:
             crossed = [rel for rel in crossed if rel.distrib]
         if crossed and len(crossed) == 1 and crossed[0].dist == len(self):
             partit.insert(0, crossed[0].relation)
@@ -990,46 +1001,98 @@
                 for candidat in candidates:
                     flds = list(set(rel.relation[i]
                                 for rel in candidat for i in [0, 1]))
                     if (reduce(mul, [fld.lencodec for fld in flds]) == len(self) and
                         len(candidat) == sum(range(len(flds))) and
                             (not distributed or min(rel.distrib for rel in candidat))):
                         partit.insert(0, flds)
-        partit = Util.view(partit, mode)
-        return [list(tup) for tup in
-                sorted(sorted(list({tuple(sorted(prt)) for prt in partit})),
-                       key=len, reverse=True)]
+        partit = [list(tup) for tup in
+                  sorted(sorted(list({tuple(sorted(prt)) for prt in partit})),
+                         key=len, reverse=True)]
+        return Util.view(partit, mode)
 
-    def field_partition(self, mode='field', partition=None, distributed=True):
+    def field_partition(self, mode='id', partition=None, distributed=True):
         '''return a partition dict with the list of primary, secondary, unique
         and variable fields.
 
-         *Parameters*
+        *Parameters*
 
-        - **mode** : str (default 'field') - AnaDfield representation
+        - **mode** : str (default 'id') - AnaDfield representation
         ('field', 'id', 'index')
-        - **partition** : list (default None) - if None, partition is the first
+        - **partition** : list of str, int, AnaDfield or AnaField(default None) -
+        if None, partition is the first
         - **distributed** : boolean (default True) - Include only distributed fields
         '''
+        partitions = self.partitions(mode='field', distributed=distributed)
+        if not partitions:
+            return Util.view(
+                {'primary': [], 'secondary': [
+                    fld for fld in self.fields if fld.category != UNIQUE],
+                 'mixte': [], 'unique': [
+                    fld for fld in self.fields if fld.category == UNIQUE],
+                 'variable': []}, mode)
         if not partition:
-            partitions = self.partitions(distributed=distributed)
-            if not partitions:
-                return {'primary': [], 'secondary': [], 'unique': [], 'variable': []}
             partition = partitions[0]
         else:
-            partition = [self.dfield(fld) for fld in partition]
+            # partition = [self.dfield(fld) for fld in tuple(sorted(partition))]
+            partition = [self.dfield(fld) for fld in tuple(partition)]
         secondary = []
         for field in partition:
             self._add_child(field, secondary)
         secondary = [fld for fld in secondary if not fld in partition]
         unique = [fld for fld in self.fields if fld.category == UNIQUE]
+        mixte = list(self._mixte_dims(partition, partitions))
         variable = [fld for fld in self.fields
-                    if not fld in partition + secondary + unique]
+                    if not fld in partition + secondary + unique + mixte]
         return Util.view({'primary': partition, 'secondary': secondary,
-                          'unique': unique, 'variable': variable}, mode)
+                          'mixte': mixte, 'unique': unique,
+                          'variable': variable}, mode)
+
+    def relation_partition(self, partition=None, primary=False, noroot=False):
+        '''return a dict with the list of relationships for fields in a partition.
+
+        *Parameters*
+
+        - **partition** : list (default None) - if None, partition is the first
+        - **primary** : boolean (default False) - if True, relations are primary fields
+        - **noroot** : boolean (default False) - if True and single primary,
+        'root' field is replaced by the primary field'''
+        partitions = self.partitions(mode='field')
+        if not partitions:
+            partition = None
+        else:
+            partition = Util.view(partition, mode='field',
+                                  ana=self) if partition else partitions[0]
+        part = self.field_partition(
+            mode='field', partition=partition, distributed=True)
+        fields_cat = {fld: cat for cat, l_fld in part.items() for fld in l_fld}
+        relations = {}
+        for field in fields_cat:
+            rel = []
+            match fields_cat[field]:
+                case 'primary':
+                    rel = [field.idfield]
+                case 'unique': ...
+                case 'variable':
+                    rel = [fld.idfield for fld in part['primary']]
+                case 'secondary' if not primary:
+                    rel = [field.p_derived.idfield]
+                case 'secondary' if primary:
+                    rel = [fld.idfield for fld in field.ascendants()
+                           if fld in part['primary']]
+                case 'mixte':
+                    rel = [fld.idfield for fld in self._mixte_dims(
+                        partition, partitions)[field]]
+                case _: ...
+            if rel == ['root'] and len(part['primary']) == 1 and noroot:
+                rel = [part['primary'][0].idfield]
+            if rel == ['root'] and len(part['primary']) == 0 and noroot:
+                rel = [part['secondary'][0].idfield]
+            relations[field.idfield] = rel
+        return relations
 
     def indicator(self, fullsize, size):
         '''generate size indicators: ol (object lightness), ul (unicity level),
         gain (sizegain)
 
         *Parameters*
 
@@ -1061,51 +1124,63 @@
         for rel in field.list_c_derived + field.list_coupled:
             child = rel.relation[1]
             if not child in childs and not child.category == UNIQUE:
                 childs.append(child)
                 if not child.category in (COUPLED, UNIQUE):
                     self._add_child(child, childs)
 
+    def _mixte_dims(self, partition, partitions):
+        '''return dict with dimensions associated to each mixte field'''
+        dic_mixte = {}
+        for part in partitions:
+            not_part = [fld for fld in part if not fld in partition]
+            if len(not_part) == 1 and len(partition) > len(part) > 1:
+                sub_part = [fld for fld in partition if not fld in part]
+                if min(self.get_relation(not_part[0], fld).typecoupl == 'derived'
+                       for fld in sub_part) is True:
+                    dic_mixte[not_part[0]] = sub_part
+        return dic_mixte
+
 
 class Util:
     ''' common functions for analysis package'''
 
     @staticmethod
-    def view(field_struc, mode):
-        ''' return a representation of a AnaDfields structure (fields, id, index).
+    def view(field_struc, mode, ana=None):
+        ''' return a representation of a AnaDfields structure (field, id, index).
 
          *Parameters*
 
         - **mode** : str - AnaDfield representation ('field', 'id', 'index')
         - **field_struc** : list or dict - structure to represent
+        - **ana** : AnaDataset (default None) - to convert string or index in AnaDfield
         '''
-        if mode is None or mode == 'field' or not field_struc:
+
+        if mode is None or not field_struc:
             return field_struc
         if isinstance(field_struc, dict):
-            return {key: [fld.idfield if mode == 'id' else fld.index for fld in val]
+            return {key: Util.view(val, mode=mode, ana=ana)
                     for key, val in field_struc.items()}
-        if isinstance(field_struc, list) and isinstance(field_struc[0], list):
-            return [[fld.idfield if mode == 'id' else fld.index for fld in val]
-                    for val in field_struc]
         if isinstance(field_struc, list):
-            return [fld.idfield if mode == 'id' else fld.index for fld in field_struc]
-        if isinstance(field_struc, AnaField):
-            return field_struc.idfield if mode == 'id' else field_struc.index
-        return field_struc
+            return [Util.view(val, mode=mode, ana=ana) for val in field_struc]
+        if not isinstance(field_struc, AnaDfield) and mode != 'id':
+            return Util.view(ana.dfield(field_struc), mode=mode)
+        return field_struc if mode == 'field' else (
+            field_struc.index if mode == 'index' else field_struc.idfield)
 
     @staticmethod
-    def reduce_dic(obj):
+    def reduce_dic(obj, notempty=False):
         '''return a dict without None values'''
         if isinstance(obj, dict):
-            return {key: Util.reduce_dic(val) for key, val in obj.items() 
-                    if not val is None}
+            return {key: Util.reduce_dic(val) for key, val in obj.items()
+                    if not val is None and (not notempty or val)}
         if isinstance(obj, list):
             return [Util.reduce_dic(val) for val in obj]
         return obj
-    
+
     @staticmethod
     def clean_dic(obj, old, new):
         '''return a dict or list with updated strings by replacing "old" substring
         with "new" substring'''
         if isinstance(obj, dict):
             return {Util.clean_dic(key, old, new): Util.clean_dic(val, old, new)
                     for key, val in obj.items()}
@@ -1134,8 +1209,7 @@
         if isinstance(keys, (list, tuple)) and isinstance(obj, dict):
             return {key: val for key, val in obj.items() if key in keys}
         return obj
 
 
 class AnaError(Exception):
     ''' Analysis Exception'''
-    # pass
```

### Comparing `tab_analysis-0.1.1/tab_analysis.egg-info/PKG-INFO` & `tab_analysis-0.2.0/tab_analysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tab_analysis
-Version: 0.1.1
-Summary: TAB-analysis : A tool to Analyse tabular and multi-dimensionnal structures
+Version: 0.2.0
+Summary: TAB-analysis : A tool to analyse tabular and multi-dimensionnal structures
 Home-page: https://github.com/loco-philippe/tab-analysis/blob/main/README.md
 Author: Philippe Thomy
 Author-email: philippe@loco-labs.io
 Keywords: tabular data,open data,environmental data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
-### *TAB-analysis : A tool to Analyse tabular and multi-dimensionnal structures*
+### *TAB-analysis : A tool to Analyse tabular and multi-dimensional structures*
 
 *TAB-analysis analyzes and measures the relationships between Fields in any tabular Dataset.*
 
 *The TAB-analysis tool is part of the [Environmental Sensing Project](https://github.com/loco-philippe/Environmental-Sensing#readme)*
 
 For more information, see the [user guide](https://loco-philippe.github.io/tab-analysis/docs/user_guide.html) or the [github repository](https://github.com/loco-philippe/tab-analysis).
 
@@ -27,15 +27,15 @@
 ## Principles
 
 Each field in a dataset has global properties (e.g. the number of different values).
 The relationships between two fields can also be characterized in a similar way (e.g. number of pairs of values from the two different fields).
 
 Analyzing these properties gives us a measure of the entire dataset.
 
-The TAB-analysis module carries out these measurements and analyzes. It also identifies data that does not respect given relationships.
+The TAB-analysis module carries out these measurements and analyzes. It also identifies data that does not respect given relationships and multidimensional structure.* .
 
 ## Examples
 
 Here is a price list of different foods based on packaging.
 
 | 'plants'    | 'quantity' | 'product' | 'price' |
 |-------------|------------|-----------|---------|
@@ -63,15 +63,15 @@
                    'quantity': ['1 kg' , '10 kg', '1 kg',   '10 kg',  '1 kg',    '10 kg',   '1 kg',     '10 kg'     ], 
                    'product':  ['apple', 'apple', 'orange', 'orange', 'peppers', 'peppers', 'carrot',   'carrot'    ], 
                    'price':    [1,       10,      2,        20,       1.5,       15,        0.5,        5           ]}
         analysis = AnaDataset(Sdataset.ntv(tabular).to_analysis(True))
         # `analysis` is also available from pandas data
         import pandas as pd
         import ntv_pandas as npd
-        analysis = pd.DataFrame(tabular).npd.analysis()
+        analysis = pd.DataFrame(tabular).npd.analysis(distr=True)
 
 In [2]: # each relationship is evaluated and measured 
         analysis.get_relation('plants', 'product').typecoupl
 Out[2]: 'derived'
 
 In [3]: analysis.get_relation('quantity', 'product').typecoupl
 Out[3]: 'crossed'
@@ -85,21 +85,22 @@
 Out[5]: -1: root-derived (8)
            1 : quantity (6 - 2)
            2 : product (4 - 4)
               0 : plants (2 - 2)
            3 : price (0 - 8)
 
 In [6]: # 'partitions' are found (partitions are multi-dimensionnal data)'
-        analysis.partitions(mode='id')
-Out[6]: [['product', 'quantity'], ['price']]
+        analysis.partitions()
+Out[6]: [['quantity', 'product'], ['price']]
 
 In [7]: # the `field_partition` method return the main structure of the dataset
-        analysis.field_partition(mode='id')
+        analysis.field_partition()
 Out[7]: {'primary': ['quantity', 'product'],
          'secondary': ['plants'],
+         'mixte': [],
          'unique': [],
          'variable': ['price']}
 ```
 
 ## Uses
 
 A TAB-analysis object is initialized by a set of properties (a dict with specific keys). It can therefore be used from any tabular data manager (e.g. pandas).
@@ -110,8 +111,9 @@
 - quality indicators of a dataset
 - analysis of datasets
 
 and in connection with the tabular application:
 
 - error detection and correction,
 - generation of optimized data formats
+- conversion to multidimensional data
 - interface to specific applications
```

### Comparing `tab_analysis-0.1.1/tests/tests_analysis.py` & `tab_analysis-0.2.0/tests/tests_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,16 +118,16 @@
           {'1 ': ['i1 (3 - 3)',
           {'2 ': ['i2 (1 - 2)', {'3 ': ['i3 (2 - 2)', {'4 ': ['i4 (0 - 2)']}]}]}]}]})
         self.assertEqual(dts.tree('distomin', string=False), {'-1': ['root-distomin (6)',
           {'0 ': ['i0 (0 - 6)', {'1 ': ['i1 (0 - 3)']}, {'2 ': ['i2 (0 - 2)']},
           {'3 ': ['i3 (0 - 2)']}, {'4 ': ['i4 (0 - 2)']}]}]})
 
     def test_partitions(self):
-        self.assertEqual(dts.partitions('index', distributed=False), [[1, 3], [0]])
-        self.assertEqual(dts.partitions('id', distributed=False), [['i1', 'i3'], ['i0']])
+        self.assertEqual(dts.partitions(mode='index', distributed=False), [[1, 3], [0]])
+        self.assertEqual(dts.partitions(mode='id', distributed=False), [['i1', 'i3'], ['i0']])
         
 class Test_AnaDataset(unittest.TestCase):
 
     def test_sdataset(self):
         fruits = {'plants': ['fruit', 'fruit', 'fruit', 'fruit',
                                  'vegetable', 'vegetable', 'vegetable', 'vegetable'],
                      'plts': ['fr', 'fr', 'fr', 'fr', 've', 've', 've', 've'], 
@@ -140,74 +140,74 @@
                      'group': ['fruit 1', 'fruit 10', 'fruit 1', 'veget',
                                 'veget', 'veget', 'veget', 'veget'],
                      'id': [1001, 1002, 1003, 1004, 1005, 1006, 1007, 1008],
                      'supplier': ["sup1", "sup1", "sup1", "sup2", "sup2", "sup2", "sup2", "sup1"],
                      'location': 	["fr", "gb", "es", "ch", "gb", "fr", "es", "ch"],
                      'valid': ["ok", "ok", "ok", "ok", "ok", "ok", "ok", "ok"]}
         ilm = Sdataset.ntv(fruits) 
-        self.assertEqual(ilm.analysis.partitions('index'), [[0, 2, 5], [2, 5, 8], [0, 9], [2, 3], [8, 9], [7]])  
+        self.assertEqual(ilm.analysis.partitions(mode='index'), [[0, 2, 5], [2, 5, 8], [0, 9], [2, 3], [8, 9], [7]])  
         
         ana = AnaDataset(ilm.to_analysis())
-        self.assertEqual(ana.partitions('index', distributed=False), 
+        self.assertEqual(ana.partitions(mode='index', distributed=False), 
                          [[0, 2, 5], [0, 2, 8], [0, 5, 8], [2, 5, 8], [0, 9], [2, 3], [8, 9], [7]])
         ana = AnaDataset(ilm.to_analysis(True))
-        self.assertEqual(ana.partitions('index'), [[0, 2, 5], [2, 5, 8], [0, 9], [2, 3], [8, 9], [7]])
+        self.assertEqual(ana.partitions(mode='index'), [[0, 2, 5], [2, 5, 8], [0, 9], [2, 3], [8, 9], [7]])
         self.assertEqual(ana.field_partition(mode='index', distributed=False), 
-                         {'primary': [0, 2, 5], 'secondary': [1], 'unique': [10], 'variable': [3, 4, 6, 7, 8, 9]})
+                         {'mixte': [3], 'primary': [0, 2, 5], 'secondary': [1], 'unique': [10], 'variable': [4, 6, 7, 8, 9]})
         self.assertEqual(ana.field_partition(mode='index'), 
-                         {'primary': [0, 2, 5], 'secondary': [1], 'unique': [10], 'variable': [3, 4, 6, 7, 8, 9]})
+                         {'mixte': [3], 'primary': [0, 2, 5], 'secondary': [1], 'unique': [10], 'variable': [4, 6, 7, 8, 9]})
         self.assertEqual(ana.field_partition(mode='index', partition=ana.partitions()[1]), 
-                         {'primary': [2, 5, 8], 'secondary': [], 'unique': [10], 'variable': [0, 1, 3, 4, 6, 7, 9]})
-        self.assertEqual(ana.field_partition()['variable'], ana.variable)
-        self.assertEqual(ana.field_partition()['primary'], ana.primary)
-        self.assertEqual(ana.field_partition()['secondary'], ana.secondary)
-        self.assertEqual(ana.field_partition()['unique'], ana.unique)
+                         {'mixte': [], 'primary': [2, 5, 8], 'secondary': [], 'unique': [10], 'variable': [0, 1, 3, 4, 6, 7, 9]})
+        self.assertEqual(ana.field_partition(mode='field')['variable'], ana.variable)
+        self.assertEqual(ana.field_partition(mode='field')['primary'], ana.primary)
+        self.assertEqual(ana.field_partition(mode='field')['secondary'], ana.secondary)
+        self.assertEqual(ana.field_partition(mode='field')['unique'], ana.unique)
 
     def test_partitions(self):
         ilm = Sdataset.ntv({'i0': [1, 2, 3], 'test': [0, 1, 1]})
         self.assertEqual(ilm.partitions, [[0]])
         ilm = Sdataset.from_ntv({'i0': ['a', 'b', 'c'], 'i1': [1, 2, 2], 
                                  'i2': [4, 5, 5], 'i3': [6, 7, 8], 'i4': [6, 7, 8]})
-        self.assertEqual(ilm.analysis.field_partition('index'), 
-                         {'primary': [0], 'secondary': [1, 2, 3, 4], 'unique': [], 'variable': []})
+        self.assertEqual(ilm.analysis.field_partition(mode='index'), 
+                         {'mixte': [], 'primary': [0], 'secondary': [1, 2, 3, 4], 'unique': [], 'variable': []})
         ilm = Sdataset.ntv([['math', 'english', 'software', 'physic', 'english', 'software'],
                          ['philippe', 'philippe', 'philippe',
                           'anne', 'anne', 'anne'],
                          [None, None, None, 'gr1', 'gr1', 'gr2'],
                          ['philippe white', 'philippe white', 'philippe white',
                           'anne white', 'anne white', 'anne white']])
-        self.assertEqual(AnaDataset(ilm.to_analysis(True)).partitions('index'), [])
+        self.assertEqual(AnaDataset(ilm.to_analysis(True)).partitions(mode='index'), [])
         ilm = Cdataset.from_ntv([['math', 'english', 'software', 'math', 'english', 'software'],
                           ['philippe', 'philippe', 'philippe', 'anne', 'anne', 'anne'],
                           [None, None, None, 'gr1', 'gr1', 'gr2'],
                           ['philippe white', 'philippe white', 'philippe white',
                            'anne white', 'anne white', 'anne white']])
         ana = AnaDataset(ilm.to_analysis(True))
-        self.assertEqual(ana.partitions('index')[0], [0, 1])
+        self.assertEqual(ana.partitions(mode='index')[0], [0, 1])
         self.assertEqual(ana.dimension, 2)
         
         ilm = Cdataset.from_ntv([['er', 'rt', 'er', 'ry'], [0, 2, 0, 2], [30, 12, 12, 15],
                      [2, 0, 2, 0], [2, 2, 0, 0], ['info', 'info', 'info', 'info'], [12, 12, 15, 30]])
         ana = AnaDataset(ilm.to_analysis(True))
-        self.assertEqual(ana.partitions('index')[0], [1, 4])
+        self.assertEqual(ana.partitions(mode='index')[0], [1, 4])
         
         ilm = Cdataset.from_ntv([['er', 'rt', 'er', 'ry'], [0, 2, 0, 2], [30, 12, 20, 30],
                      [2, 0, 2, 0], [2, 2, 0, 0], ['info', 'info', 'info', 'info'], [12, 20, 20, 12]])
         ana = AnaDataset(ilm.to_analysis(True))
-        self.assertEqual(ana.partitions('index')[0], [1, 4])
+        self.assertEqual(ana.partitions(mode='index')[0], [1, 4])
         
         ilm = Cdataset.from_ntv([[0, 2, 0, 2], [30, 12, 12, 15], [2, 0, 2, 0], [2, 2, 0, 0],
                           ['info', 'info', 'info', 'info'], [12, 12, 15, 30]])
         ana = AnaDataset(ilm.to_analysis(True))
-        self.assertEqual(ana.partitions('index')[0], [0, 3])
+        self.assertEqual(ana.partitions(mode='index')[0], [0, 3])
         
         ilm = Cdataset.from_ntv([[0, 2, 0, 2], [30, 12, 20, 30], [2, 0, 2, 0], [2, 2, 0, 0],
                           ['info', 'info', 'info', 'info'], [12, 20, 20, 12]])
         ana = AnaDataset(ilm.to_analysis(True))
-        self.assertEqual(ana.partitions('index')[0], [0, 3])        
+        self.assertEqual(ana.partitions(mode='index')[0], [0, 3])        
 
     def test_tree(self):
         il = Sdataset.ntv([[1,2,3,4], [5,6,7,8], [0,0,1,1]])
         self.assertEqual(AnaDataset(il.to_analysis(True)).tree(),
                          '-1: root-derived (4)\n   0 : i0 (0 - 4)\n   1 : i1 (0 - 4)\n   2 : i2 (2 - 2)')
         
 if __name__ == '__main__':
```

