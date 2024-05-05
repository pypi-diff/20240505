# Comparing `tmp/rns-0.7.3.tar.gz` & `tmp/rns-0.7.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rns-0.7.3.tar", last modified: Sat Mar  9 20:05:15 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

