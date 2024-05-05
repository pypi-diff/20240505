# Comparing `tmp/thothglyph_doc-0.2.2.tar.gz` & `tmp/thothglyph_doc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thothglyph_doc-0.2.2.tar", max compression
+gzip compressed data, was "thothglyph_doc-0.2.3.tar", max compression
```

## Comparing `thothglyph_doc-0.2.2.tar` & `thothglyph_doc-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1065 2023-09-03 08:30:24.832210 thothglyph_doc-0.2.2/LICENSE
--rw-r--r--   0        0        0      813 2024-04-07 14:47:55.090699 thothglyph_doc-0.2.2/README.md
--rw-r--r--   0        0        0      697 2024-04-08 23:53:27.001795 thothglyph_doc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/__init__.py
--rw-r--r--   0        0        0        0 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/app/__init__.py
--rw-r--r--   0        0        0     2500 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/app/converter.py
--rw-r--r--   0        0        0     3115 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/data/tglyph.svg
--rw-r--r--   0        0        0     7412 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/data/tglyph_256.png
--rw-r--r--   0        0        0     1651 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/data/tglyph_64.png
--rw-r--r--   0        0        0       43 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/error.py
--rw-r--r--   0        0        0     3064 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/blockdiag.py
--rw-r--r--   0        0        0     1164 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/graphviz.py
--rw-r--r--   0        0        0     2243 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/math.py
--rw-r--r--   0        0        0       74 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/mermaid.py
--rw-r--r--   0        0        0       74 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/plantuml.py
--rw-r--r--   0        0        0     1277 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/ext/wavedrom.py
--rw-r--r--   0        0        0      580 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/node/logging.py
--rw-r--r--   0        0        0    17162 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/node/nd.py
--rw-r--r--   0        0        0      485 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/reader/__init__.py
--rw-r--r--   0        0        0    26011 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/reader/md.py
--rw-r--r--   0        0        0     7344 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/reader/reader.py
--rw-r--r--   0        0        0    47815 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/reader/tglyph.py
--rw-r--r--   0        0        0     1557 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_dis.pdf
--rw-r--r--   0        0        0      627 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_dis.svg
--rw-r--r--   0        0        0     1597 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_en.pdf
--rw-r--r--   0        0        0      748 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_en.svg
--rw-r--r--   0        0        0     1638 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_im.pdf
--rw-r--r--   0        0        0      735 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/common/check_im.svg
--rw-r--r--   0        0        0    52673 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/docx/default/style.docx
--rw-r--r--   0        0        0     5439 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.2/thothglyph/template/html/default/index.html
--rw-r--r--   0        0        0     4322 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.2/thothglyph/template/html/preview/index.html
--rw-r--r--   0        0        0     6793 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/template/latex/default/document-ja.tex
--rw-r--r--   0        0        0      363 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/writer/__init__.py
--rw-r--r--   0        0        0    18936 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/writer/docx.py
--rw-r--r--   0        0        0    16577 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/writer/html.py
--rw-r--r--   0        0        0    18375 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/writer/latex.py
--rw-r--r--   0        0        0     4530 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.2/thothglyph/writer/pdf.py
--rw-r--r--   0        0        0     5474 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.2/thothglyph/writer/writer.py
--rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 thothglyph_doc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-09-03 08:30:24.832210 thothglyph_doc-0.2.3/LICENSE
+-rw-r--r--   0        0        0      899 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/README.md
+-rw-r--r--   0        0        0      697 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/app/__init__.py
+-rw-r--r--   0        0        0     2500 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/app/converter.py
+-rw-r--r--   0        0        0     3115 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/data/tglyph.svg
+-rw-r--r--   0        0        0     7412 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/data/tglyph_256.png
+-rw-r--r--   0        0        0     1651 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/data/tglyph_64.png
+-rw-r--r--   0        0        0       43 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/error.py
+-rw-r--r--   0        0        0     3079 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/ext/blockdiag.py
+-rw-r--r--   0        0        0     1179 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/ext/graphviz.py
+-rw-r--r--   0        0        0     2243 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/ext/math.py
+-rw-r--r--   0        0        0     2185 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/ext/mermaid.py
+-rw-r--r--   0        0        0     2342 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/ext/plantuml.py
+-rw-r--r--   0        0        0     1292 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/ext/wavedrom.py
+-rw-r--r--   0        0        0      580 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/node/logging.py
+-rw-r--r--   0        0        0    17283 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/node/nd.py
+-rw-r--r--   0        0        0      485 2024-04-08 23:53:27.005795 thothglyph_doc-0.2.3/thothglyph/reader/__init__.py
+-rw-r--r--   0        0        0    26011 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/reader/md.py
+-rw-r--r--   0        0        0     7344 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/reader/reader.py
+-rw-r--r--   0        0        0    52416 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/reader/tglyph.py
+-rw-r--r--   0        0        0     1557 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_dis.pdf
+-rw-r--r--   0        0        0      627 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_dis.svg
+-rw-r--r--   0        0        0     1597 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_en.pdf
+-rw-r--r--   0        0        0      748 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_en.svg
+-rw-r--r--   0        0        0     1638 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_im.pdf
+-rw-r--r--   0        0        0      735 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/common/check_im.svg
+-rw-r--r--   0        0        0    52673 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/template/docx/default/style.docx
+-rw-r--r--   0        0        0     5439 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.3/thothglyph/template/html/default/index.html
+-rw-r--r--   0        0        0     4322 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.3/thothglyph/template/html/preview/index.html
+-rw-r--r--   0        0        0     6793 2024-05-04 04:58:45.492809 thothglyph_doc-0.2.3/thothglyph/template/latex/default/document-ja.tex
+-rw-r--r--   0        0        0     1428 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/util/svg.py
+-rw-r--r--   0        0        0      363 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/writer/__init__.py
+-rw-r--r--   0        0        0    18936 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.3/thothglyph/writer/docx.py
+-rw-r--r--   0        0        0    17349 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/writer/html.py
+-rw-r--r--   0        0        0    18962 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/writer/latex.py
+-rw-r--r--   0        0        0     4528 2024-05-05 12:00:25.198545 thothglyph_doc-0.2.3/thothglyph/writer/pdf.py
+-rw-r--r--   0        0        0     5474 2024-05-03 06:04:24.989564 thothglyph_doc-0.2.3/thothglyph/writer/writer.py
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 thothglyph_doc-0.2.3/PKG-INFO
```

### Comparing `thothglyph_doc-0.2.2/LICENSE` & `thothglyph_doc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/pyproject.toml` & `thothglyph_doc-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thothglyph-doc"
-version = "0.2.2"
+version = "0.2.3"
 description = "A Documentation converter and language for Engineers"
 authors = ["nakandev <nakandev.s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "thothglyph" },
 ]
```

### Comparing `thothglyph_doc-0.2.2/thothglyph/app/converter.py` & `thothglyph_doc-0.2.3/thothglyph/app/converter.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/data/tglyph.svg` & `thothglyph_doc-0.2.3/thothglyph/data/tglyph.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/data/tglyph_256.png` & `thothglyph_doc-0.2.3/thothglyph/data/tglyph_256.png`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/data/tglyph_64.png` & `thothglyph_doc-0.2.3/thothglyph/data/tglyph_64.png`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/ext/blockdiag.py` & `thothglyph_doc-0.2.3/thothglyph/ext/blockdiag.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import re
-import cairosvg
 import blockdiag.parser
 import blockdiag.builder
 import blockdiag.drawer
 import actdiag.parser
 import actdiag.builder
 import actdiag.drawer
 import seqdiag.parser
@@ -15,14 +14,15 @@
 import nwdiag.drawer
 import rackdiag.parser
 import rackdiag.builder
 import rackdiag.drawer
 import packetdiag.parser
 import packetdiag.builder
 import packetdiag.drawer
+from thothglyph.util.svg import svg2pdf
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
 def _get_svgstr(text):
     if text.startswith('blockdiag'):
@@ -81,13 +81,13 @@
 
 
 def customblock_write_latex(self, node):
     text = node.text
     svgstr, w, h = _get_svgstr(text)
     w, h = int(w), int(h)
     fname = os.path.join(self.tmpdirname, node.treeid() + '.pdf')
-    cairosvg.svg2pdf(bytestring=svgstr, write_to=fname)
+    svg2pdf(bytestring=svgstr, write_to=fname)
     w = '{}bp'.format(int(w * self.bp_scale))
     self.data += '\\tgincludegraphics[{}]{{{}}}\n\n'.format(w, fname)
 
 def customblock_write_pdf(self, node):
     customblock_write_latex(self, node)
```

### Comparing `thothglyph_doc-0.2.2/thothglyph/ext/graphviz.py` & `thothglyph_doc-0.2.3/thothglyph/ext/graphviz.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import re
-import cairosvg
 import graphviz
+from thothglyph.util.svg import svg2pdf
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
 def customblock_write_html(self, node):
     text = node.text
@@ -19,15 +19,15 @@
 
 
 def customblock_write_latex(self, node):
     text = node.text
     graph = graphviz.Source(text)  # type: ignore
     svgstr = graph.pipe(format='svg')
     fname = os.path.join(self.tmpdirname, node.treeid() + '.pdf')
-    cairosvg.svg2pdf(bytestring=svgstr, write_to=fname)
+    svg2pdf(bytestring=svgstr, write_to=fname)
     m = re.match(
         r'.+<svg width="(.+)pt" height="(.+)pt"', svgstr.decode(),
         flags=re.MULTILINE | re.DOTALL
     )
     assert m
     w, _ = int(m.group(1)), int(m.group(2))
     wstr = '{}bp'.format(int(w * self.bp_scale))
```

### Comparing `thothglyph_doc-0.2.2/thothglyph/ext/math.py` & `thothglyph_doc-0.2.3/thothglyph/ext/math.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/ext/wavedrom.py` & `thothglyph_doc-0.2.3/thothglyph/ext/wavedrom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import cairosvg
 import os
 import re
 import wavedrom
 
+from thothglyph.util.svg import svg2pdf
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
 def customblock_write_html(self, node):
     text = node.text
@@ -20,15 +20,15 @@
 
 
 def customblock_write_latex(self, node):
     text = node.text
     svg = wavedrom.render(text)  # type: ignore
     w = svg.attribs['width']
     fname = os.path.join(self.tmpdirname, node.treeid() + '.pdf')
-    cairosvg.svg2pdf(bytestring=svg._repr_svg_(), write_to=fname)
+    svg2pdf(bytestring=svg._repr_svg_(), write_to=fname)
     w = '{}bp'.format(int(w * self.bp_scale))
     self.data += '\\tgincludegraphics[{}]{{{}}}\n\n'.format(w, fname)
 
 
 def customblock_write_pdf(self, node):
     customblock_write_latex(self, node)
```

### Comparing `thothglyph_doc-0.2.2/thothglyph/node/logging.py` & `thothglyph_doc-0.2.3/thothglyph/node/logging.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/node/nd.py` & `thothglyph_doc-0.2.3/thothglyph/node/nd.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,16 @@
         self.type: str = 'normal'  # 'normal', 'long'
         self.row: int = 0
         self.col: int = 0
         self.headers: int = 0
         self.caption: Optional[str] = None
         self.align: str = 'l'  # table align
         self.aligns: List[str] = list()  # column alings
+        self.width: str = str()
+        self.widths: List[int] = list()  # column widths
 
     def cell(self, row: int, col: int) -> ASTNode:
         return self.children[row].children[col]
 
     def cells(self) -> Iterator:
         for row in self.children:
             for cell in row.children:
@@ -376,14 +378,15 @@
             self.x: int = x
             self.y: int = y
 
     def __init__(self):
         super().__init__()
         self.idx: int = -1
         self.align: str = 'c'
+        self.width: str = str()
         self.mergeto: Optional[TableCellNode] = None
         self.size: TableCellNode.Size = TableCellNode.Size(1, 1)
 
 
 class LiteralBlockNode(BlockNode):
     def __init__(self):
         super().__init__()
