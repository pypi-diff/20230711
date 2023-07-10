# Comparing `tmp/typetest-cli-1.1.0.tar.gz` & `tmp/typetest_cli-1.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetest-cli-1.1.0.tar", last modified: Sat Jul  8 22:23:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

