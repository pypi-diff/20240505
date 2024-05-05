# Comparing `tmp/feffery_antd_charts-0.1.0rc0.tar.gz` & `tmp/feffery_antd_charts-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_antd_charts-0.1.0rc0.tar", last modified: Tue Apr 30 04:38:03 2024, max compression
+gzip compressed data, was "feffery_antd_charts-0.1.0rc1.tar", last modified: Sun May  5 03:30:00 2024, max compression
```

## Comparing `feffery_antd_charts-0.1.0rc0.tar` & `feffery_antd_charts-0.1.0rc1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 04:38:03.965143 feffery_antd_charts-0.1.0rc0/
--rw-rw-rw-   0        0        0     1087 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc0/LICENSE
--rw-rw-rw-   0        0        0      434 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc0/MANIFEST.in
--rw-rw-rw-   0        0        0      274 2024-04-30 04:38:03.963711 feffery_antd_charts-0.1.0rc0/PKG-INFO
--rw-rw-rw-   0        0        0       49 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 04:38:03.952912 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/
--rw-rw-rw-   0        0        0     6640 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdArea.py
--rw-rw-rw-   0        0        0     7493 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdBar.py
--rw-rw-rw-   0        0        0     5139 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdBidirectionalBar.py
--rw-rw-rw-   0        0        0     5534 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdBox.py
--rw-rw-rw-   0        0        0     5644 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdBullet.py
--rw-rw-rw-   0        0        0     4673 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdChord.py
--rw-rw-rw-   0        0        0     7920 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdColumn.py
--rw-rw-rw-   0        0        0     6716 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdDecompositionTree.py
--rw-rw-rw-   0        0        0     6061 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdDualAxes.py
--rw-rw-rw-   0        0        0     6389 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdFundFlow.py
--rw-rw-rw-   0        0        0     5921 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdFunnel.py
--rw-rw-rw-   0        0        0     6081 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdGauge.py
--rw-rw-rw-   0        0        0     7537 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdHeatmap.py
--rw-rw-rw-   0        0        0     5484 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdHistogram.py
--rw-rw-rw-   0        0        0     6167 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdLine.py
--rw-rw-rw-   0        0        0     5731 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdLiquid.py
--rw-rw-rw-   0        0        0     6727 2024-04-30 04:37:56.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdPie.py
--rw-rw-rw-   0        0        0     3837 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdProgress.py
--rw-rw-rw-   0        0        0     6502 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdRadar.py
--rw-rw-rw-   0        0        0     7255 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdRadialBar.py
--rw-rw-rw-   0        0        0     8018 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdRadialTree.py
--rw-rw-rw-   0        0        0     5206 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdRingProgress.py
--rw-rw-rw-   0        0        0     5913 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdRose.py
--rw-rw-rw-   0        0        0     5126 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdSankey.py
--rw-rw-rw-   0        0        0     6869 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdScatter.py
--rw-rw-rw-   0        0        0     5405 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdStock.py
--rw-rw-rw-   0        0        0     5870 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdSunburst.py
--rw-rw-rw-   0        0        0     4856 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdTinyArea.py
--rw-rw-rw-   0        0        0     4704 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdTinyColumn.py
--rw-rw-rw-   0        0        0     4965 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdTinyLine.py
--rw-rw-rw-   0        0        0     5162 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdTreemap.py
--rw-rw-rw-   0        0        0     5391 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdVenn.py
--rw-rw-rw-   0        0        0     5758 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdViolin.py
--rw-rw-rw-   0        0        0     6250 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdWaterfall.py
--rw-rw-rw-   0        0        0     6095 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdWordCloud.py
--rw-rw-rw-   0        0        0     2666 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/__init__.py
--rw-rw-rw-   0        0        0     2063 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/_imports_.py
--rw-rw-rw-   0        0        0     1614 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/alias.py
--rw-rw-rw-   0        0        0  1302494 2024-04-30 04:37:53.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/async-graphs.js
--rw-rw-rw-   0        0        0  1410792 2024-04-30 04:37:53.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/async-plots.js
--rw-rw-rw-   0        0        0    76624 2024-04-30 04:37:53.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/feffery_antd_charts.min.js
--rw-rw-rw-   0        0        0   442996 2024-04-30 04:37:57.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/metadata.json
--rw-rw-rw-   0        0        0     2482 2024-04-30 04:37:54.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts/package-info.json
-drwxrwxrwx   0        0        0        0 2024-04-30 04:38:03.962703 feffery_antd_charts-0.1.0rc0/feffery_antd_charts.egg-info/
--rw-rw-rw-   0        0        0      274 2024-04-30 04:38:03.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1780 2024-04-30 04:38:03.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 04:38:03.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-30 04:38:03.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-30 04:38:03.000000 feffery_antd_charts-0.1.0rc0/feffery_antd_charts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2482 2024-04-29 08:40:44.000000 feffery_antd_charts-0.1.0rc0/package.json
--rw-rw-rw-   0        0        0       42 2024-04-30 04:38:03.966514 feffery_antd_charts-0.1.0rc0/setup.cfg
--rw-rw-rw-   0        0        0      622 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 03:30:00.144135 feffery_antd_charts-0.1.0rc1/
+-rw-rw-rw-   0        0        0     1087 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc1/LICENSE
+-rw-rw-rw-   0        0        0      434 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0      274 2024-05-05 03:30:00.142715 feffery_antd_charts-0.1.0rc1/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 03:30:00.132350 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/
+-rw-rw-rw-   0        0        0     6640 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdArea.py
+-rw-rw-rw-   0        0        0     7493 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdBar.py
+-rw-rw-rw-   0        0        0     5139 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdBidirectionalBar.py
+-rw-rw-rw-   0        0        0     5534 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdBox.py
+-rw-rw-rw-   0        0        0     5644 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdBullet.py
+-rw-rw-rw-   0        0        0     4673 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdChord.py
+-rw-rw-rw-   0        0        0     7920 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdColumn.py
+-rw-rw-rw-   0        0        0     7128 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdDecompositionTree.py
+-rw-rw-rw-   0        0        0     6061 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdDualAxes.py
+-rw-rw-rw-   0        0        0     6785 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdFundFlow.py
+-rw-rw-rw-   0        0        0     5921 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdFunnel.py
+-rw-rw-rw-   0        0        0     6081 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdGauge.py
+-rw-rw-rw-   0        0        0     7537 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdHeatmap.py
+-rw-rw-rw-   0        0        0     5484 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdHistogram.py
+-rw-rw-rw-   0        0        0     6167 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdLine.py
+-rw-rw-rw-   0        0        0     5731 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdLiquid.py
+-rw-rw-rw-   0        0        0     6727 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdPie.py
+-rw-rw-rw-   0        0        0     3837 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdProgress.py
+-rw-rw-rw-   0        0        0     6502 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdRadar.py
+-rw-rw-rw-   0        0        0     7255 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdRadialBar.py
+-rw-rw-rw-   0        0        0     9688 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdRadialTree.py
+-rw-rw-rw-   0        0        0     5206 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdRingProgress.py
+-rw-rw-rw-   0        0        0     5913 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdRose.py
+-rw-rw-rw-   0        0        0     5126 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdSankey.py
+-rw-rw-rw-   0        0        0     6869 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdScatter.py
+-rw-rw-rw-   0        0        0     5405 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdStock.py
+-rw-rw-rw-   0        0        0     5870 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdSunburst.py
+-rw-rw-rw-   0        0        0     4856 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdTinyArea.py
+-rw-rw-rw-   0        0        0     4704 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdTinyColumn.py
+-rw-rw-rw-   0        0        0     4965 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdTinyLine.py
+-rw-rw-rw-   0        0        0     5162 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdTreemap.py
+-rw-rw-rw-   0        0        0     5391 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdVenn.py
+-rw-rw-rw-   0        0        0     5758 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdViolin.py
+-rw-rw-rw-   0        0        0     6250 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdWaterfall.py
+-rw-rw-rw-   0        0        0     6095 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdWordCloud.py
+-rw-rw-rw-   0        0        0     2666 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/__init__.py
+-rw-rw-rw-   0        0        0     2063 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/_imports_.py
+-rw-rw-rw-   0        0        0     2317 2024-05-05 03:28:36.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/alias.py
+-rw-rw-rw-   0        0        0  1304078 2024-05-05 03:29:51.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/async-graphs.js
+-rw-rw-rw-   0        0        0  1410792 2024-05-05 03:29:51.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/async-plots.js
+-rw-rw-rw-   0        0        0    77099 2024-05-05 03:29:51.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/feffery_antd_charts.min.js
+-rw-rw-rw-   0        0        0   447318 2024-05-05 03:29:55.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/metadata.json
+-rw-rw-rw-   0        0        0     2521 2024-05-05 03:29:52.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts/package-info.json
+drwxrwxrwx   0        0        0        0 2024-05-05 03:30:00.141704 feffery_antd_charts-0.1.0rc1/feffery_antd_charts.egg-info/
+-rw-rw-rw-   0        0        0      274 2024-05-05 03:30:00.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1780 2024-05-05 03:30:00.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 03:30:00.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-05 03:30:00.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-05 03:30:00.000000 feffery_antd_charts-0.1.0rc1/feffery_antd_charts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2521 2024-05-01 14:52:03.000000 feffery_antd_charts-0.1.0rc1/package.json
+-rw-rw-rw-   0        0        0       42 2024-05-05 03:30:00.145354 feffery_antd_charts-0.1.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0      622 2024-03-22 06:14:30.000000 feffery_antd_charts-0.1.0rc1/setup.py
```

### Comparing `feffery_antd_charts-0.1.0rc0/LICENSE` & `feffery_antd_charts-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdArea.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdArea.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdBar.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdBar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdBidirectionalBar.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdBidirectionalBar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdBox.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdBox.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdBullet.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdBullet.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdChord.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdChord.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdColumn.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdColumn.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdDecompositionTree.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdDecompositionTree.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 - id (string; optional)
 
 - animate (boolean; optional)
 
 - autoFit (boolean; optional)
 
-- behaviors (list of a value equal to: 'drag-canvas', 'scroll-canvas', 'zoom-canvas', 'drag-node's; optional)
+- behaviors (list of a value equal to: 'drag-canvas', 'scroll-canvas', 'zoom-canvas', 'drag-node', 'click-select's; optional)
 
 - className (string; optional)
 
 - data (dict; required)
 
 - edgeCfg (dict; optional)
 
@@ -222,26 +222,37 @@
 
             `style` is a dict with keys:
 
     - func (string; optional)
 
     - type (a value equal to: 'indicator-card'; optional)
 
+- recentlyNodeClickRecord (dict; optional):
+    节点点击事件监听.
+
+    `recentlyNodeClickRecord` is a dict with keys:
+
+    - data (dict; optional):
+        事件对应节点信息，点击空白处时为空.
+
+    - timestamp (number; optional):
+        事件触发时间戳.
+
 - style (dict; optional)
 
 - width (number; optional)"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_antd_charts'
     _type = 'AntdDecompositionTree'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, key=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, data=Component.REQUIRED, width=Component.UNDEFINED, height=Component.UNDEFINED, autoFit=Component.UNDEFINED, nodeCfg=Component.UNDEFINED, edgeCfg=Component.UNDEFINED, level=Component.UNDEFINED, behaviors=Component.UNDEFINED, markerCfg=Component.UNDEFINED, animate=Component.UNDEFINED, minimapCfg=Component.UNDEFINED, layout=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'animate', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'level', 'loading_state', 'markerCfg', 'minimapCfg', 'nodeCfg', 'style', 'width']
