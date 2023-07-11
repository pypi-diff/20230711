# Comparing `tmp/notros2-23.7.11.13747.tar.gz` & `tmp/notros2-23.7.11.13756-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notros2-23.7.11.13747.tar", last modified: Tue Jul 11 01:37:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

