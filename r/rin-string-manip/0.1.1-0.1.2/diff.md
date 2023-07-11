# Comparing `tmp/rin_string_manip-0.1.1.tar.gz` & `tmp/rin_string_manip-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rin_string_manip-0.1.1.tar", max compression
+gzip compressed data, was "rin_string_manip-0.1.2.tar", max compression
```

## Comparing `rin_string_manip-0.1.1.tar` & `rin_string_manip-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-07-11 09:00:11.252912 rin_string_manip-0.1.1/README.md
--rw-r--r--   0        0        0      413 2023-07-11 09:00:50.756809 rin_string_manip-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 05:56:34.768991 rin_string_manip-0.1.1/rin_string_manip/__init__.py
--rw-r--r--   0        0        0      102 2023-07-11 08:26:33.403502 rin_string_manip-0.1.1/rin_string_manip/config.yaml
--rw-r--r--   0        0        0      747 2023-07-11 07:39:54.547307 rin_string_manip-0.1.1/rin_string_manip/log_error.py
--rw-r--r--   0        0        0      378 2023-07-11 07:21:26.032932 rin_string_manip-0.1.1/rin_string_manip/logging.yaml
--rw-r--r--   0        0        0     1071 2023-07-11 08:32:40.767598 rin_string_manip-0.1.1/rin_string_manip/main.py
--rw-r--r--   0        0        0      556 2023-07-11 08:56:35.401328 rin_string_manip-0.1.1/rin_string_manip/stopwords.yaml
--rw-r--r--   0        0        0     1479 2023-07-11 08:43:55.314709 rin_string_manip-0.1.1/rin_string_manip/string_funcs.py
--rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 rin_string_manip-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-11 09:00:11.252912 rin_string_manip-0.1.2/README.md
+-rw-r--r--   0        0        0      417 2023-07-11 09:24:10.822038 rin_string_manip-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 05:56:34.768991 rin_string_manip-0.1.2/rin_string_manip/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-11 08:26:33.403502 rin_string_manip-0.1.2/rin_string_manip/config.yaml
+-rw-r--r--   0        0        0      747 2023-07-11 07:39:54.547307 rin_string_manip-0.1.2/rin_string_manip/log_error.py
+-rw-r--r--   0        0        0      378 2023-07-11 07:21:26.032932 rin_string_manip-0.1.2/rin_string_manip/logging.yaml
+-rw-r--r--   0        0        0      975 2023-07-11 09:22:33.442937 rin_string_manip-0.1.2/rin_string_manip/main.py
+-rw-r--r--   0        0        0      540 2023-07-11 09:18:04.917640 rin_string_manip-0.1.2/rin_string_manip/stopwords.yaml
+-rw-r--r--   0        0        0     1356 2023-07-11 09:22:55.258733 rin_string_manip-0.1.2/rin_string_manip/string_funcs.py
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 rin_string_manip-0.1.2/PKG-INFO
```

### Comparing `rin_string_manip-0.1.1/README.md` & `rin_string_manip-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rin_string_manip-0.1.1/rin_string_manip/log_error.py` & `rin_string_manip-0.1.2/rin_string_manip/log_error.py`

 * *Files identical despite different names*

### Comparing `rin_string_manip-0.1.1/rin_string_manip/main.py` & `rin_string_manip-0.1.2/rin_string_manip/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,30 +5,28 @@
 from rin_string_manip.string_funcs import stair_case, prepend_number, append_date, remove_stop_words, coalesce_spaces
 from rin_string_manip.log_error import error_log, get_yaml
 
 app = typer.Typer()
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def pipe_func(*args, func, write_path):
-    func = globals()[func]
-    with open(write_path, "w") as write_file:
-        write_file.write(func(*args))
-    write_file.close()
-
-
 @app.command()
 @error_log
 def apply_pipline(config_path: str = os.path.dirname(__file__) + "/config.yaml", file_path: str = "file.txt") -> None:
     pipeline = get_yaml(config_path)
+    with open(file_path, "r") as read_file:
+        content = read_file.read()
+    read_file.close()
+
     for func in pipeline["pipeline"]:
-        with open(file_path, "r") as read_file:
-            content = read_file.read()
-        read_file.close()
         logger.info(f"Executing {func} function.")
-        pipe_func(content, func=func, write_path=file_path)
+        content = globals()[func](content)
         logger.debug(str(globals()[func]) + str(type(globals()[func])))
+
+    with open("new_file.txt", "w") as write_file:
+        write_file.write(content)
+    write_file.close()
     logger.debug("Finished executing pipeline")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `rin_string_manip-0.1.1/rin_string_manip/stopwords.yaml` & `rin_string_manip-0.1.2/rin_string_manip/stopwords.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -51,12 +51,10 @@
   - They
   - I
   - In
   - If
   - Is
   - Into
   - It
-  - No
+  - "No"
   - Nor
-  - Not
-  - Then
-  - They
+  - Not
```

### Comparing `rin_string_manip-0.1.1/rin_string_manip/string_funcs.py` & `rin_string_manip-0.1.2/rin_string_manip/string_funcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 def append_date(string: str) -> str:
     return string+" "+str(dt.now())
 
 
 def get_stop_words() -> list:
     with open(os.path.dirname(__file__)+"/stopwords.yaml", 'r') as file:
         stop_words: list = yaml.safe_load(file)["stopwords"]
+    logging.debug(stop_words)
     sw_lower = [word.lower() for word in stop_words]
     return sw_lower
 
 
 def remove_stop_words(string: str) -> str:
     stop_words = get_stop_words()
     new_str = []
@@ -46,13 +47,7 @@
 def coalesce_spaces(string: str) -> str:
     new_str = []
     for word in string.split(' '):
         if new_str and new_str[-1] == " " and word == " ":
             continue
         new_str.append(word)
     return ' '.join(new_str)
-
-
-if __name__ == "__main__":
-    print(coalesce_spaces("hello  everynyan I     am a  bird"))
-    pass
-    # print(prepend_number("hii\nthis is line 2"))
```

### Comparing `rin_string_manip-0.1.1/PKG-INFO` & `rin_string_manip-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: rin-string-manip
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Harine
-Author-email: you@example.com
+Author-email: haariinee@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

