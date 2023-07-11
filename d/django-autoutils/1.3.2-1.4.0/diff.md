# Comparing `tmp/django_autoutils-1.3.2.tar.gz` & `tmp/django_autoutils-1.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_autoutils-1.3.2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

