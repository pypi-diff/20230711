# Comparing `tmp/dccsx-0.0.2.tar.gz` & `tmp/dccsx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dccsx-0.0.2.tar", last modified: Mon Jul 10 19:39:01 2023, max compression
+gzip compressed data, was "dccsx-0.0.3.tar", last modified: Tue Jul 11 02:18:27 2023, max compression
```

## Comparing `dccsx-0.0.2.tar` & `dccsx-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-10 19:39:01.100000 dccsx-0.0.2/
--rw-rw----   0 root         (0) everybody  (9997)     1036 2023-07-10 12:00:56.000000 dccsx-0.0.2/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     5462 2023-07-10 19:39:01.100000 dccsx-0.0.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     4752 2023-07-10 19:10:37.000000 dccsx-0.0.2/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-10 19:39:01.096000 dccsx-0.0.2/dccsx/
--rw-rw----   0 root         (0) everybody  (9997)      111 2023-07-10 19:29:46.000000 dccsx-0.0.2/dccsx/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    40419 2023-07-10 19:32:11.000000 dccsx-0.0.2/dccsx/dccsfb.py
--rw-rw----   0 root         (0) everybody  (9997)    31342 2023-07-10 12:02:39.000000 dccsx-0.0.2/dccsx/lan_change.py
--rw-rw----   0 root         (0) everybody  (9997)    27126 2023-07-10 12:02:50.000000 dccsx-0.0.2/dccsx/logo.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-10 19:39:01.100000 dccsx-0.0.2/dccsx.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     5462 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      308 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       46 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-10 19:35:05.000000 dccsx-0.0.2/dccsx.egg-info/not-zip-safe
--rw-rw----   0 root         (0) everybody  (9997)       13 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-10 19:39:01.000000 dccsx-0.0.2/dccsx.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)      650 2023-07-10 19:39:01.104000 dccsx-0.0.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1046 2023-07-10 19:34:26.000000 dccsx-0.0.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-11 02:18:27.588788 dccsx-0.0.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1036 2023-07-10 12:00:56.000000 dccsx-0.0.3/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     5846 2023-07-11 02:18:27.588788 dccsx-0.0.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     5136 2023-07-11 02:17:33.000000 dccsx-0.0.3/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-11 02:18:27.580788 dccsx-0.0.3/dccsx/
+-rw-rw----   0 root         (0) everybody  (9997)      111 2023-07-10 19:29:46.000000 dccsx-0.0.3/dccsx/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    40975 2023-07-11 02:02:31.000000 dccsx-0.0.3/dccsx/dccsfb.py
+-rw-rw----   0 root         (0) everybody  (9997)    31342 2023-07-10 12:02:39.000000 dccsx-0.0.3/dccsx/lan_change.py
+-rw-rw----   0 root         (0) everybody  (9997)    27126 2023-07-10 12:02:50.000000 dccsx-0.0.3/dccsx/logo.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-11 02:18:27.588788 dccsx-0.0.3/dccsx.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     5846 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      308 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       46 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-11 02:18:21.000000 dccsx-0.0.3/dccsx.egg-info/not-zip-safe
+-rw-rw----   0 root         (0) everybody  (9997)       13 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        6 2023-07-11 02:18:27.000000 dccsx-0.0.3/dccsx.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)      650 2023-07-11 02:18:27.588788 dccsx-0.0.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1046 2023-07-11 02:05:20.000000 dccsx-0.0.3/setup.py
```

### Comparing `dccsx-0.0.2/LICENSE` & `dccsx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dccsx-0.0.2/PKG-INFO` & `dccsx-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dccsx
-Version: 0.0.2
+Version: 0.0.3
 Summary: this module team dccs personal module for using shortcut python code
 Home-page: https://github.com/Dccs-team/dccsx
 Author: Md Saimun
 Author-email: teamdccs@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -51,17 +51,17 @@
 ```
 
 ## How To Use? 
 Everything Is Easy Full Documentation Below.
 
 ### Available Features On This Version:
 
-		• Team Logo 
-		• Change Facebook Language (lan_change)
-		• Facebook Auto bot (dccsfb)
+	• Team Logo 
+	• Change Facebook Language (lan_change)
+	• Facebook Auto bot (dccsfb)
 
 
 ### Example Codes (Team Logo):
 
 ```python
 from dccs_logo import logo
 from rich import print as pprint
