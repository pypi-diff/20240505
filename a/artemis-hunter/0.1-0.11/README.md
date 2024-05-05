# Comparing `tmp/artemis_hunter-0.1.tar.gz` & `tmp/artemis_hunter-0.11-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artemis_hunter-0.1.tar", last modified: Sun May  5 02:29:50 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