+    def __init__(self, id=Component.UNDEFINED, key=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, data=Component.REQUIRED, width=Component.UNDEFINED, height=Component.UNDEFINED, autoFit=Component.UNDEFINED, nodeCfg=Component.UNDEFINED, edgeCfg=Component.UNDEFINED, level=Component.UNDEFINED, behaviors=Component.UNDEFINED, markerCfg=Component.UNDEFINED, animate=Component.UNDEFINED, minimapCfg=Component.UNDEFINED, layout=Component.UNDEFINED, recentlyNodeClickRecord=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'animate', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'level', 'loading_state', 'markerCfg', 'minimapCfg', 'nodeCfg', 'recentlyNodeClickRecord', 'style', 'width']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'animate', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'level', 'loading_state', 'markerCfg', 'minimapCfg', 'nodeCfg', 'style', 'width']
+        self.available_properties = ['id', 'animate', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'level', 'loading_state', 'markerCfg', 'minimapCfg', 'nodeCfg', 'recentlyNodeClickRecord', 'style', 'width']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         for k in ['data']:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdDualAxes.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdDualAxes.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdFundFlow.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdFundFlow.py`

 * *Files 11% similar despite different names*

```diff
@@ -214,26 +214,37 @@
 
             `style` is a dict with keys:
 
     - func (string; optional)
 
     - type (a value equal to: 'fund-card'; optional)
 
+- recentlyNodeClickRecord (dict; optional):
+    节点点击事件监听.
+
+    `recentlyNodeClickRecord` is a dict with keys:
+
+    - data (dict; optional):
+        事件对应节点信息，点击空白处时为空.
+
+    - timestamp (number; optional):
+        事件触发时间戳.
+
 - style (dict; optional)
 
 - width (number; optional)"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_antd_charts'
     _type = 'AntdFundFlow'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, key=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, data=Component.REQUIRED, width=Component.UNDEFINED, height=Component.UNDEFINED, autoFit=Component.UNDEFINED, nodeCfg=Component.UNDEFINED, edgeCfg=Component.UNDEFINED, behaviors=Component.UNDEFINED, markerCfg=Component.UNDEFINED, minimapCfg=Component.UNDEFINED, layout=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'loading_state', 'markerCfg', 'minimapCfg', 'nodeCfg', 'style', 'width']
+    def __init__(self, id=Component.UNDEFINED, key=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, data=Component.REQUIRED, width=Component.UNDEFINED, height=Component.UNDEFINED, autoFit=Component.UNDEFINED, nodeCfg=Component.UNDEFINED, edgeCfg=Component.UNDEFINED, behaviors=Component.UNDEFINED, markerCfg=Component.UNDEFINED, minimapCfg=Component.UNDEFINED, layout=Component.UNDEFINED, recentlyNodeClickRecord=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'loading_state', 'markerCfg', 'minimapCfg', 'nodeCfg', 'recentlyNodeClickRecord', 'style', 'width']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'loading_state', 'markerCfg', 'minimapCfg', 'nodeCfg', 'style', 'width']
+        self.available_properties = ['id', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'loading_state', 'markerCfg', 'minimapCfg', 'nodeCfg', 'recentlyNodeClickRecord', 'style', 'width']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         for k in ['data']:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdFunnel.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdFunnel.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdGauge.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdGauge.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdHeatmap.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdHeatmap.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdHistogram.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdHistogram.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdLine.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdLine.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdLiquid.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdLiquid.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdPie.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdPie.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdProgress.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdRadar.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdRadar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdRadialBar.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdRadialBar.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdRadialTree.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdRadialTree.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 - animate (boolean; default False):
     是否开启动画  默认值：`False`.
 
 - autoFit (boolean; default True):
     图表是否自适应容器宽高，设置为`True`时，`width`与`height`参数将失效  默认值：`True`.
 
-- behaviors (list of a value equal to: 'drag-canvas', 'scroll-canvas', 'zoom-canvas', 'drag-node's; default ['drag-canvas', 'zoom-canvas']):
+- behaviors (list of a value equal to: 'drag-canvas', 'scroll-canvas', 'zoom-canvas', 'drag-node', 'click-select's; default ['drag-canvas', 'zoom-canvas']):
     启用的交互模式，可选项有`'drag-canvas'`（拖拽画布）、`'scroll-canvas'`（滚轮滚动画布）、
-    `'zoom-canvas'`（缩放画布）、`'drag-node'`（拖拽节点）  默认值：`['drag-canvas',
-    'zoom-canvas']`.
+    `'zoom-canvas'`（缩放画布）、`'drag-node'`（拖拽节点）、'click-select'（节点选择）
+    默认值：`['drag-canvas', 'zoom-canvas']`.
 
 - className (string; optional):
     css类名.
 
 - data (dict; required):
     必填，定义绘图所需数据.
 
@@ -195,39 +195,83 @@
 
             回调函数字符串.
 
     - type (a value equal to: 'icon-node', 'card', 'circle', 'rect', 'ellipse', 'diamond', 'triangle', 'star', 'image', 'modelRect', 'donut'; optional):
         节点类型，可选项有`'icon-node'`、`'card'`、`'circle'`、`'rect'`、`'ellipse'`、`'diamond'`、`'triangle'`、
         `'star'`、`'image'`、`'modelRect'`、`'donut'`.
 
+- recentlyEdgeClickRecord (dict; optional):
+    边点击事件监听.
+
+    `recentlyEdgeClickRecord` is a dict with keys:
+
+    - data (dict; optional):
+        事件对应节点信息，点击空白处时为空.
+
+    - timestamp (number; optional):
+        事件触发时间戳.
+
+- recentlyEdgeDoubleClickRecord (dict; optional):
+    边双击事件监听.
+
+    `recentlyEdgeDoubleClickRecord` is a dict with keys:
+
+    - data (dict; optional):
+        事件对应节点信息，点击空白处时为空.
+
+    - timestamp (number; optional):
+        事件触发时间戳.
+
 - recentlyNodeClickRecord (dict; optional):
     节点点击事件监听.
 
     `recentlyNodeClickRecord` is a dict with keys:
 
     - data (dict; optional):
         事件对应节点信息，点击空白处时为空.
 
     - timestamp (number; optional):
         事件触发时间戳.
 
+- recentlyNodeDoubleClickRecord (dict; optional):
+    节点双击事件监听.
+
+    `recentlyNodeDoubleClickRecord` is a dict with keys:
+
+    - data (dict; optional):
+        事件对应节点信息，点击空白处时为空.
+
+    - timestamp (number; optional):
+        事件触发时间戳.
+
+- selectedNodes (dict; optional):
+    节点选中事件监听，需要在``behaviors``中开启``click-select``.
+
+    `selectedNodes` is a dict with keys:
+
+    - data (list; optional):
+        对应选中的节点信息数组.
+
+    - timestamp (number; optional):
+        事件触发时间戳.
+
 - style (dict; optional):
     css样式.
 
 - width (number; optional):
     图表容器像素宽度."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'feffery_antd_charts'
     _type = 'AntdRadialTree'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, key=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, data=Component.REQUIRED, width=Component.UNDEFINED, height=Component.UNDEFINED, autoFit=Component.UNDEFINED, nodeCfg=Component.UNDEFINED, edgeCfg=Component.UNDEFINED, behaviors=Component.UNDEFINED, animate=Component.UNDEFINED, minimapCfg=Component.UNDEFINED, layout=Component.UNDEFINED, recentlyNodeClickRecord=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'animate', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'loading_state', 'minimapCfg', 'nodeCfg', 'recentlyNodeClickRecord', 'style', 'width']
