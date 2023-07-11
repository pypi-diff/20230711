# Comparing `tmp/jk_version-0.2022.8.7.tar.gz` & `tmp/jk_version-0.2023.7.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jk_version-0.2022.8.7.tar", last modified: Sun Aug  7 13:48:05 2022, max compression
+gzip compressed data, was "jk_version-0.2023.7.11.tar", last modified: Tue Jul 11 04:41:30 2023, max compression
```

## Comparing `jk_version-0.2022.8.7.tar` & `jk_version-0.2023.7.11.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-07 13:48:05.152029 jk_version-0.2022.8.7/
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)    10173 2022-02-11 06:52:46.000000 jk_version-0.2022.8.7/LICENSE.txt
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)       38 2022-08-06 07:47:41.000000 jk_version-0.2022.8.7/MANIFEST.in
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     5710 2022-08-07 13:48:05.152029 jk_version-0.2022.8.7/PKG-INFO
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     4012 2022-08-06 07:47:41.000000 jk_version-0.2022.8.7/README.md
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-07 13:48:05.152029 jk_version-0.2022.8.7/jk_version/
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1697 2022-02-01 21:12:35.000000 jk_version-0.2022.8.7/jk_version/BaseVersionConstraint.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     7797 2022-08-07 13:43:35.000000 jk_version-0.2022.8.7/jk_version/Version.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2394 2022-01-30 13:49:22.000000 jk_version-0.2022.8.7/jk_version/VersionConstraintAND.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1769 2022-01-30 13:49:03.000000 jk_version-0.2022.8.7/jk_version/VersionConstraintEQ.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1769 2022-01-30 13:48:54.000000 jk_version-0.2022.8.7/jk_version/VersionConstraintGE.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1765 2022-01-30 13:48:44.000000 jk_version-0.2022.8.7/jk_version/VersionConstraintGT.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1769 2022-01-30 13:48:35.000000 jk_version-0.2022.8.7/jk_version/VersionConstraintLE.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1765 2022-01-30 13:48:24.000000 jk_version-0.2022.8.7/jk_version/VersionConstraintLT.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1769 2022-01-30 13:48:16.000000 jk_version-0.2022.8.7/jk_version/VersionConstraintNE.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2337 2022-01-30 13:48:07.000000 jk_version-0.2022.8.7/jk_version/VersionConstraintOR.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     3487 2022-01-30 16:18:18.000000 jk_version-0.2022.8.7/jk_version/_ConstraintDeserializer.py
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      641 2022-08-07 13:45:54.000000 jk_version-0.2022.8.7/jk_version/__init__.py
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-08-07 13:48:05.152029 jk_version-0.2022.8.7/jk_version.egg-info/
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     5710 2022-08-07 13:48:05.000000 jk_version-0.2022.8.7/jk_version.egg-info/PKG-INFO
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      603 2022-08-07 13:48:05.000000 jk_version-0.2022.8.7/jk_version.egg-info/SOURCES.txt
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)        1 2022-08-07 13:48:05.000000 jk_version-0.2022.8.7/jk_version.egg-info/dependency_links.txt
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)        1 2020-02-11 18:04:19.000000 jk_version-0.2022.8.7/jk_version.egg-info/not-zip-safe
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)       11 2022-08-07 13:48:05.000000 jk_version-0.2022.8.7/jk_version.egg-info/top_level.txt
--rw-rw----   0 woodoo    (1000) woodoo    (1000)       38 2022-08-07 13:48:05.152029 jk_version-0.2022.8.7/setup.cfg
--rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1425 2022-08-07 13:45:54.000000 jk_version-0.2022.8.7/setup.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-07-11 04:41:30.536067 jk_version-0.2023.7.11/
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)    10173 2022-02-11 06:52:46.000000 jk_version-0.2023.7.11/LICENSE.txt
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)       38 2022-08-06 07:47:41.000000 jk_version-0.2023.7.11/MANIFEST.in
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)     5711 2023-07-11 04:41:30.536067 jk_version-0.2023.7.11/PKG-INFO
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     4012 2022-08-06 07:47:41.000000 jk_version-0.2023.7.11/README.md
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-07-11 04:41:30.536067 jk_version-0.2023.7.11/jk_version/
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1697 2022-02-01 21:12:35.000000 jk_version-0.2023.7.11/jk_version/BaseVersionConstraint.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     7897 2023-07-08 16:09:58.000000 jk_version-0.2023.7.11/jk_version/Version.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2394 2022-01-30 13:49:22.000000 jk_version-0.2023.7.11/jk_version/VersionConstraintAND.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1769 2022-01-30 13:49:03.000000 jk_version-0.2023.7.11/jk_version/VersionConstraintEQ.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1769 2022-01-30 13:48:54.000000 jk_version-0.2023.7.11/jk_version/VersionConstraintGE.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1765 2022-01-30 13:48:44.000000 jk_version-0.2023.7.11/jk_version/VersionConstraintGT.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1769 2022-01-30 13:48:35.000000 jk_version-0.2023.7.11/jk_version/VersionConstraintLE.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1765 2022-01-30 13:48:24.000000 jk_version-0.2023.7.11/jk_version/VersionConstraintLT.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1769 2022-01-30 13:48:16.000000 jk_version-0.2023.7.11/jk_version/VersionConstraintNE.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     2337 2022-01-30 13:48:07.000000 jk_version-0.2023.7.11/jk_version/VersionConstraintOR.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     3395 2022-08-18 10:49:11.000000 jk_version-0.2023.7.11/jk_version/_ConstraintDeserializer.py
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)      642 2023-07-11 04:38:03.000000 jk_version-0.2023.7.11/jk_version/__init__.py
+drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2023-07-11 04:41:30.536067 jk_version-0.2023.7.11/jk_version.egg-info/
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)     5711 2023-07-11 04:41:30.000000 jk_version-0.2023.7.11/jk_version.egg-info/PKG-INFO
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)      603 2023-07-11 04:41:30.000000 jk_version-0.2023.7.11/jk_version.egg-info/SOURCES.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)        1 2023-07-11 04:41:30.000000 jk_version-0.2023.7.11/jk_version.egg-info/dependency_links.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)        1 2023-07-11 04:41:30.000000 jk_version-0.2023.7.11/jk_version.egg-info/not-zip-safe
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)       11 2023-07-11 04:41:30.000000 jk_version-0.2023.7.11/jk_version.egg-info/top_level.txt
+-rw-rw----   0 woodoo    (1000) woodoo    (1000)       38 2023-07-11 04:41:30.536067 jk_version-0.2023.7.11/setup.cfg
+-rw-rw-r--   0 woodoo    (1000) woodoo    (1000)     1426 2023-07-11 04:38:03.000000 jk_version-0.2023.7.11/setup.py
```

### Comparing `jk_version-0.2022.8.7/LICENSE.txt` & `jk_version-0.2023.7.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/PKG-INFO` & `jk_version-0.2023.7.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jk_version
-Version: 0.2022.8.7
+Version: 0.2023.7.11
 Summary: This python module provides a version class. Instances of this class may be used in representing and version numbers and compare them.
 Home-page: UNKNOWN
 Author: Jürgen Knauth
 Author-email: pubsrc@binary-overflow.de
 License: Apache2
 Description: jk_version
         ==========
