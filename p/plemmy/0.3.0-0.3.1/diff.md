# Comparing `tmp/plemmy-0.3.0.tar.gz` & `tmp/plemmy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plemmy-0.3.0.tar", last modified: Sat Jul  8 04:04:43 2023, max compression
+gzip compressed data, was "plemmy-0.3.1.tar", last modified: Tue Jul 11 14:30:07 2023, max compression
```

## Comparing `plemmy-0.3.0.tar` & `plemmy-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-08 04:04:43.174264 plemmy-0.3.0/
--rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.3.0/LICENSE
--rw-r--r--   0 tjkessler   (501) staff       (20)     2706 2023-07-08 04:04:43.174104 plemmy-0.3.0/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     2420 2023-07-08 04:04:32.000000 plemmy-0.3.0/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-08 04:04:43.173018 plemmy-0.3.0/plemmy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      209 2023-07-08 04:04:32.000000 plemmy-0.3.0/plemmy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    71480 2023-07-08 03:39:07.000000 plemmy-0.3.0/plemmy/lemmyhttp.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    13963 2023-07-08 04:04:32.000000 plemmy-0.3.0/plemmy/objects.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    19156 2023-07-08 04:04:32.000000 plemmy-0.3.0/plemmy/responses.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     2866 2023-06-30 20:43:38.000000 plemmy-0.3.0/plemmy/utils.py
--rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-07-08 04:04:32.000000 plemmy-0.3.0/plemmy/version.py
--rw-r--r--   0 tjkessler   (501) staff       (20)    16980 2023-07-08 04:04:32.000000 plemmy-0.3.0/plemmy/views.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-08 04:04:43.173893 plemmy-0.3.0/plemmy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)     2706 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      331 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/requires.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-07-08 04:04:43.000000 plemmy-0.3.0/plemmy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-07-08 04:04:43.174310 plemmy-0.3.0/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.3.0/setup.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-11 14:30:07.064181 plemmy-0.3.1/
+-rw-r--r--   0 tjkessler   (501) staff       (20)    11367 2023-06-20 19:47:16.000000 plemmy-0.3.1/LICENSE
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2658 2023-07-11 14:30:07.064025 plemmy-0.3.1/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2372 2023-07-08 04:32:47.000000 plemmy-0.3.1/README.md
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-11 14:30:07.062904 plemmy-0.3.1/plemmy/
+-rw-r--r--   0 tjkessler   (501) staff       (20)      209 2023-07-08 04:04:32.000000 plemmy-0.3.1/plemmy/__init__.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    71480 2023-07-08 03:39:07.000000 plemmy-0.3.1/plemmy/lemmyhttp.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    13987 2023-07-11 14:28:15.000000 plemmy-0.3.1/plemmy/objects.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    19156 2023-07-08 04:04:32.000000 plemmy-0.3.1/plemmy/responses.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2866 2023-06-30 20:43:38.000000 plemmy-0.3.1/plemmy/utils.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)      120 2023-07-11 14:29:11.000000 plemmy-0.3.1/plemmy/version.py
+-rw-r--r--   0 tjkessler   (501) staff       (20)    16980 2023-07-08 04:04:32.000000 plemmy-0.3.1/plemmy/views.py
+drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2023-07-11 14:30:07.063800 plemmy-0.3.1/plemmy.egg-info/
+-rw-r--r--   0 tjkessler   (501) staff       (20)     2658 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/PKG-INFO
+-rw-r--r--   0 tjkessler   (501) staff       (20)      331 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/SOURCES.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/dependency_links.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        1 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/not-zip-safe
+-rw-r--r--   0 tjkessler   (501) staff       (20)       17 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/requires.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)        7 2023-07-11 14:30:07.000000 plemmy-0.3.1/plemmy.egg-info/top_level.txt
+-rw-r--r--   0 tjkessler   (501) staff       (20)       38 2023-07-11 14:30:07.064227 plemmy-0.3.1/setup.cfg
+-rw-r--r--   0 tjkessler   (501) staff       (20)      878 2023-06-20 19:47:16.000000 plemmy-0.3.1/setup.py
```

### Comparing `plemmy-0.3.0/LICENSE` & `plemmy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.0/PKG-INFO` & `plemmy-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -81,12 +81,12 @@
 post = response.post_view.post
 print(post.creator_id)
 print(post.community_id)
 print(post.name)
 print(post.body)
 ```
 
-Full documentation is on its way, but in the meantime check out our source code and some [examples]([https://github.com/tjkessler/plemmy/examples](https://github.com/tjkessler/plemmy/tree/main/examples)).
+Full documentation is on its way, but in the meantime check out our source code and some [examples](https://github.com/tjkessler/plemmy/tree/main/examples).
 
 ## Reporting issues, making contributions, etc. ##
 
 Don't hesitate to report a bug or unexpected results! Want to contribute? Make a pull request. Contact [@tjkessler](https://github.com/tjkessler) with any questions.
```

