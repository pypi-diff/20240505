# Comparing `tmp/FlowAnalyzer-0.2.8.tar.gz` & `tmp/FlowAnalyzer-0.2.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowAnalyzer-0.2.8.tar", last modified: Sun Jan  7 07:26:26 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

