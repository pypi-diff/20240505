# Comparing `tmp/meds_etl_cpp-0.1.2.tar.gz` & `tmp/meds_etl_cpp-0.2.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meds_etl_cpp-0.1.2.tar", last modified: Thu Apr 11 16:03:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