+    def __init__(self, id=Component.UNDEFINED, key=Component.UNDEFINED, className=Component.UNDEFINED, style=Component.UNDEFINED, data=Component.REQUIRED, width=Component.UNDEFINED, height=Component.UNDEFINED, autoFit=Component.UNDEFINED, nodeCfg=Component.UNDEFINED, edgeCfg=Component.UNDEFINED, behaviors=Component.UNDEFINED, animate=Component.UNDEFINED, minimapCfg=Component.UNDEFINED, layout=Component.UNDEFINED, recentlyNodeClickRecord=Component.UNDEFINED, recentlyNodeDoubleClickRecord=Component.UNDEFINED, recentlyEdgeClickRecord=Component.UNDEFINED, recentlyEdgeDoubleClickRecord=Component.UNDEFINED, selectedNodes=Component.UNDEFINED, loading_state=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'animate', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'loading_state', 'minimapCfg', 'nodeCfg', 'recentlyEdgeClickRecord', 'recentlyEdgeDoubleClickRecord', 'recentlyNodeClickRecord', 'recentlyNodeDoubleClickRecord', 'selectedNodes', 'style', 'width']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'animate', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'loading_state', 'minimapCfg', 'nodeCfg', 'recentlyNodeClickRecord', 'style', 'width']
+        self.available_properties = ['id', 'animate', 'autoFit', 'behaviors', 'className', 'data', 'edgeCfg', 'height', 'key', 'layout', 'loading_state', 'minimapCfg', 'nodeCfg', 'recentlyEdgeClickRecord', 'recentlyEdgeDoubleClickRecord', 'recentlyNodeClickRecord', 'recentlyNodeDoubleClickRecord', 'selectedNodes', 'style', 'width']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         for k in ['data']:
```

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdRingProgress.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdRingProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdRose.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdRose.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdSankey.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdSankey.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdScatter.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdScatter.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdStock.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdStock.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdSunburst.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdSunburst.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdTinyArea.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdTinyArea.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdTinyColumn.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdTinyColumn.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdTinyLine.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdTinyLine.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdTreemap.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdTreemap.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdVenn.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdVenn.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdViolin.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdViolin.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdWaterfall.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdWaterfall.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/AntdWordCloud.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/AntdWordCloud.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/__init__.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/_imports_.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/_imports_.py`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/alias.py` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/alias.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,50 +4,70 @@
 from .AntdBox import AntdBox as Box
 from .AntdBullet import AntdBullet as Bullet
 from .AntdChord import AntdChord as Chord
 from .AntdColumn import AntdColumn as Column
 from .AntdDualAxes import AntdDualAxes as DualAxes
 from .AntdFunnel import AntdFunnel as Funnel
 from .AntdGauge import AntdGauge as Gauge
+from .AntdHeatmap import AntdHeatmap as Heatmap
 from .AntdHistogram import AntdHistogram as Histogram
 from .AntdLine import AntdLine as Line
 from .AntdLiquid import AntdLiquid as Liquid
 from .AntdPie import AntdPie as Pie
+from .AntdProgress import AntdProgress as Progress
 from .AntdRadar import AntdRadar as Radar
+from .AntdRadialBar import AntdRadialBar as RadialBar
+from .AntdRingProgress import AntdRingProgress as RingProgress
 from .AntdRose import AntdRose as Rose
 from .AntdSankey import AntdSankey as Sankey
 from .AntdScatter import AntdScatter as Scatter
 from .AntdStock import AntdStock as Stock
 from .AntdSunburst import AntdSunburst as Sunburst
+from .AntdTinyArea import AntdTinyArea as TinyArea
+from .AntdTinyColumn import AntdTinyColumn as TinyColumn
 from .AntdTinyLine import AntdTinyLine as TinyLine
 from .AntdTreemap import AntdTreemap as Treemap
+from .AntdVenn import AntdVenn as Venn
+from .AntdViolin import AntdViolin as Violin
+from .AntdWaterfall import AntdWaterfall as Waterfall
 from .AntdWordCloud import AntdWordCloud as WordCloud
 from .AntdDecompositionTree import AntdDecompositionTree as DecompositionTree
 from .AntdFundFlow import AntdFundFlow as FundFlow
+from .AntdRadialTree import AntdRadialTree as RadialTree
 
 __all__ = [
-    "Area",
-    "Bar",
-    "BidirectionalBar",
-    "Box",
-    "Bullet",
-    "Chord",
-    "Column",
-    "DualAxes",
-    "Funnel",
-    "Gauge",
-    "Histogram",
-    "Line",
-    "Liquid",
-    "Pie",
-    "Radar",
-    "Rose",
-    "Sankey",
-    "Scatter",
-    "Stock",
-    "Sunburst",
-    "TinyLine",
-    "Treemap",
-    "WordCloud",
-    "DecompositionTree",
-    "FundFlow"
+    'Area',
+    'Bar',
+    'BidirectionalBar',
+    'Box',
+    'Bullet',
+    'Chord',
+    'Column',
+    'DualAxes',
+    'Funnel',
+    'Gauge',
+    'Heatmap',
+    'Histogram',
+    'Line',
+    'Liquid',
+    'Pie',
+    'Progress',
+    'Radar',
+    'RadialBar',
+    'RingProgress',
+    'Rose',
+    'Sankey',
+    'Scatter',
+    'Stock',
+    'Sunburst',
+    'TinyArea',
+    'TinyColumn',
+    'TinyLine',
+    'Treemap',
+    'Venn',
+    'Violin',
+    'Waterfall',
+    'WordCloud',
+    'DecompositionTree',
+    'FundFlow',
+    'RadialTree',
 ]
```

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/async-graphs.js` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/async-graphs.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -175,14 +175,34 @@
                             layout: layout
                         });
                     return config.nodeCfg = Object(lodash__WEBPACK_IMPORTED_MODULE_2__.cloneDeep)(nodeCfg), null != nodeCfg && null != (_nodeCfg$style = nodeCfg.style) && _nodeCfg$style.func && (config.nodeCfg.style = eval(nodeCfg.style.func)), null != nodeCfg && null != (_nodeCfg$title = nodeCfg.title) && null != (_nodeCfg$title = _nodeCfg$title.style) && _nodeCfg$title.func && (config.nodeCfg.title.style = eval(nodeCfg.title.style.func)), null != nodeCfg && null != (_nodeCfg$label = nodeCfg.label) && null != (_nodeCfg$label = _nodeCfg$label.style) && _nodeCfg$label.func && (config.nodeCfg.label.style = eval(nodeCfg.label.style.func)), null != nodeCfg && null != (_nodeCfg$items = nodeCfg.items) && null != (_nodeCfg$items = _nodeCfg$items.style) && _nodeCfg$items.func && (config.nodeCfg.items.style = eval(nodeCfg.items.style.func)), null != nodeCfg && null != (_nodeCfg$badge = nodeCfg.badge) && null != (_nodeCfg$badge = _nodeCfg$badge.style) && _nodeCfg$badge.func && (config.nodeCfg.badge.style = eval(nodeCfg.badge.style.func)), null != nodeCfg && null != (_nodeCfg$percent = nodeCfg.percent) && null != (_nodeCfg$percent = _nodeCfg$percent.style) && _nodeCfg$percent.func && (config.nodeCfg.percent.style = eval(nodeCfg.percent.style.func)), config.edgeCfg = Object(lodash__WEBPACK_IMPORTED_MODULE_2__.cloneDeep)(edgeCfg), null != edgeCfg && null != (_edgeCfg$style = edgeCfg.style) && _edgeCfg$style.func && (config.edgeCfg.style = eval(edgeCfg.style.func)), null != edgeCfg && null != (_edgeCfg$label = edgeCfg.label) && null != (_edgeCfg$label = _edgeCfg$label.style) && _edgeCfg$label.func && (config.edgeCfg.label.style = eval(edgeCfg.label.style.func)), config.markerCfg = Object(lodash__WEBPACK_IMPORTED_MODULE_2__.cloneDeep)(markerCfg), null != markerCfg && markerCfg.func && (config.markerCfg = eval(markerCfg.func)), config = Object(lodash__WEBPACK_IMPORTED_MODULE_2__.omitBy)(config, lodash__WEBPACK_IMPORTED_MODULE_2__.isUndefined), react__WEBPACK_IMPORTED_MODULE_1___default.a.createElement(_ant_design_graphs__WEBPACK_IMPORTED_MODULE_0__.a, _extends({
                         id: id,
                         key: key,
                         className: className,
                         style: style,
+                        onReady: function(t) {
+                            t.on("canvas:click", function(t) {
+                                setProps({
+                                    recentlyNodeClickRecord: {
+                                        timestamp: (new Date).valueOf(),
+                                        data: null
+                                    }
+                                })
+                            }), t.on("node:mousedown", function(t) {
+                                setProps({
+                                    recentlyNodeClickRecord: {
+                                        timestamp: (new Date).valueOf(),
+                                        data: {
+                                            id: t.item._cfg.model.id,
+                                            value: t.item._cfg.model.value
+                                        }
+                                    }
+                                })
+                            })
+                        },
                         "data-dash-is-loading": loading_state && loading_state.is_loading || void 0
                     }, config))
                 }
             }])
         }(react__WEBPACK_IMPORTED_MODULE_1__.Component);
         AntdDecompositionTree.defaultProps = _components_graphs_AntdDecompositionTree_react__WEBPACK_IMPORTED_MODULE_3__.b, AntdDecompositionTree.propTypes = _components_graphs_AntdDecompositionTree_react__WEBPACK_IMPORTED_MODULE_3__.c
     }, function(module, __webpack_exports__, __webpack_require__) {
@@ -357,14 +377,34 @@
                             layout: layout
                         });
                     return config.nodeCfg = Object(lodash__WEBPACK_IMPORTED_MODULE_2__.cloneDeep)(nodeCfg), null != nodeCfg && null != (_nodeCfg$style = nodeCfg.style) && _nodeCfg$style.func && (config.nodeCfg.style = eval(nodeCfg.style.func)), null != nodeCfg && null != (_nodeCfg$title = nodeCfg.title) && null != (_nodeCfg$title = _nodeCfg$title.style) && _nodeCfg$title.func && (config.nodeCfg.title.style = eval(nodeCfg.title.style.func)), null != nodeCfg && null != (_nodeCfg$label = nodeCfg.label) && null != (_nodeCfg$label = _nodeCfg$label.style) && _nodeCfg$label.func && (config.nodeCfg.label.style = eval(nodeCfg.label.style.func)), null != nodeCfg && null != (_nodeCfg$items = nodeCfg.items) && null != (_nodeCfg$items = _nodeCfg$items.style) && _nodeCfg$items.func && (config.nodeCfg.items.style = eval(nodeCfg.items.style.func)), null != nodeCfg && null != (_nodeCfg$badge = nodeCfg.badge) && null != (_nodeCfg$badge = _nodeCfg$badge.style) && _nodeCfg$badge.func && (config.nodeCfg.badge.style = eval(nodeCfg.badge.style.func)), null != nodeCfg && null != (_nodeCfg$percent = nodeCfg.percent) && null != (_nodeCfg$percent = _nodeCfg$percent.style) && _nodeCfg$percent.func && (config.nodeCfg.percent.style = eval(nodeCfg.percent.style.func)), config.edgeCfg = Object(lodash__WEBPACK_IMPORTED_MODULE_2__.cloneDeep)(edgeCfg), null != edgeCfg && null != (_edgeCfg$style = edgeCfg.style) && _edgeCfg$style.func && (config.edgeCfg.style = eval(edgeCfg.style.func)), null != edgeCfg && null != (_edgeCfg$label = edgeCfg.label) && null != (_edgeCfg$label = _edgeCfg$label.style) && _edgeCfg$label.func && (config.edgeCfg.label.style = eval(edgeCfg.label.style.func)), config.markerCfg = Object(lodash__WEBPACK_IMPORTED_MODULE_2__.cloneDeep)(markerCfg), null != markerCfg && markerCfg.func && (config.markerCfg = eval(markerCfg.func)), config = Object(lodash__WEBPACK_IMPORTED_MODULE_2__.omitBy)(config, lodash__WEBPACK_IMPORTED_MODULE_2__.isUndefined), react__WEBPACK_IMPORTED_MODULE_1___default.a.createElement(_ant_design_graphs__WEBPACK_IMPORTED_MODULE_0__.a, _extends({
                         id: id,
                         key: key,
                         className: className,
                         style: style,
+                        onReady: function(t) {
+                            t.on("canvas:click", function(t) {
+                                setProps({
+                                    recentlyNodeClickRecord: {
+                                        timestamp: (new Date).valueOf(),
+                                        data: null
+                                    }
+                                })
+                            }), t.on("node:mousedown", function(t) {
+                                setProps({
+                                    recentlyNodeClickRecord: {
+                                        timestamp: (new Date).valueOf(),
+                                        data: {
+                                            id: t.item._cfg.model.id,
+                                            value: t.item._cfg.model.value
+                                        }
+                                    }
+                                })
+                            })
+                        },
                         "data-dash-is-loading": loading_state && loading_state.is_loading || void 0
                     }, config))
                 }
             }])
         }(react__WEBPACK_IMPORTED_MODULE_1__.Component);
         AntdFundFlow.defaultProps = _components_graphs_AntdFundFlow_react__WEBPACK_IMPORTED_MODULE_3__.b, AntdFundFlow.propTypes = _components_graphs_AntdFundFlow_react__WEBPACK_IMPORTED_MODULE_3__.c
     }, , , , , , , , , , , , , function(module, __webpack_exports__, __webpack_require__) {
@@ -471,26 +511,83 @@
                 style: style,
                 onReady: function(t) {
                     t.on("canvas:click", function(t) {
                         setProps({
                             recentlyNodeClickRecord: {
                                 timestamp: (new Date).valueOf(),
                                 data: null
+                            },
+                            recentlyEdgeClickRecord: {
+                                timestamp: (new Date).valueOf(),
+                                data: null
+                            }
+                        })
+                    }), t.on("canvas:dblclick", function(t) {
+                        setProps({
+                            recentlyNodeDoubleClickRecord: {
+                                timestamp: (new Date).valueOf(),
+                                data: null
+                            },
+                            recentlyEdgeDoubleClickRecord: {
+                                timestamp: (new Date).valueOf(),
+                                data: null
                             }
                         })
                     }), t.on("node:mousedown", function(t) {
                         setProps({
                             recentlyNodeClickRecord: {
                                 timestamp: (new Date).valueOf(),
                                 data: {
                                     id: t.item._cfg.model.id,
                                     value: t.item._cfg.model.value
                                 }
                             }
                         })
+                    }), t.on("node:dblclick", function(t) {
+                        setProps({
+                            recentlyNodeDoubleClickRecord: {
+                                timestamp: (new Date).valueOf(),
+                                data: {
+                                    id: t.item._cfg.model.id,
+                                    value: t.item._cfg.model.value
+                                }
+                            }
+                        })
+                    }), t.on("edge:mousedown", function(t) {
+                        setProps({
+                            recentlyEdgeClickRecord: {
+                                timestamp: (new Date).valueOf(),
+                                data: {
+                                    source: t.item._cfg.model.source,
+                                    target: t.item._cfg.model.target
+                                }
+                            }
+                        })
+                    }), t.on("edge:dblclick", function(t) {
+                        setProps({
+                            recentlyEdgeDoubleClickRecord: {
+                                timestamp: (new Date).valueOf(),
+                                data: {
+                                    source: t.item._cfg.model.source,
+                                    target: t.item._cfg.model.target
+                                }
+                            }
+                        })
+                    }), t.on("nodeselectchange", function(t) {
+                        setProps({
+                            selectedNodes: {
+                                timestamp: (new Date).valueOf(),
+                                data: t.selectedItems.nodes.map(function(t) {
+                                    return {
+                                        id: t._cfg.model.id,
+                                        value: t._cfg.model.value
+                                    }
+                                })
+                            }
+                        })
                     })
                 },
                 "data-dash-is-loading": loading_state && loading_state.is_loading || void 0
             }, config))
         };
         AntdRadialTree.defaultProps = _components_graphs_AntdRadialTree_react__WEBPACK_IMPORTED_MODULE_3__.b, AntdRadialTree.propTypes = _components_graphs_AntdRadialTree_react__WEBPACK_IMPORTED_MODULE_3__.c, __webpack_exports__.default = AntdRadialTree
     }, , , , , , , , , , , , , , function(t, e, n) {
```

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/async-plots.js` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/async-plots.js`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/feffery_antd_charts.min.js` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/feffery_antd_charts.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
-window.feffery_antd_charts = function(s) {
+window.feffery_antd_charts = function(l) {
     function a(a) {
-        for (var e, n, t = a[0], r = a[1], o = 0, i = []; o < t.length; o++) n = t[o], Object.prototype.hasOwnProperty.call(l, n) && l[n] && i.push(l[n][0]), l[n] = 0;
-        for (e in r) Object.prototype.hasOwnProperty.call(r, e) && (s[e] = r[e]);
+        for (var e, n, t = a[0], r = a[1], o = 0, i = []; o < t.length; o++) n = t[o], Object.prototype.hasOwnProperty.call(s, n) && s[n] && i.push(s[n][0]), s[n] = 0;
+        for (e in r) Object.prototype.hasOwnProperty.call(r, e) && (l[e] = r[e]);
         for (g && g(a); i.length;) i.shift()()
     }
     var n = {},
-        l = {
+        s = {
             2: 0
         };
 
     function c(a) {
         return u.p + "" + ({
             0: "async-plots",
             1: "async-graphs"
@@ -18,32 +18,32 @@
 
     function u(a) {
         var e;
         return (n[a] || (e = n[a] = {
             i: a,
             l: !1,
             exports: {}
-        }, s[a].call(e.exports, e, e.exports, u), e.l = !0, e)).exports
+        }, l[a].call(e.exports, e, e.exports, u), e.l = !0, e)).exports
     }
     u.e = function(t) {
         var a, r, o, e, i, n = [],
-            s = l[t];
-        return 0 !== s && (s ? n.push(s[2]) : (a = new Promise(function(a, e) {
-            s = l[t] = [a, e]
-        }), n.push(s[2] = a), (r = document.createElement("script")).charset = "utf-8", r.timeout = 120, u.nc && r.setAttribute("nonce", u.nc), r.src = c(t), o = new Error, e = function(a) {
+            l = s[t];
+        return 0 !== l && (l ? n.push(l[2]) : (a = new Promise(function(a, e) {
+            l = s[t] = [a, e]
+        }), n.push(l[2] = a), (r = document.createElement("script")).charset = "utf-8", r.timeout = 120, u.nc && r.setAttribute("nonce", u.nc), r.src = c(t), o = new Error, e = function(a) {
             r.onerror = r.onload = null, clearTimeout(i);
-            var e, n = l[t];
-            0 !== n && (n && (e = a && ("load" === a.type ? "missing" : a.type), a = a && a.target && a.target.src, o.message = "Loading chunk " + t + " failed.\n(" + e + ": " + a + ")", o.name = "ChunkLoadError", o.type = e, o.request = a, n[1](o)), l[t] = void 0)
+            var e, n = s[t];
+            0 !== n && (n && (e = a && ("load" === a.type ? "missing" : a.type), a = a && a.target && a.target.src, o.message = "Loading chunk " + t + " failed.\n(" + e + ": " + a + ")", o.name = "ChunkLoadError", o.type = e, o.request = a, n[1](o)), s[t] = void 0)
         }, i = setTimeout(function() {
             e({
                 type: "timeout",
                 target: r
             })
         }, 12e4), r.onerror = r.onload = e, document.head.appendChild(r))), Promise.all(n)
-    }, u.m = s, u.c = n, u.d = function(a, e, n) {
+    }, u.m = l, u.c = n, u.d = function(a, e, n) {
         u.o(a, e) || Object.defineProperty(a, e, {
             enumerable: !0,
             get: n
         })
     }, u.r = function(a) {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(a, Symbol.toStringTag, {
             value: "Module"
@@ -89,15 +89,15 @@
     Object.defineProperty(u, "p", {
         get: (e = t().src.split("/").slice(0, -1).join("/") + "/", function() {
             return e
         })
     }), void 0 !== c && (r = c, c = function(a) {
         var e, n = /\/_dash-component-suites\//.test(t().src),
             a = r(a);
-        return n ? ((e = (n = a.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_1_0-rc0m1714451856"), n.splice(-1, 1, e.join(".")), n.join("/")) : a
+        return n ? ((e = (n = a.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_1_0-rc1m1714879774"), n.splice(-1, 1, e.join(".")), n.join("/")) : a
     });
     var o = (i = window.webpackJsonpfeffery_antd_charts = window.webpackJsonpfeffery_antd_charts || []).push.bind(i);
     i.push = a;
     for (var i = i.slice(), d = 0; d < i.length; d++) a(i[d]);
     var g = o;
     return u(u.s = 34)
 }([function(a, e) {
@@ -105,17 +105,17 @@
 }, function(a, e, n) {
     "use strict";
     n.d(e, "d", function() {
         return o
     }), n.d(e, "h", function() {
         return i
     }), n.d(e, "c", function() {
-        return s
-    }), n.d(e, "g", function() {
         return l
+    }), n.d(e, "g", function() {
+        return s
     }), n.d(e, "f", function() {
         return c
     }), n.d(e, "n", function() {
         return u
     }), n.d(e, "b", function() {
         return d
     }), n.d(e, "j", function() {
@@ -200,15 +200,15 @@
             nice: n.a.bool,
             ticks: n.a.arrayOf(n.a.any),
             minTickInterval: n.a.number,
             tickCount: n.a.number,
             maxTickCount: n.a.number,
             showLast: n.a.bool
         })),
-        s = n.a.oneOfType([n.a.bool, n.a.exact({
+        l = n.a.oneOfType([n.a.bool, n.a.exact({
             top: n.a.bool,
             range: n.a.arrayOf(n.a.number),
             position: n.a.string,
             title: n.a.exact({
                 text: n.a.string,
                 style: o,
                 position: n.a.string,
@@ -256,15 +256,15 @@
             min: n.a.number,
             max: n.a.number,
             minLimit: n.a.number,
             maxLimit: n.a.number,
             tickCount: n.a.number,
             tickInterval: n.a.number
         })]),
-        l = n.a.oneOfType([n.a.bool, n.a.exact({
+        s = n.a.oneOfType([n.a.bool, n.a.exact({
             position: n.a.string,
             layout: n.a.string,
             radio: n.a.bool,
             title: n.a.exact({
                 text: n.a.string,
                 spacing: n.a.number,
                 style: o
@@ -512,72 +512,72 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 55))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.number).isRequired,
-            meta: s.h,
+            meta: l.h,
             smooth: i.a.bool,
             connectNulls: i.a.bool,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            lineStyle: i.a.oneOfType([s.d, i.a.exact({
+            lineStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             point: i.a.exact({
                 color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                     func: i.a.string
                 })]),
                 shape: i.a.oneOfType([i.a.string, i.a.exact({
                     func: i.a.string
                 })]),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })])
             }),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -592,106 +592,106 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 39))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.string.isRequired,
             seriesField: i.a.string,
             groupField: i.a.string,
             isStack: i.a.bool,
             isGroup: i.a.bool,
             isRange: i.a.bool,
             isPercent: i.a.bool,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            slider: s.k,
+            slider: l.k,
             intervalPadding: i.a.number,
             dodgePadding: i.a.number,
             minColumnWidth: i.a.number,
             maxColumnWidth: i.a.number,
-            columnStyle: i.a.oneOfType([s.d, i.a.exact({
+            columnStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             columnBackground: i.a.exact({
-                style: s.d
+                style: l.d
             }),
             columnWidthRatio: i.a.number,
             marginRatio: i.a.number,
-            scrollbar: s.j,
+            scrollbar: l.j,
             conversionTag: i.a.exact({
                 size: i.a.number,
                 spacing: i.a.number,
                 offset: i.a.number,
                 arrow: i.a.oneOfType([i.a.bool, i.a.exact({
                     headSize: i.a.number
                 })]),
                 text: i.a.oneOfType([i.a.bool, i.a.exact({
                     formatter: i.a.exact({
                         func: i.a.string
                     }),
-                    style: s.d
+                    style: l.d
                 })])
             }),
             connectedArea: i.a.oneOfType([i.a.exact({
                 trigger: i.a.oneOfType([i.a.bool, i.a.string])
             }), i.a.bool]),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyColumnClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            pattern: s.i,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            pattern: l.i,
+            interactions: l.e,
+            state: l.l,
             recentlyBarClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
@@ -710,88 +710,88 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 36))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.string.isRequired,
             seriesField: i.a.string,
             smooth: i.a.bool,
             stepType: i.a.string,
             connectNulls: i.a.bool,
             isStack: i.a.bool,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            lineStyle: i.a.oneOfType([s.d, i.a.exact({
+            lineStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             point: i.a.exact({
                 color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                     func: i.a.string
                 })]),
                 shape: i.a.oneOfType([i.a.string, i.a.exact({
                     func: i.a.string
                 })]),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })])
             }),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            slider: s.k,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            slider: l.k,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyPointClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -806,97 +806,97 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 37))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.string.isRequired,
             seriesField: i.a.string,
             isPercent: i.a.bool,
             smooth: i.a.bool,
             isStack: i.a.bool,
             startOnZero: i.a.bool,
-            areaStyle: i.a.oneOfType([s.d, i.a.exact({
+            areaStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             line: i.a.exact({
                 color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                     func: i.a.string
                 })]),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })])
             }),
             point: i.a.exact({
                 color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                     func: i.a.string
                 })]),
                 shape: i.a.oneOfType([i.a.string, i.a.exact({
                     func: i.a.string
                 })]),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })])
             }),
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            slider: s.k,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            slider: l.k,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyPointClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            pattern: s.i,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            pattern: l.i,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -911,31 +911,31 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 38))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.string.isRequired,
             seriesField: i.a.string,
             groupField: i.a.string,
             isStack: i.a.bool,
             isGroup: i.a.bool,
             isRange: i.a.bool,
@@ -943,73 +943,73 @@
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
             intervalPadding: i.a.number,
             dodgePadding: i.a.number,
             minBarWidth: i.a.number,
             maxBarWidth: i.a.number,
-            barStyle: i.a.oneOfType([s.d, i.a.exact({
+            barStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             barBackground: i.a.exact({
-                style: s.d
+                style: l.d
             }),
             barWidthRatio: i.a.number,
             marginRatio: i.a.number,
-            scrollbar: s.j,
+            scrollbar: l.j,
             conversionTag: i.a.exact({
                 size: i.a.number,
                 spacing: i.a.number,
                 offset: i.a.number,
                 arrow: i.a.oneOfType([i.a.bool, i.a.exact({
                     headSize: i.a.number
                 })]),
                 text: i.a.oneOfType([i.a.bool, i.a.exact({
                     formatter: i.a.exact({
                         func: i.a.string
                     }),
-                    style: s.d
+                    style: l.d
                 })])
             }),
             connectedArea: i.a.oneOfType([i.a.exact({
                 trigger: i.a.oneOfType([i.a.bool, i.a.string])
             }), i.a.bool]),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyBarClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            pattern: s.i,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            pattern: l.i,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -1024,31 +1024,31 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 40))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             angleField: i.a.string,
             colorField: i.a.string,
             radius: i.a.number,
             innerRadius: i.a.number,
             startAngle: i.a.number,
             endAngle: i.a.number,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
@@ -1078,36 +1078,36 @@
                         func: i.a.string
                     }),
                     rotate: i.a.number,
                     offsetX: i.a.number,
                     offsetY: i.a.number
                 })])
             }), i.a.bool]),
-            pieStyle: i.a.oneOfType([s.d, i.a.exact({
+            pieStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            downloadTrigger: i.a.string,
-            theme: s.m,
-            pattern: s.i,
-            interactions: s.e,
-            state: s.l,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            downloadTrigger: i.a.string,
+            theme: l.m,
+            pattern: l.i,
+            interactions: l.e,
+            state: l.l,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlySectorClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
@@ -1134,101 +1134,101 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 41))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.string.isRequired,
             colorField: i.a.string,
             sizeField: i.a.string,
             shapeField: i.a.string,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
             size: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.exact({
                 func: i.a.string
             })]),
             shape: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            pointStyle: i.a.oneOfType([s.d, i.a.exact({
+            pointStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
-            shapeLegend: s.g,
-            sizeLegend: s.g,
+            shapeLegend: l.g,
+            sizeLegend: l.g,
             quadrant: i.a.exact({
                 xBaseline: i.a.number,
                 yBaseline: i.a.number,
-                lineStyle: s.d,
-                regionStyle: i.a.oneOfType([s.d, i.a.arrayOf(s.d)]),
+                lineStyle: l.d,
+                regionStyle: i.a.oneOfType([l.d, i.a.arrayOf(l.d)]),
                 labels: i.a.arrayOf(i.a.exact({
                     content: i.a.string,
                     position: i.a.arrayOf(i.a.number),
-                    style: s.d
+                    style: l.d
                 }))
             }),
             regressionLine: i.a.exact({
                 type: i.a.oneOf(["exp", "linear", "loess", "log", "poly", "pow", "quad"]),
-                style: s.d,
+                style: l.d,
                 algorithm: i.a.exact({
                     func: i.a.string
                 }),
                 top: i.a.bool
             }),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyPointClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -1243,71 +1243,71 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 42))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.objectOf(i.a.oneOfType([i.a.string, i.a.number]))).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.arrayOf(i.a.string).isRequired,
             risingFill: i.a.string,
             fallingFill: i.a.string,
-            stockStyle: i.a.oneOfType([s.d, i.a.exact({
+            stockStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            slider: s.k,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            slider: l.k,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyAreaClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.any
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -1324,96 +1324,96 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 43))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.string.isRequired,
             seriesField: i.a.string,
             smooth: i.a.bool,
             radius: i.a.number,
             startAngle: i.a.number,
             endAngle: i.a.number,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            lineStyle: i.a.oneOfType([s.d, i.a.exact({
+            lineStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             point: i.a.exact({
                 color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                     func: i.a.string
                 })]),
                 shape: i.a.oneOfType([i.a.string, i.a.exact({
                     func: i.a.string
                 })]),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })])
             }),
             area: i.a.exact({
                 smooth: i.a.bool,
                 color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                     func: i.a.string
                 })]),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })])
             }),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyAreaClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.any
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -1428,31 +1428,31 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 44))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.object.isRequired,
-            meta: s.h,
+            meta: l.h,
             colorField: i.a.string,
             rawFields: i.a.arrayOf(i.a.string),
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
@@ -1465,45 +1465,45 @@
                 ignoreParentValue: i.a.bool
             }),
             drilldown: i.a.exact({
                 enabled: i.a.bool,
                 breadCrumb: i.a.exact({
                     rootText: i.a.string,
                     dividerText: i.a.string,
-                    textStyle: s.d,
-                    activeTextStyle: s.d,
+                    textStyle: l.d,
+                    activeTextStyle: l.d,
                     position: i.a.oneOf(["top-left", "bottom-left"])
                 })
             }),
             radius: i.a.number,
             innerRadius: i.a.number,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            sunburstStyle: i.a.oneOfType([s.d, i.a.exact({
+            sunburstStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             reflect: i.a.bool,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.any
             }),
             recentlyAreaClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.any
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            pattern: s.i,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            pattern: l.i,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -1519,65 +1519,65 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 45))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object),
-            meta: s.h,
+            meta: l.h,
             sourceField: i.a.string,
             targetField: i.a.string,
             weightField: i.a.string,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            nodeStyle: i.a.oneOfType([s.d, i.a.exact({
+            nodeStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
-            edgeStyle: i.a.oneOfType([s.d, i.a.exact({
+            edgeStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             nodeWidthRatio: i.a.number,
             nodePaddingRatio: i.a.number,
-            label: s.f,
-            animation: s.a,
+            label: l.f,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyAreaClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -1592,31 +1592,31 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 46))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object),
-            meta: s.h,
+            meta: l.h,
             wordField: i.a.string.isRequired,
             weightField: i.a.string.isRequired,
             colorField: i.a.string,
             spiral: i.a.oneOf(["archimedean", "rectangular"]),
             placementStrategy: i.a.exact({
                 func: i.a.string
             }),
@@ -1638,35 +1638,35 @@
                 func: i.a.string
             }),
             imageMask: i.a.string,
             randomState: i.a.number,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyWordClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -1681,70 +1681,70 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 47))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object),
-            meta: s.h,
+            meta: l.h,
             sourceField: i.a.string,
             targetField: i.a.string,
             weightField: i.a.string,
             rawFields: i.a.arrayOf(i.a.string),
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            nodeStyle: i.a.oneOfType([s.d, i.a.exact({
+            nodeStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
-            edgeStyle: i.a.oneOfType([s.d, i.a.exact({
+            edgeStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
             nodeWidthRatio: i.a.number,
             nodePaddingRatio: i.a.number,
             nodeAlign: i.a.oneOf(["left", "right", "center", "justify"]),
             nodeDraggable: i.a.bool,
-            animation: s.a,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyAreaClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -1759,79 +1759,79 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 48))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string,
             yField: i.a.string,
             seriesField: i.a.string,
             isGroup: i.a.bool,
             isStack: i.a.bool,
             radius: i.a.number,
             innerRadius: i.a.number,
             startAngle: i.a.number,
             endAngle: i.a.number,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            sectorStyle: i.a.oneOfType([s.d, i.a.exact({
+            sectorStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            xAxis: s.c,
-            yAxis: s.c,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            xAxis: l.c,
+            yAxis: l.c,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyAreaClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.any
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            pattern: s.i,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            pattern: l.i,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -1846,70 +1846,70 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 49))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.object,
-            meta: s.h,
+            meta: l.h,
             colorField: i.a.string.isRequired,
             rawFields: i.a.arrayOf(i.a.string),
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            rectStyle: i.a.oneOfType([s.d, i.a.exact({
+            rectStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyAreaClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            pattern: s.i,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            pattern: l.i,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -1925,74 +1925,74 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 50))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             binField: i.a.string.isRequired,
             stackField: i.a.string,
             binWidth: i.a.number,
             binNumber: i.a.number,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            columnStyle: i.a.oneOfType([s.d, i.a.exact({
+            columnStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyAreaClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            pattern: s.i,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            pattern: l.i,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -2007,76 +2007,76 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 51))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.oneOfType([i.a.arrayOf(i.a.string), i.a.string]).isRequired,
             groupField: i.a.string,
             outliersField: i.a.string,
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            boxStyle: i.a.oneOfType([s.d, i.a.exact({
+            boxStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
-            outliersStyle: i.a.oneOfType([s.d, i.a.exact({
+            outliersStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyBoxClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -2091,129 +2091,133 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return Promise.all([n.e(0), n.e(1)]).then(n.bind(null, 52))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.object.isRequired,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             nodeCfg: i.a.exact({
                 type: i.a.oneOf(["indicator-card"]),
                 size: i.a.arrayOf(i.a.number),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })]),
                 label: i.a.exact({
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })])
                 }),
                 anchorPoints: i.a.arrayOf(i.a.arrayOf(i.a.number)),
                 title: i.a.exact({
-                    containerStyle: s.d,
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    containerStyle: l.d,
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })]),
                     autoEllipsis: i.a.bool
                 }),
                 items: i.a.exact({
-                    containerStyle: s.d,
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    containerStyle: l.d,
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })]),
                     layout: i.a.oneOf(["bundled", "flex", "follow"]),
                     sort: i.a.bool,
                     padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)])
                 }),
                 padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
                 badge: i.a.exact({
                     position: i.a.oneOf(["left", "top", "right", "bottom"]),
                     size: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })])
                 }),
                 percent: i.a.exact({
                     position: i.a.oneOf(["top", "bottom"]),
                     size: i.a.number,
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })]),
-                    backgroundStyle: s.d
+                    backgroundStyle: l.d
                 }),
                 autoWidth: i.a.bool,
-                nodeStateStyles: i.a.oneOfType([i.a.objectOf(s.d), i.a.bool])
+                nodeStateStyles: i.a.oneOfType([i.a.objectOf(l.d), i.a.bool])
             }),
             edgeCfg: i.a.exact({
                 type: i.a.oneOf(["line", "polyline", "arc", "quadratic", "cubic", "cubic-vertical", "cubic-horizontal", "loop"]),
                 label: i.a.exact({
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })])
                 }),
                 startArrow: i.a.exact({
                     type: i.a.oneOf(["vee", "triangle"]),
                     d: i.a.number,
                     path: i.a.string,
                     stroke: i.a.string,
                     fill: i.a.string
                 }),
                 endArrow: i.a.exact({
                     fill: i.a.string,
                     show: i.a.bool
                 }),
-                edgeStateStyles: i.a.oneOfType([i.a.objectOf(s.d), i.a.bool]),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                edgeStateStyles: i.a.oneOfType([i.a.objectOf(l.d), i.a.bool]),
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })])
             }),
             level: i.a.number,
-            behaviors: i.a.arrayOf(i.a.oneOf(["drag-canvas", "scroll-canvas", "zoom-canvas", "drag-node"])),
+            behaviors: i.a.arrayOf(i.a.oneOf(["drag-canvas", "scroll-canvas", "zoom-canvas", "drag-node", "click-select"])),
             markerCfg: i.a.oneOfType([i.a.exact({
                 show: i.a.bool,
                 collapsed: i.a.bool,
                 position: i.a.oneOf(["left", "right", "top", "bottom"]),
-                style: s.d
+                style: l.d
             }), i.a.exact({
                 func: i.a.string
             })]),
             animate: i.a.bool,
             minimapCfg: i.a.exact({
                 show: i.a.bool,
                 viewportClassName: i.a.string,
                 type: i.a.oneOf(["default", "keyShape", "delegate"]),
                 size: i.a.arrayOf(i.a.number),
-                delegateStyle: s.d,
+                delegateStyle: l.d,
                 refresh: i.a.bool,
                 padding: i.a.number
             }),
             layout: i.a.exact({
                 direction: i.a.oneOf(["TB", "BT", "LR", "RL"]),
                 type: i.a.oneOf(["indented"]),
                 dropCap: i.a.bool,
                 indent: i.a.number
             }),
+            recentlyNodeClickRecord: i.a.exact({
+                timestamp: i.a.number,
+                data: i.a.object
+            }),
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {}, (e.a = t).propTypes),
@@ -2225,125 +2229,129 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return Promise.all([n.e(0), n.e(1)]).then(n.bind(null, 53))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.object.isRequired,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             nodeCfg: i.a.exact({
                 type: i.a.oneOf(["fund-card"]),
                 size: i.a.arrayOf(i.a.number),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })]),
                 label: i.a.exact({
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })])
                 }),
                 anchorPoints: i.a.arrayOf(i.a.arrayOf(i.a.number)),
                 title: i.a.exact({
-                    containerStyle: s.d,
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    containerStyle: l.d,
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })]),
                     autoEllipsis: i.a.bool
                 }),
                 items: i.a.exact({
-                    containerStyle: s.d,
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    containerStyle: l.d,
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })]),
                     layout: i.a.oneOf(["bundled", "flex", "follow"]),
                     sort: i.a.bool,
                     padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)])
                 }),
                 padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
                 badge: i.a.exact({
                     position: i.a.oneOf(["left", "top", "right", "bottom"]),
                     size: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })])
                 }),
                 percent: i.a.exact({
                     position: i.a.oneOf(["top", "bottom"]),
                     size: i.a.number,
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })]),
-                    backgroundStyle: s.d
+                    backgroundStyle: l.d
                 }),
                 autoWidth: i.a.bool,
-                nodeStateStyles: i.a.oneOfType([i.a.objectOf(s.d), i.a.bool])
+                nodeStateStyles: i.a.oneOfType([i.a.objectOf(l.d), i.a.bool])
             }),
             edgeCfg: i.a.exact({
                 type: i.a.oneOf(["line", "polyline", "arc", "quadratic", "cubic", "cubic-vertical", "cubic-horizontal", "loop"]),
                 label: i.a.exact({
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })])
                 }),
                 startArrow: i.a.exact({
                     type: i.a.oneOf(["vee", "triangle"]),
                     d: i.a.number,
                     path: i.a.string,
                     stroke: i.a.string,
                     fill: i.a.string
                 }),
                 endArrow: i.a.exact({
                     fill: i.a.string,
                     show: i.a.bool
                 }),
-                edgeStateStyles: i.a.oneOfType([i.a.objectOf(s.d), i.a.bool]),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                edgeStateStyles: i.a.oneOfType([i.a.objectOf(l.d), i.a.bool]),
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })])
             }),
             behaviors: i.a.arrayOf(i.a.oneOf(["drag-canvas", "scroll-canvas", "zoom-canvas", "drag-node"])),
             markerCfg: i.a.oneOfType([i.a.exact({
                 show: i.a.bool,
                 collapsed: i.a.bool,
                 position: i.a.oneOf(["left", "right", "top", "bottom"]),
-                style: s.d
+                style: l.d
             }), i.a.exact({
                 func: i.a.string
             })]),
             minimapCfg: i.a.exact({
                 show: i.a.bool,
                 viewportClassName: i.a.string,
                 type: i.a.oneOf(["default", "keyShape", "delegate"]),
                 size: i.a.arrayOf(i.a.number),
-                delegateStyle: s.d,
+                delegateStyle: l.d,
                 refresh: i.a.bool,
                 padding: i.a.number
             }),
             layout: i.a.exact({
                 nodesep: i.a.number,
                 ranksep: i.a.number
             }),
+            recentlyNodeClickRecord: i.a.exact({
+                timestamp: i.a.number,
+                data: i.a.object
+            }),
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {}, (e.a = t).propTypes),
@@ -2355,81 +2363,81 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 54))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.string.isRequired,
             compareField: i.a.string,
             seriesField: i.a.string,
             isTransposed: i.a.bool,
             shape: i.a.oneOf(["funnel", "pyramid"]),
             dynamicHeight: i.a.bool,
             maxSize: i.a.number,
             minSize: i.a.number,
-            funnelStyle: i.a.oneOfType([s.d, i.a.exact({
+            funnelStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             conversionTag: i.a.oneOfType([i.a.bool, i.a.exact({
                 offsetX: i.a.number,
                 offsetY: i.a.number,
-                style: s.d,
+                style: l.d,
                 formatter: i.a.exact({
                     func: i.a.string
                 })
             })]),
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyAreaClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -2444,96 +2452,96 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 56))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.arrayOf(i.a.object)).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.arrayOf(i.a.string).isRequired,
             geometryOptions: i.a.arrayOf(i.a.oneOfType([i.a.exact({
                 geometry: i.a.oneOf(["line", "column"]),
                 seriesField: i.a.string,
                 smooth: i.a.bool,
                 connectNulls: i.a.bool,
-                lineStyle: i.a.oneOfType([s.d, i.a.exact({
+                lineStyle: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })]),
                 point: i.a.exact({
                     color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                         func: i.a.string
                     })]),
                     shape: i.a.oneOfType([i.a.string, i.a.exact({
                         func: i.a.string
                     })]),
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })])
                 }),
-                label: s.f,
+                label: l.f,
                 color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                     func: i.a.string
                 })])
             }), i.a.exact({
                 geometry: i.a.oneOf(["line", "column"]),
                 seriesField: i.a.string,
                 groupField: i.a.string,
                 isGroup: i.a.bool,
                 isStack: i.a.bool,
                 columnWidthRatio: i.a.number,
                 marginRatio: i.a.number,
-                columnStyle: i.a.oneOfType([s.d, i.a.exact({
+                columnStyle: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })]),
-                label: s.f,
+                label: l.f,
                 color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                     func: i.a.string
                 })])
             })])),
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            tooltip: s.n,
-            xAxis: s.c,
-            yAxis: i.a.objectOf(s.c),
-            annotations: i.a.objectOf(s.b),
-            legend: s.g,
-            slider: s.k,
-            animation: s.a,
+            tooltip: l.n,
+            xAxis: l.c,
+            yAxis: i.a.objectOf(l.c),
+            annotations: i.a.objectOf(l.b),
+            legend: l.g,
+            slider: l.k,
+            animation: l.a,
             recentlyClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -2548,22 +2556,22 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 57))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
@@ -2574,15 +2582,15 @@
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            liquidStyle: i.a.oneOfType([s.d, i.a.exact({
+            liquidStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             shape: i.a.oneOf(["circle", "diamond", "triangle", "pin", "rect"]),
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
             outline: i.a.exact({
@@ -2621,20 +2629,20 @@
                         func: i.a.string
                     }),
                     rotate: i.a.number,
                     offsetX: i.a.number,
                     offsetY: i.a.number
                 })])
             })]),
-            animation: s.a,
+            animation: l.a,
             downloadTrigger: i.a.string,
-            theme: s.m,
-            pattern: s.i,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            pattern: l.i,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -2651,37 +2659,37 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 58))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             measureField: i.a.string.isRequired,
             rangeField: i.a.string.isRequired,
             targetField: i.a.string.isRequired,
             xField: i.a.string,
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
@@ -2701,36 +2709,36 @@
                     func: i.a.string
                 })]),
                 target: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.exact({
                     func: i.a.string
                 })])
             }),
             bulletStyle: i.a.exact({
-                range: i.a.oneOfType([s.d, i.a.exact({
+                range: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })]),
-                measure: i.a.oneOfType([s.d, i.a.exact({
+                measure: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })]),
-                target: i.a.oneOfType([s.d, i.a.exact({
+                target: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })])
             }),
             label: i.a.exact({
-                range: s.f,
-                measure: s.f,
-                target: s.f
-            }),
-            tooltip: s.n,
-            legend: s.g,
-            animation: s.a,
-            downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+                range: l.f,
+                measure: l.f,
+                target: l.f
+            }),
+            tooltip: l.n,
+            legend: l.g,
+            animation: l.a,
+            downloadTrigger: i.a.string,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -2746,22 +2754,22 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 59))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
@@ -2785,24 +2793,24 @@
                 width: i.a.number
             }),
             type: i.a.oneOf(["meter"]),
             meter: i.a.exact({
                 steps: i.a.number,
                 stepRatio: i.a.number
             }),
-            gaugeStyle: i.a.oneOfType([s.d, i.a.exact({
+            gaugeStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
-            axis: s.c,
+            axis: l.c,
             indicator: i.a.exact({
                 pointer: i.a.exact({
-                    style: s.d
+                    style: l.d
                 }),
                 pin: i.a.exact({
-                    style: s.d
+                    style: l.d
                 }),
                 shape: i.a.oneOf(["default", "cursor", "ring-cursor", "simple"])
             }),
             statistic: i.a.oneOfType([i.a.bool, i.a.exact({
                 title: i.a.oneOfType([i.a.bool, i.a.exact({
                     style: i.a.object,
                     content: i.a.string,
@@ -2825,21 +2833,21 @@
                     customHtml: i.a.exact({
                         func: i.a.string
                     }),
                     rotate: i.a.number,
                     offsetX: i.a.number,
                     offsetY: i.a.number
                 })]),
-                style: s.d
+                style: l.d
             })]),
-            animation: s.a,
+            animation: l.a,
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -2855,69 +2863,69 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 60))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.arrayOf(i.a.string).isRequired,
             layout: i.a.oneOf(["horizontal", "vertical"]),
-            barStyle: i.a.oneOfType([s.d, i.a.exact({
+            barStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyBarClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -2932,31 +2940,31 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 61))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.string.isRequired,
             colorField: i.a.string,
             sizeField: i.a.string,
             reflect: i.a.oneOf(["x", "y"]),
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
@@ -2968,46 +2976,46 @@
                     startAngle: i.a.number,
                     endAngle: i.a.number,
                     radius: i.a.number,
                     innerRadius: i.a.number
                 })
             }),
             sizeRatio: i.a.number,
-            heatmapStyle: i.a.oneOfType([s.d, i.a.exact({
+            heatmapStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            pattern: s.i,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            pattern: l.i,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyGridClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -3022,65 +3030,65 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 62))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.number).isRequired,
-            meta: s.h,
+            meta: l.h,
             smooth: i.a.bool,
             color: i.a.string,
-            areaStyle: s.d,
+            areaStyle: l.d,
             line: i.a.exact({
                 color: i.a.string,
-                style: s.d
+                style: l.d
             }),
             point: i.a.exact({
                 color: i.a.string,
-                style: s.d
+                style: l.d
             }),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.oneOf(["auto"])]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number)]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            tooltip: s.n,
-            annotations: s.b,
-            pattern: s.i,
-            animation: s.a,
+            tooltip: l.n,
+            annotations: l.b,
+            pattern: l.i,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -3095,31 +3103,31 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 63))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.string.isRequired,
             colorField: i.a.string,
             isStack: i.a.bool,
             isGroup: i.a.bool,
             radius: i.a.number,
             innerRadius: i.a.number,
@@ -3127,56 +3135,56 @@
             endAngle: i.a.number,
             maxAngle: i.a.number,
             type: i.a.oneOf(["line"]),
             intervalPadding: i.a.number,
             dodgePadding: i.a.number,
             minBarWidth: i.a.number,
             maxBarWidth: i.a.number,
-            barStyle: i.a.oneOfType([s.d, i.a.exact({
+            barStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             barBackground: i.a.exact({
-                style: s.d
+                style: l.d
             }),
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyBarClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            pattern: s.i,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            pattern: l.i,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -3191,73 +3199,73 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 64))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             xField: i.a.string.isRequired,
             yField: i.a.string.isRequired,
             seriesField: i.a.string,
             box: i.a.bool,
             shape: i.a.oneOf(["smooth", "hollow", "hollow-smooth"]),
-            violinStyle: i.a.oneOfType([s.d, i.a.exact({
+            violinStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
-            xAxis: s.c,
-            yAxis: s.c,
+            xAxis: l.c,
+            yAxis: l.c,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            tooltip: s.n,
-            annotations: s.b,
-            animation: s.a,
+            legend: l.g,
+            tooltip: l.n,
+            annotations: l.b,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyViolinClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -3272,69 +3280,69 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return n.e(0).then(n.bind(null, 65))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.arrayOf(i.a.object).isRequired,
-            meta: s.h,
+            meta: l.h,
             setsField: i.a.string,
             sizeField: i.a.string,
             blendMode: i.a.oneOf(["multiply", "normal", "darken", "lighten", "screen", "overlay", "burn", "dodge"]),
-            pointStyle: i.a.oneOfType([s.d, i.a.exact({
+            pointStyle: i.a.oneOfType([l.d, i.a.exact({
                 func: i.a.string
             })]),
             color: i.a.oneOfType([i.a.string, i.a.arrayOf(i.a.string), i.a.exact({
                 func: i.a.string
             })]),
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             padding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             appendPadding: i.a.oneOfType([i.a.number, i.a.arrayOf(i.a.number), i.a.string]),
             renderer: i.a.oneOf(["canvas", "svg"]),
             pixelRatio: i.a.number,
             locale: i.a.oneOf(["zh-CN", "en-US"]),
             limitInPlot: i.a.bool,
-            legend: s.g,
-            label: s.f,
-            tooltip: s.n,
-            animation: s.a,
+            legend: l.g,
+            label: l.f,
+            tooltip: l.n,
+            animation: l.a,
             recentlyTooltipChangeRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.arrayOf(i.a.object)
             }),
             recentlyCircleClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
             recentlyLegendInfo: i.a.exact({
                 triggerItemName: i.a.any,
                 items: i.a.arrayOf(i.a.object)
             }),
             downloadTrigger: i.a.string,
-            theme: s.m,
-            interactions: s.e,
-            state: s.l,
+            theme: l.m,
+            interactions: l.e,
+            state: l.l,
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -3349,53 +3357,53 @@
     }), n.d(e, "b", function() {
         return u
     });
 
     function t(a) {
         return o.a.createElement(r.Suspense, {
             fallback: null
-        }, o.a.createElement(l, a))
+        }, o.a.createElement(s, a))
     }
     var r = n(2),
         o = n.n(r),
         i = n(0),
         i = n.n(i),
-        s = n(1),
-        l = o.a.lazy(function() {
+        l = n(1),
+        s = o.a.lazy(function() {
             return Promise.all([n.e(0), n.e(1)]).then(n.bind(null, 66))
         }),
         c = (t.propTypes = {
             id: i.a.string,
             key: i.a.string,
             className: i.a.string,
             style: i.a.object,
             data: i.a.object.isRequired,
             width: i.a.number,
             height: i.a.number,
             autoFit: i.a.bool,
             nodeCfg: i.a.exact({
                 type: i.a.oneOf(["icon-node", "card", "circle", "rect", "ellipse", "diamond", "triangle", "star", "image", "modelRect", "donut"]),
                 size: i.a.arrayOf(i.a.number),
-                style: i.a.oneOfType([s.d, i.a.exact({
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })]),
                 label: i.a.exact({
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })])
                 }),
-                nodeStateStyles: i.a.objectOf(s.d)
+                nodeStateStyles: i.a.objectOf(l.d)
             }),
             edgeCfg: i.a.exact({
-                style: i.a.oneOfType([s.d, i.a.exact({
+                style: i.a.oneOfType([l.d, i.a.exact({
                     func: i.a.string
                 })]),
                 type: i.a.oneOf(["line", "polyline", "arc", "quadratic", "cubic", "cubic-vertical", "cubic-horizontal", "loop"]),
                 label: i.a.exact({
-                    style: i.a.oneOfType([s.d, i.a.exact({
+                    style: i.a.oneOfType([l.d, i.a.exact({
                         func: i.a.string
                     })])
                 }),
                 startArrow: i.a.exact({
                     type: i.a.oneOf(["vee", "triangle"]),
                     size: i.a.number,
                     d: i.a.number,
@@ -3407,36 +3415,52 @@
                     type: i.a.oneOf(["vee", "triangle"]),
                     size: i.a.number,
                     d: i.a.number,
                     path: i.a.string,
                     stroke: i.a.string,
                     fill: i.a.string
                 }),
-                edgeStateStyles: i.a.objectOf(s.d)
+                edgeStateStyles: i.a.objectOf(l.d)
             }),
-            behaviors: i.a.arrayOf(i.a.oneOf(["drag-canvas", "scroll-canvas", "zoom-canvas", "drag-node"])),
+            behaviors: i.a.arrayOf(i.a.oneOf(["drag-canvas", "scroll-canvas", "zoom-canvas", "drag-node", "click-select"])),
             animate: i.a.bool,
             minimapCfg: i.a.exact({
                 show: i.a.bool,
                 viewportClassName: i.a.string,
                 type: i.a.oneOf(["default", "keyShape", "delegate"]),
                 size: i.a.arrayOf(i.a.number),
-                delegateStyle: s.d,
+                delegateStyle: l.d,
                 refresh: i.a.bool,
                 padding: i.a.number
             }),
             layout: i.a.exact({
                 direction: i.a.oneOf(["TB", "BT", "LR", "RL"]),
                 nodesep: i.a.number,
                 ranksep: i.a.number
             }),
             recentlyNodeClickRecord: i.a.exact({
                 timestamp: i.a.number,
                 data: i.a.object
             }),
+            recentlyNodeDoubleClickRecord: i.a.exact({
+                timestamp: i.a.number,
+                data: i.a.object
+            }),
+            recentlyEdgeClickRecord: i.a.exact({
+                timestamp: i.a.number,
+                data: i.a.object
+            }),
+            recentlyEdgeDoubleClickRecord: i.a.exact({
+                timestamp: i.a.number,
+                data: i.a.object
+            }),
+            selectedNodes: i.a.exact({
+                timestamp: i.a.number,
+                data: i.a.array
+            }),
             loading_state: i.a.shape({
                 is_loading: i.a.bool,
                 prop_name: i.a.string,
                 component_name: i.a.string
             }),
             setProps: i.a.func
         }, t.defaultProps = {
@@ -3446,17 +3470,17 @@
         }, (e.a = t).propTypes),
         u = t.defaultProps
 }, function(E, a, e) {
     "use strict";
     e.r(a), e.d(a, "AntdLine", function() {
         return i.a
     }), e.d(a, "AntdArea", function() {
-        return s.a
-    }), e.d(a, "AntdBar", function() {
         return l.a
+    }), e.d(a, "AntdBar", function() {
+        return s.a
     }), e.d(a, "AntdColumn", function() {
         return c.a
     }), e.d(a, "AntdPie", function() {
         return u.a
     }), e.d(a, "AntdScatter", function() {
         return d.a
     }), e.d(a, "AntdStock", function() {
@@ -3484,19 +3508,19 @@
     }), e.d(a, "AntdFundFlow", function() {
         return P.a
     }), e.d(a, "AntdFunnel", function() {
         return R.a
     }), e.d(a, "AntdTinyLine", function() {
         return v.a
     }), e.d(a, "AntdDualAxes", function() {
-        return S.a
-    }), e.d(a, "AntdLiquid", function() {
         return j.a
-    }), e.d(a, "AntdBullet", function() {
+    }), e.d(a, "AntdLiquid", function() {
         return k.a
+    }), e.d(a, "AntdBullet", function() {
+        return S.a
     }), e.d(a, "AntdGauge", function() {
         return C.a
     }), e.d(a, "AntdBidirectionalBar", function() {
         return _.a
     }), e.d(a, "AntdHeatmap", function() {
         return z.a
     }), e.d(a, "AntdTinyArea", function() {
@@ -3508,19 +3532,19 @@
     }), e.d(a, "AntdRingProgress", function() {
         return H
     }), e.d(a, "AntdWaterfall", function() {
         return Y
     }), e.d(a, "AntdRadialBar", function() {
         return M.a
     }), e.d(a, "AntdViolin", function() {
-        return G.a
+        return D.a
     }), e.d(a, "AntdVenn", function() {
-        return V.a
+        return G.a
     }), e.d(a, "AntdRadialTree", function() {
-        return D.a
+        return V.a
     });
 
     function n(a) {
         return A.a.createElement(F.Suspense, {
             fallback: null
         }, A.a.createElement(I, a))
     }
@@ -3539,16 +3563,16 @@
 
     function o(a) {
         return A.a.createElement(F.Suspense, {
             fallback: null
         }, A.a.createElement(X, a))
     }
     var i = e(5),
-        s = e(6),
-        l = e(7),
+        l = e(6),
+        s = e(7),
         c = e(4),
         u = e(8),
         d = e(9),
         g = e(10),
         f = e(11),
         m = e(12),
         p = e(13),
@@ -3558,17 +3582,17 @@
         h = e(17),
         x = e(18),
         T = e(19),
         w = e(20),
         P = e(21),
         R = e(22),
         v = e(3),
-        S = e(23),
-        j = e(24),
-        k = e(25),
+        j = e(23),
+        k = e(24),
+        S = e(25),
         C = e(26),
         _ = e(27),
         z = e(28),
         N = e(29),
         F = e(2),
         A = e.n(F),
         a = e(0),
@@ -3796,13 +3820,13 @@
             }),
             setProps: a.a.func
         }, o),
         M = (o.defaultProps = {
             locale: "zh-CN",
             downloadTrigger: "download-trigger"
         }, e(30)),
-        G = e(31),
-        V = e(32),
-        D = e(33)
+        D = e(31),
+        G = e(32),
+        V = e(33)
 }, function(a, e) {
     a.exports = window.ReactDOM
 }]);
```

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/metadata.json` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994553580066896%*

 * *Differences: {"'src/lib/components/graphs/AntdDecompositionTree.react.js'": "{'props': {'behaviors': {'type': "*

 * *                                                               "{'value': {'value': {insert: [(4, "*

 * *                                                               "OrderedDict([('value', "*

 * *                                                               '"\'click-select\'"), '*

 * *                                                               "('computed', False)]))]}}}}, "*

 * *                                           […]*

```diff
@@ -15438,14 +15438,18 @@
                             {
                                 "computed": false,
                                 "value": "'zoom-canvas'"
                             },
                             {
                                 "computed": false,
                                 "value": "'drag-node'"
+                            },
+                            {
+                                "computed": false,
+                                "value": "'click-select'"
                             }
                         ]
                     }
                 }
             },
             "className": {
                 "description": "",
@@ -16154,14 +16158,33 @@
                                     "value": "'indicator-card'"
                                 }
                             ]
                         }
                     }
                 }
             },
