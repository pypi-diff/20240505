# Comparing `tmp/sinli-1.2.0.tar.gz` & `tmp/sinli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinli-1.2.0.tar", last modified: Wed May  1 13:40:29 2024, max compression
+gzip compressed data, was "sinli-1.2.1.tar", last modified: Sun May  5 14:14:53 2024, max compression
```

## Comparing `sinli-1.2.0.tar` & `sinli-1.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    34449 2024-05-01 13:40:18.000000 sinli-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    46399 2024-05-01 13:40:29.183218 sinli-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6102 2024-05-01 13:40:18.000000 sinli-1.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-01 13:40:18.000000 sinli-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 13:40:29.187218 sinli-1.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.179218 sinli-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/common/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5523 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/common/encoded_values.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/devolu/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/devolu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2390 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/devolu/v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/envio/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/envio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/envio/v8.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/factul/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/factul/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2432 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/factul/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/libros/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/libros/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4962 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/libros/v8.py
--rw-rw-rw-   0 root         (0) root         (0)     5239 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/libros/v9.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/mensaj/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/mensaj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/mensaj/v1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli/doctype/pedido/
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/pedido/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/doctype/pedido/v7.py
--rw-rw-rw-   0 root         (0) root         (0)     5490 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/document.py
--rw-rw-rw-   0 root         (0) root         (0)     8072 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/line.py
--rw-rw-rw-   0 root         (0) root         (0)     2486 2024-05-01 13:40:18.000000 sinli-1.2.0/src/sinli/subject.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/src/sinli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    46399 2024-05-01 13:40:29.000000 sinli-1.2.0/src/sinli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2024-05-01 13:40:29.000000 sinli-1.2.0/src/sinli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 13:40:29.000000 sinli-1.2.0/src/sinli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-01 13:40:29.000000 sinli-1.2.0/src/sinli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-01 13:40:29.000000 sinli-1.2.0/src/sinli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:40:29.183218 sinli-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-01 13:40:18.000000 sinli-1.2.0/tests/test_document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)    34449 2024-05-05 14:14:42.000000 sinli-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    46338 2024-05-05 14:14:53.726207 sinli-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6041 2024-05-05 14:14:42.000000 sinli-1.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-05 14:14:42.000000 sinli-1.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 14:14:53.726207 sinli-1.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.722207 sinli-1.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.722207 sinli-1.2.1/src/sinli/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/common/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5851 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/common/encoded_values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/devolu/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/devolu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2390 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/devolu/v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/envio/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/envio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/envio/v8.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/factul/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/factul/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2432 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/factul/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/libros/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/libros/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4962 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/libros/v8.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/libros/v9.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/mensaj/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/mensaj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/mensaj/v1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli/doctype/pedido/
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/pedido/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/doctype/pedido/v7.py
+-rw-rw-rw-   0 root         (0) root         (0)     5490 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     8072 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/line.py
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2024-05-05 14:14:42.000000 sinli-1.2.1/src/sinli/subject.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/src/sinli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46338 2024-05-05 14:14:53.000000 sinli-1.2.1/src/sinli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2024-05-05 14:14:53.000000 sinli-1.2.1/src/sinli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 14:14:53.000000 sinli-1.2.1/src/sinli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-05 14:14:53.000000 sinli-1.2.1/src/sinli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-05 14:14:53.000000 sinli-1.2.1/src/sinli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:14:53.726207 sinli-1.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-05 14:14:42.000000 sinli-1.2.1/tests/test_document.py
```

### Comparing `sinli-1.2.0/LICENSE` & `sinli-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/PKG-INFO` & `sinli-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.2.0
+Version: 1.2.1
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -722,14 +722,15 @@
 
 d = Document.from_filename("/path/to/document.sinli")
 ```
 
 Generate a SINLI document
 ```python
 from sinli import *
+from sinli.common import SinliCode as c
 from stdnum import isbn
 
 # Create a catalog document
 catalog = libros.v9.LibrosDoc()
 catalog.long_id_line.FROM = "LIB12345"
 catalog.long_id_line.TO = "LIB98765"
 catalog.short_id_line.FROM = "sinli@provider.example.org"
