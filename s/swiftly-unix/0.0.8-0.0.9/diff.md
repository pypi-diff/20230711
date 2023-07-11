# Comparing `tmp/swiftly-unix-0.0.8.tar.gz` & `tmp/swiftly-unix-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.0.8.tar", last modified: Tue Jul 11 16:07:33 2023, max compression
+gzip compressed data, was "swiftly-unix-0.0.9.tar", last modified: Tue Jul 11 16:37:08 2023, max compression
```

## Comparing `swiftly-unix-0.0.8.tar` & `swiftly-unix-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:07:33.177972 swiftly-unix-0.0.8/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.8/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-11 16:07:33.177834 swiftly-unix-0.0.8/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:07:33.175863 swiftly-unix-0.0.8/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     2533 2023-07-11 15:31:20.000000 swiftly-unix-0.0.8/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-11 16:07:33.178013 swiftly-unix-0.0.8/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-11 16:03:31.000000 swiftly-unix-0.0.8/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:07:33.177023 swiftly-unix-0.0.8/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.8/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3097 2023-07-10 21:24:14.000000 swiftly-unix-0.0.8/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2161 2023-07-11 15:27:32.000000 swiftly-unix-0.0.8/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      522 2023-07-10 21:12:52.000000 swiftly-unix-0.0.8/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      337 2023-07-11 15:36:13.000000 swiftly-unix-0.0.8/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:07:33.177646 swiftly-unix-0.0.8/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-11 16:07:33.000000 swiftly-unix-0.0.8/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      295 2023-07-11 16:07:33.000000 swiftly-unix-0.0.8/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-11 16:07:33.000000 swiftly-unix-0.0.8/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-11 16:07:33.000000 swiftly-unix-0.0.8/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:37:08.730257 swiftly-unix-0.0.9/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.9/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-11 16:37:08.730116 swiftly-unix-0.0.9/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:37:08.728075 swiftly-unix-0.0.9/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     2727 2023-07-11 16:28:53.000000 swiftly-unix-0.0.9/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-11 16:37:08.730301 swiftly-unix-0.0.9/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-11 16:36:56.000000 swiftly-unix-0.0.9/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:37:08.729312 swiftly-unix-0.0.9/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.9/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3097 2023-07-10 21:24:14.000000 swiftly-unix-0.0.9/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2161 2023-07-11 15:27:32.000000 swiftly-unix-0.0.9/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      522 2023-07-10 21:12:52.000000 swiftly-unix-0.0.9/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      337 2023-07-11 15:36:13.000000 swiftly-unix-0.0.9/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:37:08.729956 swiftly-unix-0.0.9/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-11 16:37:08.000000 swiftly-unix-0.0.9/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      295 2023-07-11 16:37:08.000000 swiftly-unix-0.0.9/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-11 16:37:08.000000 swiftly-unix-0.0.9/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-11 16:37:08.000000 swiftly-unix-0.0.9/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.0.8/LICENSE` & `swiftly-unix-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.0.8/scripts/swiftly` & `swiftly-unix-0.0.9/scripts/swiftly`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/bin/bash
 
 function init(){
     if [ -z "$1" ]
     then
         fetch_remote=$(git fetch | tr '\n' ' ')
-        git_status=$(git status -uno)
+        git_status=$(git status -uno | tr '\n' ' ' | sed 's/"/\\"/g')
         pull_changes=$(python -c 'from swiftly_unix.init import pull_changes; print(pull_changes("'$git_status'"))')
         if [ "$pull_changes" = "True" ]
         then
             git pull
         fi
 
 
@@ -22,14 +22,17 @@
         if [ "$new_packages" = "True" ]
         then
             pip install -r requirements.txt
             pip install --upgrade pip
             install swiftly-unix
         fi
 
+        project_name=$(python -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
+        export PROJECT_NAME=$project_name
+
     else
         is_github_repo=$(python -c "from swiftly_unix.init import is_repo; print(is_repo('$1'))")
         if [ "$is_github_repo" = "True" ]
         then
             git clone $1
         fi
 
@@ -38,18 +41,19 @@
         export PROJECT_VENV_LOCATION=$venv_location
 
         pip install --upgrade pip
         cd $venv_location
         cd ..
         pip install -r requirements.txt
         install swiftly-unix
+
+        project_name=$(python -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
+        export PROJECT_NAME=$project_name
     fi
 
-    project_name=$(python -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
-    export PROJECT_NAME=$project_name
     echo "Initialisation completed!"
 }
 
 function makeapp(){
     python -c "from swiftly_unix.makeapp import makeapp; makeapp('$1')"
 }
```

### Comparing `swiftly-unix-0.0.8/swiftly_unix/gitignore.py` & `swiftly-unix-0.0.9/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.0.8/swiftly_unix/init.py` & `swiftly-unix-0.0.9/swiftly_unix/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.0.8/swiftly_unix/makeapp.py` & `swiftly-unix-0.0.9/swiftly_unix/makeapp.py`

 * *Files identical despite different names*

