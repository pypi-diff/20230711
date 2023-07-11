# Comparing `tmp/swiftly-unix-0.0.7.tar.gz` & `tmp/swiftly-unix-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.0.7.tar", last modified: Mon Jul 10 22:35:28 2023, max compression
+gzip compressed data, was "swiftly-unix-0.0.8.tar", last modified: Tue Jul 11 16:07:33 2023, max compression
```

## Comparing `swiftly-unix-0.0.7.tar` & `swiftly-unix-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 22:35:28.268061 swiftly-unix-0.0.7/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.7/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 22:35:28.267787 swiftly-unix-0.0.7/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 22:35:28.264909 swiftly-unix-0.0.7/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     2364 2023-07-10 22:29:40.000000 swiftly-unix-0.0.7/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 22:35:28.268115 swiftly-unix-0.0.7/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 22:33:44.000000 swiftly-unix-0.0.7/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 22:35:28.266628 swiftly-unix-0.0.7/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.7/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3097 2023-07-10 21:24:14.000000 swiftly-unix-0.0.7/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2154 2023-07-10 22:19:30.000000 swiftly-unix-0.0.7/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      522 2023-07-10 21:12:52.000000 swiftly-unix-0.0.7/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      335 2023-07-10 21:52:38.000000 swiftly-unix-0.0.7/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 22:35:28.267583 swiftly-unix-0.0.7/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 22:35:28.000000 swiftly-unix-0.0.7/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      295 2023-07-10 22:35:28.000000 swiftly-unix-0.0.7/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 22:35:28.000000 swiftly-unix-0.0.7/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-10 22:35:28.000000 swiftly-unix-0.0.7/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:07:33.177972 swiftly-unix-0.0.8/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.8/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-11 16:07:33.177834 swiftly-unix-0.0.8/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:07:33.175863 swiftly-unix-0.0.8/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     2533 2023-07-11 15:31:20.000000 swiftly-unix-0.0.8/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-11 16:07:33.178013 swiftly-unix-0.0.8/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-11 16:03:31.000000 swiftly-unix-0.0.8/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:07:33.177023 swiftly-unix-0.0.8/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.8/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3097 2023-07-10 21:24:14.000000 swiftly-unix-0.0.8/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2161 2023-07-11 15:27:32.000000 swiftly-unix-0.0.8/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      522 2023-07-10 21:12:52.000000 swiftly-unix-0.0.8/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      337 2023-07-11 15:36:13.000000 swiftly-unix-0.0.8/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-11 16:07:33.177646 swiftly-unix-0.0.8/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-11 16:07:33.000000 swiftly-unix-0.0.8/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      295 2023-07-11 16:07:33.000000 swiftly-unix-0.0.8/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-11 16:07:33.000000 swiftly-unix-0.0.8/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-11 16:07:33.000000 swiftly-unix-0.0.8/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.0.7/LICENSE` & `swiftly-unix-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.0.7/scripts/swiftly` & `swiftly-unix-0.0.8/scripts/swiftly`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/bin/bash
 
 function init(){
     if [ -z "$1" ]
     then
         fetch_remote=$(git fetch | tr '\n' ' ')
-        git_status=$(git status | tr '\n' ' ' | tr "'" '"' | sed 's/"/\\"/g')
+        git_status=$(git status -uno)
         pull_changes=$(python -c 'from swiftly_unix.init import pull_changes; print(pull_changes("'$git_status'"))')
         if [ "$pull_changes" = "True" ]
         then
             git pull
         fi
 
+
         venv_location=$(python -c 'from swiftly_unix.init import get_venv_location; print(get_venv_location())')
         source $venv_location/bin/activate
         export PROJECT_VENV_LOCATION=$venv_location
 
-        pip install --upgrade pip
-
         available_packages=$(pip freeze | tr '\n' ' ')
         new_packages=$(python -c "from swiftly_unix.init import check_new_packages; print(check_new_packages('$available_packages'))")
 
         if [ "$new_packages" = "True" ]
         then
             pip install -r requirements.txt
+            pip install --upgrade pip
+            install swiftly-unix
         fi
 
-        echo "Initialisation completed!"
     else
         is_github_repo=$(python -c "from swiftly_unix.init import is_repo; print(is_repo('$1'))")
         if [ "$is_github_repo" = "True" ]
         then
             git clone $1
         fi
 
@@ -37,24 +37,28 @@
         source $venv_location/bin/activate
         export PROJECT_VENV_LOCATION=$venv_location
 
         pip install --upgrade pip
         cd $venv_location
         cd ..
         pip install -r requirements.txt
-        echo "Initialisation completed!"
+        install swiftly-unix
     fi
+
+    project_name=$(python -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
+    export PROJECT_NAME=$project_name
+    echo "Initialisation completed!"
 }
 
 function makeapp(){
     python -c "from swiftly_unix.makeapp import makeapp; makeapp('$1')"
 }
 
 function run(){
-    path=$(python -c "from swiftly_unix.runapp import run_app; print(run_app('$1'))")
+    path=$(python -c "from swiftly_unix.runapp import run_app; print(run_app('$1', '$PROJECT_NAME', '$PROJECT_VENV_LOCATION'))")
     python -m $path
 }
 
 function install(){
     pip install $1
     updated_packages=$(pip freeze)
     requirements_path=$PROJECT_VENV_LOCATION/../requirements.txt
```

### Comparing `swiftly-unix-0.0.7/swiftly_unix/gitignore.py` & `swiftly-unix-0.0.8/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.0.7/swiftly_unix/init.py` & `swiftly-unix-0.0.8/swiftly_unix/init.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,23 +21,23 @@
                 f.write(GITIGNORE)
         with open('.gitignore', 'a') as f:
             f.write(f'\n{venv_name}/')
 
     venv_location = os.path.abspath(venv_name)
     return venv_location
 
-
+def get_project_name():
+    config = configparser.ConfigParser()
+    config.read('swiftly.config.py')
+    project_name = config.get('DEFAULT', 'PROJECT_NAME')
+    
+    return project_name
 
 def pull_changes(git_status):
-    not_to_pull = ["fatal: not a git repository", "Your branch is up to date with"]
-    
-    for i, message in enumerate(not_to_pull):
-        not_to_pull[i] = message in git_status
-        
-    return not (False in not_to_pull)
+    return 'Your branch is behind' in git_status
 
 def check_new_packages(available_packages):
     with open('requirements.txt', 'r') as f:
         required_packages = f.read().splitlines()
 
     available_packages = set(available_packages.split())
     required_packages = set(required_packages)
```

### Comparing `swiftly-unix-0.0.7/swiftly_unix/makeapp.py` & `swiftly-unix-0.0.8/swiftly_unix/makeapp.py`

 * *Files identical despite different names*

