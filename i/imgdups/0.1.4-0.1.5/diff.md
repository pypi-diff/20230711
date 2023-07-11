# Comparing `tmp/imgdups-0.1.4.tar.gz` & `tmp/imgdups-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgdups-0.1.4.tar", last modified: Sun Jul  9 21:13:43 2023, max compression
+gzip compressed data, was "imgdups-0.1.5.tar", last modified: Tue Jul 11 15:18:08 2023, max compression
```

## Comparing `imgdups-0.1.4.tar` & `imgdups-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 21:13:43.044994 imgdups-0.1.4/
--rw-rw-r--   0 nice      (1000) nice      (1000)    35149 2023-07-03 20:54:00.000000 imgdups-0.1.4/LICENSE
--rw-rw-r--   0 nice      (1000) nice      (1000)     2484 2023-07-09 21:13:43.044994 imgdups-0.1.4/PKG-INFO
--rw-r--r--   0 nice      (1000) nice      (1000)     1508 2023-07-04 17:37:18.000000 imgdups-0.1.4/README.md
-drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 21:13:43.040994 imgdups-0.1.4/imgdups/
--rw-rw-r--   0 nice      (1000) nice      (1000)      114 2023-07-04 16:54:42.000000 imgdups-0.1.4/imgdups/__init__.py
--rwxrwxr-x   0 nice      (1000) nice      (1000)    11418 2023-07-09 20:37:54.000000 imgdups-0.1.4/imgdups/imgdups.py
-drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 21:13:43.040994 imgdups-0.1.4/imgdups.egg-info/
--rw-rw-r--   0 nice      (1000) nice      (1000)     2484 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/PKG-INFO
--rw-rw-r--   0 nice      (1000) nice      (1000)      316 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/SOURCES.txt
--rw-rw-r--   0 nice      (1000) nice      (1000)        1 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/dependency_links.txt
--rw-rw-r--   0 nice      (1000) nice      (1000)       49 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/entry_points.txt
--rw-rw-r--   0 nice      (1000) nice      (1000)       20 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/requires.txt
--rw-rw-r--   0 nice      (1000) nice      (1000)        8 2023-07-09 21:13:43.000000 imgdups-0.1.4/imgdups.egg-info/top_level.txt
--rw-rw-r--   0 nice      (1000) nice      (1000)        1 2023-07-04 16:37:56.000000 imgdups-0.1.4/imgdups.egg-info/zip-safe
--rw-rw-r--   0 nice      (1000) nice      (1000)       82 2023-07-03 21:28:15.000000 imgdups-0.1.4/pyproject.toml
--rw-rw-r--   0 nice      (1000) nice      (1000)       38 2023-07-09 21:13:43.044994 imgdups-0.1.4/setup.cfg
--rw-rw-r--   0 nice      (1000) nice      (1000)     1613 2023-07-09 20:21:25.000000 imgdups-0.1.4/setup.py
-drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-09 21:13:43.044994 imgdups-0.1.4/tests/
--rw-rw-r--   0 nice      (1000) nice      (1000)      166 2023-07-04 17:05:07.000000 imgdups-0.1.4/tests/test_imgdups.py
+drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-11 15:18:08.688451 imgdups-0.1.5/
+-rw-rw-r--   0 nice      (1000) nice      (1000)    35149 2023-07-03 20:54:00.000000 imgdups-0.1.5/LICENSE
+-rw-rw-r--   0 nice      (1000) nice      (1000)     2484 2023-07-11 15:18:08.688451 imgdups-0.1.5/PKG-INFO
+-rw-r--r--   0 nice      (1000) nice      (1000)     1508 2023-07-04 17:37:18.000000 imgdups-0.1.5/README.md
+drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-11 15:18:08.688451 imgdups-0.1.5/imgdups/
+-rw-rw-r--   0 nice      (1000) nice      (1000)      114 2023-07-04 16:54:42.000000 imgdups-0.1.5/imgdups/__init__.py
+-rwxrwxr-x   0 nice      (1000) nice      (1000)    11811 2023-07-11 15:16:53.000000 imgdups-0.1.5/imgdups/imgdups.py
+drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-11 15:18:08.688451 imgdups-0.1.5/imgdups.egg-info/
+-rw-rw-r--   0 nice      (1000) nice      (1000)     2484 2023-07-11 15:18:08.000000 imgdups-0.1.5/imgdups.egg-info/PKG-INFO
+-rw-rw-r--   0 nice      (1000) nice      (1000)      316 2023-07-11 15:18:08.000000 imgdups-0.1.5/imgdups.egg-info/SOURCES.txt
+-rw-rw-r--   0 nice      (1000) nice      (1000)        1 2023-07-11 15:18:08.000000 imgdups-0.1.5/imgdups.egg-info/dependency_links.txt
+-rw-rw-r--   0 nice      (1000) nice      (1000)       49 2023-07-11 15:18:08.000000 imgdups-0.1.5/imgdups.egg-info/entry_points.txt
+-rw-rw-r--   0 nice      (1000) nice      (1000)       20 2023-07-11 15:18:08.000000 imgdups-0.1.5/imgdups.egg-info/requires.txt
+-rw-rw-r--   0 nice      (1000) nice      (1000)        8 2023-07-11 15:18:08.000000 imgdups-0.1.5/imgdups.egg-info/top_level.txt
+-rw-rw-r--   0 nice      (1000) nice      (1000)        1 2023-07-04 16:37:56.000000 imgdups-0.1.5/imgdups.egg-info/zip-safe
+-rw-rw-r--   0 nice      (1000) nice      (1000)       82 2023-07-03 21:28:15.000000 imgdups-0.1.5/pyproject.toml
+-rw-rw-r--   0 nice      (1000) nice      (1000)       38 2023-07-11 15:18:08.688451 imgdups-0.1.5/setup.cfg
+-rw-rw-r--   0 nice      (1000) nice      (1000)     1613 2023-07-11 15:14:50.000000 imgdups-0.1.5/setup.py
+drwxrwxr-x   0 nice      (1000) nice      (1000)        0 2023-07-11 15:18:08.688451 imgdups-0.1.5/tests/
+-rw-rw-r--   0 nice      (1000) nice      (1000)      166 2023-07-04 17:05:07.000000 imgdups-0.1.5/tests/test_imgdups.py
```

### Comparing `imgdups-0.1.4/LICENSE` & `imgdups-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `imgdups-0.1.4/PKG-INFO` & `imgdups-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgdups
-Version: 0.1.4
+Version: 0.1.5
 Summary: Very fast two folder image duplicate finder programmed with pickle and cv2
 Home-page: https://github.com/ChuckNorrison/imgdups/
 Author: Chuck Norrison
 Author-email: itsmells@yourshorts.club
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `imgdups-0.1.4/README.md` & `imgdups-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `imgdups-0.1.4/imgdups/imgdups.py` & `imgdups-0.1.5/imgdups/imgdups.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,29 @@
     """check pickle folder existence"""
     pickle_folder = os.path.join(path, "imgdups")
     if not os.path.exists(pickle_folder):
         os.makedirs(pickle_folder)
 
     return pickle_folder
 
+def validate_file_extension(file):
+    """Check valid image file extensions"""
+    validate = False
+    if file.lower().endswith(('.jpg', '.png', 'jpeg', '.bmp')):
+        validate = True
+
+    return validate
+
 def get_files_from_path(path):
     """walk through directory and return files list"""
-    files = [f for f in os.listdir(path)
-        if os.path.isfile(os.path.join(path, f))]
+    files = []
+    for file in os.listdir(path):
+        if ( os.path.isfile(os.path.join(path, file))
+                and validate_file_extension(file) ):
+            files.append(file)
 
     return files
 
 def scale_image(image):
     """scale image temporary for comparison"""
     if np.shape(image) != (500, 500, 1):
         image = cv2.resize(image, (500, 500))
@@ -174,15 +185,17 @@
         self.image_processed, self.image_cache = load_cache_index(pickle_file)
         self.image_processed, self.image_cache = rebuild_cache_index(path, self.image_cache)
 
         index_check = False
 
         files = get_files_from_path(path)
         for file in files:
-            if "imgdups" in file or "thumb" in file:
+            # skip folder imgdups and thumb files
+            if ( "imgdups" in file
+                    or "thumb" in file ):
                 continue
 
             image_path = os.path.join(path, file)
             if not file in self.image_processed:
                 descriptors = get_descriptors(image_path)
                 self.image_cache.append((image_path, descriptors))
                 self.image_processed.append(file)
```

### Comparing `imgdups-0.1.4/imgdups.egg-info/PKG-INFO` & `imgdups-0.1.5/imgdups.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgdups
-Version: 0.1.4
+Version: 0.1.5
 Summary: Very fast two folder image duplicate finder programmed with pickle and cv2
 Home-page: https://github.com/ChuckNorrison/imgdups/
 Author: Chuck Norrison
 Author-email: itsmells@yourshorts.club
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `imgdups-0.1.4/setup.py` & `imgdups-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 test_requirements = [
     'pylint',
     'pytest',
 ]
 
 setup(
     name='imgdups',
-    version='0.1.4',
+    version='0.1.5',
     description="Very fast two folder image duplicate finder programmed with pickle and cv2",
     long_description=readme,
     long_description_content_type = 'text/markdown',
     author="Chuck Norrison",
     author_email='itsmells@yourshorts.club',
     url='https://github.com/ChuckNorrison/imgdups/',
     packages=['imgdups'],
```

