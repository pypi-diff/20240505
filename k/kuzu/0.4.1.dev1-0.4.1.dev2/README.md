# Comparing `tmp/kuzu-0.4.1.dev1.tar.gz` & `tmp/kuzu-0.4.1.dev2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.4.1.dev1.tar", last modified: Sat May  4 08:04:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