@@ -107,14 +107,39 @@
         print("Language change failed.")
 
 if __name__ == "__main__":
     main()
 ```
 ### Example Codes (Facebook auto Bot):
 
+```
+from os import system as phone
+import requests
+try:
+    from dccsx import dccsfb
+except:
+	phone("pip install dccsx")
+import time 
+
+##must need this 
+session = requests.session()
+fb =dccsfb(session)
+cookie="your cookie"
+fb.set_cookie(cookie)
+
+
+fb.set_bio("i am a bot")
+fb.add_nickname("balu")
+fb.follow("100077473742575")
+
+## have a many options try like this 
+
+```
+## many options 
+
 ```python
 import requests
 from bs4 import BeautifulSoup
 from dccsx import dccsfb
 import time
 import re
 import random
```

### Comparing `dccsx-0.0.2/README.md` & `dccsx-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 ```
 
 ## How To Use? 
 Everything Is Easy Full Documentation Below.
 
 ### Available Features On This Version:
 
-		• Team Logo 
-		• Change Facebook Language (lan_change)
-		• Facebook Auto bot (dccsfb)
+	• Team Logo 
+	• Change Facebook Language (lan_change)
+	• Facebook Auto bot (dccsfb)
 
 
 ### Example Codes (Team Logo):
 
 ```python
 from dccs_logo import logo
 from rich import print as pprint
@@ -88,14 +88,39 @@
         print("Language change failed.")
 
 if __name__ == "__main__":
     main()
 ```
 ### Example Codes (Facebook auto Bot):
 
+```
+from os import system as phone
+import requests
+try:
+    from dccsx import dccsfb
+except:
+	phone("pip install dccsx")
+import time 
+
+##must need this 
+session = requests.session()
+fb =dccsfb(session)
+cookie="your cookie"
+fb.set_cookie(cookie)
+
+
+fb.set_bio("i am a bot")
+fb.add_nickname("balu")
+fb.follow("100077473742575")
+
+## have a many options try like this 
+
+```
+## many options 
+
 ```python
 import requests
 from bs4 import BeautifulSoup
 from dccsx import dccsfb
 import time
 import re
 import random
```

### Comparing `dccsx-0.0.2/dccsx/lan_change.py` & `dccsx-0.0.3/dccsx/lan_change.py`

 * *Files identical despite different names*

### Comparing `dccsx-0.0.2/dccsx/logo.py` & `dccsx-0.0.3/dccsx/logo.py`

 * *Files identical despite different names*

### Comparing `dccsx-0.0.2/dccsx.egg-info/PKG-INFO` & `dccsx-0.0.3/dccsx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dccsx
-Version: 0.0.2
+Version: 0.0.3
 Summary: this module team dccs personal module for using shortcut python code
 Home-page: https://github.com/Dccs-team/dccsx
 Author: Md Saimun
 Author-email: teamdccs@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -51,17 +51,17 @@
 ```
 
 ## How To Use? 
 Everything Is Easy Full Documentation Below.
 
 ### Available Features On This Version:
 
-		• Team Logo 
-		• Change Facebook Language (lan_change)
-		• Facebook Auto bot (dccsfb)
+	• Team Logo 
+	• Change Facebook Language (lan_change)
+	• Facebook Auto bot (dccsfb)
 
 
 ### Example Codes (Team Logo):
 
 ```python
 from dccs_logo import logo
 from rich import print as pprint
@@ -107,14 +107,39 @@
         print("Language change failed.")
 
 if __name__ == "__main__":
     main()
 ```
 ### Example Codes (Facebook auto Bot):
 
+```
+from os import system as phone
+import requests
+try:
+    from dccsx import dccsfb
+except:
+	phone("pip install dccsx")
+import time 
+
+##must need this 
+session = requests.session()
+fb =dccsfb(session)
+cookie="your cookie"
+fb.set_cookie(cookie)
+
+
+fb.set_bio("i am a bot")
+fb.add_nickname("balu")
+fb.follow("100077473742575")
+
+## have a many options try like this 
+
+```
+## many options 
+
 ```python
 import requests
 from bs4 import BeautifulSoup
 from dccsx import dccsfb
 import time
 import re
 import random
```

### Comparing `dccsx-0.0.2/setup.cfg` & `dccsx-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dccsx
-version = 1.0.0
+version = 0.0.3
 author = Md Saimun
 author_email = teamdccs@gmail.com
 description = this module team dccs personal module for using shortcut python code
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Dccs-team/dccsx
```

### Comparing `dccsx-0.0.2/setup.py` & `dccsx-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dccsx",
-    version="0.0.2",
+    version="0.0.3",
     author="Md Saimun",
     author_email="teamdccs@gmail.com",
     description="this module team dccs personal module for using shortcut python code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Dccs-team/dccsx",
     packages=["dccsx"],
```

