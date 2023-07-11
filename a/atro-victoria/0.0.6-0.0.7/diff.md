# Comparing `tmp/atro_victoria-0.0.6.tar.gz` & `tmp/atro_victoria-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_victoria-0.0.6.tar", max compression
+gzip compressed data, was "atro_victoria-0.0.7.tar", max compression
```

## Comparing `atro_victoria-0.0.6.tar` & `atro_victoria-0.0.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-09 16:47:06.656790 atro_victoria-0.0.6/README.md
--rw-r--r--   0        0        0     1887 2023-07-11 20:47:33.747785 atro_victoria-0.0.6/atro_victoria/__init__.py
--rw-r--r--   0        0        0      409 2023-07-11 20:47:38.201212 atro_victoria-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 atro_victoria-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 16:47:06.656790 atro_victoria-0.0.7/README.md
+-rw-r--r--   0        0        0     1967 2023-07-11 20:51:13.945750 atro_victoria-0.0.7/atro_victoria/__init__.py
+-rw-r--r--   0        0        0      409 2023-07-11 20:50:25.904739 atro_victoria-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 atro_victoria-0.0.7/PKG-INFO
```

### Comparing `atro_victoria-0.0.6/atro_victoria/__init__.py` & `atro_victoria-0.0.7/atro_victoria/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,30 +19,34 @@
   def format(self):
     vals = self.model_dump()
     counter = 0
     output = ""
     vals.pop('url')
     for val in vals:
       counter+=1
-      if val == "timestamp" and vals[val] is not None and isinstance(vals[val], datetime):
-        output += "," + str(counter) + ":time:unix_ms"
+      if val == "timestamp":
+        if vals[val] is not None and isinstance(vals[val], datetime):
+          output += "," + str(counter) + ":time:unix_ms"
         continue
       if isinstance(vals[val], (int, float)):
         output += "," + str(counter) + ":metric:" + val
       else:
         output += "," + str(counter) + ":label:" + val
     if output == "":
       raise Exception("No values to format")
     return output[1:]
 
   def data_as_csv(self):
     vals = self.model_dump()
     vals.pop('url')
     if "timestamp" in vals and vals["timestamp"] is not None and isinstance(vals["timestamp"], datetime):
       vals['timestamp'] = strigify_datetime(vals['timestamp'])
+    else:
+      if "timestamp" in vals:
+        vals.pop('timestamp')
     output = ""
     for val in vals.values():
       
       output += "," + str(val)
     if output == "":
       raise Exception("No values to format")
     return output[1:]
```

