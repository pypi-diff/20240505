# Comparing `tmp/parseq-2023.5.0.zip` & `tmp/parseq-2024.5.0.zip`

## zipinfo {}

```diff
@@ -1,179 +1,202 @@
-Zip file size: 2245699 bytes, number of entries: 177
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/
--rw-rw-rw-  2.0 fat     1099 b- defN 20-Nov-24 00:11 parseq-2023.5.0/LICENSE
--rw-rw-rw-  2.0 fat     5037 b- defN 23-May-30 17:00 parseq-2023.5.0/PKG-INFO
--rw-rw-rw-  2.0 fat       42 b- defN 23-May-30 17:00 parseq-2023.5.0/setup.cfg
--rw-rw-rw-  2.0 fat     3613 b- defN 23-May-30 16:48 parseq-2023.5.0/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/core/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/fits/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/gui/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/third_party/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/utils/
--rw-rw-rw-  2.0 fat      386 b- defN 18-Nov-18 11:39 parseq-2023.5.0/parseq/CODERULES.txt
--rw-rw-rw-  2.0 fat     4202 b- defN 23-May-29 10:53 parseq-2023.5.0/parseq/description.py
--rw-rw-rw-  2.0 fat      137 b- defN 23-May-30 16:51 parseq-2023.5.0/parseq/version.py
--rw-rw-rw-  2.0 fat      753 b- defN 23-Apr-04 11:34 parseq-2023.5.0/parseq/__init__.py
--rw-rw-rw-  2.0 fat     7916 b- defN 23-Mar-30 17:09 parseq-2023.5.0/parseq/core/commons.py
--rw-rw-rw-  2.0 fat     2546 b- defN 23-May-08 15:31 parseq-2023.5.0/parseq/core/config.py
--rw-rw-rw-  2.0 fat     1251 b- defN 23-Feb-18 18:40 parseq-2023.5.0/parseq/core/logger.py
--rw-rw-rw-  2.0 fat    10207 b- defN 23-Feb-18 16:09 parseq-2023.5.0/parseq/core/nodes.py
--rw-rw-rw-  2.0 fat     9439 b- defN 23-May-10 23:46 parseq-2023.5.0/parseq/core/plotExport.py
--rw-rw-rw-  2.0 fat    15090 b- defN 23-May-10 16:47 parseq-2023.5.0/parseq/core/save_restore.py
--rw-rw-rw-  2.0 fat     1295 b- defN 23-May-08 16:03 parseq-2023.5.0/parseq/core/singletons.py
--rw-rw-rw-  2.0 fat    67284 b- defN 23-May-29 21:45 parseq-2023.5.0/parseq/core/spectra.py
--rw-rw-rw-  2.0 fat    28882 b- defN 23-May-30 16:09 parseq-2023.5.0/parseq/core/transforms.py
--rw-rw-rw-  2.0 fat     7290 b- defN 23-May-30 10:44 parseq-2023.5.0/parseq/core/__init__.py
--rw-rw-rw-  2.0 fat    23452 b- defN 23-May-30 16:02 parseq-2023.5.0/parseq/fits/basefit.py
--rw-rw-rw-  2.0 fat     6018 b- defN 23-May-30 14:50 parseq-2023.5.0/parseq/fits/functionfit.py
--rw-rw-rw-  2.0 fat    11104 b- defN 23-May-29 17:27 parseq-2023.5.0/parseq/fits/lcf.py
--rw-rw-rw-  2.0 fat       57 b- defN 23-May-30 16:39 parseq-2023.5.0/parseq/fits/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/gui/fits/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/gui/_images/
--rw-rw-rw-  2.0 fat    14810 b- defN 23-May-28 23:01 parseq-2023.5.0/parseq/gui/aboutDialog.py
--rw-rw-rw-  2.0 fat     9545 b- defN 22-Dec-16 16:01 parseq-2023.5.0/parseq/gui/calibrateEnergy.py
--rw-rw-rw-  2.0 fat    17918 b- defN 23-Mar-28 10:46 parseq-2023.5.0/parseq/gui/columnFormat.py
--rw-rw-rw-  2.0 fat     5605 b- defN 23-Mar-22 18:09 parseq-2023.5.0/parseq/gui/combineSpectra.py
--rw-rw-rw-  2.0 fat    18954 b- defN 23-Apr-13 12:04 parseq-2023.5.0/parseq/gui/dataRebin.py
--rw-rw-rw-  2.0 fat    50740 b- defN 23-May-23 19:59 parseq-2023.5.0/parseq/gui/dataTreeModelView.py
--rw-rw-rw-  2.0 fat     9343 b- defN 23-May-29 23:05 parseq-2023.5.0/parseq/gui/fileDialogs.py
--rw-rw-rw-  2.0 fat    64592 b- defN 23-May-08 23:37 parseq-2023.5.0/parseq/gui/fileTreeModelView.py
--rw-rw-rw-  2.0 fat    17817 b- defN 23-Apr-27 09:30 parseq-2023.5.0/parseq/gui/gcommons.py
--rw-rw-rw-  2.0 fat    33432 b- defN 23-May-17 13:32 parseq-2023.5.0/parseq/gui/mainWindow.py
--rw-rw-rw-  2.0 fat    53525 b- defN 23-May-30 11:39 parseq-2023.5.0/parseq/gui/nodeWidget.py
--rw-rw-rw-  2.0 fat     3663 b- defN 23-Jan-03 15:01 parseq-2023.5.0/parseq/gui/plot.py
--rw-rw-rw-  2.0 fat    25381 b- defN 23-Mar-15 15:16 parseq-2023.5.0/parseq/gui/plotOptions.py
--rw-rw-rw-  2.0 fat     9346 b- defN 23-Mar-01 12:11 parseq-2023.5.0/parseq/gui/propsOfData.py
--rw-rw-rw-  2.0 fat    36606 b- defN 23-May-08 20:39 parseq-2023.5.0/parseq/gui/propWidget.py
--rw-rw-rw-  2.0 fat    46720 b- defN 23-May-26 21:19 parseq-2023.5.0/parseq/gui/roi.py
--rw-rw-rw-  2.0 fat     1653 b- defN 23-May-08 15:59 parseq-2023.5.0/parseq/gui/tasker.py
--rw-rw-rw-  2.0 fat     4937 b- defN 22-Oct-14 12:12 parseq-2023.5.0/parseq/gui/undoredo.py
--rw-rw-rw-  2.0 fat     9804 b- defN 23-May-28 22:26 parseq-2023.5.0/parseq/gui/webWidget.py
--rw-rw-rw-  2.0 fat     7206 b- defN 23-May-30 11:59 parseq-2023.5.0/parseq/gui/__init__.py
--rw-rw-rw-  2.0 fat     4463 b- defN 23-May-30 16:08 parseq-2023.5.0/parseq/gui/fits/gbasefit.py
--rw-rw-rw-  2.0 fat    15986 b- defN 23-May-30 14:50 parseq-2023.5.0/parseq/gui/fits/gfunctionfit.py
--rw-rw-rw-  2.0 fat    19210 b- defN 23-May-29 17:26 parseq-2023.5.0/parseq/gui/fits/glcf.py
--rw-rw-rw-  2.0 fat       25 b- defN 23-May-30 16:42 parseq-2023.5.0/parseq/gui/fits/__init__.py
--rw-rw-rw-  2.0 fat     2255 b- defN 23-May-29 00:07 parseq-2023.5.0/parseq/gui/_images/icon-fit-32.png
--rw-rw-rw-  2.0 fat     4846 b- defN 23-May-29 00:06 parseq-2023.5.0/parseq/gui/_images/icon-fit-64.png
--rw-rw-rw-  2.0 fat     5831 b- defN 21-Apr-21 15:48 parseq-2023.5.0/parseq/gui/_images/icon-help.png
--rw-rw-rw-  2.0 fat     5473 b- defN 21-Apr-21 15:48 parseq-2023.5.0/parseq/gui/_images/icon-info.png
--rw-rw-rw-  2.0 fat     1340 b- defN 21-May-13 14:48 parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-32.png
--rw-rw-rw-  2.0 fat     2414 b- defN 22-Jun-02 12:07 parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-64.png
--rw-rw-rw-  2.0 fat     1244 b- defN 22-Jul-20 22:55 parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-32.png
--rw-rw-rw-  2.0 fat     2221 b- defN 22-Jul-20 22:55 parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-64.png
--rw-rw-rw-  2.0 fat      461 b- defN 21-May-13 14:39 parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-32.png
--rw-rw-rw-  2.0 fat      582 b- defN 22-Jun-02 12:09 parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-64.png
--rw-rw-rw-  2.0 fat      452 b- defN 22-Jul-20 22:56 parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-busy-32.png
--rw-rw-rw-  2.0 fat      557 b- defN 22-Jul-20 22:56 parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-busy-64.png
--rw-rw-rw-  2.0 fat     1441 b- defN 21-May-13 14:39 parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-32.png
--rw-rw-rw-  2.0 fat     2834 b- defN 22-Jun-02 12:10 parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-64.png
--rw-rw-rw-  2.0 fat     1347 b- defN 22-Jul-20 22:57 parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-32.png
--rw-rw-rw-  2.0 fat     2673 b- defN 22-Jul-20 22:57 parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-64.png
--rw-rw-rw-  2.0 fat     2164 b- defN 22-Jul-21 12:50 parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-32.png
--rw-rw-rw-  2.0 fat     4780 b- defN 22-Jul-21 12:50 parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-64.png
--rw-rw-rw-  2.0 fat     2005 b- defN 22-Jul-21 12:50 parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-32.png
--rw-rw-rw-  2.0 fat     4515 b- defN 22-Jul-21 12:51 parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-64.png
--rw-rw-rw-  2.0 fat     5529 b- defN 21-Apr-22 22:43 parseq-2023.5.0/parseq/gui/_images/icon-load-proj.png
--rw-rw-rw-  2.0 fat     3575 b- defN 21-Apr-21 15:56 parseq-2023.5.0/parseq/gui/_images/icon-redo.png
--rw-rw-rw-  2.0 fat     5462 b- defN 21-Apr-22 22:44 parseq-2023.5.0/parseq/gui/_images/icon-save-proj.png
--rw-rw-rw-  2.0 fat     4662 b- defN 21-Apr-22 22:44 parseq-2023.5.0/parseq/gui/_images/icon-save-text.png
--rw-rw-rw-  2.0 fat     3625 b- defN 21-Apr-21 15:56 parseq-2023.5.0/parseq/gui/_images/icon-undo.png
--rw-rw-rw-  2.0 fat    67646 b- defN 17-Aug-08 13:54 parseq-2023.5.0/parseq/gui/_images/parseq.ico
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/exts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_images/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_static/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_templates/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_themes/
--rw-rw-rw-  2.0 fat     7052 b- defN 23-Mar-10 09:23 parseq-2023.5.0/parseq/help/conf.py
--rw-rw-rw-  2.0 fat     3547 b- defN 22-Sep-30 12:10 parseq-2023.5.0/parseq/help/conf_doc.py
--rw-rw-rw-  2.0 fat      173 b- defN 22-Sep-28 19:08 parseq-2023.5.0/parseq/help/data.rst
--rw-rw-rw-  2.0 fat      222 b- defN 23-May-30 16:09 parseq-2023.5.0/parseq/help/fits.rst
--rw-rw-rw-  2.0 fat       43 b- defN 22-Sep-30 15:27 parseq-2023.5.0/parseq/help/howto.rst
--rw-rw-rw-  2.0 fat      405 b- defN 23-May-30 11:34 parseq-2023.5.0/parseq/help/index.rst
--rw-rw-rw-  2.0 fat     1134 b- defN 22-Sep-28 17:01 parseq-2023.5.0/parseq/help/license.rst
--rwx---     2.0 fat     5356 b- defN 16-Aug-10 15:09 parseq-2023.5.0/parseq/help/make.bat
--rw-rw-rw-  2.0 fat      141 b- defN 22-Sep-28 19:02 parseq-2023.5.0/parseq/help/nodes.rst
--rw-rw-rw-  2.0 fat       45 b- defN 22-Sep-28 19:30 parseq-2023.5.0/parseq/help/notesgui.rst
--rw-rw-rw-  2.0 fat      804 b- defN 23-Mar-09 10:03 parseq-2023.5.0/parseq/help/top.rst
--rw-rw-rw-  2.0 fat      143 b- defN 22-Sep-28 19:21 parseq-2023.5.0/parseq/help/transforms.rst
--rw-rw-rw-  2.0 fat      189 b- defN 23-Jan-23 18:49 parseq-2023.5.0/parseq/help/widgets.rst
--rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-2023.5.0/parseq/help/__init__.py
--rw-rw-rw-  2.0 fat     8824 b- defN 22-Sep-30 10:44 parseq-2023.5.0/parseq/help/exts/animation.py
--rw-rw-rw-  2.0 fat   873847 b- defN 21-Jun-21 17:49 parseq-2023.5.0/parseq/help/_images/mickey-rtfm.gif
--rw-rw-rw-  2.0 fat   176184 b- defN 23-Mar-10 17:16 parseq-2023.5.0/parseq/help/_images/node1.png
--rw-rw-rw-  2.0 fat    98843 b- defN 23-Mar-10 17:17 parseq-2023.5.0/parseq/help/_images/node2.png
--rw-rw-rw-  2.0 fat   187993 b- defN 23-Mar-10 17:17 parseq-2023.5.0/parseq/help/_images/node3.png
--rw-rw-rw-  2.0 fat   115965 b- defN 23-Mar-10 17:18 parseq-2023.5.0/parseq/help/_images/node4.png
--rw-rw-rw-  2.0 fat    67646 b- defN 17-Aug-08 13:54 parseq-2023.5.0/parseq/help/_images/parseq.ico
--rw-rw-rw-  2.0 fat   216689 b- defN 22-Sep-28 15:24 parseq-2023.5.0/parseq/help/_images/parseq_big.png
--rw-rw-rw-  2.0 fat    19518 b- defN 19-Mar-15 00:18 parseq-2023.5.0/parseq/help/_images/XAS_icon.ico
--rw-rw-rw-  2.0 fat    19518 b- defN 21-Jul-23 18:16 parseq-2023.5.0/parseq/help/_images/XES_dispersive_icon.ico
--rw-rw-rw-  2.0 fat    19518 b- defN 21-Jun-18 22:43 parseq-2023.5.0/parseq/help/_images/XES_scan_icon.ico
--rw-rw-rw-  2.0 fat     1171 b- defN 16-Aug-16 17:36 parseq-2023.5.0/parseq/help/_static/animation.js
--rw-rw-rw-  2.0 fat     1148 b- defN 21-Sep-22 15:17 parseq-2023.5.0/parseq/help/_static/thumbnail.css
--rw-rw-rw-  2.0 fat      504 b- defN 22-Sep-28 22:11 parseq-2023.5.0/parseq/help/_templates/layout.html
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_themes/mytheme/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_themes/parseq/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_themes/mytheme/static/
--rw-rw-rw-  2.0 fat      384 b- defN 18-Jun-28 10:33 parseq-2023.5.0/parseq/help/_themes/mytheme/layout.html
--rw-rw-rw-  2.0 fat       74 b- defN 23-Mar-03 12:15 parseq-2023.5.0/parseq/help/_themes/mytheme/theme.conf
--rw-rw-rw-  2.0 fat     4514 b- defN 23-Apr-02 12:36 parseq-2023.5.0/parseq/help/_themes/mytheme/static/mycss.css_t
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_themes/parseq/static/
--rw-rw-rw-  2.0 fat      868 b- defN 21-Jun-20 14:53 parseq-2023.5.0/parseq/help/_themes/parseq/layout.html
--rw-rw-rw-  2.0 fat      525 b- defN 18-Aug-13 16:19 parseq-2023.5.0/parseq/help/_themes/parseq/page.html
--rw-rw-rw-  2.0 fat      721 b- defN 18-Aug-13 16:19 parseq-2023.5.0/parseq/help/_themes/parseq/theme.conf
--rw-rw-rw-  2.0 fat     8115 b- defN 23-May-28 23:33 parseq-2023.5.0/parseq/help/_themes/parseq/static/default.css_t
--rw-rw-rw-  2.0 fat      488 b- defN 18-Aug-13 16:19 parseq-2023.5.0/parseq/help/_themes/parseq/static/math_config_win32.js
--rw-rw-rw-  2.0 fat     2243 b- defN 22-Jan-28 15:42 parseq-2023.5.0/parseq/help/_themes/parseq/static/utils.js
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/tests/data/
--rw-rw-rw-  2.0 fat    69161 b- defN 22-Nov-02 17:20 parseq-2023.5.0/parseq/tests/circles-rect.png
--rw-rw-rw-  2.0 fat    33688 b- defN 22-Aug-01 18:50 parseq-2023.5.0/parseq/tests/circles.png
--rw-rw-rw-  2.0 fat    21073 b- defN 21-Aug-09 10:56 parseq-2023.5.0/parseq/tests/modeltest.py
--rw-rw-rw-  2.0 fat      503 b- defN 22-Aug-27 11:17 parseq-2023.5.0/parseq/tests/test_aboutWidget.py
--rw-rw-rw-  2.0 fat      841 b- defN 22-Aug-27 11:15 parseq-2023.5.0/parseq/tests/test_calibrateEnergyWidget.py
--rw-rw-rw-  2.0 fat     1570 b- defN 22-Jul-13 15:11 parseq-2023.5.0/parseq/tests/test_columnStrings.py
--rw-rw-rw-  2.0 fat      592 b- defN 22-Aug-27 11:16 parseq-2023.5.0/parseq/tests/test_combineSpectraWidget.py
--rw-rw-rw-  2.0 fat     1027 b- defN 23-Feb-12 19:15 parseq-2023.5.0/parseq/tests/test_commons.py
--rw-rw-rw-  2.0 fat     1859 b- defN 22-Aug-02 14:07 parseq-2023.5.0/parseq/tests/test_curve_shear.py
--rw-rw-rw-  2.0 fat     2339 b- defN 23-Jan-24 14:23 parseq-2023.5.0/parseq/tests/test_dataRebinWidget.py
--rw-rw-rw-  2.0 fat     2641 b- defN 22-Aug-27 11:16 parseq-2023.5.0/parseq/tests/test_dataTreeModelView.py
--rw-rw-rw-  2.0 fat      646 b- defN 22-Aug-27 11:15 parseq-2023.5.0/parseq/tests/test_fileDialog.py
--rw-rw-rw-  2.0 fat     1612 b- defN 22-Jul-15 10:53 parseq-2023.5.0/parseq/tests/test_fileTreeModelView.py
--rw-rw-rw-  2.0 fat     9805 b- defN 23-May-30 14:47 parseq-2023.5.0/parseq/tests/test_fit.py
--rw-rw-rw-  2.0 fat      760 b- defN 22-Apr-15 08:28 parseq-2023.5.0/parseq/tests/test_flowLayout.py
--rw-rw-rw-  2.0 fat     2302 b- defN 22-Jul-13 15:37 parseq-2023.5.0/parseq/tests/test_hdf5.py
--rw-rw-rw-  2.0 fat     1300 b- defN 22-Aug-27 11:17 parseq-2023.5.0/parseq/tests/test_mainWindow.py
--rw-rw-rw-  2.0 fat     1160 b- defN 22-Sep-24 11:41 parseq-2023.5.0/parseq/tests/test_node.py
--rw-rw-rw-  2.0 fat      817 b- defN 22-Aug-27 11:15 parseq-2023.5.0/parseq/tests/test_nodeWidget.py
--rw-rw-rw-  2.0 fat     2649 b- defN 22-Nov-18 11:49 parseq-2023.5.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py
--rw-rw-rw-  2.0 fat     2762 b- defN 22-Aug-20 22:24 parseq-2023.5.0/parseq/tests/test_plotInteractiveImageSingleROI.py
--rw-rw-rw-  2.0 fat     1060 b- defN 22-Aug-27 11:15 parseq-2023.5.0/parseq/tests/test_plotOptions.py
--rw-rw-rw-  2.0 fat     1485 b- defN 22-Jul-23 17:28 parseq-2023.5.0/parseq/tests/test_QSortFilterProxyModel.py
--rw-rw-rw-  2.0 fat     1248 b- defN 21-Aug-09 10:56 parseq-2023.5.0/parseq/tests/test_ROI.py
--rw-rw-rw-  2.0 fat     1028 b- defN 21-Aug-09 10:56 parseq-2023.5.0/parseq/tests/test_slice.py
--rw-rw-rw-  2.0 fat      572 b- defN 23-Feb-24 09:56 parseq-2023.5.0/parseq/tests/test_stateButtons.py
--rw-rw-rw-  2.0 fat      218 b- defN 22-Aug-27 11:17 parseq-2023.5.0/parseq/tests/__init__.py
--rw-rw-rw-  2.0 fat   209750 b- defN 19-Nov-27 14:45 parseq-2023.5.0/parseq/tests/data/cu-ref-mix.res
--rw-rw-rw-  2.0 fat    77692 b- defN 19-Nov-27 14:47 parseq-2023.5.0/parseq/tests/data/pb-ref-mix.res
--rw-rw-rw-  2.0 fat   167161 b- defN 19-Nov-27 14:46 parseq-2023.5.0/parseq/tests/data/zn-ref-mix.res
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/third_party/data/
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-03 20:36 parseq-2023.5.0/parseq/third_party/XAFSmass.py
--rw-rw-rw-  2.0 fat      732 b- defN 22-Aug-28 12:11 parseq-2023.5.0/parseq/third_party/xrt.py
--rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-2023.5.0/parseq/third_party/__init__.py
--rw-rw-rw-  2.0 fat     7812 b- defN 17-Aug-04 10:49 parseq-2023.5.0/parseq/third_party/data/Energies.txt
--rw-rw-rw-  2.0 fat      345 b- defN 22-Mar-31 11:43 parseq-2023.5.0/parseq/utils/format.py
--rw-rw-rw-  2.0 fat     2009 b- defN 23-Mar-29 00:12 parseq-2023.5.0/parseq/utils/ft.py
--rw-rw-rw-  2.0 fat     1660 b- defN 23-Mar-20 16:04 parseq-2023.5.0/parseq/utils/h5reduce.py
--rw-rw-rw-  2.0 fat     3873 b- defN 23-Apr-26 18:43 parseq-2023.5.0/parseq/utils/math.py
--rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-2023.5.0/parseq/utils/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat     5037 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      140 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/requires.txt
--rw-rw-rw-  2.0 fat     5003 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        7 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/top_level.txt
-177 files, 3319887 bytes uncompressed, 2216633 bytes compressed:  33.2%
+Zip file size: 2598712 bytes, number of entries: 200
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq.egg-info/
+-rw-rw-rw-  2.0 fat     1099 b- defN 20-Nov-24 00:11 parseq-2024.5.0/LICENSE
+-rw-rw-rw-  2.0 fat     5796 b- defN 24-May-04 21:38 parseq-2024.5.0/PKG-INFO
+-rw-rw-rw-  2.0 fat       42 b- defN 24-May-04 21:38 parseq-2024.5.0/setup.cfg
+-rw-rw-rw-  2.0 fat     3642 b- defN 24-Apr-29 16:03 parseq-2024.5.0/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/core/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/fits/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/gui/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/help/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/tests/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/third_party/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/utils/
+-rw-rw-rw-  2.0 fat      386 b- defN 18-Nov-18 11:39 parseq-2024.5.0/parseq/CODERULES.txt
+-rw-rw-rw-  2.0 fat     4442 b- defN 24-Apr-29 15:06 parseq-2024.5.0/parseq/description.py
+-rw-rw-rw-  2.0 fat      136 b- defN 24-May-04 18:42 parseq-2024.5.0/parseq/version.py
+-rw-rw-rw-  2.0 fat      731 b- defN 22-Sep-28 11:28 parseq-2024.5.0/parseq/__init__.py
+-rw-rw-rw-  2.0 fat     8120 b- defN 24-Apr-25 11:26 parseq-2024.5.0/parseq/core/commons.py
+-rw-rw-rw-  2.0 fat     2546 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/core/config.py
+-rw-rw-rw-  2.0 fat     2144 b- defN 24-Apr-24 20:41 parseq-2024.5.0/parseq/core/correction.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 24-Apr-28 11:17 parseq-2024.5.0/parseq/core/logger.py
+-rw-rw-rw-  2.0 fat    10409 b- defN 24-May-04 11:19 parseq-2024.5.0/parseq/core/nodes.py
+-rw-rw-rw-  2.0 fat    10247 b- defN 24-Mar-25 15:43 parseq-2024.5.0/parseq/core/plotExport.py
+-rw-rw-rw-  2.0 fat    19269 b- defN 24-Apr-27 14:52 parseq-2024.5.0/parseq/core/save_restore.py
+-rw-rw-rw-  2.0 fat     1564 b- defN 24-Apr-22 23:59 parseq-2024.5.0/parseq/core/singletons.py
+-rw-rw-rw-  2.0 fat    80830 b- defN 24-May-04 16:11 parseq-2024.5.0/parseq/core/spectra.py
+-rw-rw-rw-  2.0 fat    30281 b- defN 24-May-04 12:47 parseq-2024.5.0/parseq/core/transforms.py
+-rw-rw-rw-  2.0 fat    20282 b- defN 24-May-04 20:46 parseq-2024.5.0/parseq/core/__init__.py
+-rw-rw-rw-  2.0 fat    23800 b- defN 23-Dec-06 09:21 parseq-2024.5.0/parseq/fits/basefit.py
+-rw-rw-rw-  2.0 fat    23390 b- defN 23-Dec-03 11:19 parseq-2024.5.0/parseq/fits/exafsfit.py
+-rw-rw-rw-  2.0 fat     6214 b- defN 23-Nov-24 09:23 parseq-2024.5.0/parseq/fits/functionfit.py
+-rw-rw-rw-  2.0 fat    11294 b- defN 23-Nov-24 09:23 parseq-2024.5.0/parseq/fits/lcf.py
+-rw-rw-rw-  2.0 fat       67 b- defN 23-Sep-28 09:23 parseq-2024.5.0/parseq/fits/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/gui/fits/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/gui/_images/
+-rw-rw-rw-  2.0 fat    16599 b- defN 24-Apr-30 11:08 parseq-2024.5.0/parseq/gui/aboutDialog.py
+-rw-rw-rw-  2.0 fat     9823 b- defN 24-Apr-26 16:13 parseq-2024.5.0/parseq/gui/calibrateEnergy.py
+-rw-rw-rw-  2.0 fat    18422 b- defN 24-May-04 09:36 parseq-2024.5.0/parseq/gui/columnFormat.py
+-rw-rw-rw-  2.0 fat     5680 b- defN 23-Oct-04 09:56 parseq-2024.5.0/parseq/gui/combineSpectra.py
+-rw-rw-rw-  2.0 fat    18954 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/gui/dataRebin.py
+-rw-rw-rw-  2.0 fat    52100 b- defN 24-May-04 18:25 parseq-2024.5.0/parseq/gui/dataTreeModelView.py
+-rw-rw-rw-  2.0 fat    10208 b- defN 23-Dec-05 23:29 parseq-2024.5.0/parseq/gui/fileDialogs.py
+-rw-rw-rw-  2.0 fat    65879 b- defN 24-May-04 19:43 parseq-2024.5.0/parseq/gui/fileTreeModelView.py
+-rw-rw-rw-  2.0 fat    17848 b- defN 24-Apr-18 15:57 parseq-2024.5.0/parseq/gui/gcommons.py
+-rw-rw-rw-  2.0 fat    33339 b- defN 24-Apr-28 19:48 parseq-2024.5.0/parseq/gui/gcorrection.py
+-rw-rw-rw-  2.0 fat    34067 b- defN 24-May-04 13:03 parseq-2024.5.0/parseq/gui/mainWindow.py
+-rw-rw-rw-  2.0 fat    58694 b- defN 24-May-04 09:31 parseq-2024.5.0/parseq/gui/nodeWidget.py
+-rw-rw-rw-  2.0 fat     5105 b- defN 23-Sep-15 18:28 parseq-2024.5.0/parseq/gui/plot.py
+-rw-rw-rw-  2.0 fat    25381 b- defN 23-Mar-22 21:32 parseq-2024.5.0/parseq/gui/plotOptions.py
+-rw-rw-rw-  2.0 fat     9444 b- defN 23-Dec-06 11:08 parseq-2024.5.0/parseq/gui/propsOfData.py
+-rw-rw-rw-  2.0 fat    37959 b- defN 24-May-04 13:04 parseq-2024.5.0/parseq/gui/propWidget.py
+-rw-rw-rw-  2.0 fat    51505 b- defN 24-Apr-21 08:31 parseq-2024.5.0/parseq/gui/roi.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/gui/tasker.py
+-rw-rw-rw-  2.0 fat     4937 b- defN 22-Oct-14 12:12 parseq-2024.5.0/parseq/gui/undoredo.py
+-rw-rw-rw-  2.0 fat     9801 b- defN 23-Aug-27 20:56 parseq-2024.5.0/parseq/gui/webWidget.py
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-04 16:07 parseq-2024.5.0/parseq/gui/__init__.py
+-rw-rw-rw-  2.0 fat    13402 b- defN 23-Dec-06 10:40 parseq-2024.5.0/parseq/gui/fits/gbasefit.py
+-rw-rw-rw-  2.0 fat    33365 b- defN 23-Nov-29 22:32 parseq-2024.5.0/parseq/gui/fits/gexafsfit.py
+-rw-rw-rw-  2.0 fat    16083 b- defN 23-Nov-24 16:10 parseq-2024.5.0/parseq/gui/fits/gfunctionfit.py
+-rw-rw-rw-  2.0 fat    19236 b- defN 23-Nov-21 20:47 parseq-2024.5.0/parseq/gui/fits/glcf.py
+-rw-rw-rw-  2.0 fat       25 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/gui/fits/__init__.py
+-rw-rw-rw-  2.0 fat      559 b- defN 24-Apr-28 19:51 parseq-2024.5.0/parseq/gui/_images/icon-add-correction-delete-24.png
+-rw-rw-rw-  2.0 fat      687 b- defN 24-Apr-19 14:29 parseq-2024.5.0/parseq/gui/_images/icon-add-correction-delete-32.png
+-rw-rw-rw-  2.0 fat      556 b- defN 24-Apr-28 19:51 parseq-2024.5.0/parseq/gui/_images/icon-add-correction-scale-24.png
+-rw-rw-rw-  2.0 fat      685 b- defN 24-Apr-19 14:29 parseq-2024.5.0/parseq/gui/_images/icon-add-correction-scale-32.png
+-rw-rw-rw-  2.0 fat      924 b- defN 24-Apr-28 19:52 parseq-2024.5.0/parseq/gui/_images/icon-add-correction-spline-24.png
+-rw-rw-rw-  2.0 fat     1254 b- defN 24-Apr-21 16:50 parseq-2024.5.0/parseq/gui/_images/icon-add-correction-spline-32.png
+-rw-rw-rw-  2.0 fat      621 b- defN 24-Apr-28 19:52 parseq-2024.5.0/parseq/gui/_images/icon-add-correction-step-24.png
+-rw-rw-rw-  2.0 fat      765 b- defN 24-Apr-21 16:50 parseq-2024.5.0/parseq/gui/_images/icon-add-correction-step-32.png
+-rw-rw-rw-  2.0 fat     2255 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/gui/_images/icon-fit-32.png
+-rw-rw-rw-  2.0 fat     4846 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/gui/_images/icon-fit-64.png
+-rw-rw-rw-  2.0 fat     5831 b- defN 21-Apr-21 15:48 parseq-2024.5.0/parseq/gui/_images/icon-help.png
+-rw-rw-rw-  2.0 fat     5473 b- defN 21-Apr-21 15:48 parseq-2024.5.0/parseq/gui/_images/icon-info.png
+-rw-rw-rw-  2.0 fat     1340 b- defN 21-May-13 14:48 parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-32.png
+-rw-rw-rw-  2.0 fat     2414 b- defN 22-Jun-02 12:07 parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-64.png
+-rw-rw-rw-  2.0 fat     1244 b- defN 22-Jul-20 22:55 parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-busy-32.png
+-rw-rw-rw-  2.0 fat     2221 b- defN 22-Jul-20 22:55 parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-busy-64.png
+-rw-rw-rw-  2.0 fat      461 b- defN 21-May-13 14:39 parseq-2024.5.0/parseq/gui/_images/icon-item-2dim-32.png
+-rw-rw-rw-  2.0 fat      582 b- defN 22-Jun-02 12:09 parseq-2024.5.0/parseq/gui/_images/icon-item-2dim-64.png
+-rw-rw-rw-  2.0 fat      452 b- defN 22-Jul-20 22:56 parseq-2024.5.0/parseq/gui/_images/icon-item-2dim-busy-32.png
+-rw-rw-rw-  2.0 fat      557 b- defN 22-Jul-20 22:56 parseq-2024.5.0/parseq/gui/_images/icon-item-2dim-busy-64.png
+-rw-rw-rw-  2.0 fat     1441 b- defN 21-May-13 14:39 parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-32.png
+-rw-rw-rw-  2.0 fat     2834 b- defN 22-Jun-02 12:10 parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-64.png
+-rw-rw-rw-  2.0 fat     1347 b- defN 22-Jul-20 22:57 parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-busy-32.png
+-rw-rw-rw-  2.0 fat     2673 b- defN 22-Jul-20 22:57 parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-busy-64.png
+-rw-rw-rw-  2.0 fat     2164 b- defN 22-Jul-21 12:50 parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-32.png
+-rw-rw-rw-  2.0 fat     4780 b- defN 22-Jul-21 12:50 parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-64.png
+-rw-rw-rw-  2.0 fat     2005 b- defN 22-Jul-21 12:50 parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-busy-32.png
+-rw-rw-rw-  2.0 fat     4515 b- defN 22-Jul-21 12:51 parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-busy-64.png
+-rw-rw-rw-  2.0 fat     5529 b- defN 21-Apr-22 22:43 parseq-2024.5.0/parseq/gui/_images/icon-load-proj.png
+-rw-rw-rw-  2.0 fat     3575 b- defN 21-Apr-21 15:56 parseq-2024.5.0/parseq/gui/_images/icon-redo.png
+-rw-rw-rw-  2.0 fat     5462 b- defN 21-Apr-22 22:44 parseq-2024.5.0/parseq/gui/_images/icon-save-proj.png
+-rw-rw-rw-  2.0 fat     4662 b- defN 21-Apr-22 22:44 parseq-2024.5.0/parseq/gui/_images/icon-save-text.png
+-rw-rw-rw-  2.0 fat     3625 b- defN 21-Apr-21 15:56 parseq-2024.5.0/parseq/gui/_images/icon-undo.png
+-rw-rw-rw-  2.0 fat    67646 b- defN 17-Aug-08 13:54 parseq-2024.5.0/parseq/gui/_images/parseq.ico
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/help/exts/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/help/_images/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/help/_static/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/help/_templates/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/help/_themes/
+-rw-rw-rw-  2.0 fat     7052 b- defN 23-Mar-22 21:32 parseq-2024.5.0/parseq/help/conf.py
+-rw-rw-rw-  2.0 fat     3547 b- defN 22-Sep-30 12:10 parseq-2024.5.0/parseq/help/conf_doc.py
+-rw-rw-rw-  2.0 fat      173 b- defN 22-Sep-28 19:08 parseq-2024.5.0/parseq/help/data.rst
+-rw-rw-rw-  2.0 fat      222 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/help/fits.rst
+-rw-rw-rw-  2.0 fat      614 b- defN 24-May-04 21:30 parseq-2024.5.0/parseq/help/history.rst
+-rw-rw-rw-  2.0 fat       43 b- defN 22-Sep-30 15:27 parseq-2024.5.0/parseq/help/howto.rst
+-rw-rw-rw-  2.0 fat      388 b- defN 24-May-04 16:08 parseq-2024.5.0/parseq/help/index.rst
+-rw-rw-rw-  2.0 fat     1134 b- defN 22-Sep-28 17:01 parseq-2024.5.0/parseq/help/license.rst
+-rwx---     2.0 fat     5356 b- defN 16-Aug-10 15:09 parseq-2024.5.0/parseq/help/make.bat
+-rw-rw-rw-  2.0 fat      141 b- defN 22-Sep-28 19:02 parseq-2024.5.0/parseq/help/nodes.rst
+-rw-rw-rw-  2.0 fat      837 b- defN 24-Apr-29 16:07 parseq-2024.5.0/parseq/help/top.rst
+-rw-rw-rw-  2.0 fat      143 b- defN 22-Sep-28 19:21 parseq-2024.5.0/parseq/help/transforms.rst
+-rw-rw-rw-  2.0 fat      189 b- defN 23-Jan-23 18:49 parseq-2024.5.0/parseq/help/widgets.rst
+-rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-2024.5.0/parseq/help/__init__.py
+-rw-rw-rw-  2.0 fat     9866 b- defN 24-May-03 20:13 parseq-2024.5.0/parseq/help/exts/animation.py
+-rw-rw-rw-  2.0 fat   873847 b- defN 21-Jun-21 17:49 parseq-2024.5.0/parseq/help/_images/mickey-rtfm.gif
+-rw-rw-rw-  2.0 fat    67646 b- defN 17-Aug-08 13:54 parseq-2024.5.0/parseq/help/_images/parseq.ico
+-rw-rw-rw-  2.0 fat   216689 b- defN 22-Sep-28 16:24 parseq-2024.5.0/parseq/help/_images/parseq_big.png
+-rw-rw-rw-  2.0 fat    32215 b- defN 24-Apr-30 12:14 parseq-2024.5.0/parseq/help/_images/pipeline-data-tree.png
+-rw-rw-rw-  2.0 fat    24471 b- defN 24-May-03 13:47 parseq-2024.5.0/parseq/help/_images/pipeline-file-tree.png
+-rw-rw-rw-  2.0 fat    23341 b- defN 24-Apr-30 12:02 parseq-2024.5.0/parseq/help/_images/pipeline-fit-EXAFS.png
+-rw-rw-rw-  2.0 fat    63444 b- defN 24-Apr-30 11:34 parseq-2024.5.0/parseq/help/_images/pipeline-graph-XAS.png
+-rw-rw-rw-  2.0 fat    16467 b- defN 24-May-03 16:10 parseq-2024.5.0/parseq/help/_images/pipeline-line-props.png
+-rw-rw-rw-  2.0 fat    99630 b- defN 24-May-03 16:43 parseq-2024.5.0/parseq/help/_images/pipeline-proj-load.png
+-rw-rw-rw-  2.0 fat    91072 b- defN 24-May-03 16:43 parseq-2024.5.0/parseq/help/_images/pipeline-proj-save.png
+-rw-rw-rw-  2.0 fat    38292 b- defN 24-May-03 19:02 parseq-2024.5.0/parseq/help/_images/pipeline-timing.png
+-rw-rw-rw-  2.0 fat    15242 b- defN 24-May-01 14:58 parseq-2024.5.0/parseq/help/_images/pipeline-transform-apply.png
+-rw-rw-rw-  2.0 fat    27073 b- defN 24-May-02 20:22 parseq-2024.5.0/parseq/help/_images/pipeline-undo.png
+-rw-rw-rw-  2.0 fat   433429 b- defN 24-Apr-28 23:58 parseq-2024.5.0/parseq/help/_images/XAS-foils.gif
+-rw-rw-rw-  2.0 fat     1171 b- defN 24-May-01 10:54 parseq-2024.5.0/parseq/help/_static/animation.js
+-rw-rw-rw-  2.0 fat     1151 b- defN 24-May-02 20:28 parseq-2024.5.0/parseq/help/_static/thumbnail.css
+-rw-rw-rw-  2.0 fat      504 b- defN 22-Sep-28 22:11 parseq-2024.5.0/parseq/help/_templates/layout.html
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/help/_themes/mytheme/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/help/_themes/parseq/
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/help/_themes/mytheme/static/
+-rw-rw-rw-  2.0 fat      384 b- defN 18-Jun-28 10:33 parseq-2024.5.0/parseq/help/_themes/mytheme/layout.html
+-rw-rw-rw-  2.0 fat       74 b- defN 23-Mar-03 12:15 parseq-2024.5.0/parseq/help/_themes/mytheme/theme.conf
+-rw-rw-rw-  2.0 fat     4556 b- defN 24-May-03 18:01 parseq-2024.5.0/parseq/help/_themes/mytheme/static/mycss.css_t
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/help/_themes/parseq/static/
+-rw-rw-rw-  2.0 fat      868 b- defN 21-Jun-20 14:53 parseq-2024.5.0/parseq/help/_themes/parseq/layout.html
+-rw-rw-rw-  2.0 fat      525 b- defN 18-Aug-13 16:19 parseq-2024.5.0/parseq/help/_themes/parseq/page.html
+-rw-rw-rw-  2.0 fat      721 b- defN 18-Aug-13 16:19 parseq-2024.5.0/parseq/help/_themes/parseq/theme.conf
+-rw-rw-rw-  2.0 fat     8170 b- defN 24-Mar-28 22:06 parseq-2024.5.0/parseq/help/_themes/parseq/static/default.css_t
+-rw-rw-rw-  2.0 fat      488 b- defN 18-Aug-13 16:19 parseq-2024.5.0/parseq/help/_themes/parseq/static/math_config_win32.js
+-rw-rw-rw-  2.0 fat     2384 b- defN 23-Sep-03 11:48 parseq-2024.5.0/parseq/help/_themes/parseq/static/utils.js
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/tests/data/
+-rw-rw-rw-  2.0 fat    69161 b- defN 24-Apr-26 21:17 parseq-2024.5.0/parseq/tests/circles-rect.png
+-rw-rw-rw-  2.0 fat    33688 b- defN 22-Aug-01 18:50 parseq-2024.5.0/parseq/tests/circles.png
+-rw-rw-rw-  2.0 fat    21073 b- defN 21-Aug-09 10:56 parseq-2024.5.0/parseq/tests/modeltest.py
+-rw-rw-rw-  2.0 fat      503 b- defN 22-Aug-27 11:17 parseq-2024.5.0/parseq/tests/test_aboutWidget.py
+-rw-rw-rw-  2.0 fat      841 b- defN 22-Aug-27 11:15 parseq-2024.5.0/parseq/tests/test_calibrateEnergyWidget.py
+-rw-rw-rw-  2.0 fat     1570 b- defN 22-Jul-13 15:11 parseq-2024.5.0/parseq/tests/test_columnStrings.py
+-rw-rw-rw-  2.0 fat      592 b- defN 22-Aug-27 11:16 parseq-2024.5.0/parseq/tests/test_combineSpectraWidget.py
+-rw-rw-rw-  2.0 fat     1027 b- defN 23-Feb-12 19:15 parseq-2024.5.0/parseq/tests/test_commons.py
+-rw-rw-rw-  2.0 fat     1859 b- defN 22-Aug-02 14:07 parseq-2024.5.0/parseq/tests/test_curve_shear.py
+-rw-rw-rw-  2.0 fat     2862 b- defN 24-Apr-22 17:04 parseq-2024.5.0/parseq/tests/test_dataCorrection.py
+-rw-rw-rw-  2.0 fat     2339 b- defN 23-Jan-24 14:23 parseq-2024.5.0/parseq/tests/test_dataRebinWidget.py
+-rw-rw-rw-  2.0 fat     2641 b- defN 22-Aug-27 11:16 parseq-2024.5.0/parseq/tests/test_dataTreeModelView.py
+-rw-rw-rw-  2.0 fat      646 b- defN 22-Aug-27 11:15 parseq-2024.5.0/parseq/tests/test_fileDialog.py
+-rw-rw-rw-  2.0 fat     2711 b- defN 24-Mar-13 17:41 parseq-2024.5.0/parseq/tests/test_fileTreeModelView.py
+-rw-rw-rw-  2.0 fat     9867 b- defN 23-Nov-09 16:50 parseq-2024.5.0/parseq/tests/test_fit.py
+-rw-rw-rw-  2.0 fat     9917 b- defN 23-Nov-21 15:10 parseq-2024.5.0/parseq/tests/test_fit_EXAFS.py
+-rw-rw-rw-  2.0 fat      760 b- defN 22-Apr-15 08:28 parseq-2024.5.0/parseq/tests/test_flowLayout.py
+-rw-rw-rw-  2.0 fat     2376 b- defN 24-Feb-24 10:26 parseq-2024.5.0/parseq/tests/test_hdf5.py
+-rw-rw-rw-  2.0 fat     1300 b- defN 22-Aug-27 11:17 parseq-2024.5.0/parseq/tests/test_mainWindow.py
+-rw-rw-rw-  2.0 fat     1160 b- defN 22-Sep-24 11:41 parseq-2024.5.0/parseq/tests/test_node.py
+-rw-rw-rw-  2.0 fat      817 b- defN 22-Aug-27 11:15 parseq-2024.5.0/parseq/tests/test_nodeWidget.py
+-rw-rw-rw-  2.0 fat     2649 b- defN 22-Nov-18 11:49 parseq-2024.5.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py
+-rw-rw-rw-  2.0 fat     2762 b- defN 22-Aug-20 22:24 parseq-2024.5.0/parseq/tests/test_plotInteractiveImageSingleROI.py
+-rw-rw-rw-  2.0 fat     1060 b- defN 22-Aug-27 11:15 parseq-2024.5.0/parseq/tests/test_plotOptions.py
+-rw-rw-rw-  2.0 fat     1485 b- defN 22-Jul-23 17:28 parseq-2024.5.0/parseq/tests/test_QSortFilterProxyModel.py
+-rw-rw-rw-  2.0 fat     1248 b- defN 21-Aug-09 10:56 parseq-2024.5.0/parseq/tests/test_ROI.py
+-rw-rw-rw-  2.0 fat     1028 b- defN 21-Aug-09 10:56 parseq-2024.5.0/parseq/tests/test_slice.py
+-rw-rw-rw-  2.0 fat      572 b- defN 23-Feb-24 09:56 parseq-2024.5.0/parseq/tests/test_stateButtons.py
+-rw-rw-rw-  2.0 fat      218 b- defN 22-Aug-27 11:17 parseq-2024.5.0/parseq/tests/__init__.py
+-rw-rw-rw-  2.0 fat     6035 b- defN 23-Sep-29 16:49 parseq-2024.5.0/parseq/tests/data/BFT-Cu-foil_EXAFS_23070.txt.gz
+-rw-rw-rw-  2.0 fat     6775 b- defN 23-Nov-11 23:29 parseq-2024.5.0/parseq/tests/data/Ce-CeRu2.bft
+-rw-rw-rw-  2.0 fat   209750 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/tests/data/cu-ref-mix.res
+-rw-rw-rw-  2.0 fat    21906 b- defN 23-Sep-25 21:40 parseq-2024.5.0/parseq/tests/data/fitTestEXAFS.h5
+-rw-rw-rw-  2.0 fat    77692 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/tests/data/pb-ref-mix.res
+-rw-rw-rw-  2.0 fat    11620 b- defN 23-Nov-11 23:29 parseq-2024.5.0/parseq/tests/data/Ru-CeRu2.bft
+-rw-rw-rw-  2.0 fat   167161 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/tests/data/zn-ref-mix.res
+drwxrwxrwx  2.0 fat        0 b- stor 24-May-04 21:38 parseq-2024.5.0/parseq/third_party/data/
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/third_party/XAFSmass.py
+-rw-rw-rw-  2.0 fat      732 b- defN 22-Aug-28 12:11 parseq-2024.5.0/parseq/third_party/xrt.py
+-rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-2024.5.0/parseq/third_party/__init__.py
+-rw-rw-rw-  2.0 fat     7812 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/third_party/data/Energies.txt
+-rw-rw-rw-  2.0 fat      144 b- defN 23-Nov-03 11:41 parseq-2024.5.0/parseq/utils/constants.py
+-rw-rw-rw-  2.0 fat      345 b- defN 22-Mar-31 11:43 parseq-2024.5.0/parseq/utils/format.py
+-rw-rw-rw-  2.0 fat     2090 b- defN 23-Dec-15 20:40 parseq-2024.5.0/parseq/utils/ft.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 24-Feb-24 10:26 parseq-2024.5.0/parseq/utils/h5reduce.py
+-rw-rw-rw-  2.0 fat     3873 b- defN 23-Jun-12 21:56 parseq-2024.5.0/parseq/utils/math.py
+-rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-2024.5.0/parseq/utils/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-04 21:38 parseq-2024.5.0/parseq.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 24-May-04 21:38 parseq-2024.5.0/parseq.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat     5796 b- defN 24-May-04 21:38 parseq-2024.5.0/parseq.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      163 b- defN 24-May-04 21:38 parseq-2024.5.0/parseq.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat     5958 b- defN 24-May-04 21:38 parseq-2024.5.0/parseq.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-04 21:38 parseq-2024.5.0/parseq.egg-info/top_level.txt
+200 files, 3766841 bytes uncompressed, 2565232 bytes compressed:  31.9%
```

## zipnote {}

```diff
@@ -1,532 +1,601 @@
-Filename: parseq-2023.5.0/
+Filename: parseq-2024.5.0/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/
+Filename: parseq-2024.5.0/parseq/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq.egg-info/
+Filename: parseq-2024.5.0/parseq.egg-info/
 Comment: 
 
-Filename: parseq-2023.5.0/LICENSE
+Filename: parseq-2024.5.0/LICENSE
 Comment: 
 
-Filename: parseq-2023.5.0/PKG-INFO
+Filename: parseq-2024.5.0/PKG-INFO
 Comment: 
 
-Filename: parseq-2023.5.0/setup.cfg
+Filename: parseq-2024.5.0/setup.cfg
 Comment: 
 
-Filename: parseq-2023.5.0/setup.py
+Filename: parseq-2024.5.0/setup.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/
+Filename: parseq-2024.5.0/parseq/core/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/fits/
+Filename: parseq-2024.5.0/parseq/fits/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/
+Filename: parseq-2024.5.0/parseq/gui/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/
+Filename: parseq-2024.5.0/parseq/help/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/
+Filename: parseq-2024.5.0/parseq/tests/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/third_party/
+Filename: parseq-2024.5.0/parseq/third_party/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/utils/
+Filename: parseq-2024.5.0/parseq/utils/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/CODERULES.txt
+Filename: parseq-2024.5.0/parseq/CODERULES.txt
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/description.py
+Filename: parseq-2024.5.0/parseq/description.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/version.py
+Filename: parseq-2024.5.0/parseq/version.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/__init__.py
+Filename: parseq-2024.5.0/parseq/__init__.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/commons.py
+Filename: parseq-2024.5.0/parseq/core/commons.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/config.py
+Filename: parseq-2024.5.0/parseq/core/config.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/logger.py
+Filename: parseq-2024.5.0/parseq/core/correction.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/nodes.py
+Filename: parseq-2024.5.0/parseq/core/logger.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/plotExport.py
+Filename: parseq-2024.5.0/parseq/core/nodes.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/save_restore.py
+Filename: parseq-2024.5.0/parseq/core/plotExport.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/singletons.py
+Filename: parseq-2024.5.0/parseq/core/save_restore.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/spectra.py
+Filename: parseq-2024.5.0/parseq/core/singletons.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/transforms.py
+Filename: parseq-2024.5.0/parseq/core/spectra.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/core/__init__.py
+Filename: parseq-2024.5.0/parseq/core/transforms.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/fits/basefit.py
+Filename: parseq-2024.5.0/parseq/core/__init__.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/fits/functionfit.py
+Filename: parseq-2024.5.0/parseq/fits/basefit.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/fits/lcf.py
+Filename: parseq-2024.5.0/parseq/fits/exafsfit.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/fits/__init__.py
+Filename: parseq-2024.5.0/parseq/fits/functionfit.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/fits/
+Filename: parseq-2024.5.0/parseq/fits/lcf.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/
+Filename: parseq-2024.5.0/parseq/fits/__init__.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/aboutDialog.py
+Filename: parseq-2024.5.0/parseq/gui/fits/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/calibrateEnergy.py
+Filename: parseq-2024.5.0/parseq/gui/_images/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/columnFormat.py
+Filename: parseq-2024.5.0/parseq/gui/aboutDialog.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/combineSpectra.py
+Filename: parseq-2024.5.0/parseq/gui/calibrateEnergy.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/dataRebin.py
+Filename: parseq-2024.5.0/parseq/gui/columnFormat.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/dataTreeModelView.py
+Filename: parseq-2024.5.0/parseq/gui/combineSpectra.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/fileDialogs.py
+Filename: parseq-2024.5.0/parseq/gui/dataRebin.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/fileTreeModelView.py
+Filename: parseq-2024.5.0/parseq/gui/dataTreeModelView.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/gcommons.py
+Filename: parseq-2024.5.0/parseq/gui/fileDialogs.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/mainWindow.py
+Filename: parseq-2024.5.0/parseq/gui/fileTreeModelView.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/nodeWidget.py
+Filename: parseq-2024.5.0/parseq/gui/gcommons.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/plot.py
+Filename: parseq-2024.5.0/parseq/gui/gcorrection.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/plotOptions.py
+Filename: parseq-2024.5.0/parseq/gui/mainWindow.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/propsOfData.py
+Filename: parseq-2024.5.0/parseq/gui/nodeWidget.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/propWidget.py
+Filename: parseq-2024.5.0/parseq/gui/plot.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/roi.py
+Filename: parseq-2024.5.0/parseq/gui/plotOptions.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/tasker.py
+Filename: parseq-2024.5.0/parseq/gui/propsOfData.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/undoredo.py
+Filename: parseq-2024.5.0/parseq/gui/propWidget.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/webWidget.py
+Filename: parseq-2024.5.0/parseq/gui/roi.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/__init__.py
+Filename: parseq-2024.5.0/parseq/gui/tasker.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/fits/gbasefit.py
+Filename: parseq-2024.5.0/parseq/gui/undoredo.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/fits/gfunctionfit.py
+Filename: parseq-2024.5.0/parseq/gui/webWidget.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/fits/glcf.py
+Filename: parseq-2024.5.0/parseq/gui/__init__.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/fits/__init__.py
+Filename: parseq-2024.5.0/parseq/gui/fits/gbasefit.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-fit-32.png
+Filename: parseq-2024.5.0/parseq/gui/fits/gexafsfit.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-fit-64.png
+Filename: parseq-2024.5.0/parseq/gui/fits/gfunctionfit.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-help.png
+Filename: parseq-2024.5.0/parseq/gui/fits/glcf.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-info.png
+Filename: parseq-2024.5.0/parseq/gui/fits/__init__.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-32.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-add-correction-delete-24.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-64.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-add-correction-delete-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-32.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-add-correction-scale-24.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-64.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-add-correction-scale-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-32.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-add-correction-spline-24.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-64.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-add-correction-spline-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-busy-32.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-add-correction-step-24.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-busy-64.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-add-correction-step-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-32.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-fit-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-64.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-fit-64.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-32.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-help.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-64.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-info.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-32.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-64.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-64.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-32.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-busy-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-64.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-busy-64.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-load-proj.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-2dim-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-redo.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-2dim-64.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-save-proj.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-2dim-busy-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-save-text.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-2dim-busy-64.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/icon-undo.png
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/gui/_images/parseq.ico
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-64.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/exts/
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-busy-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-busy-64.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_static/
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_templates/
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-64.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-busy-32.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/conf.py
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-busy-64.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/conf_doc.py
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-load-proj.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/data.rst
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-redo.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/fits.rst
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-save-proj.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/howto.rst
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-save-text.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/index.rst
+Filename: parseq-2024.5.0/parseq/gui/_images/icon-undo.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/license.rst
+Filename: parseq-2024.5.0/parseq/gui/_images/parseq.ico
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/make.bat
+Filename: parseq-2024.5.0/parseq/help/exts/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/nodes.rst
+Filename: parseq-2024.5.0/parseq/help/_images/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/notesgui.rst
+Filename: parseq-2024.5.0/parseq/help/_static/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/top.rst
+Filename: parseq-2024.5.0/parseq/help/_templates/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/transforms.rst
+Filename: parseq-2024.5.0/parseq/help/_themes/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/widgets.rst
+Filename: parseq-2024.5.0/parseq/help/conf.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/__init__.py
+Filename: parseq-2024.5.0/parseq/help/conf_doc.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/exts/animation.py
+Filename: parseq-2024.5.0/parseq/help/data.rst
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/mickey-rtfm.gif
+Filename: parseq-2024.5.0/parseq/help/fits.rst
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/node1.png
+Filename: parseq-2024.5.0/parseq/help/history.rst
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/node2.png
+Filename: parseq-2024.5.0/parseq/help/howto.rst
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/node3.png
+Filename: parseq-2024.5.0/parseq/help/index.rst
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/node4.png
+Filename: parseq-2024.5.0/parseq/help/license.rst
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/parseq.ico
+Filename: parseq-2024.5.0/parseq/help/make.bat
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/parseq_big.png
+Filename: parseq-2024.5.0/parseq/help/nodes.rst
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/XAS_icon.ico
+Filename: parseq-2024.5.0/parseq/help/top.rst
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/XES_dispersive_icon.ico
+Filename: parseq-2024.5.0/parseq/help/transforms.rst
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_images/XES_scan_icon.ico
+Filename: parseq-2024.5.0/parseq/help/widgets.rst
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_static/animation.js
+Filename: parseq-2024.5.0/parseq/help/__init__.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_static/thumbnail.css
+Filename: parseq-2024.5.0/parseq/help/exts/animation.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_templates/layout.html
+Filename: parseq-2024.5.0/parseq/help/_images/mickey-rtfm.gif
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/mytheme/
+Filename: parseq-2024.5.0/parseq/help/_images/parseq.ico
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/parseq/
+Filename: parseq-2024.5.0/parseq/help/_images/parseq_big.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/mytheme/static/
+Filename: parseq-2024.5.0/parseq/help/_images/pipeline-data-tree.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/mytheme/layout.html
+Filename: parseq-2024.5.0/parseq/help/_images/pipeline-file-tree.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/mytheme/theme.conf
+Filename: parseq-2024.5.0/parseq/help/_images/pipeline-fit-EXAFS.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/mytheme/static/mycss.css_t
+Filename: parseq-2024.5.0/parseq/help/_images/pipeline-graph-XAS.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/parseq/static/
+Filename: parseq-2024.5.0/parseq/help/_images/pipeline-line-props.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/parseq/layout.html
+Filename: parseq-2024.5.0/parseq/help/_images/pipeline-proj-load.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/parseq/page.html
+Filename: parseq-2024.5.0/parseq/help/_images/pipeline-proj-save.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/parseq/theme.conf
+Filename: parseq-2024.5.0/parseq/help/_images/pipeline-timing.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/parseq/static/default.css_t
+Filename: parseq-2024.5.0/parseq/help/_images/pipeline-transform-apply.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/parseq/static/math_config_win32.js
+Filename: parseq-2024.5.0/parseq/help/_images/pipeline-undo.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/help/_themes/parseq/static/utils.js
+Filename: parseq-2024.5.0/parseq/help/_images/XAS-foils.gif
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/data/
+Filename: parseq-2024.5.0/parseq/help/_static/animation.js
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/circles-rect.png
+Filename: parseq-2024.5.0/parseq/help/_static/thumbnail.css
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/circles.png
+Filename: parseq-2024.5.0/parseq/help/_templates/layout.html
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/modeltest.py
+Filename: parseq-2024.5.0/parseq/help/_themes/mytheme/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_aboutWidget.py
+Filename: parseq-2024.5.0/parseq/help/_themes/parseq/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_calibrateEnergyWidget.py
+Filename: parseq-2024.5.0/parseq/help/_themes/mytheme/static/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_columnStrings.py
+Filename: parseq-2024.5.0/parseq/help/_themes/mytheme/layout.html
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_combineSpectraWidget.py
+Filename: parseq-2024.5.0/parseq/help/_themes/mytheme/theme.conf
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_commons.py
+Filename: parseq-2024.5.0/parseq/help/_themes/mytheme/static/mycss.css_t
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_curve_shear.py
+Filename: parseq-2024.5.0/parseq/help/_themes/parseq/static/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_dataRebinWidget.py
+Filename: parseq-2024.5.0/parseq/help/_themes/parseq/layout.html
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_dataTreeModelView.py
+Filename: parseq-2024.5.0/parseq/help/_themes/parseq/page.html
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_fileDialog.py
+Filename: parseq-2024.5.0/parseq/help/_themes/parseq/theme.conf
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_fileTreeModelView.py
+Filename: parseq-2024.5.0/parseq/help/_themes/parseq/static/default.css_t
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_fit.py
+Filename: parseq-2024.5.0/parseq/help/_themes/parseq/static/math_config_win32.js
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_flowLayout.py
+Filename: parseq-2024.5.0/parseq/help/_themes/parseq/static/utils.js
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_hdf5.py
+Filename: parseq-2024.5.0/parseq/tests/data/
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_mainWindow.py
+Filename: parseq-2024.5.0/parseq/tests/circles-rect.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_node.py
+Filename: parseq-2024.5.0/parseq/tests/circles.png
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_nodeWidget.py
+Filename: parseq-2024.5.0/parseq/tests/modeltest.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py
+Filename: parseq-2024.5.0/parseq/tests/test_aboutWidget.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_plotInteractiveImageSingleROI.py
+Filename: parseq-2024.5.0/parseq/tests/test_calibrateEnergyWidget.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_plotOptions.py
+Filename: parseq-2024.5.0/parseq/tests/test_columnStrings.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_QSortFilterProxyModel.py
+Filename: parseq-2024.5.0/parseq/tests/test_combineSpectraWidget.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_ROI.py
+Filename: parseq-2024.5.0/parseq/tests/test_commons.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_slice.py
+Filename: parseq-2024.5.0/parseq/tests/test_curve_shear.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/test_stateButtons.py
+Filename: parseq-2024.5.0/parseq/tests/test_dataCorrection.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/__init__.py
+Filename: parseq-2024.5.0/parseq/tests/test_dataRebinWidget.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/data/cu-ref-mix.res
+Filename: parseq-2024.5.0/parseq/tests/test_dataTreeModelView.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/data/pb-ref-mix.res
+Filename: parseq-2024.5.0/parseq/tests/test_fileDialog.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/tests/data/zn-ref-mix.res
+Filename: parseq-2024.5.0/parseq/tests/test_fileTreeModelView.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/third_party/data/
+Filename: parseq-2024.5.0/parseq/tests/test_fit.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/third_party/XAFSmass.py
+Filename: parseq-2024.5.0/parseq/tests/test_fit_EXAFS.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/third_party/xrt.py
+Filename: parseq-2024.5.0/parseq/tests/test_flowLayout.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/third_party/__init__.py
+Filename: parseq-2024.5.0/parseq/tests/test_hdf5.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/third_party/data/Energies.txt
+Filename: parseq-2024.5.0/parseq/tests/test_mainWindow.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/utils/format.py
+Filename: parseq-2024.5.0/parseq/tests/test_node.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/utils/ft.py
+Filename: parseq-2024.5.0/parseq/tests/test_nodeWidget.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/utils/h5reduce.py
+Filename: parseq-2024.5.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/utils/math.py
+Filename: parseq-2024.5.0/parseq/tests/test_plotInteractiveImageSingleROI.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq/utils/__init__.py
+Filename: parseq-2024.5.0/parseq/tests/test_plotOptions.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq.egg-info/dependency_links.txt
+Filename: parseq-2024.5.0/parseq/tests/test_QSortFilterProxyModel.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq.egg-info/not-zip-safe
+Filename: parseq-2024.5.0/parseq/tests/test_ROI.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq.egg-info/PKG-INFO
+Filename: parseq-2024.5.0/parseq/tests/test_slice.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq.egg-info/requires.txt
+Filename: parseq-2024.5.0/parseq/tests/test_stateButtons.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq.egg-info/SOURCES.txt
+Filename: parseq-2024.5.0/parseq/tests/__init__.py
 Comment: 
 
-Filename: parseq-2023.5.0/parseq.egg-info/top_level.txt
+Filename: parseq-2024.5.0/parseq/tests/data/BFT-Cu-foil_EXAFS_23070.txt.gz
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/tests/data/Ce-CeRu2.bft
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/tests/data/cu-ref-mix.res
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/tests/data/fitTestEXAFS.h5
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/tests/data/pb-ref-mix.res
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/tests/data/Ru-CeRu2.bft
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/tests/data/zn-ref-mix.res
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/third_party/data/
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/third_party/XAFSmass.py
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/third_party/xrt.py
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/third_party/__init__.py
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/third_party/data/Energies.txt
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/utils/constants.py
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/utils/format.py
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/utils/ft.py
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/utils/h5reduce.py
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/utils/math.py
+Comment: 
+
+Filename: parseq-2024.5.0/parseq/utils/__init__.py
+Comment: 
+
+Filename: parseq-2024.5.0/parseq.egg-info/dependency_links.txt
+Comment: 
+
+Filename: parseq-2024.5.0/parseq.egg-info/not-zip-safe
+Comment: 
+
+Filename: parseq-2024.5.0/parseq.egg-info/PKG-INFO
+Comment: 
+
+Filename: parseq-2024.5.0/parseq.egg-info/requires.txt
+Comment: 
+
+Filename: parseq-2024.5.0/parseq.egg-info/SOURCES.txt
+Comment: 
+
+Filename: parseq-2024.5.0/parseq.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `parseq-2023.5.0/LICENSE` & `parseq-2024.5.0/LICENSE`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/PKG-INFO` & `parseq-2024.5.0/parseq/description.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,33 @@
-Metadata-Version: 2.1
-Name: parseq
-Version: 2023.5.0
-Summary: ParSeq is a python software library for Parallel execution of Sequential data analysis.
-Home-page: http://parseq.readthedocs.io
-Author: Konstantin Klementiev
-Author-email: konstantin.klementiev@gmail.com
-License: MIT License
-Project-URL: Source, https://github.com/kklmn/ParSeq
-Keywords: data-analysis pipeline framework gui synchrotron spectroscopy
-Platform: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: User Interfaces
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
+# -*- coding: utf-8 -*-
+r"""
 Package ParSeq is a python software library for **Par**\ allel execution of
 **Seq**\ uential data analysis. It implements a general analysis framework that
 consists of transformation nodes -- intermediate stops along the data pipeline
-to visualize data, display status and provide user input -- and transformations
-that connect the nodes. It provides an adjustable data model (supports
-grouping, renaming, moving and drag-and-drop), tunable data format definitions,
-plotters for 1D, 2D and 3D data, cross-data analysis routines and flexible
-widget work space suitable for single- and multi-screen computers. It also
-defines a structure to implement particular analysis pipelines as relatively
-lightweight Python packages.
+for data visualization, cross-data operations (e.g. taking average), providing
+user input and displaying status -- and transformations that connect the nodes.
+
+It provides an adjustable data tree model (supports grouping, renaming, moving
+and drag-and-drop arrangement), tunable data format definitions, plotters for
+1D, 2D and 3D data, cross-data analysis routines and flexible widget work space
+suitable for single- and multi-screen computers. It also defines a structure to
+implement particular analysis pipelines as lightweight Python packages.
 
 ParSeq is intended for synchrotron based techniques, first of all spectroscopy.
 
+A screenshot of ParSeq-XAS (an EXAFS analysis pipeline) as an application
+example:
+
+.. image:: _images/XAS-foils.gif
+   :scale: 50 %
+
 Main features
 -------------
 
--  ParSeq allows creating analysis pipelines as lightweight modules.
+-  ParSeq allows creating analysis pipelines as lightweight Python packages.
 
 -  Flexible use of screen area by detachable/dockable transformation nodes
    (parts of analysis pipeline).
 
 -  Two ways of acting from GUI onto multiple data: (a) simultaneous work with
    multiply selected data and (b) copying a specific parameter or a group of
    parameters from active data items to later selected data items.
@@ -53,52 +38,57 @@
    pipeline.
 
 -  Creation of cross-data combinations (e.g. averaging, RMS or PCA) and their
    propagation downstream the pipeline together with the parental data. The
    possibility of termination of the parental data at any selected downstream
    node.
 
+-  General data correction routines for 1D data: range deletion, scaling,
+   replacement by a spline and jump correction.
+
 -  Parallel execution of data transformations with multiprocessing or
    multithreading (can be opted by the pipeline application).
 
 -  Optional curve fitting solvers, also executed in parallel for multiple data
    items.
 
 -  Informative error handling that provides alerts and stack traceback -- the
    type and location of the occurred error.
 
+-  Optional time profiling of the pipeline, as controlled by a command-line
+   argument.
+
 -  Export of the workflow into a project file. Export of data into various data
    formats with accompanied Python scripts that visualize the exported data for
    the user to tune their publication plots.
 
 -  ParSeq understands container files (presently only hdf5) and adds them to
    the system file tree as subfolders. The file tree, including hdf5
    containers, is lazy loaded thus enabling big data collections.
 
 -  A web viewer widget near each analysis widget displays help pages generated
    from the analysis widget doc strings. The help pages are built by Sphinx at
    the startup time.
 
--  The pipeline can be operated via scripts or GUI.
+-  The pipeline can be operated by the GUI or from a Python script without GUI.
 
 -  Optional automatic loading of new data during a measurement time.
 
 The mechanisms for creating nodes, transformations and curve fitting solvers,
 connecting them together and creating Qt widgets for the transformations and
 and curve fits are exemplified by separately installed analysis packages:
 
-- `ParSeq-XES-scan <https://github.com/kklmn/ParSeq-XES-scan>`_
-- `ParSeq-XES-dispersive <https://github.com/kklmn/ParSeq-XES-dispersive>`_
 - `ParSeq-XAS <https://github.com/kklmn/ParSeq-XAS>`_
+- `ParSeq-XES-scan <https://github.com/kklmn/ParSeq-XES-scan>`_
 
 Dependencies
 ------------
 
-- `silx <https://github.com/silx-kit/silx>`_ -- for plotting and Qt imports
-- `sphinx <https://github.com/sphinx-doc/sphinx>`_ -- for building html documentation
+- `silx <https://github.com/silx-kit/silx>`_ -- plotting, hdf5 handling, Qt
+- `sphinx <https://github.com/sphinx-doc/sphinx>`_ -- building documentation
 
 Launch an example
 -----------------
 
 Either install ParSeq and a ParSeq pipeline application by their installers to
 the standard location or put them to any folder in their respective folders
 (``parseq`` and e.g. ``parseq_XES_scan``) and run the ``*_start.py`` module of
@@ -107,7 +97,9 @@
 the starting command line.
 
 Hosting and contact
 -------------------
 
 The ParSeq project is hosted on `GitHub <https://github.com/kklmn/ParSeq>`_.
 Please use the project's Issues tab to get help or report an issue.
+
+"""
```

## Comparing `parseq-2023.5.0/setup.py` & `parseq-2024.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             '_themes/*/*.*', '_themes/*/*/*.*', 'exts/*.*'],
         'parseq.tests': ['*.png', 'data/*.*'],
         'parseq.third_party': ['data/*.*'],
         },
     install_requires=['numpy>=1.8.0', 'scipy>=0.17.0', 'matplotlib>=2.0.0',
                       'sphinx>=1.6.2', 'sphinxcontrib-jquery', 'autopep8',
                       'h5py', 'silx>=1.1.0', 'hdf5plugin', 'psutil',
-                      'docutils', 'distro'],
+                      'pyqtwebengine', 'docutils', 'distro', 'colorama'],
     classifiers=['Development Status :: 5 - Production/Stable',
                  'Intended Audience :: Science/Research',
                  'Natural Language :: English',
                  'Operating System :: OS Independent',
                  'Programming Language :: Python',
                  'License :: OSI Approved :: MIT License',
                  'Intended Audience :: Science/Research',
```

## Comparing `parseq-2023.5.0/parseq/description.py` & `parseq-2024.5.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,69 @@
-# -*- coding: utf-8 -*-
-r"""
+Metadata-Version: 2.1
+Name: parseq
+Version: 2024.5.0
+Summary: ParSeq is a python software library for Parallel execution of Sequential data analysis.
+Home-page: http://parseq.readthedocs.io
+Author: Konstantin Klementiev
+Author-email: konstantin.klementiev@gmail.com
+License: MIT License
+Project-URL: Source, https://github.com/kklmn/ParSeq
+Keywords: data-analysis pipeline framework gui synchrotron spectroscopy
+Platform: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: User Interfaces
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy>=1.8.0
+Requires-Dist: scipy>=0.17.0
+Requires-Dist: matplotlib>=2.0.0
+Requires-Dist: sphinx>=1.6.2
+Requires-Dist: sphinxcontrib-jquery
+Requires-Dist: autopep8
+Requires-Dist: h5py
+Requires-Dist: silx>=1.1.0
+Requires-Dist: hdf5plugin
+Requires-Dist: psutil
+Requires-Dist: pyqtwebengine
+Requires-Dist: docutils
+Requires-Dist: distro
+Requires-Dist: colorama
+
 Package ParSeq is a python software library for **Par**\ allel execution of
 **Seq**\ uential data analysis. It implements a general analysis framework that
 consists of transformation nodes -- intermediate stops along the data pipeline
-to visualize data, display status and provide user input -- and transformations
-that connect the nodes. It provides an adjustable data model (supports
-grouping, renaming, moving and drag-and-drop), tunable data format definitions,
-plotters for 1D, 2D and 3D data, cross-data analysis routines and flexible
-widget work space suitable for single- and multi-screen computers. It also
-defines a structure to implement particular analysis pipelines as relatively
-lightweight Python packages.
+for data visualization, cross-data operations (e.g. taking average), providing
+user input and displaying status -- and transformations that connect the nodes.
+
+It provides an adjustable data tree model (supports grouping, renaming, moving
+and drag-and-drop arrangement), tunable data format definitions, plotters for
+1D, 2D and 3D data, cross-data analysis routines and flexible widget work space
+suitable for single- and multi-screen computers. It also defines a structure to
+implement particular analysis pipelines as lightweight Python packages.
 
 ParSeq is intended for synchrotron based techniques, first of all spectroscopy.
 
-A screenshot of a scanning XES analysis pipeline as an application example:
+A screenshot of ParSeq-XAS (an EXAFS analysis pipeline) as an application
+example:
 
-.. imagezoom:: _images/node1.png
+.. image:: _images/XAS-foils.gif
    :scale: 50 %
 
 Main features
 -------------
 
--  ParSeq allows creating analysis pipelines as lightweight modules.
+-  ParSeq allows creating analysis pipelines as lightweight Python packages.
 
 -  Flexible use of screen area by detachable/dockable transformation nodes
    (parts of analysis pipeline).
 
 -  Two ways of acting from GUI onto multiple data: (a) simultaneous work with
    multiply selected data and (b) copying a specific parameter or a group of
    parameters from active data items to later selected data items.
@@ -36,52 +74,57 @@
    pipeline.
 
 -  Creation of cross-data combinations (e.g. averaging, RMS or PCA) and their
    propagation downstream the pipeline together with the parental data. The
    possibility of termination of the parental data at any selected downstream
    node.
 
+-  General data correction routines for 1D data: range deletion, scaling,
+   replacement by a spline and jump correction.
+
 -  Parallel execution of data transformations with multiprocessing or
    multithreading (can be opted by the pipeline application).
 
 -  Optional curve fitting solvers, also executed in parallel for multiple data
    items.
 
 -  Informative error handling that provides alerts and stack traceback -- the
    type and location of the occurred error.
 
+-  Optional time profiling of the pipeline, as controlled by a command-line
+   argument.
+
 -  Export of the workflow into a project file. Export of data into various data
    formats with accompanied Python scripts that visualize the exported data for
    the user to tune their publication plots.
 
 -  ParSeq understands container files (presently only hdf5) and adds them to
    the system file tree as subfolders. The file tree, including hdf5
    containers, is lazy loaded thus enabling big data collections.
 
 -  A web viewer widget near each analysis widget displays help pages generated
    from the analysis widget doc strings. The help pages are built by Sphinx at
    the startup time.
 
--  The pipeline can be operated via scripts or GUI.
+-  The pipeline can be operated by the GUI or from a Python script without GUI.
 
 -  Optional automatic loading of new data during a measurement time.
 
 The mechanisms for creating nodes, transformations and curve fitting solvers,
 connecting them together and creating Qt widgets for the transformations and
 and curve fits are exemplified by separately installed analysis packages:
 
-- `ParSeq-XES-scan <https://github.com/kklmn/ParSeq-XES-scan>`_
-- `ParSeq-XES-dispersive <https://github.com/kklmn/ParSeq-XES-dispersive>`_
 - `ParSeq-XAS <https://github.com/kklmn/ParSeq-XAS>`_
+- `ParSeq-XES-scan <https://github.com/kklmn/ParSeq-XES-scan>`_
 
 Dependencies
 ------------
 
-- `silx <https://github.com/silx-kit/silx>`_ -- for plotting and Qt imports
-- `sphinx <https://github.com/sphinx-doc/sphinx>`_ -- for building html documentation
+- `silx <https://github.com/silx-kit/silx>`_ -- plotting, hdf5 handling, Qt
+- `sphinx <https://github.com/sphinx-doc/sphinx>`_ -- building documentation
 
 Launch an example
 -----------------
 
 Either install ParSeq and a ParSeq pipeline application by their installers to
 the standard location or put them to any folder in their respective folders
 (``parseq`` and e.g. ``parseq_XES_scan``) and run the ``*_start.py`` module of
@@ -90,9 +133,7 @@
 the starting command line.
 
 Hosting and contact
 -------------------
 
 The ParSeq project is hosted on `GitHub <https://github.com/kklmn/ParSeq>`_.
 Please use the project's Issues tab to get help or report an issue.
-
-"""
```

## Comparing `parseq-2023.5.0/parseq/core/commons.py` & `parseq-2024.5.0/parseq/core/commons.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,20 @@
 MIME_TYPE_HDF5 = 'parseq-hdf5-model-items'
 
 (DATA_COLUMN_FILE, DATA_DATASET, DATA_COMBINATION, DATA_FUNCTION, DATA_GROUP,
  DATA_BRANCH) = range(6)
 COMBINE_NONE, COMBINE_AVE, COMBINE_SUM, COMBINE_PCA, COMBINE_RMS = range(5)
 combineNames = '', 'ave', 'sum', 'PCA', 'RMS'
 
-(DATA_STATE_GOOD, DATA_STATE_BAD, DATA_STATE_UNDEFINED, DATA_STATE_NOTFOUND,
- DATA_STATE_MATHERROR) = 1, 0, -1, -2, -3
+DATA_STATE_GOOD = 1
+DATA_STATE_BAD = 0
+DATA_STATE_UNDEFINED = -1
+DATA_STATE_NOTFOUND = -2
+DATA_STATE_MATHERROR = -3
+DATA_STATE_MARKED_FOR_DELETION = -4
 
 
 def expandDotAttr(attr):
     """ *attr* is str or list of str, each str can have a dot notation"""
     if not isinstance(attr, (tuple, list)):
         res = attr.split(".")
         try:
@@ -201,15 +205,15 @@
 # -> "(2..5, 7..9, 11, 15..18)"
 #
 #a = ['03', '02', '04', '05']
 #print(make_int_ranges(a))
 # -> "(02..05)"
 
 
-def get_header(fname, readkwargs):
+def get_header(fname, readkwargs, searchAllLines=False):
     skipUntil = readkwargs.pop('lastSkipRowContains', '')
     headerLen = -1
     if 'skiprows' not in readkwargs:
         if skipUntil:
             with open(fname, 'r', encoding="utf-8") as f:
                 for il, line in enumerate(f):
                     if skipUntil in line:
@@ -217,21 +221,24 @@
                     if il == MAX_HEADER_LINES:
                         break
             if headerLen >= 0:
                 readkwargs['skiprows'] = headerLen + 1
     else:
         headerLen = readkwargs['skiprows']
     header = []
-    with open(fname, 'r', encoding="utf-8") as f:
-        for il, line in enumerate(f):
-            if il == MAX_HEADER_LINES:
-                break
-            if ((headerLen >= 0) and (il <= headerLen)) or \
-                    line.startswith('#'):
-                header.append(line)
+    try:
+        with open(fname, 'r', encoding="utf-8") as f:
+            for il, line in enumerate(f):
+                if il == MAX_HEADER_LINES and not searchAllLines:
+                    break
+                if ((headerLen >= 0) and (il <= headerLen)) or \
+                        line.startswith('#'):
+                    header.append(line)
+    except FileNotFoundError as e:
+        print('core.commons.get_header():', e)
     return header
 
 
 def parse_slice_str(slice_str):
     parts = slice_str.split(':')
     if len(parts) == 1:
         try:
```

## Comparing `parseq-2023.5.0/parseq/core/config.py` & `parseq-2024.5.0/parseq/core/config.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/core/logger.py` & `parseq-2024.5.0/parseq/core/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 # -*- coding: utf-8 -*-
 __author__ = "Konstantin Klementiev"
 __date__ = "18 Feb 2023"
 # !!! SEE CODERULES.TXT !!!
 
 import time
 from functools import wraps
+try:
+    import colorama
+    colorama.init(autoreset=True)
+    green = colorama.Fore.GREEN
+    red = colorama.Fore.RED
+    reset = colorama.Fore.RESET
+except ImportError:
+    colorama = None
+    green = red = reset = ''
 
 from . import singletons as csi
 
+longTime = 1.
+
 
 def logger(minLevel=1, printClass=False, attrs=None):
     """Printed if csi.DEBUG_LEVEL > *minLevel*.
        *attrs*: a list of (iarg[int], attr[str]) pairs to print out.
     """
     def decorate(func):
         @wraps(func)
@@ -27,11 +38,14 @@
                         except Exception as e:
                             out += f", {e}"
                 print(f"enter {out}")
                 tstart = time.time()
             res = func(*args, **kwargs)
             if csi.DEBUG_LEVEL > minLevel:
                 dt = time.time() - tstart
-                print(f"exit {out} in {dt:.5f}s")
+                mark = green if dt < longTime else red
+                print(f"exit {out} in {mark}{dt:.6f}{reset}s")
+                if 'worker' in out:
+                    print()
             return res
         return wrapper
     return decorate
```

## Comparing `parseq-2023.5.0/parseq/core/nodes.py` & `parseq-2024.5.0/parseq/core/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
         *role*: str, default = '1D' (not plotted)
             The array's role. Can be 'x', 'y', 'yleft', 'yright', 'z' or '1D'
             for 1D arrays (one and only one x-axis array is required), '2D' for
             2D plots and '3D' for stacked 2D images. '0D' values are listed in
             the data tree. 'optional' array is not required in data files and
             can be used as an auxiliary. Unless with a '0D' role, each array
-            will appear in `data location` dialog to define its location.
+            will appear in `data format` dialog (resides under the file tree)
+            to define its location.
 
         *raw*: str, default = array name
             Can define an intermediate array at the pipeline head when the main
             array (the key in *arrays*) is supposed to be obtained by an after
             load transformation. The plotted array is still the main one. The
             idea of having a *raw* version of an array is in the possibility of
             creating a transformation that not only begins at the first node
@@ -66,17 +67,20 @@
 
         *plotUnit*: str, default = *qUnit*
             Attached to the plot label in parentheses. For example,
             for Å^-1: *qUnit* = u'Å\u207B\u00B9' and *plotUnit* = r'Å$^{-1}$'.
 
         *plotParams*: dict, default is `{}` that assumes thin solid lines
             Default parameters for plotting. Can have the following keys:
-            *linewidth* (or *lw*), *style*, *symbol* and *symbolsize*. Note
-            that color is set for a data item and is equal across the nodes, so
-            it is set not here.
+            *linewidth* (or *lw*), *style*, *symbol* and *symbolsize*.
+
+            .. note::
+                Color is set for a data item as its attribute and is equal
+                for all 1D curves of the data item across the nodes, so it is
+                set not here.
 
     *checkShapes*: list of str
         Can be useful at data file reading. If given, the list contains keys of
         *arrays*. The corresponding arrays will be checked for equal shape. The
         names of multidimensional arrays can be ended by a slice. Example:
         `checkShapes = ['theta', 'i0', 'xes3D[0]']`.
 
@@ -188,14 +192,17 @@
         return ans
 
     def get_prop(self, arrayName, prop):
         u"""Returns the property *prop* for a given array name defined in this
         node. This method can be useful in creating the GUI part of a
         transformation node."""
 
+        if prop in ('key', 'name'):
+            return arrayName
+
         if prop not in self.properties:
             raise ValueError("unknown prop {0} in arrays['{1}']".format(
                 prop, arrayName))
 
         if prop == 'qLabel':
             res = self.arrays[arrayName].get(prop, arrayName)
             return res.decode("utf-8") if isOldPyton else res
```

## Comparing `parseq-2023.5.0/parseq/core/plotExport.py` & `parseq-2024.5.0/parseq/core/plotExport.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,33 +59,35 @@
         if h5file is not None:
             h5file.close()
     return curves  # end read1D
 
 
 def plot1Dmpl(nodeData):
     saveType = nodeData[0]
-    fig = plt.figure()
+    fig = plt.figure(figsize=(7, 5))
     fig.suptitle(nodeData[1] + ' ' + saveType)
     axl = fig.add_subplot(111)
     axl.set_xmargin(0.)
     axl.set_ymargin(0.)
     axl.set_xlabel(nodeData[3][0])
     axl.set_ylabel(nodeData[3][1])
     if nodeData[3][2]:
         axr = axl.twinx()
         axr.set_ylabel(nodeData[3][2])
         axr.set_xmargin(0.)
         axr.set_ymargin(0.)
 
     savedColumns = nodeData[4]
-    for fname, props in savedColumns.items():
+    # colors = [f'C{i%9}' for i in range(len(savedColumns))]  # custom colors
+    for icurve, (fname, props) in enumerate(savedColumns.items()):
         curves = read1D(saveType, fname, props)
         if len(props) > 3:
             yprops = props[3]
-            clr = props[1]
+            clr = props[1]  # same color as in ParSeq wanted
+            # clr = colors[icurve]  # custom color wanted
 
         for curve in curves:
             x, ys, headers = curve
             for y, header in zip(ys, headers):
                 try:
                     kw = dict(yprops[header])
                 except KeyError:
@@ -94,19 +96,28 @@
                 yaxis = kw.pop('yaxis', 'left')
                 if 'symbolsize' in kw:
                     ms = kw.pop('symbolsize')
                     kw['markersize'] = ms
                 if 'symbol' in kw:
                     m = kw.pop('symbol')
                     kw['marker'] = m
-                lbl = props[0]  # + '.' + header
+                lbl = props[0]
+                if len(headers) > 1:
+                    lbl += '.' + header
                 ax = axl if yaxis.startswith('l') else axr
                 ax.plot(x, y, color=clr, label=lbl, **kw)
+
     ax.legend()
-    # fig.savefig('test.png')
+    # ax.legend([(l1, l2) for l1, l2 in zip(lines[::2], lines[1::2])],
+    #           usedLabels, handler_map={tuple: NLineObjectsHandler()})
+
+    # if 'eV' in nodeData[3][0]:
+    #     ax.set_xlim(5950, 6125)  # set energy limits for XANES
+
+    fig.savefig('{0}_{1}.png'.format(nodeData[1], saveType))
     # end plot1Dmpl
 
 
 def plot1Dsilx(nodeData):
     from silx.gui.plot import Plot1D
 
     saveType = nodeData[0]
@@ -130,21 +141,27 @@
                 try:
                     kw = dict(yprops[header])
                 except KeyError:
                     kw = {'yaxis': 'left'}
                     clr = 'gray'
                 symbolsize = kw.pop('symbolsize', 2)
                 symbol = kw.get('symbol', None)
-                lbl = props[0]  # + '.' + header
+                lbl = props[0]
+                if len(headers) > 1:
+                    lbl += '.' + header
                 plot.addCurve(x, y, color=clr, legend=lbl, **kw)
                 if symbol is not None:
                     curve = plot.getCurve(lbl)
                     if curve is not None:
                         curve.setSymbolSize(symbolsize)
 
+    # # This is how one can set energy limits for XANES:
+    # if 'eV' in nodeData[3][0]:
+    #     plot.getXAxis().setLimits(5950, 6125)
+
     plot.show()
     return plot  # end plot1Dsilx
 
 
 def read2D(saveType, fname, props):
     maps = []
     if saveType.endswith(('json', 'pickle', 'h5')):
@@ -267,23 +284,24 @@
     plotGrp = h5file['plots']
     plots = []
     for key in plotGrp.keys():
         ndim = plotGrp[key]['ndim'][()]
         axes = eval(plotGrp[key]['axes'][()])
         curves = eval(plotGrp[key]['plots'][()])
         plots.append([path, key, ndim, axes, curves])
-    return(plots)  # end getPlotsFromHDF5
+    return plots  # end getPlotsFromHDF5
 
 
 def plotSavedData(plots, lib='mpl'):
     global widgets
     widgets = []
     for nodeData in plots:
         ndim = nodeData[2]
-        plotFunc = globals()['plot{0}D{1}'.format(ndim, lib)]
+        plotFuncName = 'plot{0}D{1}'.format(ndim, lib)  # e.g. plot1Dmpl
+        plotFunc = globals()[plotFuncName]
         widgets.append(plotFunc(nodeData))  # to keep references to silx polots
     if lib == 'mpl':
         plt.show()  # end plotSavedData
 
 
 if __name__ == '__main__':
     h5name = r'c:\ParSeq\Scripts\aaa.h5'
```

## Comparing `parseq-2023.5.0/parseq/core/save_restore.py` & `parseq-2024.5.0/parseq/core/save_restore.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 import os
 import numpy as np
 import pickle
 import json
 import autopep8
 
-import hdf5plugin  # needed to prevent h5py's "OSError: Can't read data"
+os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"  # to work with external links
+# import hdf5plugin  # needed to prevent h5py's "OSError: Can't read data"
 import h5py
 
 from ..core import config
 from ..core import singletons as csi
 from ..core import spectra as csp
 from ..core import transforms as ctr
 from ..gui import gcommons as gco
@@ -53,27 +54,37 @@
         root.color2 = config.get(configProject, 'Root', 'color2', 'b')
     elif root.colorPolicy == gco.COLOR_POLICY_INDIVIDUAL:
         root.color = config.get(configProject, 'Root', 'color', 'm')
     root.colorAutoUpdate = config.get(
         configProject, 'Root', 'colorAutoUpdate',
         csp.DEFAULT_COLOR_AUTO_UPDATE)
 
+    # cwd = os.getcwd()
     os.chdir(os.path.dirname(fname))
     if csi.model is not None:
         csi.model.importData(dataTree, configData=configProject)
     else:
         items = root.insert_data(dataTree, configData=configProject)
         ctr.connect_combined(items, root)
         ctr.run_transforms(items, root)
+    # os.chdir(cwd)  # don't! This breaks file list update by data selection
 
 
 def save_project(fname, save_perspective=None):
     configProject = config.ConfigParser(allow_no_value=True)
     configProject.optionxform = str  # makes it case sensitive
 
+    config.put(
+        configProject, 'ParSeq Application', 'pipelineName', csi.pipelineName)
+    config.put(configProject, 'ParSeq Application', 'appPath', csi.appPath)
+    config.put(
+        configProject, 'ParSeq Application', 'appVersion', csi.appVersion)
+    config.put(
+        configProject, 'ParSeq Application', 'appSynopsis', csi.appSynopsis)
+
     root = csi.dataRootItem
     config.put(configProject, 'Root', 'tree', repr(root))
     config.put(configProject, 'Root', 'groups', str(len(root.get_groups())))
     config.put(configProject, 'Root', 'items', str(len(root.get_items())))
 
     config.put(configProject, 'Root', 'colorPolicy',
                gco.COLOR_POLICY_NAMES[root.colorPolicy])
@@ -109,27 +120,54 @@
             if node.plotDimension == 1:
                 header = [node.plotXArray] + [y for y in node.plotYArrays]
             else:
                 continue
 
             curves = {}
             for it in csi.selectedItems:
-                dataToSave = [getattr(it, arr) for arr in header]
+                dataToSave = []
+                try:
+                    x = getattr(it, node.plotXArray)
+                except AttributeError:
+                    continue
+                for aN in node.arrays:
+                    d = getattr(it, aN)
+                    if ((aN in node.plotYArrays) and
+                        hasattr(node.widget.transformWidget,
+                                'extraPlotTransform')):
+                        x, d = \
+                            node.widget.transformWidget.extraPlotTransform(
+                                it, node.plotXArray, x, aN, d)
+                    dataToSave.append(d)
                 dataToSave = [d for d in dataToSave if d is not None]
+
+                headerAll = list(header)
+                plotPropsAll = it.plotProps[node.name]
+                for fit in csi.fits.values():
+                    if fit.node is node:
+                        fitAttrName = fit.dataAttrs['fit']
+                        try:
+                            fity = getattr(it, fitAttrName)
+                            dataToSave.append(fity)
+                            headerAll.append(fitAttrName)
+                            plotPropsAll[fitAttrName] = fit.plotParams['fit']
+                        except AttributeError:
+                            continue
+
                 nname = nodeName.translate(chars2removeMap)
                 dname = it.alias.translate(chars2removeMap)
                 sname = u'{0}-{1}-{2}'.format(iNode+1, nname, dname)
                 if 'txt' in saveTypes:
                     np.savetxt(sname+'.txt', np.column_stack(dataToSave),
-                               fmt='%.12g', header=' '.join(header))
+                               fmt='%.12g', header=' '.join(headerAll))
                 if 'txt.gz' in saveTypes:
                     np.savetxt(sname+'.txt.gz', np.column_stack(dataToSave),
-                               fmt='%.12g', header=' '.join(header))
-                curves[sname] = [it.alias, it.color, header,
-                                 it.plotProps[node.name]]
+                               fmt='%.12g', header=' '.join(headerAll))
+
+                curves[sname] = [it.alias, it.color, headerAll, plotPropsAll]
 
                 for iG, aG in enumerate(node.auxArrays):
                     dataAux, headerAux = [], []
                     for yN in aG:
                         try:
                             dataAux.append(getattr(it, yN))
                         except AttributeError:
@@ -142,14 +180,15 @@
                     if 'txt' in saveTypes:
                         np.savetxt(sname+'.txt', np.column_stack(dataAux),
                                    fmt='%.12g', header=' '.join(headerAux))
                     if 'txt.gz' in saveTypes:
                         np.savetxt(sname+'.txt.gz', np.column_stack(dataAux),
                                    fmt='%.12g', header=' '.join(headerAux))
                     curves[sname] = [it.alias, it.color, headerAux]
+
             if 'txt' in saveTypes:
                 plots.append(['txt', node.name, node.plotDimension,
                               node.widget.getAxisLabels(), curves])
             if 'txt.gz' in saveTypes:
                 plots.append(['txt.gz', node.name, node.plotDimension,
                               node.widget.getAxisLabels(), curves])
 
@@ -168,25 +207,50 @@
             elif node.plotDimension == 2:
                 header = node.plot2DArray
             elif node.plotDimension == 3:
                 header = node.plot3DArray
 
             curves = {}
             for it, sname in zip(csi.selectedItems, snames):
+                if node.plotDimension == 1:
+                    try:
+                        x = getattr(it, node.plotXArray)
+                    except AttributeError:
+                        continue
                 for aN in node.arrays:
                     d = getattr(it, aN)
+                    if (node.plotDimension == 1 and
+                        (aN in node.plotYArrays) and
+                        hasattr(node.widget.transformWidget,
+                                'extraPlotTransform')):
+                        x, d = \
+                            node.widget.transformWidget.extraPlotTransform(
+                                it, node.plotXArray, x, aN, d)
                     dataToSave[it][aN] = d.tolist() if d is not None else None
                 for aN in [j for i in node.auxArrays for j in i]:
                     try:
                         d = getattr(it, aN)
                     except AttributeError:
                         continue
                     dataToSave[it][aN] = d.tolist() if d is not None else None
-                curves[sname] = [it.alias, it.color, header,
-                                 it.plotProps[node.name]]
+
+                headerAll = list(header)
+                plotPropsAll = it.plotProps[node.name]
+                for fit in csi.fits.values():
+                    if fit.node is node:
+                        fitAttrName = fit.dataAttrs['fit']
+                        try:
+                            fity = getattr(it, fitAttrName)
+                            dataToSave[it][fitAttrName] = fity.tolist()
+                            headerAll.append(fitAttrName)
+                            plotPropsAll[fitAttrName] = fit.plotParams['fit']
+                        except AttributeError:
+                            continue
+
+                curves[sname] = [it.alias, it.color, headerAll, plotPropsAll]
                 if node.auxArrays:
                     headerAux = []
                     for aG in node.auxArrays:
                         for yN in aG:
                             if not hasattr(it, yN):
                                 break
                         else:
@@ -226,26 +290,53 @@
             elif node.plotDimension == 2:
                 header = node.plot2DArray
             elif node.plotDimension == 3:
                 header = node.plot3DArray
 
             curves = {}
             for it, sname in zip(csi.selectedItems, snames):
+                if node.plotDimension == 1:
+                    try:
+                        x = getattr(it, node.plotXArray)
+                    except AttributeError:
+                        continue
                 for aN in node.arrays:
                     try:
-                        dataToSave[it][aN] = getattr(it, aN)
+                        y = getattr(it, aN)
+                        if (node.plotDimension == 1 and
+                            (aN in node.plotYArrays) and
+                            hasattr(node.widget.transformWidget,
+                                    'extraPlotTransform')):
+                            x, y = \
+                                node.widget.transformWidget.extraPlotTransform(
+                                    it, node.plotXArray, x, aN, y)
+                        dataToSave[it][aN] = y
                     except AttributeError:
                         continue
+
                 for aN in [j for i in node.auxArrays for j in i]:
                     try:
                         dataToSave[it][aN] = getattr(it, aN)
                     except AttributeError:
                         continue
-                curves[sname] = [it.alias, it.color, header,
-                                 it.plotProps[node.name]]
+
+                headerAll = list(header)
+                plotPropsAll = it.plotProps[node.name]
+                for fit in csi.fits.values():
+                    if fit.node is node:
+                        fitAttrName = fit.dataAttrs['fit']
+                        try:
+                            fity = getattr(it, fitAttrName)
+                            dataToSave[it][fitAttrName] = fity
+                            headerAll.append(fitAttrName)
+                            plotPropsAll[fitAttrName] = fit.plotParams['fit']
+                        except AttributeError:
+                            continue
+
+                curves[sname] = [it.alias, it.color, headerAll, plotPropsAll]
                 if node.auxArrays:
                     headerAux = []
                     for aG in node.auxArrays:
                         for yN in aG:
                             if not hasattr(it, yN):
                                 break
                         else:
```

## Comparing `parseq-2023.5.0/parseq/core/spectra.py` & `parseq-2024.5.0/parseq/core/spectra.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 items and groups are instances of :class:`Spectrum`.
 
 The tree model can be manipulated in a script, and the following reference
 documentation explains how. Otherwise, most typically it is used within the
 ParSeq GUI, where the tree model feeds the `model-view-controller
 <https://doc.qt.io/qt-6/model-view-programming.html>`_ software architecture of
 Qt, where the user does not have to know about the underlying objects and
-methods. See :ref:`Notes on usage of GUI <notesgui>`.
+methods.
 """
 __author__ = "Konstantin Klementiev"
-__date__ = "6 Apr 2023"
+__date__ = "22 Apr 2024"
 # !!! SEE CODERULES.TXT !!!
 
 # import sys
 import os.path as osp
 import re
 import time
 import copy
@@ -30,14 +30,15 @@
 from collections import Counter
 
 import silx.io as silx_io
 
 from . import singletons as csi
 from . import commons as cco
 from . import config
+from .correction import calc_correction
 from .logger import logger
 from ..utils.format import format_memory_size
 
 DEFAULT_COLOR_AUTO_UPDATE = False
 
 
 class TreeItem(object):
@@ -110,22 +111,23 @@
         else:
             res = ""
             if hasattr(self, 'name'):  # instance of TreeItem
                 if isinstance(self.name, type("")):
                     res = self.name
             elif hasattr(self, 'madeOf'):  # instance of Spectrum
                 if self.error is not None:
-                    return self.error
+                    res = self.error
                 elif self.beingTransformed:
-                    return '{0} is {1:.0f}% done'.format(
-                        self.beingTransformed, self.progress*100)
+                    res = '{0} is {1:.0f}% done'.format(self.beingTransformed,
+                                                        self.progress*100)
                 elif isinstance(self.madeOf, (type(""), dict, tuple, list)):
                     if isinstance(self.madeOf, type("")):
                         res = str(self.madeOf)
-                    elif isinstance(self.madeOf, (tuple, list)):
+                    elif isinstance(self.madeOf, (tuple, list)) and\
+                            'combine' in self.dataFormat:
                         what = self.dataFormat['combine']
                         if type(self.madeOf[0]) is str:
                             names = self.madeOf
                         else:
                             names = [it.alias for it in self.madeOf]
                         cNames = cco.combine_names(names)
                         res = '{0} of [{1}]'.format(
@@ -147,15 +149,21 @@
                         if self.state[node.name] == cco.DATA_STATE_NOTFOUND:
                             if res:
                                 res += '\n'
                             res += 'data not found!'
                         elif self.state[node.name] == cco.DATA_STATE_BAD:
                             if res:
                                 res += '\n'
-                            res += 'incompatible data shapes!'
+                            res += 'incompatible data shapes in {0}'.format(
+                                node.name)
+                            if hasattr(self, 'badShapes'):
+                                res += ':\n'
+                                res += ', '.join(
+                                    ['{0}={1}'.format(k, v) for
+                                     k, v in self.badShapes.items()])
                         elif self.state[node.name] == cco.DATA_STATE_GOOD:
                             try:
                                 if self.terminalNodeName is not None:
                                     res += \
                                         '\nthis data terminates at node "{0}"'\
                                         .format(self.terminalNodeName)
                                 if node.plotDimension == 1:
@@ -205,14 +213,18 @@
                                     if res:
                                         res += '\n'
                                     res += 'This data finishes at node "{0}"'\
                                         .format(self.terminalNodeName)
                             else:
                                 res += 'This node is out of the pipeline'\
                                     ' for this data'
+                        elif self.state[node.name] == cco.DATA_STATE_MATHERROR:
+                            res += '\nSee the error message in `metadata` '\
+                                'widget'
+
             return res
 
     def data(self, column):
         leadingColumns = len(csi.modelLeadingColumns)
         if column < leadingColumns:
             if column == 0:
                 return self.alias
@@ -327,24 +339,38 @@
         if hasattr(self, 'alias'):
             alias = self.alias
         elif hasattr(self, 'madeOf'):
             alias = self.madeOf
         elif hasattr(self, 'name'):
             alias = self.name
 
-        if isinstance(data, str):
+        if isinstance(data, (list, tuple)) and \
+                'concatenate' in kwargs and kwargs['concatenate']:
             item = self.insert_item(data, insertAt, **kwargs)
             if item not in items:  # inclusion check that keeps the order
                 items.append(item)
+        elif isinstance(data, str):
+            item = self.insert_item(data, insertAt, **kwargs)
+            if item.state[item.originNodeName] == \
+                    cco.DATA_STATE_MARKED_FOR_DELETION:
+                item.remove_from_parent()
+            else:
+                if item not in items:  # inclusion check that keeps the order
+                    items.append(item)
         elif isinstance(data, (list, tuple)):
             si = self
             for subdata in data:
                 if isinstance(subdata, str):
                     si = self.insert_item(subdata, insertAt, **kwargs)
-                    subItems = [si]
+                    if si.state[si.originNodeName] == \
+                            cco.DATA_STATE_MARKED_FOR_DELETION:
+                        si.remove_from_parent()
+                        subItems = []
+                    else:
+                        subItems = [si]
                 elif isinstance(subdata, (list, tuple)):
                     if si in items:
                         items.remove(si)
                     subItems = si.insert_data(subdata, **kwargs)  # no insertAt
                 else:
                     raise ValueError(
                         "data in '{0}' must be a sequence or a string, not {1}"
@@ -354,17 +380,17 @@
             raise ValueError(
                 "data in {0} must be a sequence or a string, not {1}"
                 " of type {2}".format(alias, data, type(data)))
 
         csi.recentlyLoadedItems = list(items)
         csi.allLoadedItems[:] = []
         csi.allLoadedItems.extend(csi.dataRootItem.get_items())
-        if len(csi.selectedItems) == 0:
-            if len(csi.allLoadedItems) == 0:
-                raise ValueError("No valid data added")
+        # if len(csi.selectedItems) == 0:
+        #     if len(csi.allLoadedItems) == 0:
+        #         raise ValueError("No valid data added")
         csi.selectedItems = list(items)
         csi.selectedTopItems = list(items)
 
         shouldMakeColor = len(self.childItems) > 0 and csi.withGUI
         if shouldMakeColor:
             self.init_colors(self.childItems)
         return items
@@ -373,14 +399,16 @@
         from ..gui import gcommons as gco  # only needed with gui
         if not hasattr(self, 'colorAutoUpdate'):
             return
         citems = self.childItems if self.colorAutoUpdate else items
         if citems is None:
             return
 
+        if not hasattr(self, 'colorPolicy'):
+            self.colorPolicy = gco.COLOR_POLICY_GRADIENT
         if self.colorPolicy == gco.COLOR_POLICY_GRADIENT:
             colors = gco.makeGradientCollection(
                 self.color1, self.color2, len(citems))
         for i, item in enumerate(citems):
             if hasattr(item, 'colorIndividual'):
                 item.color = item.colorIndividual
                 continue
@@ -471,15 +499,15 @@
                 Controls the way the *transformParams* of the Spectrum are
                 initialized: If False, they are copied from *defaultParams* of
                 all transforms. If True, they are copied from the first
                 selected spectrum when at least one is selected or otherwise
                 from the ini file.
         """
 
-        assert len(csi.nodes) > 0, "A data pipeline must be first created."
+        assert len(csi.nodes) > 0, "A data pipeline must first be created."
         self.madeOf = madeOf
         self.parentItem = parentItem
         self.childItems = []
         self.branch = None  # can be a group of branched out items
         self.error = None  # if a transform fails, contains traceback
         self.transfortmTimes = {}
         self.progress = 1.
@@ -487,15 +515,15 @@
         self.beingTransformed = False
         if parentItem is None:  # i.e. self is the root item
             assert csi.dataRootItem is None, "Data tree already exists."
             csi.dataRootItem = self
             if csi.withGUI:
                 from ..gui import gcommons as gco
                 self.colorPolicy = gco.COLOR_POLICY_LOOP1
-                self.colorAutoUpdate = DEFAULT_COLOR_AUTO_UPDATE
+            self.colorAutoUpdate = DEFAULT_COLOR_AUTO_UPDATE
             self.kwargs = dict(
                 alias='auto', dataFormat={}, originNodeName=None,
                 terminalNodeName=None, transformNames='each',
                 copyTransformParams=True)
             return
 
         originNodeName = kwargs.get(
@@ -513,14 +541,15 @@
         self.terminalNodeName = terminalNodeName
 
         self.transformNames = kwargs.get(
             'transformNames', csi.dataRootItem.kwargs['transformNames'])
         if self.transformNames is None:
             self.transformNames = 'each'
 
+        self.state = dict((nn, cco.DATA_STATE_UNDEFINED) for nn in csi.nodes)
         self.alias = kwargs.get('alias',
                                 csi.dataRootItem.kwargs['alias'])
         self.suffix = kwargs.get('suffix',
                                  csi.dataRootItem.kwargs.get('suffix', None))
         self.dataFormat = copy.deepcopy(
             kwargs.get('dataFormat', csi.dataRootItem.kwargs['dataFormat']))
         # make forward slashes in file names:
@@ -532,15 +561,14 @@
         self.isExpanded = True
         self.colorTag = kwargs.get('colorTag',
                                    csi.dataRootItem.kwargs.get('colorTag', 0))
         if 'colorIndividual' in kwargs:
             self.colorIndividual = kwargs['colorIndividual']
 
         self.hasChanged = False
-        self.state = dict((nn, cco.DATA_STATE_UNDEFINED) for nn in csi.nodes)
         self.aliasExtra = None  # for extra name qualifier
         self.meta = {'text': '', 'modified': '', 'size': 0}
         self.combinesTo = []  # list of instances of Spectrum if not empty
 
         self.transformParams = {}  # each transform will add to this dict
         # init self.transformParams:
         for tr in csi.transforms.values():
@@ -573,19 +601,28 @@
                 csi.dataRootItem.kwargs.get('runDownstream', False))
             if csi.withGUI:
                 self.init_plot_props()
                 plotProps = kwargs.pop('plotProps', {})
                 if plotProps:
                     self.plotProps.update(copy.deepcopy(plotProps))
 
+            if 'concatenate' in kwargs and kwargs['concatenate']:
+                concatenate = kwargs['concatenate']
+                self.concatenateOf = self.madeOf
+                self.concatenate = concatenate
+            else:
+                concatenate = False
+            lengthCheck = kwargs.pop('lengthCheck', None)
             self.read_data(shouldLoadNow=shouldLoadNow,
                            runDownstream=runDownstream,
                            copyTransformParams=copyTransformParams,
                            transformParams=transformParams,
-                           fitParams=fitParams)
+                           fitParams=fitParams,
+                           concatenate=concatenate,
+                           lengthCheck=lengthCheck)
 
         elif isinstance(self.madeOf, str) and not self.dataFormat:
             # i.e. is a group
             self.dataType = cco.DATA_GROUP
             if csi.withGUI:
                 from ..gui import gcommons as gco
                 cp = (kwargs.pop('colorPolicy', 'loop1')).lower()
@@ -605,50 +642,60 @@
                 else:
                     raise ValueError("wrong choice of color type")
                 self.colorAutoUpdate = bool(kwargs.pop(
                     'colorAutoUpdate', DEFAULT_COLOR_AUTO_UPDATE))
             if self.alias == 'auto':
                 self.alias = str(madeOf)
         else:
-            raise ValueError('unknown data type of {0}'.format(self.alias))
+            raise ValueError('unknown data type {0} of {1}'.format(
+                type(self.madeOf), self.alias))
 
     def init_plot_props(self):
         row = self.row()
         if row is None:
             row = 0
         self.color = 'k'
         self.plotProps = {}
         for node in csi.nodes.values():
             self.plotProps[node.name] = {}
             if node.plotDimension == 1:
-                if len(csi.selectedItems) > 0:
-                    self.plotProps[node.name] = dict(
-                        csi.selectedItems[0].plotProps[node.name])
+                # items = csi.selectedItems
+                items = csi.allLoadedItems
+                if len(items) > 0:
+                    if hasattr(items[0], 'plotProps'):
+                        self.plotProps[node.name] = dict(
+                            items[0].plotProps[node.name])
+                    else:
+                        self.init_default_plot_props(node)
                 else:
-                    for ind, yName in enumerate(node.plotYArrays):
-                        plotParams = {}
-                        plotParams['yaxis'] = \
-                            'right' if node.get_prop(yName, 'role').endswith(
-                                'right') else 'left'
-                        nodePlotParams = node.get_prop(yName, 'plotParams')
-                        for k, v in nodePlotParams.items():
-                            if isinstance(v, (list, tuple)):
-                                pv = v[ind]
-                            else:
-                                pv = v
-                            plotParams[k] = pv
-                        self.plotProps[node.name][yName] = plotParams
+                    self.init_default_plot_props(node)
+
+    def init_default_plot_props(self, node):
+        for ind, yName in enumerate(node.plotYArrays):
+            plotParams = {}
+            plotParams['yaxis'] = \
+                'right' if node.get_prop(yName, 'role').endswith(
+                    'right') else 'left'
+            nodePlotParams = node.get_prop(yName, 'plotParams')
+            for k, v in nodePlotParams.items():
+                if isinstance(v, (list, tuple)):
+                    pv = v[ind]
+                else:
+                    pv = v
+                plotParams[k] = pv
+            self.plotProps[node.name][yName] = plotParams
 
     def get_state(self, nodeName):
         if self.error is not None:
             return cco.DATA_STATE_BAD
         return self.state[nodeName]
 
     def read_data(self, shouldLoadNow=True, runDownstream=False,
-                  copyTransformParams=True, transformParams={}, fitParams={}):
+                  copyTransformParams=True, transformParams={}, fitParams={},
+                  concatenate=False, lengthCheck=None):
         fromNode = csi.nodes[self.originNodeName]
         if isinstance(self.madeOf, dict):
             self.dataType = cco.DATA_BRANCH
             if self.alias == 'auto':
                 tmpalias = '{0}_{1}'.format(
                     self.parentItem.alias, self.parentItem.child_count())
             if shouldLoadNow:
@@ -656,40 +703,92 @@
         elif callable(self.madeOf):
             self.dataType = cco.DATA_FUNCTION
             if self.alias == 'auto':
                 tmpalias = "generated_{0}".format(self.madeOf.__name__)
             if shouldLoadNow:
                 self.create_data()
         elif isinstance(self.madeOf, (list, tuple)):
-            self.dataType = cco.DATA_COMBINATION
-            self.colorTag = 5
-            if shouldLoadNow:
-                self.calc_combined()
-            if self.alias == 'auto':
-                cs = self.madeOf[0].alias
-                for data in self.madeOf[1:]:
-                    cs = cco.common_substring((cs, data.alias))
-                what = self.dataFormat['combine']
-                lenC = len(self.madeOf)
-                tmpalias = "{0}_{1}{2}".format(
-                    cs, cco.combineNames[what], lenC)
+            if concatenate:
+                axis, reduce = concatenate[:2] \
+                    if isinstance(concatenate, (list, tuple)) else (0, False)
+                madeOfTmp = list(self.madeOf)
+                for iconcat, madeOf in enumerate(madeOfTmp):
+                    self.madeOf = madeOf.replace('\\', '/')
+                    if iconcat == 0:
+                        if self.madeOf.startswith('silx:'):
+                            self.dataType = cco.DATA_DATASET
+                        else:
+                            self.dataType = cco.DATA_COLUMN_FILE
+                        self.set_auto_color_tag()
+                    if shouldLoadNow:
+                        self.read_file()
+                    for aName in fromNode.arrays:
+                        setName = fromNode.get_prop(aName, 'raw')
+                        if iconcat == 0:
+                            if reduce:
+                                concatTmp = getattr(self, setName).sum(
+                                    axis=axis, keepdims=True)
+                            else:
+                                concatTmp = copy.copy(getattr(self, setName))
+                            setattr(self, setName+'Concat', concatTmp)
+                        else:
+                            if reduce:
+                                tmp = getattr(self, setName).sum(
+                                    axis=axis, keepdims=True)
+                            else:
+                                tmp = copy.copy(getattr(self, setName))
+                            if getattr(self, setName+'Concat') is not None:
+                                concatTmp = np.concatenate(
+                                    (getattr(self, setName+'Concat'), tmp))
+                                setattr(self, setName+'Concat', concatTmp)
+                                setattr(self, setName, concatTmp)
+                            else:
+                                setattr(self, setName, None)
+                if self.state[fromNode.name] == cco.DATA_STATE_GOOD:
+                    shapes = self.check_shape()
+                    if isinstance(shapes, dict):
+                        print('Incompatible data shapes in {0}:\n{1}'.format(
+                            fromNode.name, shapes))
+                        self.state[self.originNodeName] = cco.DATA_STATE_BAD
+                        self.badShapes = shapes
+                        self.colorTag = 3
+                if self.alias == 'auto':
+                    tmpalias = 'concatenation'
+            else:
+                self.dataType = cco.DATA_COMBINATION
+                self.colorTag = 5
+                if shouldLoadNow:
+                    self.calc_combined()
+                if self.alias == 'auto':
+                    cs = self.madeOf[0].alias
+                    for data in self.madeOf[1:]:
+                        cs = cco.common_substring((cs, data.alias))
+                    what = self.dataFormat['combine']
+                    lenC = len(self.madeOf)
+                    tmpalias = "{0}_{1}{2}".format(
+                        cs, cco.combineNames[what], lenC)
         elif isinstance(self.madeOf, str):
             self.madeOf = self.madeOf.replace('\\', '/')
             if self.madeOf.startswith('silx:'):
                 self.dataType = cco.DATA_DATASET
             else:
                 self.dataType = cco.DATA_COLUMN_FILE
             self.set_auto_color_tag()
             if shouldLoadNow:
-                self.read_file()
+                self.read_file(lengthCheck=lengthCheck)
 
-            if self.state[fromNode.name] == cco.DATA_STATE_GOOD:
-                if not self.check_shape():
-                    print('Incompatible data shapes!')
+            if self.state[fromNode.name] == cco.DATA_STATE_MARKED_FOR_DELETION:
+                return
+            elif self.state[fromNode.name] == cco.DATA_STATE_GOOD:
+                shapes = self.check_shape()
+                if isinstance(shapes, dict):
+                    print('Incompatible data shapes in {0}:\n{1}'.format(
+                        fromNode.name, shapes))
                     self.state[self.originNodeName] = cco.DATA_STATE_BAD
+                    self.badShapes = shapes
                     self.colorTag = 3
 
             basename = osp.basename(self.madeOf)
             if self.alias == 'auto':
                 tmpalias = osp.splitext(basename)[0]
                 if '::' in self.madeOf:
                     h5name = osp.splitext(osp.basename(
@@ -736,14 +835,16 @@
         # be replotted by that transform:
         for tr in fromNode.transformsOut:
             if tr.fromNode is tr.toNode:
                 break
         else:
             csi.nodesToReplot = [fromNode]
 
+        self.make_corrections(fromNode)
+
         if runDownstream and fromNode.transformsOut and \
                 self.state[fromNode.name] == cco.DATA_STATE_GOOD:
             for tr in fromNode.transformsOut:
                 tr.run(dataItems=[self])  # no need for multiprocessing here
                 if csi.model is not None:
                     csi.model.invalidateData()
 
@@ -757,30 +858,38 @@
         if self.dataType == cco.DATA_DATASET:
             self.colorTag = 1
         elif self.dataType == cco.DATA_COLUMN_FILE:
             self.colorTag = 2
 
     def check_shape(self):
         fromNode = csi.nodes[self.originNodeName]
+        shapes = {}
+        hasFailed = False
         for iarr, arrName in enumerate(fromNode.checkShapes):
             pos = arrName.find('[')
             if pos > 0:
                 stem = arrName[:pos]
                 sl = arrName[pos+1:-1]
             else:
                 stem = arrName
                 sl = '0'
             checkName = fromNode.get_prop(stem, 'raw')
             arr = getattr(self, checkName)
-            shape = arr.shape[eval(sl)] if arr is not None else []
+            try:
+                shape = arr.shape[eval(sl)] if arr is not None else []
+                shapes[checkName] = shape
+            except IndexError:
+                return False
             if iarr == 0:
                 shape0 = shape
                 continue
             if shape != shape0:
-                return False
+                hasFailed = True
+        if hasFailed:
+            return shapes
         return True
 
     def insert_data(self, data, insertAt=None, **kwargs):
         u"""This method inserts a tree-like structure *data* into the list of
         children. An example of *data*:
         :code:`data=["groupName", ["fName1.dat", "fName2.dat"]]` for a group
         with two items in it. All other key word parameters lumped into
@@ -804,14 +913,19 @@
         of the longest sequence(s)."""
 
         def getTransformParams(configData):
             res = {}
             for tr in csi.transforms.values():
                 for key, val in tr.defaultParams.items():
                     res[key] = config.get(configData, name, key, default=val)
+            for node in csi.nodes.values():
+                corr_param_name = 'correction_' + node.name
+                vv = config.get(configData, name, corr_param_name)
+                if vv is not None:
+                    res[corr_param_name] = vv
             return res
 
         def getFitParams(configData):
             res = {}
             for fit in csi.fits.values():
                 for key, val in fit.defaultParams.items():
                     if key == fit.ioAttrs['result']:
@@ -837,39 +951,51 @@
                         tmp['colorIndividual'] = config.get(
                             configData, name, 'colorIndividual')
                     if 'plotProps' in configData[name]:
                         tmp['plotProps'] = config.get(
                             configData, name, 'plotProps')
                     tmp['transformParams'] = getTransformParams(configData)
                     tmp['fitParams'] = getFitParams(configData)
-                    name = tmp.pop('madeOf_relative')
+                    nameRel = tmp.pop('madeOf_relative')
+                    if nameRel is not None:
+                        name = nameRel
+                    else:
+                        name = tmp.get('madeOf')
                     nameFull = tmp.pop('madeOf')
                 elif isinstance(madeOf, (dict, list, tuple)):
                     tmp = {entry: config.get(configData, name, entry)
                            for entry in self.configFieldsCombined}
                     tmp['alias'] = name
                     tmp['transformParams'] = getTransformParams(configData)
                     tmp['fitParams'] = getFitParams(configData)
                     if isinstance(madeOf, dict):
                         tmp['dataFormat'] = {}
                         name = tmp.pop('madeOf')
                     elif isinstance(madeOf, (list, tuple)):
+                        if 'concatenate' in configData[name]:
+                            tmp['concatenate'] = config.get(
+                                configData, name, 'concatenate')
+                            tmp['shouldLoadNow'] = True
+                        else:
+                            tmp['shouldLoadNow'] = False
                         name = tmp.pop('madeOf')
-                        tmp['shouldLoadNow'] = False
                         # for spName in madeOf:
                         #     item = self.get_top().find_data_item(spName)
                         #     if item is None:
                         #         raise ValueError(
                         #             'Error while loading "{0}": '
                         #             'no data "{1}" among the loaded ones!'
                         #             .format(tmp['alias'], spName))
                         #     name.append(item)
                 elif 'colorPolicy' in configData[name]:  # group entry
                     tmp = {entry: config.get(configData, name, entry)
                            for entry in self.configFieldsGroup}
+                    if tmp['colorPolicy'] == 'gradient':
+                        tmp['color1'] = config.get(configData, name, 'color1')
+                        tmp['color2'] = config.get(configData, name, 'color2')
                 else:
                     tmp = {}
                 kwargs = dict(tmp)
             else:
                 kwargs = {}
             kwargs['runDownstream'] = False
         elif 'configDict' in kwargs:
@@ -877,14 +1003,17 @@
             kwargs = dict(configDict[name]) if name in configDict else {}
 
         df = kwargs.get('dataFormat', {})
         if isinstance(name, str) and not df:
             # is a group
             return Spectrum(name, self, insertAt, **kwargs)
 
+        if 'concatenate' in kwargs and kwargs['concatenate']:
+            return Spectrum(name, self, insertAt, **kwargs)
+
         spectraInOneFile = 1
         dataSource = list(df.get('dataSource', []))
         dataSourceSplit = []
         for ds in dataSource:
             ds = str(ds)
             if "np." in ds:
                 continue
@@ -912,15 +1041,15 @@
                     else:
                         self.childItems.pop(insertAt)
                     print('local file {0} not found, will load {1}'.format(
                         name, nameFull))
                     kwargs['dataFormat'] = dataFormatFull
                     return Spectrum(nameFull, self, insertAt, **kwargs)
                 else:
-                    raise(e)
+                    raise e
 
         basename = osp.basename(name)
         groupName = osp.splitext(basename)[0]
         group = Spectrum(groupName, self, insertAt, colorPolicy='loop1')
 
         multiArr = []
         for ids, ds in enumerate(dataSourceSplit):
@@ -945,25 +1074,25 @@
             Spectrum(name, group, dataFormat=df, alias=alias, **kwargs)
 
         if csi.withGUI:
             group.init_colors(group.childItems)
 
         return group
 
-    def read_file(self):
+    def read_file(self, lengthCheck=None):
         madeOf = self.madeOf
         fromNode = csi.nodes[self.originNodeName]
         df = dict(self.dataFormat)
         df.update(csi.extraDataFormat)
         formatSection = 'Format_' + fromNode.name
         config.configLoad[formatSection] = dict(df)
 
         arr = []
         if self.dataType == cco.DATA_COLUMN_FILE:
-            header = cco.get_header(madeOf, df)
+            header = cco.get_header(madeOf, df, searchAllLines=True)
         elif self.dataType == cco.DATA_DATASET:
             header = []
             try:
                 label = silx_io.get_data(madeOf + "/" + df["labelName"])
                 self.aliasExtra = label.decode("utf-8")
                 header.append(label)
             except (ValueError, KeyError):
@@ -982,21 +1111,38 @@
                         mdres = mdres.decode("utf-8")
                     header.append("<b>{0}</b>: {1}<br>".format(md, mdres))
                 except (ValueError, KeyError, OSError) as e:
                     print('No metadata: {0}'.format(e))
         else:
             raise TypeError('wrong datafile type')
 
-        try:
+        # try:
+        if True:
             df['skip_header'] = df.pop('skiprows', 0)
             dataSource = df.pop('dataSource', None)
             sliceStrs = df.pop('slices', ['' for ds in dataSource])
             conversionFactors = df.pop('conversionFactors',
                                        [None for arr in fromNode.arrays])
             df.pop('metadata', None)
+            cols = 0
+            for ds in dataSource:
+                try:
+                    ds = int(ds)
+                except Exception:
+                    pass
+                if isinstance(ds, str) and "Col" in ds:
+                    regex = re.compile('Col([0-9]*)')
+                    # remove possible duplicates by list(dict.fromkeys())
+                    subkeys = list(dict.fromkeys(regex.findall(ds)))
+                    for ch in subkeys:
+                        cols = max(cols, int(ch))
+                elif isinstance(ds, int):
+                    cols = max(cols, ds)
+            # important for column files that have incomplete columns:
+            df['usecols'] = list(range(cols+1))
             if dataSource is None:
                 raise ValueError('bad dataSource settings')
             if self.dataType == cco.DATA_COLUMN_FILE:
                 with warnings.catch_warnings():
                     warnings.simplefilter("ignore")
                     arrs = np.genfromtxt(madeOf, unpack=True, **df)
                 if len(arrs) == 0:
@@ -1007,22 +1153,28 @@
             # Create optional arrays and assign None.
             # This loop is needed when dataSource list is shorter than arrays.
             for aName, role in zip(fromNode.arrays, roles):
                 setName = fromNode.get_prop(aName, 'raw')
                 if role == 'optional':
                     setattr(self, setName, None)
 
+            sortIndices = None
+            sortArrayName = 'x'
             for aName, txt, sliceStr, role in zip(
                     fromNode.arrays, dataSource, sliceStrs, roles):
                 setName = fromNode.get_prop(aName, 'raw')
                 if (role == 'optional') and (txt == ''):
                     setattr(self, setName, None)
                     continue
                 try:
                     if self.dataType == cco.DATA_COLUMN_FILE:
+                        try:
+                            txt = int(txt)
+                        except Exception:
+                            pass
                         if isinstance(txt, int):
                             arr = arrs[txt]
                         else:
                             arr = self.interpret_array_formula(txt, arrs)
                     else:
                         arr = self.interpret_array_formula(txt)
                         if sliceStr:
@@ -1034,22 +1186,48 @@
                             else:
                                 sliceTuple = tuple(
                                     cco.parse_slice_str(slc)
                                     for slc in sliceStr.split(','))
                                 arr = arr[sliceTuple]
                     setattr(self, setName, arr)
                 except Exception as e:
+                    print(e)
                     setattr(self, setName, None)
-                    raise ValueError(e)
+                    # raise ValueError(e)
 
+                if lengthCheck and role == 'x':
+                    if isinstance(lengthCheck, (int, float)):
+                        if arr.max() - arr.min() < lengthCheck:
+                            # print('too short')
+                            self.state[fromNode.name] = \
+                                cco.DATA_STATE_MARKED_FOR_DELETION
+                            return
+                if role == 'x':
+                    sortArrayName = aName
+                    _, sortIndices, sortCounts = np.unique(
+                        arr, return_index=True, return_counts=True)
+
+            if sortIndices is not None:
+                count = sortCounts[sortCounts > 1].sum()
+                if count > 0:
+                    print("{0} duplicate {1} value{2} ha{3} been removed"
+                          .format(count,
+                                  fromNode.get_prop(sortArrayName, 'qLabel'),
+                                  '' if count == 1 else 's',
+                                  's' if count == 1 else 've'))
+                for aName in fromNode.arrays:
+                    setName = fromNode.get_prop(aName, 'raw')
+                    arrt = getattr(self, setName)
+                    if isinstance(arrt, np.ndarray):
+                        setattr(self, setName, arrt[sortIndices])
             self.state[fromNode.name] = cco.DATA_STATE_GOOD
-        except (ValueError, OSError, IndexError) as e:
-            print('Error in read_file(): {0}'.format(e))
-            self.state = dict((n, cco.DATA_STATE_NOTFOUND) for n in csi.nodes)
-            return
+        # except (ValueError, OSError, IndexError) as e:
+        #     print('Error in read_file(): {0}'.format(e))
+        #     self.state = dict((n, cco.DATA_STATE_NOTFOUND) for n in csi.nodes)
+        #     return
 
         self.convert_units(conversionFactors)
         # define metadata
         if self.dataType == cco.DATA_COLUMN_FILE:
             self.meta['text'] = r''.join(header)
             self.meta['modified'] = time.strftime(
                 "%a, %d %b %Y %H:%M:%S", time.gmtime(osp.getmtime(madeOf)))
@@ -1059,25 +1237,28 @@
                 if isinstance(header[0], bytes):
                     self.meta['text'] = '\n'.join(
                         h.decode("utf-8") for h in header)
                 else:
                     self.meta['text'] = '\n'.join(header)
             else:
                 self.meta['text'] = ''
-        self.meta['length'] = len(arr)
+        try:
+            self.meta['length'] = len(arr)
+        except TypeError:  # another type, not array
+            pass
 
         start = 5 if self.madeOf.startswith('silx:') else 0
         end = self.madeOf.find('::') if '::' in self.madeOf else None
         path = self.madeOf[start:end]
         abspath = osp.abspath(path).replace('\\', '/')
         toSave = self.madeOf[:start] + abspath
         if end is not None:
             toSave += self.madeOf[end:]
         config.put(config.configLoad, 'Data', fromNode.name, toSave)
-        config.write_configs('transform')
+        config.write_configs('transform, load')
 
     def interpret_array_formula(self, colStr, treeObj=None):
         if "np." in colStr:
             try:
                 arr = eval(colStr)
                 return arr
             except Exception:
@@ -1124,22 +1305,30 @@
                 locals()[k] = k
         return eval(colStr)
 
     def convert_units(self, conversionFactors):
         if not conversionFactors:
             return
         fromNode = csi.nodes[self.originNodeName]
+        secondPassNeeded = False
         for aName, cFactor in zip(fromNode.arrays, conversionFactors):
             if not cFactor:
                 continue
             setName = fromNode.get_prop(aName, 'raw')
             arr = getattr(self, setName)
+            if arr is None:
+                continue
             try:
                 if isinstance(cFactor, str):
-                    if cFactor.startswith('transpose'):
+                    if cFactor.startswith('lim'):
+                        secondPassNeeded = True
+                        mn, mx = eval(cFactor[3:])
+                        where = ((mn < arr) if mn is not None else True) & \
+                            ((arr < mx) if mx is not None else True)
+                    elif cFactor.startswith('transpose'):
                         axes = eval(cFactor[9:])
                         setattr(self, setName, arr.transpose(*axes))
                     elif cFactor.startswith('f'):
                         arr *= 1e15
                     elif cFactor.startswith('p'):
                         arr *= 1e12
                     elif cFactor.startswith('n'):
@@ -1150,21 +1339,33 @@
                         arr *= 1e3
                     elif cFactor.startswith('k'):
                         arr *= 1e-3
                     elif cFactor.startswith('M'):
                         arr *= 1e-6
                     elif cFactor.startswith('G'):
                         arr *= 1e-9
+                    self.hasChanged = True
                     continue
                 arr *= cFactor
-                self.hasChanged = True
             except Exception as e:
-                print(e)
+                print(e, aName)
                 setattr(self, setName, None)
 
+        if secondPassNeeded:
+            for aName in fromNode.arrays:
+                setName = fromNode.get_prop(aName, 'raw')
+                arr = getattr(self, setName)
+                if arr is None:
+                    continue
+                try:
+                    setattr(self, setName, arr[where])
+                except Exception as e:
+                    print(aName, e)
+                    setattr(self, setName, None)
+
     def calc_combined(self):
         """Case of *madeOf* as list of Spectrum instances. self.dataFormat is
         the type of the combination being made: one of COMBINE_XXX constants.
         """
         madeOf = self.madeOf
         what = self.dataFormat['combine']
         # define metadata
@@ -1239,15 +1440,15 @@
 
             self.meta['length'] = len(dimArray) if dimArray is not None else 0
             self.state[fromNode.name] = cco.DATA_STATE_GOOD
         except AssertionError:
             self.state[fromNode.name] = cco.DATA_STATE_MATHERROR
             msg = '\nThe conbined arrays have different lengths'
             self.meta['text'] += msg
-            if csi.DEBUG_LEVEL > 50:
+            if csi.DEBUG_LEVEL > 0:
                 print('calc_combined', self.alias, msg)
 
     @logger(minLevel=50, attrs=[(0, 'alias')])
     def branch_data(self):
         """Case of *madeOf* as dict, when branching out."""
         fromNode = csi.nodes[self.originNodeName]
         try:
@@ -1309,28 +1510,35 @@
 
     def save_to_project(self, configProject, dirname):
         from ..gui import gcommons as gco  # only needed with gui
         item = self
         if ((isinstance(item.madeOf, str) and item.dataFormat) or
                 isinstance(item.madeOf, (list, tuple, dict))):
             if isinstance(item.madeOf, str):
-                start = 5 if item.madeOf.startswith('silx:') else 0
-                end = item.madeOf.find('::') if '::' in item.madeOf else None
-                path = item.madeOf[start:end]
-                abspath = osp.abspath(path).replace('\\', '/')
-                madeOf = item.madeOf[:start] + abspath
-                if end is not None:
-                    madeOf += item.madeOf[end:]
-                config.put(configProject, item.alias, 'madeOf', madeOf)
-                relpath = osp.relpath(path, dirname).replace('\\', '/')
-                madeOfRel = item.madeOf[:start] + relpath
-                if end is not None:
-                    madeOfRel += item.madeOf[end:]
-                config.put(configProject, item.alias, 'madeOf_relative',
-                           madeOfRel)
+                if hasattr(item, 'concatenateOf'):
+                    config.put(configProject, item.alias, 'madeOf',
+                               str(item.concatenateOf))
+                    config.put(configProject, item.alias, 'concatenate',
+                               str(item.concatenate))
+                else:
+                    start = 5 if item.madeOf.startswith('silx:') else 0
+                    end = item.madeOf.find('::') if '::' in item.madeOf else \
+                        None
+                    path = item.madeOf[start:end]
+                    abspath = osp.abspath(path).replace('\\', '/')
+                    madeOf = item.madeOf[:start] + abspath
+                    if end is not None:
+                        madeOf += item.madeOf[end:]
+                    config.put(configProject, item.alias, 'madeOf', madeOf)
+                    relpath = osp.relpath(path, dirname).replace('\\', '/')
+                    madeOfRel = item.madeOf[:start] + relpath
+                    if end is not None:
+                        madeOfRel += item.madeOf[end:]
+                    config.put(configProject, item.alias, 'madeOf_relative',
+                               madeOfRel)
 
                 dataFormatCopy = copy.deepcopy(item.dataFormat)
                 dataSource = list(dataFormatCopy.get('dataSource', []))
                 if 'conversionFactors' in dataFormatCopy:
                     if dataFormatCopy['conversionFactors'] == \
                             [None for ds in dataSource]:  # all None's
                         dataFormatCopy.pop('conversionFactors', None)
@@ -1449,34 +1657,35 @@
                 configProject, item.alias, 'colorTag', str(item.colorTag))
             config.put(
                 configProject, item.alias, 'colorAutoUpdate',
                 str(item.colorAutoUpdate))
 
     @logger(minLevel=50, attrs=[(0, 'alias')])
     def branch_out(self, nbrunch, toTransfer, nodeStop, nodeStart,
-                   transformNames, label=''):
+                   transformNames=[], groupLabel='_rois', label=''):
         """Brach this spectrum into a group of *nbrunch* new items. Example:
         a 3D item has n ROIs that result in n 1D spectra; these spectra are put
         to a new group and start at *nodeStart* (str) whereas the original data
         item stops at *nodeStop* (str). The sequence *toTransfer* has field
         names that will be created in the new branches and will be assigned the
         values of the same fields from the branched out spectrum.
         """
 
         if csi.model is not None:
             csi.model.beginResetModel()
         self.terminalNodeName = nodeStop
         self.colorTag = 3
         if self.branch is None:
-            kw = dict(colorPolicy='loop2', colorTag=4)
+            c1, c2 = '#ff0000', '#0000ff'
+            kw = dict(colorPolicy='grad', color1=c1, color2=c2, colorTag=4)
             self.branch = self.parentItem.insert_item(
-                self.alias+'_rois', self.row()+1, **kw)
-            if hasattr(self.branch.parentItem, 'colorAutoUpdate'):
-                self.branch.colorAutoUpdate = \
-                    self.branch.parentItem.colorAutoUpdate
+                self.alias+groupLabel, self.row()+1, **kw)
+            self.branch.color1 = c1
+            self.branch.color2 = c2
+            self.branch.colorAutoUpdate = csi.dataRootItem.colorAutoUpdate
         while self.branch.child_count() > nbrunch:
             self.branch.childItems[-1].remove_from_parent()
         while self.branch.child_count() < nbrunch:
             kw = dict(
                 alias='{0}_{1}{2}'.format(self.alias, label,
                                           self.branch.child_count()+1),
                 originNodeName=nodeStart, transformNames=transformNames,
@@ -1484,15 +1693,93 @@
             dictToTransfer = {key: self.alias for key in toTransfer}
             newItem = self.branch.insert_item(
                 dictToTransfer, self.branch.child_count(), **kw)
             newItem.transformParams = self.transformParams
             newItem.fitParams = self.fitParams
             newItem.meta = self.meta
             newItem.colorTag = 4
-        self.init_colors(self.branch.childItems)
+        self.branch.init_colors(self.branch.childItems)
         for newItem in self.branch.childItems:
             newItem.state[nodeStart] = cco.DATA_STATE_GOOD
             for key in toTransfer:
                 setattr(newItem, key, getattr(self, key))
+        self.state[nodeStart] == cco.DATA_STATE_UNDEFINED
 
         if csi.model is not None:
             csi.model.endResetModel()
+
+    def make_corrections(self, node):
+        wasCorrected = False
+        corr_param_name = 'correction_' + node.name
+        if corr_param_name not in self.transformParams:
+            return wasCorrected
+        corrections = self.transformParams[corr_param_name]
+        for correction in corrections:
+            # if correction['kind'] in ('delete',):
+            #     prop = 'raw'
+            # else:
+            #     prop = 'key'
+            prop = 'raw'
+            if 'ndim' not in correction:
+                correction['ndim'] = 1
+
+            if correction['ndim'] == 1:
+                xkeys = node.get_arrays_prop('name', role='x')
+                if len(xkeys) == 0:
+                    continue
+                # xkey = xkeys[0]
+                xkey = node.get_prop(xkeys[0], prop)
+                try:
+                    x = getattr(self, xkey)
+                except AttributeError:
+                    continue
+                shapeBefore = x.shape
+
+                corrKeys = []
+                for k, arr in node.arrays.items():
+                    key = node.get_prop(k, prop)
+                    if key == xkey:
+                        continue
+                    try:
+                        y = getattr(self, key)
+                    except AttributeError:
+                        continue
+                    if y is not None and y.shape == shapeBefore:
+                        # if node.widget is not None:
+                        #     x, y = \
+                        #         node.widget.transformWidget.extraPlotTransform(
+                        #             self, xkey, x, k, y)
+                        res = calc_correction(x, y, correction)
+                        if res is None:
+                            continue
+                        wasCorrected = True
+                        xn, yn = res
+                        setattr(self, key, yn)
+                        corrKeys.append(key)
+
+                if correction['kind'] == 'delete':
+                    for nodeOther in csi.nodes.values():
+                        if nodeOther is node:
+                            continue
+                        xkeysOther = nodeOther.get_arrays_prop(
+                            'name', role='x')
+                        if len(xkeysOther) == 0:
+                            continue
+                        xkeyOther = xkeysOther[0]
+                        if xkeyOther != xkey:
+                            continue
+                        for k, arr in nodeOther.arrays.items():
+                            key = nodeOther.get_prop(k, prop)
+                            try:
+                                attr = getattr(self, key)
+                            except AttributeError:
+                                continue
+                            if key in corrKeys:
+                                continue
+                            if attr is not None and attr.shape == shapeBefore:
+                                _, aC = calc_correction(x, attr, correction)
+                                setattr(self, key, aC)
+                    setattr(self, xkey, xn)
+
+            elif correction['ndim'] == 2:
+                pass
+        return wasCorrected
```

## Comparing `parseq-2023.5.0/parseq/core/transforms.py` & `parseq-2024.5.0/parseq/core/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 Data transformations provide values for all the arrays defined in one
 transformation node (`fromNode`) given arrays defined in another transformation
 node (`toNode`). Each transformation defines a dictionary of transformation
 parameters; the values of these parameters are individual per data item. Each
 transformation in a pipeline requires subclassing from :class:`Transform`.
 """
 __author__ = "Konstantin Klementiev"
-__date__ = "17 Feb 2023"
+__date__ = "28 Apr 2024"
 # !!! SEE CODERULES.TXT !!!
 
 import sys
-# import os
+import os
 import numpy as np
 
 import traceback
 # import types
 if sys.version_info < (3, 1):
     from inspect import getargspec
 else:
@@ -35,15 +35,14 @@
 import errno
 
 from . import singletons as csi
 from . import commons as cco
 from .logger import logger
 from .config import configTransforms
 
-
 # class Param(object):
 #     def __init__(self, value, limits=[], step=None):
 #         self.limits = limits
 #         self.step = step
 #         self.value = value
 
 #     @property
@@ -114,15 +113,15 @@
                 "@staticmethod or @classmethod".format(self.__class__))
 
         self.fromNode = fromNode
         self.toNode = toNode
         if self.name in csi.transforms:
             raise ValueError("A transform '{0}' already exists. One instance "
                              "is allowed".format(self.name))
-        self.isHeadNode = len(csi.transforms) == 0
+        self.isHeadTransform = len(csi.transforms) == 0
         csi.transforms[self.name] = self
 
         if self not in fromNode.transformsOut:
             fromNode.transformsOut.append(self)
         if self not in toNode.transformsIn:
             toNode.transformsIn.append(self)
         self.sendSignals = False
@@ -164,16 +163,17 @@
                     self.iniParams[key] = eval(testStr)
                 except (SyntaxError, NameError):
                     self.iniParams[key] = testStr
 
     def update_params(self, params, dataItems):
         for data in dataItems:
             for par in params:
-                if par not in data.transformParams:
-                    raise KeyError("Unknown parameter '{0}'".format(par))
+                if par not in data.transformParams and not par.startswith(
+                        'correction_'):
+                    raise KeyError(u"Unknown parameter '{0}'".format(par))
                 data.transformParams[par] = params[par]
         # data = csi.selectedItems[0]
         # dtparams = data.transformParams
 
     def _get_progress1(self, alias, progress):
         if not hasattr(self.toNode, 'widget'):
             return
@@ -190,20 +190,21 @@
             self.toNode.widget.tree.transformProgress.emit([alias, 1.0])
         else:
             ps = worker.get_progress()
             if len(ps) == 0:
                 return
             self.toNode.widget.tree.transformProgress.emit([alias, ps[-1]])
 
+    @logger(minLevel=20, attrs=[(0, 'name')])
     def _run_multi_worker(self, workers, workedItems, args):
+        time0 = time.time()
         wt = workers[0].workerType
         if csi.DEBUG_LEVEL > 1:
-            print('run "{0}" in {1} {2}{3} for {4}'.format(
-                self.name, len(workers), wt, '' if len(workers) == 1 else 's',
-                [d.alias for d in workedItems]))
+            print('run "{0}" in {1} {2}{3}'.format(
+                self.name, len(workers), wt, '' if len(workers) == 1 else 's'))
         if self.sendSignals:
             csi.mainWindow.beforeDataTransformSignal.emit(workedItems)
 
         for worker, item in zip(workers, workedItems):
             if 'progress' in args and self.sendSignals:
                 worker.timer = NTimer(
                     self.progressTimeDelta,
@@ -211,24 +212,27 @@
                 worker.timer.start()
             if not worker.put_in_data(item):
                 item.state[self.toNode.name] = cco.DATA_STATE_BAD
                 item.beingTransformed = False
                 continue
             else:
                 item.beingTransformed = self.name
-            worker.start()
             item.transfortm_t0 = time.time()
+            worker.start()
 
         for worker, item in zip(workers, workedItems):
             if not item.beingTransformed:
                 continue
             worker.get_out_data(item)
             res = worker.get_results(self)
-            item.state[self.toNode.name] = cco.DATA_STATE_GOOD\
-                if res else cco.DATA_STATE_BAD
+            if isinstance(res, bool):
+                item.state[self.toNode.name] = cco.DATA_STATE_GOOD\
+                    if res else cco.DATA_STATE_BAD
+            elif isinstance(res, int):
+                item.state[self.toNode.name] = res
             item.error = worker.get_error()
             item.transfortmTimes[self.name] = time.time() - item.transfortm_t0
 
         for worker, item in zip(workers, workedItems):
             if 'progress' in args and self.sendSignals:
                 worker.timer.cancel()
             if not item.beingTransformed:
@@ -237,14 +241,15 @@
             item.beingTransformed = False
             if 'progress' in args and self.sendSignals:
                 self._get_progressN(item.alias)
 
         if self.sendSignals:
             csi.mainWindow.afterDataTransformSignal.emit(workedItems)
 
+    @logger(minLevel=20, attrs=[(0, 'name')])
     def _run_single_worker(self, data, args):
         data.beingTransformed = self.name
         data.transfortm_t0 = time.time()
         if self.sendSignals:
             csi.mainWindow.beforeDataTransformSignal.emit([data])
         if csi.DEBUG_LEVEL > 1:
             print('run "{0}" for {1}'.format(self.name, data.alias))
@@ -278,62 +283,69 @@
             errorMsg += "\nwith the followith traceback:\n"
             tb = traceback.format_exc()
             errorMsg += "".join(tb[:-1])  # remove last empty line
             # if csi.DEBUG_LEVEL > 20:
             if True:
                 print(errorMsg)
             data.error = errorMsg
-        if isinstance(res, dict):
+        if res is None:
+            data.state[self.toNode.name] = cco.DATA_STATE_BAD
+        elif isinstance(res, dict):
             for field in res:
                 setattr(self, field, res[field])
-        data.state[self.toNode.name] = cco.DATA_STATE_GOOD \
-            if res is not None else cco.DATA_STATE_BAD
+        elif isinstance(res, bool):
+            data.state[self.toNode.name] = cco.DATA_STATE_GOOD \
+                if res is not None else cco.DATA_STATE_BAD
+        elif isinstance(res, int):
+            data.state[self.toNode.name] = res
         data.beingTransformed = False
-        data.transfortmTimes[self.name] = \
-            time.time() - data.transfortm_t0
+        data.transfortmTimes[self.name] = time.time() - data.transfortm_t0
         if self.sendSignals:
             csi.mainWindow.afterDataTransformSignal.emit([data])
 
     @logger(minLevel=20, attrs=[(0, 'name')])
     def run(self, params={}, updateUndo=True, runDownstream=True,
             dataItems=None):
         np.seterr(all='raise')
         items = dataItems if dataItems is not None else csi.selectedItems
         self.run_pre(params, items, updateUndo)
 
         nC = multiprocessing.cpu_count()
         if isinstance(self.nThreads, type('')):
-            self.nThreads = nC//2 if self.nThreads.startswith('h') else nC
+            self.nThreads = max(nC//2, 1) if self.nThreads.startswith('h')\
+                else nC
         if isinstance(self.nProcesses, type('')):
-            self.nProcesses = nC//2 if self.nProcesses.startswith('h') else nC
+            self.nProcesses = max(nC//2, 1) if self.nProcesses.startswith('h')\
+                else nC
 
-        if self.nThreads > 1:
-            workerClass = BackendThread
-            cpus = self.nThreads
-        elif self.nProcesses > 1:
-            workerClass = BackendProcess
-            cpus = self.nProcesses
-        else:
-            workerClass = None
-        if workerClass is not None:
-            workers, workedItems = [], []
+        workerClass = None
+        if len(items) > 1:
+            if self.nThreads > 1:
+                workerClass = BackendThread
+                cpus = self.nThreads
+            elif self.nProcesses > 1:
+                workerClass = BackendProcess
+                cpus = self.nProcesses
+            if workerClass is not None:
+                workers, workedItems = [], []
 
         args = getargspec(self.__class__.run_main)[0]
         if 'allData' in args and workerClass is not None:
             raise SyntaxError(
                 'IMPORTANT: remove "allData" when running in multithreading'
                 ' or multiprocessing!')
         if args[0] == 'self':
             raise SyntaxError(
                 'IMPORTANT: remove "self" from "run_main()" parameters as'
                 ' this is a static method, not an instance method!')
 
         for data in items:
-            if (not self.isHeadNode and
-                    data.state[self.fromNode.name] == cco.DATA_STATE_BAD):
+            # if (not self.isHeadTransform and
+            #         data.state[self.fromNode.name] == cco.DATA_STATE_BAD):
+            if data.state[self.fromNode.name] == cco.DATA_STATE_BAD:
                 data.state[self.toNode.name] = cco.DATA_STATE_BAD
                 if csi.DEBUG_LEVEL > 1:
                     print('bad data at', self.fromNode.name, data.alias)
                 continue
             elif data.state[self.fromNode.name] == cco.DATA_STATE_NOTFOUND:
                 if csi.DEBUG_LEVEL > 20:
                     print('data not found', data.alias)
@@ -409,31 +421,33 @@
         | run_main(cls, data, allData)
         | run_main(cls, data, progress)
 
         *data* is a data item, instance of :class:`.Spectrum`.
 
         *allData* and *progress* are both optional in the method’s signature.
         The keyword names must be kept as given above if they are used and must
-        be in this given order if both are present.
+        be in this given order.
 
         *allData* is a list of all data items living in the data model. If
         *allData* is needed, both *nThreads* or *nProcesses* must be set to 1.
 
         *progress* is an object having a field `value`. A heavy transformation
         should periodically update this field, like this:
         :code:`progress.value = 0.5` (means 50% completion). If used with GUI,
         progress will be visualized as an expanding colored background
         rectangle in the data tree. Quick transformations do not need progress
         reporting.
 
         Should an error happen during the transformation, the error state will
-        be notified in the ParSeq status bar and the traceback will be shown in
+        be reported in the ParSeq status bar and the traceback will be shown in
         the data item's tooltip in the data tree view.
 
-        Returns True when successful.
+        Returns True when successful. If returns an int, this int will be set
+        as the data state at the destination node (the state is a dict of node
+        names).
         """
         raise NotImplementedError  # must be overridden
 
     def run_post(self, dataItems, runDownstream=True):
         # do data.calc_combined() if a member of data.combinesTo has
         # its originNode as toNode:
         toBeUpdated = []
@@ -447,42 +461,45 @@
                     toBeUpdated.append(d)
         if toBeUpdated:
             for d in toBeUpdated:
                 d.calc_combined()
             if self.fromNode.name == self.toNode.name:
                 self.run(dataItems=toBeUpdated, runDownstream=False)
 
+        for data in dataItems:
+            data.make_corrections(self.toNode)
+
         if self.sendSignals:
             csi.mainWindow.afterTransformSignal.emit(self.toNode.widget)
         if hasattr(self.toNode, 'widget'):
             if self.toNode.widget is not None:
                 self.toNode.widget.onTransform = False
 
         if runDownstream:
             for tr in self.toNode.transformsOut:
                 if self is tr:
                     continue
                 newItems = dataItems.copy()
                 newItems += [it for it in toBeUpdated if it not in newItems]
-                for data in dataItems:
-                    if data.branch is not None:
-                        newItems += [it for it in data.branch.get_items()
-                                     if it not in newItems]
+                # for data in dataItems:
+                #     if data.branch is not None:
+                #         newItems += [it for it in data.branch.get_items()
+                #                      if it not in newItems]
                 tr.run(dataItems=newItems)
 
 
 class GenericProcessOrThread(object):
     def __init__(self, func, inArrays, outArrays):
         self.func = func
         self.inArrays = inArrays
         self.outArrays = outArrays
         # self.started_event.clear()
         # self.finished_event.clear()
 
-    @logger(minLevel=20, attrs=[(1, 'alias')])
+    @logger(minLevel=20, attrs=[(0, 'transformName'), (1, 'alias')])
     def put_in_data(self, item):
         res = {'transformParams': item.transformParams,
                'alias': item.alias}
         for key in self.inArrays:
             try:
                 # if not hasattr(item, key):
                 #     setattr(item, key, None)
@@ -492,46 +509,49 @@
                 print('{0} for spectrum {1}'.format(e, item.alias))
                 # raise e
                 return False
                 # res[key] = None
         self.inDataQueue.put(res)
         return True
 
-    @logger(minLevel=20)
+    @logger(minLevel=20, attrs=[(0, 'transformName')])
     def get_in_data(self, item):
         outDict = retry_on_eintr(self.inDataQueue.get)
         for field in outDict:
             setattr(item, field, outDict[field])
 
-    @logger(minLevel=20, attrs=[(1, 'alias')])
+    @logger(minLevel=20, attrs=[(0, 'transformName'), (1, 'alias')])
     def put_out_data(self, item):
         res = {'transformParams': item.transformParams}
         for key in self.outArrays:
             try:
                 res[key] = getattr(item, key)
             except AttributeError:  # arrays can be conditionally missing
                 pass
         self.outDataQueue.put(res)
 
-    @logger(minLevel=20, attrs=[(1, 'alias')])
+    @logger(minLevel=20, attrs=[(0, 'transformName'), (1, 'alias')])
     def get_out_data(self, item):
         outDict = retry_on_eintr(self.outDataQueue.get)
         for field in outDict:
             setattr(item, field, outDict[field])
 
     def put_results(self, obj):
         self.resultQueue.put(obj)
 
-    @logger(minLevel=20, attrs=[(1, 'name')])
+    @logger(minLevel=20, attrs=[(0, 'transformName'), (1, 'name')])
     def get_results(self, obj):
         res = retry_on_eintr(self.resultQueue.get)
-        if isinstance(res, dict):
+        if res is None:
+            return False
+        elif isinstance(res, dict):
             for field in res:
                 setattr(obj, field, res[field])
-        return res is not None
+            return True
+        return res
 
     def put_error(self, obj):
         self.errorQueue.put(obj)
 
     def get_error(self):
         return retry_on_eintr(self.errorQueue.get)
 
@@ -543,15 +563,15 @@
         try:
             while not self.progressQueue.empty():
                 values.append(retry_on_eintr(self.progressQueue.get_nowait))
         except Exception:
             pass
         return values
 
-    @logger(minLevel=20, printClass=True)
+    # @logger(minLevel=20, printClass=True)
     def run(self):
         # self.started_event.set()
         np.seterr(all='raise')
         data = DataProxy()
         self.get_in_data(data)
         try:
             args = getargspec(self.func)[0]
@@ -601,15 +621,17 @@
             else:
                 raise
 
 
 class DataProxy(object):
     """An empty object to attach fields to it. With a simple instance of
     object() this is impossible but doable with an empty class."""
-    pass
+
+    def __repr__(self):
+        return "DataProxy object for '{0}'".format(self.alias)
 
 
 class BackendProcess(GenericProcessOrThread, multiprocessing.Process):
     def __init__(self, func, transformName, inArrays, outArrays,
                  progressTimeDelta):
         multiprocessing.Process.__init__(self)
         self.transformName = transformName
@@ -619,16 +641,21 @@
         self.inDataQueue = multiprocessing.Queue()
         self.outDataQueue = multiprocessing.Queue()
         self.resultQueue = multiprocessing.Queue()
         self.errorQueue = multiprocessing.Queue()
         # self.started_event = multiprocessing.Event()
         # self.finished_event = multiprocessing.Event()
         self.progressQueue = multiprocessing.Queue()
+        sys.path.append(csi.parseqPath)  # to find parseq in multiprocessing
         GenericProcessOrThread.__init__(self, func, inArrays, outArrays)
 
+    def run(self):
+        sys.path.append(csi.parseqPath)  # to find parseq in multiprocessing
+        GenericProcessOrThread.run(self)
+
 
 class BackendThread(GenericProcessOrThread, threading.Thread):
     def __init__(self, func, transformName, inArrays, outArrays,
                  progressTimeDelta):
         threading.Thread.__init__(self)
         self.transformName = transformName
         self.progressTimeDelta = progressTimeDelta
@@ -661,17 +688,18 @@
     toBeUpdated = []
     for item in items:
         if isinstance(item.madeOf, (list, tuple)):  # combined
             newMadeOf = []
             for itemName in item.madeOf:
                 if isinstance(itemName, str):
                     dataItem = parentItem.find_data_item(itemName)
-                    newMadeOf.append(dataItem)
-                    if item not in dataItem.combinesTo:
-                        dataItem.combinesTo.append(item)
+                    if dataItem is not None:
+                        newMadeOf.append(dataItem)
+                        if item not in dataItem.combinesTo:
+                            dataItem.combinesTo.append(item)
             if newMadeOf:
                 item.madeOf = newMadeOf
                 toBeUpdated.append(item)
     try:
         for d in toBeUpdated:
             d.calc_combined()
     except AttributeError:
```

## Comparing `parseq-2023.5.0/parseq/fits/basefit.py` & `parseq-2024.5.0/parseq/fits/basefit.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     nProcesses = 1
     progressTimeDelta = 1.0  # sec
     defaultResult = dict(R=1., mesg='', ier=None, info={}, nparam=0)
     # dataAttrs = dict(x='e', y='mu', fit='fit')
     # allDataAttrs = dict(x='e', y='mu')
     plotParams = dict(fit=dict(linewidth=1.5, linestyle=':'),
                       residue=dict(linewidth=1.5, linestyle='--'))
-    tooltip = ""
+    tooltip = ''
 
     def __init__(self, node=None, widgetClass=None):  # node is None in test
         """
         *node* is instance of :class:`.core.nodes.Node`.
 
         *widgetClass* optional, widget class, descendant of
         :class:`.gui.fits.gbasefit.FitWidget`.
@@ -90,15 +90,20 @@
         isStatic = isinstance(getattr_static(self, "run_main"), staticmethod)
         isClass = isinstance(getattr_static(self, "run_main"), classmethod)
         if not (isStatic or isClass):
             raise NotImplementedError(
                 "The method run_main() of {0} must be declared with either"
                 "@staticmethod or @classmethod".format(self.__class__))
 
-        self.node = node
+        if isinstance(node, (list, tuple)):
+            self.node = node[0]
+            if len(node) > 1:
+                self.extraNodes = node[1:]
+        else:
+            self.node = node
         self.widgetClass = widgetClass
         if self.name in csi.fits:
             raise ValueError("A fit '{0}' already exists. Only one instance "
                              "is allowed".format(self.name))
         csi.fits[self.name] = self
         self.sendSignals = False
         self.read_ini_params()
@@ -245,17 +250,19 @@
     def run(self, params={}, updateUndo=True, dataItems=None):
         np.seterr(all='raise')
         items = dataItems if dataItems is not None else csi.selectedItems
         self.run_pre(params, items, updateUndo)
 
         nC = multiprocessing.cpu_count()
         if isinstance(self.nThreads, type('')):
-            self.nThreads = nC//2 if self.nThreads.startswith('h') else nC
+            self.nThreads = max(nC//2, 1) if self.nThreads.startswith('h')\
+                else nC
         if isinstance(self.nProcesses, type('')):
-            self.nProcesses = nC//2 if self.nProcesses.startswith('h') else nC
+            self.nProcesses = max(nC//2, 1) if self.nProcesses.startswith('h')\
+                else nC
 
         if self.nThreads > 1:
             workerClass = BackendThread
             cpus = self.nThreads
         elif self.nProcesses > 1:
             workerClass = BackendProcess
             cpus = self.nProcesses
@@ -270,18 +277,19 @@
                 'IMPORTANT: remove "self" from "run_main()" parameters as'
                 ' this is a static method, not an instance method!')
         if 'allData' in args:
             allData = []
             for data in csi.allLoadedItems:
                 proxy = DataProxy()
                 proxy.alias = str(data.alias)
-                xname = self.allDataAttrs['x']
-                setattr(proxy, xname, getattr(data, xname))
-                yname = self.allDataAttrs['y']
-                setattr(proxy, yname, getattr(data, yname))
+                if hasattr(self, 'allDataAttrs'):
+                    xname = self.allDataAttrs['x']
+                    setattr(proxy, xname, getattr(data, xname))
+                    yname = self.allDataAttrs['y']
+                    setattr(proxy, yname, getattr(data, yname))
                 allData.append(proxy)
 
         inArrays = [self.dataAttrs['x'], self.dataAttrs['y']]
         outArrays = [self.dataAttrs['fit']]
         for data in items:
             if workerClass is not None:  # with multipro
                 worker = workerClass(
@@ -384,15 +392,16 @@
 
     @logger(minLevel=20)
     def get_in_all_data(self):
         return retry_on_eintr(self.allDataQueue.get)
 
     @logger(minLevel=20, attrs=[(1, 'alias')])
     def put_in_data(self, item):
-        res = {'fitParams': item.fitParams, 'alias': item.alias}
+        res = {'fitParams': item.fitParams, 'alias': item.alias,
+               'transformParams': item.transformParams}
         for key in self.inArrays:
             try:
                 # if not hasattr(item, key):
                 #     setattr(item, key, None)
                 res[key] = getattr(item, key)
             except AttributeError as e:
                 print('Error in put_in_data():')
```

## Comparing `parseq-2023.5.0/parseq/fits/functionfit.py` & `parseq-2024.5.0/parseq/fits/functionfit.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         tie = {}
         try:
             for k, v in fitVars.items():
                 if 'tie' in v:
                     tieStr = v['tie']
                     if not cls.can_interpret_tie_str(tieStr, fitVars):
                         raise ValueError(f'wrong tie expression for {k}')
-                    tie[k] = v['value'] if tieStr.startswith('f') else tieStr
+                    tie[k] = v['value'] if tieStr.startswith('fix') else tieStr
                     # if tieStr[0] in '<>' then k is in both tie and varied
                     if tieStr[0] not in '<>':
                         continue
                 vMin, vMax = v['lim'] if 'lim' in v else (-np.inf, np.inf)
                 if vMin < vMax:
                     varied.append(k)
                     args.append(v['value'])
@@ -96,19 +96,21 @@
                     tie[k] = vMin
                     v['value'] = vMin
 
             where = (xRange[0] <= x) & (x <= xRange[1]) \
                 if isinstance(xRange, (list, tuple)) else None
             locx = x[where]
             locy = y[where]
+            fcounter = {'nfev': 0}
             popt, pcov, info, mesg, ier = curve_fit(
                 partial(cls.evaluate_formula, formula=formula,
-                        keys=varied, tie=tie),
+                        keys=varied, tie=tie, fcounter=fcounter),
                 locx, locy, p0=args, bounds=(mins, maxs), full_output=True)
-            info2 = {'nfev': info['nfev']}
+            # info2 = {'nfev': info['nfev']}
+            info2 = fcounter
             fitProps = dict(mesg=mesg, ier=ier, info=info2, nparam=len(popt))
             tieRes = {}
             fit = cls.evaluate_formula(x, *popt, formula=formula,
                                        keys=varied, tie=tie, tieRes=tieRes)
             fitProps['R'] = ((locy - fit[where])**2).sum() / (locy**2).sum()
 
             perr = np.sqrt(np.diag(pcov))
@@ -128,28 +130,31 @@
             fitProps['mesg'] = str(e)
 
         setattr(data, cls.dataAttrs['fit'], fit)
         dfparams['ffit_result'] = fitProps
 
     @classmethod
     def can_interpret_tie_str(cls, tieStr, fitVars):
-        if tieStr.startswith('f'):
+        if tieStr.startswith('fix'):  # fixed
             return True
         if tieStr[0] not in '=<>':
             return False
         for k, v in fitVars.items():
             locals()[k] = v['value']
         try:
             eval(tieStr[1:])
             return True
         except Exception:
             return False
 
     @classmethod
-    def evaluate_formula(cls, x, *params, formula, keys, tie={}, tieRes={}):
+    def evaluate_formula(cls, x, *params, formula, keys, tie={}, tieRes={},
+                         fcounter={}):
+        if fcounter:
+            fcounter['nfev'] += 1
         res = 0.
         for key, param in zip(keys, params):
             locals()[key] = param
         for key, param in tie.items():
             if isinstance(param, str):
                 val = eval(param[1:])
                 if (param[0] == '=' or
```

## Comparing `parseq-2023.5.0/parseq/fits/lcf.py` & `parseq-2024.5.0/parseq/fits/lcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,16 @@
                 refs[k] = dict(x=xref, y=yref)
 
                 wantVary = True
                 if 'wtie' in v:
                     tieStr = v['wtie']
                     if not cls.can_interpret_LCF_tie_str(tieStr, lcf):
                         raise ValueError('wrong tie expr for w[{0}]'.format(k))
-                    refs[k]['w'] = v['w'] if tieStr.startswith('f') else tieStr
+                    refs[k]['w'] = v['w'] if tieStr.startswith('fix') else \
+                        tieStr
                     refs[k]['wtie'] = tieStr
                     # if tieStr[0] in '<>' then w is both tied and varied
                     if tieStr[0] not in '<>':
                         wantVary = False
                 if wantVary:
                     wMin, wMax = v['wBounds'][:2]
                     if wMin < wMax:
@@ -134,15 +135,15 @@
                     k = v['name']
                     wantVary = True
                     if kdt in v:
                         tieStr = v[kdt]
                         if not cls.can_interpret_LCF_tie_str(tieStr, lcf):
                             raise ValueError(
                                 'wrong tie expr for {0}[{1}]'.format(kd, k))
-                        refs[k][kd] = v[kd] if tieStr.startswith('f') else \
+                        refs[k][kd] = v[kd] if tieStr.startswith('fix') else \
                             tieStr
                         refs[k][kdt] = tieStr
                         # if tieStr[0] in '<>' then dE is both tied and varied
                         if tieStr[0] not in '<>':
                             wantVary = False
                     if wantVary:
                         dEMin, dEMax = v[kd+'Bounds'][:2]
@@ -156,18 +157,20 @@
                             refs[k][kd] = float(dEMin)
                             v[kd] = dEMin
 
             where = (xRange[0] <= x) & (x <= xRange[1]) \
                 if isinstance(xRange, (list, tuple)) else None
             locx = x[where]
             locy = y[where]
+            fcounter = {'nfev': 0}
             wopt, pcov, info, mesg, ier = curve_fit(partial(
-                cls.linear_combination, refs=refs),
+                cls.linear_combination, refs=refs, fcounter=fcounter),
                 locx, locy, p0=args, bounds=(mins, maxs), full_output=True)
-            info2 = {'nfev': info['nfev']}
+            # info2 = {'nfev': info['nfev']}
+            info2 = fcounter
             lcfProps = dict(mesg=mesg, ier=ier, info=info2, nparam=len(wopt))
             fit = cls.linear_combination(x, *wopt, refs=refs)
             lcfProps['R'] = ((locy - fit[where])**2).sum() / (locy**2).sum()
 
             werr = np.sqrt(np.diag(pcov))
             for v in lcf:
                 if not v['use']:
@@ -206,24 +209,45 @@
             lcfProps = dict(cls.defaultResult)
             lcfProps['mesg'] = str(e)
 
         setattr(data, cls.dataAttrs['fit'], fit)
         dfparams['lcf_result'] = lcfProps
 
     @classmethod
-    def linear_combination(cls, x, *params, refs):
+    def can_interpret_LCF_tie_str(cls, tieStr, lcf):
+        if tieStr.startswith('fix'):  # fixed
+            return True
+        if tieStr[0] not in '=<>':
+            return False
+        w = [0]  # w list indexing is 1-based
+        if cls.xVary:
+            dx = [0]  # dE list indexing is 1-based
+        for ref in lcf:
+            w.append(ref['w'])
+            if cls.xVary:
+                dx.append(ref['dx'])
+        try:
+            eval(tieStr[1:])
+            return True
+        except Exception:
+            return False
+
+    @classmethod
+    def linear_combination(cls, x, *params, refs, fcounter={}):
         """
         *x* : array of energy of the fitted spectrum,
 
         *params*: sequence of fitting parameters, weights and energy shifts,
 
         *refs*: dict of [ref name]: dict with keys 'x', 'y', 'w', 'dx'
         The values of 'w' and 'dx' are indices of *params* list.
         """
 
+        if fcounter:
+            fcounter['nfev'] += 1
         w = [0]  # w list indexing is 1-based for tie formulae
         for ref in refs.values():
             wr = ref['w']
             w.append(params[wr] if isinstance(wr, int) else
                      wr if isinstance(wr, float) else 0.)
         kd = 'dx'
         if cls.xVary:
@@ -259,26 +283,7 @@
                             sh = val
                             ref['shres'] = val
             f = interpolate.interp1d(
                 xref+sh, yref, kind='linear', copy=False,
                 fill_value='extrapolate', assume_sorted=True)
             res += wi * f(x)
         return res
-
-    @classmethod
-    def can_interpret_LCF_tie_str(cls, tieStr, lcf):
-        if tieStr.startswith('f'):  # fixed
-            return True
-        if tieStr[0] not in '=<>':
-            return False
-        w = [0]  # w list indexing is 1-based
-        if cls.xVary:
-            dx = [0]  # dE list indexing is 1-based
-        for ref in lcf:
-            w.append(ref['w'])
-            if cls.xVary:
-                dx.append(ref['dx'])
-        try:
-            eval(tieStr[1:])
-            return True
-        except Exception:
-            return False
```

## Comparing `parseq-2023.5.0/parseq/gui/aboutDialog.py` & `parseq-2024.5.0/parseq/gui/aboutDialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 __author__ = "Konstantin Klementiev"
-__date__ = "28 May 2023"
+__date__ = "21 Nov 2023"
 # !!! SEE CODERULES.TXT !!!
 
 import os
 import os.path as osp
 import numpy as np
 import re
 import sphinx
 from silx.gui import qt
 from silx import version as versilx
 import platform as pythonplatform
+import multiprocessing
 import webbrowser
 
 from ..core import singletons as csi
 from . import gcommons as gco
 from . import webWidget as gww
 # path to ParSeq:
 import sys; sys.path.append(osp.join('..', '..'))  # analysis:ignore
@@ -30,14 +31,16 @@
 except ImportError:
     isOpenCL = False
     isOpenStatus = redStr.format('not found')
 except cl.LogicError:
     isOpenCL = False
     isOpenStatus = 'is installed '+redStr.format('but no OpenCL driver found')
 
+nC = multiprocessing.cpu_count()
+
 PARSEQPATH = osp.dirname(osp.dirname(osp.abspath(__file__)))
 ICONPATHP = osp.join(osp.dirname(__file__), '_images', 'parseq.ico')
 ICONPATHR = osp.join(osp.dirname(__file__), '_images', 'icon-info.png')
 
 
 class AboutDialog(qt.QDialog):
     def __init__(self, parent):
@@ -70,18 +73,28 @@
         layout.addWidget(self.tabBar)
         layout.setSpacing(0)
         layout.addWidget(self.webView)
         self.setLayout(layout)
         self.resize(0, 0)
 
     def makeWebView(self):
+        path = csi.appPath
+        self.prFiles = []
+        for root, dirs, files in os.walk(path):
+            for file in files:
+                if file.endswith(".pspj"):
+                    pr = os.path.join(root, file)
+                    self.prFiles.append(
+                        osp.relpath(pr, path).replace('\\', '/'))
+
         self.webView = gww.QWebView(self)
         self.webView.page().setLinkDelegationPolicy(2)
         self.webView.setMinimumWidth(560)
-        self.webView.setMinimumHeight(450+30*len(csi.nodes))
+        self.webView.setMinimumHeight(
+            480 + 30*len(csi.nodes) + 15*len(self.prFiles))
         self.webView.history().clear()
         self.webView.page().history().clear()
         self.lastBrowserLink = ''
         self.webView.page().linkClicked.connect(
             self.linkClicked, type=qt.Qt.UniqueConnection)
 
         self.sphinxThread = qt.QThread(self)
@@ -97,14 +110,18 @@
     def _on_sphinx_html_ready(self):
         self.canLoadHTML = True
         currentIndex = 1
         self.tabBar.setCurrentIndex(currentIndex)
         self.changePage(currentIndex)
 
     def makeTextMain(self):
+        # https://stackoverflow.com/a/69325836/2696065
+        def isWin11():
+            return True if sys.getwindowsversion().build > 22000 else False
+
         if qt.BINDING.lower().startswith('pyside2'):
             import PySide2.QtCore
             Qt_version = PySide2.QtCore.qVersion()
             PyQt_version = PySide2.__version__
         elif qt.BINDING.lower().startswith('pyside6'):
             import PySide6.QtCore
             Qt_version = PySide6.QtCore.qVersion()
@@ -119,14 +136,18 @@
             except AttributeError:  # no platform.linux_distribution in py3.8
                 try:
                     import distro
                     locos = " ".join(distro.linux_distribution())
                 except ImportError:
                     print("do 'pip install distro' for a better view of Linux"
                           " distro string")
+        elif 'Windows' in locos:
+            if isWin11():
+                locos = 'Windows 11'
+
         if isOpenCL:
             vercl = cl.VERSION
             if isinstance(vercl, (list, tuple)):
                 vercl = '.'.join(map(str, vercl))
         else:
             vercl = isOpenStatus
         strNumpy = r'numpy {0}'.format(np.__version__)
@@ -178,14 +199,27 @@
             parseq.__synopsis__, parseq.__doc__, strParSeq, parseqversion,
             locos, pythonplatform.python_version(),
             Qt_version, qt.BINDING, PyQt_version,
             strNumpy, strOpenCL, strSphinx, strSilx)
 #        txt = txt.replace('imagezoom::', 'image::')
         return txt
 
+    def makeThreadProcessStr(self, nThreads, nProcesses):
+        if isinstance(nThreads, type('')):
+            nThreads = max(nC//2, 1) if nThreads.startswith('h') else nC
+        if isinstance(nProcesses, type('')):
+            nProcesses = max(nC//2, 1) if nProcesses.startswith('h') else nC
+
+        res = ''
+        if nProcesses > 1:
+            res = ' ({0} processes)'.format(nProcesses)
+        elif nThreads > 1:
+            res = ' ({0} threads)'.format(nThreads)
+        return res
+
     def makeGraphPipeline(self):
         ranks = {}
         for i in range(len(csi.nodes)):
             nodes = []
             transforms = []
             icons = []
             fits = {}
@@ -198,22 +232,24 @@
                     elif node.plotDimension < 4:
                         iName = 'icon-item-{0}dim-32'.format(
                             node.plotDimension)
                     else:
                         iName = 'icon-item-ndim-32'
                     icons.append(iName)
                     for tr in node.transformsOut:
-                        transforms.append(
-                            [tr.name, tr.fromNode.name, tr.toNode.name])
+                        trEntry = [tr.name, tr.fromNode.name, tr.toNode.name,
+                                   tr.nThreads, tr.nProcesses]
+                        transforms.append(trEntry)
                     for fit in csi.fits.values():
                         if fit.node is node:
+                            fitEntry = [fit.name, fit.nThreads, fit.nProcesses]
                             if name in fits:
-                                fits[name].append(fit.name)
+                                fits[name].append(fitEntry)
                             else:
-                                fits[name] = [fit.name]
+                                fits[name] = [fitEntry]
 
             ranks[i] = dict(nodes=nodes, icons=icons, transforms=transforms,
                             fits=fits)
 
         # ranks = {  # a fake test pipeline
         #     0: {'nodes': ['aaaaa', 'bbbbbbbbb'],
         #         'transforms': [['tr ac jhvcqwvedvsd', 'aaaaa', 'cccc'],
@@ -268,18 +304,20 @@
                     '<img src="_images/{0}.png" height="20" />'.format(iName)
                 flowChart += u"""\n
                     <div id="pn_{0}" class="pipeline-node">{1} {2}""".format(
                     name_, iconTxt, name)
                 if name in fits:
                     ficonTxt = '<img src="_images/{0}.png" height="20" />'\
                         .format(fitIcon)
-                    for fitName in fits[name]:
-                        flowChart += u"""&nbsp <span id=
-                            "fn_{0}" class="pipeline-fit">{1} {2}</span>"""\
-                                .format(name_, ficonTxt, fitName)
+                    for fit in fits[name]:
+                        fitName = fit[0]
+                        thr_pr = self.makeThreadProcessStr(fit[1], fit[2])
+                        flowChart += u"""&nbsp <span id="fn_{0}"
+                            class="pipeline-fit">{1} {2} {3}&nbsp</span>"""\
+                                .format(name_, ficonTxt, fitName, thr_pr)
                 flowChart += "</div>"
             flowChart += """\n      </div>"""  # class="pipeline-rank"
 
             transforms = rankDict['transforms']
             if not transforms:
                 continue
             flowChart += """\n      <div class="pipeline-transforms">"""
@@ -287,77 +325,88 @@
                 flowChart += u"""\n        <div class="pipeline-tr" ></div>"""
             for transform in transforms:
                 iline_ = iline % len(gco.colorCycle1)
                 color = gco.colorCycle1[iline_]
                 colorStr = \
                     'style="color: {0}; text-shadow: 1px 1.5px 3px {0}99;"'\
                     .format(color)
+                thr_pr = self.makeThreadProcessStr(transform[3], transform[4])
                 flowChart += u"""\n        <div class="pipeline-tr" {1}>
-                {0}</div>""".format(transform[0], colorStr)
+                {0}{2}</div>""".format(transform[0], colorStr, thr_pr)
                 name1_ = "_".join(transform[1].split())
                 name2_ = "_".join(transform[2].split())
                 colorStr = """style="stroke: {0}; """\
                     """marker-end: url(#arrow{1}); filter: url(#flt{1})" """\
                     .format(color, iline % len(gco.colorCycle1))
                 if name1_ == name2_:
                     flowChart += u"""\n
             <svg><path id="arc_{0}" node=pn_{1} class="shadow" {2} />
             </svg>""".format(iline, name1_, colorStr)
                 else:
                     flowChart += u"""\n
             <svg><line id="line_{0}" node1=pn_{1} node2=pn_{2} class="shadow"
+            transform="translate(0, 0)"
             {3} /></svg>""".format(iline, name1_, name2_, colorStr)
                 iline += 1
             flowChart += """\n      </div>"""  # class="pipeline-rank"
         flowChart += u"""\n
     </div>"""  # </div class="pipeline">
         return flowChart
 
     def makeTextPipeline(self):
         iconPath = csi.appIconPath
         path = csi.appPath
         if os.name == 'nt':
             iconPath = iconPath.replace('\\', '/')
-            path = path.replace('\\', '/')
         elif os.name.startswith('posix'):
             iconPath = '/' + iconPath
 
+        if self.prFiles:
+            testStr = """
+Test it as::
+
+"""
+            for prFile in self.prFiles:
+                testStr += """
+        python {0} -p {1}""".format(sys.argv[0], prFile)
+        else:
+            testStr = ""
         flowChart = self.makeGraphPipeline()
         txt = u"""
 .. list-table::
    :widths: 25 75
 
    * - |ico|
      - |synopsis|
 
 .. |ico| image:: {0}
    :scale: {1:.0%}
 
 .. |synopsis| replace::
    :bigger:`{2}`
 
-.. inheritance-diagram:: sphinx.ext.inheritance_diagram.InheritanceDiagram
-
 .. raw:: html
 
    {3}
 
 {4}
 
+{5}
+
 :Created by:
-    {5}
-:License:
     {6}
-:Located at:
+:License:
     {7}
-:Version:
+:Located at:
     {8}
+:Version:
+    {9}
     """.format(iconPath, csi.appIconScale, csi.appSynopsis, flowChart,
-               csi.appDescription, csi.appAuthor, csi.appLicense, path,
-               csi.appVersion)
+               csi.appDescription, testStr, csi.appAuthor, csi.appLicense,
+               path.replace('\\', '/'), csi.appVersion)
         return txt
 
     def changePage(self, itab):
         if not self.canLoadHTML:
             return
         docName = self.tabNames[itab].replace(' ', '_')
         html = 'file:///' + osp.join(gww.DOCDIR, docName+'.html')
```

## Comparing `parseq-2023.5.0/parseq/gui/calibrateEnergy.py` & `parseq-2024.5.0/parseq/gui/calibrateEnergy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 __author__ = "Konstantin Klementiev"
-__date__ = "17 Nov 2018"
+__date__ = "28 Nov 2023"
 # !!! SEE CODERULES.TXT !!!
 
 from functools import partial
 
-from silx.gui import qt
+from silx.gui import qt, icons
 
 from ..core import singletons as csi
 # from ..core import commons as cco
 from ..core import spectra as csp
 from ..third_party import xrt
 
-HEADERS = ['reference data', 'slice', 'energy', 'DCM', 'FWHM']
-columnWidths = (114, 44, 64, 64, 54)
+HEADERS = ['ref data', 'slice', 'energy', 'DCM', 'FWHM']
+columnWidths = (80, 44, 64, 64, 54)
 
 
 class CalibrationModel(qt.QAbstractTableModel):
     def __init__(self, dataCollection=None, header=None, formatStr='{0}'):
         super().__init__()
         self.headerList = header if header is not None else []
         self.formatStr = formatStr
@@ -102,21 +102,21 @@
                 return self.headerList[section]
             else:
                 return section
         elif role == qt.Qt.TextAlignmentRole:
             return qt.Qt.AlignHCenter
         elif role == qt.Qt.ToolTipRole:
             if section == 0:
-                return('data name (alias) of elastic scans')
+                return 'data name (alias) of elastic scans'
             elif section == 1:
-                return('data slice if needed, otherwise :')
+                return 'data slice if needed, otherwise :'
             elif section == 2:
-                return('formal energy value')
+                return 'formal energy value'
             elif section == 3:
-                return('crystals for calculating\nFWHM of DCM bandwidth')
+                return 'crystals for calculating\nFWHM of DCM bandwidth'
 
     def setDataCollection(self, dataCollection=None):
         self.beginResetModel()
         if dataCollection is None:
             self.dataCollection = {}
         else:
             self.dataCollection = dict(dataCollection)
@@ -190,24 +190,30 @@
         layout = qt.QVBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
 
         layoutB = qt.QHBoxLayout()
         self.autoSetButton = qt.QPushButton('auto set references')
         # self.autoSetButton.setMinimumWidth(120)
         layoutB.addWidget(self.autoSetButton)
-        self.addButton = qt.QPushButton('add')
-        self.addButton.setMinimumWidth(int(12*csi.screenFactor))
+        # self.addButton = qt.QPushButton('add')
+        self.addButton = qt.QToolButton()
+        self.addButton.setIcon(icons.getQIcon('add'))
         self.addButton.clicked.connect(self.add)
         layoutB.addWidget(self.addButton)
-        self.clearButton = qt.QPushButton('clear')
-        self.clearButton.setMinimumWidth(int(36*csi.screenFactor))
+        # self.clearButton = qt.QPushButton('clear')
+        self.clearButton = qt.QToolButton()
+        self.clearButton.setIcon(icons.getQIcon('rm'))
+        self.clearButton.setSizePolicy(
+            qt.QSizePolicy.Minimum, qt.QSizePolicy.Minimum)
         self.clearButton.clicked.connect(self.clear)
         layoutB.addWidget(self.clearButton)
         self.acceptButton = qt.QPushButton('accept')
-        self.acceptButton.setMinimumWidth(int(46*csi.screenFactor))
+        self.acceptButton.setSizePolicy(
+            qt.QSizePolicy.Minimum, qt.QSizePolicy.Minimum)
+        # self.acceptButton.setMinimumWidth(int(46*csi.screenFactor))
         layoutB.addWidget(self.acceptButton)
         layoutB.addStretch()
 
         layout.addLayout(layoutB)
 
         self.calibrationModel = CalibrationModel(
             dataCollection, HEADERS, formatStr)
@@ -218,21 +224,21 @@
         self.setLayout(layout)
 
     def add(self):
         col = self.calibrationModel.dataCollection
         if len(col) == 0:
             col['base'] = ['none', 'none']
             col['slice'] = [':', ':']
-            col['energy'] = [9000, 10000]
+            col['energy'] = [9000.0, 10000.0]
             col['DCM'] = ['Si111', 'Si111']
             col['FWHM'] = [0, 0]
         else:
             col['base'].append('none')
             col['slice'].append(':')
-            col['energy'].append(col['energy'][-1] + 20)
+            col['energy'].append(col['energy'][-1] + 20.0)
             col['DCM'].append(col['DCM'][-1])
             col['FWHM'].append(0)
         self.calibrationModel.setDataCollection(col)
 
     def clear(self):
         self.calibrationModel.setDataCollection()
```

## Comparing `parseq-2023.5.0/parseq/gui/columnFormat.py` & `parseq-2024.5.0/parseq/gui/columnFormat.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,27 @@
         self.headerTab = self.makeHeaderTab()
         self.tabWidget.addTab(self.headerTab, 'header')
 
         self.dataLocationTab = self.makeDataLocationTab()
         ind = self.tabWidget.addTab(self.dataLocationTab, 'arrays')
         self.tabWidget.setTabToolTip(
             ind, "For HDF5/SPEC datasets: use context menu on data arrays.\n"
-            "For column files: use expressions of variables `Col1`, `Col2`, …"
+            "For column files: use expressions of variables `Col0`, `Col1`, …"
             "\n(zero-based!) or give a zero-based int column index.\n"
-            "Example: `np.log(Col6/Col7)`")
+            "numpy can be used as `np`. Example: `np.log(Col6/Col7)`")
 
         self.conversionTab = self.makeConversionTab()
         ind = self.tabWidget.addTab(self.conversionTab, 'conversion')
         self.tabWidget.setTabToolTip(
-            ind, "Give one of:\n1) a float factor,\n"
+            ind, "Give one of:\n"
+            "1) a float factor,\n"
             "2) a new str unit (not for abscissa),\n"
-            "3) transpose(*axes), e.g. transpose(2, 1, 0)\n"
-            "4) leave empty (no conversion).")
+            "3) lim(min, max) (typ. for abscissa), e.g. lim(None, 9900)\n"
+            "4) transpose(*axes), e.g. transpose(2, 1, 0)\n"
+            "5) leave empty (no conversion).")
 
         self.metadataTab = self.makeMetadataTab()
         ind = self.tabWidget.addTab(self.metadataTab, 'metadata')
         self.tabWidget.setTabToolTip(
             ind, "Give a set of hdf5 paths by using the right-click menu.\n"
             "These str fields will appear in the 'metadata' widget under the"
             " plot")
@@ -140,17 +142,19 @@
             role = self.node.get_prop(arrayName, 'role')
             if role.startswith('0'):
                 continue
             arrayLayout = qt.QHBoxLayout()
             arrayLayout.setContentsMargins(0, 0, 0, 0)
             lbl = self.node.get_prop(arrayName, 'qLabel')
             unit = self.node.get_prop(arrayName, 'qUnit')
+            ndim = self.node.get_prop(arrayName, 'ndim')
             if unit:
                 lbl += '({0})'.format(unit)
             dataLabel = qt.QLabel(lbl)
+            dataLabel.setToolTip('{0}D'.format(ndim))
             dataEdit = qt.QLineEdit()
             dataEdit.setMinimumWidth(62)
             if role == 'optional':
                 dataEdit.setPlaceholderText('non-mandatory')
             dataEdit.setSizePolicy(
                 qt.QSizePolicy.Expanding, qt.QSizePolicy.Fixed)
             self.dataEdits.append(dataEdit)
@@ -301,15 +305,15 @@
             self.tabWidget.setCurrentIndex(1)
 
     def updateProp(self):
         needReplot = False
         for it in csi.selectedItems:
             if it.hasChanged:
                 needReplot = True
-                it.read_data()
+                it.read_data(runDownstream=True)
                 it.hasChanged = False
         if needReplot:
             self.node.widget.replot(keepExtent=False)
             for subnode in self.node.downstreamNodes:
                 subnode.widget.replot(keepExtent=False)
         # print([cco.getDotAttr(it, 'dataFormat') for it in csi.selectedItems])
 
@@ -327,15 +331,23 @@
                         self.radioButtons, self.edits, self.headerKW):
                     if rb.isChecked():
                         txt = ed.text()
                         if kw == 'skiprows':
                             txt = int(txt)
                         dres[kw] = txt
 
-            cols = [edit.text() for edit in self.dataEdits]
+            # cols = [edit.text() for edit in self.dataEdits]
+            cols = []
+            for edit in self.dataEdits:
+                txt = edit.text()
+                try:
+                    txt = int(txt)
+                except Exception:
+                    pass
+                cols.append(txt)
             dres['dataSource'] = cols
             slices = [edit.text() for edit in self.sliceEdits]
             if slices.count('') != len(slices):
                 dres['slices'] = slices
             convs = [try_float(edit.text()) for edit in self.conversionEdits]
             dres['conversionFactors'] = convs
             dres['metadata'] = ', '.join(self.metadata.keys())
```

## Comparing `parseq-2023.5.0/parseq/gui/combineSpectra.py` & `parseq-2024.5.0/parseq/gui/combineSpectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,21 +106,23 @@
         if ind == cco.COMBINE_PCA:
             msgBox = qt.QMessageBox()
             msgBox.information(self, 'Not implemented',
                                'PCA is not implemented yet',
                                buttons=qt.QMessageBox.Close)
             return
             nPCA = self.combineN.value()  # !!! TODO !!!
-#        isStopHere = self.stopHereCB.checkState() == qt.Qt.Checked
+        # isStopHere = self.stopHereCB.checkState() == qt.Qt.Checked
         isStoppedAt = self.combineStopCB.checkState() == qt.Qt.Checked
         kw = dict(dataFormat={'combine': ind}, colorTag=ind,
                   originNodeName=self.node.name, runDownstream=False)
         if isStoppedAt:
             for it in csi.selectedItems:
                 it.terminalNodeName = self.combineStop.currentText()
+                it.colorTag = 0
+                it.set_auto_color_tag()
         isMoveToGroup = self.combineMoveToGroupCB.checkState() == qt.Qt.Checked
         model = self.node.widget.tree.model()
 
         model.beginResetModel()
         first = csi.selectedItems[0]
         pit = first.parentItem
         newItem = pit.insert_item(list(csi.selectedItems), first.row(), **kw)
```

## Comparing `parseq-2023.5.0/parseq/gui/dataRebin.py` & `parseq-2024.5.0/parseq/gui/dataRebin.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/dataTreeModelView.py` & `parseq-2024.5.0/parseq/gui/dataTreeModelView.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,25 +238,29 @@
 
     def selectItems(self, items=None):
         mode = qt.QItemSelectionModel.Select | qt.QItemSelectionModel.Rows
         if items is None:
             items = self.rootItem.get_items()
         elif not isinstance(items, (list, tuple)):
             items = [items]
+        selection = None
         for i, item in enumerate(items):
             row = item.row()
             index = self.createIndex(row, 0, item)
             if i == 0:
                 selection = qt.QItemSelection(index, index)
             else:
                 selection.select(index, index)
+        if selection is None:
+            return
         csi.selectionModel.select(selection, mode)
         csi.selectionModel.setCurrentIndex(index, mode)
-        csi.selectedItems[:] = []
-        csi.selectedItems.extend(items)
+        # csi.selectedItems[:] = []
+        # csi.selectedItems.extend(items)
+        csi.selectedItems = list(items)
 
     def _removeFromGlobalLists(self, item):
         for ll in (csi.selectedItems, csi.selectedTopItems,
                    csi.recentlyLoadedItems, csi.allLoadedItems):
             if item in ll:
                 ll.remove(item)
 
@@ -509,15 +513,16 @@
                     return "line properties (Ctrl+P)"
         elif role == qt.Qt.TextAlignmentRole:
             if section > 0:
                 return qt.Qt.AlignHCenter
 
 
 class SelectionModel(qt.QItemSelectionModel):
-    pass
+    def select(self, index, command):
+        super().select(index, command)
 
 
 class NodeDelegate(qt.QItemDelegate):
     def __init__(self, parent, nodeName=''):
         self.nodeName = nodeName
         super().__init__(parent)
 
@@ -831,14 +836,15 @@
 class DataTreeView(qt.QTreeView):
 
     transformProgress = qt.pyqtSignal(list)  # alias, progress.value
 
     def __init__(self, node=None, parent=None):
         super().__init__(parent)
         self.node = node
+        self.isDockVisible = False
         self.plotDimension = 1 if node is None else self.node.plotDimension
 
         if csi.model is None:
             csi.model = DataTreeModel()
         self.setModel(csi.model)
 
         if csi.selectionModel is None:
@@ -934,33 +940,49 @@
     def makeActions(self):
         self.actionDND = self._addAction(
             "Allow internal drag-and-drop", self.allowDND)  # , "Ctrl+D")
         self.actionDND.setCheckable(True)
 
         self.actionMoveUp = self._addAction(
             "Move up", partial(self.moveItems, +1), "Ctrl+Up")
+        iconUp = self.style().standardIcon(qt.QStyle.SP_ArrowUp)
+        self.actionMoveUp.setIcon(iconUp)
+
         self.actionMoveDown = self._addAction(
             "Move down", partial(self.moveItems, -1), "Ctrl+Down")
+        iconDown = self.style().standardIcon(qt.QStyle.SP_ArrowDown)
+        self.actionMoveDown.setIcon(iconDown)
 
         self.actionMakeGroup = self._addAction(
             "Make group", self.groupItems, "Ctrl+G")
+        iconDir = self.style().standardIcon(qt.QStyle.SP_FileDialogNewFolder)
+        self.actionMakeGroup.setIcon(iconDir)
+
         self.actionUngroup = self._addAction("Ungroup", self.ungroup, "Ctrl+U")
+        iconUn = self.style().standardIcon(qt.QStyle.SP_DockWidgetCloseButton)
+        self.actionUngroup.setIcon(iconUn)
 
         self.actionRemove = self._addAction(
             "Remove", self.removeItemsView, "Del")
+        iconDel = self.style().standardIcon(qt.QStyle.SP_DialogCloseButton)
+        self.actionRemove.setIcon(iconDel)
 
         self.actionCopyError = self._addAction(
             "Copy error traceback", self.copyError, "Ctrl+C")
+        iconT = self.style().standardIcon(qt.QStyle.SP_FileDialogContentsView)
+        self.actionCopyError.setIcon(iconT)
 
         self.actionAUCC = self._addAction(
             "Auto update collective colors", self.autoUpdateColors)
         self.actionAUCC.setCheckable(True)
 
         self.actionLines = self._addAction(
             "Line properties", self.setLines, "Ctrl+P")
+        iconL = self.style().standardIcon(qt.QStyle.SP_FileDialogDetailedView)
+        self.actionLines.setIcon(iconL)
 
     def _addAction(self, text, slot, shortcut=None):
         action = qt.QAction(text, self)
         action.triggered.connect(slot)
         if shortcut:
             action.setShortcut(qt.QKeySequence(shortcut))
         action.setShortcutContext(qt.Qt.WidgetWithChildrenShortcut)
@@ -1168,14 +1190,18 @@
         lineDialog.exec_()
 
     def _setVisibleItems(self, value, emit=True):
         if self.plotDimension == 1:
             if not csi.dataRootItem.isVisible:  # visible are those selected
                 for it in csi.selectedItems:
                     csi.model.setVisible(it, value, emit)
+                for it in csi.allLoadedItems:  # unselect the others
+                    if it in csi.selectedItems:
+                        continue
+                    csi.model.setVisible(it, False, False)
             else:
                 if emit:
                     csi.model.needReplot.emit(False, True, '_setVisibleItems')
         else:
             if value:
                 it = csi.selectedItems[0]
                 csi.model.setVisible(it, value, emit)
@@ -1183,17 +1209,18 @@
                 if csi.currentNode is self.node:
                     csi.model.setVisible(csi.dataRootItem, False, True)
                     for it in csi.selectedItems:
                         csi.model.setVisible(it, value, emit)
                     self.header().update()
 
     def selChanged(self, selected=None, deselected=None):
-        if not self.hasFocus():
+        if self.hasFocus():
+            csi.currentNode = self.node
+        if not self.isDockVisible:
             return
-        csi.currentNode = self.node
 
         selectedIndexes = csi.selectionModel.selectedRows()
         items = csi.model.getItems(selectedIndexes)
         if len(items) == 0:
             mode = qt.QItemSelectionModel.Select | qt.QItemSelectionModel.Rows
             if deselected is not None:
                 csi.selectionModel.select(deselected, mode)
@@ -1206,16 +1233,17 @@
         csi.selectedItems.extend(items)
         csi.selectedTopItems[:] = []
         csi.selectedTopItems.extend(csi.model.getTopItems(selectedIndexes))
 
         if csi.selectionModel.customSelectionMode:
             self._setVisibleItems(True, True)
 
-        if csi.mainWindow is not None:
-            csi.mainWindow.selChanged()
+        if self.hasFocus():
+            if csi.mainWindow is not None:
+                csi.mainWindow.selChanged()
 
         if csi.DEBUG_LEVEL > 0 and self.parent() is None:  # only for testing
             selNames = ', '.join([i.alias for i in csi.selectedItems])
             dataCount = len(csi.allLoadedItems)
             self.setWindowTitle('{0} total; {1}'.format(dataCount, selNames))
 
     def dragMoveEvent(self, event):
```

## Comparing `parseq-2023.5.0/parseq/gui/fileDialogs.py` & `parseq-2024.5.0/parseq/gui/fileDialogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,32 +134,39 @@
         self.previewSlider.setTickPosition(qt.QSlider.TicksAbove)
         self.previewSlider.setVisible(False)
         self.previewSlider.valueChanged.connect(self.sliderValueChanged)
         layout.addWidget(self.previewSlider)
 
         self.groups = None
         self.items = None
+        self.pipelineName = ''
+        self.pipelineToolTip = ''
         self.pms = []
         self.pmIndex = 1e6
         self.previewContent = qt.QLabel(self)
         layout.addWidget(self.previewContent, 1)
         layout.addStretch()
 
         self.setLayout(layout)
         self.setMinimumWidth(400)
 
     def resizeEvent(self, ev):
         self.updatePreview()
 
     def updatePreview(self):
-        txt = '{0} group{1}, '.format(
+        if self.pipelineName:
+            txt = '{0}, '.format(self.pipelineName)
+        else:
+            txt = ''
+        txt += '{0} group{1}, '.format(
             self.groups, 's' if self.groups > 1 else '') if self.groups else ''
         txt += '{0} item{1}'.format(
             self.items, 's' if self.items > 1 else '') if self.items else ''
         self.content.setText(txt)
+        self.content.setToolTip(self.pipelineToolTip)
 
         self.previewSlider.setVisible(len(self.pms) > 1)
         if not self.pms:
             self.previewContent.setPixmap(qt.QPixmap())
             self.previewLabel.setText('Preview')
             return
         if self.pmIndex > len(self.pms)-1:
@@ -209,18 +216,29 @@
     def updatePreview(self, path):
         if path.endswith('.pspj'):
             fname = path.replace('.pspj', '')
         else:
             return
 
         configProject = config.ConfigParser()
+        active = ''
         try:
             configProject.read(path, encoding=config.encoding)
             self.previewPanel.groups = int(configProject.get('Root', 'groups'))
             self.previewPanel.items = int(configProject.get('Root', 'items'))
+            if configProject.has_section('ParSeq Application'):
+                pName = configProject.get('ParSeq Application', 'pipelineName')
+                isOwn = pName == csi.pipelineName
+                colorStr = "#008800" if isOwn else "#ff0000"
+                self.previewPanel.pipelineName = \
+                    "<font color={0}>{1}</font>".format(colorStr, pName)
+                self.previewPanel.pipelineToolTip = '' if isOwn else \
+                    "this project file was made by another pipeline!"
+            else:
+                self.previewPanel.pipelineName = ''
             active = config.get(configProject, 'Docks', 'active', '')
         except Exception:
             pass
 
         self.previewPanel.pmIndex = 0
         self.previewPanel.pms = []
         self.previewPanel.pmNames = []
```

## Comparing `parseq-2023.5.0/parseq/gui/fileTreeModelView.py` & `parseq-2024.5.0/parseq/gui/fileTreeModelView.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,56 +4,59 @@
 extended by the hdf5 model from silx (silx.gui.hdf5.Hdf5TreeModel), so that
 hdf5 containers can be viewed in the same tree.
 """
 __author__ = "Konstantin Klementiev"
 __date__ = "2 Mar 2023"
 # !!! SEE CODERULES.TXT !!!
 
+
 import os
 import os.path as osp
 import glob
 import re
 from functools import partial
 import pickle
 import time
 import numpy as np
 import warnings
 
-os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"
+os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"  # to work with external links
 os.environ["QT_FILESYSTEMMODEL_WATCH_FILES"] = '1'  # potentially heavy load!!
-import hdf5plugin  # needed to prevent h5py's "OSError: Can't read data"
+# import hdf5plugin  # needed to prevent h5py's "OSError: Can't read data"
 
 import silx
 from distutils.version import LooseVersion  # , StrictVersion
 assert LooseVersion(silx.version) >= LooseVersion("1.1.0")
 from silx.gui import qt
 import silx.io as silx_io
 from silx.gui.hdf5.Hdf5TreeModel import Hdf5TreeModel
-from silx.gui.hdf5.NexusSortFilterProxyModel import NexusSortFilterProxyModel
 
 from ..core import commons as cco
 from ..core import singletons as csi
 from ..core import config
 from . import gcommons as gco
 
 useProxyFileModel = False  # proxy model for FileSystemWithHdf5Model
 useProxyH5Model = True  # for decoration and sorting
+if useProxyH5Model:
+    from silx.gui.hdf5.NexusSortFilterProxyModel import \
+        NexusSortFilterProxyModel
 
 NODE_FS, NODE_HDF5, NODE_HDF5_HEAD = range(3)
 LOAD_DATASET_ROLE = Hdf5TreeModel.USER_ROLE
 USE_HDF5_ARRAY_ROLE = Hdf5TreeModel.USER_ROLE + 1
 LOAD_ITEM_PATH_ROLE = Hdf5TreeModel.USER_ROLE + 2
 H5PY_OBJECT_ROLE = Hdf5TreeModel.H5PY_OBJECT_ROLE
 
 NEXUS_HDF5_EXT = [e[1:] if e.startswith('.') else e for e in
                   silx_io.utils.NEXUS_HDF5_EXT]
 # = ["h5", "nx5", "nxs",  "hdf", "hdf5", "cxi"]
 COLUMN_FILE_EXT = ["dat", "fio"]
 
-COLUMN_NAME_WIDTH = 300
+COLUMN_NAME_WIDTH = 250
 NODE_INDENTATION = 12
 
 
 def is_text_file(file_name):
     try:
         with open(file_name, 'r') as check_file:  # try open file in text mode
             check_file.read()
@@ -78,50 +81,47 @@
             return 0
         if node._Hdf5Node__child is None:
             return 0
         return node.childCount()
 
     def hasChildren(self, parent=qt.QModelIndex()):
         node = self.nodeFromIndex(parent)
-        try:  # may fail during loading
-            return node.isGroupObj()
-        except Exception:
-            return False
+        # try:  # may fail during loading
+        return node.isGroupObj()
+        # except Exception:
+        #     return False
 
     def canFetchMore(self, parent):
         node = self.nodeFromIndex(parent)
         if node is None:
             return False
-        try:
-            if not node.isGroupObj():
-                return False
-            if node._Hdf5Node__child is None:
-                return True
-        except AttributeError:
+        # try:
+        if not node.isGroupObj():
             return False
+        if node._Hdf5Node__child is None:
+            return True
+        # except AttributeError:
+        #     return False
         return True
 
     def fetchMore(self, parent):
         node = self.nodeFromIndex(parent)
         if node is None:
             return
-        # try:
         super().fetchMore(parent)
         added = 0
         for row in range(node.childCount()):
             node.child(row)
             ind = self.index(row, 0, parent)
             intId = ind.internalId()
             if intId not in self.nodesH5:
                 added += 1
                 self.nodesH5.append(intId)
         # if added:
         #     print('Added from {0}: {1}'.format(node.basename, added))
-        # except RuntimeError:
-        #     pass
 
     def findIndex(self, hdf5Obj):
         return self.index(self.h5pyObjectRow(hdf5Obj.obj), 0)
 
     def hdf5ObjFromFileName(self, filename):
         root = self.nodeFromIndex(qt.QModelIndex())
         for ic in range(root.childCount()):
@@ -278,21 +278,21 @@
             if hdf5Obj is not None:
                 return self.h5Model.findIndex(hdf5Obj)
             else:
                 return qt.QModelIndex()
         else:
             return qt.QModelIndex()
 
-    def mapH5toFS(self, indexH5):  # only for h5 heads
-        parentH5 = self.h5Model.parent(indexH5)
-        if not parentH5.isValid():
-            hdf5Obj = self.h5Model.nodeFromIndex(indexH5)
-            return self.indexFileName(hdf5Obj.obj.file.filename)
-        else:
-            return qt.QModelIndex()
+    # def mapH5toFS(self, indexH5):  # only for h5 heads
+    #     parentH5 = self.h5Model.parent(indexH5)
+    #     if not parentH5.isValid():
+    #         hdf5Obj = self.h5Model.nodeFromIndex(indexH5)
+    #         return self.indexFileName(hdf5Obj.obj.file.filename)
+    #     else:
+    #         return qt.QModelIndex()
 
     def rowCount(self, parent=qt.QModelIndex()):
         nodeType = self.nodeType(parent)
         if nodeType == NODE_FS:
             return super().rowCount(parent)
         elif nodeType == NODE_HDF5_HEAD:
             return self.h5Model.rowCount(self.mapFStoH5(parent))
@@ -327,16 +327,16 @@
             # raise ValueError('unknown node type in `hasChildren`')
 
     def canFetchMore(self, parent):
         nodeType = self.nodeType(parent)
         if nodeType == NODE_FS:
             return super().canFetchMore(parent)
         elif nodeType == NODE_HDF5_HEAD:
-            # return self.h5Model.canFetchMore(self.mapFStoH5(parent))
-            return True
+            return self.h5Model.canFetchMore(self.mapFStoH5(parent))
+            # return True
         elif nodeType == NODE_HDF5:
             return self.h5Model.canFetchMore(self.mapToH5(parent))
         else:
             return False
             # raise ValueError('unknown node type in `canFetchMore`')
 
     def fetchMore(self, parent):
@@ -416,14 +416,15 @@
                 self.pathReady.emit(self.pendingPath[1])
 
     def interpretArrayFormula(self, dataStr, treeObj, kind):
         """Returnes a list of (expr, d[xx]-styled-expr, data-keys, shape).
         *dataStr* may have several expressions with the syntax of a list or a
         tuple or just one expression if it is a simple string.
         """
+        dataStr = str(dataStr)
         if "np." in dataStr:
             try:
                 arr = eval(dataStr)
                 return [(dataStr, None, None, arr.shape)]
             except Exception:
                 pass
         try:
@@ -526,15 +527,15 @@
             if len(arrs) == 0:
                 return
 
             for data, nd, role in zip(dataS, nds, roles):
                 if role == 'optional':
                     lres.append('')
                     continue
-                if len(data) == 0:
+                if isinstance(data, str) and len(data) == 0:
                     return
                 colEval = self.interpretArrayFormula(data, arrs, 'col')
                 if colEval is None:
                     return
                 if nd:
                     if len(colEval[0][3]) < nd:
                         return
@@ -649,15 +650,18 @@
 
         node = self.h5Model.nodeFromIndex(indexH5)
         nodePath = self.h5Model.getHDF5NodePath(node)
         # if node.dataLink(qt.Qt.DisplayRole) == 'External':
         #     nodePath = self.h5Model.getHDF5NodePath(node)
         # else:
         #     nodePath = node.obj.name
-        return 'silx:' + '::'.join((node.obj.file.filename, nodePath))
+        try:
+            return 'silx:' + '::'.join((node.obj.file.filename, nodePath))
+        except AttributeError:
+            return
 
     def data(self, index, role=qt.Qt.DisplayRole):
         shouldSkip = False
         if csi.currentNode is not None:
             if csi.currentNode.widget.onTransform:
                 shouldSkip = True
         if shouldSkip and role in [LOAD_DATASET_ROLE, USE_HDF5_ARRAY_ROLE,
@@ -888,18 +892,20 @@
             if self.parent().comparePathWithLastLoaded(path):
                 option.font.setWeight(qt.QFont.Bold)
             # if self.parent().comparePathWithLastLoaded(path, suffix='_silx'):
             #     option.font.setWeight(qt.QFont.Bold)
 
         active = (option.state & qt.QStyle.State_Selected or
                   option.state & qt.QStyle.State_MouseOver)
-        if active:
+        if active and self.parent().transformNode:
             loadState = index.data(LOAD_DATASET_ROLE)
             cf = self.parent().transformNode.widget.columnFormat
             cf = cf.saveButton.setEnabled(loadState is not None)
+        else:
+            loadState = None
 
         if option.state & qt.QStyle.State_MouseOver:
             # color = self.parent().palette().highlight().color()
             if loadState is not None:
                 color = qt.QColor(gco.COLOR_LOAD_CAN)
             else:
                 color = qt.QColor(gco.COLOR_LOAD_CANNOT)
@@ -934,18 +940,18 @@
     def __init__(self, transformNode=None, parent=None, rootPath=''):
         super().__init__(parent)
         self.rootPath = rootPath
         self.transformNode = transformNode
 
         self.initModel()
 
-        if transformNode is not None:
-            self.setItemDelegateForColumn(0, SelectionDelegate(self))
-            if parent is not None:
-                self.parent().setMouseTracking(True)
+        self.setItemDelegateForColumn(0, SelectionDelegate(self))
+        if parent is not None:
+            self.parent().setMouseTracking(True)  # for Windows
+        self.viewport().setAttribute(qt.Qt.WA_Hover)  # for Linux
 
         # self.setMinimumSize(
         #     qt.QSize(int(COLUMN_NAME_WIDTH*csi.screenFactor), 250))
         # self.setColumnWidth(0, int(COLUMN_NAME_WIDTH*csi.screenFactor))
         self.setMinimumSize(qt.QSize(COLUMN_NAME_WIDTH, 50))
         self.setColumnWidth(0, COLUMN_NAME_WIDTH)
         self.setIndentation(NODE_INDENTATION)
@@ -964,22 +970,28 @@
         self.prevSelectedIndexes = []
         self.reloadDirFiles = {}
 
         if transformNode is not None:
             strLoad = "Load data (you can also drag it to the data tree)"
             self.actionLoad = self._addAction(
                 strLoad, self.transformNode.widget.loadFiles, "Ctrl+L")
+            iconLoad = self.style().standardIcon(qt.QStyle.SP_ArrowRight)
+            self.actionLoad.setIcon(iconLoad)
         self.actionSynchronize = self._addAction(
             "Reload location", self.reload, ["Ctrl+R", "F5"])
+        iconReload = self.style().standardIcon(qt.QStyle.SP_BrowserReload)
+        self.actionSynchronize.setIcon(iconReload)
         self.actionViewTextFile = self._addAction(
             "View text file (will be displayed in 'metadata' panel)",
             self.viewTextFile, "F3")
+        iconT = self.style().standardIcon(qt.QStyle.SP_FileDialogContentsView)
+        self.actionViewTextFile.setIcon(iconT)
 
-        self.setStyleSheet("QTreeView"
-                           "{selection-background-color: transparent;}")
+        # self.setStyleSheet("QTreeView"
+        #                    "{selection-background-color: transparent;}")
 
         # # uncomment for testing the file model:
         # from ..tests.modeltest import ModelTest
         # self.ModelTest = ModelTest
         # self.actionTestModel = self._addAction(
         #     "Test file model", self.testModel)
 
@@ -1185,18 +1197,26 @@
                     break
             else:
                 isEnabled = True
             menu.addAction(self.actionLoad)
             self.actionLoad.setEnabled(isEnabled)
 
         if lenSelectedIndexes > 1:
-            actionN = menu.addAction(
-                "Concatenate {0} datasets and load as one".format(
-                    lenSelectedIndexes))
-            actionN.setEnabled(isEnabled)
+            actionN0 = menu.addAction(
+                "Concatenate {0} datasets along 0 axis and load as one".format(
+                    lenSelectedIndexes),
+                partial(self.transformNode.widget.loadFiles,
+                        concatenate=(0, False)))
+            actionN0.setEnabled(True)
+            actionN1 = menu.addAction(
+                "Sum {0} datasets individually".format(lenSelectedIndexes) +
+                " along 0 axis, concatenate and load as one",
+                partial(self.transformNode.widget.loadFiles,
+                        concatenate=(0, True)))
+            actionN1.setEnabled(True)
 
         if self.transformNode is not None:
             formats = self.getSavedFormats()
             if formats is not None:
                 cf = self.transformNode.widget.columnFormat
                 for fmtName, fmt in formats.items():
                     strFmt = "Define data format as '{0}'".format(fmtName)
@@ -1209,14 +1229,17 @@
         if hasattr(model, 'nodeType'):  # when not with a test model
             nodeType0 = model.nodeType(ind)
             menu.addAction(self.actionSynchronize)
 
             if len(paths) > 0:
                 menu.addSeparator()
                 action = qt.QAction("Add to metadata list", menu)
+                iconL = self.style().standardIcon(
+                    qt.QStyle.SP_FileDialogDetailedView)
+                action.setIcon(iconL)
                 action.triggered.connect(partial(self.addMetadata, paths))
                 menu.addAction(action)
 
             if nodeType0 == NODE_FS:
                 # try:
                 fname = model.filePath(ind)
                 if not qt.QFileInfo(fname).isDir():
@@ -1425,20 +1448,20 @@
         group `measurement`."""
         model = self.model()
 
         if model.rowCount(index) == 1:
             child = model.index(0, 0, index)
             self.expand(child)
 
-        nodeType = model.nodeType(index)
-        if nodeType == NODE_HDF5:
-            res = model.h5Model.indexFromPath(index, 'measurement')
-            if res.isValid():
-                child = model.index(res.row(), 0, index)
-                self.expand(child)
+        # nodeType = model.nodeType(index)
+        # if nodeType == NODE_HDF5:
+        #     res = model.h5Model.indexFromPath(index, 'measurement')
+        #     if res.isValid():
+        #         child = model.index(res.row(), 0, index)
+        #         self.expand(child)
 
     # def restoreExpand(self, parent=qt.QModelIndex()):
     #     if not parent.isValid():
     #         if len(self._expandedNodes) == 0:
     #             return
     #     # try:
     #     for row in range(self.model().rowCount(parent)):
@@ -1554,15 +1577,15 @@
             defaultDropAction = qt.Qt.IgnoreAction
             dragQDrag.exec_(supportedActions, defaultDropAction)
 
     def gotoWhenReady(self, path, callback=True):
         """Going directly to a file or directory is not possible because of the
         lazy loading mechanism. This is implemented here in 3 steps:
 
-        1) Go to the containing dir. This sends reques to QFileSystemModel to
+        1) Go to the containing dir. This sends request to QFileSystemModel to
            populate it.
 
         2) When the dir is ready, QFileSystemModel emits directoryLoaded
            signal. We create hdf5 tree nodes if the dir contains hdf5 files.
 
         3) When hdf5's are ready, pathReady signal is emitted, in whose slot we
            scroll to the requested path after a delay. The view doesn't scroll
@@ -1590,18 +1613,19 @@
                 index = model.indexFromH5Path(path)
             elif pathType == NODE_FS:
                 index = model.indexFileName(path)
         else:
             model.pendingPath = (dirname, path) if callback else None
             index = model.indexFileName(dirname)
 
-        ind = self.getProxyIndex(index)
-        if ind.isValid():
-            self.scrollTo(ind, qt.QAbstractItemView.PositionAtCenter)
-            self.setCurrentIndex(ind)
+        if index.isValid():
+            ind = self.getProxyIndex(index)
+            if ind.isValid():
+                self.scrollTo(ind, qt.QAbstractItemView.PositionAtCenter)
+                self.setCurrentIndex(ind)
 
     def _gotoIsReady(self, path, delay=2500):  # ms
         """The delay can be as short as 500 ms for a stand alone treeView. In
         a bigger GUI it needs to be longer, otherwise it doesn't scroll to the
         path."""
         scrollTimer = qt.QTimer(self)
         scrollTimer.setSingleShot(True)
```

## Comparing `parseq-2023.5.0/parseq/gui/gcommons.py` & `parseq-2024.5.0/parseq/gui/gcommons.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 from silx.gui import qt, icons
 
 colorCycle1 = ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd',
                '#8c564b', '#e377c2', '#7f7f7f', '#bcbd22', '#17becf']  # mpl
 colorCycle2 = ['#0000ff', '#00ee00', '#ff0000', '#00ffff', '#ff00ff',
                '#ffff00', '#aaaaaa', '#000000']
 
-COLOR_POLICY_INDIVIDUAL, COLOR_POLICY_LOOP1, COLOR_POLICY_LOOP2,\
+COLOR_POLICY_INDIVIDUAL, COLOR_POLICY_LOOP1, COLOR_POLICY_LOOP2, \
     COLOR_POLICY_GRADIENT = range(4)
 COLOR_POLICY_NAMES = 'individual', 'loop1', 'loop2', 'gradient'
 
 COLOR_HDF5_HEAD = '#2299f0'
 COLOR_FS_COLUMN_FILE = '#32aa12'
 COLOR_LOAD_CAN = '#44c044'
 COLOR_LOAD_CANNOT = '#d03333'
 COLOR_UNDEFINED = '#ff160c'
 COLOR_ROI = '#f7b43e'
+COLOR_CORRECTION = '#ff55dd'
 COLOR_COMBINED = '#ff00ff'
 
 GROUP_COLOR = qt.QColor('#f4f0f0')
 BUSY_COLOR_BGND = qt.QColor('#ffe9a1')
 BUSY_COLOR_FGND = qt.QColor('#aaaa00')
 BAD_COLOR = qt.QColor('#f47070')
 UNDEFINED_COLOR = qt.QColor('#cccccc')
```

## Comparing `parseq-2023.5.0/parseq/gui/mainWindow.py` & `parseq-2024.5.0/parseq/gui/mainWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 __date__ = "26 Feb 2023"
 # !!! SEE CODERULES.TXT !!!
 
 # import sys
 import os.path as osp
 import time
 from functools import partial
-import hdf5plugin  # needed to prevent h5py's "OSError: Can't read data"
+# import hdf5plugin  # needed to prevent h5py's "OSError: Can't read data"
 import textwrap
 import re
 import shutil
 import psutil
 import glob
 import inspect
 import webbrowser
@@ -54,17 +54,18 @@
             self.show()
 
             # Custom title bar:
             self.titleBar = qt.QWidget(self)
             self.titleBar.setAutoFillBackground(True)
             # self.titleBar.setStyleSheet(
             #     "QWidget {font: bold; font-size: " + str(fontSize) + "pt;}")
-            pal = self.titleBar.palette()
-            pal.setColor(qt.QPalette.Window, qt.QColor("lightgray"))
-            self.titleBar.setPalette(pal)
+
+            # pal = self.titleBar.palette()
+            # pal.setColor(qt.QPalette.Window, qt.QColor("lightgray"))
+            # self.titleBar.setPalette(pal)
             height = qt.QApplication.style().pixelMetric(
                 qt.QStyle.PM_TitleBarHeight)
             self.titleBar.setMaximumHeight(height)
             layout = qt.QHBoxLayout()
             self.titleBar.setLayout(layout)
 
             bSize = height - int(16*csi.screenFactor)
@@ -131,16 +132,17 @@
 class MainWindowParSeq(qt.QMainWindow):
     intervalCPU = 2000
     beforeTransformSignal = qt.pyqtSignal(qt.QWidget)
     afterTransformSignal = qt.pyqtSignal(qt.QWidget)
     beforeDataTransformSignal = qt.pyqtSignal(list)
     afterDataTransformSignal = qt.pyqtSignal(list)
 
-    def __init__(self, parent=None):
+    def __init__(self, parent=None, tabPos=qt.QTabWidget.West):
         super().__init__(parent)
+        self.tabPos = tabPos
         csi.screenFactor = qt.qApp.desktop().logicalDpiX() / 120.
 
         selfDir = osp.dirname(__file__)
         self.iconDir = osp.join(selfDir, '_images')
         self.runIcon = qt.QIcon(osp.join(self.iconDir, 'parseq.ico'))
         # self.emptyIcon = qt.QIcon(qt.QPixmap.fromImage(qt.QImage.fromData(
         #     b'<svg version="1.1" viewBox="0 0  32"'
@@ -265,31 +267,31 @@
         self.toolbar.addAction(self.undoAction)
         self.toolbar.addAction(self.redoAction)
         self.toolbar.addSeparator()
         self.toolbar.addAction(infoAction)
         self.toolbar.addAction(helpAction)
 
     def initTabs(self):
-        self.setTabPosition(qt.Qt.AllDockWidgetAreas, qt.QTabWidget.West)
+        self.setTabPosition(qt.Qt.AllDockWidgetAreas, self.tabPos)
 
         dockFeatures = (qt.QDockWidget.DockWidgetMovable |
                         qt.QDockWidget.DockWidgetFloatable)  # |
         #                qt.QDockWidget.DockWidgetVerticalTitleBar)
         self.docks = {}  # nodeWidget: (dock, node, tabName)
         self.setDockNestingEnabled(True)
         for i, (name, node) in enumerate(csi.nodes.items()):
             tabName = u'{0} \u2013 {1}'.format(i+1, name)
             dock = QDockWidgetNoClose(tabName, self)
             dock.setAllowedAreas(qt.Qt.AllDockWidgetAreas)
             dock.setFeatures(dockFeatures)
             dock.defStyleSheet = "QDockWidget {font: bold; padding-left: 5px;}"
-            # dock.setStyleSheet(dock.defStyleSheet)
+            dock.setStyleSheet(dock.defStyleSheet)
             self.addDockWidget(qt.Qt.LeftDockWidgetArea, dock)
             nodeWidget = NodeWidget(node, dock)
-            # nodeWidget = None  # for testing fo app closure
+            # nodeWidget = None  # for testing app closure
             dock.setWidget(nodeWidget)
 
             if node.plotDimension is None:
                 dock.dimIcon = qt.QIcon()
                 dock.dimIconBusy = qt.QIcon()
             elif node.plotDimension < 4:
                 dim = node.plotDimension if node.plotDimension < 4 else 'n'
@@ -298,26 +300,32 @@
                 name = 'icon-item-{0}dim-busy-{1}.png'.format(dim, ICON_SIZE)
                 dock.dimIconBusy = qt.QIcon(osp.join(self.iconDir, name))
 
             if i == 0:
                 dock0, node0, tabName0 = dock, nodeWidget, tabName
             else:
                 self.tabifyDockWidget(dock0, dock)
+
             # the pipeline head(s) with initially opened file tree:
             first = 1 if len(node.upstreamNodes) == 0 else 0
 
             try:
                 last = 0 if node.widget.transformWidget.hideInitialView \
                     else 1
             except AttributeError:
                 last = 1
             if node.widgetClass is None:
                 last = 0
             if nodeWidget:
-                nodeWidget.splitter.setSizes([first, 1, 1, last])
+                splitterStates = [0] * nodeWidget.splitter.count()
+                splitterStates[0] = first  # files
+                splitterStates[1] = 1  # data
+                splitterStates[2] = 1  # plot
+                splitterStates[-1] = last  # transform
+                nodeWidget.splitter.setSizes(splitterStates)
             self.docks[nodeWidget] = dock, node, tabName
             dock.visibilityChanged.connect(partial(self.nodeChanged, node))
             dock.topLevelChanged.connect(dock.changeWindowFlags)
 
         for node in csi.nodes.values():
             if hasattr(node.widget.transformWidget, 'extraGUISetup'):
                 node.widget.transformWidget.extraGUISetup()
@@ -328,16 +336,17 @@
             csi.currentNode = node0.node
 
         self.tabWidget = None
         for tab in self.findChildren(qt.QTabBar):
             if tab.tabText(0) == tabName0:
                 self.tabWidget = tab
                 break
-        # self.tabWidget.setStyleSheet("QTabBar::tab { font:bold };")
-        # self.tabWidget.setStyleSheet("QTabBar::tab {padding: 4;};")
+        self.tabWidget.setStyleSheet(
+            "QTabBar::tab:selected {font:bold; "
+            "padding-left: 10; padding-right: 10;};")
 
         self.setTabIcons()
 
         self.makeHelpPages()
         self.makeDocPages()
 
     def makeHelpPages(self):
@@ -383,15 +392,16 @@
             try:
                 tSource = osp.getmtime(inspect.getfile(node.widgetClass))
                 docName = name.replace(' ', '_')
                 fname = osp.join(gww.DOCDIR, docName) + '.html'
                 if osp.exists(fname):
                     tDoc = osp.getmtime(fname)
                     shouldBuild = tSource > tDoc  # source newer than doc
-            except Exception:
+            except Exception as e:
+                print('Cannot build doc pages with error:\n{0}'.format(e))
                 pass
             if not shouldBuild:
                 continue
 
             rawTexts.append(textwrap.dedent(node.widgetClass.__doc__))
             rawTextNames.append(name)
 
@@ -471,23 +481,26 @@
         self.saveAction.setEnabled(cData > 0)
         cSelected = len(csi.selectedItems)
         if cSelected:
             self.statusBarLeft.setText('{0} selected: {1}'.format(
                 cSelected, combinedNames))
         else:
             self.statusBarLeft.setText('')
+        self.statusBarLeft.update()
         sLoaded = '{0} loaded'.format(cLoaded) if cLoaded else ''
         sBranched = '{0} branched'.format(cBranched) if cBranched else ''
         sCreated = '{0} created'.format(cCreated) if cCreated else ''
         sCombined = '{0} combined'.format(cCombined) if cCombined else ''
         ss = [s for s in (sLoaded, sBranched, sCreated, sCombined) if s]
         self.statusBarCenter.setText(', '.join(ss))
 
     def nodeChanged(self, node, visible):
         if visible:
+            if hasattr(node, 'widget'):
+                node.widget.tree.isDockVisible = True
             csi.currentNode = node
 
     def undoGroup(self):
         csi.undoGrouping = not csi.undoGrouping
 
     def _populateMenu(self, menu, iconName, actionDeque, bkgndColor,
                       closeSlot, actionSlot):
@@ -613,24 +626,27 @@
         except OSError:
             msg = qt.QMessageBox()
             msg.setIcon(qt.QMessageBox.Critical)
             msg.critical(self, "Cannot write file",
                          "Invalid file name {0}".format(fname))
             return
         self.save_project(fname)
+
+        activeNode = csi.currentNode
         for i, (name, node) in enumerate(csi.nodes.items()):
             node.widget.saveGraph(fname, i, name)
-        if len(res) < 5:
-            return
-        saveNodes, saveTypes, saveScriptMpl, saveScriptSilx = res[1:5]
-        plots, h5plots = self.save_data(fname, saveNodes, saveTypes)
-        if saveScriptMpl:
-            self.save_script(fname, plots, h5plots, 'mpl')
-        if saveScriptSilx:
-            self.save_script(fname, plots, h5plots, 'silx')
+        self.docks[activeNode.widget][0].raise_()
+
+        if len(res) > 4:
+            saveNodes, saveTypes, saveScriptMpl, saveScriptSilx = res[1:5]
+            plots, h5plots = self.save_data(fname, saveNodes, saveTypes)
+            if saveScriptMpl:
+                self.save_script(fname, plots, h5plots, 'mpl')
+            if saveScriptSilx:
+                self.save_script(fname, plots, h5plots, 'silx')
         config.put(config.configLoad, 'Project', csi.pipelineName, fname)
 
     def slotLoadProject(self):
         dlg = LoadProjectDlg(self)
         if config.configLoad.has_option('Project', csi.pipelineName):
             d = osp.dirname(config.configLoad.get('Project', csi.pipelineName))
             dlg.setDirectory(d)
```

## Comparing `parseq-2023.5.0/parseq/gui/nodeWidget.py` & `parseq-2024.5.0/parseq/gui/nodeWidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import sys
 import os.path as osp
 import webbrowser
 from collections import Counter
 from functools import partial
 import traceback
-# import time
+import time
 import glob
 
 from silx.gui import qt, colors, icons
 
 from ..core import singletons as csi
 from ..core import commons as cco
 # from ..core import spectra as csp
@@ -22,14 +22,15 @@
 from ..gui import fileTreeModelView as gft
 from ..gui.fileTreeModelView import FileTreeView
 from ..gui.dataTreeModelView import DataTreeView
 from ..gui.plot import Plot1D, Plot2D, Plot3D
 from ..gui.webWidget import QWebView
 from ..gui.columnFormat import ColumnFormatWidget
 from ..gui.combineSpectra import CombineSpectraWidget
+from ..gui.gcorrection import Correction1DWidget
 from . import gcommons as gco
 
 SPLITTER_WIDTH, SPLITTER_BUTTON_MARGIN = 14, 6
 COLORMAP = 'viridis'
 
 autoLoadDelay = 3000  # msec
 
@@ -47,14 +48,15 @@
         self.setStyleSheet("""
             QPushButton {
                 font-size: """ + fontSize + """pt; color: #151575;
                 text-align: bottom; border-radius: 6px;
                 margin: 0px 0px """ + bottomMargin + """px 0px;
                 background-color: qlineargradient(
                 """ + grad + """, stop: 0 #e6e7ea, stop: 1 #cacbce);}
+            QPushButton:disabled {color: #777777;}
             QPushButton:pressed {
                 background-color: qlineargradient(
                 """ + grad + """, stop: 0 #cacbce, stop: 1 #e6e7ea);}
             QPushButton:hover {
                 background-color: qlineargradient(
                 """ + grad + """, stop: 0 #6087cefa, stop: 1 #7097eeff);} """)
         myFont = qt.QFont()
@@ -113,49 +115,54 @@
     def __init__(self, node, parent=None):
         super().__init__(parent)
         self.mainWindow = parent
 #        self.setContentsMargins(0, 0, 0, 0)
         self.node = node
         self.helpFile = ''
         node.widget = self
+        self.correctionWidget = None
         self.transformWidget = None
         self.tree = None
         self.help = None
         self.pendingPropDialog = None
         self.wasNeverPlotted = True
         self.onTransform = False
         self.fitLines = []
 
         self.makeSplitters()
 
         self.fillSplitterFiles()
         self.fillSplitterData()
         self.fillSplitterPlot()
+        self.fillSplitterCorrection()
         self.makeTransformWidget(self.splitterTransform)
         self.fillSplitterTransform()
+
         self.makeSplitterButtons()
         self.splitter.setStretchFactor(0, 0)
         self.splitter.setStretchFactor(1, 0)
         self.splitter.setStretchFactor(2, 1)
         self.splitter.setStretchFactor(3, 0)
 
         # if not osp.exists(self.helpFile):
         if True:
             self.splitterTransform.setSizes([1, 0])
         self.splitterButtons['files && containers'].clicked.emit()
         self.splitterButtons['transform'].clicked.emit()
 
-        self.splitter.setSizes([1, 1, 1, 1])  # set in MainWindowParSeq
+        # self.splitter.setSizes([1, 1, 1, 1])  # set in MainWindowParSeq
         if len(csi.selectedItems) > 0:
             self.updateNodeForSelectedItems()
             self.replot()
         else:
-            self.gotoLastData()
+            # self.gotoLastData()  # on beamline computers may get very slow
+            pass
         # # doesn't work in Linux:
         # self.fileSystemWatcher = qt.QFileSystemWatcher(self)
+        self.setMinimumWidth(600)
 
     def gotoLastData(self):
         self.files.gotoLastData()
         if configLoad.has_section('Format_'+self.node.name):
             formats = dict(configLoad.items('Format_'+self.node.name))
             self.columnFormat.setDataFormat(formats)
 
@@ -185,14 +192,16 @@
 
         self.splitterFiles = qt.QSplitter(self.splitter)
         self.splitterFiles.setOrientation(qt.Qt.Vertical)
         self.splitterData = qt.QSplitter(self.splitter)
         self.splitterData.setOrientation(qt.Qt.Vertical)
         self.splitterPlot = qt.QSplitter(self.splitter)
         self.splitterPlot.setOrientation(qt.Qt.Vertical)
+        self.splitterCorrection = qt.QSplitter(self.splitter)
+        self.splitterCorrection.setOrientation(qt.Qt.Vertical)
         self.splitterTransform = qt.QSplitter(self.splitter)
         self.splitterTransform.setOrientation(qt.Qt.Vertical)
 
     def fillSplitterFiles(self):
         splitterInner = qt.QWidget(self.splitterFiles)
 
         labelIncludeFilter = qt.QLabel('include')
@@ -219,14 +228,16 @@
         self.autoPanel.setTitle('auto load new data from current location')
         self.autoPanel.setCheckable(True)
         self.autoPanel.setChecked(False)
         # self.autoPanel.setEnabled(False)
         self.autoPanel.toggled.connect(self.autoLoadToggled)
         self.enableAutoLoad.connect(self.autoLoadChangeEnabled)
         self.autoFileList = []
+
+        layoutAP = qt.QVBoxLayout()
         layoutA = qt.QHBoxLayout()
         layoutA.setContentsMargins(6, 0, 0, 0)
         labelA1 = qt.QLabel('auto load every')
         layoutA.addWidget(labelA1)
         self.filesAutoLoadEvery = qt.QSpinBox()
         self.filesAutoLoadEvery.setMinimum(1)
         self.filesAutoLoadEvery.setMaximum(1000)
@@ -235,15 +246,38 @@
         self.filesAutoLoadEvery.valueChanged.connect(self.autoLoadEveryChanged)
         self.autoLoadTimer = None
 
         layoutA.addWidget(self.filesAutoLoadEvery)
         labelA2 = qt.QLabel('file/dataset')
         layoutA.addWidget(labelA2)
         layoutA.addStretch()
-        self.autoPanel.setLayout(layoutA)
+        layoutAP.addLayout(layoutA)
+
+        for arrayName in self.node.arrays:
+            role = self.node.get_prop(arrayName, 'role')
+            if role.startswith('x'):
+                lbl = self.node.get_prop(arrayName, 'qLabel')
+                unit = self.node.get_prop(arrayName, 'qUnit')
+                layoutB = qt.QHBoxLayout()
+                layoutB.setContentsMargins(6, 0, 0, 0)
+                layoutB.setSpacing(0)
+                self.cbLonger = qt.QCheckBox(
+                    'only long scans Δ{0} >'.format(lbl))
+                layoutB.addWidget(self.cbLonger)
+                self.xLonger = qt.QLineEdit()
+                layoutB.addWidget(self.xLonger)
+                labelB1 = qt.QLabel(unit)
+                layoutB.addWidget(labelB1)
+                layoutB.addStretch()
+                layoutAP.addLayout(layoutB)
+                break
+        else:
+            self.cbLonger = None
+
+        self.autoPanel.setLayout(layoutAP)
 
         gotoLastButton = qt.QToolButton()
         gotoLastButton.setFixedSize(24, 24)
         gotoLastButton.setIcon(icons.getQIcon('last'))
         tt = "Go to the latest loaded data"
         if configLoad.has_option('Data', self.node.name):
             tt += "\n" + configLoad.get('Data', self.node.name)
@@ -321,18 +355,28 @@
         self.splitterPlot.setStretchFactor(0, 1)  # don't remove
         for i in range(1, self.splitterPlot.count()):
             self.splitterPlot.setStretchFactor(i, 0)
         sizes = [0] * self.splitterPlot.count()
         sizes[0] = 1
         self.splitterPlot.setSizes(sizes)
 
+    def fillSplitterCorrection(self):
+        if self.node.plotDimension == 1:
+            self.correctionWidget = Correction1DWidget(
+                self.splitterCorrection, self.node, self.plot,
+                ['CorrectionDelete', 'CorrectionScale',
+                 'CorrectionSpline', 'CorrectionStep'])
+            po = qt.QSizePolicy(
+                qt.QSizePolicy.Preferred, qt.QSizePolicy.Preferred)
+            self.correctionWidget.setSizePolicy(po)
+
     def fillSplitterTransform(self):
         self.help = QWebView(self.splitterTransform)
         # self.help.setHtml('no documentation available')
-        self.help.setMinimumSize(qt.QSize(100, 5))
+        self.help.setMinimumSize(qt.QSize(50, 5))
         self.help.page().setLinkDelegationPolicy(2)
         self.help.history().clear()
         self.help.page().history().clear()
         self.lastBrowserLink = ''
         self.help.page().linkClicked.connect(
             self.linkClicked, type=qt.Qt.UniqueConnection)
 
@@ -360,16 +404,23 @@
             tr.widget = self.transformWidget
 
     def makeSplitterButtons(self):
         "Orientation should be given for the closed state."
         self.splitterButtons = {}
         self.makeSplitterButton('files && containers', self.splitter, 1, 0)
         self.makeSplitterButton('data', self.splitter, 2, 1)
-        self.makeSplitterButton('transform', self.splitter, 3, 3)
-        self.makeSplitterButton('data format', self.splitterFiles, 1, 1)
+        but = self.makeSplitterButton('data corrections', self.splitter, 3, 3)
+        if self.node.plotDimension == 1:
+            but.setEnabled(True)
+        else:
+            but.setEnabled(False)
+            but.setToolTip("corrections are available only for 1D data")
+        self.makeSplitterButton('transform', self.splitter, 4, 4)
+        self.makeSplitterButton('data format (see tab tooltips)',
+                                self.splitterFiles, 1, 1)
         self.makeSplitterButton('combine', self.splitterData, 1, 1)
 
         ind = 1
         for fit in csi.fits.values():
             if fit.node is self.node and fit.widgetClass is not None:
                 but = self.makeSplitterButton(
                     fit.name, self.splitterPlot, ind, ind)
@@ -522,16 +573,18 @@
         try:
             return title.format(ind)
         except Exception:
             return ""
 
     def makePlotWidget(self):
         node = self.node
-        # self.backend = dict(backend='opengl')
-        self.backend = dict(backend='matplotlib')
+        if csi.plotBackend in ('matplotlib', 'opengl'):
+            self.backend = dict(backend=csi.plotBackend)
+        else:
+            self.backend = dict(backend='matplotlib')
 
         if node.plotDimension == 3:
             self.plot = Plot3D(self.splitterPlot, position=Plot3D.posInfo,
                                **self.backend)
             self.plot.setCustomPosInfo()
             self.plot.setTitleCallback(self.titleCallback3D)
         elif node.plotDimension == 2:
@@ -555,15 +608,15 @@
                                **self.backend)
             self.plot.getXAxis().setLabel(xLbl)
             self.plot.getYAxis().setLabel(yLbl)
         else:
             raise ValueError("wrong plot dimension")
         self.plotSetup()
         self.plot.setMinimumWidth(20)
-        self.savedPlotProps = {}
+        self.savedPlotProps = {'cm.vmin': None, 'cm.vmax': None}
 
     def plotSetup(self):
         node = self.node
         if node.plotDimension == 1:
             try:
                 unit = node.get_arrays_prop('plotUnit', role='x')[0]
                 strUnit = u" ({0})".format(unit) if unit else ""
@@ -581,31 +634,45 @@
             self.plot.setColormap(COLORMAP)
             labels = node.get_prop(node.plot3DArray, 'plotLabel')
             axisLabels = self._makeAxisLabels(labels)
             self.plot.setLabels(axisLabels)
 
     def makeFitWidgets(self):
         self.fitWidgets = []
-        for ifit, fit in enumerate(csi.fits.values()):
+        ifit = 0
+        for fit in csi.fits.values():
             if fit.node is self.node and fit.widgetClass is not None:
-                fitWidget = fit.widgetClass(self.splitterPlot, fit, self.plot)
-                fitWidget.fitReady.connect(
-                    partial(self.replotFit, fit, ifit))
+                if hasattr(fit, 'extraNodes'):
+                    plots = [self.plot] + \
+                        [node.widget.plot for node in fit.extraNodes]
+                else:
+                    plots = self.plot
+                fitWidget = fit.widgetClass(self.splitterPlot, fit, plots)
+                fitWidget.fitReady.connect(partial(self.replotFit, fit, ifit))
+                if hasattr(fit, 'extraNodes'):
+                    for inode, node in enumerate(fit.extraNodes):
+                        axtraFitAttrs = ['{0}{1}'.format(attr, inode+2)
+                                         for attr in ('x', 'y', 'fit')]
+                        fitWidget.fitReady.connect(partial(
+                            node.widget.replotFit, fit, (self, ifit),
+                            fitAttrs=axtraFitAttrs))
+                ifit += 1
                 self.fitWidgets.append(fitWidget)
                 curveLabel = fit.dataAttrs['fit']
                 if curveLabel not in self.fitLines:
                     self.fitLines.append(curveLabel)
                     self.fitLines.append(curveLabel+'.residue')
 
     def makeMetadataWidget(self):
         self.metadata = qt.QTextEdit(self.splitterPlot)
         self.metadata.setStyleSheet("QTextEdit {border: none;}")
         self.metadata.setReadOnly(True)
         # self.metadata.setContentsMargins(0, 0, 0, 0)
         self.metadata.setMinimumHeight(84)
+        self.metadata.setMinimumWidth(20)
         self.metadata.setAlignment(qt.Qt.AlignLeft | qt.Qt.AlignTop)
         self.metadata.setText("text metadata here")
         self.metadata.setHorizontalScrollBarPolicy(qt.Qt.ScrollBarAlwaysOff)
         self.metadata.setVerticalScrollBarPolicy(qt.Qt.ScrollBarAlwaysOn)
         self.metadata.setSizePolicy(
             qt.QSizePolicy.Expanding, qt.QSizePolicy.Expanding)
 
@@ -644,16 +711,14 @@
             self.savedPlotProps['yaxisR.range'] = ylimR
         else:
             return
         self.savedPlotProps['xaxis.range'] = plot.getXAxis().getLimits()
         self.savedPlotProps['yaxis.range'] = plot.getYAxis().getLimits()
 
         if self.node.plotDimension in [3, 2]:
-            self.savedPlotProps['cm.vmin'] = None
-            self.savedPlotProps['cm.vmax'] = None
             activeImage = self.plot.getActiveImage()
             if activeImage is not None:
                 cm = activeImage.getColormap()
                 self.savedPlotProps['cm.vmin'] = cm.getVMin()
                 self.savedPlotProps['cm.vmax'] = cm.getVMax()
 
     def _restorePlotState(self):
@@ -799,24 +864,29 @@
                             if cN not in rightAxisUnits:
                                 rightAxisUnits.append(cN)
                         else:
                             unit = node.get_prop(yN, 'plotUnit')
                             if unit:
                                 if unit not in rightAxisUnits:
                                     rightAxisUnits.append(unit)
+            self.plot.isRightAxisVisible = len(rightAxisColumns) > 0
+            zoomModeAction = self.plot.getInteractiveModeToolBar().\
+                getZoomModeAction()
+            if hasattr(zoomModeAction, 'setAxesMenuEnabled'):
+                zoomModeAction.setAxesMenuEnabled(self.plot.isRightAxisVisible)
             if nPlottedItems == 0:
                 self.plot.clearCurves()
                 return
             self.plotLeftYLabel = self._makeYLabel(
                 leftAxisColumns, leftAxisUnits)
             self.plot.setGraphYLabel(label=self.plotLeftYLabel, axis='left')
             self.plotRightYLabel = self._makeYLabel(
                 rightAxisColumns, rightAxisUnits)
             self.plot.setGraphYLabel(label=self.plotRightYLabel, axis='right')
-        if node.plotDimension == 2:
+        elif node.plotDimension == 2:
             self.plot.clearCurves()
             # if needClear:
             if True:
                 self.plot.clearImages()
                 # self.plot.clearMarkers()  # clears roi lines, don't add
             if len(csi.selectedItems) > 0:
                 item = csi.selectedItems[0]  # it could be the last one but
@@ -840,15 +910,15 @@
                 return
 
             xOrigin, xScale = self.getCalibration(item, 'x')
             yOrigin, yScale = self.getCalibration(item, 'y')
             self.plot.addImage(image, colormap=colors.Colormap(COLORMAP),
                                origin=(xOrigin, yOrigin),
                                scale=(xScale, yScale), z=-100)
-        if node.plotDimension == 3:
+        elif node.plotDimension == 3:
             self.plot._plot.clearCurves()
             # if needClear:
             if True:
                 self.plot._plot.clearImages()
                 # self.plot._plot.clearMarkers()  # clears roi lines, don't add
             item = None
             if len(csi.selectedItems) > 0:
@@ -874,25 +944,23 @@
 
         if keepExtent:
             self._restorePlotState()
 
         try:
             if hasattr(self.transformWidget, 'extraPlot'):
                 self.transformWidget.extraPlot()
-        except AttributeError:  # as e:
-            # if not self.wasNeverPlotted:
-            #     print(e)
-            pass
+        except Exception as e:
+            print('extraPlot in {0} failed: {1}'.format(self.node.name, e))
 
         # if self.wasNeverPlotted and node.plotDimension == 1:
         #     self.plot.resetZoom()
         self.wasNeverPlotted = False
 
     @logger(minLevel=50, attrs=[(0, 'node')])
-    def replotFit(self, fitWorker, ifit):
+    def replotFit(self, fitWorker, ifit, fitAttrs=('x', 'y', 'fit')):
         def plotOne(item, x, y, curveLabel, plotProps):
             symbolsize = plotProps.pop('symbolsize', 2)
             curve = self.plot.getCurve(curveLabel)
             z = 1 if item in csi.selectedItems else 0
             try:
                 if curve is None:
                     self.plot.addCurve(
@@ -916,50 +984,66 @@
                     if self.backend['backend'] == 'opengl':
                         # don't know why it is small with opengl
                         symbolsize *= 2
                     curve.setSymbolSize(symbolsize)
 
         node = self.node
         xAttrName, yAttrName, fitAttrName = [
-            fitWorker.dataAttrs[a] for a in ('x', 'y', 'fit')]
-        fitSizes = self.splitterPlot.sizes()[1:-1]
-        assert len(fitSizes) == len(self.fitWidgets)
+            fitWorker.dataAttrs[a] for a in fitAttrs]
+        if isinstance(ifit, int):
+            fitSizes = self.splitterPlot.sizes()[1:-1]
+            assert len(fitSizes) == len(self.fitWidgets)
+        if isinstance(ifit, tuple):  # (nodeWidget, ifit)
+            fitSizes = ifit[0].splitterPlot.sizes()[1:-1]
+            assert len(fitSizes) == len(ifit[0].fitWidgets)
+            ifit = ifit[1]
 
         if node.plotDimension == 1:
             plotProps = fitWorker.plotParams['fit']
-            residueProps = fitWorker.plotParams['residue']
+            residueProps = fitWorker.plotParams['residue'] if \
+                'residue' in fitWorker.plotParams else None
             for item in csi.allLoadedItems:
                 curveLabel = item.alias + '.' + fitAttrName
                 residueLabel = curveLabel + '.residue'
                 if not self.shouldPlotItem(item) or fitSizes[ifit] == 0:
                     self.plot.remove(curveLabel, kind='curve')
                     self.plot.remove(residueLabel, kind='curve')
                     continue
                 try:
                     x = getattr(item, xAttrName)
                     y = getattr(item, yAttrName)
                     fity = getattr(item, fitAttrName)
                 except AttributeError:
                     continue
                 plotOne(item, x, fity, curveLabel, dict(plotProps))
-                if fity.any():  # any non-zero
+                # if xAttrName == 'bftk':  # keep for tests
+                #     plotOne(item, x, item.ftfitwindow, curveLabel+'Window',
+                #             dict(plotProps))
+                if residueProps and fity.any():  # any non-zero
                     plotOne(item, x, y-fity, residueLabel, dict(residueProps))
         else:
             raise NotImplementedError('fit plot not implemented for dim={0}'
                                       .format(node.plotDimension))
 
     def saveGraph(self, fname, i, name):
         if fname.endswith('.pspj'):
             fname = fname.replace('.pspj', '')
-        if len(self.plot.getItems()) == 0:
-            return
         fname += '-{0}-{1}.png'.format(i+1, name)
         if self.node.plotDimension in [1, 2]:
+            if len(self.plot.getItems()) == 0:
+                return
+            if csi.mainWindow is not None:
+                # If a node has never been activated, its plot has an undefined
+                # size. Raising the node sets a correct size to its plot:
+                dock = csi.mainWindow.docks[self][0]
+                dock.raise_()
             self.plot.saveGraph(fname)
         elif self.node.plotDimension in [3]:
+            if len(self.plot.getPlotWidget().getItems()) == 0:
+                return
             self.plot._plot.saveGraph(fname)
 
     def _makeYLabel(self, yNames, yUnits):
         if not yNames:
             return ""
         yLabels = self.node.get_arrays_prop('plotLabel', yNames)
         axisLabel = ", ".join(yLabels)
@@ -1005,14 +1089,15 @@
             self.updateNodeForSelectedItems()
         if csi.DEBUG_LEVEL > 0 and self.mainWindow is None:  # for test purpose
             selNames = ', '.join([it.alias for it in csi.selectedItems])
             dataCount = len(csi.allLoadedItems)
             self.setWindowTitle('{0} total; {1}'.format(dataCount, selNames))
 
     def updateNodeForSelectedItems(self):
+        time.sleep(0.01)  # roi counts do not update with 0 wait
         self.updateSplittersForSelectedItems()
         fname = self.shouldUpdateFileModel()
         if fname:
             self.files.gotoWhenReady(fname)
             self.columnFormat.setUIFromData()
 
         self.updateMeta()
@@ -1022,15 +1107,16 @@
 
     def shouldUpdateFileModel(self):
         for it in csi.selectedItems:
             if it.dataType in (cco.DATA_COLUMN_FILE, cco.DATA_DATASET) and\
                     csi.nodes[it.originNodeName] is self.node:
                 return it.madeOf
 
-    def loadFiles(self, fileNamesFull=None, parentItem=None, insertAt=None):
+    def loadFiles(self, fileNamesFull=None, parentItem=None, insertAt=None,
+                  concatenate=False, lengthCheck=None):
         def times(n):
             return " ({0} times)".format(n) if n > 1 else ""
 
         selectedIndexes = self.files.selectionModel().selectedRows()
         if len(selectedIndexes) == 0:
             return
         selectedIndex = selectedIndexes[0]
@@ -1102,15 +1188,16 @@
                 parentItem = csi.selectedItems[0].parentItem
             else:
                 parentItem = csi.dataRootItem
 
         # df['dataSource'] = [col[0][0] for col in colRecs]
         csi.model.importData(
             fileNamesFull, parentItem, insertAt, dataFormat=df,
-            originNodeName=self.node.name)
+            originNodeName=self.node.name, concatenate=concatenate,
+            lengthCheck=lengthCheck)
 
     def shouldShowColumnDialog(self):
         for it in csi.selectedItems:
             if it.dataType in (cco.DATA_COLUMN_FILE, cco.DATA_DATASET) and\
                     csi.nodes[it.originNodeName] is self.node:
                 return True
         return False
@@ -1152,19 +1239,29 @@
             return
         fitSizes = self.splitterPlot.sizes()[1:-1]
         assert len(fitSizes) == len(self.fitWidgets)
         for fitWidget, fitSize in zip(self.fitWidgets, fitSizes):
             if fitSize > 0 or shouldClear:
                 fitWidget.setSpectrum(csi.selectedItems[0])
             if shouldClear:
-                roi = fitWidget.rangeWidget.roi
-                if roi is not None:
-                    roi.blockSignals(True)
-                    roi.setVisible(fitSize > 0)
-                    roi.blockSignals(False)
+                if isinstance(fitWidget.rangeWidget, (list, tuple)):
+                    rangeWidgets = fitWidget.rangeWidget
+                else:
+                    rangeWidgets = [fitWidget.rangeWidget]
+                for rangeWidget in rangeWidgets:
+                    roi = rangeWidget.roi
+                    if roi is not None:
+                        p = rangeWidget.panel
+                        if p.isCheckable():
+                            isChecked = p.isChecked()
+                        else:
+                            isChecked = True
+                        roi.blockSignals(True)
+                        roi.setVisible((fitSize > 0) and isChecked)
+                        roi.blockSignals(False)
 
     def linkClicked(self, url):
         strURL = str(url.toString())
         if strURL.startswith('http') or strURL.startswith('ftp'):
             if self.lastBrowserLink == strURL:
                 return
             webbrowser.open(strURL)
@@ -1248,8 +1345,15 @@
         print('auto', self.autoDirName, diffs, self.autoIndex, self.autoChunk)
         if len(diffs) > 0:
             toLoad = [diff for i, diff in enumerate(diffs) if
                       (i+self.autoIndex) % self.autoChunk == self.autoChunk-1]
             self.autoIndex += len(diffs)
             self.autoFileList = newFileList
             if toLoad:
-                self.loadFiles(toLoad)
+                if self.cbLonger is not None and self.cbLonger.isChecked():
+                    try:
+                        xLonger = float(self.xLonger.text())
+                    except Exception:
+                        xLonger = None
+                else:
+                    xLonger = None
+                self.loadFiles(toLoad, lengthCheck=xLonger)
```

## Comparing `parseq-2023.5.0/parseq/gui/plot.py` & `parseq-2024.5.0/parseq/gui/plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,28 +2,46 @@
 __author__ = "Konstantin Klementiev"
 __date__ = "16 Feb 2019"
 # !!! SEE CODERULES.TXT !!!
 
 import os
 from silx.gui import qt
 from silx.gui import plot as splot
+from silx.gui.plot.actions.control import ZoomBackAction, CrosshairAction
+try:
+    from silx.gui.plot.tools.menus import ZoomEnabledAxesMenu
+except ModuleNotFoundError:
+    ZoomEnabledAxesMenu = None
 
 from ..core import singletons as csi
 
 
 class Plot1D(splot.PlotWindow):
     def __init__(self, parent=None, backend=None, position=True):
         super().__init__(
             parent=parent, backend=backend, resetzoom=True, autoScale=True,
             logScale=True, grid=True, curveStyle=True, colormap=False,
             aspectRatio=False, yInverted=False, copy=True, save=True,
             print_=True, control=True, position=position, roi=False,
             mask=False, fit=False)
         if parent is None:
             self.setWindowTitle('Plot1D')
+
+        self._zoomBackAction = ZoomBackAction(plot=self, parent=self)
+        self._crosshairAction = CrosshairAction(plot=self, parent=self)
+        if ZoomEnabledAxesMenu is not None:
+            self._zoomEnabledAxesMenu = ZoomEnabledAxesMenu(
+                plot=self, parent=self)
+        self.isRightAxisVisible = False
+        # Retrieve PlotWidget's plot area widget
+        plotArea = self.getWidgetHandle()
+        # Set plot area custom context menu
+        plotArea.setContextMenuPolicy(qt.Qt.CustomContextMenu)
+        plotArea.customContextMenuRequested.connect(self._contextMenu)
+
         action = self.getFitAction()
         action.setXRangeUpdatedOnZoom(True)
         action.setFittedItemUpdatedFromActiveCurve(True)
 
     def graphCallback(self, ddict=None):
         """This callback is going to receive all the events from the plot."""
         if ddict is None:
@@ -52,14 +70,31 @@
             index, qt.QItemSelectionModel.ClearAndSelect |
             qt.QItemSelectionModel.Rows)
         nodeWidget = self.parent().parent().parent()
         nodeWidget.tree.setCurrentIndex(index)
         nodeWidget.tree.selChanged()
         nodeWidget.updateNodeForSelectedItems()
 
+    def _contextMenu(self, pos):
+        """Handle plot area customContextMenuRequested signal.
+
+        :param QPoint pos: Mouse position relative to plot area
+        """
+        # Create the context menu
+        menu = qt.QMenu(self)
+        menu.addAction(self._zoomBackAction)
+        if self.isRightAxisVisible and ZoomEnabledAxesMenu is not None:
+            menu.addMenu(self._zoomEnabledAxesMenu)
+        menu.addSeparator()
+        menu.addAction(self._crosshairAction)
+
+        plotArea = self.getWidgetHandle()
+        globalPosition = plotArea.mapToGlobal(pos)
+        menu.exec(globalPosition)
+
 
 class Plot2D(splot.Plot2D):
     pass
 
 
 class Plot3D(splot.StackView):
     posInfo = [
```

## Comparing `parseq-2023.5.0/parseq/gui/plotOptions.py` & `parseq-2024.5.0/parseq/gui/plotOptions.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/propsOfData.py` & `parseq-2024.5.0/parseq/gui/propsOfData.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,22 +59,24 @@
 def setComboBoxFromData(comboBox, prop, compareWith=None, defaultIndex=0):
     common = getCommonPropInSelectedItems(prop)
     if common is not None:
         if isinstance(common, float):
             comboBox.lineEdit().setText(str(common))
             return
         ind = compareWith.index(common) if compareWith is not None else common
-        if isinstance(ind, int):
-            comboBox.setCurrentIndex(ind)
-        else:
-            comboBox.setCurrentIndex(comboBox.findText(ind))
+        newInd = ind if isinstance(ind, int) else comboBox.findText(ind)
     else:
         if defaultIndex in ['last', -1]:
             defaultIndex = comboBox.count() - 1
-        comboBox.setCurrentIndex(defaultIndex)
+        newInd = defaultIndex
+
+    curInd = comboBox.currentIndex()
+    comboBox.setCurrentIndex(newInd)
+    if curInd == newInd:  # force the signal for updating gui
+        comboBox.currentIndexChanged.emit(newInd)
 
 
 def setRangeWidgetFromData(rWidget, prop):
     common = getCommonPropInSelectedItems(prop)
     rWidget.setRange(common)
 
 
@@ -110,15 +112,15 @@
         if textFormat == '':
             sf = '{0}'
         elif 'strip' in textFormat:
             sf = '{0:.0e}'
         else:
             sf = '{0:' + textFormat + '}'
         ss = sf.format(common)
-        if 'strip' in textFormat:
+        if ('strip' in textFormat) or ('g' in textFormat):
             ss = ss.lower()
             for r in (("e-0", "e-"), ("e+0", "e+")):
                 ss = ss.replace(*r)
         if ss.endswith("e+0") or ss.endswith("e-0"):
             ss = ss[:-3]
         edit.setText(ss)
         return ss
@@ -126,15 +128,15 @@
 
 setLabelFromData = setEditFromData
 
 
 def setSpinBoxFromData(sb, prop):
     common = getCommonPropInSelectedItems(prop)
     if common is None:
-        sb.setSpecialValueText(' ')  # can't be just ''
+        sb.lineEdit().setText('')
         return
     if isinstance(common, type("")):
         sb.lineEdit().setText(common)
     else:
         sb.setValue(common)
         sb.update()
```

## Comparing `parseq-2023.5.0/parseq/gui/propWidget.py` & `parseq-2024.5.0/parseq/gui/propWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 User transformation widgets can profit from using `silx library
 <https://www.silx.org/>`_, as ParSeq already uses it heavily. It has many
 widgets that are internally integrated to plotting e.g. ROIs. A good first
 point of interaction with silx is its collection of examples.
 """
 __author__ = "Konstantin Klementiev"
-__date__ = "17 Feb 2021"
+__date__ = "4 May 2024"
 # !!! SEE CODERULES.TXT !!!
 
 from functools import partial
 from collections import OrderedDict
 import reprlib
 
 from silx.gui import qt
@@ -32,17 +32,17 @@
 from ..core import config
 from ..core.logger import logger
 from . import undoredo as gur
 from . import propsOfData as gpd
 
 propWidgetTypes = (
     'edit', 'label', 'spinbox', 'groupbox', 'checkbox', 'pushbutton',
-    'tableview', 'combobox', 'rangewidget', 'statebuttons')
+    'tableview', 'combobox', 'rangewidget', 'statebuttons', 'correction')
 
-spinBoxDelay = 500  # ms
+spinBoxDelay = 100  # ms
 
 
 class FloatRepr(reprlib.Repr):
     def repr_float(self, value, level):
         return format(value, '.3f')
 
     def repr_float64(self, value, level):
@@ -120,14 +120,22 @@
                 try:
                     self.properties[key] = eval(testStr)
                 except (SyntaxError, NameError):
                     self.properties[key] = testStr
 
     def _addAction(self, menu, text, slot, shortcut=None):
         action = qt.QAction(text, self)
+        if text.startswith('apply'):
+            icon = self.style().standardIcon(qt.QStyle.SP_DialogApplyButton)
+        elif text.startswith('reset'):
+            icon = self.style().standardIcon(qt.QStyle.SP_DialogCancelButton)
+        else:
+            icon = None
+        if icon is not None:
+            action.setIcon(icon)
         action.triggered.connect(slot)
         if shortcut:
             action.setShortcut(qt.QKeySequence(shortcut))
         action.setShortcutContext(qt.Qt.WidgetWithChildrenShortcut)
         menu.addAction(action)
         return action
 
@@ -202,15 +210,16 @@
             if widget in self.propGroups:
                 props = self._getPropListGroup(widget)
                 if props is None:  # when a widget in the group is disabled
                     continue
                 cap = self.propGroups[widget]['caption']
             elif widget in self.propWidgets:
                 propWidget = self.propWidgets[widget]
-                tNames = propWidget['transformNames']
+                tNames = list(propWidget['transformNames'])
+                tNames += [tr.name for tr in self.node.transformsOut]
                 props = self._getPropListWidget(widget)
                 if 'copyValue' in propWidget:
                     res = propWidget['copyValue']
                     if not isinstance(res, (list, tuple)):
                         res = [res]
                     values = [
                         cco.getDotAttr(data, prop) if v == 'from data' else v
@@ -245,44 +254,54 @@
                 partial(self.startPick, props, values, actionName))
             if csi.DEBUG_LEVEL > 10:
                 print('widget in widgetsOver')
                 print('actionName', actionName)
                 print('props', props)
                 print('values', values)
 
+        if len(tNames) == 0:
+            return
+
         for tName in tNames:
             tr = csi.transforms[tName]
+            validProps = []
+            for prop in props:
+                key = cco.shrinkTransformParam(prop)
+                if key in tr.defaultParams:
+                    validProps.append(prop)
+            if len(validProps) == 0:
+                continue
+
             keys = tr.defaultParams.keys()
-            props = [cco.expandTransformParam(key) for key in keys]
-            values = [data.transformParams[key] for key in keys]
-            actionName = 'apply all params of "{0}" transform to picked data'\
-                .format(tName)
+            allDefProps = [cco.expandTransformParam(key) for key in keys]
+            allDefValues = [data.transformParams[key] for key in keys]
+            actionName = 'apply all params of "{0}"'.format(tName)
             actionName2 = actionName + ' to picked data'
             self._addAction(
                 menu, actionName2,
-                partial(self.startPick, props, values, actionName))
+                partial(self.startPick, allDefProps, allDefValues, actionName))
             if csi.DEBUG_LEVEL > 10:
                 print('apply all params of the transform')
                 print('actionName', actionName)
-                print('props', props)
-                print('values', values)
+                print('allDEfProps', allDefProps)
+                print('allDefValues', allDefValues)
 
-            props = [cco.expandTransformParam(key)
-                     for key in data.transformParams.keys()]
-            values = list(data.transformParams.values())
-            actionName = 'apply all params of all transforms to picked data'
-            actionName2 = actionName + ' to picked data'
-            self._addAction(
-                menu, actionName2,
-                partial(self.startPick, props, values, actionName))
-            if csi.DEBUG_LEVEL > 10:
-                print('apply all params of all transforms')
-                print('actionName', actionName)
-                print('props', props)
-                print('values', values)
+        allProps = [cco.expandTransformParam(key)
+                    for key in data.transformParams.keys()]
+        allValues = list(data.transformParams.values())
+        actionName = 'apply all params of all transforms'
+        actionName2 = actionName + ' to picked data'
+        self._addAction(
+            menu, actionName2,
+            partial(self.startPick, allProps, allValues, actionName))
+        if csi.DEBUG_LEVEL > 10:
+            print('apply all params of all transforms')
+            print('actionName', actionName)
+            print('allProps', allProps)
+            print('allValues', allValues)
 
     def fillMenuReset(self, widgetsOver, menu):
         actionStr = 'reset {0} to default value{1}'
 
         tr = None
         for widget in widgetsOver:
             tNames = []
@@ -292,29 +311,31 @@
                 props = self._getPropListGroup(widget)
                 if props is None:  # when a widget in the group is disabled
                     continue
                 cap = self.propGroups[widget]['caption']
             elif widget in self.propWidgets:
                 props = self._getPropListWidget(widget)
                 cap = self.propWidgets[widget]['caption']
-                tNames = self.propWidgets[widget]['transformNames']
+                tNames = list(self.propWidgets[widget]['transformNames'])
+                tNames += [tr.name for tr in self.node.transformsOut]
             elif widget in self.exclusivePropGroups:
                 props = self._getPropListExclusiveGroup(widget)
                 cap = self.exclusivePropGroups[widget]['caption']
             else:
                 continue
             values, validProps = [], []
             for tName in tNames:
                 if tName is None:
                     continue
                 tr = csi.transforms[tName]
                 for prop in props:
                     key = cco.shrinkTransformParam(prop)
                     if key in tr.defaultParams:
-                        values.append(tr.defaultParams[key])
+                        defVal = tr.defaultParams[key]
+                        values.append(defVal)
                         validProps.append(prop)
 
             if len(values) == 0:
                 continue
             elif len(values) == 1:
                 curValue = values[0]
                 if isinstance(curValue, float):
@@ -329,15 +350,15 @@
                 partial(self.resetProps, validProps, values, actionName))
 
         if tr is None:
             return
         keys = tr.defaultParams.keys()
         props = [cco.expandTransformParam(key) for key in keys]
         values = list(tr.defaultParams.values())
-        actionName = 'reset all params of "{0}" transform to default values'\
+        actionName = 'reset all params of "{0}" to default values'\
             .format(tr.name)
         self._addAction(menu, actionName,
                         partial(self.resetProps, props, values, actionName))
 
         props, values = [], []
         for transform in csi.transforms.values():
             for key in transform.defaultParams.keys():
@@ -535,18 +556,22 @@
                         widget.currentIndexChanged.connect(
                             partial(self.updatePropFromComboBox, widget,
                                     dataItems, prop, **kw))
                     elif iwt == 8:  # 'rangewidget' from gui.roi
                         widget.rangeChanged.connect(
                             partial(self.updatePropFromRangeWidget, widget,
                                     dataItems, prop))
-                    elif iwt == 9:  # 'statebuttons' from gui.roi
+                    elif iwt == 9:  # 'statebuttons' from gui.gcommons
                         widget.statesActive.connect(
                             partial(self.updatePropFromStateButtons, widget,
                                     dataItems, prop))
+                    elif iwt == 10:  # 'correction' from gui.gcorrection
+                        widget.sigCorrectionChanged.connect(
+                            partial(self.updatePropFromCorrections, widget,
+                                    dataItems, prop))
                     break
             else:
                 raise ValueError("unknown widgetType {0}".format(className))
 
             self.propWidgets[widget] = dict(
                 widgetTypeIndex=iwt, caption=caption, prop=prop,
                 transformNames=transformNames, kw=kw)
@@ -637,16 +662,16 @@
                       list(self.exclusivePropGroups.values())]
             if len(tNames) == 0:
                 return
         else:
             for dd in (list(self.propWidgets.values()) +
                        list(self.exclusivePropGroups.values())):
                 try:
+                    # may start with 'transformParams':
                     if dd['prop'].endswith(key):
-                        # may start with 'transformParams'
                         tNames = dd['transformNames']
                         break
                 except Exception:  # dd['prop'] can be a list
                     continue
             else:
                 raise ValueError('unknown parameter {0}'.format(key))
             if len(tNames) == 0:
@@ -680,15 +705,16 @@
                     tr = csi.transforms[tN]
                     if (tr.fromNode.is_between_nodes(
                         data.originNodeName, data.terminalNodeName) and
                         tr.toNode.is_between_nodes(
                             data.originNodeName, data.terminalNodeName)):
                         break
         else:
-            tr = csi.nodes[data.originNodeName].transformsOut[0]
+            trs = csi.nodes[data.originNodeName].transformsOut
+            tr = trs[0] if trs else None
         if tr is None:
             return
 
         if csi.tasker is not None:
             csi.tasker.prepare(
                 tr, params=params, runDownstream=True, dataItems=dataItems,
                 starter=self)
@@ -708,16 +734,14 @@
     def extraPlotActionAfterTransform(self, props):
         return
 
     def replotAllDownstream(self, tName):
         if hasattr(csi, 'nodesToReplot'):
             for node in csi.nodesToReplot:
                 node.widget.replot()
-            if csi.mainWindow is not None:
-                csi.mainWindow.selChanged()
 
         if tName:
             tr = csi.transforms[tName]
             csi.model.dataChanged.emit(qt.QModelIndex(), qt.QModelIndex())
             tr.toNode.widget.replot()
             for subnode in tr.toNode.downstreamNodes:
                 if subnode.widget is not None:
@@ -790,14 +814,23 @@
         self.updateProp(key, value, dataItems)
 
     def updatePropFromStateButtons(self, widget, dataItems, key, value):
         # if not widget.hasFocus():
         #     return
         self.updateProp(key, value, dataItems)
 
+    def updatePropFromCorrections(self, widget, dataItems, key):
+        # # if not widget.hasFocus():
+        # #     return
+        corrections = widget.getCorrections()
+
+        if dataItems is None:
+            dataItems = csi.selectedItems
+        self.updateProp(key, corrections, dataItems)
+
     def setUIFromData(self):
         for widget in self.exclusivePropGroups:
             dd = self.exclusivePropGroups[widget]
             if 'props' in dd:
                 # for Py3 only:
                 # gpd.setRButtonGroupWithEditsFromData(
                 #     *dd['widgets'], dd['props'])
```

## Comparing `parseq-2023.5.0/parseq/gui/roi.py` & `parseq-2024.5.0/parseq/gui/roi.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,16 @@
             elif isinstance(roi, HorizontalRangeROI):
                 name = 'range'
             roi.setName('{0}{1}'.format(name, len(self.getRois())))
 
         try:
             roi.setLineWidth(0.5)
             roi.setLineStyle('-')
-        except AttributeError:
+        except AttributeError as e:
+            # print(e)
             pass
         # roi.setSymbolSize(5)
         roi.setSelectable(True)
         roi.setEditable(True)
 
     def _feedContextMenu(self, menu):
         """when the default plot context menu is about to be displayed"""
@@ -61,21 +62,25 @@
             if roi.isEditable():
                 # Filter by data position
                 plot = self.parent()
                 pos = plot.getWidgetHandle().mapFromGlobal(qt.QCursor.pos())
                 data = plot.pixelToData(pos.x(), pos.y())
                 if roi.contains(data):
                     if isinstance(roi, InteractionModeMixIn):
-                        self._contextMenuForInteractionMode(menu, roi)
-
-                # removeAction = qt.QAction(menu)
-                # removeAction.setText("Remove %s" % roi.getName())
-                # callback = partial(self.removeRoi, roi)
-                # removeAction.triggered.connect(callback)
-                # menu.addAction(removeAction)
+                        try:
+                            intMenu = roi.createMenuForInteractionMode(menu)
+                            menu.addMenu(intMenu)
+                        except Exception as e:
+                            print(e)
+
+                removeAction = qt.QAction(menu)
+                removeAction.setText("Remove %s" % roi.getName())
+                callback = partial(self.removeRoi, roi)
+                removeAction.triggered.connect(callback)
+                menu.addAction(removeAction)
 
 
 class RoiModel(qt.QAbstractTableModel):
     def __init__(self, roiManager=None, fmt='auto'):
         super().__init__()
         self.roiCounts = []
         self.setRoiManager(roiManager)
@@ -110,15 +115,15 @@
                 return section
         elif role == qt.Qt.TextAlignmentRole:
             return qt.Qt.AlignHCenter
 
     def flags(self, index):
         if not index.isValid():
             return qt.Qt.NoItemFlags
-        res = qt.Qt.ItemIsEnabled  # | qt.Qt.ItemIsSelectable
+        res = qt.Qt.ItemIsEnabled | qt.Qt.ItemIsSelectable
         column = index.column()
         if column == 1:  # use
             res |= qt.Qt.ItemIsUserCheckable
         elif column in (0, 2):  # label, geometry
             res |= qt.Qt.ItemIsEditable
         return res
 
@@ -349,16 +354,16 @@
     maxVisibleTableRows = 4  # in the scroll area
 
     def __init__(self, parent, roiManager, fmt='auto'):
         super().__init__(parent)
         self.roiModel = RoiModel(roiManager, fmt)
         self.setModel(self.roiModel)
 
-        self.setSelectionMode(qt.QAbstractItemView.SingleSelection)
-        self.setSelectionBehavior(qt.QAbstractItemView.SelectRows)
+        self.setSelectionMode(self.SingleSelection)
+        self.setSelectionBehavior(self.SelectItems)
         self.selectionModel().selectionChanged.connect(self.selChanged)
 
         horHeaders = self.horizontalHeader()  # QHeaderView instance
         horHeaders.setHighlightSections(False)
         verHeaders = self.verticalHeader()  # QHeaderView instance
         verHeaders.setVisible(False)
 
@@ -389,15 +394,18 @@
         self.setMinimumHeight(int(horHeaders.height()*4*csi.screenFactor))
 
         roiManager.sigCurrentRoiChanged.connect(self.currentRoiChanged)
 
     def selChanged(self):
         if not self.hasFocus():
             return
-        selectedIndex = self.selectionModel().selectedRows()[0]
+        selectedIndexes = self.selectionModel().selectedIndexes()
+        if not selectedIndexes:
+            return
+        selectedIndex = selectedIndexes[0]
         manager = self.roiModel.roiManager
         rois = manager.getRois()
         manager.setCurrentRoi(rois[selectedIndex.row()])
 
     def currentRoiChanged(self, roi):
         rois = self.roiModel.roiManager.getRois()
         try:
@@ -722,15 +730,15 @@
                 print('The dict of rois is broken')
 
 
 class RoiWidget(RoiWidgetBase):
     def __init__(self, parent, plot, roiClassNames, roiMaxN=1, fmt='auto'):
         """
         *roiClassNames*: sequence of class names to appear in the toolbar
-        *roiMaxN*: max number of rois in the tabe
+        *roiMaxN*: max number of rois in the tabel
         """
         super().__init__(parent)
         self.plot = plot
         self.is3dStack = hasattr(self.plot, '_plot')
         if self.is3dStack:
             self.roiManager = RoiManager(plot._plot)
         else:
@@ -854,20 +862,26 @@
 
     def getRois(self):
         rois = self.roiManager.getRois()
         model = self.table.roiModel
         return [model.getRoiGeometry(roi) for roi in rois]
 
 
-class RangeWidgetBase(qt.QWidget):
+class BaseRangeWidget(qt.QWidget):
     rangeChanged = qt.pyqtSignal(list)
+    rangeToggled = qt.pyqtSignal(bool)
 
     def createRoi(self, vmin=None, vmax=None):
         if self.plot is None:
             return
+        elif isinstance(self.plot, str):
+            if csi.nodes[self.plot].widget is None:
+                return
+            self.plot = csi.nodes[self.plot].widget.plot
+
         needNew = False
         if self.roiManager is None:
             if self.is3dStack:
                 self.roiManager = RoiManager(self.plot._plot)
             else:
                 self.roiManager = RoiManager(self.plot)
             needNew = True
@@ -932,15 +946,15 @@
         """Converts from spinbox values to roi limits and backward.
         direction: 1: from spinbox values to roi limits, -1: from roi limits to
         spinbox values.
         """
         return vmin, vmax  # just pass through
 
 
-class RangeWidget(RangeWidgetBase):
+class SimpleRangeWidget(BaseRangeWidget):
     def __init__(self, parent, plot, caption, tooltip, rangeName, color,
                  formatStr, defaultRange=[0, 1]):
         """
         *defaultRange*: callable or 2-sequence
         """
         super().__init__(parent)
         self.plot = plot
@@ -955,44 +969,162 @@
         self.roiManager = None
         self.roi = None
         self.color = color
         self.roiClass = HorizontalRangeROI
 
         layout = qt.QVBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
-        panel = qt.QGroupBox(self)
-        panel.setFlat(True)
-        panel.setTitle(caption)
+        self.panel = qt.QGroupBox(self)
+        self.panel.setFlat(True)
+        self.panel.setTitle(caption)
+        # self.panel is by default uncheckable
+        self.panel.toggled.connect(self.toggled)
         layoutP = qt.QHBoxLayout()
         layoutP.setContentsMargins(10, 0, 0, 0)
-        self.rbAuto = qt.QRadioButton('auto', panel)
+        self.setCustomRange()
+        self.editCustom = qt.QLineEdit()
+        self.editCustom.setStyleSheet("QLineEdit{color: " + color + ";}")
+        if not callable(self.defaultRange):
+            self.editSetText(self.defaultRange)
+        layoutP.addWidget(self.editCustom)
+        if tooltip:
+            self.editCustom.setToolTip(tooltip)
+        self.panel.setLayout(layoutP)
+        layout.addWidget(self.panel)
+        self.setLayout(layout)
+
+    def toggled(self, on):
+        self.rangeToggled.emit(on)
+        if self.roi is None:
+            ran = self.defaultRange() if callable(self.defaultRange) else \
+                self.defaultRange
+            self.createRoi(ran)
+        if self.roi is None:  # cannot create roi because self.plot is stll str
+            return
+        self.roi.blockSignals(True)
+        self.roi.setVisible(on)
+        self.roi.blockSignals(False)
+
+    def editSetText(self, ran):
+        try:
+            self.editCustom.setText(self.formatStr.format(ran))
+        except Exception:
+            self.editCustom.setText('')
+
+    def setRange(self, ran):
+        if not isinstance(ran, (tuple, list)):
+            return
+        if self.roi is None:
+            ran = self.defaultRange() if callable(self.defaultRange) else \
+                self.defaultRange
+            self.createRoi(ran)
+        if self.roi is None:  # cannot create roi because self.plot is stll str
+            return
+
+        if len(ran) == 2:
+            self.editSetText(ran)
+            self.createRoi(*ran)
+            self.roi.blockSignals(True)
+            if self.panel.isCheckable():
+                use = self.panel.isChecked()
+            else:
+                use = True
+            self.roi.setVisible(use)
+            self.roi.blockSignals(False)
+
+    def setCustomRange(self):
+        self.createRoi()
+        if self.roi is None:
+            return
+        vmin, vmax = self.roi.getRange()
+        ran = self.convert(-1, vmin, vmax)
+        if ran is None:
+            return
+        self.roi.blockSignals(True)
+        self.roi.setVisible(True)
+        self.rangeChanged.emit(list(ran))
+        self.roi.blockSignals(False)
+
+    def acceptEdit(self):
+        if self.roi is None:
+            return
+        txt = self.editCustom.text()
+        try:
+            t1, t2 = txt.split(',')
+            vmin = float(t1.strip())
+            vmax = float(t2.strip())
+            self.setRange([vmin, vmax])
+            return [vmin, vmax]
+        except Exception:
+            pass
+
+
+class AutoRangeWidget(BaseRangeWidget):
+    def __init__(self, parent, plot, caption, tooltip, rangeName, color,
+                 formatStr, defaultRange=[0, 1]):
+        """
+        *defaultRange*: callable or 2-sequence
+        """
+        super().__init__(parent)
+        self.plot = plot
+        self.is3dStack = hasattr(plot, '_plot')
+        self.formatStr = formatStr
+        if callable(defaultRange):
+            self.defaultRange = defaultRange
+        else:
+            self.defaultRange = list(defaultRange)
+        self.tooltip = tooltip
+        self.rangeName = rangeName
+        self.roiManager = None
+        self.roi = None
+        self.color = color
+        self.roiClass = HorizontalRangeROI
+
+        layout = qt.QVBoxLayout()
+        layout.setContentsMargins(0, 0, 0, 0)
+        self.panel = qt.QGroupBox(self)
+        self.panel.setFlat(True)
+        self.panel.setTitle(caption)
+        # self.panel is by default uncheckable
+        self.panel.toggled.connect(self.toggled)
+        layoutP = qt.QHBoxLayout()
+        layoutP.setContentsMargins(10, 0, 0, 0)
+        self.rbAuto = qt.QRadioButton('auto', self.panel)
         self.rbAuto.clicked.connect(self.setAutoRange)
         layoutP.addWidget(self.rbAuto)
-        self.rbCustom = qt.QRadioButton('custom', panel)
+        self.rbCustom = qt.QRadioButton('custom', self.panel)
         self.rbCustom.setStyleSheet("QRadioButton{color: " + color + ";}")
         self.rbCustom.clicked.connect(self.setCustomRange)
         layoutP.addWidget(self.rbCustom)
         self.editCustom = qt.QLineEdit()
         self.editCustom.setStyleSheet("QLineEdit{color: " + color + ";}")
         if not callable(self.defaultRange):
             self.editSetText(self.defaultRange)
         layoutP.addWidget(self.editCustom)
         if tooltip:
             self.editCustom.setToolTip(tooltip)
-        panel.setLayout(layoutP)
-        layout.addWidget(panel)
+        self.panel.setLayout(layoutP)
+        layout.addWidget(self.panel)
         self.setLayout(layout)
 
+    def toggled(self, on):
+        self.rangeToggled.emit(on)
+        if self.roi is None:
+            return
+        self.roi.blockSignals(True)
+        self.roi.setVisible(on and self.rbCustom.isChecked())
+        self.roi.blockSignals(False)
+
     def editSetText(self, ran):
         try:
             self.editCustom.setText(self.formatStr.format(ran))
         except Exception:
             self.editCustom.setText('')
 
-    def setRange(self, ran):
+    def setRange(self, ran, use=True):
         if not isinstance(ran, (tuple, list)):
             self.rbAuto.setChecked(True)
             self.rbCustom.setChecked(False)
             return
 
         if len(ran) == 2:
             self.editSetText(ran)
@@ -1000,27 +1132,32 @@
             if callable(self.defaultRange):
                 defRange = self.defaultRange()
             else:
                 defRange = self.defaultRange
             isDefault = np.allclose(ran, defRange)
             self.rbAuto.setChecked(isDefault)
             self.rbCustom.setChecked(not isDefault)
-            self.roi.setVisible(not isDefault)
+
+            self.roi.blockSignals(True)
+            self.roi.setVisible(use and not isDefault)
+            self.roi.blockSignals(False)
 
     def setAutoRange(self):
         if callable(self.defaultRange):
             defRange = self.defaultRange()
+            if defRange is None:
+                return
         else:
             defRange = self.defaultRange
             fs = "[" + self.formatStr + "]{1}{2}"
             self.rbAuto.setToolTip(fs.format(
                 defRange, ' as ' if self.tooltip else '', self.tooltip))
         if self.roi is not None:
             self.setRange(defRange)
-        self.rangeChanged.emit(defRange)
+        self.rangeChanged.emit(list(defRange))
         self.editSetText(defRange)
         self.rbAuto.setChecked(True)
         self.rbCustom.setChecked(False)
 
     def setCustomRange(self):
         self.createRoi()
         vmin, vmax = self.roi.getRange()
@@ -1042,15 +1179,15 @@
             vmax = float(t2.strip())
             self.setRange([vmin, vmax])
             return [vmin, vmax]
         except Exception:
             pass
 
 
-class RangeWidgetSplit(RangeWidgetBase):
+class SplitRangeWidget(BaseRangeWidget):
     spinBoxDelay = 500  # ms
 
     def __init__(self, parent, plot, var, optionsMin, optionsMax, rangeName,
                  color, defaultRange, addVisibleCB=False):
         """
         *optionsMin*, *optionsMax*: list [min, max, step, decimals]
         *defaultRange*: callable or 2-sequence
@@ -1183,18 +1320,19 @@
     def acceptEdit(self):
         self.fromSpinBox(100)
         return self.spinBoxProps
 
     def spinDelayed(self):
         if self.spinBoxProps is None:
             return
-        self.rangeChanged.emit(self.spinBoxProps)
+        self.rangeChanged.emit(list(self.spinBoxProps))
         self.spinBoxProps = None
 
     def toggleVisible(self, on):
         if self.roi is None:
             return
         self.roi.setVisible(on)
 
     def setRangeVisible(self, on):
-        self.visibleCB.setChecked(on)
+        if hasattr(self, 'visibleCB'):
+            self.visibleCB.setChecked(on)
         self.toggleVisible(on)
```

## Comparing `parseq-2023.5.0/parseq/gui/tasker.py` & `parseq-2024.5.0/parseq/gui/tasker.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/undoredo.py` & `parseq-2024.5.0/parseq/gui/undoredo.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/webWidget.py` & `parseq-2024.5.0/parseq/gui/webWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from docutils.utils import SystemMessage
 from sphinx.application import Sphinx
 from sphinx.errors import SphinxError
 try:
     import sphinxcontrib.jquery  # to check if it exists
 except ImportError as e:
     print('do "pip install sphinxcontrib-jquery"')
-    raise(e)
+    raise e
 import codecs
 
 from ..core import singletons as csi
 from ..core.logger import logger
 
 os.environ["QTWEBENGINE_CHROMIUM_FLAGS"] = "--disable-gpu"
 
@@ -95,15 +95,15 @@
     sphinx_app = Sphinx(srcdir, confdir, outdir, doctreedir, 'html',
                         confoverrides, status=status, warning=warning,
                         freshenv=True, warningiserror=False, tags=None)
     try:
         sphinx_app.build()
     except (SystemMessage, SphinxError) as e:
         print(e)
-        raise(e)
+        raise e
 #        output = ("It was not possible to generate rich text help for this "
 #                  "object.</br>Please see it in plain text.")
 
 
 if 'pyqt4' in qt.BINDING.lower():
     import PyQt4.QtWebKit as myQtWeb
 elif 'pyqt5' in qt.BINDING.lower():
@@ -111,15 +111,15 @@
         import PyQt5.QtWebEngineWidgets as myQtWeb
     except ImportError:
         try:
             import PyQt5.QtWebKitWidgets as myQtWeb
         except ImportError as e:
             print('do "conda install -c conda-forge pyqtwebengine"'
                   ' or "pip install pyqtwebengine"')
-            raise(e)
+            raise e
 elif 'pyside2' in qt.BINDING.lower():
     import PySide2.QtWebEngineWidgets as myQtWeb
 elif 'pyside6' in qt.BINDING.lower():
     import PySide6.QtWebEngineWidgets as myQtWeb
 else:
     raise ImportError("Cannot import any Python Qt package!")
```

## Comparing `parseq-2023.5.0/parseq/gui/fits/gfunctionfit.py` & `parseq-2024.5.0/parseq/gui/fits/gfunctionfit.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,15 +221,18 @@
 class FunctionFitTableView(qt.QTableView):
     columnWidths = [60, 80, 50, 80, 150, 55]
 
     def __init__(self, parent, model):
         super().__init__(parent)
         self.setModel(model)
 
-        horHeaders = self.horizontalHeader()  # QHeaderView instance
+        # horHeaders = self.horizontalHeader()  # QHeaderView instance
+        horHeaders = gbf.UnderlinedHeaderView(qt.Qt.Horizontal, self)
+        self.setHorizontalHeader(horHeaders)
+
         verHeaders = self.verticalHeader()  # QHeaderView instance
         verHeaders.setVisible(True)
 
         nC = model.columnCount()
         if 'pyqt4' in qt.BINDING.lower():
             horHeaders.setMovable(False)
             horHeaders.setResizeMode(0, qt.QHeaderView.Stretch)
@@ -239,26 +242,26 @@
         else:
             horHeaders.setSectionsMovable(False)
             horHeaders.setSectionResizeMode(0, qt.QHeaderView.Stretch)
             for i in range(1, nC):
                 horHeaders.setSectionResizeMode(i, qt.QHeaderView.Interactive)
             horHeaders.setSectionsClickable(True)
         horHeaders.setStretchLastSection(False)
-        horHeaders.setMinimumSectionSize(20)
+        # horHeaders.setMinimumSectionSize(20)
         verHeaders.setDefaultSectionSize(20)
 
         for i, cw in enumerate(self.columnWidths[:nC]):
             self.setColumnWidth(i, int(cw*csi.screenFactor))
 
         kw = dict(alignment=qt.Qt.AlignHCenter | qt.Qt.AlignVCenter)
         self.setItemDelegateForColumn(1, gco.DoubleSpinBoxDelegate(self, **kw))
 
         self.setMinimumHeight(horHeaders.height() * max(2, model.rowCount()+1))
-        self.setMinimumWidth(
-            int(sum(self.columnWidths[:nC])*csi.screenFactor) + 30)
+        # self.setMinimumWidth(
+        #     int(sum(self.columnWidths[:nC])*csi.screenFactor) + 30)
 
         # self.setSelectionMode(qt.QAbstractItemView.NoSelection)
         self.setSelectionMode(qt.QAbstractItemView.SingleSelection)
         # self.setSelectionBehavior(qt.QAbstractItemView.SelectItems)
         # self.setFocusPolicy(qt.Qt.NoFocus)
 
         self.setContextMenuPolicy(qt.Qt.CustomContextMenu)
@@ -302,18 +305,17 @@
 
     def applyPendingProps(self):
         if self.pickReason == 1:  # copy fit params
             srcParams = self.parent().spectrum.fitParams
             for item in csi.selectedItems:
                 dfparams = item.fitParams
                 dfparams['ffit_formula'] = str(srcParams['ffit_formula'])
-                dfparams['ffit_params'] = copy.deepcopy(
-                    srcParams['ffit_params'])
-                dfparams['ffit_result'] = copy.deepcopy(
-                    srcParams['ffit_params'])
+                for prop in self.model().worker.defaultParams:
+                    if prop in srcParams:
+                        dfparams[prop] = copy.deepcopy(srcParams[prop])
 
         csi.selectionModel.clear()
         csi.model.selectItems(self.parent().spectrum)
 
     def moveItem(self, to):
         newRow = self.model().moveItem(self.currentIndex(), to)
         if newRow is None:
```

## Comparing `parseq-2023.5.0/parseq/gui/fits/glcf.py` & `parseq-2024.5.0/parseq/gui/fits/glcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,15 +274,18 @@
 class LCFTableView(qt.QTableView):
     columnWidths = [140, 55, 170, 80, 50, 55, 140, 80, 50]
 
     def __init__(self, parent, model):
         super().__init__(parent)
         self.setModel(model)
 
-        horHeaders = self.horizontalHeader()  # QHeaderView instance
+        # horHeaders = self.horizontalHeader()  # QHeaderView instance
+        horHeaders = gbf.UnderlinedHeaderView(qt.Qt.Horizontal, self)
+        self.setHorizontalHeader(horHeaders)
+
         verHeaders = self.verticalHeader()  # QHeaderView instance
         verHeaders.setVisible(True)
 
         nC = model.columnCount()
         if 'pyqt4' in qt.BINDING.lower():
             horHeaders.setMovable(False)
             horHeaders.setResizeMode(0, qt.QHeaderView.Stretch)
@@ -292,28 +295,28 @@
         else:
             horHeaders.setSectionsMovable(False)
             horHeaders.setSectionResizeMode(0, qt.QHeaderView.Stretch)
             for i in range(1, nC):
                 horHeaders.setSectionResizeMode(i, qt.QHeaderView.Interactive)
             horHeaders.setSectionsClickable(True)
         horHeaders.setStretchLastSection(False)
-        horHeaders.setMinimumSectionSize(20)
+        # horHeaders.setMinimumSectionSize(20)
         verHeaders.setDefaultSectionSize(20)
         horHeaders.sectionClicked.connect(self.headerClicked)
 
         for i, cw in enumerate(self.columnWidths[:nC]):
             self.setColumnWidth(i, int(cw*csi.screenFactor))
         for i in [1, 5]:
             kw = dict(alignment=qt.Qt.AlignHCenter | qt.Qt.AlignVCenter)
             self.setItemDelegateForColumn(
                 i, gco.DoubleSpinBoxDelegate(self, **kw))
 
         self.setMinimumHeight(horHeaders.height() * max(2, model.rowCount()+1))
-        self.setMinimumWidth(
-            int(sum(self.columnWidths[:nC])*csi.screenFactor) + 30)
+        # self.setMinimumWidth(
+        #     int(sum(self.columnWidths[:nC])*csi.screenFactor) + 30)
 
         # self.setSelectionMode(qt.QAbstractItemView.NoSelection)
         self.setSelectionMode(qt.QAbstractItemView.SingleSelection)
         # self.setSelectionBehavior(qt.QAbstractItemView.SelectItems)
         # self.setFocusPolicy(qt.Qt.NoFocus)
 
         self.setContextMenuPolicy(qt.Qt.CustomContextMenu)
@@ -411,17 +414,16 @@
             self.setCurrentIndex(newInd)
 
     def applyPendingProps(self):
         if self.pickReason == 1:  # copy fit params
             srcParams = self.parent().spectrum.fitParams
             for item in csi.selectedItems:
                 dfparams = item.fitParams
-                dfparams['lcf_xRange'] = copy.deepcopy(srcParams['lcf_xRange'])
-                dfparams['lcf_params'] = copy.deepcopy(srcParams['lcf_params'])
-                dfparams['lcf_result'] = copy.deepcopy(srcParams['lcf_result'])
+                for prop in ('lcf_xRange', 'lcf_params', 'lcf_result'):
+                    dfparams[prop] = copy.deepcopy(srcParams[prop])
         elif self.pickReason == 2:  # add ref spectra
             names = [item.alias for item in csi.selectedItems]
             newRow = self.model().appendRefs(names)
             if newRow is None:
                 return
             newInd = self.model().index(newRow, 0)
             if newInd.isValid():
```

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-fit-32.png` & `parseq-2024.5.0/parseq/gui/_images/icon-fit-32.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-fit-64.png` & `parseq-2024.5.0/parseq/gui/_images/icon-fit-64.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-help.png` & `parseq-2024.5.0/parseq/gui/_images/icon-help.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-info.png` & `parseq-2024.5.0/parseq/gui/_images/icon-info.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-32.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-32.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-64.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-64.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-32.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-busy-32.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-64.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-1dim-busy-64.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-64.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-2dim-64.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-busy-64.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-2dim-busy-64.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-32.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-32.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-64.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-64.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-32.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-busy-32.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-64.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-3dim-busy-64.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-32.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-32.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-64.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-64.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-32.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-busy-32.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-64.png` & `parseq-2024.5.0/parseq/gui/_images/icon-item-ndim-busy-64.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-load-proj.png` & `parseq-2024.5.0/parseq/gui/_images/icon-load-proj.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-redo.png` & `parseq-2024.5.0/parseq/gui/_images/icon-redo.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-save-proj.png` & `parseq-2024.5.0/parseq/gui/_images/icon-save-proj.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-save-text.png` & `parseq-2024.5.0/parseq/gui/_images/icon-save-text.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/icon-undo.png` & `parseq-2024.5.0/parseq/gui/_images/icon-undo.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/gui/_images/parseq.ico` & `parseq-2024.5.0/parseq/gui/_images/parseq.ico`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/conf.py` & `parseq-2024.5.0/parseq/help/conf.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/conf_doc.py` & `parseq-2024.5.0/parseq/help/conf_doc.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/license.rst` & `parseq-2024.5.0/parseq/help/license.rst`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/make.bat` & `parseq-2024.5.0/parseq/help/make.bat`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/top.rst` & `parseq-2024.5.0/parseq/help/top.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ParSeq
 ======
 
-:GitHub: |GHver| |GHdate|
+:GitHub: |GHver| |GHdate| :ref:`version history <history>`
 :PyPI: |PPver| |PPdate|
 :License:  |GHlic|
 :Author: Konstantin Klementiev (MAX IV Laboratory)
 
 -----
 
 .. |GHver| image:: https://badge.fury.io/gh/kklmn%2FParSeq.svg
```

## Comparing `parseq-2023.5.0/parseq/help/exts/animation.py` & `parseq-2024.5.0/parseq/help/exts/animation.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 
 
 class AnimationDirective(Directive):
     required_arguments = 0
     optional_arguments = 0
     final_argument_whitespace = True
     option_spec = {'alt': directives.unchanged,
-# "upper-left-corner" (def), "lower-left-corner",
-# "upper-right-corner", "lower-right-corner" or e.g."top: -500px; left: 400px;"
+                   # for loc:
+                   # "upper-left-corner", "lower-left-corner",
+                   # "upper-right-corner", "lower-right-corner"
+                   # or e.g."top: -500px; left: 400px;"
                    'loc': directives.unchanged,
                    'width': directives.length_or_unitless,
                    'height': directives.length_or_unitless,
                    'scale': directives.percentage,
                    'widthzoom': directives.length_or_unitless,
                    'heightzoom': directives.length_or_unitless,
                    'scalezoom': directives.percentage,
                    'name': directives.unchanged,
+                   'align': directives.unchanged,
                    'target': directives.unchanged_required,
                    'class': directives.class_option}
     has_content = True
     aclass = "thumbnail"
 
     def run(self):
         if not lapp.builder.format.startswith('html'):
@@ -104,71 +107,98 @@
         sizezoom = ''
         if widthzoom:
             sizezoom += ' width="{0}"'.format(widthzoom)
         if heightzoom:
             sizezoom += ' height="{0}"'.format(heightzoom)
 #        print sizezoom
 
-        loc = self.options.get('loc', 'upper-left-corner')
-        ta = "text-align: left"
+        loc = self.options.get('loc', None)
+        align = self.options.get('align', None)
+        alignC = ''
+        if align is not None:
+            if align == 'left':
+                alignC = 'align-left'
+                if loc is None:
+                    loc = "upper-left-corner"
+            elif align == 'center':
+                alignC = 'align-center'
+                if loc is None:
+                    loc = "center"
+            elif align == 'right':
+                alignC = 'align-right'
+                if loc is None:
+                    loc = "upper-right-corner"
+            else:
+                if loc is None:
+                    loc = "upper-left-corner"
+        else:
+            alignC = 'align-left'
+            if loc is None:
+                loc = "upper-left-corner"
+
+        lochor = u'width: {}px; '.format(int(widthzoom))
         if 'corner' in loc:
             if 'lower' in loc:
-                loctop = u'top: -{0}px'.format(int(heightzoom)-20)
+                loctop = u'top: -{0}px; '.format(int(heightzoom-height//2))
             else:
-                loctop = u'top: -{0}px'.format(height)
+                loctop = u'top: {0}px; '.format(0)
             if 'right' in loc:
-                locleft = u'left: -{0}px'.format(int(widthzoom)-int(width))
+                ta = 'text-align: right; '
+                lochor += u'right: {0}px; '.format(0)
             else:
-                locleft = u'left: -{0}px'.format(0)
-            locst = u'style="{0}; {1}; {2}"'.format(loctop, locleft, ta)
-        else:
-            locst = u'style="{0}; {1}"'.format(loc, ta)
+                ta = 'text-align: left; '
+                lochor += u'left: {0}px; '.format(0)
+        elif loc == "center":
+            ta = 'text-align: center ;'
+            loctop = u'top: 0px; '
+            lochor += u'left: 50%; transform: translate(-50%, 0%); '
+        locst = u'style="{0} {1} {2}"'.format(loctop, lochor, ta)
 
         alt = self.options.get('alt', '')
         if alt:
             if alt.startswith("&ensp;") or alt.startswith("&emsp;"):
                 # Unicode &ensp; or &emsp;
-#                alt = '<br />{0}'.format(alt)
                 alt = '{0}'.format(alt)
-            else: # otherwise the substitution name is passed by docutils as 'alt'
+            else:
                 alt = ''
 #        self.options['uri'] = uri
         env = self.state.document.settings.env
         targetid = "animation{0}".format(env.new_serialno('animation'))
         if uri.endswith('.png'):
-            text = '<a class={6}>'\
-            '<img src="{0}" {1} />'\
-            '<span {5}>{2}'\
-            '<canvas id="{3}" {4} ></canvas>{2}'\
-            '<script>set_static("{0}", "{3}")</script></span></a>'.format(
-                uri, size, alt, targetid, sizezoom, locst, self.aclass)
+            text = '<a class="{6}">'\
+                '<img class="{7}" src="{0}" {1} />'\
+                '<span {5}>{2}<br><canvas id="{3}" {4} ></canvas><br>{2}'\
+                '<script>set_static("{0}", "{3}")</script></span></a>'\
+                .format(
+                    uri, size, alt, targetid, sizezoom, locst, self.aclass,
+                    alignC)
         else:
             text = '<a class={6}>'\
-            '<script type="text/javascript" src="{0}/s_anim.js"></script>'\
-            '<script type="text/javascript" src="{0}/b_anim.js"></script>'\
-            '<canvas id="s_{1}" {2}></canvas>'\
-            '<script>set_animation("{0}/s_packed.png", s_timeline, "s_{1}")'\
-            '</script><span {5}>{3}<canvas id="b_{1}" {4}></canvas>{3}'\
-            '<script>set_animation("{0}/b_packed.png", b_timeline, "b_{1}")'\
-            '</script></span></a>'.format(
-                uri, targetid, size, alt, sizezoom, locst, self.aclass)
+                '<script type="text/javascript" src="{0}/s_anim.js"></script>'\
+                '<script type="text/javascript" src="{0}/b_anim.js"></script>'\
+                '<canvas id="s_{1}" {2}></canvas>'\
+                '<script>set_animation("{0}/s_packed.png",s_timeline,"s_{1}")'\
+                '</script><span {5}>{3}<canvas id="b_{1}" {4}></canvas>{3}'\
+                '<script>set_animation("{0}/b_packed.png",b_timeline,"b_{1}")'\
+                '</script></span></a>'.format(
+                    uri, targetid, size, alt, sizezoom, locst, self.aclass)
         return [nodes.raw('', text, format='html')]
 
 
 class AnimationHoverDirective(AnimationDirective):
     aclass = "thumbnailhover"
 
 
 class VideoDirective(Directive):
     required_arguments = 0
     optional_arguments = 0
     final_argument_whitespace = True
     option_spec = {'autoplay': directives.flag,
-                   'controls': directives.flag,                   
-                   'loop': directives.flag,                   
+                   'controls': directives.flag,
+                   'loop': directives.flag,
                    'width': directives.length_or_unitless,
                    'height': directives.length_or_unitless}
     has_content = True
     aclass = "video"
 
     def run(self):
         if not lapp.builder.format.startswith('html'):
```

## Comparing `parseq-2023.5.0/parseq/help/_images/mickey-rtfm.gif` & `parseq-2024.5.0/parseq/help/_images/mickey-rtfm.gif`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/_images/parseq.ico` & `parseq-2024.5.0/parseq/help/_images/parseq.ico`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/_images/parseq_big.png` & `parseq-2024.5.0/parseq/help/_images/parseq_big.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/_static/animation.js` & `parseq-2024.5.0/parseq/help/_static/animation.js`

 * *Files 22% similar despite different names*

### js-beautify {}

```diff
@@ -1,41 +1,41 @@
-var timer = null
+var timer = null;
 
 function set_animation(img_url, timeline, canvas_id) {
-    var canvas = document.getElementById(canvas_id)
-    var ctx = canvas.getContext("2d")
-    var img = new Image()
+    var canvas = document.getElementById(canvas_id);
+    var ctx = canvas.getContext("2d");
+    var img = new Image();
     img.onload = function() {
-        var i = 0
+        var i = 0;
         var f = function() {
-            var frame = i++ % timeline.length
-            var delay = timeline[frame].delay
-            var blits = timeline[frame].blit
+            var frame = i++ % timeline.length;
+            var delay = timeline[frame].delay;
+            var blits = timeline[frame].blit;
             for (j = 0; j < blits.length; ++j) {
-                var blit = blits[j]
-                var sx = blit[0]
-                var sy = blit[1]
-                var w = blit[2]
-                var h = blit[3]
-                var dx = blit[4]
-                var dy = blit[5]
-                ctx.drawImage(img, sx, sy, w, h, dx, dy, w, h)
+                var blit = blits[j];
+                var sx = blit[0];
+                var sy = blit[1];
+                var w = blit[2];
+                var h = blit[3];
+                var dx = blit[4];
+                var dy = blit[5];
+                ctx.drawImage(img, sx, sy, w, h, dx, dy, w, h);
             }
-            timer = window.setTimeout(f, delay)
+            timer = window.setTimeout(f, delay);
         }
         f()
     }
-    img.src = img_url
+    img.src = img_url;
     img.onunload = function() {
-        if (timer) window.clearTimeout(timer)
+        if (timer) window.clearTimeout(timer);
     }
 }
 
 function set_static(img_url, canvas_id) {
-    var canvas = document.getElementById(canvas_id)
-    var ctx = canvas.getContext("2d")
-    var img = new Image()
-    img.src = img_url
+    var canvas = document.getElementById(canvas_id);
+    var ctx = canvas.getContext("2d");
+    var img = new Image();
+    img.src = img_url;
     img.onload = function() {
-        ctx.drawImage(img, 0, 0)
+        ctx.drawImage(img, 0, 0);
     }
 }
```

## Comparing `parseq-2023.5.0/parseq/help/_static/thumbnail.css` & `parseq-2024.5.0/parseq/help/_static/thumbnail.css`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 .thumbnail{
 position: relative;
+display: inherit;
 z-index: 0;
 cursor: zoom-in;
 transition: 0.3s;
 }
 .thumbnail:hover{
 background-color: transparent;
 z-index: 50;
 }
 .thumbnail span{ /*CSS for enlarged image*/
 position: absolute;
-background-color: #F2F2F2;
+background-color: #ddeeff;
 padding: 5px;
-left: -1000px; 
 border: 2px solid gray;
 visibility: hidden;
 color: black;
 text-decoration: none;
-text-align: left
+text-align: left;
 }
 .thumbnail span img{ /*CSS for enlarged image*/
 border-width: 0;
 padding: 0px;
 }
 .thumbnail:active span{ /*CSS for enlarged image on hover or active*/
 visibility: visible;
```

## Comparing `parseq-2023.5.0/parseq/help/_themes/mytheme/static/mycss.css_t` & `parseq-2024.5.0/parseq/help/_themes/mytheme/static/mycss.css_t`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     font-size: 100%;
     background-color: #fff;
     color: #555;
     margin: 0;
     padding: 0;
 }
 
+section {
+    text-align: justify;
+}
+
 div.documentwrapper {
     float: left;
     width: 100%;
 }
 
 div.bodywrapper {
     margin: 0 0 0 {{ theme_sidebarwidth|todim }};
```

## Comparing `parseq-2023.5.0/parseq/help/_themes/parseq/layout.html` & `parseq-2024.5.0/parseq/help/_themes/parseq/layout.html`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/_themes/parseq/page.html` & `parseq-2024.5.0/parseq/help/_themes/parseq/page.html`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/_themes/parseq/theme.conf` & `parseq-2024.5.0/parseq/help/_themes/parseq/theme.conf`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/help/_themes/parseq/static/default.css_t` & `parseq-2024.5.0/parseq/help/_themes/parseq/static/default.css_t`

 * *Files 1% similar despite different names*

```diff
@@ -376,26 +376,27 @@
     margin-left: 10px;
     width: auto;
     height: 24px;
     border-radius: 11px;
     background: #eef;
     box-shadow: 1px 2px 3px #aac, inset 0px 0px 7px rgba(0,0,50,1);
     text-align: center;
+    line-height: 95%;
 
     /* center a div insie another div*/
     display: flex;
     justify-content: center;
     align-items: center;
 }
 
 .pipeline-fit {
-    padding: 7px;
+    padding: 2px;
     margin: 0 auto;
     width: auto;
-    height: 16px;
+/*    height: 16px; */
     border-radius: 7px;
     background: #ded;
     box-shadow: 1px 2px 3px #caa, inset 0px 0px 3px rgba(0,0,0,1);
     vertical-align: middle;
     text-align: center;
     position: relative;
 }
@@ -420,14 +421,15 @@
 svg {    
     position: absolute;
     left: 0px;
     top: 0px;
     margin: auto;
     width: 100%;
     height: 100%;
+    pointer-events: none;
 }
 
 svg .shadow {
     stroke-width: 3;
     stroke-linecap: round;
     fill: none;
 }
```

## Comparing `parseq-2023.5.0/parseq/help/_themes/parseq/static/utils.js` & `parseq-2024.5.0/parseq/help/_themes/parseq/static/utils.js`

 * *Files 9% similar despite different names*

### js-beautify {}

```diff
@@ -30,25 +30,26 @@
 
 function redrawConnectors() {
     $('[id^=line_]').each(function() {
         div1 = document.getElementById(this.getAttribute("node1"));
         div2 = document.getElementById(this.getAttribute("node2"));
         var rect1 = div1.getBoundingClientRect();
         var rect2 = div2.getBoundingClientRect();
-        this.setAttribute("x1", (rect1.left + rect1.right) * 0.5);
-        this.setAttribute("y1", rect1.bottom + 1);
-        this.setAttribute("x2", (rect2.left + rect2.right) * 0.5);
-        this.setAttribute("y2", rect2.top - 1);
+        this.setAttribute("x1", (rect1.left + rect1.right) * 0.5 + window.scrollX);
+        this.setAttribute("y1", rect1.bottom + 1 + window.scrollY);
+        this.setAttribute("x2", (rect2.left + rect2.right) * 0.5 + window.scrollX);
+        this.setAttribute("y2", rect2.top - 1 + window.scrollY);
     });
     $('[id^=arc_]').each(function() {
         div1 = document.getElementById(this.getAttribute("node"));
         //      var pad = parseFloat(window.getComputedStyle(div1, null).getPropertyValue('padding'))
         var rr = div1.getBoundingClientRect();
         this.setAttribute("d",
-            "M " + rr.left + " " + rr.bottom +
+            "M " + (rr.left + window.scrollX).toString() +
+            " " + (rr.bottom + window.scrollY).toString() +
             "m 10 0 c 5 15 15 15 20 0");
     });
 }
 
 window.onresize = resize;
 
 function resize() {
```

## Comparing `parseq-2023.5.0/parseq/tests/circles-rect.png` & `parseq-2024.5.0/parseq/tests/circles-rect.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/circles.png` & `parseq-2024.5.0/parseq/tests/circles.png`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/modeltest.py` & `parseq-2024.5.0/parseq/tests/modeltest.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_calibrateEnergyWidget.py` & `parseq-2024.5.0/parseq/tests/test_calibrateEnergyWidget.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_columnStrings.py` & `parseq-2024.5.0/parseq/tests/test_columnStrings.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_combineSpectraWidget.py` & `parseq-2024.5.0/parseq/tests/test_combineSpectraWidget.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_commons.py` & `parseq-2024.5.0/parseq/tests/test_commons.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_curve_shear.py` & `parseq-2024.5.0/parseq/tests/test_curve_shear.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_dataRebinWidget.py` & `parseq-2024.5.0/parseq/tests/test_dataRebinWidget.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_dataTreeModelView.py` & `parseq-2024.5.0/parseq/tests/test_dataTreeModelView.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_fileDialog.py` & `parseq-2024.5.0/parseq/tests/test_fileDialog.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_fileTreeModelView.py` & `parseq-2024.5.0/parseq/tests/test_fileTreeModelView.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,83 @@
 # -*- coding: utf-8 -*-
 __author__ = "Konstantin Klementiev"
 __date__ = "01 Jan 2019"
 # !!! SEE CODERULES.TXT !!!
 
+# import os
+# os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"  # to work with external links
 # import hdf5plugin  # needed to prevent h5py's "OSError: Can't read data"
 
 from silx.gui import qt, icons
+
 import sys; sys.path.append('../..')  # analysis:ignore
 from parseq.gui.fileTreeModelView import FileTreeView
 
 
-def test():
+def test1():
+    import h5py
+    fname = r"c:\_MaxIV\Balder data\20240213-Mo-XES\scan-29270_albaem_2d_01.h5"
+    entry = "entry/instrument/albaem"
+    with h5py.File(fname, "r") as f:
+        print(f.get(entry))
+        print(f.get(entry, getclass=True))
+        print(f.get(entry, getclass=True, getlink=True))
+
+    fname = r"c:\_MaxIV\Balder data\20240213-Mo-XES\20240213.h5 "
+    entry = "entry29270/instrument"
+    with h5py.File(fname, "r") as f:
+        print(f.get(entry))
+        print(f.get(entry, getclass=True))
+        print(f.get(entry, getclass=True, getlink=True))
+
+    fname = r"c:\_MaxIV\Balder data\20240213-Mo-XES\20240213.h5 "
+    entry = "entry29270/instrument/albaem_2d_01"
+    with h5py.File(fname, "r") as f:
+        print(f.get(entry))
+        print(f.get(entry, getclass=True))
+        print(f.get(entry, getclass=True, getlink=True))
+
+
+def test2():
     def gotoLastData():
         view.gotoWhenReady(path)
 
     app = qt.QApplication(sys.argv)
 
-    # view = FileTreeView(rootPath=r'../..')
-    view = FileTreeView(rootPath='')
+    # path = 'C:/ParSeq/parseq_XES_scan/data'
+    # path = 'C:/ParSeq/parseq_XES_scan/data/20201112.h5'
+    # path = 'silx:C:/ParSeq/parseq_XES_scan/data/20201112.h5::/entry10170'
+    # path = 'silx:C:/ParSeq/parseq_XES_scan/data/20201112.h5::/entry10170/measurement'
+    # path = 'c:/_MaxIV/Balder data/20240213-Mo-XES/20240213.h5'
+    path = 'silx:data/hdf5/20240213s.h5::/entry29270/instrument'
 
+    view = FileTreeView()
     view.setMinimumSize(qt.QSize(700, 600))
     view.header().resizeSection(0, 320)
     view.setWindowTitle("Merged Tree Model: QFileSystemModel + h5Model")
-
-    # path = 'C:/ParSeq/parseq_XES_scan/data'
-    # path = 'C:/ParSeq/parseq_XES_scan/data/20201112.h5'
-    # path = 'silx:C:/ParSeq/parseq_XES_scan/data/20201112.h5::/entry10170'
-    path = 'silx:C:/ParSeq/parseq_XES_scan/data/20201112.h5::/entry10170/measurement'
     view.gotoWhenReady(path)
 
     # if "qt5" in qt.BINDING.lower():
     #     from modeltest import ModelTest
     #     ModelTest(view.model(), view)
 
     gotoButton = qt.QToolButton()
     gotoButton.setFixedSize(24, 24)
     gotoButton.setIcon(icons.getQIcon('last'))
     gotoButton.setToolTip("Go to the latest loaded data")
     gotoButton.clicked.connect(gotoLastData)
 
     # Main widget
     widget = qt.QWidget()
-    layout = qt.QVBoxLayout()
-    layout.addWidget(gotoButton)
+    layout = qt.QHBoxLayout()
+    # layout.addWidget(gotoButton)
     layout.addWidget(view)
     widget.setLayout(layout)
 
     widget.show()
     app.exec_()
+    app.deleteLater()
 
 
 if __name__ == '__main__':
-    test()
+    # test1()
+    test2()
```

## Comparing `parseq-2023.5.0/parseq/tests/test_fit.py` & `parseq-2024.5.0/parseq/tests/test_fit.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         allData.append(spectrum)
     csi.allLoadedItems = allData
 
     mix1 = DataProxy()
     mix1.alias = 'mix1'
     mix1.e = e
     mix1.mu = data[:, -2]
+    mix1.transformParams = []
     mix1.transfortmTimes = {}
     mix1BasisNames = ['cufe2o4_ave4', 'cus_ave2', 'cucl_w_ave2']
     w1 = 1./len(mix1BasisNames)
     lcfParams = []
     for refName in mix1BasisNames:
         lcfParams.append(
             dict(name=refName, use=True, w=w1, wBounds=[0., 1., 0.01],
@@ -217,14 +218,15 @@
         ffit_xRange=[8850, 9100]
         )
 
     mix2 = DataProxy()
     mix2.alias = 'mix2'
     mix2.e = e
     mix2.mu = data[:, -1]
+    mix2.transformParams = []
     mix2.transfortmTimes = {}
     mix2BasisNames = ['cuoh2_ave4', 'cucl2_ave2', 'cuco36h2o_ave3', 'cuo_ave2']
     w2 = 1./len(mix2BasisNames)
     lcfParams = []
     for refName in mix2BasisNames:
         lcfParams.append(
             dict(name=refName, use=True, w=w2, wBounds=[0., 1., 0.01],
```

## Comparing `parseq-2023.5.0/parseq/tests/test_flowLayout.py` & `parseq-2024.5.0/parseq/tests/test_flowLayout.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_hdf5.py` & `parseq-2024.5.0/parseq/tests/test_hdf5.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 __author__ = "Konstantin Klementiev"
 __date__ = "20 Sep 2018"
 # !!! SEE CODERULES.TXT !!!
 
 #from silx.gui import qt
 
-import os.path as osp
+import os
 import sys; sys.path.append('../..')  # analysis:ignore
 import numpy as np
+os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"  # to work with external links
 import h5py
 from silx.gui.data.DataViewerFrame import DataViewerFrame
 from silx.gui import qt
 crop = 0, 0, 1555, 515
 
 
 def write_avi(fName):
     import cv2
 
-    fPath = osp.join('../../_data_big', fName+'.hdf5')
+    fPath = os.path.join('../../_data_big', fName+'.hdf5')
     f = h5py.File(fPath, 'r')
 #    data = 'und_energy'
 #    e = f[data][:]
     data = 'i0'
     i0 = f[data][:]
     data = 'lambdaOne_images'
     images = f[data][:len(i0), :, :]
@@ -47,15 +48,15 @@
         frame *= 255. / maxInTime
         frameOut = np.array(frame, dtype='>u1')
         writer.write(frameOut)
     f.close()
 
 
 def showInWidget(fName):
-    fPath = osp.join('../../_data_big', fName+'.hdf5')
+    fPath = os.path.join('../../_data_big', fName+'.hdf5')
     f = h5py.File(fPath, 'r')
 #    data = 'und_energy'
 #    e = f[data][:]
     data = 'i0'
     i0 = f[data][:]
     data = 'lambdaOne_images'
     images = f[data][:len(i0), :, :]
```

## Comparing `parseq-2023.5.0/parseq/tests/test_mainWindow.py` & `parseq-2024.5.0/parseq/tests/test_mainWindow.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_node.py` & `parseq-2024.5.0/parseq/tests/test_node.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_nodeWidget.py` & `parseq-2024.5.0/parseq/tests/test_nodeWidget.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py` & `parseq-2024.5.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_plotInteractiveImageSingleROI.py` & `parseq-2024.5.0/parseq/tests/test_plotInteractiveImageSingleROI.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_plotOptions.py` & `parseq-2024.5.0/parseq/tests/test_plotOptions.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_QSortFilterProxyModel.py` & `parseq-2024.5.0/parseq/tests/test_QSortFilterProxyModel.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_ROI.py` & `parseq-2024.5.0/parseq/tests/test_ROI.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_slice.py` & `parseq-2024.5.0/parseq/tests/test_slice.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/test_stateButtons.py` & `parseq-2024.5.0/parseq/tests/test_stateButtons.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/data/cu-ref-mix.res` & `parseq-2024.5.0/parseq/tests/data/cu-ref-mix.res`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/data/pb-ref-mix.res` & `parseq-2024.5.0/parseq/tests/data/pb-ref-mix.res`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/tests/data/zn-ref-mix.res` & `parseq-2024.5.0/parseq/tests/data/zn-ref-mix.res`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/third_party/XAFSmass.py` & `parseq-2024.5.0/parseq/third_party/XAFSmass.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/third_party/xrt.py` & `parseq-2024.5.0/parseq/third_party/xrt.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/third_party/data/Energies.txt` & `parseq-2024.5.0/parseq/third_party/data/Energies.txt`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq/utils/ft.py` & `parseq-2024.5.0/parseq/utils/ft.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import numpy as np
 
 ft_windows = ('none', 'box', 'linear-tapered', 'cosine-tapered',
               'Gaussian-tapered')
 
 
-def make_ft_window(kind, x, xmin, xmax, width, vmin):
+def make_ft_window(kind, x, xmin, xmax, width, vmin=0):
     """
     Create a tapered FT window function.
 
     *kind*: str
     one of `ft_windows`,
 
     *x*: array
@@ -25,15 +25,15 @@
     *width*: float
     the distance in x from xmin to the flat top and from the flat top to xmax,
 
     *vmin*: float
     the minimum value of the resulting window function at the ends.
     """
     res = np.ones_like(x)
-    if not kind or kind == 'none':
+    if not kind or kind == 'none' or xmin is None or xmax is None:
         return res
     if kind == 'box':
         res[x < xmin] = 0
         res[x > xmax] = 0
         return res
 
     left_lobe = (x-xmin >= 0) & (x-xmin <= width)
@@ -51,10 +51,12 @@
             res[right_lobe] = 0.5 * (1-np.cos(phi)) * (1-v0) + v0
     elif kind == 'Gaussian-tapered':
         v0 = vmin if 0 <= vmin <= 1 else 0
         if (width > 1e-12) and (v0 >= 1e-3):
             sigma2 = width**2 / (2*abs(np.log(v0)))
             res[left_lobe] = np.exp(-0.5*(x[left_lobe]-xmin-width)**2/sigma2)
             res[right_lobe] = np.exp(-0.5*(xmax-width-x[right_lobe])**2/sigma2)
-    res[x < xmin] = res[left_lobe][0]
-    res[x > xmax] = res[right_lobe][-1]
+    if len(res[left_lobe]) > 0:
+        res[x < xmin] = vmin
+    if len(res[right_lobe]) > 0:
+        res[x > xmax] = vmin
     return res
```

## Comparing `parseq-2023.5.0/parseq/utils/h5reduce.py` & `parseq-2024.5.0/parseq/utils/h5reduce.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 3. Repack the file into another hdf5 file by `repack()`.
 """
 
 __author__ = "Konstantin Klementiev"
 __date__ = "13 Jun 2021"
 # !!! SEE CODERULES.TXT !!!
 
+import os
+os.environ["HDF5_USE_FILE_LOCKING"] = "FALSE"  # to work with external links
 import h5py
 
 
 def print_entries(fname):
     with h5py.File(fname, "a") as f:
         print(list(f.keys()))
```

## Comparing `parseq-2023.5.0/parseq/utils/math.py` & `parseq-2024.5.0/parseq/utils/math.py`

 * *Files identical despite different names*

## Comparing `parseq-2023.5.0/parseq.egg-info/PKG-INFO` & `parseq-2024.5.0/parseq.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parseq
-Version: 2023.5.0
+Version: 2024.5.0
 Summary: ParSeq is a python software library for Parallel execution of Sequential data analysis.
 Home-page: http://parseq.readthedocs.io
 Author: Konstantin Klementiev
 Author-email: konstantin.klementiev@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/kklmn/ParSeq
 Keywords: data-analysis pipeline framework gui synchrotron spectroscopy
@@ -17,32 +17,53 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: numpy>=1.8.0
+Requires-Dist: scipy>=0.17.0
+Requires-Dist: matplotlib>=2.0.0
+Requires-Dist: sphinx>=1.6.2
+Requires-Dist: sphinxcontrib-jquery
+Requires-Dist: autopep8
+Requires-Dist: h5py
+Requires-Dist: silx>=1.1.0
+Requires-Dist: hdf5plugin
+Requires-Dist: psutil
+Requires-Dist: pyqtwebengine
+Requires-Dist: docutils
+Requires-Dist: distro
+Requires-Dist: colorama
 
 Package ParSeq is a python software library for **Par**\ allel execution of
 **Seq**\ uential data analysis. It implements a general analysis framework that
 consists of transformation nodes -- intermediate stops along the data pipeline
-to visualize data, display status and provide user input -- and transformations
-that connect the nodes. It provides an adjustable data model (supports
-grouping, renaming, moving and drag-and-drop), tunable data format definitions,
-plotters for 1D, 2D and 3D data, cross-data analysis routines and flexible
-widget work space suitable for single- and multi-screen computers. It also
-defines a structure to implement particular analysis pipelines as relatively
-lightweight Python packages.
+for data visualization, cross-data operations (e.g. taking average), providing
+user input and displaying status -- and transformations that connect the nodes.
+
+It provides an adjustable data tree model (supports grouping, renaming, moving
+and drag-and-drop arrangement), tunable data format definitions, plotters for
+1D, 2D and 3D data, cross-data analysis routines and flexible widget work space
+suitable for single- and multi-screen computers. It also defines a structure to
+implement particular analysis pipelines as lightweight Python packages.
 
 ParSeq is intended for synchrotron based techniques, first of all spectroscopy.
 
+A screenshot of ParSeq-XAS (an EXAFS analysis pipeline) as an application
+example:
+
+.. image:: _images/XAS-foils.gif
+   :scale: 50 %
+
 Main features
 -------------
 
--  ParSeq allows creating analysis pipelines as lightweight modules.
+-  ParSeq allows creating analysis pipelines as lightweight Python packages.
 
 -  Flexible use of screen area by detachable/dockable transformation nodes
    (parts of analysis pipeline).
 
 -  Two ways of acting from GUI onto multiple data: (a) simultaneous work with
    multiply selected data and (b) copying a specific parameter or a group of
    parameters from active data items to later selected data items.
@@ -53,52 +74,57 @@
    pipeline.
 
 -  Creation of cross-data combinations (e.g. averaging, RMS or PCA) and their
    propagation downstream the pipeline together with the parental data. The
    possibility of termination of the parental data at any selected downstream
    node.
 
+-  General data correction routines for 1D data: range deletion, scaling,
+   replacement by a spline and jump correction.
+
 -  Parallel execution of data transformations with multiprocessing or
    multithreading (can be opted by the pipeline application).
 
 -  Optional curve fitting solvers, also executed in parallel for multiple data
    items.
 
 -  Informative error handling that provides alerts and stack traceback -- the
    type and location of the occurred error.
 
+-  Optional time profiling of the pipeline, as controlled by a command-line
+   argument.
+
 -  Export of the workflow into a project file. Export of data into various data
    formats with accompanied Python scripts that visualize the exported data for
    the user to tune their publication plots.
 
 -  ParSeq understands container files (presently only hdf5) and adds them to
    the system file tree as subfolders. The file tree, including hdf5
    containers, is lazy loaded thus enabling big data collections.
 
 -  A web viewer widget near each analysis widget displays help pages generated
    from the analysis widget doc strings. The help pages are built by Sphinx at
    the startup time.
 
--  The pipeline can be operated via scripts or GUI.
+-  The pipeline can be operated by the GUI or from a Python script without GUI.
 
 -  Optional automatic loading of new data during a measurement time.
 
 The mechanisms for creating nodes, transformations and curve fitting solvers,
 connecting them together and creating Qt widgets for the transformations and
 and curve fits are exemplified by separately installed analysis packages:
 
-- `ParSeq-XES-scan <https://github.com/kklmn/ParSeq-XES-scan>`_
-- `ParSeq-XES-dispersive <https://github.com/kklmn/ParSeq-XES-dispersive>`_
 - `ParSeq-XAS <https://github.com/kklmn/ParSeq-XAS>`_
+- `ParSeq-XES-scan <https://github.com/kklmn/ParSeq-XES-scan>`_
 
 Dependencies
 ------------
 
-- `silx <https://github.com/silx-kit/silx>`_ -- for plotting and Qt imports
-- `sphinx <https://github.com/sphinx-doc/sphinx>`_ -- for building html documentation
+- `silx <https://github.com/silx-kit/silx>`_ -- plotting, hdf5 handling, Qt
+- `sphinx <https://github.com/sphinx-doc/sphinx>`_ -- building documentation
 
 Launch an example
 -----------------
 
 Either install ParSeq and a ParSeq pipeline application by their installers to
 the standard location or put them to any folder in their respective folders
 (``parseq`` and e.g. ``parseq_XES_scan``) and run the ``*_start.py`` module of
```