```

### Comparing `jk_version-0.2022.8.7/README.md` & `jk_version-0.2023.7.11/README.md`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/jk_version/BaseVersionConstraint.py` & `jk_version-0.2023.7.11/jk_version/BaseVersionConstraint.py`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/jk_version/Version.py` & `jk_version-0.2023.7.11/jk_version/Version.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,17 +90,22 @@
 	#
 
 	@property
 	def numbers(self) -> list:
 		return list(self.__numbers)
 	#
 
-	# TODO: rename to "isDateBased"
+	# Deprecated, but still present for compatibility reasons
 	@property
 	def isDateBase(self) -> bool:
+		return self.isDateBased
+	#
+
+	@property
+	def isDateBased(self) -> bool:
 		if len(self.__numbers) < 4:
 			return False
 		if self.__numbers[0] != 0:
 			return False
 		if (self.__numbers[1] < 2010) or (self.__numbers[1] > 2100):
 			return False
 		if (self.__numbers[2] < 1) or (self.__numbers[2] > 12):
@@ -135,15 +140,15 @@
 
 	@staticmethod
 	def __parseFromStr(text:str, bStrict:bool = False) -> tuple:
 		try:
 			m = re.match(r"^((?P<epoch>[0-9]+):)?(?P<version>[0-9\.]+)([\-~\+](?P<extra>.+))?$", text)
 			if not bStrict:
 				if not m:
