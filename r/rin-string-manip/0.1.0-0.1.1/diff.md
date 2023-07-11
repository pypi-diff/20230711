# Comparing `tmp/rin_string_manip-0.1.0.tar.gz` & `tmp/rin_string_manip-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rin_string_manip-0.1.0.tar", max compression
+gzip compressed data, was "rin_string_manip-0.1.1.tar", max compression
```

## Comparing `rin_string_manip-0.1.0.tar` & `rin_string_manip-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1152 2023-07-11 08:45:35.271673 rin_string_manip-0.1.0/README.md
--rw-r--r--   0        0        0      416 2023-07-11 06:18:52.276905 rin_string_manip-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 05:56:34.768991 rin_string_manip-0.1.0/rin_string_manip/__init__.py
--rw-r--r--   0        0        0      102 2023-07-11 08:26:33.403502 rin_string_manip-0.1.0/rin_string_manip/config.yaml
--rw-r--r--   0        0        0      747 2023-07-11 07:39:54.547307 rin_string_manip-0.1.0/rin_string_manip/log_error.py
--rw-r--r--   0        0        0      378 2023-07-11 07:21:26.032932 rin_string_manip-0.1.0/rin_string_manip/logging.yaml
--rw-r--r--   0        0        0     1071 2023-07-11 08:32:40.767598 rin_string_manip-0.1.0/rin_string_manip/main.py
--rw-r--r--   0        0        0     2156 2023-07-11 08:29:04.181697 rin_string_manip-0.1.0/rin_string_manip/main_old.py
--rw-r--r--   0        0        0       87 2023-07-11 08:08:07.779036 rin_string_manip-0.1.0/rin_string_manip/stopwords.yaml
--rw-r--r--   0        0        0     1479 2023-07-11 08:43:55.314709 rin_string_manip-0.1.0/rin_string_manip/string_funcs.py
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 rin_string_manip-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-11 09:00:11.252912 rin_string_manip-0.1.1/README.md
+-rw-r--r--   0        0        0      413 2023-07-11 09:00:50.756809 rin_string_manip-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 05:56:34.768991 rin_string_manip-0.1.1/rin_string_manip/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-11 08:26:33.403502 rin_string_manip-0.1.1/rin_string_manip/config.yaml
+-rw-r--r--   0        0        0      747 2023-07-11 07:39:54.547307 rin_string_manip-0.1.1/rin_string_manip/log_error.py
+-rw-r--r--   0        0        0      378 2023-07-11 07:21:26.032932 rin_string_manip-0.1.1/rin_string_manip/logging.yaml
+-rw-r--r--   0        0        0     1071 2023-07-11 08:32:40.767598 rin_string_manip-0.1.1/rin_string_manip/main.py
+-rw-r--r--   0        0        0      556 2023-07-11 08:56:35.401328 rin_string_manip-0.1.1/rin_string_manip/stopwords.yaml
+-rw-r--r--   0        0        0     1479 2023-07-11 08:43:55.314709 rin_string_manip-0.1.1/rin_string_manip/string_funcs.py
+-rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 rin_string_manip-0.1.1/PKG-INFO
```

### Comparing `rin_string_manip-0.1.0/README.md` & `rin_string_manip-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Perform string manipulation operations using a single command.<br>
 <h1>Usage</h1>
 run the following command
 
 ```bash
-ring-string-manip --OPTIONS
+rin_string_manip --OPTIONS
 ```
 OPTIONS that can be provided are:
 
 ```commandline
 config-path: path/to/config.yaml
 file-path: path/to/file.txt
 ```
@@ -30,29 +30,15 @@
   - append_date
   - prepend_number
 ```
 Refer below for available functions.
 <hr>
 <h1>Functions available</h1>
 <h3>remove_stop_words</h3>
-Removes stop_words from given string. Default stop_words are
-
-```yaml
-stopwords:
-  - A
-  - The
-  - An
-  - Is
-  - For
-  - It
-  - Our
-  - We
-  - They
-  - Their
-```
+Removes stop_words from given string. Stop words are taken from stopwords.yaml
 <h3>coalesce_spaces</h3>
 Converts multiple spaces into one space
 <br>
 
 <h3>stair_case</h3>
 Converts first letter upper, second lower, third upper and so on.
 <br>
```

### Comparing `rin_string_manip-0.1.0/rin_string_manip/log_error.py` & `rin_string_manip-0.1.1/rin_string_manip/log_error.py`

 * *Files identical despite different names*

### Comparing `rin_string_manip-0.1.0/rin_string_manip/main.py` & `rin_string_manip-0.1.1/rin_string_manip/main.py`

 * *Files identical despite different names*

### Comparing `rin_string_manip-0.1.0/rin_string_manip/string_funcs.py` & `rin_string_manip-0.1.1/rin_string_manip/string_funcs.py`

 * *Files identical despite different names*

### Comparing `rin_string_manip-0.1.0/PKG-INFO` & `rin_string_manip-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: rin-string-manip
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
-Author: Your Name
+Author: Harine
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 Perform string manipulation operations using a single command.<br>
 <h1>Usage</h1>
 run the following command
 
 ```bash
-ring-string-manip --OPTIONS
+rin_string_manip --OPTIONS
 ```
 OPTIONS that can be provided are:
 
 ```commandline
 config-path: path/to/config.yaml
 file-path: path/to/file.txt
 ```
@@ -44,29 +44,15 @@
   - append_date
   - prepend_number
 ```
 Refer below for available functions.
 <hr>
 <h1>Functions available</h1>
 <h3>remove_stop_words</h3>
-Removes stop_words from given string. Default stop_words are
-
-```yaml
-stopwords:
-  - A
-  - The
-  - An
-  - Is
-  - For
-  - It
-  - Our
-  - We
-  - They
-  - Their
-```
+Removes stop_words from given string. Stop words are taken from stopwords.yaml
 <h3>coalesce_spaces</h3>
 Converts multiple spaces into one space
 <br>
 
 <h3>stair_case</h3>
 Converts first letter upper, second lower, third upper and so on.
 <br>
```

