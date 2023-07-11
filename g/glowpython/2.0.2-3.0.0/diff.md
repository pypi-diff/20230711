# Comparing `tmp/glowpython-2.0.2.tar.gz` & `tmp/glowpython-3.0.0-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glowpython-2.0.2.tar", last modified: Thu Mar  2 22:59:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

