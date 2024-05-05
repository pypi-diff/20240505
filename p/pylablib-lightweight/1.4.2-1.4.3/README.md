# Comparing `tmp/pylablib-lightweight-1.4.2.tar.gz` & `tmp/pylablib_lightweight-1.4.3-cp312-cp312-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pylablib-lightweight-1.4.2.tar", last modified: Sun Oct  8 14:01:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

