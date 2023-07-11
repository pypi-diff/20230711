# Comparing `tmp/dccsx-0.0.3.tar.gz` & `tmp/dccsx-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dccsx-0.0.3.tar", last modified: Tue Jul 11 02:18:27 2023, max compression
+gzip compressed data, was "dccsx-0.0.4.tar", last modified: Tue Jul 11 03:40:30 2023, max compression
```

## Comparing `dccsx-0.0.3.tar` & `dccsx-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-11 02:18:27.588788 dccsx-0.0.3/
--rw-rw----   0 root         (0) everybody  (9997)     1036 2023-07-10 12:00:56.000000 dccsx-0.0.3/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     5846 2023-07-11 02:18:27.588788 dccsx-0.0.3/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     5136 2023-07-11 02:17:33.000000 dccsx-0.0.3/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-11 02:18:27.580788 dccsx-0.0.3/dccsx/
--rw-rw----   0 root         (0) everybody  (9997)      111 2023-07-10 19:29:46.000000 dccsx-0.0.3/dccsx/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    40975 2023-07-11 02:02:31.000000 dccsx-0.0.3/dccsx/dccsfb.py
--rw-rw----   0 root         (0) everybody  (9997)    31342 2023-07-10 12:02:39.000000 dccsx-0.0.3/dccsx/lan_change.py
--rw-rw----   0 root         (0) everybody  (9997)    27126 2023-07-10 12:02:50.000000 dccsx-0.0.3/dccsx/logo.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-11 02:18:27.588788 dccsx-0.0.3/dccsx.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     5846 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      308 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       46 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-11 02:18:21.000000 dccsx-0.0.3/dccsx.egg-info/not-zip-safe
--rw-rw----   0 root         (0) everybody  (9997)       13 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)      650 2023-07-11 02:18:27.588788 dccsx-0.0.3/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1046 2023-07-11 02:05:20.000000 dccsx-0.0.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-11 03:40:30.679000 dccsx-0.0.4/
+-rw-rw----   0 root         (0) everybody  (9997)     1036 2023-07-10 12:00:56.000000 dccsx-0.0.4/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     5852 2023-07-11 03:40:30.679000 dccsx-0.0.4/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     5142 2023-07-11 02:30:42.000000 dccsx-0.0.4/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-11 03:40:30.667000 dccsx-0.0.4/dccsx/
+-rw-rw----   0 root         (0) everybody  (9997)      111 2023-07-10 19:29:46.000000 dccsx-0.0.4/dccsx/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    41647 2023-07-11 03:39:29.000000 dccsx-0.0.4/dccsx/dccsfb.py
+-rw-rw----   0 root         (0) everybody  (9997)    31342 2023-07-10 12:02:39.000000 dccsx-0.0.4/dccsx/lan_change.py
+-rw-rw----   0 root         (0) everybody  (9997)    27126 2023-07-10 12:02:50.000000 dccsx-0.0.4/dccsx/logo.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-11 03:40:30.679000 dccsx-0.0.4/dccsx.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     5852 2023-07-11 03:40:30.000000 dccsx-0.0.4/dccsx.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      308 2023-07-11 03:40:30.000000 dccsx-0.0.4/dccsx.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-11 03:40:30.000000 dccsx-0.0.4/dccsx.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       46 2023-07-11 03:40:30.000000 dccsx-0.0.4/dccsx.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-11 03:40:30.000000 dccsx-0.0.4/dccsx.egg-info/not-zip-safe
+-rw-rw----   0 root         (0) everybody  (9997)       13 2023-07-11 03:40:30.000000 dccsx-0.0.4/dccsx.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-11 03:40:30.000000 dccsx-0.0.4/dccsx.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)      650 2023-07-11 03:40:30.679000 dccsx-0.0.4/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1046 2023-07-11 03:37:42.000000 dccsx-0.0.4/setup.py
```

### Comparing `dccsx-0.0.3/LICENSE` & `dccsx-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dccsx-0.0.3/PKG-INFO` & `dccsx-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dccsx
-Version: 0.0.3
+Version: 0.0.4
 Summary: this module team dccs personal module for using shortcut python code
 Home-page: https://github.com/Dccs-team/dccsx
 Author: Md Saimun
 Author-email: teamdccs@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -107,15 +107,15 @@
         print("Language change failed.")
 
 if __name__ == "__main__":
     main()
 ```
 ### Example Codes (Facebook auto Bot):
 
-```
+```python
 from os import system as phone
 import requests
 try:
     from dccsx import dccsfb
 except:
 	phone("pip install dccsx")
 import time
```

### Comparing `dccsx-0.0.3/README.md` & `dccsx-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         print("Language change failed.")
 
 if __name__ == "__main__":
     main()
 ```
 ### Example Codes (Facebook auto Bot):
 
-```
+```python
 from os import system as phone
 import requests
 try:
     from dccsx import dccsfb
 except:
 	phone("pip install dccsx")
 import time
```

### Comparing `dccsx-0.0.3/dccsx/lan_change.py` & `dccsx-0.0.4/dccsx/lan_change.py`

 * *Files identical despite different names*

### Comparing `dccsx-0.0.3/dccsx/logo.py` & `dccsx-0.0.4/dccsx/logo.py`

 * *Files identical despite different names*

### Comparing `dccsx-0.0.3/dccsx.egg-info/PKG-INFO` & `dccsx-0.0.4/dccsx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dccsx
-Version: 0.0.3
+Version: 0.0.4
 Summary: this module team dccs personal module for using shortcut python code
 Home-page: https://github.com/Dccs-team/dccsx
 Author: Md Saimun
 Author-email: teamdccs@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -107,15 +107,15 @@
         print("Language change failed.")
 
 if __name__ == "__main__":
     main()
 ```
 ### Example Codes (Facebook auto Bot):
 
-```
+```python
 from os import system as phone
 import requests
 try:
     from dccsx import dccsfb
 except:
 	phone("pip install dccsx")
 import time
```

### Comparing `dccsx-0.0.3/setup.cfg` & `dccsx-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dccsx
-version = 0.0.3
+version = 0.0.4
 author = Md Saimun
 author_email = teamdccs@gmail.com
 description = this module team dccs personal module for using shortcut python code
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Dccs-team/dccsx
```

### Comparing `dccsx-0.0.3/setup.py` & `dccsx-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dccsx",
-    version="0.0.3",
+    version="0.0.4",
     author="Md Saimun",
     author_email="teamdccs@gmail.com",
     description="this module team dccs personal module for using shortcut python code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Dccs-team/dccsx",
     packages=["dccsx"],
```