+            "recentlyNodeClickRecord": {
+                "description": "\u8282\u70b9\u70b9\u51fb\u4e8b\u4ef6\u76d1\u542c",
+                "required": false,
+                "type": {
+                    "name": "exact",
+                    "value": {
+                        "data": {
+                            "description": "\u4e8b\u4ef6\u5bf9\u5e94\u8282\u70b9\u4fe1\u606f\uff0c\u70b9\u51fb\u7a7a\u767d\u5904\u65f6\u4e3a\u7a7a",
+                            "name": "object",
+                            "required": false
+                        },
+                        "timestamp": {
+                            "description": "\u4e8b\u4ef6\u89e6\u53d1\u65f6\u95f4\u6233",
+                            "name": "number",
+                            "required": false
+                        }
+                    }
+                }
+            },
             "setProps": {
                 "description": "Dash-assigned callback that should be called to report property changes\r\nto Dash, to make them available for callbacks.",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
@@ -16889,14 +16912,33 @@
                                     "value": "'fund-card'"
                                 }
                             ]
                         }
                     }
                 }
             },
+            "recentlyNodeClickRecord": {
+                "description": "\u8282\u70b9\u70b9\u51fb\u4e8b\u4ef6\u76d1\u542c",
+                "required": false,
+                "type": {
+                    "name": "exact",
+                    "value": {
+                        "data": {
+                            "description": "\u4e8b\u4ef6\u5bf9\u5e94\u8282\u70b9\u4fe1\u606f\uff0c\u70b9\u51fb\u7a7a\u767d\u5904\u65f6\u4e3a\u7a7a",
+                            "name": "object",
+                            "required": false
+                        },
+                        "timestamp": {
+                            "description": "\u4e8b\u4ef6\u89e6\u53d1\u65f6\u95f4\u6233",
+                            "name": "number",
+                            "required": false
+                        }
+                    }
+                }
+            },
             "setProps": {
                 "description": "Dash-assigned callback that should be called to report property changes\r\nto Dash, to make them available for callbacks.",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
@@ -16944,15 +16986,15 @@
                 }
             },
             "behaviors": {
                 "defaultValue": {
                     "computed": false,
                     "value": "['drag-canvas', 'zoom-canvas']"
                 },
-                "description": "\u542f\u7528\u7684\u4ea4\u4e92\u6a21\u5f0f\uff0c\u53ef\u9009\u9879\u6709`'drag-canvas'`\uff08\u62d6\u62fd\u753b\u5e03\uff09\u3001`'scroll-canvas'`\uff08\u6eda\u8f6e\u6eda\u52a8\u753b\u5e03\uff09\u3001\r\n`'zoom-canvas'`\uff08\u7f29\u653e\u753b\u5e03\uff09\u3001`'drag-node'`\uff08\u62d6\u62fd\u8282\u70b9\uff09\r\n\u9ed8\u8ba4\u503c\uff1a`['drag-canvas', 'zoom-canvas']`",
+                "description": "\u542f\u7528\u7684\u4ea4\u4e92\u6a21\u5f0f\uff0c\u53ef\u9009\u9879\u6709`'drag-canvas'`\uff08\u62d6\u62fd\u753b\u5e03\uff09\u3001`'scroll-canvas'`\uff08\u6eda\u8f6e\u6eda\u52a8\u753b\u5e03\uff09\u3001\r\n`'zoom-canvas'`\uff08\u7f29\u653e\u753b\u5e03\uff09\u3001`'drag-node'`\uff08\u62d6\u62fd\u8282\u70b9\uff09\u3001'click-select'\uff08\u8282\u70b9\u9009\u62e9\uff09\r\n\u9ed8\u8ba4\u503c\uff1a`['drag-canvas', 'zoom-canvas']`",
                 "required": false,
                 "type": {
                     "name": "arrayOf",
                     "value": {
                         "name": "enum",
                         "value": [
                             {
@@ -16966,14 +17008,18 @@
                             {
                                 "computed": false,
                                 "value": "'zoom-canvas'"
                             },
                             {
                                 "computed": false,
                                 "value": "'drag-node'"
+                            },
+                            {
+                                "computed": false,
+                                "value": "'click-select'"
                             }
                         ]
                     }
                 }
             },
             "className": {
                 "description": "css\u7c7b\u540d",
@@ -17456,14 +17502,52 @@
                                     "value": "'donut'"
                                 }
                             ]
                         }
                     }
                 }
             },