```

### Comparing `thothglyph_doc-0.2.2/thothglyph/reader/md.py` & `thothglyph_doc-0.2.3/thothglyph/reader/md.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/reader/reader.py` & `thothglyph_doc-0.2.3/thothglyph/reader/reader.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/reader/tglyph.py` & `thothglyph_doc-0.2.3/thothglyph/reader/tglyph.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from thothglyph.error import ThothglyphError
 from thothglyph.reader import ReaderClass
 from thothglyph.reader.reader import Reader, Parser
 from thothglyph.node import nd
 import re
 import os
 import sys
+import traceback
 
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
 class Lexer():
@@ -28,21 +29,21 @@
 
     newline_token: str = '\n'
     preproc_keywords: Tuple[str] = (
         'if', 'elif', 'else',
         'end',
     )
     preproc_tokens: Dict[str, str] = {
-        'CONFIG_LINE': r'⑇⑇⑇$',
-        'COMMENT': r'⑇⑇(.+)',
-        'CONTROL_FLOW': r'⑇(\w+)(.*)',
+        'CONFIG_LINE': r'^⑇⑇⑇$',
+        'COMMENT': r'⑇⑇(.+)$',
+        'CONTROL_FLOW': r'^ *⑇(\w+)([^⑇]*)⑇?',
         'TEXT': r'[^⑇]*',
     }
     block_tokens: Dict[str, str] = {
-        'PREPROCESSED_LINE': r'^⑇$',
+        'PREPROCESSED_SYMBOL': r'⑇+',
         'SECTION_TITLE_LINE': r' *((?:▮+)|(?:▯+))([*+]?) +([^⟦]+) *(?:⟦([^⟧]*)⟧)?',
         'TOC_LINE': r' *¤toc(?:⟦([^⟧]*)⟧)?⸨([^⸩]*)⸩ *$',
         'FIGURE_LINE': r' *¤figure(?:⟦([^⟧]*)⟧)?⸨([^⸩]*)⸩ *$',
         'TABLE_LINE': r'^ *\|.+\| *$',
         'LISTTABLE_BEGIN_LINE': r'^ *\|=== *(?:⟦([^⟧]*)⟧)? *$',
         'LISTTABLE_END_LINE': r'^ *===\| *$',
         'FOOTNOTE_LIST_SYMBOL': r' *•\[\^(.+)\](?: +|$)',
@@ -55,14 +56,15 @@
         'ORDERED_LIST_SYMBOL': r' *(꓾+)(?: +|$)',
         'DESC_LIST_SYMBOL': r' *(ᛝ+)([^ᛝ]+)ᛝ(?: +|$)',
         'LIST_TERMINATOR_SYMBOL': r' *(◃+) *$',
         'CUSTOM_LINE': r'( *)¤¤¤(.*)',
         'CODE_LINE': r'( *)⸌⸌⸌(.*)',
         'QUOTE_SYMBOL': r'^ *> ',
         'HR_LINE': r'^ *(?:(={4,})|(-{4,}))$',
+        'OPTION_LINE': r'^ *⟦([^⟧]*)⟧',
         'BREAK_PARAGRAPH': r' *⊹',
         'STR_LINE': r'.+',
         'EMPTY_LINE': r'^$',
     }
     listblock_keys: Tuple[str, ...] = (
         'BULLET_LIST_SYMBOL',
         'ORDERED_LIST_SYMBOL',
@@ -182,38 +184,42 @@
             self.tokens = self.lexer.lex_block(ppdata)
         except ThothglyphError as e:
             lineno, line, rests = e.args
             lineno += 1
             msg = 'Unknown token.'
             msg = f'{self.reader.path}:{lineno}: {msg}'
             raise ThothglyphError(msg)
+        self._remove_preprocessed_tokens()
         tokens = list() + self.tokens
         tokens = self.p_document(tokens)
         return self.rootnode
 
     def _tokens(self, token: Lexer.Token, offset: int) -> Lexer.Token:
-        return self.tokens[token.no + offset]
+        if token.no + offset >= len(self.tokens):
+            return None
+        return self.tokens[self.tokens.index(token) + offset]
 
     def preprocess(self, data: str) -> str:
         self._init_config()
         try:
-            tokens = self.lexer.lex_preproc(data)
+            self.tokens = self.lexer.lex_preproc(data)
         except ThothglyphError as e:
             lineno, line, rests = e.args
             lineno += 1
             msg = 'Unknown token.'
             msg = f'{self.reader.path}:{lineno}: {msg}'
             raise ThothglyphError(msg)
         self.pplines = list()
+        tokens = list() + self.tokens
         while tokens:
             if tokens[0].key == 'CONFIG_LINE':
                 tokens = self.p_configblock(tokens)
             elif tokens[0].key == 'COMMENT':
                 if tokens[0].pos == 0:
-                    self._line_preprocessed()
+                    self._line_preprocessed(tokens[0])
                 tokens.pop(0)
             elif tokens[0].key == 'CONTROL_FLOW':
                 tokens = self.p_controlflow(tokens)
             else:
                 self.pplines.append(tokens[0].value)
                 tokens.pop(0)
         ppdata = '\n'.join(self.pplines)
@@ -226,34 +232,40 @@
             pattrs = dict(pconfig.__dict__)
             for key in ('parent', 'children', 'id'):
                 pattrs.pop(key)
             for key in pattrs:
                 setattr(config, key, pattrs[key])
         self.rootnode.config = config
 
-    def _line_preprocessed(self):
-        self.pplines.append('⑇')
+    def _line_preprocessed(self, token: Lexer.Token) -> None:
+        is_head = (token.pos == 0)
+        is_tail = token == self.tokens[-1] or \
+            token.line + 1 == self._tokens(token, +1).line
+        if is_head and is_tail:
+            self.pplines.append('⑇' * len(token.value))
+        else:
+            self.pplines[-1] += '⑇' * len(token.value)
 
     def p_configblock(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
         config = self.rootnode.config
         begintoken = tokens[0]
-        self._line_preprocessed()
+        self._line_preprocessed(tokens[0])
         tokens.pop(0)
         subtokens = list()
         while tokens:
             if tokens[0].key == 'CONFIG_LINE':
                 break
-            self._line_preprocessed()
+            self._line_preprocessed(tokens[0])
             subtokens.append(tokens.pop(0))
         else:
             lineno = begintoken.line + 1
             msg = 'Config block is not closed.'
             msg = f'{self.reader.path}:{lineno}: {msg}'
             raise ThothglyphError(msg)
-        self._line_preprocessed()
+        self._line_preprocessed(tokens[0])
         tokens.pop(0)
         m = re.match(Lexer.inline_tokens['ROLE'], subtokens[0].value) if subtokens else None
         if m and m.group(1) == 'include':
             role = nd.RoleNode()
             role.role = m.group(1)
             role.opts = m.group(2).split(',') if m.group(2) is not None else ['']
             role.value = self.replace_text_attrs(m.group(3))
@@ -296,45 +308,77 @@
         return tokens
 
     def p_controlflow(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
         match = re.match(Lexer.preproc_tokens['CONTROL_FLOW'], tokens[0].value)
         assert match
         keyword, sentence = match.group(1), match.group(2)
         if keyword == 'if':
-            self._line_preprocessed()
+            self._line_preprocessed(tokens[0])
             tokens.pop(0)
             cond = eval(sentence, {}, self.rootnode.config.attrs)
-            tokens = self.p_if_else(tokens, cond)
+            tokens = self.p_if_else(tokens, [cond])
         else:
             lineno = tokens[0].line + 1
-            msg = 'Illegal text token.'
+            msg = 'Illegal ControlFlow token.'
             msg = f'{self.reader.path}:{lineno}: {msg}'
             raise ThothglyphError(msg)
         return tokens
 
-    def p_if_else(self, tokens: List[Lexer.Token], cond: bool) -> List[Lexer.Token]:
+    def p_if_else(self, tokens: List[Lexer.Token], conds: List[bool]) -> List[Lexer.Token]:
+        firstflowtoken = self._tokens(tokens[0], -1)
+        lastflowtoken = tokens[0]
+        lasttoken = tokens[0]
         while tokens:
-            if tokens[0].key == 'TEXT' and cond:
+            if tokens[0].key == 'TEXT' and all(conds):
                 self.pplines.append(tokens[0].value)
+                lasttoken = tokens.pop(0)
             elif tokens[0].key == 'CONTROL_FLOW':
                 match = re.match(Lexer.preproc_tokens['CONTROL_FLOW'], tokens[0].value)
                 assert match
+                lastflowtoken = tokens[0]
                 keyword, sentence = match.group(1), match.group(2)
                 if keyword == 'end':
                     break
+                elif keyword == 'if':
+                    self._line_preprocessed(tokens[0])
+                    tokens.pop(0)
+                    conds += [all(conds) and eval(sentence, {}, self.rootnode.config.attrs)]
+                    tokens = self.p_if_else(tokens, conds)
+                    lasttoken = tokens[0]
+                    conds.pop()
                 elif keyword == 'elif':
-                    cond = not cond and eval(sentence, {}, self.rootnode.config.attrs)
+                    conds[-1] = not all(conds) and eval(sentence, {}, self.rootnode.config.attrs)
+                    self._line_preprocessed(tokens[0])
+                    lasttoken = tokens.pop(0)
                 elif keyword == 'else':
-                    cond = not cond
-            self._line_preprocessed()
-            tokens.pop(0)
-        self._line_preprocessed()
+                    conds[-1] = not all(conds)
+                    self._line_preprocessed(tokens[0])
+                    lasttoken = tokens.pop(0)
+                else:
+                    lineno = lastflowtoken.line + 1
+                    msg = f'Unknown ControlFlow keyword: "{keyword}".'
+                    msg = f'{self.reader.path}:{lineno}: {msg}'
+                    raise ThothglyphError(msg)
+            else:
+                self._line_preprocessed(tokens[0])
+                lasttoken = tokens.pop(0)
+        else:
+            lineno0 = firstflowtoken.line + 1
+            # lineno1 = lastflowtoken.line + 1
+            lineno1 = lasttoken.line + 1
+            msg = 'ControlFlow is not closed.'
+            msg = f'{self.reader.path}:{lineno0}-{lineno1}: {msg}'
+            raise ThothglyphError(msg)
+        self._line_preprocessed(tokens[0])
         tokens.pop(0)
         return tokens
 
+    def _remove_preprocessed_tokens(self) -> None:
+        self.tokens = [t for t in self.tokens if t.key != 'PREPROCESSED_SYMBOL']
+
     def p_document(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
         tokens = self.p_ignore_emptylines(tokens)
         tokens = self.p_blocks(tokens)
         tokens = self.p_ignore_emptylines(tokens)
         return tokens
 
     @property
@@ -689,20 +733,27 @@
             subtokens.append(tokens.pop(0))
         else:
             lineno = begintoken.line + 1
             msg = 'Code block is not closed.'
             msg = f'{self.reader.path}:{lineno}: {msg}'
             raise ThothglyphError(msg)
         tokens.pop(0)
-        m = re.match(Lexer.inline_tokens['ROLE'], subtokens[0].value) if subtokens else None
-        if m and m.group(1) == 'include':
+        roleline_pat = r'( *)' + Lexer.inline_tokens['ROLE']
+        m = re.match(roleline_pat, subtokens[0].value) if subtokens else None
+        if m and m.group(2) == 'include':
+            numspace = len(m.group(1))
+            if numspace < indent:
+                msg = 'Code indentation is to the left of the block indentation.'
+                lineno = subtokens[0].line + 1
+                msg = f'{self.reader.path}:{lineno}: {msg}'
+                logger.warn(msg)
             role = nd.RoleNode()
-            role.role = m.group(1)
-            role.opts = m.group(2).split(',') if m.group(2) is not None else ['']
-            role.value = self.replace_text_attrs(m.group(3))
+            role.role = m.group(2)
+            role.opts = m.group(3).split(',') if m.group(3) is not None else ['']
+            role.value = self.replace_text_attrs(m.group(4))
             self.nodes.append(code)
             self.p_plaininclude(subtokens, role)
             self.nodes.pop()
         else:
             text = str()
             prev = begintoken
             warned = False
@@ -745,20 +796,27 @@
             subtokens.append(tokens.pop(0))
         else:
             lineno = begintoken.line + 1
             msg = 'Custom block is not closed.'
             msg = f'{self.reader.path}:{lineno}: {msg}'
             raise ThothglyphError(msg)
         tokens.pop(0)
-        m = re.match(Lexer.inline_tokens['ROLE'], subtokens[0].value) if subtokens else None
-        if m and m.group(1) == 'include':
+        roleline_pat = r'( *)' + Lexer.inline_tokens['ROLE']
+        m = re.match(roleline_pat, subtokens[0].value) if subtokens else None
+        if m and m.group(2) == 'include':
+            numspace = len(m.group(1))
+            if numspace < indent:
+                msg = 'Custom indentation is to the left of the block indentation.'
+                lineno = subtokens[0].line + 1
+                msg = f'{self.reader.path}:{lineno}: {msg}'
+                logger.warn(msg)
             role = nd.RoleNode()
-            role.role = m.group(1)
-            role.opts = m.group(2).split(',') if m.group(2) is not None else ['']
-            role.value = self.replace_text_attrs(m.group(3))
+            role.role = m.group(2)
+            role.opts = m.group(3).split(',') if m.group(3) is not None else ['']
+            role.value = self.replace_text_attrs(m.group(4))
             self.nodes.append(custom)
             self.p_plaininclude(subtokens, role)
             self.nodes.pop()
         else:
             prev = begintoken
             text = str()
             warned = False
@@ -815,31 +873,60 @@
         return ''
 
     def _extract_tablecell_merge_vmarker(self, text: str):
         if text.startswith('⏶'):
             return '⏶'
         return ''
 
+    def _parse_table_optargs(self, argstr: str) -> Dict[str, str]:
+        opts = nd.parse_optargs(argstr)
+        newopts: Dict[str, str] = dict()
+        newopts['type'] = opts.get('type', 'normal')
+        newopts['w'] = opts.get('w', '')
+        for k, v in opts.items():
+            if k == 'align':
+                newopts['align'] = [c for c in v]
+            elif k == 'widths':
+                newopts['widths'] = [int(x.strip()) for x in v.split(',')]
+            elif k == 'colspec':
+                colspec_ptn = r'(-1|[1-9]|[1-9][0-9]+)?([lcrx])'
+                colmatchs = [re.match(colspec_ptn, x.strip()) for x in v.split(',')]
+                if not all(colmatchs):
+                    pass  # logger.warn()
+                newopts['align'] = list()
+                newopts['widths'] = list()
+                for m in colmatchs:
+                    newopts['widths'].append(m.group(1) or 1)
+                    newopts['align'].append(m.group(2))
+        return newopts
+
     def p_basictableblock(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
+        prevtoken = self._tokens(tokens[0], -1)
+        opts: Dict[str, str] = dict()
+        if prevtoken and prevtoken.key == 'OPTION_LINE':
+            m = re.match(Lexer.block_tokens['OPTION_LINE'], prevtoken.value)
+            assert m
+            opts = self._parse_table_optargs(m.group(1))
         table = nd.TableBlockNode()
         self.nodes[-1].add(table)
         lines = list()
         begintoken = tokens[0]
         while tokens:
             if tokens[0].key != 'TABLE_LINE':
                 break
             lines.append(tokens[0].value)
             tokens.pop(0)
         tabletexts = list()
-        aligns = list()
+        aligns = opts.get('align', list())
         header_splitter = -1
         for i, line in enumerate(lines):
             rowtexts = re.split(r' *\| *', line.strip())[1:-1]
             ms = [re.match(r'^[+:]?-+[+:]?$', c) for c in rowtexts]
             if all(ms) and header_splitter == -1:
+                aligns = list()
                 for m in ms:
                     assert m
                     mg = m.group(0)
                     if mg[0] == mg[-1] == ':':
                         aligns.append('c')
                     elif mg[-1] == ':':
                         aligns.append('r')
@@ -848,21 +935,23 @@
                     else:
                         aligns.append('l')
                 header_splitter = i
             else:
                 tabletexts.append(rowtexts)
         if header_splitter < 0:
             header_splitter = 0
-        # table.type = opts.get('type', 'normal')
+        table.type = opts.get('type', 'normal')
         table.row = len(tabletexts)
         table.col = len(tabletexts[0])
         table.headers = header_splitter
         if len(aligns) == 0:
             aligns = ['c' for i in range(table.col)]
         table.aligns = aligns
+        table.widths = opts.get('widths', [0 for i in range(table.col)])
+        table.width = opts.get('w')
         for r, rowtexts in enumerate(tabletexts):
             row = nd.TableRowNode()
             row.idx = r
             if r < table.headers:
                 row.tp = 'header'
             table.add(row)
             if len(rowtexts) != table.col or len(table.aligns) != table.col:
@@ -873,29 +962,31 @@
                 msg = f'{self.reader.path}:{lineno}: {msg}'
                 raise ThothglyphError(msg)
             for c, celltext in enumerate(rowtexts):
                 cell = nd.TableCellNode()
                 row.add(cell)
                 cell.idx = c
                 cell.align = table.aligns[c]
+                cell.width = table.widths[c]
                 text = self.replace_text_attrs(celltext)
                 text = self._tablecell_merge(table, cell, r, c, text)
                 try:
                     texttokens = self.lexer.lex_inline(text)
                     self.nodes.append(cell)
                     self.p_inlinemarkup(texttokens)
                     self.nodes.pop()
                 except Exception:
                     cell.add(nd.TextNode(text))
         return tokens
 
     def p_listtableblock(self, tokens: List[Lexer.Token]) -> List[Lexer.Token]:
         m = re.match(Lexer.block_tokens['LISTTABLE_BEGIN_LINE'], tokens[0].value)
         assert m
-        opts = nd.parse_optargs(m.group(1))
+        # opts = nd.parse_optargs(m.group(1))
+        opts = self._parse_table_optargs(m.group(1))
         begintoken = tokens[0]
         tokens.pop(0)
         nested = 1
         subtokens = list()
         while tokens:
             if tokens[0].key == 'LISTTABLE_BEGIN_LINE':
                 nested += 1
@@ -941,14 +1032,16 @@
         table.type = opts.get('type', 'normal')
         table.aligns = ['l' for i in range(len(rowitems[0].children[0].children))]
         for i, align in enumerate(opts.get('align', '')):
             table.aligns[i] = align
         table.row = len(rowitems)
         table.col = len(rowitems[0].children[0].children)
         table.headers = len(header_rowlist.children)
+        table.widths = opts.get('widths', [0 for i in range(table.col)])
+        table.width = opts.get('w')
         for r, rowitem in enumerate(rowitems):
             row = nd.TableRowNode()
             row.idx = r
             if r < table.headers:
                 row.tp = 'header'
             table.add(row)
             collist = rowitem.children[0]
@@ -956,14 +1049,15 @@
                 cell = nd.TableCellNode()
                 for node in citem.children[:]:
                     citem.remove(node)
                     cell.add(node)
                 row.add(cell)
                 cell.idx = c
                 cell.align = table.aligns[c]
+                cell.width = table.widths[c]
                 if not (all([
                     cell.children,
                     isinstance(cell.children[0], nd.ParagraphNode),
                     cell.children[0].children,
                     isinstance(cell.children[0].children[0], nd.TextNode),
                 ])):
                     continue
@@ -1230,12 +1324,15 @@
             return super().read(path, encoding)
         except ThothglyphError as e:
             msg = e.args[-1]
             raise ThothglyphError(msg)
         except OSError as e:
             msg = '{}: {}'.format(e.strerror, e.filename)
             raise ThothglyphError(msg)
-        except Exception:
-            exc_type, exc_msg, exc_tb = sys.exc_info()
-            tbinfo = 'file {}, line {}'.format(exc_tb.tb_frame.f_code.co_filename, exc_tb.tb_lineno)
-            msg = '{} ({})'.format(exc_msg, tbinfo)
+        except Exception as e:
+            te = traceback.TracebackException.from_exception(e)
+            exc_msg = str(te)
+            tbinfo = 'file {}, line {}'.format(
+                te.stack[-1].filename, te.stack[-1].lineno
+            )
+            msg = 'inner error: {} ({})'.format(exc_msg, tbinfo)
             raise ThothglyphError(msg)
```

### Comparing `thothglyph_doc-0.2.2/thothglyph/template/common/check_dis.pdf` & `thothglyph_doc-0.2.3/thothglyph/template/common/check_dis.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/template/common/check_dis.svg` & `thothglyph_doc-0.2.3/thothglyph/template/common/check_dis.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/template/common/check_en.pdf` & `thothglyph_doc-0.2.3/thothglyph/template/common/check_en.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/template/common/check_en.svg` & `thothglyph_doc-0.2.3/thothglyph/template/common/check_en.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/template/common/check_im.pdf` & `thothglyph_doc-0.2.3/thothglyph/template/common/check_im.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/template/common/check_im.svg` & `thothglyph_doc-0.2.3/thothglyph/template/common/check_im.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/template/docx/default/style.docx` & `thothglyph_doc-0.2.3/thothglyph/template/docx/default/style.docx`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/template/html/default/index.html` & `thothglyph_doc-0.2.3/thothglyph/template/html/default/index.html`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/template/html/preview/index.html` & `thothglyph_doc-0.2.3/thothglyph/template/html/preview/index.html`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/template/latex/default/document-ja.tex` & `thothglyph_doc-0.2.3/thothglyph/template/latex/default/document-ja.tex`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/writer/docx.py` & `thothglyph_doc-0.2.3/thothglyph/writer/docx.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/thothglyph/writer/html.py` & `thothglyph_doc-0.2.3/thothglyph/writer/latex.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,65 @@
+# sudo apt install texlive-luatex texlive-fonts-recommended texlive-fonts-extra texlive-lang-cjk
 from __future__ import annotations
-from typing import Dict, List, Optional
-import html
+from typing import Dict, Optional, Tuple, Union
 import importlib
 import os
 import re
-import shutil
 import tempfile
+from PIL import Image
 from thothglyph.error import ThothglyphError
 from thothglyph.writer.writer import Writer
 from thothglyph.node import nd
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
-class HtmlWriter(Writer):
-    target = 'html'
-    ext = 'html'
-
-    decoration_table: Dict[str, str] = {
-        'EMPHASIS': 'em',
-        'STRONG': 'strong',
-        'MARKED': 'u',
-        'STRIKE': 's',
-        'VAR': 'var',
-        'CODE': 'code',
-        'SUP': 'sup',
-        'SUB': 'sub',
+class LatexWriter(Writer):
+    target = 'latex'
+    ext = 'tex'
+
+    sectlevel_cmds: Dict[str, Tuple[str, ...]] = {
+        'article': ('section', 'subsection', 'paragraph', 'subparagraph'),
+        'report': ('chapter', 'section', 'subsection', 'paragraph', 'subparagraph'),
+        'book': ('chapter', 'section', 'subsection', 'paragraph', 'subparagraph'),
     }
+    decoration_table: Dict[str, Tuple[str, str]] = {
+        'EMPHASIS': ('\\textit{', '}'),
+        'STRONG': ('\\textbf{', '}'),
+        'MARKED': ('\\uline{', '}'),
+        'STRIKE': ('\\sout{', '}'),
+        'VAR': ('\\varbox{', '}'),
+        'CODE': ('\\codebox{', '}'),
+        'SUP': ('\\textsuperscript{', '}'),
+        'SUB': ('\\textsubscript{', '}'),
+    }
+    code_decoration_table: Dict[str, Tuple[str, str]] = {
+        'EMPHASIS': '<?tg:I?>',
+        'STRONG': '<?tg:S?>',
+        'MARKED': '<?tg:U?>',
+        'STRIKE': '<?tg:SO?>',
+        'VAR': '<?tg:VAR?>',
+        'CODE': '',
+        'SUP': '',
+        'SUB': '',
+    }
+    bp_scale: float = 72.0 / 150.0
 
     def __init__(self):
         super().__init__()
         self.tmpdirname: Optional[str] = None
-        self.imgdirname: str = 'img'
+        self.contentphase: str = 'before'  # before, main, after
 
-    def parse(self, node: nd.ASTNode) -> None:
+    def parse(self, node) -> None:
         super().parse(node)
         template_dir = self.template_dir()
-        target = self.target
+        target = LatexWriter.target
         theme = self.theme()
-        template_path = os.path.join(template_dir, target, theme, 'index.html')
+        template_path = os.path.join(template_dir, target, theme, 'document-ja.tex')
         if not os.path.exists(template_path):
             raise ThothglyphError('template not found: {}'.format(template_path))
         with open(template_path, 'r', encoding=self.encoding) as f:
             template = f.read()
         t = template.replace('{', '{{').replace('}', '}}')
         t = re.sub(r'\$\{\{([^}]+)\}\}', r'{\1}', t)
         self.data = t.format(doc=self.template_docdata)
@@ -51,405 +67,452 @@
     def write(self, fpath: str, node: nd.ASTNode) -> None:
         clsname = self.__class__.__name__
         logger.info('{}: write document'.format(clsname))
         self.rootnode = node
         with tempfile.TemporaryDirectory() as tmpdirname:
             self.tmpdirname = tmpdirname
             self.parse(node)
-            self._copy_template(fpath)
-            self._copy_resources(fpath)
-            fdir = os.path.abspath(fpath + '.dir')
-            indexpath = os.path.join(self.tmpdirname, 'index.html')
-            with open(indexpath, 'w', encoding=self.encoding) as f:
+            with open(fpath, 'w', encoding=self.encoding) as f:
                 f.write(self.data)
-            os.makedirs(fdir, exist_ok=True)
-            shutil.copytree(self.tmpdirname, fdir, dirs_exist_ok=True)
         self.tmpdirname = None
 
-    def _copy_template(self, fpath: str) -> None:
-        commondir = os.path.join(self.template_dir(), 'common')
-        if not os.path.exists(commondir):
-            commondir = os.path.join(self.pkg_template_dir(), 'common')
-        newcommondir = os.path.join(self.tmpdirname, 'template', 'common')
-        shutil.copytree(commondir, newcommondir, dirs_exist_ok=True)
-
-    def _copy_resources(self, fpath: str) -> None:
-        rscs: Dict[str, List[str]] = dict()
-        typetable: Dict[str, Dict[str, str]] = {
-            'img': {
-                'dir': os.path.join(self.tmpdirname, self.imgdirname),
-            },
-        }
-        for n, gofoward in self.rootnode.walk_depth():
-            if not gofoward:
-                continue
-            if isinstance(n, nd.ImageRoleNode):
-                tp = 'img'
-                path = os.path.abspath(n.value)
-            else:
-                continue
-            rscs.setdefault(tp, list())
-            if path not in rscs[tp]:
-                rscs[tp].append(path)
-        for tp, paths in rscs.items():
-            newrscdir = typetable[tp]['dir']
-            os.makedirs(newrscdir, exist_ok=True)
-            for rscpath in paths:
-                _, rscfname = os.path.split(rscpath)
-                shutil.copy2(rscpath, os.path.join(newrscdir, rscfname))
+    def visit_document(self, node: nd.ASTNode) -> None:
+        self.data += '\\setcounter{page}{0}\n'
+        self.data += '\\pagenumbering{arabic}\\pagestyle{beforecontents}\n'
 
     def visit_section(self, node: nd.ASTNode) -> None:
-        self.data += '<section>'
+        level_offset = 0
         _id = node.id or node.title.replace(' ', '_')
-        if node.opts.get('nonum'):
-            title = node.title
-        else:
-            title = '{}. {}'.format(node.sectnum, node.title)
-        if node.opts.get('notoc'):
-            toc = 'class="notoc"'
-        else:
-            toc = ''
-        if node.level < 7:
-            tag = '<h{0} {3} id="{2}">{1}</h{0}>\n'
-            self.data += tag.format(node.level, title, _id, toc)
-        else:
-            tag = '<div class="section h{0}" id="{2}">{1}</div>\n'
-            self.data += tag.format(node.level, title, _id)
+        title = tex_escape(node.title)
+        doctype = 'report'
+        level = min(node.level - 1, len(self.sectlevel_cmds[doctype]) - 1) + level_offset
+        cmd = self.sectlevel_cmds[doctype][level]
+        asterisk = ''
+        if node.opts.get('notoc') or node.opts.get('nonum'):
+            asterisk = '*'
+        if not node.opts.get('notoc') and node.level == 1 and self.contentphase == 'before':
+            self.data += '\\pagenumbering{arabic}\\pagestyle{fancy}\n'
+            self.contentphase = 'main'
+        self.data += '\\{}{}{{{}}}'.format(cmd, asterisk, title)
+        if not node.opts.get('notoc') and node.opts.get('nonum'):
+            self.data += '\\addcontentsline{{toc}}{{{}}}{{{}}}'.format(cmd, title)
+        self.data += '\\label{{{}}}\n'.format(_id)
 
     def leave_section(self, node: nd.ASTNode) -> None:
-        self.data += '</section>\n'
+        pass
 
     def visit_tocblock(self, node: nd.ASTNode) -> None:
-        self.data += '<div>\n'
-        maxlevel = int(node.opts.get('level', '100'))
-        for n, gofoward in node.walk_sections():
-            if n.opts.get('notoc'):
-                continue
-            if gofoward and n.level <= maxlevel:
-                bros = [s for s in n.parent.children if isinstance(n, nd.SectionNode)]
-                if bros.index(n) == 0:
-                    self.data += '<ul>\n'
-                if n.opts.get('nonum'):
-                    title = '{}'.format(n.title)
-                else:
-                    title = '{}. {}'.format(n.sectnum, n.title)
-                _id = n.id or n.title.replace(' ', '_')
-                self.data += '<li><a href="#{}">{}</a></li>\n'.format(_id, title)
-                if bros.index(n) == len(bros) - 1:
-                    self.data += '</ul>\n'
-        self.data += '</div>\n'
+        self.data += '\\tableofcontents\n'
 
     def leave_tocblock(self, node: nd.ASTNode) -> None:
-        pass
+        self.data += '\\clearpage\\setcounter{page}{0}\n'
 
     def visit_bulletlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '<ul>\n'
+        self.data += '\\begin{itemize}\n'
 
     def leave_bulletlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '</ul>\n'
+        self.data += '\\end{itemize}\n'
 
     def visit_orderedlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '<ol>\n'
+        self.data += '\\begin{enumerate}\n'
 
     def leave_orderedlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '</ol>\n'
+        self.data += '\\end{enumerate}\n'
 
     def visit_descriptionlistblock(self, node: nd.ASTNode) -> None:
-        if not node.titlebreak:
-            self.data += '<dl class="compactdl">\n'
-        else:
-            self.data += '<dl>\n'
+        self.data += '\\begin{description}\n'
 
     def leave_descriptionlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '</dl>\n'
+        self.data += '\\end{description}\n'
 
     def visit_checklistblock(self, node: nd.ASTNode) -> None:
-        self.data += '<ul class="checklist">\n'
+        self.data += '\\begin{tgchecklist}\n'
 
     def leave_checklistblock(self, node: nd.ASTNode) -> None:
-        self.data += '</ul>\n'
+        self.data += '\\end{tgchecklist}\n'
 
     def visit_footnotelistblock(self, node: nd.ASTNode) -> None:
-        self.data += '<ul class="footnotelist">'
+        self._continue()
 
     def leave_footnotelistblock(self, node: nd.ASTNode) -> None:
-        self.data += '</ul>'
+        pass
 
     def visit_referencelistblock(self, node: nd.ASTNode) -> None:
-        self.data += '<ul class="referencelist">'
+        self.data += '\\begin{thebibliography}{{99}}\n'
 
     def leave_referencelistblock(self, node: nd.ASTNode) -> None:
-        self.data += '</ul>'
+        self.data += '\\end{thebibliography}\n'
 
     def visit_listitem(self, node: nd.ASTNode) -> None:
         if isinstance(node.parent, nd.DescriptionListBlockNode):
             pass
         elif isinstance(node.parent, nd.CheckListBlockNode):
             if node.marker == 'x':
-                liclass = 'check_en'
+                self.data += '\\item[{\\tgcheck[en]}] '
             elif node.marker == '-':
-                liclass = 'check_im'
+                self.data += '\\item[{\\tgcheck[im]}] '
             else:
-                liclass = 'check_dis'
-            self.data += '<li class="checklist {}">'.format(liclass)
+                self.data += '\\item[{\\tgcheck[dis]}] '
         elif isinstance(node.parent, nd.FootnoteListBlockNode):
-            url = 'fn.{}-{}'.format(node.treeindex()[1], node.fn_num)
-            text = node.fn_num  # node.title
-            self.data += '<li> '
-            self.data += '<span id="{}">{}</span>. '.format(url, text)
+            pass  # unreach
         elif isinstance(node.parent, nd.ReferenceListBlockNode):
             url = 'ref.{}'.format(node.ref_num)
-            text = node.ref_num  # node.title
-            self.data += '<li> '
-            self.data += '[<span id="{}">{}</span>] '.format(url, text)
-            # self.data += '<li id="{}">[{}] '.format(url, text)
+            self.data += '\\bibitem{{{}}} '.format(url)
         else:
-            self.data += '<li>'
+            self.data += '\\item '
 
     def leave_listitem(self, node: nd.ASTNode) -> None:
-        if isinstance(node.parent, nd.DescriptionListBlockNode):
-            self.data += '</dd>\n'
-            if not node.parent.titlebreak:
-                self.data += '</div>'
-        else:
-            self.data += '</li>\n'
+        if isinstance(node.parent, nd.FootnoteListBlockNode):
+            pass  # unreach
+        elif isinstance(node.parent, nd.ReferenceListBlockNode):
+            self.data += '\n'
 
     def visit_quoteblock(self, node: nd.ASTNode) -> None:
-        self.data += '<blockquote>'
+        self.data += '\\begin{quote}\n'
 
     def leave_quoteblock(self, node: nd.ASTNode) -> None:
-        self.data += '</blockquote>'
+        self.data += '\\end{quote}\n'
 
     def visit_codeblock(self, node: nd.ASTNode) -> None:
-        self.data += '<pre><code>'
+        self.data += '\\begin{lstlisting}'
+        if node.lang:
+            self.data += '[style={}]'.format(node.lang)
+        self.data += '\n'
 
     def leave_codeblock(self, node: nd.ASTNode) -> None:
-        self.data += '</code></pre>\n'
+        self.data += '\\end{lstlisting}\n'
 
     def visit_figureblock(self, node: nd.ASTNode) -> None:
-        if node.align == 'l':
-            style = 'style="text-align:left;"'
-        elif node.align == 'c':
-            style = 'style="text-align:center;"'
-        elif node.align == 'r':
-            style = 'style="text-align:right;"'
+        align = node.align
+        table_align_cmd = {
+            'l': 'raggedright',
+            'c': 'centering',
+            'r': 'raggedleft',
+        }
+        self.data += '\\begin{figure}[H]\n'
+        self.data += '\\{}\n'.format(table_align_cmd[align])
+        opts = 'singlelinecheck=false,justification={}'
+        opts = opts.format(table_align_cmd[align])
+        self.data += '\\captionsetup{{{}}}\n'.format(opts)
         if isinstance(node.children[0], nd.TableBlockNode):
-            self.data += '<figure {}>\n'.format(style)
-            self.data += '<figcaption>'
-            self.data += '{} {}'.format(node.fignum, node.caption)
-            self.data += '</figcaption>\n'
+            self.data += '\\captionof{{table}}{{{}}}\n'.format(node.caption)
         else:
-            self.data += '<figure {}>\n'.format(style)
+            self.data += '\\captionof{{figure}}{{{}}}\n'.format(node.caption)
 
     def leave_figureblock(self, node: nd.ASTNode) -> None:
-        if isinstance(node.children[0], nd.TableBlockNode):
-            self.data += '</figure>\n'
-        else:
-            self.data += '<figcaption>'
-            self.data += '{} {}'.format(node.fignum, node.caption)
-            self.data += '</figcaption>\n'
-            self.data += '</figure>\n'
+        self.data += '\\end{figure}\n'
+
+    style_gridtable = True
 
     def visit_tableblock(self, node: nd.ASTNode) -> None:
         align = node.align
         if isinstance(node.parent, nd.FigureBlockNode):
             align = node.parent.align
-        if align == 'l':
-            style = 'style="margin-right:auto;"'
-        elif align == 'c':
-            style = 'style="margin-left:auto;margin-right:auto;"'
-        elif align == 'r':
-            style = 'style="margin-left:auto;"'
-        self.data += '<table {}>\n'.format(style)
+        table_align_cmd = {
+            'l': 'raggedright',
+            'c': 'centering',
+            'r': 'raggedleft',
+        }
+        aligns = node.aligns[:]
+        widths = [int(v) for v in node.widths]
+        for i, a in enumerate(aligns):
+            if a == 'x':
+                if widths[i]:
+                    aligns[i] = 'X[{},l]'.format(widths[i])
+                else:
+                    aligns[i] = 'X[l]'
+            else:
+                if widths[i]:
+                    aligns[i] = 'X[{},{}]'.format(widths[i], a)
+                else:
+                    aligns[i] = a
+        if self.style_gridtable:
+            col_aligns = '|{}|'.format('|'.join(aligns))
+        else:
+            col_aligns = '{}'.format(' '.join(aligns))
+        if not node._parent_table():
+            self.data += '\\{}'.format(table_align_cmd[align])
+            if node.type == 'long':
+                self.data += '\\begin{longtblr}\n'
+            # elif isinstance(node.parent, nd.FigureBlockNode):
+            #     self.data += '\\begin{talltblr}\n'
+            else:
+                self.data += '\\begin{tblr}\n'
+            self.data += '['
+            self.data += 'entry=none, label=none,'
+            self.data += ']\n'
+        else:
+            self.data += '\\begin{tblr}\n'
+        self.data += '{'
+        if node.width:
+            w = node.width
+            if w.endswith('px'):
+                w = '{}bp'.format(int(float(w[0:-2]) * self.bp_scale))
+            elif w.endswith('%'):
+                w = '{}\\linewidth'.format(float(w[0:-1]) * 0.01)
+            self.data += 'width = {} ,'.format(w)
+        self.data += 'colspec = {{{}}}, '.format(col_aligns)
+        self.data += 'hlines, vlines, '
+        self.data += 'measure = vbox, '
+        self.data += '}\n'
 
     def leave_tableblock(self, node: nd.ASTNode) -> None:
-        self.data += '</table>\n'
+        if not node._parent_table():
+            if node.type == 'long':
+                self.data += '\\end{longtblr}\n\n'
+            # elif isinstance(node.parent, nd.FigureBlockNode):
+            #     self.data += '\\end{talltblr}\n\n'
+            else:
+                self.data += '\\end{tblr}\n\n'
+        else:
+            self.data += '\\end{tblr}\n\n'
+
+        fns = list()
+        for n, gofoward in node.walk_depth():
+            if not gofoward:
+                continue
+            if isinstance(n, nd.FootnoteNode):
+                fns.append(n)
+        for i, fn in enumerate(fns):
+            self.data += '\\footnotetext[{}]{{\n'.format(fn.fn_num)
+            for n in fn.description.children:
+                Writer.parse(self, n)
+            self.data += '}\n'
 
     def visit_tablerow(self, node: nd.ASTNode) -> None:
-        self.data += '<tr>\n'
+        if node.idx > 0:
+            self.data += ' \\\\\n'
+        # if node.tp == 'header':
+        #     self.data += '\\tgthrowcolor\n'
+        # else:
+        #     self.data += '\\tgtdrowcolor\n'
 
     def leave_tablerow(self, node: nd.ASTNode) -> None:
-        self.data += '</tr>\n'
+        if node.idx == len(node.parent.children) - 1:
+            self.data += ' \\\\\n'
 
     def visit_tablecell(self, node: nd.ASTNode) -> None:
-        tagname = 'td'
-        if node.parent.tp == 'header':
-            tagname = 'th'
+        if self.style_gridtable:
+            align = '{}|'.format(node.align)
+        else:
+            align = '{}'.format(node.align)
         if node.mergeto is None:
+            if node.idx != 0:
+                self.data += ' & '
             s = node.size
-            align = {'l': 'left', 'c': 'center', 'r': 'right', 'x': 'left'}
-            attrs = ['style="text-align:{}"'.format(align[node.align])]
-            attrs += ['colspan="{}"'.format(s.x), 'rowspan="{}"'.format(s.y)]
-            self.data += '<{} {}>'.format(tagname, ' '.join(attrs))
+            if s.x > 1:
+                self.data += '\\multicolumn{{{}}}{{{}}}{{'.format(s.x, align)
+            if s.y > 1:
+                self.data += '\\multirow{{{}}}{{*}}{{'.format(s.y)
+            self.data += '\n{\\begin{varwidth}{\\linewidth}\n'
+        elif node.mergeto.idx == node.idx and node.mergeto.parent.idx != node.parent.idx:
+            # horizontal cell merging
+            if node.idx != 0:
+                self.data += ' & '
+            s = node.mergeto.size
+            if s.x > 1:
+                self.data += '\\multicolumn{{{}}}{{{}}}{{'.format(s.x, align)
         else:
-            self._continue()
+            # vertical cell merging
+            pass
 
     def leave_tablecell(self, node: nd.ASTNode) -> None:
-        tagname = 'td'
-        if node.parent.tp == 'header':
-            tagname = 'th'
         if node.mergeto is None:
-            self.data += '</{}>'.format(tagname)
-        else:
-            pass
+            self.data += '\n\\end{varwidth}}\n'
+            s = node.size
+            if s.x > 1:
+                self.data += '}'
+            if s.y > 1:
+                self.data += '}'
+        elif node.mergeto.idx == node.idx and node.mergeto.parent.idx != node.parent.idx:
+            s = node.mergeto.size
+            if s.x > 1:
+                self.data += '}'
 
     def visit_customblock(self, node: nd.ASTNode) -> None:
         if node.ext == '':
-            self.data += '<pre><code>'
-            self.data += html.escape(node.text) + '\n'
-            self.data += '</code></pre>\n'
+            self.data += '\\begin{lstlisting}\n'
+            self.data += node.text + '\n'
+            self.data += '\\end{lstlisting}\n'
         else:
             try:
                 extpath = 'thothglyph.ext.{}'.format(node.ext)
                 extmodule = importlib.import_module(extpath)
-                extmodule.customblock_write_html(self, node)
+                extmodule.customblock_write_latex(self, node)
             except Exception:
-                self.data += '<pre><code>'
-                self.data += html.escape(node.text) + '\n'
-                self.data += '</code></pre>\n'
+                self.data += '\\begin{lstlisting}\n'
+                self.data += node.text + '\n'
+                self.data += '\\end{lstlisting}\n'
 
     def leave_customblock(self, node: nd.ASTNode) -> None:
         pass
 
-    def visit_horizonblock(self, node: nd.ASTNode) -> None:
-        self.data += '<hr />'
-
-    def leave_horizonblock(self, node: nd.ASTNode) -> None:
-        pass
-
     def visit_paragraph(self, node: nd.ASTNode) -> None:
-        if not all([
-            isinstance(node.parent, nd.ListItemNode),
-            len(node.parent.children) == 1
-        ]):
-            self.data += '<p>'
+        pass
 
     def leave_paragraph(self, node: nd.ASTNode) -> None:
-        if not all([
-            isinstance(node.parent, nd.ListItemNode),
-            len(node.parent.children) == 1
-        ]):
-            self.data += '</p>\n'
+        self.data += '\n\n'
 
     def visit_title(self, node: nd.ASTNode) -> None:
         if isinstance(node.parent, nd.ListItemNode):
-            if not node.parent.parent.titlebreak:
-                self.data += '<div>'
-            self.data += '<dt>'
+            self.data += '\\item[\\desctitle{'
 
     def leave_title(self, node: nd.ASTNode) -> None:
         if isinstance(node.parent, nd.ListItemNode):
-            self.data += '</dt><dd>'
+            self.data += '}] '
+            if node.parent.titlebreak:
+                self.data += '\\mbox{}\\\\ '
 
     def visit_decorationrole(self, node: nd.ASTNode) -> None:
-        self.data += '<{}>'.format(self.decoration_table[node.role])
+        if isinstance(node.parent_block, nd.CodeBlockNode):
+            self.data += self.code_decoration_table[node.role]
+        else:
+            self.data += self.decoration_table[node.role][0]
 
     def leave_decorationrole(self, node: nd.ASTNode) -> None:
-        self.data += '</{}>'.format(self.decoration_table[node.role])
+        if isinstance(node.parent_block, nd.CodeBlockNode):
+            self.data += self.code_decoration_table[node.role]
+        else:
+            self.data += self.decoration_table[node.role][1]
 
     def visit_role(self, node: nd.ASTNode) -> None:
         if node.role == '':
-            self.data += '<code>'
-            self.data += html.escape(node.value)
-            self.data += '</code>\n'
+            self.data += '\\fbox{\\lstinline{'
+            self.data += node.value
+            self.data += '}}\n'
         else:
             try:
                 extpath = 'thothglyph.ext.{}'.format(node.role)
                 extmodule = importlib.import_module(extpath)
-                extmodule.role_write_html(self, node)
+                extmodule.role_write_latex(self, node)
             except Exception:
-                self.data += '<code>'
-                self.data += html.escape(node.value)
-                self.data += '</code>\n'
+                self.data += '\\fbox{\\lstinline{'
+                self.data += node.value
+                self.data += '}}\n'
 
     def leave_role(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_imagerole(self, node: nd.ASTNode) -> None:
-        options = dict()
+        fname, ext = os.path.splitext(node.value)
+        if ext == '.svg':
+            assert self.tmpdirname
+            imgpath = os.path.join(self.tmpdirname, node.value)
+            inc_imgpath = '{}.pdf'.format(imgpath)
+        else:
+            imgpath = node.value
+            inc_imgpath = imgpath
         if 'w' in node.opts:
-            options['width'] = node.opts['w']
-        optstr = ' '.join(['{}="{}"'.format(k, v) for k, v in options.items()])
-        fname = os.path.basename(node.value)
-        _, ext = os.path.splitext(fname)
-        imgpath = os.path.join(self.imgdirname, fname)
-        if ext.lower() == '.svg':
-            src = 'type="image/svg+xml" data="{}"'.format(imgpath)
-            self.data += '<object {} {}></object>'.format(src, optstr)
+            w = node.opts['w']
+            if w.endswith('px'):
+                w = '{}bp'.format(int(float(w[0:-2]) * self.bp_scale))
+            elif w.endswith('%'):
+                w = '{}\\linewidth'.format(float(w[0:-1]) * 0.01)
         else:
-            src = 'src="{}"'.format(imgpath)
-            self.data += '<image {} {} />'.format(src, optstr)
+            try:
+                with Image.open(node.value) as img:
+                    w = '{}bp'.format(img.width)
+            except Exception:
+                w = '\\linewidth'
+        self.data += '\\tgincludegraphics[{}]{{{}}}'.format(w, inc_imgpath)
 
     def leave_imagerole(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_kbdrole(self, node: nd.ASTNode) -> None:
-        texts = [html.escape(t) for t in node.value]
-        value = ' + '.join(['<kbd>{}</kbd>'.format(v) for v in texts])
-        self.data += value
+        value = ['\\kbdbox{{{}}}'.format(v) for v in node.value]
+        valuestr = ' {\\scriptsize+} '.join(value)
+        self.data += valuestr
 
     def leave_kbdrole(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_btnrole(self, node: nd.ASTNode) -> None:
-        value = '<kbd>{}</kbd>'.format(html.escape(node.value))
+        value = '\\btnbox{{{}}}'.format(node.value)
         self.data += value
 
     def leave_btnrole(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_menurole(self, node: nd.ASTNode) -> None:
-        texts = [html.escape(t) for t in node.value]
-        value = ' > '.join(['<span class="menu">{}</span>'.format(v) for v in texts])
-        self.data += value
+        value = ['\\menubox{{{}}}'.format(v) for v in node.value]
+        valuestr = ' {\\tiny>} '.join(value)
+        self.data += valuestr
 
     def leave_menurole(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_link(self, node: nd.ASTNode) -> None:
         if '://' in node.value:
-            blank = 'target=”_blank”'
             url = node.value
             text = node.opts[0] if node.opts[0] else node.value
+            text = tex_escape(text)
+            self.data += '\\href{{{}}}{{{}}}'.format(url, text)
         else:
-            blank = ''
-            url = '#' + node.target_id
+            url = node.target_id or node.value.replace(' ', '_')
             text = node.opts[0] if node.opts[0] else node.target_title
-        text = html.escape(text)
-        self.data += '<a href="{}" {}>{}</a>'.format(url, blank, text)
+            text = tex_escape(text)
+            self.data += '\\nameref{{{}}}'.format(url)
 
     def leave_link(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_footnote(self, node: nd.ASTNode) -> None:
-        url = '#fn.{}-{}'.format(node.treeindex()[1], node.fn_num)
-        text = node.fn_num  # node.value
-        self.data += '<sup><a href="{}">{}</a></sup>'.format(url, text)
+        table = node._parent_table()
+        if table:
+            self.data += ' \\footnotemark[{}] '.format(node.fn_num)
+        else:
+            url = node.fn_num
+            self.data += '\\footnote[{}]{{'.format(url)
+            for n in node.description.children:
+                Writer.parse(self, n)
+            self.data += '}'
 
     def leave_footnote(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_reference(self, node: nd.ASTNode) -> None:
-        url = '#ref.{}'.format(node.ref_num)
-        text = node.ref_num  # node.value
-        self.data += '[<a href="{}">{}</a>]'.format(url, text)
+        url = 'ref.{}'.format(node.ref_num)
+        self.data += '\\cite{{{}}}'.format(url)
 
     def leave_reference(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_linebreak(self, node: nd.ASTNode) -> None:
-        self.data += '<br />'
+        self.data += '{\\newline}'
 
     def leave_linebreak(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_text(self, node: nd.ASTNode) -> None:
-        self.data += node.text
+        if isinstance(node.parent_block, nd.CodeBlockNode):
+            text = node.text
+            for key, delim in self.code_decoration_table.items():
+                text = text.replace(key, delim)
+            self.data += text
+        else:
+            text = tex_escape(node.text)
+            self.data += text
 
     def leave_text(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_other(self, node: nd.ASTNode) -> None:
         pass
 
     def leave_other(self, node: nd.ASTNode) -> None:
         pass
+
+
+def tex_escape(text: str) -> str:
+    text = text.replace('\\', '\\textbackslash ')
+    text = re.sub(r'([#%&{}$_])', r'\\\1', text)
+    trans: Dict[str, Union[int, str, None]] = {
+        '~': '{\\textasciitilde}',
+        '^': '{\\textasciicircum}',
+        '|': '{\\textbar}',
+        '<': '{\\textless}',
+        '>': '{\\textgreater}',
+        '-': '{\\phantom{}}-',
+    }
+    text = text.translate(str.maketrans(trans))
+    return text
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `thothglyph_doc-0.2.2/thothglyph/writer/latex.py` & `thothglyph_doc-0.2.3/thothglyph/writer/html.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,49 @@
-# sudo apt install texlive-luatex texlive-fonts-recommended texlive-fonts-extra texlive-lang-cjk
 from __future__ import annotations
-from typing import Dict, Optional, Tuple, Union
+from typing import Dict, List, Optional
+import html
 import importlib
 import os
 import re
+import shutil
 import tempfile
-from PIL import Image
 from thothglyph.error import ThothglyphError
 from thothglyph.writer.writer import Writer
 from thothglyph.node import nd
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
-class LatexWriter(Writer):
-    target = 'latex'
-    ext = 'tex'
-
-    sectlevel_cmds: Dict[str, Tuple[str, ...]] = {
-        'article': ('section', 'subsection', 'paragraph', 'subparagraph'),
-        'report': ('chapter', 'section', 'subsection', 'paragraph', 'subparagraph'),
-        'book': ('chapter', 'section', 'subsection', 'paragraph', 'subparagraph'),
+class HtmlWriter(Writer):
+    target = 'html'
+    ext = 'html'
+
+    decoration_table: Dict[str, str] = {
+        'EMPHASIS': 'em',
+        'STRONG': 'strong',
+        'MARKED': 'u',
+        'STRIKE': 's',
+        'VAR': 'var',
+        'CODE': 'code',
+        'SUP': 'sup',
+        'SUB': 'sub',
     }
-    decoration_table: Dict[str, Tuple[str, str]] = {
-        'EMPHASIS': ('\\textit{', '}'),
-        'STRONG': ('\\textbf{', '}'),
-        'MARKED': ('\\uline{', '}'),
-        'STRIKE': ('\\sout{', '}'),
-        'VAR': ('\\varbox{', '}'),
-        'CODE': ('\\codebox{', '}'),
-        'SUP': ('\\textsuperscript{', '}'),
-        'SUB': ('\\textsubscript{', '}'),
-    }
-    code_decoration_table: Dict[str, Tuple[str, str]] = {
-        'EMPHASIS': '<?tg:I?>',
-        'STRONG': '<?tg:S?>',
-        'MARKED': '<?tg:U?>',
-        'STRIKE': '<?tg:SO?>',
-        'VAR': '<?tg:VAR?>',
-        'CODE': '',
-        'SUP': '',
-        'SUB': '',
-    }
-    bp_scale: float = 72.0 / 150.0
 
     def __init__(self):
         super().__init__()
         self.tmpdirname: Optional[str] = None
-        self.contentphase: str = 'before'  # before, main, after
+        self.imgdirname: str = 'img'
 
-    def parse(self, node) -> None:
+    def parse(self, node: nd.ASTNode) -> None:
         super().parse(node)
         template_dir = self.template_dir()
-        target = LatexWriter.target
+        target = self.target
         theme = self.theme()
-        template_path = os.path.join(template_dir, target, theme, 'document-ja.tex')
+        template_path = os.path.join(template_dir, target, theme, 'index.html')
         if not os.path.exists(template_path):
             raise ThothglyphError('template not found: {}'.format(template_path))
         with open(template_path, 'r', encoding=self.encoding) as f:
             template = f.read()
         t = template.replace('{', '{{').replace('}', '}}')
         t = re.sub(r'\$\{\{([^}]+)\}\}', r'{\1}', t)
         self.data = t.format(doc=self.template_docdata)
@@ -67,438 +51,424 @@
     def write(self, fpath: str, node: nd.ASTNode) -> None:
         clsname = self.__class__.__name__
         logger.info('{}: write document'.format(clsname))
         self.rootnode = node
         with tempfile.TemporaryDirectory() as tmpdirname:
             self.tmpdirname = tmpdirname
             self.parse(node)
-            with open(fpath, 'w', encoding=self.encoding) as f:
+            self._copy_template(fpath)
+            self._copy_resources(fpath)
+            fdir = os.path.abspath(fpath + '.dir')
+            indexpath = os.path.join(self.tmpdirname, 'index.html')
+            with open(indexpath, 'w', encoding=self.encoding) as f:
                 f.write(self.data)
+            os.makedirs(fdir, exist_ok=True)
+            shutil.copytree(self.tmpdirname, fdir, dirs_exist_ok=True)
         self.tmpdirname = None
 
-    def visit_document(self, node: nd.ASTNode) -> None:
-        self.data += '\\setcounter{page}{0}\n'
-        self.data += '\\pagenumbering{arabic}\\pagestyle{beforecontents}\n'
+    def _copy_template(self, fpath: str) -> None:
+        commondir = os.path.join(self.template_dir(), 'common')
+        if not os.path.exists(commondir):
+            commondir = os.path.join(self.pkg_template_dir(), 'common')
+        newcommondir = os.path.join(self.tmpdirname, 'template', 'common')
+        shutil.copytree(commondir, newcommondir, dirs_exist_ok=True)
+
+    def _copy_resources(self, fpath: str) -> None:
+        rscs: Dict[str, List[str]] = dict()
+        typetable: Dict[str, Dict[str, str]] = {
+            'img': {
+                'dir': os.path.join(self.tmpdirname, self.imgdirname),
+            },
+        }
+        for n, gofoward in self.rootnode.walk_depth():
+            if not gofoward:
+                continue
+            if isinstance(n, nd.ImageRoleNode):
+                tp = 'img'
+                path = os.path.abspath(n.value)
+            else:
+                continue
+            rscs.setdefault(tp, list())
+            if path not in rscs[tp]:
+                rscs[tp].append(path)
+        for tp, paths in rscs.items():
+            newrscdir = typetable[tp]['dir']
+            os.makedirs(newrscdir, exist_ok=True)
+            for rscpath in paths:
+                _, rscfname = os.path.split(rscpath)
+                shutil.copy2(rscpath, os.path.join(newrscdir, rscfname))
 
     def visit_section(self, node: nd.ASTNode) -> None:
-        level_offset = 0
+        self.data += '<section>'
         _id = node.id or node.title.replace(' ', '_')
-        title = tex_escape(node.title)
-        doctype = 'report'
-        level = min(node.level - 1, len(self.sectlevel_cmds[doctype]) - 1) + level_offset
-        cmd = self.sectlevel_cmds[doctype][level]
-        asterisk = ''
-        if node.opts.get('notoc') or node.opts.get('nonum'):
-            asterisk = '*'
-        if not node.opts.get('notoc') and node.level == 1 and self.contentphase == 'before':
-            self.data += '\\pagenumbering{arabic}\\pagestyle{fancy}\n'
-            self.contentphase = 'main'
-        self.data += '\\{}{}{{{}}}'.format(cmd, asterisk, title)
-        if not node.opts.get('notoc') and node.opts.get('nonum'):
-            self.data += '\\addcontentsline{{toc}}{{{}}}{{{}}}'.format(cmd, title)
-        self.data += '\\label{{{}}}\n'.format(_id)
+        if node.opts.get('nonum'):
+            title = node.title
+        else:
+            title = '{}. {}'.format(node.sectnum, node.title)
+        if node.opts.get('notoc'):
+            toc = 'class="notoc"'
+        else:
+            toc = ''
+        if node.level < 7:
+            tag = '<h{0} {3} id="{2}">{1}</h{0}>\n'
+            self.data += tag.format(node.level, title, _id, toc)
+        else:
+            tag = '<div class="section h{0}" id="{2}">{1}</div>\n'
+            self.data += tag.format(node.level, title, _id)
 
     def leave_section(self, node: nd.ASTNode) -> None:
-        pass
+        self.data += '</section>\n'
 
     def visit_tocblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\tableofcontents\n'
+        self.data += '<div>\n'
+        maxlevel = int(node.opts.get('level', '100'))
+        for n, gofoward in node.walk_sections():
+            if n.opts.get('notoc'):
+                continue
+            if gofoward and n.level <= maxlevel:
+                bros = [s for s in n.parent.children if isinstance(n, nd.SectionNode)]
+                if bros.index(n) == 0:
+                    self.data += '<ul>\n'
+                if n.opts.get('nonum'):
+                    title = '{}'.format(n.title)
+                else:
+                    title = '{}. {}'.format(n.sectnum, n.title)
+                _id = n.id or n.title.replace(' ', '_')
+                self.data += '<li><a href="#{}">{}</a></li>\n'.format(_id, title)
+                if bros.index(n) == len(bros) - 1:
+                    self.data += '</ul>\n'
+        self.data += '</div>\n'
 
     def leave_tocblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\clearpage\\setcounter{page}{0}\n'
+        pass
 
     def visit_bulletlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\begin{itemize}\n'
+        self.data += '<ul>\n'
 
     def leave_bulletlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\end{itemize}\n'
+        self.data += '</ul>\n'
 
     def visit_orderedlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\begin{enumerate}\n'
+        self.data += '<ol>\n'
 
     def leave_orderedlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\end{enumerate}\n'
+        self.data += '</ol>\n'
 
     def visit_descriptionlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\begin{description}\n'
+        if not node.titlebreak:
+            self.data += '<dl class="compactdl">\n'
+        else:
+            self.data += '<dl>\n'
 
     def leave_descriptionlistblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\end{description}\n'
+        self.data += '</dl>\n'
 
     def visit_checklistblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\begin{tgchecklist}\n'
+        self.data += '<ul class="checklist">\n'
 
     def leave_checklistblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\end{tgchecklist}\n'
+        self.data += '</ul>\n'
 
     def visit_footnotelistblock(self, node: nd.ASTNode) -> None:
-        self._continue()
+        self.data += '<ul class="footnotelist">'
 
     def leave_footnotelistblock(self, node: nd.ASTNode) -> None:
-        pass
+        self.data += '</ul>'
 
     def visit_referencelistblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\begin{thebibliography}{{99}}\n'
+        self.data += '<ul class="referencelist">'
 
     def leave_referencelistblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\end{thebibliography}\n'
+        self.data += '</ul>'
 
     def visit_listitem(self, node: nd.ASTNode) -> None:
         if isinstance(node.parent, nd.DescriptionListBlockNode):
             pass
         elif isinstance(node.parent, nd.CheckListBlockNode):
             if node.marker == 'x':
-                self.data += '\\item[{\\tgcheck[en]}] '
+                liclass = 'check_en'
             elif node.marker == '-':
-                self.data += '\\item[{\\tgcheck[im]}] '
+                liclass = 'check_im'
             else:
-                self.data += '\\item[{\\tgcheck[dis]}] '
+                liclass = 'check_dis'
+            self.data += '<li class="checklist {}">'.format(liclass)
         elif isinstance(node.parent, nd.FootnoteListBlockNode):
-            pass  # unreach
+            url = 'fn.{}-{}'.format(node.treeindex()[1], node.fn_num)
+            text = node.fn_num  # node.title
+            self.data += '<li> '
+            self.data += '<span id="{}">{}</span>. '.format(url, text)
         elif isinstance(node.parent, nd.ReferenceListBlockNode):
             url = 'ref.{}'.format(node.ref_num)
-            self.data += '\\bibitem{{{}}} '.format(url)
+            text = node.ref_num  # node.title
+            self.data += '<li> '
+            self.data += '[<span id="{}">{}</span>] '.format(url, text)
+            # self.data += '<li id="{}">[{}] '.format(url, text)
         else:
-            self.data += '\\item '
+            self.data += '<li>'
 
     def leave_listitem(self, node: nd.ASTNode) -> None:
-        if isinstance(node.parent, nd.FootnoteListBlockNode):
-            pass  # unreach
-        elif isinstance(node.parent, nd.ReferenceListBlockNode):
-            self.data += '\n'
+        if isinstance(node.parent, nd.DescriptionListBlockNode):
+            self.data += '</dd>\n'
+            if not node.parent.titlebreak:
+                self.data += '</div>'
+        else:
+            self.data += '</li>\n'
 
     def visit_quoteblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\begin{quote}\n'
+        self.data += '<blockquote>'
 
     def leave_quoteblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\end{quote}\n'
+        self.data += '</blockquote>'
 
     def visit_codeblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\begin{lstlisting}'
-        if node.lang:
-            self.data += '[style={}]'.format(node.lang)
-        self.data += '\n'
+        self.data += '<pre><code>'
 
     def leave_codeblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\end{lstlisting}\n'
+        self.data += '</code></pre>\n'
 
     def visit_figureblock(self, node: nd.ASTNode) -> None:
-        align = node.align
-        table_align_cmd = {
-            'l': 'raggedright',
-            'c': 'centering',
-            'r': 'raggedleft',
-        }
-        self.data += '\\begin{figure}[H]\n'
-        self.data += '\\{}\n'.format(table_align_cmd[align])
-        opts = 'singlelinecheck=false,justification={}'
-        opts = opts.format(table_align_cmd[align])
-        self.data += '\\captionsetup{{{}}}\n'.format(opts)
+        if node.align == 'l':
+            style = 'style="text-align:left;"'
+        elif node.align == 'c':
+            style = 'style="text-align:center;"'
+        elif node.align == 'r':
+            style = 'style="text-align:right;"'
         if isinstance(node.children[0], nd.TableBlockNode):
-            self.data += '\\captionof{{table}}{{{}}}\n'.format(node.caption)
+            self.data += '<figure {}>\n'.format(style)
+            self.data += '<figcaption>'
+            self.data += '{} {}'.format(node.fignum, node.caption)
+            self.data += '</figcaption>\n'
         else:
-            self.data += '\\captionof{{figure}}{{{}}}\n'.format(node.caption)
+            self.data += '<figure {}>\n'.format(style)
 
     def leave_figureblock(self, node: nd.ASTNode) -> None:
-        self.data += '\\end{figure}\n'
-
-    style_gridtable = True
+        if isinstance(node.children[0], nd.TableBlockNode):
+            self.data += '</figure>\n'
+        else:
+            self.data += '<figcaption>'
+            self.data += '{} {}'.format(node.fignum, node.caption)
+            self.data += '</figcaption>\n'
+            self.data += '</figure>\n'
 
     def visit_tableblock(self, node: nd.ASTNode) -> None:
         align = node.align
         if isinstance(node.parent, nd.FigureBlockNode):
             align = node.parent.align
-        table_align_cmd = {
-            'l': 'raggedright',
-            'c': 'centering',
-            'r': 'raggedleft',
-        }
-        aligns = node.aligns[:]
-        for i, a in enumerate(aligns):
-            if a == 'x':
-                aligns[i] = 'X[l]'
-            else:
-                aligns[i] = a
-        if self.style_gridtable:
-            col_aligns = '|{}|'.format('|'.join(aligns))
-        else:
-            col_aligns = '{}'.format(' '.join(aligns))
-        if not node._parent_table():
-            self.data += '\\{}'.format(table_align_cmd[align])
-            if node.type == 'long':
-                self.data += '\\begin{longtblr}\n'
-            # elif isinstance(node.parent, nd.FigureBlockNode):
-            #     self.data += '\\begin{talltblr}\n'
-            else:
-                self.data += '\\begin{tblr}\n'
-            self.data += '['
-            self.data += 'entry=none, label=none,'
-            self.data += ']\n'
-        else:
-            self.data += '\\begin{tblr}\n'
-        self.data += '{'
-        self.data += 'colspec = {{{}}}, '.format(col_aligns)
-        self.data += 'hlines, vlines, '
-        self.data += 'measure = vbox, '
-        self.data += '}\n'
+        styles = []
+        style = ''
+        if align == 'l':
+            styles += ['margin-right:auto']
+        elif align == 'c':
+            styles += ['margin-left:auto;margin-right:auto']
+        elif align == 'r':
+            styles += ['margin-left:auto']
+        if node.width:
+            styles += ['width:{}'.format(node.width)]
+        if len(styles) > 0:
+            style = 'style="{}"'.format(';'.join(styles))
+        self.data += '<table {}>\n'.format(style)
+        self._normalize_table_widths(node)
+
+    def _normalize_table_widths(self, node: nd.ASTNode) -> None:
+        sum_widths = sum([int(v) for v in node.widths if int(v) > 0])
+        if sum_widths > 0:
+            for row in node.children:
+                for cell in row.children:
+                    if int(cell.width) <= 0:
+                        continue
+                    cell.width = int(int(cell.width) / sum_widths * 100)
 
     def leave_tableblock(self, node: nd.ASTNode) -> None:
-        if not node._parent_table():
-            if node.type == 'long':
-                self.data += '\\end{longtblr}\n\n'
-            # elif isinstance(node.parent, nd.FigureBlockNode):
-            #     self.data += '\\end{talltblr}\n\n'
-            else:
-                self.data += '\\end{tblr}\n\n'
-        else:
-            self.data += '\\end{tblr}\n\n'
-
-        fns = list()
-        for n, gofoward in node.walk_depth():
-            if not gofoward:
-                continue
-            if isinstance(n, nd.FootnoteNode):
-                fns.append(n)
-        for i, fn in enumerate(fns):
-            self.data += '\\footnotetext[{}]{{\n'.format(fn.fn_num)
-            for n in fn.description.children:
-                Writer.parse(self, n)
-            self.data += '}\n'
+        self.data += '</table>\n'
 
     def visit_tablerow(self, node: nd.ASTNode) -> None:
-        if node.idx > 0:
-            self.data += ' \\\\\n'
-        # if node.tp == 'header':
-        #     self.data += '\\tgthrowcolor\n'
-        # else:
-        #     self.data += '\\tgtdrowcolor\n'
+        self.data += '<tr>\n'
 
     def leave_tablerow(self, node: nd.ASTNode) -> None:
-        if node.idx == len(node.parent.children) - 1:
-            self.data += ' \\\\\n'
+        self.data += '</tr>\n'
 
     def visit_tablecell(self, node: nd.ASTNode) -> None:
-        if self.style_gridtable:
-            align = '{}|'.format(node.align)
-        else:
-            align = '{}'.format(node.align)
+        tagname = 'td'
+        if node.parent.tp == 'header':
+            tagname = 'th'
         if node.mergeto is None:
-            if node.idx != 0:
-                self.data += ' & '
             s = node.size
-            if s.x > 1:
-                self.data += '\\multicolumn{{{}}}{{{}}}{{'.format(s.x, align)
-            if s.y > 1:
-                self.data += '\\multirow{{{}}}{{*}}{{'.format(s.y)
-            self.data += '\n{\\begin{varwidth}{\\linewidth}\n'
-        elif node.mergeto.idx == node.idx and node.mergeto.parent.idx != node.parent.idx:
-            # horizontal cell merging
-            if node.idx != 0:
-                self.data += ' & '
-            s = node.mergeto.size
-            if s.x > 1:
-                self.data += '\\multicolumn{{{}}}{{{}}}{{'.format(s.x, align)
+            align = {'l': 'left', 'c': 'center', 'r': 'right', 'x': 'left'}
+            styles = ['text-align:{}'.format(align[node.align])]
+            if int(node.width) > 0:
+                styles += ['width:{}%'.format(node.width)]
+            attrs = ['style="{}"'.format(';'.join(styles))]
+            attrs += ['colspan="{}"'.format(s.x), 'rowspan="{}"'.format(s.y)]
+            self.data += '<{} {}>'.format(tagname, ' '.join(attrs))
         else:
-            # vertical cell merging
-            pass
+            self._continue()
 
     def leave_tablecell(self, node: nd.ASTNode) -> None:
+        tagname = 'td'
+        if node.parent.tp == 'header':
+            tagname = 'th'
         if node.mergeto is None:
-            self.data += '\n\\end{varwidth}}\n'
-            s = node.size
-            if s.x > 1:
-                self.data += '}'
-            if s.y > 1:
-                self.data += '}'
-        elif node.mergeto.idx == node.idx and node.mergeto.parent.idx != node.parent.idx:
-            s = node.mergeto.size
-            if s.x > 1:
-                self.data += '}'
+            self.data += '</{}>'.format(tagname)
+        else:
+            pass
 
     def visit_customblock(self, node: nd.ASTNode) -> None:
         if node.ext == '':
-            self.data += '\\begin{lstlisting}\n'
-            self.data += node.text + '\n'
-            self.data += '\\end{lstlisting}\n'
+            self.data += '<pre><code>'
+            self.data += html.escape(node.text) + '\n'
+            self.data += '</code></pre>\n'
         else:
             try:
                 extpath = 'thothglyph.ext.{}'.format(node.ext)
                 extmodule = importlib.import_module(extpath)
-                extmodule.customblock_write_latex(self, node)
+                extmodule.customblock_write_html(self, node)
             except Exception:
-                self.data += '\\begin{lstlisting}\n'
-                self.data += node.text + '\n'
-                self.data += '\\end{lstlisting}\n'
+                self.data += '<pre><code>'
+                self.data += html.escape(node.text) + '\n'
+                self.data += '</code></pre>\n'
 
     def leave_customblock(self, node: nd.ASTNode) -> None:
         pass
 
-    def visit_paragraph(self, node: nd.ASTNode) -> None:
+    def visit_horizonblock(self, node: nd.ASTNode) -> None:
+        self.data += '<hr />'
+
+    def leave_horizonblock(self, node: nd.ASTNode) -> None:
         pass
 
+    def visit_paragraph(self, node: nd.ASTNode) -> None:
+        if not all([
+            isinstance(node.parent, nd.ListItemNode),
+            len(node.parent.children) == 1
+        ]):
+            self.data += '<p>'
+
     def leave_paragraph(self, node: nd.ASTNode) -> None:
-        self.data += '\n\n'
+        if not all([
+            isinstance(node.parent, nd.ListItemNode),
+            len(node.parent.children) == 1
+        ]):
+            self.data += '</p>\n'
 
     def visit_title(self, node: nd.ASTNode) -> None:
         if isinstance(node.parent, nd.ListItemNode):
-            self.data += '\\item[\\desctitle{'
+            if not node.parent.parent.titlebreak:
+                self.data += '<div>'
+            self.data += '<dt>'
 
     def leave_title(self, node: nd.ASTNode) -> None:
         if isinstance(node.parent, nd.ListItemNode):
-            self.data += '}] '
-            if node.parent.titlebreak:
-                self.data += '\\mbox{}\\\\ '
+            self.data += '</dt><dd>'
 
     def visit_decorationrole(self, node: nd.ASTNode) -> None:
-        if isinstance(node.parent_block, nd.CodeBlockNode):
-            self.data += self.code_decoration_table[node.role]
-        else:
-            self.data += self.decoration_table[node.role][0]
+        self.data += '<{}>'.format(self.decoration_table[node.role])
 
     def leave_decorationrole(self, node: nd.ASTNode) -> None:
-        if isinstance(node.parent_block, nd.CodeBlockNode):
-            self.data += self.code_decoration_table[node.role]
-        else:
-            self.data += self.decoration_table[node.role][1]
+        self.data += '</{}>'.format(self.decoration_table[node.role])
 
     def visit_role(self, node: nd.ASTNode) -> None:
         if node.role == '':
-            self.data += '\\fbox{\\lstinline{'
-            self.data += node.value
-            self.data += '}}\n'
+            self.data += '<code>'
+            self.data += html.escape(node.value)
+            self.data += '</code>\n'
         else:
             try:
                 extpath = 'thothglyph.ext.{}'.format(node.role)
                 extmodule = importlib.import_module(extpath)
-                extmodule.role_write_latex(self, node)
+                extmodule.role_write_html(self, node)
             except Exception:
-                self.data += '\\fbox{\\lstinline{'
-                self.data += node.value
-                self.data += '}}\n'
+                self.data += '<code>'
+                self.data += html.escape(node.value)
+                self.data += '</code>\n'
 
     def leave_role(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_imagerole(self, node: nd.ASTNode) -> None:
-        fname, ext = os.path.splitext(node.value)
-        if ext == '.svg':
-            assert self.tmpdirname
-            imgpath = os.path.join(self.tmpdirname, node.value)
-            inc_imgpath = '{}.pdf'.format(imgpath)
-        else:
-            imgpath = node.value
-            inc_imgpath = imgpath
+        options = dict()
         if 'w' in node.opts:
-            w = node.opts['w']
-            if w.endswith('px'):
-                w = '{}bp'.format(int(float(w[0:-2]) * self.bp_scale))
-            elif w.endswith('%'):
-                w = '{}\\linewidth'.format(float(w[0:-1]) * 0.01)
+            options['width'] = node.opts['w']
+        optstr = ' '.join(['{}="{}"'.format(k, v) for k, v in options.items()])
+        fname = os.path.basename(node.value)
+        _, ext = os.path.splitext(fname)
+        imgpath = os.path.join(self.imgdirname, fname)
+        if ext.lower() == '.svg':
+            src = 'type="image/svg+xml" data="{}"'.format(imgpath)
+            self.data += '<object {} {}></object>'.format(src, optstr)
         else:
-            try:
-                with Image.open(node.value) as img:
-                    w = '{}bp'.format(img.width)
-            except Exception:
-                w = '\\linewidth'
-        self.data += '\\tgincludegraphics[{}]{{{}}}'.format(w, inc_imgpath)
+            src = 'src="{}"'.format(imgpath)
+            self.data += '<image {} {} />'.format(src, optstr)
 
     def leave_imagerole(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_kbdrole(self, node: nd.ASTNode) -> None:
-        value = ['\\kbdbox{{{}}}'.format(v) for v in node.value]
-        valuestr = ' {\\scriptsize+} '.join(value)
-        self.data += valuestr
+        texts = [html.escape(t) for t in node.value]
+        value = ' + '.join(['<kbd>{}</kbd>'.format(v) for v in texts])
+        self.data += value
 
     def leave_kbdrole(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_btnrole(self, node: nd.ASTNode) -> None:
-        value = '\\btnbox{{{}}}'.format(node.value)
+        value = '<kbd>{}</kbd>'.format(html.escape(node.value))
         self.data += value
 
     def leave_btnrole(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_menurole(self, node: nd.ASTNode) -> None:
-        value = ['\\menubox{{{}}}'.format(v) for v in node.value]
-        valuestr = ' {\\tiny>} '.join(value)
-        self.data += valuestr
+        texts = [html.escape(t) for t in node.value]
+        value = ' > '.join(['<span class="menu">{}</span>'.format(v) for v in texts])
+        self.data += value
 
     def leave_menurole(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_link(self, node: nd.ASTNode) -> None:
         if '://' in node.value:
+            blank = 'target=”_blank”'
             url = node.value
             text = node.opts[0] if node.opts[0] else node.value
-            text = tex_escape(text)
-            self.data += '\\href{{{}}}{{{}}}'.format(url, text)
         else:
-            url = node.target_id or node.value.replace(' ', '_')
+            blank = ''
+            url = '#' + node.target_id
             text = node.opts[0] if node.opts[0] else node.target_title
-            text = tex_escape(text)
-            self.data += '\\nameref{{{}}}'.format(url)
+        text = html.escape(text)
+        self.data += '<a href="{}" {}>{}</a>'.format(url, blank, text)
 
     def leave_link(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_footnote(self, node: nd.ASTNode) -> None:
-        table = node._parent_table()
-        if table:
-            self.data += ' \\footnotemark[{}] '.format(node.fn_num)
-        else:
-            url = node.fn_num
-            self.data += '\\footnote[{}]{{'.format(url)
-            for n in node.description.children:
-                Writer.parse(self, n)
-            self.data += '}'
+        url = '#fn.{}-{}'.format(node.treeindex()[1], node.fn_num)
+        text = node.fn_num  # node.value
+        self.data += '<sup><a href="{}">{}</a></sup>'.format(url, text)
 
     def leave_footnote(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_reference(self, node: nd.ASTNode) -> None:
-        url = 'ref.{}'.format(node.ref_num)
-        self.data += '\\cite{{{}}}'.format(url)
+        url = '#ref.{}'.format(node.ref_num)
+        text = node.ref_num  # node.value
+        self.data += '[<a href="{}">{}</a>]'.format(url, text)
 
     def leave_reference(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_linebreak(self, node: nd.ASTNode) -> None:
-        self.data += '{\\newline}'
+        self.data += '<br />'
 
     def leave_linebreak(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_text(self, node: nd.ASTNode) -> None:
-        if isinstance(node.parent_block, nd.CodeBlockNode):
-            text = node.text
-            for key, delim in self.code_decoration_table.items():
-                text = text.replace(key, delim)
-            self.data += text
-        else:
-            text = tex_escape(node.text)
-            self.data += text
+        self.data += node.text
 
     def leave_text(self, node: nd.ASTNode) -> None:
         pass
 
     def visit_other(self, node: nd.ASTNode) -> None:
         pass
 
     def leave_other(self, node: nd.ASTNode) -> None:
         pass
-
-
-def tex_escape(text: str) -> str:
-    text = text.replace('\\', '\\textbackslash ')
-    text = re.sub(r'([#%&{}$_])', r'\\\1', text)
-    trans: Dict[str, Union[int, str, None]] = {
-        '~': '{\\textasciitilde}',
-        '^': '{\\textasciicircum}',
-        '|': '{\\textbar}',
-        '<': '{\\textless}',
-        '>': '{\\textgreater}',
-        '-': '{\\phantom{}}-',
-    }
-    text = text.translate(str.maketrans(trans))
-    return text
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `thothglyph_doc-0.2.2/thothglyph/writer/pdf.py` & `thothglyph_doc-0.2.3/thothglyph/writer/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from typing import Optional
 import importlib
 import os
 import subprocess
 import tempfile
-import cairosvg
 from thothglyph.error import ThothglyphError
+from thothglyph.util.svg import svg2pdf
 from thothglyph.writer.latex import LatexWriter
 from thothglyph.node import nd
 from thothglyph.node import logging
 
 logger = logging.getLogger(__file__)
 
 
@@ -106,13 +106,13 @@
 
     def visit_imagerole(self, node: nd.ASTNode) -> None:
         super().visit_imagerole(node)
         fname, ext = os.path.splitext(node.value)
         if ext == '.svg':
             assert self.tmpdirname
             imgpath = os.path.join(self.tmpdirname, node.value)
-            cairosvg.svg2pdf(url=node.value, write_to='{}.pdf'.format(imgpath))
+            svg2pdf(url=node.value, write_to=imgpath)
         else:
             pass
 
     def leave_imagerole(self, node: nd.ASTNode) -> None:
         pass
```

### Comparing `thothglyph_doc-0.2.2/thothglyph/writer/writer.py` & `thothglyph_doc-0.2.3/thothglyph/writer/writer.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.2/PKG-INFO` & `thothglyph_doc-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thothglyph-doc
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Documentation converter and language for Engineers
 License: MIT
 Author: nakandev
 Author-email: nakandev.s@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -48,16 +48,20 @@
 
 \+ extensions
 
 ```
 # graphviz
 sudo apt install graphviz
 pip install graphviz
+# plantuml
+sudo apt install plantuml
 # blockdiag
 pip install blockdiag actdiag seqdiag nwdiag
+# mermaid
+npm install -g @mermaid-js/mermaid-cli
 # wavedrom
 pip install wavedrom
 ```
 
 ## Usage
 
 ```sh
```

