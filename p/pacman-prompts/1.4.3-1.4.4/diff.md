# Comparing `tmp/pacman-prompts-1.4.3.tar.gz` & `tmp/pacman-prompts-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacman-prompts-1.4.3.tar", last modified: Sat Jul  8 23:49:32 2023, max compression
+gzip compressed data, was "pacman-prompts-1.4.4.tar", last modified: Tue Jul 11 18:39:14 2023, max compression
```

## Comparing `pacman-prompts-1.4.3.tar` & `pacman-prompts-1.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-08 23:49:32.736074 pacman-prompts-1.4.3/
--rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-07-08 23:49:32.735922 pacman-prompts-1.4.3/PKG-INFO
--rw-r--r--   0 anishthite   (501) staff       (20)     2044 2023-03-27 18:03:15.000000 pacman-prompts-1.4.3/README.md
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-08 23:49:32.734640 pacman-prompts-1.4.3/pacman/
--rw-r--r--   0 anishthite   (501) staff       (20)       56 2023-03-15 16:30:00.000000 pacman-prompts-1.4.3/pacman/__init__.py
--rw-r--r--   0 anishthite   (501) staff       (20)      121 2023-03-17 18:53:13.000000 pacman-prompts-1.4.3/pacman/file_utils.py
--rw-r--r--   0 anishthite   (501) staff       (20)      637 2023-04-25 19:15:29.000000 pacman-prompts-1.4.3/pacman/pacman.py
--rw-r--r--   0 anishthite   (501) staff       (20)     3324 2023-07-08 20:49:58.000000 pacman-prompts-1.4.3/pacman/prompt.py
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-08 23:49:32.735713 pacman-prompts-1.4.3/pacman_prompts.egg-info/
--rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-07-08 23:49:32.000000 pacman-prompts-1.4.3/pacman_prompts.egg-info/PKG-INFO
--rw-r--r--   0 anishthite   (501) staff       (20)      281 2023-07-08 23:49:32.000000 pacman-prompts-1.4.3/pacman_prompts.egg-info/SOURCES.txt
--rw-r--r--   0 anishthite   (501) staff       (20)        1 2023-07-08 23:49:32.000000 pacman-prompts-1.4.3/pacman_prompts.egg-info/dependency_links.txt
--rw-r--r--   0 anishthite   (501) staff       (20)       35 2023-07-08 23:49:32.000000 pacman-prompts-1.4.3/pacman_prompts.egg-info/requires.txt
--rw-r--r--   0 anishthite   (501) staff       (20)        7 2023-07-08 23:49:32.000000 pacman-prompts-1.4.3/pacman_prompts.egg-info/top_level.txt
--rw-r--r--   0 anishthite   (501) staff       (20)       38 2023-07-08 23:49:32.736115 pacman-prompts-1.4.3/setup.cfg
--rw-r--r--   0 anishthite   (501) staff       (20)      866 2023-07-08 23:48:48.000000 pacman-prompts-1.4.3/setup.py
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-11 18:39:14.054155 pacman-prompts-1.4.4/
+-rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-07-11 18:39:14.053985 pacman-prompts-1.4.4/PKG-INFO
+-rw-r--r--   0 anishthite   (501) staff       (20)     2044 2023-03-27 18:03:15.000000 pacman-prompts-1.4.4/README.md
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-11 18:39:14.053026 pacman-prompts-1.4.4/pacman/
+-rw-r--r--   0 anishthite   (501) staff       (20)       56 2023-03-15 16:30:00.000000 pacman-prompts-1.4.4/pacman/__init__.py
+-rw-r--r--   0 anishthite   (501) staff       (20)      121 2023-03-17 18:53:13.000000 pacman-prompts-1.4.4/pacman/file_utils.py
+-rw-r--r--   0 anishthite   (501) staff       (20)      637 2023-04-25 19:15:29.000000 pacman-prompts-1.4.4/pacman/pacman.py
+-rw-r--r--   0 anishthite   (501) staff       (20)     3319 2023-07-09 00:33:44.000000 pacman-prompts-1.4.4/pacman/prompt.py
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2023-07-11 18:39:14.053800 pacman-prompts-1.4.4/pacman_prompts.egg-info/
+-rw-r--r--   0 anishthite   (501) staff       (20)      575 2023-07-11 18:39:14.000000 pacman-prompts-1.4.4/pacman_prompts.egg-info/PKG-INFO
+-rw-r--r--   0 anishthite   (501) staff       (20)      281 2023-07-11 18:39:14.000000 pacman-prompts-1.4.4/pacman_prompts.egg-info/SOURCES.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)        1 2023-07-11 18:39:14.000000 pacman-prompts-1.4.4/pacman_prompts.egg-info/dependency_links.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)       43 2023-07-11 18:39:14.000000 pacman-prompts-1.4.4/pacman_prompts.egg-info/requires.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)        7 2023-07-11 18:39:14.000000 pacman-prompts-1.4.4/pacman_prompts.egg-info/top_level.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)       38 2023-07-11 18:39:14.054237 pacman-prompts-1.4.4/setup.cfg
+-rw-r--r--   0 anishthite   (501) staff       (20)      883 2023-07-11 18:39:04.000000 pacman-prompts-1.4.4/setup.py
```

### Comparing `pacman-prompts-1.4.3/PKG-INFO` & `pacman-prompts-1.4.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pacman-prompts
-Version: 1.4.3
+Version: 1.4.4
 Summary: Prompts As Code, man
 Home-page: https://github.com/anishthite/pacman
 Author: Anish Thite
 Author-email: anishthite@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pacman-prompts-1.4.3/README.md` & `pacman-prompts-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pacman-prompts-1.4.3/pacman/pacman.py` & `pacman-prompts-1.4.4/pacman/pacman.py`

 * *Files identical despite different names*

### Comparing `pacman-prompts-1.4.3/pacman/prompt.py` & `pacman-prompts-1.4.4/pacman/prompt.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 openai.api_key = os.getenv('OPENAI_API_KEY')
 if openai.api_key is None:
     raise Exception("OpenAI API key not set")
 
 openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create,
     user_email='claros@claros.com',