@@ -738,26 +739,26 @@
 # Create the header line of the doc
 header = libros.v9.LibrosDoc.Header()
 header.TYPE = "C"
 header.PROVIDER = "Traficantes de Sueños"
 header.CURRENCY = "E"
 
 catalog.doc_lines.append(header)
-                                                                               
-# Create one book for the catalog document                                     
+
+# Create one book for the catalog document
 book = libros.v9.LibrosDoc.Book()
 
 book.EAN = "9788494597879"
 book.ISBN_INVOICE = isbn.format(book.EAN)
 book.AUTHOR_NAME = "Raquel Gutiérrez Aguilar"
 book.TITLE_FULL = "Horizontes comunitario-populares"
 book.PRICE_PV = 12.00
 book.TAX_IVA = 4.00
 book.PRICE_PVP = book.PRICE_PV / (1 + book.TAX_IVA / 100) # precio sin IVA
-book.PRICE_TYPE = "F"
+book.PRICE_TYPE = c.PRICE_TYPE.FIXED
 
 catalog.doc_lines.append(book)
 
 # Final details
 catalog.long_id_line.LEN = len(catalog.doc_lines) + 2 # implementation of this field varies
 ```
 
@@ -813,15 +814,15 @@
 - [x] Manage different document versions
 - [x] Manage table-based fields
 - [x] Manage different data types
 
 ### For bookshops
 
 - [x] Albarán de pedido del cliente
-- [ ] Albarán de devolución
+- [x] Albarán de devolución
 - [x] Mensaje de texto
 
 ### For distributors
 
 - [x] Ficha del libro
 - [ ] Cambio de precio
 - [x] Albarán de envío
```

### Comparing `sinli-1.2.0/README.md` & `sinli-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 d = Document.from_filename("/path/to/document.sinli")
 ```
 
 Generate a SINLI document
 ```python
 from sinli import *
+from sinli.common import SinliCode as c
 from stdnum import isbn
 
 # Create a catalog document
 catalog = libros.v9.LibrosDoc()
 catalog.long_id_line.FROM = "LIB12345"
 catalog.long_id_line.TO = "LIB98765"
 catalog.short_id_line.FROM = "sinli@provider.example.org"
@@ -63,26 +64,26 @@
 # Create the header line of the doc
 header = libros.v9.LibrosDoc.Header()
 header.TYPE = "C"
 header.PROVIDER = "Traficantes de Sueños"
 header.CURRENCY = "E"
 
 catalog.doc_lines.append(header)
-                                                                               
-# Create one book for the catalog document                                     
+
+# Create one book for the catalog document
 book = libros.v9.LibrosDoc.Book()
 
 book.EAN = "9788494597879"
 book.ISBN_INVOICE = isbn.format(book.EAN)
 book.AUTHOR_NAME = "Raquel Gutiérrez Aguilar"
 book.TITLE_FULL = "Horizontes comunitario-populares"
 book.PRICE_PV = 12.00
 book.TAX_IVA = 4.00
 book.PRICE_PVP = book.PRICE_PV / (1 + book.TAX_IVA / 100) # precio sin IVA
-book.PRICE_TYPE = "F"
+book.PRICE_TYPE = c.PRICE_TYPE.FIXED
 
 catalog.doc_lines.append(book)
 
 # Final details
 catalog.long_id_line.LEN = len(catalog.doc_lines) + 2 # implementation of this field varies
 ```
 
@@ -138,15 +139,15 @@
 - [x] Manage different document versions
 - [x] Manage table-based fields
 - [x] Manage different data types
 
 ### For bookshops
 
 - [x] Albarán de pedido del cliente
-- [ ] Albarán de devolución
+- [x] Albarán de devolución
 - [x] Mensaje de texto
 
 ### For distributors
 
 - [x] Ficha del libro
 - [ ] Cambio de precio
 - [x] Albarán de envío
```

