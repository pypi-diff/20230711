# Comparing `tmp/github-secret-syncer-0.0.7.tar.gz` & `tmp/github-secret-syncer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-secret-syncer-0.0.7.tar", last modified: Sat Jul  8 09:45:18 2023, max compression
+gzip compressed data, was "github-secret-syncer-0.0.8.tar", last modified: Tue Jul 11 00:53:57 2023, max compression
```

## Comparing `github-secret-syncer-0.0.7.tar` & `github-secret-syncer-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-08 09:45:18.874470 github-secret-syncer-0.0.7/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-30 17:47:40.000000 github-secret-syncer-0.0.7/LICENSE
--rw-r--r--   0 j3ymac     (501) staff       (20)     1216 2023-07-08 09:45:18.874256 github-secret-syncer-0.0.7/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      734 2023-07-08 09:44:30.000000 github-secret-syncer-0.0.7/README.md
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-08 09:45:18.873089 github-secret-syncer-0.0.7/github_secret_syncer/
--rw-r--r--   0 j3ymac     (501) staff       (20)     4525 2023-07-08 09:29:14.000000 github-secret-syncer-0.0.7/github_secret_syncer/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-08 09:45:18.873702 github-secret-syncer-0.0.7/github_secret_syncer.egg-info/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1216 2023-07-08 09:45:18.000000 github-secret-syncer-0.0.7/github_secret_syncer.egg-info/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      235 2023-07-08 09:45:18.000000 github-secret-syncer-0.0.7/github_secret_syncer.egg-info/SOURCES.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-08 09:45:18.000000 github-secret-syncer-0.0.7/github_secret_syncer.egg-info/dependency_links.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-08 09:45:18.000000 github-secret-syncer-0.0.7/github_secret_syncer.egg-info/top_level.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-08 09:45:18.874526 github-secret-syncer-0.0.7/setup.cfg
--rw-r--r--   0 j3ymac     (501) staff       (20)      733 2023-07-08 09:44:16.000000 github-secret-syncer-0.0.7/setup.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:53:57.122787 github-secret-syncer-0.0.8/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-30 17:47:40.000000 github-secret-syncer-0.0.8/LICENSE
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1216 2023-07-11 00:53:57.122617 github-secret-syncer-0.0.8/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      734 2023-07-08 09:44:30.000000 github-secret-syncer-0.0.8/README.md
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:53:57.121587 github-secret-syncer-0.0.8/github_secret_syncer/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     4525 2023-07-08 09:29:14.000000 github-secret-syncer-0.0.8/github_secret_syncer/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-11 00:53:57.122418 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1216 2023-07-11 00:53:57.000000 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      278 2023-07-11 00:53:57.000000 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/SOURCES.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-11 00:53:57.000000 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/dependency_links.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       14 2023-07-11 00:53:57.000000 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/requires.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       21 2023-07-11 00:53:57.000000 github-secret-syncer-0.0.8/github_secret_syncer.egg-info/top_level.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-11 00:53:57.122832 github-secret-syncer-0.0.8/setup.cfg
+-rw-r--r--   0 j3ymac     (501) staff       (20)      788 2023-07-11 00:52:16.000000 github-secret-syncer-0.0.8/setup.py
```

### Comparing `github-secret-syncer-0.0.7/LICENSE` & `github-secret-syncer-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `github-secret-syncer-0.0.7/PKG-INFO` & `github-secret-syncer-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-secret-syncer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Github Secret Syncer.
 Home-page: https://github.com/thejimmylin/github-secret-syncer
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `github-secret-syncer-0.0.7/README.md` & `github-secret-syncer-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `github-secret-syncer-0.0.7/github_secret_syncer/__init__.py` & `github-secret-syncer-0.0.8/github_secret_syncer/__init__.py`

 * *Files identical despite different names*

### Comparing `github-secret-syncer-0.0.7/github_secret_syncer.egg-info/PKG-INFO` & `github-secret-syncer-0.0.8/github_secret_syncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-secret-syncer
-Version: 0.0.7
+Version: 0.0.8
 Summary: Github Secret Syncer.
 Home-page: https://github.com/thejimmylin/github-secret-syncer
 Author: thejimmylin
 Author-email: b00502013@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `github-secret-syncer-0.0.7/setup.py` & `github-secret-syncer-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from pathlib import Path
 
 base_dir = Path(__file__).parent.resolve()
 long_description = (base_dir / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="github-secret-syncer",
-    version="0.0.7",
+    version="0.0.8",
+    install_requires=[
+        "PyNaCl==1.5.0",
+    ],
     author="thejimmylin",
     author_email="b00502013@gmail.com",
     description="Github Secret Syncer.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thejimmylin/github-secret-syncer",
     packages=setuptools.find_packages(),
```

