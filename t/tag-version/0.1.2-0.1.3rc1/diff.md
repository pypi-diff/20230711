# Comparing `tmp/tag-version-0.1.2.tar.gz` & `tmp/tag-version-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tag-version-0.1.2.tar", last modified: Thu Dec  3 19:32:44 2020, max compression
+gzip compressed data, was "dist/tag-version-0.1.3rc1.tar", last modified: Tue Jul 11 14:40:29 2023, max compression
```

## Comparing `tag-version-0.1.2.tar` & `tag-version-0.1.3rc1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-sr-x   0 root         (0) staff       (50)        0 2020-12-03 19:32:44.000000 tag-version-0.1.2/
--rwxr-xr-x   0 root         (0) staff       (50)      606 2020-12-03 19:32:44.000000 tag-version-0.1.2/setup.py
-drwxr-sr-x   0 root         (0) staff       (50)        0 2020-12-03 19:32:44.000000 tag-version-0.1.2/src/
-drwxr-sr-x   0 root         (0) staff       (50)        0 2020-12-03 19:32:44.000000 tag-version-0.1.2/src/tag_version.egg-info/
--rw-r--r--   0 root         (0) staff       (50)        3 2020-12-03 19:32:44.000000 tag-version-0.1.2/src/tag_version.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (50)       61 2020-12-03 19:32:44.000000 tag-version-0.1.2/src/tag_version.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (50)        1 2020-12-03 19:32:44.000000 tag-version-0.1.2/src/tag_version.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (50)       11 2020-12-03 19:32:44.000000 tag-version-0.1.2/src/tag_version.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (50)      439 2020-12-03 19:32:44.000000 tag-version-0.1.2/src/tag_version.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (50)      251 2020-12-03 19:32:44.000000 tag-version-0.1.2/src/tag_version.egg-info/PKG-INFO
-drwxr-sr-x   0 root         (0) staff       (50)        0 2020-12-03 19:32:44.000000 tag-version-0.1.2/src/tagversion/
--rw-r--r--   0 root         (0) staff       (50)     1834 2020-12-03 19:31:33.000000 tag-version-0.1.2/src/tagversion/write.py
--rw-r--r--   0 root         (0) staff       (50)      617 2020-12-03 19:31:33.000000 tag-version-0.1.2/src/tagversion/entrypoints.py
--rw-r--r--   0 root         (0) staff       (50)     6481 2020-12-03 19:31:33.000000 tag-version-0.1.2/src/tagversion/version.py
--rw-r--r--   0 root         (0) staff       (50)        0 2020-12-03 19:31:33.000000 tag-version-0.1.2/src/tagversion/__init__.py
--rw-r--r--   0 root         (0) staff       (50)    13716 2020-12-03 19:31:33.000000 tag-version-0.1.2/src/tagversion/git.py
--rw-r--r--   0 root         (0) staff       (50)      126 2020-12-03 19:31:33.000000 tag-version-0.1.2/src/tagversion/exceptions.py
--rw-r--r--   0 root         (0) staff       (50)     1709 2020-12-03 19:31:33.000000 tag-version-0.1.2/src/tagversion/argparse.py
--rw-r--r--   0 root         (0) staff       (50)     4911 2020-12-03 19:31:33.000000 tag-version-0.1.2/README.md
--rw-r--r--   0 root         (0) staff       (50)      251 2020-12-03 19:32:44.000000 tag-version-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (50)       38 2020-12-03 19:32:44.000000 tag-version-0.1.2/setup.cfg
+drwxr-sr-x   0 root         (0) staff       (50)        0 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/
+-rw-r--r--   0 root         (0) staff       (50)     5388 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/README.md
+-rw-r--r--   0 root         (0) staff       (50)       38 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/setup.cfg
+drwxr-sr-x   0 root         (0) staff       (50)        0 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/
+drwxr-sr-x   0 root         (0) staff       (50)        0 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/
+-rw-r--r--   0 root         (0) staff       (50)        1 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (50)      447 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (50)       61 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (50)      271 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (50)       11 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (50)       11 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tag_version.egg-info/requires.txt
+drwxr-sr-x   0 root         (0) staff       (50)        0 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/src/tagversion/
+-rw-r--r--   0 root         (0) staff       (50)      617 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/entrypoints.py
+-rw-r--r--   0 root         (0) staff       (50)        0 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/__init__.py
+-rw-r--r--   0 root         (0) staff       (50)     1709 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/argparse.py
+-rw-r--r--   0 root         (0) staff       (50)      126 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/exceptions.py
+-rw-r--r--   0 root         (0) staff       (50)    13650 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/git.py
+-rw-r--r--   0 root         (0) staff       (50)     1834 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/write.py
+-rw-r--r--   0 root         (0) staff       (50)     6481 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/src/tagversion/version.py
+-rw-r--r--   0 root         (0) staff       (50)      271 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/PKG-INFO
+-rwxr-xr-x   0 root         (0) staff       (50)      623 2023-07-11 14:40:29.000000 tag-version-0.1.3rc1/setup.py
+-rw-r--r--   0 root         (0) staff       (50)     1320 2023-07-11 14:39:54.000000 tag-version-0.1.3rc1/LICENSE
```

### Comparing `tag-version-0.1.2/setup.py` & `tag-version-0.1.3rc1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 SCRIPT_DIR = os.path.dirname(__file__)
 if not SCRIPT_DIR:
     SCRIPT_DIR = os.getcwd()
 
 
 setup(
     name="tag-version",
-    version="0.1.2",
+    version="0.1.3rc1",
     description="semantic versioned git tags",
-    author="OpenSlate",
-    author_email="code@openslate.com",
+    author="DoubleVerify",
+    author_email="code@doubleverify.com",
     url="https://github.com/openslate/tag-version",
     package_dir={"": "src"},
     packages=["tagversion"],
-    install_requires=["sh"],
+    install_requires=["sh==1.14.3"],
     entry_points={"console_scripts": ["tag-version = tagversion.entrypoints:main"]},
 )
