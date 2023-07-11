# Comparing `tmp/gpt4-api-0.2.2.tar.gz` & `tmp/gpt4-api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpt4-api-0.2.2.tar", last modified: Fri Jun 30 06:52:10 2023, max compression
+gzip compressed data, was "dist/gpt4-api-0.2.3.tar", last modified: Tue Jul 11 07:15:50 2023, max compression
```

## Comparing `gpt4-api-0.2.2.tar` & `gpt4-api-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)     1226 2023-06-20 07:10:40.000000 gpt4-api-0.2.2/api/Logger.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.2.2/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)    10236 2023-06-30 06:51:34.000000 gpt4-api-0.2.2/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      208 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/gpt4_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-06-30 06:52:10.000000 gpt4-api-0.2.2/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.2.2/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)     1226 2023-06-20 07:10:40.000000 gpt4-api-0.2.3/api/Logger.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt4-api-0.2.3/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)    10260 2023-07-11 07:15:22.000000 gpt4-api-0.2.3/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      300 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      208 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/gpt4_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-07-11 07:15:50.000000 gpt4-api-0.2.3/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      773 2023-05-30 06:52:15.000000 gpt4-api-0.2.3/setup.py
```

### Comparing `gpt4-api-0.2.2/api/Logger.py` & `gpt4-api-0.2.3/api/Logger.py`

 * *Files identical despite different names*

### Comparing `gpt4-api-0.2.2/api/gpt.py` & `gpt4-api-0.2.3/api/gpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
                 open_ai_key = token
                 break
             else:
                 logging.info("token: %s limit: %s" % (token, token_limit))
         return open_ai_key
 
     def __release_token(self, open_ai_key):
+        time.sleep(0.5)
         self.usable_openai_keys[open_ai_key] = 0
 
     @staticmethod
     def get_active_thread_count():
         return threading.active_count() - 1
 
     def task_is_empty(self):
```

### Comparing `gpt4-api-0.2.2/setup.py` & `gpt4-api-0.2.3/setup.py`

 * *Files identical despite different names*

