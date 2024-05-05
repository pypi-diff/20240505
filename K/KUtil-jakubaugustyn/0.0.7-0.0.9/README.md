# Comparing `tmp/kutil_jakubaugustyn-0.0.7.tar.gz` & `tmp/KUtil_jakubaugustyn-0.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kutil_jakubaugustyn-0.0.7.tar", last modified: Fri Apr 26 15:29:36 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