-    queue_requests=True,
-    model_limits_dir = {"gpt-3.5-turbo-0613": {"max_token_capacity": 90000, "max_request_capacity": 3500}},
-    fallback_strategy=['gpt-3.5-turbo-0613', 'gpt-3.5-turbo-0613', 'gpt-3.5-turbo', 'gpt-3.5-turbo-16k'])
+    #model_limits_dir = {"gpt-3.5-turbo-0613": {"max_token_capacity": 90000, "max_request_capacity": 3500}},
+    fallback_strategy=['gpt-3.5-turbo-0613', 'gpt-3.5-turbo-0613', 'gpt-3.5-turbo', 'gpt-3.5-turbo-16k'],
+    caching=False)
 
 class PromptConfig:
     def __init__(self, config):
         #set attributes from config
         for name, value in config.items():
             setattr(self, name, value)
```

### Comparing `pacman-prompts-1.4.3/pacman_prompts.egg-info/PKG-INFO` & `pacman-prompts-1.4.4/pacman_prompts.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pacman-prompts
-Version: 1.4.3
+Version: 1.4.4
 Summary: Prompts As Code, man
 Home-page: https://github.com/anishthite/pacman
 Author: Anish Thite
 Author-email: anishthite@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pacman-prompts-1.4.3/setup.py` & `pacman-prompts-1.4.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'pacman-prompts',
   packages = find_packages(exclude=['examples']),
-  version = '1.4.3',
+  version = '1.4.4',
   license='MIT',
   description = 'Prompts As Code, man',
   long_description_content_type = 'text/markdown',
   author = 'Anish Thite',
   author_email = 'anishthite@gmail.com',
   url = 'https://github.com/anishthite/pacman',
   keywords = [
     'artificial intelligence',
     'attention mechanism',
     'image recognition'
   ],
   install_requires=[
       'pyyaml',
       'openai',
-      'reliableGPT==0.2.976'
+      'reliableGPT==0.2.981',
+      'posthog'
   ],
   setup_requires=[
   ],
   tests_require=[
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
```

