# Comparing `tmp/pygubu_designer-0.39.1.tar.gz` & `tmp/pygubu_designer-0.39.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygubu_designer-0.39.1.tar", last modified: Mon Apr 22 01:14:39 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