### Comparing `plemmy-0.3.0/README.md` & `plemmy-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -70,12 +70,12 @@
 post = response.post_view.post
 print(post.creator_id)
 print(post.community_id)
 print(post.name)
 print(post.body)
 ```
 
-Full documentation is on its way, but in the meantime check out our source code and some [examples]([https://github.com/tjkessler/plemmy/examples](https://github.com/tjkessler/plemmy/tree/main/examples)).
+Full documentation is on its way, but in the meantime check out our source code and some [examples](https://github.com/tjkessler/plemmy/tree/main/examples).
 
 ## Reporting issues, making contributions, etc. ##
 
 Don't hesitate to report a bug or unexpected results! Want to contribute? Make a pull request. Contact [@tjkessler](https://github.com/tjkessler) with any questions.
```

### Comparing `plemmy-0.3.0/plemmy/lemmyhttp.py` & `plemmy-0.3.1/plemmy/lemmyhttp.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.0/plemmy/objects.py` & `plemmy-0.3.1/plemmy/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     nsfw: bool = None
     actor_id: str = None
     local: bool = None
     hidden: bool = None
     posting_restricted_to_mods: bool = None
     instance_id: int = None
     updated: str = None
+    banner: bool = None
 
 
 @dataclass
 class CommunityAggregates:
     """https://join-lemmy.org/api/interfaces/CommunityAggregates.html"""
 
     id: int = None
```

### Comparing `plemmy-0.3.0/plemmy/responses.py` & `plemmy-0.3.1/plemmy/responses.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.0/plemmy/utils.py` & `plemmy-0.3.1/plemmy/utils.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.0/plemmy/views.py` & `plemmy-0.3.1/plemmy/views.py`

 * *Files identical despite different names*

### Comparing `plemmy-0.3.0/plemmy.egg-info/PKG-INFO` & `plemmy-0.3.1/plemmy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plemmy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python API for LemmyHttp
 Home-page: https://github.com/tjkessler/plemmy
 Author: Travis Kessler
 Author-email: travis.j.kessler@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -81,12 +81,12 @@
 post = response.post_view.post
 print(post.creator_id)
 print(post.community_id)
 print(post.name)
 print(post.body)
 ```
 
-Full documentation is on its way, but in the meantime check out our source code and some [examples]([https://github.com/tjkessler/plemmy/examples](https://github.com/tjkessler/plemmy/tree/main/examples)).
+Full documentation is on its way, but in the meantime check out our source code and some [examples](https://github.com/tjkessler/plemmy/tree/main/examples).
 
 ## Reporting issues, making contributions, etc. ##
 
 Don't hesitate to report a bug or unexpected results! Want to contribute? Make a pull request. Contact [@tjkessler](https://github.com/tjkessler) with any questions.
```

### Comparing `plemmy-0.3.0/setup.py` & `plemmy-0.3.1/setup.py`

 * *Files identical despite different names*

