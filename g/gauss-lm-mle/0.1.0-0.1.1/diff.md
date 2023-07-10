# Comparing `tmp/gauss-lm-mle-0.1.0.tar.gz` & `tmp/gauss_lm_mle-0.1.1-cp310-cp310-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauss-lm-mle-0.1.0.tar", last modified: Mon Jul 10 22:13:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

