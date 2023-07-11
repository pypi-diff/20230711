# Comparing `tmp/metricspace-1.1.1.tar.gz` & `tmp/metricspace-1.2.0-cp37-abi3-manylinux_2_34_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricspace-1.1.1.tar", last modified: Fri Jun  9 19:35:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