```

### Comparing `tag-version-0.1.2/src/tagversion/write.py` & `tag-version-0.1.3rc1/src/tagversion/write.py`

 * *Files identical despite different names*

### Comparing `tag-version-0.1.2/src/tagversion/entrypoints.py` & `tag-version-0.1.3rc1/src/tagversion/entrypoints.py`

 * *Files identical despite different names*

### Comparing `tag-version-0.1.2/src/tagversion/version.py` & `tag-version-0.1.3rc1/src/tagversion/version.py`

 * *Files identical despite different names*

### Comparing `tag-version-0.1.2/src/tagversion/git.py` & `tag-version-0.1.3rc1/src/tagversion/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         return logging.getLogger("{}.{}".format(__name__, self.__class__.__name__))
 
     @property
     def branch(self):
         branch = os.environ.get("GIT_BRANCH")
         if branch is None:
             command = sh.git(*shlex.split("rev-parse --abbrev-ref HEAD"))
-            lines = command.stdout.decode("utf8").strip().splitlines()
+            lines = command.strip().splitlines()
             branch = lines[0].strip()
 
             # clean out control characters that may be present in `git` command output
             color_marker_idx = branch.find("\x1b")
             if color_marker_idx >= 0:
                 self.logger.warning(
                     "found color marker in branch={}".format(branch.encode("utf8"))
@@ -88,15 +88,15 @@
             is_tagged = False
 
         try:
             command = sh.git(*shlex.split("describe --tags --always"))
         except sh.ErrorReturnCode_128:  # pylint: disable=E1101
             pass
         else:
-            version_s = command.stdout.decode("utf8").strip()
+            version_s = command.strip()
 
             # if the branch flag was given,
             # check to see if we are on a tagged commit
             if self.args.branch and not is_tagged:
                 # this commit is not tagged directly, so append the branch
                 version_s = "{}-{}".format(version_s, self.branch)
 
@@ -113,15 +113,15 @@
             Boolean whether the working copy is clean
         """
         result = False
 
         command_l = "git status --untracked --short".split()
         command = getattr(sh, command_l[0])(command_l[1:])
 
-        lines = command.stdout.decode("utf8").splitlines()
+        lines = command.splitlines()
         for line in lines:
             line = line.rstrip()
             print_error("{}".format(line))
 
         if not lines:
             result = True
```

### Comparing `tag-version-0.1.2/src/tagversion/argparse.py` & `tag-version-0.1.3rc1/src/tagversion/argparse.py`

 * *Files identical despite different names*

### Comparing `tag-version-0.1.2/README.md` & `tag-version-0.1.3rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -160,7 +160,30 @@
 tag-version --bump --minor --rc
 # latest tag: 0.1.0-rc1
 tag-version --bump --rc
 # latest tag: 0.1.0-rc2
 tag-version --bump
 # latest tag: 0.1.0
 ```
+
+### Tag Version Development
+
+Development is done w/ Docker and `compose-flow`
+
+First you setup some default evn vars
+```compose-flow -e local env edit```
+
+```
+CF_ENV=local
+PYPI_PASSWORD=
+PYPI_USERNAME=
+```
+
+Then to build the container
+```compose-flow -e local compose build```
+
+Then to shell into the container
+```compose-flow -e local compose run --rm app /bin/bash```
+
+
+Testing can then be ran via pytest 
+```compose-flow -e local compose run --rm app /bin/bash -c pytest```
```

