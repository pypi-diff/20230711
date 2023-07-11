# Comparing `tmp/jplaw-0.1.7.tar.gz` & `tmp/jplaw-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jplaw-0.1.7.tar", last modified: Sun Jul  9 23:47:50 2023, max compression
+gzip compressed data, was "jplaw-0.1.8.tar", last modified: Tue Jul 11 12:54:15 2023, max compression
```

## Comparing `jplaw-0.1.7.tar` & `jplaw-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:47:49.999112 jplaw-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-09 23:47:36.000000 jplaw-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-09 23:47:49.999112 jplaw-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-09 23:47:36.000000 jplaw-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:47:49.995112 jplaw-0.1.7/jplaw/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/api_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/community.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27141 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:47:49.999112 jplaw-0.1.7/jplaw/types/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/comment_sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/http_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/listing_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/modlog_action_type.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/post_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/registration_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/search_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/sort_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/types/subscribed_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-07-09 23:47:36.000000 jplaw-0.1.7/jplaw/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 23:47:49.999112 jplaw-0.1.7/jplaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-09 23:47:49.000000 jplaw-0.1.7/jplaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-09 23:47:49.000000 jplaw-0.1.7/jplaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 23:47:49.000000 jplaw-0.1.7/jplaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-09 23:47:49.000000 jplaw-0.1.7/jplaw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-09 23:47:36.000000 jplaw-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 23:47:49.999112 jplaw-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:54:15.261129 jplaw-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-11 12:54:04.000000 jplaw-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-11 12:54:15.257128 jplaw-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-11 12:54:04.000000 jplaw-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:54:15.257128 jplaw-0.1.8/jplaw/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/api_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27141 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:54:15.257128 jplaw-0.1.8/jplaw/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/types/comment_sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/types/http_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/types/listing_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/types/modlog_action_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/types/post_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/types/registration_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/types/search_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/types/sort_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/types/subscribed_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-07-11 12:54:04.000000 jplaw-0.1.8/jplaw/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:54:15.257128 jplaw-0.1.8/jplaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-11 12:54:15.000000 jplaw-0.1.8/jplaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-11 12:54:15.000000 jplaw-0.1.8/jplaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:54:15.000000 jplaw-0.1.8/jplaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 12:54:15.000000 jplaw-0.1.8/jplaw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-11 12:54:04.000000 jplaw-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:54:15.261129 jplaw-0.1.8/setup.cfg
```

### Comparing `jplaw-0.1.7/LICENSE` & `jplaw-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/PKG-INFO` & `jplaw-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jplaw-0.1.7/README.md` & `jplaw-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw/api_paths.py` & `jplaw-0.1.8/jplaw/api_paths.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw/comment.py` & `jplaw-0.1.8/jplaw/comment.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw/community.py` & `jplaw-0.1.8/jplaw/community.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
             "description": description,
             "icon": icon,
             "banner": banner,
             "nsfw": nsfw,
             "posting_restricted_to_mods": posting_restricted_to_mods,
             "discussion_languages": discussion_languages,
             }
-        res = self._req.lemmyRequest("createCommunity", instance=instance, form=form, optional=optional, auth=True)
+        res = self._req.lemmyRequest("editCommunity", instance=instance, form=form, optional=optional, auth=True)
         return res["community_view"]
         
     def remove(self, community_id:int, removed:bool=True, reason:str=None, expires:int=None, instance:str=None):
         """
         Remove a community
         
         Args:
```

### Comparing `jplaw-0.1.7/jplaw/emoji.py` & `jplaw-0.1.8/jplaw/emoji.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw/lemmy.py` & `jplaw-0.1.8/jplaw/lemmy.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,7 +82,22 @@
         self.Community = Community(self._req)
         self.Comment = Comment(self._req)
         self.User = User(self._req)
         self.Site = Site(self._req)
         self.Emoji = Emoji(self._req)
         self.PrivateMessage = PrivateMessage(self._req)
         # print(self._req.headers.get("Authorization"))
+        
+    def federateCommunity(self, name:str, auth:bool=True, instance:str=None):
+        """
+        Get comunity from another instance which may not have been federated.
+        
+        Args:
+            name (str): Name of the community. Include @[instance] for a community at 
+            auth (bool): Whether or not to use authentication. True by default.
+            instance (str): Remote instance to send federation command to / get federated community through. Federating "[community]@[instance A]" with instance="[instance B]" sends the federation command to instance B, which then looks for the community at instance A. Default None uses instane = logged in instance.
+        
+        Returns:
+            Community 
+        """
+        data = self.Site.resolveObject("!" + name);
+        return self.Community.get(name, instance=instance, auth=auth)["community_view"];
```

### Comparing `jplaw-0.1.7/jplaw/post.py` & `jplaw-0.1.8/jplaw/post.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw/private_message.py` & `jplaw-0.1.8/jplaw/private_message.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw/requestor.py` & `jplaw-0.1.8/jplaw/requestor.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw/site.py` & `jplaw-0.1.8/jplaw/site.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw/types/modlog_action_type.py` & `jplaw-0.1.8/jplaw/types/modlog_action_type.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw/types/sort_type.py` & `jplaw-0.1.8/jplaw/types/sort_type.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw/user.py` & `jplaw-0.1.8/jplaw/user.py`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/jplaw.egg-info/PKG-INFO` & `jplaw-0.1.8/jplaw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jplaw
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python wrapper for the lemmy HTTP API. Forked from plaw by Benjamin Jablonski (benja810)
 Author-email: Amar Persaud <tehspartaa@gmail.com>
 Project-URL: Homepage, https://github.com/amarpersaud/python-jplaw
 Project-URL: Bug Tracker, https://github.com/amarpersaud/python-jplaw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jplaw-0.1.7/jplaw.egg-info/SOURCES.txt` & `jplaw-0.1.8/jplaw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jplaw-0.1.7/pyproject.toml` & `jplaw-0.1.8/pyproject.toml`

 * *Files identical despite different names*

