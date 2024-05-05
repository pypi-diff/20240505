# Comparing `tmp/mpl_bsic-1.3.1.tar.gz` & `tmp/mpl_bsic-1.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_bsic-1.3.1.tar", max compression
+gzip compressed data, was "mpl_bsic-1.4.0a0.tar", max compression
```

## Comparing `mpl_bsic-1.3.1.tar` & `mpl_bsic-1.4.0a0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0     1095 2023-11-28 19:36:34.844975 mpl_bsic-1.3.1/LICENSE.md
--rw-r--r--   0        0        0      450 2024-02-24 18:34:47.477627 mpl_bsic-1.3.1/mpl_bsic/__init__.py
--rw-r--r--   0        0        0     6027 2023-11-30 23:26:30.040933 mpl_bsic-1.3.1/mpl_bsic/apply_bsic_logo.py
--rw-r--r--   0        0        0     7714 2024-02-24 18:34:47.479127 mpl_bsic-1.3.1/mpl_bsic/apply_bsic_style.py
--rw-r--r--   0        0        0     4882 2023-11-30 23:26:30.042432 mpl_bsic-1.3.1/mpl_bsic/check_figsize.py
--rw-r--r--   0        0        0     1272 2024-02-24 18:34:47.480126 mpl_bsic-1.3.1/mpl_bsic/export_figure.py
--rw-r--r--   0        0        0   198072 2023-12-01 10:47:04.227181 mpl_bsic-1.3.1/mpl_bsic/fonts/garamond/Garamond.TTF
--rw-r--r--   0        0        0   199772 2023-12-01 10:47:04.235181 mpl_bsic-1.3.1/mpl_bsic/fonts/garamond/Garamond_Bold.TTF
--rw-r--r--   0        0        0   189464 2023-12-01 10:47:04.247681 mpl_bsic-1.3.1/mpl_bsic/fonts/garamond/Garamond_Italic.TTF
--rw-r--r--   0        0        0    60160 2023-12-01 10:47:04.249182 mpl_bsic-1.3.1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Base.ttf
--rw-r--r--   0        0        0    68304 2023-12-01 10:47:04.250181 mpl_bsic-1.3.1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Bold.TTF
--rw-r--r--   0        0        0    71496 2023-12-01 10:47:04.251683 mpl_bsic-1.3.1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_BoldItalic.TTF
--rw-r--r--   0        0        0    69436 2023-12-01 10:47:04.252681 mpl_bsic-1.3.1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Italic.TTF
--rw-r--r--   0        0        0     1966 2023-11-30 16:41:49.328724 mpl_bsic-1.3.1/mpl_bsic/format_timeseries_axis.py
--rw-r--r--   0        0        0    10489 2023-12-01 00:50:58.631581 mpl_bsic-1.3.1/mpl_bsic/plot_trade.py
--rw-r--r--   0        0        0      779 2023-11-14 09:45:21.027794 mpl_bsic-1.3.1/mpl_bsic/preprocess_dataframe.py
--rw-r--r--   0        0        0   282980 2023-11-30 11:27:50.191357 mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_formal_1x.png
--rw-r--r--   0        0        0   921240 2023-11-30 11:27:50.197859 mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_formal_2x.png
--rw-r--r--   0        0        0  1910183 2023-11-30 11:27:50.209859 mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_formal_3x.png
--rw-r--r--   0        0        0   164720 2023-11-30 11:27:50.211358 mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_square_1x.png
--rw-r--r--   0        0        0   576512 2023-11-30 11:27:50.215358 mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_square_2x.png
--rw-r--r--   0        0        0  1208390 2023-11-30 11:27:50.223357 mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_square_3x.png
--rw-r--r--   0        0        0    10342 2024-02-24 18:34:47.481627 mpl_bsic-1.3.1/mpl_bsic/style_excel.py
--rw-r--r--   0        0        0      803 2024-04-22 23:29:32.971163 mpl_bsic-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4320 2023-12-01 14:37:36.997369 mpl_bsic-1.3.1/README.md
--rw-r--r--   0        0        0        0 2023-11-30 22:39:19.895120 mpl_bsic-1.3.1/utils/__init__.py
--rw-r--r--   0        0        0     1473 2023-12-01 10:47:04.254182 mpl_bsic-1.3.1/utils/add_fonts.py
--rw-r--r--   0        0        0      529 2023-11-30 23:26:30.044933 mpl_bsic-1.3.1/utils/run_animations.py
--rw-r--r--   0        0        0      414 2023-11-30 14:02:43.673722 mpl_bsic-1.3.1/utils/set_animations.py
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 mpl_bsic-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-11-28 19:36:34.844975 mpl_bsic-1.4.0a0/LICENSE.md
+-rw-r--r--   0        0        0      500 2024-05-05 00:44:11.361389 mpl_bsic-1.4.0a0/mpl_bsic/__init__.py
+-rw-r--r--   0        0        0     4670 2024-05-05 00:44:11.362885 mpl_bsic-1.4.0a0/mpl_bsic/add_title_subtitle.py
+-rw-r--r--   0        0        0     6019 2024-05-05 00:44:11.363885 mpl_bsic-1.4.0a0/mpl_bsic/apply_bsic_logo.py
+-rw-r--r--   0        0        0     8429 2024-05-05 00:44:11.365385 mpl_bsic-1.4.0a0/mpl_bsic/apply_bsic_style.py
+-rw-r--r--   0        0        0     4882 2023-11-30 23:26:30.042432 mpl_bsic-1.4.0a0/mpl_bsic/check_figsize.py
+-rw-r--r--   0        0        0     1823 2024-05-05 00:44:11.366887 mpl_bsic-1.4.0a0/mpl_bsic/constants.py
+-rw-r--r--   0        0        0     1457 2024-05-05 00:44:11.368385 mpl_bsic-1.4.0a0/mpl_bsic/export_figure.py
+-rw-r--r--   0        0        0   198072 2023-12-01 10:47:04.227181 mpl_bsic-1.4.0a0/mpl_bsic/fonts/garamond/Garamond.TTF
+-rw-r--r--   0        0        0   199772 2023-12-01 10:47:04.235181 mpl_bsic-1.4.0a0/mpl_bsic/fonts/garamond/Garamond_Bold.TTF
+-rw-r--r--   0        0        0   189464 2023-12-01 10:47:04.247681 mpl_bsic-1.4.0a0/mpl_bsic/fonts/garamond/Garamond_Italic.TTF
+-rw-r--r--   0        0        0    60160 2023-12-01 10:47:04.249182 mpl_bsic-1.4.0a0/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Base.ttf
+-rw-r--r--   0        0        0    68304 2023-12-01 10:47:04.250181 mpl_bsic-1.4.0a0/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Bold.TTF
+-rw-r--r--   0        0        0    71496 2023-12-01 10:47:04.251683 mpl_bsic-1.4.0a0/mpl_bsic/fonts/gill_sans_mt/GillSansMT_BoldItalic.TTF
+-rw-r--r--   0        0        0    69436 2023-12-01 10:47:04.252681 mpl_bsic-1.4.0a0/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Italic.TTF
+-rw-r--r--   0        0        0     1966 2023-11-30 16:41:49.328724 mpl_bsic-1.4.0a0/mpl_bsic/format_timeseries_axis.py
+-rw-r--r--   0        0        0    10489 2023-12-01 00:50:58.631581 mpl_bsic-1.4.0a0/mpl_bsic/plot_trade.py
+-rw-r--r--   0        0        0      779 2023-11-14 09:45:21.027794 mpl_bsic-1.4.0a0/mpl_bsic/preprocess_dataframe.py
+-rw-r--r--   0        0        0   282980 2023-11-30 11:27:50.191357 mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_formal_1x.png
+-rw-r--r--   0        0        0   921240 2023-11-30 11:27:50.197859 mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_formal_2x.png
+-rw-r--r--   0        0        0  1910183 2023-11-30 11:27:50.209859 mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_formal_3x.png
+-rw-r--r--   0        0        0   164720 2023-11-30 11:27:50.211358 mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_square_1x.png
+-rw-r--r--   0        0        0   576512 2023-11-30 11:27:50.215358 mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_square_2x.png
+-rw-r--r--   0        0        0  1208390 2023-11-30 11:27:50.223357 mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_square_3x.png
+-rw-r--r--   0        0        0    10342 2024-02-24 18:34:47.481627 mpl_bsic-1.4.0a0/mpl_bsic/style_excel.py
+-rw-r--r--   0        0        0     1022 2024-05-05 00:46:43.378385 mpl_bsic-1.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     4320 2023-12-01 14:37:36.997369 mpl_bsic-1.4.0a0/README.md
+-rw-r--r--   0        0        0        0 2023-11-30 22:39:19.895120 mpl_bsic-1.4.0a0/utils/__init__.py
+-rw-r--r--   0        0        0     1473 2023-12-01 10:47:04.254182 mpl_bsic-1.4.0a0/utils/add_fonts.py
+-rw-r--r--   0        0        0      469 2024-05-05 00:44:11.374886 mpl_bsic-1.4.0a0/utils/logger.py
+-rw-r--r--   0        0        0      529 2023-11-30 23:26:30.044933 mpl_bsic-1.4.0a0/utils/run_animations.py
+-rw-r--r--   0        0        0      414 2023-11-30 14:02:43.673722 mpl_bsic-1.4.0a0/utils/set_animations.py
+-rw-r--r--   0        0        0     4848 1970-01-01 00:00:00.000000 mpl_bsic-1.4.0a0/PKG-INFO
```

### Comparing `mpl_bsic-1.3.1/LICENSE.md` & `mpl_bsic-1.4.0a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/apply_bsic_logo.py` & `mpl_bsic-1.4.0a0/mpl_bsic/apply_bsic_logo.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         import matplotlib.pyplot as plt
 
         x = np.linspace(0, 5, 100)
         y = np.cos(x)
 
         fig, ax = plt.subplots(1, 1)
         ax.set_title('Cos(x)') # set the title before applying the style
