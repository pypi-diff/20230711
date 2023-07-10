# Comparing `tmp/swiftly-unix-0.0.6.tar.gz` & `tmp/swiftly-unix-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.0.6.tar", last modified: Mon Jul 10 19:27:09 2023, max compression
+gzip compressed data, was "swiftly-unix-0.0.7.tar", last modified: Mon Jul 10 22:35:28 2023, max compression
```

## Comparing `swiftly-unix-0.0.6.tar` & `swiftly-unix-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:27:09.503290 swiftly-unix-0.0.6/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.6/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 19:27:09.503139 swiftly-unix-0.0.6/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:27:09.501169 swiftly-unix-0.0.6/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     1890 2023-07-10 19:25:05.000000 swiftly-unix-0.0.6/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 19:27:09.503336 swiftly-unix-0.0.6/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 19:26:59.000000 swiftly-unix-0.0.6/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:27:09.502312 swiftly-unix-0.0.6/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.6/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      695 2023-07-10 19:14:51.000000 swiftly-unix-0.0.6/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      291 2023-07-10 19:16:43.000000 swiftly-unix-0.0.6/swiftly_unix/installs.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      128 2023-07-10 19:15:27.000000 swiftly-unix-0.0.6/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      148 2023-07-10 19:15:55.000000 swiftly-unix-0.0.6/swiftly_unix/run_app.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 19:27:09.502913 swiftly-unix-0.0.6/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 19:27:09.000000 swiftly-unix-0.0.6/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      295 2023-07-10 19:27:09.000000 swiftly-unix-0.0.6/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 19:27:09.000000 swiftly-unix-0.0.6/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-10 19:27:09.000000 swiftly-unix-0.0.6/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 22:35:28.268061 swiftly-unix-0.0.7/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.0.7/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 22:35:28.267787 swiftly-unix-0.0.7/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 22:35:28.264909 swiftly-unix-0.0.7/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     2364 2023-07-10 22:29:40.000000 swiftly-unix-0.0.7/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-10 22:35:28.268115 swiftly-unix-0.0.7/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      162 2023-07-10 22:33:44.000000 swiftly-unix-0.0.7/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 22:35:28.266628 swiftly-unix-0.0.7/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.0.7/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3097 2023-07-10 21:24:14.000000 swiftly-unix-0.0.7/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2154 2023-07-10 22:19:30.000000 swiftly-unix-0.0.7/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      522 2023-07-10 21:12:52.000000 swiftly-unix-0.0.7/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      335 2023-07-10 21:52:38.000000 swiftly-unix-0.0.7/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-10 22:35:28.267583 swiftly-unix-0.0.7/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       78 2023-07-10 22:35:28.000000 swiftly-unix-0.0.7/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      295 2023-07-10 22:35:28.000000 swiftly-unix-0.0.7/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-10 22:35:28.000000 swiftly-unix-0.0.7/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-10 22:35:28.000000 swiftly-unix-0.0.7/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.0.6/LICENSE` & `swiftly-unix-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.0.6/scripts/swiftly` & `swiftly-unix-0.0.7/scripts/swiftly`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #!/bin/bash
 
 function init(){
     if [ -z "$1" ]
     then
-        pull_changes=$(python -c 'from swiftly_unix.init import pull_changes; print(pull_changes())')
+        fetch_remote=$(git fetch | tr '\n' ' ')
+        git_status=$(git status | tr '\n' ' ' | tr "'" '"' | sed 's/"/\\"/g')
+        pull_changes=$(python -c 'from swiftly_unix.init import pull_changes; print(pull_changes("'$git_status'"))')
         if [ "$pull_changes" = "True" ]
         then
             git pull
         fi
 
         venv_location=$(python -c 'from swiftly_unix.init import get_venv_location; print(get_venv_location())')
         source $venv_location/bin/activate
+        export PROJECT_VENV_LOCATION=$venv_location
 
-        available_packages=$(pip freeze | tr '\n' ' ')
+        pip install --upgrade pip
 
+        available_packages=$(pip freeze | tr '\n' ' ')
         new_packages=$(python -c "from swiftly_unix.init import check_new_packages; print(check_new_packages('$available_packages'))")
 
         if [ "$new_packages" = "True" ]
         then
             pip install -r requirements.txt
         fi
 
@@ -27,36 +31,45 @@
         if [ "$is_github_repo" = "True" ]
         then
             git clone $1
         fi
 
         venv_location=$(python -c "from swiftly_unix.init import initialise; print(initialise('$1'))")
         source $venv_location/bin/activate
+        export PROJECT_VENV_LOCATION=$venv_location
+
+        pip install --upgrade pip
+        cd $venv_location
+        cd ..
         pip install -r requirements.txt
         echo "Initialisation completed!"
     fi
 }
 
 function makeapp(){
     python -c "from swiftly_unix.makeapp import makeapp; makeapp('$1')"
 }
 
 function run(){
-    path=$(python -c "from swiftly_unix.run_app import run_app; print(run_app('$1'))")
-    python $path
+    path=$(python -c "from swiftly_unix.runapp import run_app; print(run_app('$1'))")
+    python -m $path
 }
 
 function install(){
     pip install $1
-    python -c "from swiftly_unix.installs import install_package; install_package('$1')"
+    updated_packages=$(pip freeze)
+    requirements_path=$PROJECT_VENV_LOCATION/../requirements.txt
+    echo "$updated_packages" > $requirements_path
 }
 
 function uninstall(){
     pip uninstall $1
-    python -c "from swiftly_unix.installs import uninstall_package; uninstall_package('$1')"
+    updated_packages=$(pip freeze)
+    requirements_path=$PROJECT_VENV_LOCATION/../requirements.txt
+    echo "$updated_packages" > $requirements_path
 }
 
 if [ "$1" = "init" ]
 then
     init $2
 elif [ "$1" = "makeapp" ]
 then
```