### Comparing `sinli-1.2.0/pyproject.toml` & `sinli-1.2.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sinli"
-version = "1.2.0"
+version = "1.2.1"
 dependencies = [
     "typing-extensions==4.3.0",
     "pycountry==22.3.5"
 ]
 authors = [
     {name = "Devcontrol", email = "devcontrol@zici.fr"},
 ]
```

### Comparing `sinli-1.2.0/src/sinli/doctype/__init__.py` & `sinli-1.2.1/src/sinli/doctype/__init__.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli/doctype/devolu/v2.py` & `sinli-1.2.1/src/sinli/doctype/devolu/v2.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli/doctype/envio/v8.py` & `sinli-1.2.1/src/sinli/doctype/envio/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli/doctype/factul/v1.py` & `sinli-1.2.1/src/sinli/doctype/factul/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli/doctype/libros/v8.py` & `sinli-1.2.1/src/sinli/doctype/libros/v8.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli/doctype/libros/v9.py` & `sinli-1.2.1/src/sinli/doctype/libros/v9.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli/doctype/mensaj/v1.py` & `sinli-1.2.1/src/sinli/doctype/mensaj/v1.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli/doctype/pedido/v7.py` & `sinli-1.2.1/src/sinli/doctype/pedido/v7.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli/document.py` & `sinli-1.2.1/src/sinli/document.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli/line.py` & `sinli-1.2.1/src/sinli/line.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli/subject.py` & `sinli-1.2.1/src/sinli/subject.py`

 * *Files identical despite different names*

### Comparing `sinli-1.2.0/src/sinli.egg-info/PKG-INFO` & `sinli-1.2.1/src/sinli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinli
-Version: 1.2.0
+Version: 1.2.1
 Summary: Implementation of the SINLI format. It is used in the book sector in Spain to express commercial operations between book sellers, distributors and editors
 Author-email: Devcontrol <devcontrol@zici.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -722,14 +722,15 @@
 
 d = Document.from_filename("/path/to/document.sinli")
 ```
 
 Generate a SINLI document
 ```python
 from sinli import *
+from sinli.common import SinliCode as c
 from stdnum import isbn
 
 # Create a catalog document
 catalog = libros.v9.LibrosDoc()
 catalog.long_id_line.FROM = "LIB12345"
 catalog.long_id_line.TO = "LIB98765"
 catalog.short_id_line.FROM = "sinli@provider.example.org"
@@ -738,26 +739,26 @@
 # Create the header line of the doc
 header = libros.v9.LibrosDoc.Header()
 header.TYPE = "C"
 header.PROVIDER = "Traficantes de Sueños"
 header.CURRENCY = "E"
 
 catalog.doc_lines.append(header)
-                                                                               
-# Create one book for the catalog document                                     
+
+# Create one book for the catalog document
 book = libros.v9.LibrosDoc.Book()
 
 book.EAN = "9788494597879"
 book.ISBN_INVOICE = isbn.format(book.EAN)
 book.AUTHOR_NAME = "Raquel Gutiérrez Aguilar"
 book.TITLE_FULL = "Horizontes comunitario-populares"
 book.PRICE_PV = 12.00
 book.TAX_IVA = 4.00
 book.PRICE_PVP = book.PRICE_PV / (1 + book.TAX_IVA / 100) # precio sin IVA
-book.PRICE_TYPE = "F"
+book.PRICE_TYPE = c.PRICE_TYPE.FIXED
 
 catalog.doc_lines.append(book)
 
 # Final details
 catalog.long_id_line.LEN = len(catalog.doc_lines) + 2 # implementation of this field varies
 ```
 
@@ -813,15 +814,15 @@
 - [x] Manage different document versions
 - [x] Manage table-based fields
 - [x] Manage different data types
 
 ### For bookshops
 
 - [x] Albarán de pedido del cliente
-- [ ] Albarán de devolución
+- [x] Albarán de devolución
 - [x] Mensaje de texto
 
 ### For distributors
 
 - [x] Ficha del libro
 - [ ] Cambio de precio
 - [x] Albarán de envío
```

### Comparing `sinli-1.2.0/src/sinli.egg-info/SOURCES.txt` & `sinli-1.2.1/src/sinli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

