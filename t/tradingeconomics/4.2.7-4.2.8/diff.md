# Comparing `tmp/tradingeconomics-4.2.7.tar.gz` & `tmp/tradingeconomics-4.2.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingeconomics-4.2.7.tar", last modified: Tue Jul  4 10:33:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

