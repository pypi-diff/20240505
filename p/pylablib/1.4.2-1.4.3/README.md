# Comparing `tmp/pylablib-1.4.2.tar.gz` & `tmp/pylablib-1.4.3-cp312-cp312-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pylablib-1.4.2.tar", last modified: Sun Oct  8 09:11:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

