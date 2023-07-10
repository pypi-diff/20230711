# Comparing `tmp/solocast-0.2.0.tar.gz` & `tmp/solocast-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solocast-0.2.0.tar", max compression
+gzip compressed data, was "solocast-0.2.1.tar", max compression
```

## Comparing `solocast-0.2.0.tar` & `solocast-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1068 2021-12-19 21:57:40.560574 solocast-0.2.0/LICENSE
--rw-r--r--   0        0        0      421 2023-03-22 00:11:53.316067 solocast-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     7540 2023-03-22 00:11:53.316067 solocast-0.2.0/solocast/solocast.py
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 solocast-0.2.0/setup.py
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 solocast-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2021-12-19 21:57:40.560574 solocast-0.2.1/LICENSE
+-rw-r--r--   0        0        0      421 2023-07-10 23:27:13.839838 solocast-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0     7572 2023-07-10 23:22:35.993337 solocast-0.2.1/solocast/solocast.py
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 solocast-0.2.1/PKG-INFO
```

### Comparing `solocast-0.2.0/LICENSE` & `solocast-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solocast-0.2.0/solocast/solocast.py` & `solocast-0.2.1/solocast/solocast.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
         for line in script_file_reader.readlines():
             if not line.strip():
                 add_slug_text(linetext)
                 linetext = ""
 
             else:
                 linetext += f"{line}  \n"
+        add_slug_text(linetext)
 
 
 def load_md():
     linetext = ""
     with open(script_file_name()) as script_file_reader:
         for line in script_file_reader.readlines():
             for markdown_header in MARKDOWN_HEADERS:
```

### Comparing `solocast-0.2.0/PKG-INFO` & `solocast-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solocast
-Version: 0.2.0
+Version: 0.2.1
 Summary: Record audio one segment at a time
 Home-page: https://gitlab.com/norrist/solocast
 License: MIT
 Author: Todd Norris
 Author-email: norrist@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