-					m = re.match(r"^((?P<epoch>[0-9]+):)?(?P<version>[0-9\.]+)([\-~\+\.](?P<extra>[a-zA-Z][a-zA-Z0-9]*))?$", text)
+					m = re.match(r"^((?P<epoch>[0-9]+):)?(?P<version>[0-9\.]+)([\-~\+\.]?(?P<extra>[a-zA-Z][a-zA-Z0-9]*))?$", text)
 			if not m:
 				return None, None, None
 
 			_epoch = 0
 			_extra = None
 
 			sEpoch = m.group("epoch")
```

### Comparing `jk_version-0.2022.8.7/jk_version/VersionConstraintAND.py` & `jk_version-0.2023.7.11/jk_version/VersionConstraintAND.py`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/jk_version/VersionConstraintEQ.py` & `jk_version-0.2023.7.11/jk_version/VersionConstraintEQ.py`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/jk_version/VersionConstraintGE.py` & `jk_version-0.2023.7.11/jk_version/VersionConstraintGE.py`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/jk_version/VersionConstraintGT.py` & `jk_version-0.2023.7.11/jk_version/VersionConstraintGT.py`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/jk_version/VersionConstraintLE.py` & `jk_version-0.2023.7.11/jk_version/VersionConstraintLE.py`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/jk_version/VersionConstraintLT.py` & `jk_version-0.2023.7.11/jk_version/VersionConstraintLT.py`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/jk_version/VersionConstraintNE.py` & `jk_version-0.2023.7.11/jk_version/VersionConstraintNE.py`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/jk_version/VersionConstraintOR.py` & `jk_version-0.2023.7.11/jk_version/VersionConstraintOR.py`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/jk_version/_ConstraintDeserializer.py` & `jk_version-0.2023.7.11/jk_version/_ConstraintDeserializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 
 
 # from __future__ import annotations
 
 import os
 import typing
 
-import jk_typing
-import jk_utils
-import jk_logging
-import jk_json
-import jk_prettyprintobj
-
 from .BaseVersionConstraint import BaseVersionConstraint
 
 from .VersionConstraintGE import VersionConstraintGE
 from .VersionConstraintGT import VersionConstraintGT
 from .VersionConstraintLE import VersionConstraintLE
 from .VersionConstraintLT import VersionConstraintLT
 from .VersionConstraintNE import VersionConstraintNE
```

### Comparing `jk_version-0.2022.8.7/jk_version/__init__.py` & `jk_version-0.2023.7.11/jk_version/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 
 __author__ = "Jürgen Knauth"
-__version__ = "0.2022.8.7"
+__version__ = "0.2023.7.11"
 
 
 
 from .Version import Version
 
 from .BaseVersionConstraint import BaseVersionConstraint
```

### Comparing `jk_version-0.2022.8.7/jk_version.egg-info/PKG-INFO` & `jk_version-0.2023.7.11/jk_version.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jk-version
-Version: 0.2022.8.7
+Version: 0.2023.7.11
 Summary: This python module provides a version class. Instances of this class may be used in representing and version numbers and compare them.
 Home-page: UNKNOWN
 Author: Jürgen Knauth
 Author-email: pubsrc@binary-overflow.de
 License: Apache2
 Description: jk_version
         ==========
```

### Comparing `jk_version-0.2022.8.7/jk_version.egg-info/SOURCES.txt` & `jk_version-0.2023.7.11/jk_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jk_version-0.2022.8.7/setup.py` & `jk_version-0.2023.7.11/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,12 +38,12 @@
 		],
 	},
 	packages = [
 		"jk_version",
 	],
 	scripts = [
 	],
-	version = '0.2022.8.7',
+	version = "0.2023.7.11",
 	zip_safe = False,
 	long_description = readme(),
 	long_description_content_type = "text/markdown",
 )
```

