# Comparing `tmp/Finance-Hermes-0.2.4.tar.gz` & `tmp/Finance_Hermes-0.2.5-py3.7-linux-x86_64.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Hermes-0.2.4.tar", last modified: Sat Jun 24 23:09:05 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

