# Comparing `tmp/simple-git-versioning-0.1.4.tar.gz` & `tmp/simple-git-versioning-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-git-versioning-0.1.4.tar", last modified: Mon Jul 10 21:32:54 2023, max compression
+gzip compressed data, was "simple-git-versioning-0.1.6.tar", last modified: Mon Jul 10 21:56:08 2023, max compression
```

## Comparing `simple-git-versioning-0.1.4.tar` & `simple-git-versioning-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:32:54.172634 simple-git-versioning-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5099 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3862 2023-07-10 21:32:54.172634 simple-git-versioning-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    46416 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/Pipfile.lock
--rw-rw-rw-   0 root         (0) root         (0)     2845 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1878 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 21:32:54.172634 simple-git-versioning-0.1.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:32:54.169634 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3862 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      681 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      204 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 21:32:54.000000 simple-git-versioning-0.1.4/simple_git_versioning.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:32:54.169634 simple-git-versioning-0.1.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)      320 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:32:54.170634 simple-git-versioning-0.1.4/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)     7368 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    10566 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/test_pep440.py
--rw-rw-rw-   0 root         (0) root         (0)    14420 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/test_project.py
--rw-rw-rw-   0 root         (0) root         (0)     3196 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/test_semver2.py
--rw-rw-rw-   0 root         (0) root         (0)     3248 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/tests/unit/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:32:54.171634 simple-git-versioning-0.1.4/versioning/
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15269 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/pep440.py
--rw-rw-rw-   0 root         (0) root         (0)     7848 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/project.py
--rw-rw-rw-   0 root         (0) root         (0)     9062 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/semver2.py
--rw-rw-rw-   0 root         (0) root         (0)     2060 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/setuptools.py
--rw-rw-rw-   0 root         (0) root         (0)     1248 2023-07-10 21:32:40.000000 simple-git-versioning-0.1.4/versioning/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:56:08.007200 simple-git-versioning-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5099 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3883 2023-07-10 21:56:08.007200 simple-git-versioning-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    46416 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/Pipfile.lock
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 21:56:08.007200 simple-git-versioning-0.1.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:56:08.004200 simple-git-versioning-0.1.6/simple_git_versioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3883 2023-07-10 21:56:07.000000 simple-git-versioning-0.1.6/simple_git_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-10 21:56:07.000000 simple-git-versioning-0.1.6/simple_git_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 21:56:07.000000 simple-git-versioning-0.1.6/simple_git_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-10 21:56:07.000000 simple-git-versioning-0.1.6/simple_git_versioning.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-10 21:56:07.000000 simple-git-versioning-0.1.6/simple_git_versioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-10 21:56:07.000000 simple-git-versioning-0.1.6/simple_git_versioning.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:56:08.004200 simple-git-versioning-0.1.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      320 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:56:08.006200 simple-git-versioning-0.1.6/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)     7368 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/tests/unit/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    10566 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/tests/unit/test_pep440.py
+-rw-rw-rw-   0 root         (0) root         (0)    14420 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/tests/unit/test_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/tests/unit/test_semver2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/tests/unit/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:56:08.007200 simple-git-versioning-0.1.6/versioning/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/versioning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15269 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/versioning/pep440.py
+-rw-rw-rw-   0 root         (0) root         (0)     7848 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/versioning/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     9062 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/versioning/semver2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/versioning/setuptools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-07-10 21:55:53.000000 simple-git-versioning-0.1.6/versioning/version.py
```

### Comparing `simple-git-versioning-0.1.4/.gitlab-ci.yml` & `simple-git-versioning-0.1.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/.pre-commit-config.yaml` & `simple-git-versioning-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/LICENSE` & `simple-git-versioning-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/PKG-INFO` & `simple-git-versioning-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-git-versioning
-Version: 0.1.4
+Version: 0.1.6
 Summary: Thinly scoped and opinionated tool that computes a version number from git tags and trailers
 Author-email: Quentin Bouget <ypsah@devyard.org>
 License: MIT
 Project-URL: homepage, https://gitlab.com/ypsah/simple-git-versioning
 Project-URL: repository, https://gitlab.com/ypsah/simple-git-versioning
 Keywords: versioning,git,git-trailers
 Classifier: Development Status :: 3 - Alpha
