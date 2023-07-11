# Comparing `tmp/chatgpt-klient-0.0.3.tar.gz` & `tmp/chatgpt_klient-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-klient-0.0.3.tar", last modified: Mon Jun  5 11:40:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

