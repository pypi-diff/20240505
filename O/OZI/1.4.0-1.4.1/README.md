# Comparing `tmp/OZI-1.4.0.tar.gz` & `tmp/OZI-1.4.1-cp311-cp311-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.4.0.tar", last modified: Sat May  4 19:07:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