@@ -65,23 +65,23 @@
 
 ## Libraries
 
 Libraries that wish to expose their version number programatically may do so by
 including the following snippet:
 
 ```python
-from importlib.metadata import version
+from importlib.metadata import PackageNotFoundError, version
 
 from versioning.pep440 import Project
 
 try:
     __version__ = version("simple-git-versioning")
 except PackageNotFoundError:
     # package is not installed
-    with _Project(path=Path(__file__).parent) as project:
+    with Project(path=Path(__file__).parent) as project:
         try:
             __version__ = str(project.version())
         except NoVersion:
             __version__ = str(project.release(dev=0))
 ```
 
 ## `setuptools`
```

### Comparing `simple-git-versioning-0.1.4/Pipfile.lock` & `simple-git-versioning-0.1.6/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/README.md` & `simple-git-versioning-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,23 +41,23 @@
 
 ## Libraries
 
 Libraries that wish to expose their version number programatically may do so by
 including the following snippet:
 
 ```python
-from importlib.metadata import version
+from importlib.metadata import PackageNotFoundError, version
 
 from versioning.pep440 import Project
 
 try:
     __version__ = version("simple-git-versioning")
 except PackageNotFoundError:
     # package is not installed
-    with _Project(path=Path(__file__).parent) as project:
+    with Project(path=Path(__file__).parent) as project:
         try:
             __version__ = str(project.version())
         except NoVersion:
             __version__ = str(project.release(dev=0))
 ```
 
 ## `setuptools`
```

### Comparing `simple-git-versioning-0.1.4/pyproject.toml` & `simple-git-versioning-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/simple_git_versioning.egg-info/PKG-INFO` & `simple-git-versioning-0.1.6/simple_git_versioning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-git-versioning
-Version: 0.1.4
+Version: 0.1.6
 Summary: Thinly scoped and opinionated tool that computes a version number from git tags and trailers
 Author-email: Quentin Bouget <ypsah@devyard.org>
 License: MIT
 Project-URL: homepage, https://gitlab.com/ypsah/simple-git-versioning
 Project-URL: repository, https://gitlab.com/ypsah/simple-git-versioning
 Keywords: versioning,git,git-trailers
 Classifier: Development Status :: 3 - Alpha
@@ -65,23 +65,23 @@
 
 ## Libraries
 
 Libraries that wish to expose their version number programatically may do so by
 including the following snippet:
 
 ```python
-from importlib.metadata import version
+from importlib.metadata import PackageNotFoundError, version
 
 from versioning.pep440 import Project
 
 try:
     __version__ = version("simple-git-versioning")
 except PackageNotFoundError:
     # package is not installed
-    with _Project(path=Path(__file__).parent) as project:
+    with Project(path=Path(__file__).parent) as project:
         try:
             __version__ = str(project.version())
         except NoVersion:
             __version__ = str(project.release(dev=0))
 ```
 
 ## `setuptools`
```

### Comparing `simple-git-versioning-0.1.4/simple_git_versioning.egg-info/SOURCES.txt` & `simple-git-versioning-0.1.6/simple_git_versioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/tests/unit/__init__.py` & `simple-git-versioning-0.1.6/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/tests/unit/test_cli.py` & `simple-git-versioning-0.1.6/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/tests/unit/test_pep440.py` & `simple-git-versioning-0.1.6/tests/unit/test_pep440.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/tests/unit/test_project.py` & `simple-git-versioning-0.1.6/tests/unit/test_project.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/tests/unit/test_semver2.py` & `simple-git-versioning-0.1.6/tests/unit/test_semver2.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/tests/unit/test_version.py` & `simple-git-versioning-0.1.6/tests/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/versioning/__init__.py` & `simple-git-versioning-0.1.6/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/versioning/pep440.py` & `simple-git-versioning-0.1.6/versioning/pep440.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/versioning/project.py` & `simple-git-versioning-0.1.6/versioning/project.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/versioning/semver2.py` & `simple-git-versioning-0.1.6/versioning/semver2.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/versioning/setuptools.py` & `simple-git-versioning-0.1.6/versioning/setuptools.py`

 * *Files identical despite different names*

### Comparing `simple-git-versioning-0.1.4/versioning/version.py` & `simple-git-versioning-0.1.6/versioning/version.py`

 * *Files identical despite different names*

