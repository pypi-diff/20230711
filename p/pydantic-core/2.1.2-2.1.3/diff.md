# Comparing `tmp/pydantic_core-2.1.2.tar.gz` & `tmp/pydantic_core-2.1.3-pp37-pypy37_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

