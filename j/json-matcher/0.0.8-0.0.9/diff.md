# Comparing `tmp/json_matcher-0.0.8.tar.gz` & `tmp/json_matcher-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json_matcher-0.0.8.tar", last modified: Wed Nov 23 06:59:43 2022, max compression
+gzip compressed data, was "dist/json_matcher-0.0.9.tar", last modified: Thu Dec 22 06:17:41 2022, max compression
```

## Comparing `json_matcher-0.0.8.tar` & `json_matcher-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 blackmir   (502) staff       (20)        0 2022-11-23 06:59:43.000000 json_matcher-0.0.8/
--rw-r--r--   0 blackmir   (502) staff       (20)     1023 2019-10-15 02:31:07.000000 json_matcher-0.0.8/LICENSE
--rw-r--r--   0 blackmir   (502) staff       (20)     2426 2022-11-23 06:59:43.000000 json_matcher-0.0.8/PKG-INFO
--rw-r--r--   0 blackmir   (502) staff       (20)     1509 2019-10-15 06:37:36.000000 json_matcher-0.0.8/README.md
-drwxr-xr-x   0 blackmir   (502) staff       (20)        0 2022-11-23 06:59:43.000000 json_matcher-0.0.8/bin/
--rwxr-xr-x   0 blackmir   (502) staff       (20)     1821 2019-10-08 09:40:45.000000 json_matcher-0.0.8/bin/jrep
--rwxr-xr-x   0 blackmir   (502) staff       (20)     1821 2019-10-08 09:40:45.000000 json_matcher-0.0.8/bin/json_match
-drwxr-xr-x   0 blackmir   (502) staff       (20)        0 2022-11-23 06:59:43.000000 json_matcher-0.0.8/json_matcher/
--rw-r--r--   0 blackmir   (502) staff       (20)      181 2022-09-02 02:16:10.000000 json_matcher-0.0.8/json_matcher/__init__.py
--rw-r--r--   0 blackmir   (502) staff       (20)    18732 2022-11-23 06:55:48.000000 json_matcher-0.0.8/json_matcher/json_matcher.py
--rw-r--r--   0 blackmir   (502) staff       (20)     6939 2022-11-23 06:44:26.000000 json_matcher-0.0.8/json_matcher/match_environ.py
-drwxr-xr-x   0 blackmir   (502) staff       (20)        0 2022-11-23 06:59:43.000000 json_matcher-0.0.8/json_matcher.egg-info/
--rw-r--r--   0 blackmir   (502) staff       (20)     2426 2022-11-23 06:59:43.000000 json_matcher-0.0.8/json_matcher.egg-info/PKG-INFO
--rw-r--r--   0 blackmir   (502) staff       (20)      323 2022-11-23 06:59:43.000000 json_matcher-0.0.8/json_matcher.egg-info/SOURCES.txt
--rw-r--r--   0 blackmir   (502) staff       (20)        1 2022-11-23 06:59:43.000000 json_matcher-0.0.8/json_matcher.egg-info/dependency_links.txt
--rw-r--r--   0 blackmir   (502) staff       (20)       21 2022-11-23 06:59:43.000000 json_matcher-0.0.8/json_matcher.egg-info/requires.txt
--rw-r--r--   0 blackmir   (502) staff       (20)       13 2022-11-23 06:59:43.000000 json_matcher-0.0.8/json_matcher.egg-info/top_level.txt
--rw-r--r--   0 blackmir   (502) staff       (20)      102 2022-11-23 06:59:43.000000 json_matcher-0.0.8/setup.cfg
--rw-r--r--   0 blackmir   (502) staff       (20)     1071 2022-11-23 06:56:40.000000 json_matcher-0.0.8/setup.py
+drwxr-xr-x   0 blackmir   (502) staff       (20)        0 2022-12-22 06:17:41.000000 json_matcher-0.0.9/
+-rw-r--r--   0 blackmir   (502) staff       (20)     1023 2019-10-15 02:31:07.000000 json_matcher-0.0.9/LICENSE
+-rw-r--r--   0 blackmir   (502) staff       (20)     2426 2022-12-22 06:17:41.000000 json_matcher-0.0.9/PKG-INFO
+-rw-r--r--   0 blackmir   (502) staff       (20)     1509 2019-10-15 06:37:36.000000 json_matcher-0.0.9/README.md
+drwxr-xr-x   0 blackmir   (502) staff       (20)        0 2022-12-22 06:17:41.000000 json_matcher-0.0.9/bin/
+-rwxr-xr-x   0 blackmir   (502) staff       (20)     1821 2019-10-08 09:40:45.000000 json_matcher-0.0.9/bin/jrep
+-rwxr-xr-x   0 blackmir   (502) staff       (20)     1821 2019-10-08 09:40:45.000000 json_matcher-0.0.9/bin/json_match
+drwxr-xr-x   0 blackmir   (502) staff       (20)        0 2022-12-22 06:17:41.000000 json_matcher-0.0.9/json_matcher/
+-rw-r--r--   0 blackmir   (502) staff       (20)      181 2022-09-02 02:16:10.000000 json_matcher-0.0.9/json_matcher/__init__.py
+-rw-r--r--   0 blackmir   (502) staff       (20)    18732 2022-12-22 06:03:21.000000 json_matcher-0.0.9/json_matcher/json_matcher.py
+-rw-r--r--   0 blackmir   (502) staff       (20)     6917 2022-12-09 14:35:46.000000 json_matcher-0.0.9/json_matcher/match_environ.py
+drwxr-xr-x   0 blackmir   (502) staff       (20)        0 2022-12-22 06:17:41.000000 json_matcher-0.0.9/json_matcher.egg-info/
+-rw-r--r--   0 blackmir   (502) staff       (20)     2426 2022-12-22 06:17:41.000000 json_matcher-0.0.9/json_matcher.egg-info/PKG-INFO
+-rw-r--r--   0 blackmir   (502) staff       (20)      323 2022-12-22 06:17:41.000000 json_matcher-0.0.9/json_matcher.egg-info/SOURCES.txt
+-rw-r--r--   0 blackmir   (502) staff       (20)        1 2022-12-22 06:17:41.000000 json_matcher-0.0.9/json_matcher.egg-info/dependency_links.txt
+-rw-r--r--   0 blackmir   (502) staff       (20)       21 2022-12-22 06:17:41.000000 json_matcher-0.0.9/json_matcher.egg-info/requires.txt
+-rw-r--r--   0 blackmir   (502) staff       (20)       13 2022-12-22 06:17:41.000000 json_matcher-0.0.9/json_matcher.egg-info/top_level.txt
+-rw-r--r--   0 blackmir   (502) staff       (20)      102 2022-12-22 06:17:41.000000 json_matcher-0.0.9/setup.cfg
+-rw-r--r--   0 blackmir   (502) staff       (20)     1071 2022-12-22 06:15:51.000000 json_matcher-0.0.9/setup.py
```

### Comparing `json_matcher-0.0.8/LICENSE` & `json_matcher-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `json_matcher-0.0.8/PKG-INFO` & `json_matcher-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: json_matcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Match json with lucece-like query
 Home-page: https://github.com/hosung-yim/json_matcher
 Author: Greg.YIM
 Author-email: greg.yim@kakaocorp.com
 License: UNKNOWN
 Description: # json_matcher
```

