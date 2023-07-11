# Comparing `tmp/aliste-0.1.2.tar.gz` & `tmp/aliste-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aliste-0.1.2.tar", last modified: Tue Jul 11 14:43:27 2023, max compression
+gzip compressed data, was "aliste-0.1.3.tar", last modified: Tue Jul 11 14:59:57 2023, max compression
```

## Comparing `aliste-0.1.2.tar` & `aliste-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 14:43:27.879322 aliste-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-07-11 08:03:48.000000 aliste-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      763 2023-07-11 14:43:27.878314 aliste-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 14:43:27.846921 aliste-0.1.2/aliste/
--rw-rw-rw-   0        0        0       26 2023-07-11 13:34:58.000000 aliste-0.1.2/aliste/__init__.py
--rw-rw-rw-   0        0        0     1399 2023-07-11 13:25:09.000000 aliste-0.1.2/aliste/broker.py
--rw-rw-rw-   0        0        0      344 2023-07-11 13:12:35.000000 aliste-0.1.2/aliste/constants.py
--rw-rw-rw-   0        0        0     1948 2023-07-11 14:41:53.000000 aliste-0.1.2/aliste/device.py
--rw-rw-rw-   0        0        0      145 2023-07-11 11:16:10.000000 aliste-0.1.2/aliste/enums.py
--rw-rw-rw-   0        0        0      346 2023-07-11 13:20:17.000000 aliste-0.1.2/aliste/home.py
--rw-rw-rw-   0        0        0     2668 2023-07-11 14:22:38.000000 aliste-0.1.2/aliste/hub.py
--rw-rw-rw-   0        0        0      353 2023-07-11 11:01:22.000000 aliste-0.1.2/aliste/user.py
--rw-rw-rw-   0        0        0      217 2023-07-11 11:43:02.000000 aliste-0.1.2/aliste/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:43:27.877323 aliste-0.1.2/aliste.egg-info/
--rw-rw-rw-   0        0        0      763 2023-07-11 14:43:27.000000 aliste-0.1.2/aliste.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-07-11 14:43:27.000000 aliste-0.1.2/aliste.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 14:43:27.000000 aliste-0.1.2/aliste.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 14:43:27.000000 aliste-0.1.2/aliste.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 14:43:27.880316 aliste-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-07-11 14:43:19.000000 aliste-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:59:57.807340 aliste-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-07-11 08:03:48.000000 aliste-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      763 2023-07-11 14:59:57.806393 aliste-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 14:59:57.786993 aliste-0.1.3/aliste/
+-rw-rw-rw-   0        0        0       26 2023-07-11 13:34:58.000000 aliste-0.1.3/aliste/__init__.py
+-rw-rw-rw-   0        0        0     1432 2023-07-11 14:59:46.000000 aliste-0.1.3/aliste/broker.py
+-rw-rw-rw-   0        0        0      344 2023-07-11 13:12:35.000000 aliste-0.1.3/aliste/constants.py
+-rw-rw-rw-   0        0        0     1948 2023-07-11 14:41:53.000000 aliste-0.1.3/aliste/device.py
+-rw-rw-rw-   0        0        0      145 2023-07-11 11:16:10.000000 aliste-0.1.3/aliste/enums.py
+-rw-rw-rw-   0        0        0      346 2023-07-11 13:20:17.000000 aliste-0.1.3/aliste/home.py
+-rw-rw-rw-   0        0        0     2668 2023-07-11 14:22:38.000000 aliste-0.1.3/aliste/hub.py
+-rw-rw-rw-   0        0        0      353 2023-07-11 11:01:22.000000 aliste-0.1.3/aliste/user.py
+-rw-rw-rw-   0        0        0      217 2023-07-11 11:43:02.000000 aliste-0.1.3/aliste/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:59:57.805342 aliste-0.1.3/aliste.egg-info/
+-rw-rw-rw-   0        0        0      763 2023-07-11 14:59:57.000000 aliste-0.1.3/aliste.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-07-11 14:59:57.000000 aliste-0.1.3/aliste.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:59:57.000000 aliste-0.1.3/aliste.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 14:59:57.000000 aliste-0.1.3/aliste.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 14:59:57.807340 aliste-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-07-11 14:59:54.000000 aliste-0.1.3/setup.py
```

### Comparing `aliste-0.1.2/LICENSE` & `aliste-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliste-0.1.2/PKG-INFO` & `aliste-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliste
-Version: 0.1.2
+Version: 0.1.3
 Summary: Aliste Smart Home SDK for Python
 Home-page: https://github.com/Kir4Kun/aliste-smart-home-sdk
 Author: Kir4Kun
 Author-email: rkbl4ze@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aliste-0.1.2/aliste/broker.py` & `aliste-0.1.3/aliste/broker.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         }
 
         url = constants.wssUrl + urllib.parse.urlencode(params)
         await self.sio.connect(url=url, transports=["websocket"])
 
     async def disconnect(self):
         await self.sio.disconnect()
+        await self.http.close()
 
     def register_callback(self, callback):
         self.callbacks.append(callback)
 
     def message(self, data):
         for callback in self.callbacks:
             callback(data)
```

### Comparing `aliste-0.1.2/aliste/device.py` & `aliste-0.1.3/aliste/device.py`

 * *Files identical despite different names*

### Comparing `aliste-0.1.2/aliste/hub.py` & `aliste-0.1.3/aliste/hub.py`

 * *Files identical despite different names*

### Comparing `aliste-0.1.2/aliste.egg-info/PKG-INFO` & `aliste-0.1.3/aliste.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aliste
-Version: 0.1.2
+Version: 0.1.3
 Summary: Aliste Smart Home SDK for Python
 Home-page: https://github.com/Kir4Kun/aliste-smart-home-sdk
 Author: Kir4Kun
 Author-email: rkbl4ze@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aliste-0.1.2/setup.py` & `aliste-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Always prefer setuptools over distutils
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="aliste",
-    version="0.1.2",
+    version="0.1.3",
     description="Aliste Smart Home SDK for Python",
     long_description="Aliste Smart Home SDK for Python",
     long_description_content_type="text/markdown",
     url="https://github.com/Kir4Kun/aliste-smart-home-sdk",
     author="Kir4Kun",
     author_email="rkbl4ze@gmail.com",
     license="MIT",
```

