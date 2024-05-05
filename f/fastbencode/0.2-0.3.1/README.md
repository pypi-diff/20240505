# Comparing `tmp/fastbencode-0.2.tar.gz` & `tmp/fastbencode-0.3.1-pp310-pypy310_pp73-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastbencode-0.2.tar", last modified: Fri Feb 10 17:49:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