### Comparing `json_matcher-0.0.8/README.md` & `json_matcher-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `json_matcher-0.0.8/bin/jrep` & `json_matcher-0.0.9/bin/jrep`

 * *Files identical despite different names*

### Comparing `json_matcher-0.0.8/bin/json_match` & `json_matcher-0.0.9/bin/json_match`

 * *Files identical despite different names*

### Comparing `json_matcher-0.0.8/json_matcher/json_matcher.py` & `json_matcher-0.0.9/json_matcher/json_matcher.py`

 * *Files identical despite different names*

### Comparing `json_matcher-0.0.8/json_matcher/match_environ.py` & `json_matcher-0.0.9/json_matcher/match_environ.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,14 @@
 
     def expand_regexp(self, base_regexp):
         names = self.extract_keyword_set_names(base_regexp)
         regexp = base_regexp
         for name in names:
             keyword_set = self.environ.get_keyword_set(name)
             regexp = keyword_set.expand_regexp(regexp)
-        print(regexp)
         return re.compile(regexp)
 
     def search_keyword_set(self, term, input_value):
         name = self.extract_keyword_set_name(term)
         if not name:
             return False
```

### Comparing `json_matcher-0.0.8/json_matcher.egg-info/PKG-INFO` & `json_matcher-0.0.9/json_matcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: json-matcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Match json with lucece-like query
 Home-page: https://github.com/hosung-yim/json_matcher
 Author: Greg.YIM
 Author-email: greg.yim@kakaocorp.com
 License: UNKNOWN
 Description: # json_matcher
```

### Comparing `json_matcher-0.0.8/setup.py` & `json_matcher-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 scripts = ['bin/json_match', 'bin/jrep']
 
 # packages
 packages = setuptools.find_packages(exclude=['tests'])
 
 setuptools.setup(
     name="json_matcher",
-    version="0.0.8",
+    version="0.0.9",
     url="https://github.com/hosung-yim/json_matcher",
-    dowload_url="https://github.com/hosung-yim/json_matcher/archive/refs/tags/0.0.8.tar.gz",
+    dowload_url="https://github.com/hosung-yim/json_matcher/archive/refs/tags/0.0.9.tar.gz",
 
     author="Greg.YIM",
     author_email="greg.yim@kakaocorp.com",
 
     description="Match json with lucece-like query",
     long_description=open('README.md').read(),
```

