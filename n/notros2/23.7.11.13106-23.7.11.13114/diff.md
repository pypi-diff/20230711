# Comparing `tmp/notros2-23.7.11.13106.tar.gz` & `tmp/notros2-23.7.11.13114-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notros2-23.7.11.13106.tar", last modified: Tue Jul 11 01:31:06 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

