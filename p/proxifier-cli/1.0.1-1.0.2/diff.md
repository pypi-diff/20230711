# Comparing `tmp/proxifier-cli-1.0.1.tar.gz` & `tmp/proxifier_cli-1.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxifier-cli-1.0.1.tar", last modified: Sat Jun 24 20:29:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