+            "recentlyEdgeClickRecord": {
+                "description": "\u8fb9\u70b9\u51fb\u4e8b\u4ef6\u76d1\u542c",
+                "required": false,
+                "type": {
+                    "name": "exact",
+                    "value": {
+                        "data": {
+                            "description": "\u4e8b\u4ef6\u5bf9\u5e94\u8282\u70b9\u4fe1\u606f\uff0c\u70b9\u51fb\u7a7a\u767d\u5904\u65f6\u4e3a\u7a7a",
+                            "name": "object",
+                            "required": false
+                        },
+                        "timestamp": {
+                            "description": "\u4e8b\u4ef6\u89e6\u53d1\u65f6\u95f4\u6233",
+                            "name": "number",
+                            "required": false
+                        }
+                    }
+                }
+            },
+            "recentlyEdgeDoubleClickRecord": {
+                "description": "\u8fb9\u53cc\u51fb\u4e8b\u4ef6\u76d1\u542c",
+                "required": false,
+                "type": {
+                    "name": "exact",
+                    "value": {
+                        "data": {
+                            "description": "\u4e8b\u4ef6\u5bf9\u5e94\u8282\u70b9\u4fe1\u606f\uff0c\u70b9\u51fb\u7a7a\u767d\u5904\u65f6\u4e3a\u7a7a",
+                            "name": "object",
+                            "required": false
+                        },
+                        "timestamp": {
+                            "description": "\u4e8b\u4ef6\u89e6\u53d1\u65f6\u95f4\u6233",
+                            "name": "number",
+                            "required": false
+                        }
+                    }
+                }
+            },
             "recentlyNodeClickRecord": {
                 "description": "\u8282\u70b9\u70b9\u51fb\u4e8b\u4ef6\u76d1\u542c",
                 "required": false,
                 "type": {
                     "name": "exact",
                     "value": {
                         "data": {
@@ -17472,14 +17556,52 @@
                             "required": false
                         },
                         "timestamp": {
                             "description": "\u4e8b\u4ef6\u89e6\u53d1\u65f6\u95f4\u6233",
                             "name": "number",
                             "required": false
                         }
+                    }
+                }
+            },
+            "recentlyNodeDoubleClickRecord": {
+                "description": "\u8282\u70b9\u53cc\u51fb\u4e8b\u4ef6\u76d1\u542c",
+                "required": false,
+                "type": {
+                    "name": "exact",
+                    "value": {
+                        "data": {
+                            "description": "\u4e8b\u4ef6\u5bf9\u5e94\u8282\u70b9\u4fe1\u606f\uff0c\u70b9\u51fb\u7a7a\u767d\u5904\u65f6\u4e3a\u7a7a",
+                            "name": "object",
+                            "required": false
+                        },
+                        "timestamp": {
+                            "description": "\u4e8b\u4ef6\u89e6\u53d1\u65f6\u95f4\u6233",
+                            "name": "number",
+                            "required": false
+                        }
+                    }
+                }
+            },
+            "selectedNodes": {
+                "description": "\u8282\u70b9\u9009\u4e2d\u4e8b\u4ef6\u76d1\u542c\uff0c\u9700\u8981\u5728``behaviors``\u4e2d\u5f00\u542f``click-select``",
+                "required": false,
+                "type": {
+                    "name": "exact",
+                    "value": {
+                        "data": {
+                            "description": "\u5bf9\u5e94\u9009\u4e2d\u7684\u8282\u70b9\u4fe1\u606f\u6570\u7ec4",
+                            "name": "array",
+                            "required": false
+                        },
+                        "timestamp": {
+                            "description": "\u4e8b\u4ef6\u89e6\u53d1\u65f6\u95f4\u6233",
+                            "name": "number",
+                            "required": false
+                        }
                     }
                 }
             },
             "setProps": {
                 "description": "Dash-assigned callback that should be called to report property changes\r\nto Dash, to make them available for callbacks.",
                 "required": false,
                 "type": {
```

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts/package-info.json` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts/package-info.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809524%*

 * *Differences: {"'dependencies'": "{'@antv/graphin': '^2.7.27'}", "'version'": "'0.1.0-rc1'"}*

```diff
@@ -10,14 +10,15 @@
         ]
     },
     "bugs": {
         "url": "https://github.com/CNFeffery/feffery-antd-charts/issues"
     },
     "dependencies": {
         "@ant-design/charts": "^1.4.2",
+        "@antv/graphin": "^2.7.27",
         "lodash": "^4.17.21"
     },
     "description": "Best implementation of Ant Design Charts in Plotly Dash.",
     "devDependencies": {
         "@babel/core": "^7.5.4",
         "@babel/plugin-proposal-object-rest-spread": "^7.5.4",
         "@babel/preset-env": "^7.5.4",
@@ -60,9 +61,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_charts -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.1.0-rc0"
+    "version": "0.1.0-rc1"
 }
```

### Comparing `feffery_antd_charts-0.1.0rc0/feffery_antd_charts.egg-info/SOURCES.txt` & `feffery_antd_charts-0.1.0rc1/feffery_antd_charts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feffery_antd_charts-0.1.0rc0/package.json` & `feffery_antd_charts-0.1.0rc1/package.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809524%*

 * *Differences: {"'dependencies'": "{'@antv/graphin': '^2.7.27'}", "'version'": "'0.1.0-rc1'"}*

```diff
@@ -10,14 +10,15 @@
         ]
     },
     "bugs": {
         "url": "https://github.com/CNFeffery/feffery-antd-charts/issues"
     },
     "dependencies": {
         "@ant-design/charts": "^1.4.2",
+        "@antv/graphin": "^2.7.27",
         "lodash": "^4.17.21"
     },
     "description": "Best implementation of Ant Design Charts in Plotly Dash.",
     "devDependencies": {
         "@babel/core": "^7.5.4",
         "@babel/plugin-proposal-object-rest-spread": "^7.5.4",
         "@babel/preset-env": "^7.5.4",
@@ -60,9 +61,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_antd_charts -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.1.0-rc0"
+    "version": "0.1.0-rc1"
 }
```

### Comparing `feffery_antd_charts-0.1.0rc0/setup.py` & `feffery_antd_charts-0.1.0rc1/setup.py`

 * *Files identical despite different names*

