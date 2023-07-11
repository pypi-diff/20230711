# Comparing `tmp/passage-identity-2.1.2.tar.gz` & `tmp/passage-identity-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passage-identity-2.1.2.tar", last modified: Thu Apr  6 15:56:34 2023, max compression
+gzip compressed data, was "passage-identity-2.1.3.tar", last modified: Tue Jul 11 18:08:27 2023, max compression
```

## Comparing `passage-identity-2.1.2.tar` & `passage-identity-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:56:34.681238 passage-identity-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-06 15:56:19.000000 passage-identity-2.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-06 15:56:34.677238 passage-identity-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-06 15:56:19.000000 passage-identity-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:56:34.677238 passage-identity-2.1.2/passage_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-06 15:56:34.000000 passage-identity-2.1.2/passage_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-06 15:56:34.000000 passage-identity-2.1.2/passage_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:56:34.000000 passage-identity-2.1.2/passage_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-06 15:56:34.000000 passage-identity-2.1.2/passage_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 15:56:34.000000 passage-identity-2.1.2/passage_identity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:56:34.677238 passage-identity-2.1.2/passageidentity/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-06 15:56:19.000000 passage-identity-2.1.2/passageidentity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-06 15:56:19.000000 passage-identity-2.1.2/passageidentity/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-06 15:56:19.000000 passage-identity-2.1.2/passageidentity/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    17842 2023-04-06 15:56:19.000000 passage-identity-2.1.2/passageidentity/passage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-06 15:56:19.000000 passage-identity-2.1.2/passageidentity/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-06 15:56:19.000000 passage-identity-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 15:56:34.681238 passage-identity-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-06 15:56:19.000000 passage-identity-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:08:27.355817 passage-identity-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-11 18:08:16.000000 passage-identity-2.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-07-11 18:08:27.355817 passage-identity-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-11 18:08:16.000000 passage-identity-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:08:27.351817 passage-identity-2.1.3/passage_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-07-11 18:08:27.000000 passage-identity-2.1.3/passage_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-11 18:08:27.000000 passage-identity-2.1.3/passage_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:08:27.000000 passage-identity-2.1.3/passage_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 18:08:27.000000 passage-identity-2.1.3/passage_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 18:08:27.000000 passage-identity-2.1.3/passage_identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:08:27.355817 passage-identity-2.1.3/passageidentity/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 18:08:16.000000 passage-identity-2.1.3/passageidentity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 18:08:16.000000 passage-identity-2.1.3/passageidentity/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-11 18:08:16.000000 passage-identity-2.1.3/passageidentity/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-07-11 18:08:16.000000 passage-identity-2.1.3/passageidentity/passage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-11 18:08:16.000000 passage-identity-2.1.3/passageidentity/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-11 18:08:16.000000 passage-identity-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:08:27.355817 passage-identity-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-11 18:08:16.000000 passage-identity-2.1.3/setup.py
```

### Comparing `passage-identity-2.1.2/LICENSE.txt` & `passage-identity-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `passage-identity-2.1.2/PKG-INFO` & `passage-identity-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passage-identity
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python library to help manage your Passage application and users
 Home-page: https://github.com/passageidentity/passage-python
 Author: Passage Identity, Inc
 Author-email: support@passage.id
 Project-URL: Bug Tracker, https://github.com/passageidentity/passage-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `passage-identity-2.1.2/README.md` & `passage-identity-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `passage-identity-2.1.2/passage_identity.egg-info/PKG-INFO` & `passage-identity-2.1.3/passage_identity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passage-identity
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python library to help manage your Passage application and users
 Home-page: https://github.com/passageidentity/passage-python
 Author: Passage Identity, Inc
 Author-email: support@passage.id
 Project-URL: Bug Tracker, https://github.com/passageidentity/passage-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `passage-identity-2.1.2/passageidentity/helper.py` & `passage-identity-2.1.3/passageidentity/helper.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.1.2/passageidentity/passage.py` & `passage-identity-2.1.3/passageidentity/passage.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
         phone: str
         channel: ChannelType
         send: bool
         magic_link_path: str
         redirect_url: str
         ttl: int
         language: str
+        type: str
 
     """
     Create Passage MagicLink
     """
     def createMagicLink(self, magicLinkAttributes: MagicLinkAttributes) -> Union[PassageMagicLinkType, PassageError]:
         # if no api key, fail
         if self.passage_apikey == "":
```

### Comparing `passage-identity-2.1.2/passageidentity/requests.py` & `passage-identity-2.1.3/passageidentity/requests.py`

 * *Files identical despite different names*

### Comparing `passage-identity-2.1.2/setup.py` & `passage-identity-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="passage-identity",
-    version="2.1.2",
+    version="2.1.3",
     author="Passage Identity, Inc",
     author_email="support@passage.id",
     description="Python library to help manage your Passage application and users",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/passageidentity/passage-python",
     project_urls={
```