-        apply_bsic_style(fig, ax)
+        apply_bsic_style(fig)
         apply_bsic_logo(fig, ax, location='top right', scale=0.03)
 
         ax.plot(x,y)
         run_animations(fig) # only needed for the docs, don't call in the actual code
 
     .. plot::
         :alt: example plot using apply_bsic_logo() (btm left, square logo)
@@ -127,15 +127,15 @@
         import matplotlib.pyplot as plt
 
         x = np.linspace(0, 5, 100)
         y = np.cos(x)
 
         fig, ax = plt.subplots(1, 1)
         ax.set_title('Cos(x)') # set the title before applying the style
-        apply_bsic_style(fig, ax)
+        apply_bsic_style(fig)
         apply_bsic_logo(
             fig,
             ax,
             location='bottom left',
             scale=0.05,
             logo_type='square', # use the square logo
             closeness_to_border=25 # make the logo closer to the border
```

### Comparing `mpl_bsic-1.3.1/mpl_bsic/check_figsize.py` & `mpl_bsic-1.4.0a0/mpl_bsic/check_figsize.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/export_figure.py` & `mpl_bsic-1.4.0a0/mpl_bsic/export_figure.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from matplotlib.figure import Figure
 
 from utils.run_animations import run_animations
 
 
-def export_figure(fig: Figure, filename: str):
+def export_figure(fig: Figure, filename: str, transparent: bool = True):
     """
     Export a figure according to BSIC Standards.
 
     First, the function forces the animations to run,
     making sure that any style is applied before exporting.
     Additionally, exports the figure in ``svg`` format,
     with ``bbox_inches='tight'`` and ``dpi=1200``.
 
     Parameters
     ----------
     fig : Figure
         The ``matplotlib`` figure to export.
     filename : str
-        The filename that should be used when exporting.
+        The filename that should be used when exporting (including the extension).
+        Example: 'fig1.svg'
+    transparent: bool
+        Whether to transparent the figure when exporting.
+        Defaults to True.
 
     See Also
     --------
     mpl_bsic.apply_bsic_style :
         Applies the BSIC Style to plots.
 
     mpl_bsic.apply_bsic_logo :
@@ -42,8 +46,8 @@
         ax.set_title('Sin(x)')
 
         apply_bsic_style(fig, ax)
         export_figure(fig, 'output_filename')
     """
     run_animations(fig)
 
-    fig.savefig(filename + ".svg", dpi=1200, bbox_inches="tight")
+    fig.savefig(filename, dpi=1200, transparent=transparent)
```

### Comparing `mpl_bsic-1.3.1/mpl_bsic/fonts/garamond/Garamond.TTF` & `mpl_bsic-1.4.0a0/mpl_bsic/fonts/garamond/Garamond.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/fonts/garamond/Garamond_Bold.TTF` & `mpl_bsic-1.4.0a0/mpl_bsic/fonts/garamond/Garamond_Bold.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/fonts/garamond/Garamond_Italic.TTF` & `mpl_bsic-1.4.0a0/mpl_bsic/fonts/garamond/Garamond_Italic.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Base.ttf` & `mpl_bsic-1.4.0a0/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Base.ttf`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Bold.TTF` & `mpl_bsic-1.4.0a0/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Bold.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_BoldItalic.TTF` & `mpl_bsic-1.4.0a0/mpl_bsic/fonts/gill_sans_mt/GillSansMT_BoldItalic.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Italic.TTF` & `mpl_bsic-1.4.0a0/mpl_bsic/fonts/gill_sans_mt/GillSansMT_Italic.TTF`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/format_timeseries_axis.py` & `mpl_bsic-1.4.0a0/mpl_bsic/format_timeseries_axis.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/plot_trade.py` & `mpl_bsic-1.4.0a0/mpl_bsic/plot_trade.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/preprocess_dataframe.py` & `mpl_bsic-1.4.0a0/mpl_bsic/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_formal_1x.png` & `mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_formal_1x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_formal_2x.png` & `mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_formal_2x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_formal_3x.png` & `mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_formal_3x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_square_1x.png` & `mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_square_1x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_square_2x.png` & `mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_square_2x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/static/bsic_logo_square_3x.png` & `mpl_bsic-1.4.0a0/mpl_bsic/static/bsic_logo_square_3x.png`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/mpl_bsic/style_excel.py` & `mpl_bsic-1.4.0a0/mpl_bsic/style_excel.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/README.md` & `mpl_bsic-1.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/utils/add_fonts.py` & `mpl_bsic-1.4.0a0/utils/add_fonts.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/utils/run_animations.py` & `mpl_bsic-1.4.0a0/utils/run_animations.py`

 * *Files identical despite different names*

### Comparing `mpl_bsic-1.3.1/PKG-INFO` & `mpl_bsic-1.4.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_bsic
-Version: 1.3.1
+Version: 1.4.0a0
 Summary: BSIC Plotting Library
 Author: Andrea Franceschini
 Author-email: andrea.franceschini2@studbocconi.it
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mpl_bsic Version: 1.3.1 Summary: BSIC Plotting
+Metadata-Version: 2.1 Name: mpl_bsic Version: 1.4.0a0 Summary: BSIC Plotting
 Library Author: Andrea Franceschini Author-email:
 andrea.franceschini2@studbocconi.it Requires-Python: >=3.9 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: matplotlib (>=3.7,<4.0) Requires-Dist: numpy
 (>=1.25,<2.0) Requires-Dist: pandas (>=2,<3) Requires-Dist: xlsxwriter
```

