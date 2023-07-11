# Comparing `tmp/notros2-23.7.11.94920.tar.gz` & `tmp/notros2-23.7.11.94927-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notros2-23.7.11.94920.tar", last modified: Tue Jul 11 09:49:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

