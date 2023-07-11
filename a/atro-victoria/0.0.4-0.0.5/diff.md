# Comparing `tmp/atro_victoria-0.0.4.tar.gz` & `tmp/atro_victoria-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_victoria-0.0.4.tar", max compression
+gzip compressed data, was "atro_victoria-0.0.5.tar", max compression
```

## Comparing `atro_victoria-0.0.4.tar` & `atro_victoria-0.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-09 16:47:06.656790 atro_victoria-0.0.4/README.md
--rw-r--r--   0        0        0     1747 2023-07-11 20:38:12.139342 atro_victoria-0.0.4/atro_victoria/__init__.py
--rw-r--r--   0        0        0      409 2023-07-11 20:38:29.289701 atro_victoria-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 atro_victoria-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 16:47:06.656790 atro_victoria-0.0.5/README.md
+-rw-r--r--   0        0        0     1825 2023-07-11 20:40:44.572529 atro_victoria-0.0.5/atro_victoria/__init__.py
+-rw-r--r--   0        0        0      409 2023-07-11 20:40:47.455923 atro_victoria-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 atro_victoria-0.0.5/PKG-INFO
```

### Comparing `atro_victoria-0.0.4/atro_victoria/__init__.py` & `atro_victoria-0.0.5/atro_victoria/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     if output == "":
       raise Exception("No values to format")
     return output[1:]
 
   def data_as_csv(self):
     vals = self.model_dump()
     vals.pop('url')
-    if "timestamp" in vals:
+    if "timestamp" in vals and vals["timestamp"] is not None and isinstance(vals["timestamp"], datetime):
       vals['timestamp'] = strigify_datetime(vals['timestamp'])
     output = ""
     for val in vals.values():
       
       output += "," + str(val)
     if output == "":
       raise Exception("No values to format")
```

