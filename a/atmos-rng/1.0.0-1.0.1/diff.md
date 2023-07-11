# Comparing `tmp/atmos-rng-1.0.0.tar.gz` & `tmp/atmos-rng-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmos-rng-1.0.0.tar", last modified: Tue Jun 27 14:23:47 2023, max compression
+gzip compressed data, was "atmos-rng-1.0.1.tar", last modified: Tue Jul 11 04:50:01 2023, max compression
```

## Comparing `atmos-rng-1.0.0.tar` & `atmos-rng-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:23:47.781036 atmos-rng-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-27 14:23:33.000000 atmos-rng-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-27 14:23:47.777036 atmos-rng-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-27 14:23:33.000000 atmos-rng-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-27 14:23:33.000000 atmos-rng-1.0.0/atmos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:23:47.777036 atmos-rng-1.0.0/atmos_rng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-27 14:23:47.000000 atmos-rng-1.0.0/atmos_rng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-27 14:23:47.000000 atmos-rng-1.0.0/atmos_rng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:23:47.000000 atmos-rng-1.0.0/atmos_rng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-27 14:23:47.000000 atmos-rng-1.0.0/atmos_rng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-27 14:23:47.000000 atmos-rng-1.0.0/atmos_rng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:23:47.781036 atmos-rng-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-27 14:23:33.000000 atmos-rng-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:50:01.785056 atmos-rng-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 04:49:51.000000 atmos-rng-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-11 04:50:01.785056 atmos-rng-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-11 04:49:51.000000 atmos-rng-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-11 04:49:51.000000 atmos-rng-1.0.1/atmos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 04:50:01.785056 atmos-rng-1.0.1/atmos_rng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-11 04:50:01.000000 atmos-rng-1.0.1/atmos_rng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 04:50:01.000000 atmos-rng-1.0.1/atmos_rng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 04:50:01.000000 atmos-rng-1.0.1/atmos_rng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 04:50:01.000000 atmos-rng-1.0.1/atmos_rng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 04:50:01.000000 atmos-rng-1.0.1/atmos_rng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 04:50:01.785056 atmos-rng-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-11 04:49:51.000000 atmos-rng-1.0.1/setup.py
```

### Comparing `atmos-rng-1.0.0/LICENSE` & `atmos-rng-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atmos-rng-1.0.0/PKG-INFO` & `atmos-rng-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmos-rng
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple random generator based off of atmospheric noise instead of math.
 Home-page: https://github.com/therealOri/atmos-rng
 Author: therealOri
 Author-email: therealOri@duck.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,27 +31,30 @@
 __ __
 
 <br />
 <br />
 
 # Ussage and Info
 ```python
-import atmos-rng
+import atmos
 
 if __name__ == '__main__':
     atmos.clear() # clears terminal/cmd window.
     number = atmos.randint(0, 10, 1)
     print(number)
 
     stuff = [69, True, False, 420, 'Apples', 'Bananas', 'Cats', 'Dogs']
     choice = atmos.choice(stuff)
     print(choice)
 
     scrambled = atmos.shuffle(stuff)
     print(scrambled)
+
+    random_bytes = gen_bytes(32)
+    print(f"{random_bytes}\n{len(random_bytes)}")
 ```
 You can find more information here: [Documentation](https://github.com/therealOri/atmos-rng/blob/main/DOCS.md).
 __ __
 
 <br />
 <br />
 <br />
```

### Comparing `atmos-rng-1.0.0/README.md` & `atmos-rng-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,27 +20,30 @@
 __ __
 
 <br />
 <br />
 
 # Ussage and Info
 ```python
-import atmos-rng
+import atmos
 
 if __name__ == '__main__':
     atmos.clear() # clears terminal/cmd window.
     number = atmos.randint(0, 10, 1)
     print(number)
 
     stuff = [69, True, False, 420, 'Apples', 'Bananas', 'Cats', 'Dogs']
     choice = atmos.choice(stuff)
     print(choice)
 
     scrambled = atmos.shuffle(stuff)
     print(scrambled)
+
+    random_bytes = gen_bytes(32)
+    print(f"{random_bytes}\n{len(random_bytes)}")
 ```
 You can find more information here: [Documentation](https://github.com/therealOri/atmos-rng/blob/main/DOCS.md).
 __ __
 
 <br />
 <br />
 <br />
```

### Comparing `atmos-rng-1.0.0/atmos.py` & `atmos-rng-1.0.1/atmos.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,13 +87,36 @@
     else:
         raise ValueError('\nUnable to shuffle data. The data provided is not a list, tuple, or dictionary.')
 
 
 
 
 
+def gen_bytes(length):
+    if not isinstance(length, int):
+        raise ValueError(f'\n\nInvalid type, "gen_bytes()" takes integers, value given is "{type(length)}".')
+    else:
+        byte_array = bytearray()
+        if length == 1:
+            for _ in range(length):
+                number = randint(0, 255, 1)
+                byte_array.append(number)
+            return bytes(byte_array)
+        elif length > 1:
+            list_of_numbers = randint(0, 255, length)
+            for number in list_of_numbers:
+                byte_array.append(int(number))
+            return bytes(byte_array)
+        else:
+            list_of_numbers = randint(0, 255, 32)
+            for number in list_of_numbers:
+                byte_array.append(int(number))
+            return bytes(byte_array)
+
+
+
 
 
 if __name__ == '__main__':
     clear()
     print("uwu")
```

### Comparing `atmos-rng-1.0.0/atmos_rng.egg-info/PKG-INFO` & `atmos-rng-1.0.1/atmos_rng.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmos-rng
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple random generator based off of atmospheric noise instead of math.
 Home-page: https://github.com/therealOri/atmos-rng
 Author: therealOri
 Author-email: therealOri@duck.com
 License: GPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -31,27 +31,30 @@
 __ __
 
 <br />
 <br />
 
 # Ussage and Info
 ```python
-import atmos-rng
+import atmos
 
 if __name__ == '__main__':
     atmos.clear() # clears terminal/cmd window.
     number = atmos.randint(0, 10, 1)
     print(number)
 
     stuff = [69, True, False, 420, 'Apples', 'Bananas', 'Cats', 'Dogs']
     choice = atmos.choice(stuff)
     print(choice)
 
     scrambled = atmos.shuffle(stuff)
     print(scrambled)
+
+    random_bytes = gen_bytes(32)
+    print(f"{random_bytes}\n{len(random_bytes)}")
 ```
 You can find more information here: [Documentation](https://github.com/therealOri/atmos-rng/blob/main/DOCS.md).
 __ __
 
 <br />
 <br />
 <br />
```

### Comparing `atmos-rng-1.0.0/setup.py` & `atmos-rng-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="atmos-rng",
-    version="1.0.0",
+    version="1.0.1",
     author="therealOri",
     license="GPL-3.0",
     install_requires=[
         "requests",
     ],
     author_email="therealOri@duck.com",
     description="A simple random generator based off of atmospheric noise instead of math.",
```

