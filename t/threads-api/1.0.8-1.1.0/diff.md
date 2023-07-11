# Comparing `tmp/threads-api-1.0.8.tar.gz` & `tmp/threads-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.0.8.tar", last modified: Mon Jul 10 21:19:44 2023, max compression
+gzip compressed data, was "threads-api-1.1.0.tar", last modified: Tue Jul 11 20:10:55 2023, max compression
```

## Comparing `threads-api-1.0.8.tar` & `threads-api-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-10 21:19:44.623238 threads-api-1.0.8/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.0.8/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    11140 2023-07-10 21:19:44.619238 threads-api-1.0.8/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10610 2023-07-10 21:06:25.000000 threads-api-1.0.8/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      384 2023-07-10 21:19:18.000000 threads-api-1.0.8/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-10 21:19:44.623238 threads-api-1.0.8/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      789 2023-07-10 21:19:24.000000 threads-api-1.0.8/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-10 21:19:44.619238 threads-api-1.0.8/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.0.8/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-10 21:19:44.619238 threads-api-1.0.8/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.0.8/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    25108 2023-07-10 21:19:03.000000 threads-api-1.0.8/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-10 21:19:44.619238 threads-api-1.0.8/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.0.8/threads_api/tests/__init__.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      404 2023-07-07 21:21:06.000000 threads-api-1.0.8/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-10 21:19:44.619238 threads-api-1.0.8/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    11140 2023-07-10 21:19:44.000000 threads-api-1.0.8/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-10 21:19:44.000000 threads-api-1.0.8/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-10 21:19:44.000000 threads-api-1.0.8/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       17 2023-07-10 21:19:44.000000 threads-api-1.0.8/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-10 21:19:44.000000 threads-api-1.0.8/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:10:55.808246 threads-api-1.1.0/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.0/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12721 2023-07-11 20:10:55.808246 threads-api-1.1.0/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12191 2023-07-11 20:10:30.000000 threads-api-1.1.0/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      384 2023-07-11 20:06:05.000000 threads-api-1.1.0/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-11 20:10:55.808246 threads-api-1.1.0/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      768 2023-07-11 20:05:14.000000 threads-api-1.1.0/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:10:55.804246 threads-api-1.1.0/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.0/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:10:55.804246 threads-api-1.1.0/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.0/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    25004 2023-07-11 20:06:05.000000 threads-api-1.1.0/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:10:55.808246 threads-api-1.1.0/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.0/threads_api/tests/__init__.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      406 2023-07-11 20:05:14.000000 threads-api-1.1.0/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:10:55.804246 threads-api-1.1.0/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12721 2023-07-11 20:10:55.000000 threads-api-1.1.0/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-11 20:10:55.000000 threads-api-1.1.0/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-11 20:10:55.000000 threads-api-1.1.0/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-11 20:10:55.000000 threads-api-1.1.0/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-11 20:10:55.000000 threads-api-1.1.0/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.0.8/LICENSE` & `threads-api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.0.8/PKG-INFO` & `threads-api-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,22 @@
-Metadata-Version: 2.1
-Name: threads-api
-Version: 1.0.8
-Summary: Unofficial Python client for Meta Threads.net API
-Home-page: https://github.com/danie1/threads-api
-Author: Danie1
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # [<img src="https://raw.githubusercontent.com/danie1/threads-api/main/.github/logo.jpg" width="36" height="36" />](https://github.com/danie1) Meta's Threads.net API
 
 [![Downdloads](https://pepy.tech/badge/threads-api)](https://pypi.org/project/threads-api/)
 [![Version](https://img.shields.io/pypi/v/threads-api.svg?style=flat)](https://pypi.org/project/threads-api/)
 [![Python](https://img.shields.io/pypi/pyversions/threads-api.svg)](https://pypi.org/project/threads-api/) [![MIT License](https://img.shields.io/pypi/l/threads-api.svg?style=flat)](https://github.com/Danie1/threads-api/blob/main/LICENSE) 
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
 
 Inspired by [NPM Threads-API](https://github.com/junhoyeo/threads-api)
 
 # Threads API - Python
 
-Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, post, retrieve user profile information, user IDs and user profile threads.
+Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, read and publish posts, view who liked a post, retrieve user profile information, follow/unfollow and much more.
+
+It is built using `aiohttp` to ease asynchronous execution of the API, for ⚡ super-fast ⚡ results.
 
 Table of content:
 
 * [Demo](#demo)
 * [Getting started](#getting-started)
   * [Installation](#Installation)
 * [Usage Examples](#usage-examples)
@@ -60,15 +45,15 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 async def post():
     threads_api = ThreadsAPI()
-    await threads_api.login(os.environ.get('USERNAME'), os.environ,get('PASSWORD'))
+    await threads_api.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
     result = await threads_api.post("I am posting this from the threads api!")
 
     if result:
         print("Post has been successfully posted")
     else:
         print("Unable to post.")
 
@@ -113,15 +98,15 @@
 async def get_user_profile():
     threads_api = ThreadsAPI()
 
     username = "zuck"
     user_id = await threads_api.get_user_id_from_username(username)
 
     if user_id:
-        user_profile = await threads_api.get_user_profile(username, user_id)
+        user_profile = await threads_api.get_user_profile(user_id)
         print(f"User profile for '{username}':")
         print(f"Name: {user_profile['username']}")
         print(f"Bio: {user_profile['biography']}")
         print(f"Followers: {user_profile['follower_count']}")
     else:
         print(f"User ID not found for username '{username}'")
 ```
@@ -132,25 +117,25 @@
 Name: zuck
 Bio: 
 Followers: 2288633
 ```
 </details>
 
 <details>
-  <summary>"get_user_profile_threads" Function</summary>
+  <summary>"get_user_threads" Function</summary>
 
 ``` python
-async def get_user_profile_threads():
+async def get_user_threads():
     threads_api = ThreadsAPI()
 
     username = "zuck"
     user_id = await threads_api.get_user_id_from_username(username)
 
     if user_id:
-        threads = await threads_api.get_user_profile_threads(username, user_id)
+        threads = await threads_api.get_user_threads(user_id)
         print(f"The threads for user '{username}' are:")
         for thread in threads:
             print(f"Text: {thread['thread_items'][0]['post']['caption']} || Likes: {thread['thread_items'][0]['post']['like_count']}")
     else:
         print(f"User ID not found for username '{username}'")
 
 ```
@@ -167,25 +152,25 @@
 zuck's Post: {'text': "Glad you're all here on day one. Let's build something great together!"} || Likes: 175563
 zuck's Post: {'text': "Let's do this. Welcome to Threads. 🔥"} || Likes: 166987
 ```
 </details>
 
 
 <details>
-  <summary>"get_user_profile_replies" Function</summary>
+  <summary>"get_user_replies" Function</summary>
 
 ``` python
-async def get_user_profile_replies():
+async def get_user_replies():
     threads_api = ThreadsAPI()
 
     username = "zuck"
     user_id = await threads_api.get_user_id_from_username(username)
 
     if user_id:
-        threads = await threads_api.get_user_profile_replies(username, user_id)
+        threads = await threads_api.get_user_replies(user_id)
         print(f"The replies for user '{username}' are:")
         for thread in threads:
             print(f"-\n{thread['thread_items'][0]['post']['user']['username']}'s Post: {thread['thread_items'][0]['post']['caption']} || Likes: {thread['thread_items'][0]['post']['like_count']}")
 
             if len(thread["thread_items"]) > 1:
                 print(f"{username}'s Reply: {thread['thread_items'][1]['post']['caption']} || Likes: {thread['thread_items'][1]['post']['like_count']}\n-")
             else:
@@ -282,14 +267,46 @@
 winchester_757's Reply: {'text': 'If only the meta verse was this good LMAO'} || Likes: 0
 -
 winchester_757's Reply: {'text': 'Only 10 mil more to match the big guy'} || Likes: 0
 ```
 </details>
 
 <details>
+  <summary>"get_post_likes" Function</summary>
+
+``` python
+async def get_post_likes():
+    api = ThreadsAPI()
+    post_url = "https://www.threads.net/t/CuZsgfWLyiI"
+
+    post_id = await api.get_post_id_from_url(post_url)
+
+    likes = await api.get_post_likes(post_id)
+    number_of_likes_to_display = 10
+
+    for user_info in likes[:number_of_likes_to_display]:
+        print(f'Username: {user_info["username"]} || Full Name: {user_info["full_name"]} || Follower Count: {user_info["follower_count"]} ')
+```
+
+Example Output:
+```
+Username: andrew_votava || Full Name: Andrew Votava || Follower Count: 19 
+Username: herson_theeog || Full Name: Herson_theeOG || Follower Count: 323 
+Username: dhruv___kanojia || Full Name: Dhruv🌟 || Follower Count: 38 
+Username: codecrusadepk || Full Name: Code Crusade || Follower Count: 9 
+Username: toxicated_jeshim_007 || Full Name: Jeshim Akhtar Choudhury || Follower Count: 6 
+Username: jay.rex.official || Full Name: Jay Rex || Follower Count: 30 
+Username: jessy.servin || Full Name: Jessica Servín || Follower Count: 343 
+Username: joshxmadrid || Full Name: Josh Madrid || Follower Count: 1092 
+Username: ganjipro || Full Name: Song Ganji || Follower Count: 1649 
+Username: bilalmuhamadi || Full Name: B I L A L  M U H A M A D I || Follower Count: 111 
+```
+</details>
+
+<details>
   <summary>"post" Function</summary>
 
 ``` python
 async def post():
     threads_api = ThreadsAPI()
     # either set USERNAME and PASSWORD as environment variables, or replace these with your actual credentials
     await threads_api.login(os.environ.get('USERNAME'), os.environ.get('PASSWORD'))
@@ -305,33 +322,34 @@
 ```
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
 
-- [x] ✅ Login as User
-- [x] ✅ Write Posts
+- [x] ✅ Login functionality 🔒
+  - [x] 🚧 Cache login token securely (reduce login requests)
+- [x] ✅ Write Posts (Requires Login 🔒)
   - [x] ✅ Posts with just text
   - [x] ✅ Posts with text and an image
   - [x] ✅ Posts with text that share a url
-- [x] ✅ Perform Actions
+  - [ ] 🚧 Post with text and share a video
+  - [ ] 🚧 Reply to Posts
+- [x] ✅ Perform Actions (Requires Login 🔒)
   - [x] ✅ Like Posts
   - [x] ✅ Unlike Posts
   - [x] ✅ Follow User
   - [x] ✅ Unfollow User
-- [x] ✅ Read Data\
+- [x] ✅ Read Data
   - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
-  - [x] ✅ Read user profile info
-  - [x] ✅ Read list of user Threads
-  - [x] ✅ Read list of user Replies
+  - [x] ✅ Read a user's profile info
+  - [x] ✅ Read list of a user's Threads
+  - [x] ✅ Read list of a user's Replies
   - [x] ✅ Read Post and a list of its Replies
-- [ ] 🚧  Upload images and videos
-- [ ] 🚧  Reply to Posts
+  - [x] ✅ View who liked a post
 - [x] ✅  CI/CD
-  - [ ] 🚧  Pytest
   - [x] ✅  GitHub Actions Pipeline
+  - [ ] 🚧  Pytest
 
 
 # License
 This project is licensed under the MIT license.
-
```

### Comparing `threads-api-1.0.8/README.md` & `threads-api-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,39 @@
+Metadata-Version: 2.1
+Name: threads-api
+Version: 1.1.0
+Summary: Unofficial Python client for Meta Threads.net API
+Home-page: https://github.com/danie1/threads-api
+Author: Danie1
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # [<img src="https://raw.githubusercontent.com/danie1/threads-api/main/.github/logo.jpg" width="36" height="36" />](https://github.com/danie1) Meta's Threads.net API
 
 [![Downdloads](https://pepy.tech/badge/threads-api)](https://pypi.org/project/threads-api/)
 [![Version](https://img.shields.io/pypi/v/threads-api.svg?style=flat)](https://pypi.org/project/threads-api/)
 [![Python](https://img.shields.io/pypi/pyversions/threads-api.svg)](https://pypi.org/project/threads-api/) [![MIT License](https://img.shields.io/pypi/l/threads-api.svg?style=flat)](https://github.com/Danie1/threads-api/blob/main/LICENSE) 
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
 
 Inspired by [NPM Threads-API](https://github.com/junhoyeo/threads-api)
 
 # Threads API - Python
 
-Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, post, retrieve user profile information, user IDs and user profile threads.
+Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, read and publish posts, view who liked a post, retrieve user profile information, follow/unfollow and much more.
+
+It is built using `aiohttp` to ease asynchronous execution of the API, for ⚡ super-fast ⚡ results.
 
 Table of content:
 
 * [Demo](#demo)
 * [Getting started](#getting-started)
   * [Installation](#Installation)
 * [Usage Examples](#usage-examples)
@@ -43,15 +62,15 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 async def post():
     threads_api = ThreadsAPI()
-    await threads_api.login(os.environ.get('USERNAME'), os.environ,get('PASSWORD'))
+    await threads_api.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
     result = await threads_api.post("I am posting this from the threads api!")
 
     if result:
         print("Post has been successfully posted")
     else:
         print("Unable to post.")
 
@@ -96,15 +115,15 @@
 async def get_user_profile():
     threads_api = ThreadsAPI()
 
     username = "zuck"
     user_id = await threads_api.get_user_id_from_username(username)
 
     if user_id:
-        user_profile = await threads_api.get_user_profile(username, user_id)
+        user_profile = await threads_api.get_user_profile(user_id)
         print(f"User profile for '{username}':")
         print(f"Name: {user_profile['username']}")
         print(f"Bio: {user_profile['biography']}")
         print(f"Followers: {user_profile['follower_count']}")
     else:
         print(f"User ID not found for username '{username}'")
 ```
@@ -115,25 +134,25 @@
 Name: zuck
 Bio: 
 Followers: 2288633
 ```
 </details>
 
 <details>
-  <summary>"get_user_profile_threads" Function</summary>
+  <summary>"get_user_threads" Function</summary>
 
 ``` python
-async def get_user_profile_threads():
+async def get_user_threads():
     threads_api = ThreadsAPI()
 
     username = "zuck"
     user_id = await threads_api.get_user_id_from_username(username)
 
     if user_id:
-        threads = await threads_api.get_user_profile_threads(username, user_id)
+        threads = await threads_api.get_user_threads(user_id)
         print(f"The threads for user '{username}' are:")
         for thread in threads:
             print(f"Text: {thread['thread_items'][0]['post']['caption']} || Likes: {thread['thread_items'][0]['post']['like_count']}")
     else:
         print(f"User ID not found for username '{username}'")
 
 ```
@@ -150,25 +169,25 @@
 zuck's Post: {'text': "Glad you're all here on day one. Let's build something great together!"} || Likes: 175563
 zuck's Post: {'text': "Let's do this. Welcome to Threads. 🔥"} || Likes: 166987
 ```
 </details>
 
 
 <details>
-  <summary>"get_user_profile_replies" Function</summary>
+  <summary>"get_user_replies" Function</summary>
 
 ``` python
-async def get_user_profile_replies():
+async def get_user_replies():
     threads_api = ThreadsAPI()
 
     username = "zuck"
     user_id = await threads_api.get_user_id_from_username(username)
 
     if user_id:
-        threads = await threads_api.get_user_profile_replies(username, user_id)
+        threads = await threads_api.get_user_replies(user_id)
         print(f"The replies for user '{username}' are:")
         for thread in threads:
             print(f"-\n{thread['thread_items'][0]['post']['user']['username']}'s Post: {thread['thread_items'][0]['post']['caption']} || Likes: {thread['thread_items'][0]['post']['like_count']}")
 
             if len(thread["thread_items"]) > 1:
                 print(f"{username}'s Reply: {thread['thread_items'][1]['post']['caption']} || Likes: {thread['thread_items'][1]['post']['like_count']}\n-")
             else:
@@ -265,14 +284,46 @@
 winchester_757's Reply: {'text': 'If only the meta verse was this good LMAO'} || Likes: 0
 -
 winchester_757's Reply: {'text': 'Only 10 mil more to match the big guy'} || Likes: 0
 ```
 </details>
 
 <details>
+  <summary>"get_post_likes" Function</summary>
+
+``` python
+async def get_post_likes():
+    api = ThreadsAPI()
+    post_url = "https://www.threads.net/t/CuZsgfWLyiI"
+
+    post_id = await api.get_post_id_from_url(post_url)
+
+    likes = await api.get_post_likes(post_id)
+    number_of_likes_to_display = 10
+
+    for user_info in likes[:number_of_likes_to_display]:
+        print(f'Username: {user_info["username"]} || Full Name: {user_info["full_name"]} || Follower Count: {user_info["follower_count"]} ')
+```
+
+Example Output:
+```
+Username: andrew_votava || Full Name: Andrew Votava || Follower Count: 19 
+Username: herson_theeog || Full Name: Herson_theeOG || Follower Count: 323 
+Username: dhruv___kanojia || Full Name: Dhruv🌟 || Follower Count: 38 
+Username: codecrusadepk || Full Name: Code Crusade || Follower Count: 9 
+Username: toxicated_jeshim_007 || Full Name: Jeshim Akhtar Choudhury || Follower Count: 6 
+Username: jay.rex.official || Full Name: Jay Rex || Follower Count: 30 
+Username: jessy.servin || Full Name: Jessica Servín || Follower Count: 343 
+Username: joshxmadrid || Full Name: Josh Madrid || Follower Count: 1092 
+Username: ganjipro || Full Name: Song Ganji || Follower Count: 1649 
+Username: bilalmuhamadi || Full Name: B I L A L  M U H A M A D I || Follower Count: 111 
+```
+</details>
+
+<details>
   <summary>"post" Function</summary>
 
 ``` python
 async def post():
     threads_api = ThreadsAPI()
     # either set USERNAME and PASSWORD as environment variables, or replace these with your actual credentials
     await threads_api.login(os.environ.get('USERNAME'), os.environ.get('PASSWORD'))
@@ -288,32 +339,36 @@
 ```
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
 
-- [x] ✅ Login as User
-- [x] ✅ Write Posts
+- [x] ✅ Login functionality 🔒
+  - [x] 🚧 Cache login token securely (reduce login requests)
+- [x] ✅ Write Posts (Requires Login 🔒)
   - [x] ✅ Posts with just text
   - [x] ✅ Posts with text and an image
   - [x] ✅ Posts with text that share a url
-- [x] ✅ Perform Actions
+  - [ ] 🚧 Post with text and share a video
+  - [ ] 🚧 Reply to Posts
+- [x] ✅ Perform Actions (Requires Login 🔒)
   - [x] ✅ Like Posts
   - [x] ✅ Unlike Posts
   - [x] ✅ Follow User
   - [x] ✅ Unfollow User
-- [x] ✅ Read Data\
+- [x] ✅ Read Data
   - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
-  - [x] ✅ Read user profile info
-  - [x] ✅ Read list of user Threads
-  - [x] ✅ Read list of user Replies
+  - [x] ✅ Read a user's profile info
+  - [x] ✅ Read list of a user's Threads
+  - [x] ✅ Read list of a user's Replies
   - [x] ✅ Read Post and a list of its Replies
-- [ ] 🚧  Upload images and videos
-- [ ] 🚧  Reply to Posts
+  - [x] ✅ View who liked a post
 - [x] ✅  CI/CD
-  - [ ] 🚧  Pytest
   - [x] ✅  GitHub Actions Pipeline
+  - [ ] 🚧  Pytest
 
 
 # License
-This project is licensed under the MIT license.
+This project is licensed under the MIT license.
+
+
```

### Comparing `threads-api-1.0.8/setup.py` & `threads-api-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.0.8',
+    version='1.1.0',
     description='Unofficial Python client for Meta Threads.net API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
     install_requires=[
-        'aiohttp',
-        'requests',
+        'aiohttp'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
```

### Comparing `threads-api-1.0.8/threads_api/src/threads_api.py` & `threads-api-1.1.0/threads_api/src/threads_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import requests
 from typing import Optional, Dict, Union, List
 import aiohttp
 import re
 import json
 import asyncio
 import json
 import random
@@ -11,41 +10,90 @@
 import random
 import urllib
 import os
 import mimetypes
 import uuid
 import time
 import traceback
+import copy
 
 BASE_URL = "https://i.instagram.com/api/v1"
 LOGIN_URL = BASE_URL + "/bloks/apps/com.bloks.www.bloks.caa.login.async.send_login_request/"
 POST_URL_TEXTONLY = BASE_URL + "/media/configure_text_only_post/"
 POST_URL_IMAGE = BASE_URL + "/media/configure_text_post_app_feed/"
+DEFAULT_HEADERS = {
+            'Authority': 'www.threads.net',
+            'Accept': '*/*',
+            'Accept-Language': 'en-US,en;q=0.9',
+            'Cache-Control': 'no-cache',
+            'Content-Type': 'application/x-www-form-urlencoded',
+            'Origin': 'https://www.threads.net',
+            'Pragma': 'no-cache',
+             'Sec-Fetch-Dest': 'document',
+            'Sec-Fetch-Mode': 'navigate',
+            'Sec-Fetch-Site': 'cross-site',
+            'Sec-Fetch-User': '?1',
+            'Upgrade-Insecure-Requests': '1',
+            'User-Agent': (
+                'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_6) '
+                'AppleWebKit/605.1.15 (KHTML, like Gecko) Version/11.1.2 Safari/605.1.15'
+            ),
+            'X-ASBD-ID': '129477',
+            'X-FB-LSD': 'NjppQDEgONsU_1LCzrmp6q',
+            'X-IG-App-ID': '238260118697367',
+        }
 
 class ThreadsAPIOptions:
-    def __init__(self, fbLSDToken: Optional[str] = None, 
-                       token: Optional[str] = None):
-        self.fbLSDToken = fbLSDToken
+    def __init__(self, token: Optional[str] = None):
         self.token = token
 
 class ThreadsAPI:
     def __init__(self, options: Optional[ThreadsAPIOptions] = None):
-        self.fbLSDToken = 'NjppQDEgONsU_1LCzrmp6q'
         self.token = None
         self.user_id = None
 
-        if options and options.fbLSDToken:
-            self.fbLSDToken = options.fbLSDToken
-
         if options and options.token:
             self.token = options.token
 
         self.is_logged_in = False
 
+        self.FBLSDToken = 'NjppQDEgONsU_1LCzrmp6q'
+
+    async def _get_public_headers(self) -> str:
+        default_headers = copy.deepcopy(DEFAULT_HEADERS)
+        default_headers['X-FB-LSD'] = await self._refresh_public_token()
+        return default_headers
+    
+    async def _refresh_public_token(self) -> str:
+        modified_default_headers = copy.deepcopy(DEFAULT_HEADERS)
+        del modified_default_headers['X-FB-LSD']
+        async with aiohttp.ClientSession() as session:
+            async with session.get('https://www.instagram.com/instagram', headers=modified_default_headers) as response:
+                data = await response.text()
+                token_key_value = re.search('LSD",\\[\\],{"token":"(.*?)"},\\d+\\]', data).group()
+                token_key_value = token_key_value.replace('LSD",[],{"token":"', '')
+                token = token_key_value.split('"')[0]
+
+        self.FBLSDToken = token
+        return self.FBLSDToken
+    
     async def login(self, username, password):
+        """
+        Logs in the user with the provided username and password.
+
+        Args:
+            username (str): The username for authentication.
+            password (str): The password for authentication.
+
+        Returns:
+            bool: True if the login is successful, False otherwise.
+
+        Raises:
+            Exception: If the username or password are invalid, or if an error occurs during login.
+        """
         if username is None or password is None:
             raise Exception("Username or password are invalid")
 
         self.username = username
 
         try:
             blockVersion = "5f56efad68e1edec7801f630b5c122704ec5378adbee6609a448f105f34a9c73"
@@ -84,338 +132,372 @@
             if len(pos) > 1:
                 pos = pos[1]
                 pos = pos.split("==")[0]
                 token = f"{pos}=="
                 self.token = token
 
                 self.user_id = await self.get_user_id_from_username(username)
+                self.auth_headers = {
+                    'Authorization': f'Bearer IGT:2:{self.token}',
+                    'User-Agent': 'Barcelona 289.0.0.77.109 Android',
+                    'Sec-Fetch-Site': 'same-origin',
+                    'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
+                }
                 self.is_logged_in = True
                 return True
             else:
                 raise Exception("Error with the login response")
         except Exception as e:
             print("[ERROR] ", e)
             raise
 
     async def __auth_required_post_request(self, url: str):
-        headers = {
-                'Authorization': f'Bearer IGT:2:{self.token}',
-                'User-Agent': 'Barcelona 289.0.0.77.109 Android',
-                'Sec-Fetch-Site': 'same-origin',
-                'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
-            }
         async with aiohttp.ClientSession() as session:
-            async with session.post(url, headers=headers) as response:
+            async with session.post(url, headers=self.auth_headers) as response:
                 return await response.json()
-            
+    
+    
+
     async def get_user_id_from_username(self, username: str) -> str:
-        url = f"https://www.threads.net/@{username}"
-        headers = {
-            "authority": "www.threads.net",
-            "accept": "*/*",
-            'accept-language': 'en-US,en;q=0.9',
-            "cache-control": "no-cache",
-            "origin": "https://www.threads.net",
-            "pragma": "no-cache",
-            "referer": f"https://www.threads.net/@{username}",
-            "x-asbd-id": "129477",
-            "x-fb-lsd": "NjppQDEgONsU_1LCzrmp6q",
-            "x-ig-app-id": "238260118697367",
-        }
+        """
+        Retrieves the user ID associated with a given username.
         
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url, headers=headers) as response:
-                text = await response.text()
+        Args:
+            username (str): The username to retrieve the user ID for.
+        
+        Returns:
+            str: The user ID if found, or None if the user ID is not found.
+        """
+        if self.is_logged_in:
+            url = BASE_URL + "/users/{username}/usernameinfo/"
+            async with aiohttp.ClientSession() as session:
+                async with session.get(url, headers=self.auth_headers) as response:
+                    data = await response.json()
+                    user_id = int(data['user']['pk'])
+                    return user_id
+        else:
+            url = f"https://www.threads.net/@{username}"
+            
+            async with aiohttp.ClientSession() as session:
+                async with session.get(url, headers=await self._get_public_headers()) as response:
+                    text = await response.text()
 
-        text = text.replace('\\s', "").replace('\\n', "")
-        user_id = re.search(r'"props":{"user_id":"(\d+)"},', text)
+            text = text.replace('\\s', "").replace('\\n', "")
+            user_id = re.search(r'"props":{"user_id":"(\d+)"},', text)
+
+            return user_id.group(1) if user_id else None
 
-        lsd_token_match = re.search('"LSD",\[\],{"token":"(\w+)"},\d+\]', text)
-        lsd_token = lsd_token_match.group(1) if lsd_token_match else None
-        #self.fbLSDToken = lsd_token
+    async def get_user_profile(self, user_id: str):
+        """
+        Retrieves the profile information for a user with the provided user ID.
 
-        return user_id.group(1) if user_id else None
+        Args:
+            user_id (str): The user ID for which to retrieve the profile information.
 
-    async def get_user_profile(self, username: str, user_id: str):
+        Returns:
+            dict: A dictionary containing the user profile information.
+
+        Raises:
+            Exception: If an error occurs during the profile retrieval process.
+        """
         url = 'https://www.threads.net/api/graphql'
-        headers = {
-            'authority': 'www.threads.net',
-            'accept': '*/*',
-            'accept-language': 'en-US,en;q=0.9',
-            'content-type': 'application/x-www-form-urlencoded',
-            'origin': 'https://www.threads.net',
-            'referer': f'https://www.threads.net/@{username}',
-            'sec-ch-prefers-color-scheme': 'light',
-            'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
-            'sec-ch-ua-full-version-list': '"Not.A/Brand";v="8.0.0.0", "Chromium";v="114.0.5735.199", "Google Chrome";v="114.0.5735.199"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"Windows"',
-            'sec-ch-ua-platform-version': '"15.0.0"',
+
+        modified_headers = copy.deepcopy(await self._get_public_headers())
+
+        modified_headers.update({
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-origin',
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
-            'viewport-width': '897',
-            'x-asbd-id': '129477',
             'x-fb-friendly-name': 'BarcelonaProfileRootQuery',
-            'x-fb-lsd': 'I5silyPfeZJQAyrhqVdqGB',
-            'x-ig-app-id': '238260118697367'
-        }
+            'x-fb-lsd': self.FBLSDToken,
+        })
+        
         payload = {
-            'av': '0',
-            '__user': '0',
-            '__a': '1',
-            '__req': '1',
-            '__hs': '19544.HYP:barcelona_web_pkg.2.1..0.0',
-            'dpr': '1',
-            '__ccg': 'EXCELLENT',
-            '__rev': '1007798382',
-            '__s': 'hue11s:dyq74i:1fwaxg',
-            '__hsi': '7252829167888753415',
-            '__dyn': '7xeUmwlEnwn8K2WnFw9-2i5U4e0yoW3q32360CEbo1nEhw2nVE4W0om78b87C0yE465o-cw5Mx62G3i0Bo7O2l0Fwqo31wnEfovwRwlE-U2zxe2Gew9O22362W2K0zK5o4q0GpovU1aUbodEGdwtU2ewbS1LwTwNwLw8O1pwr82gxC',
-            '__csr': 'gyhelk8iS00lnm4oioC2385um28MWawVwt40km2Ordg-cGu3C4E6-2QfoJ4m8g80x6wbC0E41Jy30sQ13g0E06V08M42eNE8k0wg88gzBe',
-            '__comet_req': '29',
-            'lsd': 'I5silyPfeZJQAyrhqVdqGB',
-            'jazoest': '22056',
-            '__spin_r': '1007798382',
-            '__spin_b': 'trunk',
-            '__spin_t': '1688680883',
-            '__jssesw': '1',
-            'fb_api_caller_class': 'RelayModern',
-            'fb_api_req_friendly_name': 'BarcelonaProfileRootQuery',
-            'variables': f'{{"userID":"{user_id}"}}',
-            'server_timestamps': 'true',
-            'doc_id': '23996318473300828'
-        }
+                'lsd': self.FBLSDToken,
+                'variables': json.dumps(
+                    {
+                        'userID': user_id,
+                    }
+                ),
+                'doc_id': '23996318473300828'
+            }
 
         async with aiohttp.ClientSession() as session:
-            async with session.post(url, headers=headers, data=payload) as response:
+            async with session.post(url, headers=modified_headers, data=payload) as response:
                 text = await response.text()
                 data = json.loads(text)
                
         user = data['data']['userData']['user']
         return user
 
-    async def get_user_profile_threads(self, username: str, user_id: str):
+    async def get_user_threads(self, user_id: str):
+        """
+        Retrieves the threads associated with a user with the provided user ID.
+
+        Args:
+            user_id (str): The user ID for which to retrieve the threads.
+
+        Returns:
+            list: A list of dictionaries representing the threads associated with the user.
+
+        Raises:
+            Exception: If an error occurs during the thread retrieval process.
+        """
         url = 'https://www.threads.net/api/graphql'
-        headers = {
-            'authority': 'www.threads.net',
-            'accept': '*/*',
-            'accept-language': 'en-US,en;q=0.9',
-            'content-type': 'application/x-www-form-urlencoded',
-            'origin': 'https://www.threads.net',
-            'referer': f'https://www.threads.net/@{username}',
-            'sec-ch-prefers-color-scheme': 'light',
-            'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
-            'sec-ch-ua-full-version-list': '"Not.A/Brand";v="8.0.0.0", "Chromium";v="114.0.5735.199", "Google Chrome";v="114.0.5735.199"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"Windows"',
-            'sec-ch-ua-platform-version': '"15.0.0"',
+        
+        modified_headers = copy.deepcopy(await self._get_public_headers())
+
+        modified_headers.update({
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-origin',
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
-            'viewport-width': '897',
-            'x-asbd-id': '129477',
             'x-fb-friendly-name': 'BarcelonaProfileThreadsTabQuery',
-            'x-fb-lsd': 'I5silyPfeZJQAyrhqVdqGB',
-            'x-ig-app-id': '238260118697367'
-        }
+            'x-fb-lsd': self.FBLSDToken,
+        })
+        
         payload = {
-            'av': '0',
-            '__user': '0',
-            '__a': '1',
-            '__req': '2',
-            '__hs': '19544.HYP:barcelona_web_pkg.2.1..0.0',
-            'dpr': '1',
-            '__ccg': 'EXCELLENT',
-            '__rev': '1007798382',
-            '__s': 'hue11s:dyq74i:1fwaxg',
-            '__hsi': '7252829167888753415',
-            '__dyn': '7xeUmwlEnwn8K2WnFw9-2i5U4e0yoW3q32360CEbo1nEhw2nVE4W0om78b87C0yE465o-cw5Mx62G3i0Bo7O2l0Fwqo31wnEfovwRwlE-U2zxe2Gew9O22362W2K0zK5o4q0GpovU1aUbodEGdwtU2ewbS1LwTwNwLw8O1pwr82gxC',
-            '__csr': 'gyhelk8iS00lnm4oioC2385um28MWawVwt40km2Ordg-cGu3C4E6-2QfoJ4m8g80x6wbC0E41Jy30sQ13g0E06V08M42eNE8k0wg88gzBe',
-            '__comet_req': '29',
-            'lsd': 'I5silyPfeZJQAyrhqVdqGB',
-            'jazoest': '22056',
-            '__spin_r': '1007798382',
-            '__spin_b': 'trunk',
-            '__spin_t': '1688680883',
-            '__jssesw': '1',
-            'fb_api_caller_class': 'RelayModern',
-            'fb_api_req_friendly_name': 'BarcelonaProfileThreadsTabQuery',
-            'variables': f'{{"userID":"{user_id}"}}',
-            'server_timestamps': 'true',
-            'doc_id': '6232751443445612'
-        }
-
+                'lsd': self.FBLSDToken,
+                'variables': json.dumps(
+                    {
+                        'userID': user_id,
+                    }
+                ),
+                'doc_id': '6307072669391286'
+            }
+        
         async with aiohttp.ClientSession() as session:
-            async with session.post(url, headers=headers, data=payload) as response:
+            async with session.post(url, headers=modified_headers, data=payload) as response:
                 try:
                     text = await response.text()
                     data = json.loads(text)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         threads = data['data']['mediaData']['threads']
         return threads
     
-    async def get_user_profile_replies(self, username: str, user_id: str):
+    async def get_user_replies(self, user_id: str):
+        """
+        Retrieves the replies associated with a user with the provided user ID.
+
+        Args:
+            user_id (str): The user ID for which to retrieve the replies.
+
+        Returns:
+            list: A list of dictionaries representing the replies associated with the user.
+
+        Raises:
+            Exception: If an error occurs during the thread retrieval process.
+        """
         url = 'https://www.threads.net/api/graphql'
-        headers = {
-            'authority': 'www.threads.net',
-            'accept': '*/*',
-            'accept-language': 'en-US,en;q=0.9',
-            'content-type': 'application/x-www-form-urlencoded',
-            'origin': 'https://www.threads.net',
-            'referer': 'https://www.threads.net/@zuck/replies',
-            'sec-ch-prefers-color-scheme': 'light',
-            'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
-            'sec-ch-ua-full-version-list': '"Not.A/Brand";v="8.0.0.0", "Chromium";v="114.0.5735.199", "Google Chrome";v="114.0.5735.199"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': 'Windows',
-            'sec-ch-ua-platform-version': '15.0.0',
+
+        modified_headers = copy.deepcopy(await self._get_public_headers())
+
+        modified_headers.update({
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-origin',
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
-            'viewport-width': '897',
-            'x-asbd-id': '129477',
             'x-fb-friendly-name': 'BarcelonaProfileRepliesTabQuery',
-            'x-fb-lsd': 'tu2kTRKO1aZl9rMKmRuq9u',
-            'x-ig-app-id': '238260118697367',
-        }
+            'x-fb-lsd': self.FBLSDToken,
+        })
+        
         payload = {
-            'av': '0',
-            '__user': '0',
-            '__a': '1',
-            '__req': '2',
-            '__hs': '19545.HYP:barcelona_web_pkg.2.1..0.0',
-            'dpr': '1',
-            '__ccg': 'EXCELLENT',
-            '__rev': '1007803729',
-            '__s': 'vg5z1u:dyq74i:zgf5h2',
-            '__hsi': '7253172656040290354',
-            '__dyn': '7xeUmwlEnwn8K2WnFw9-2i5U4e0yoW3q32360CEbo1nEhw2nVE4W0om78b87C0yE465o-cw5Mx62G3i0Bo7O2l0Fwqo31wnEfovwRwlE-U2zxe2Gew9O22362W2K0zK5o4q0GpovU1aUbodEGdwtU2ewbS1LwTwNwLw8O1pwr82gxC',
-            '__csr': 'gA-AlUx9k00lp25u17xS6UvwhUO3gMym8g4Ry82GwwAN0rx11dxW4E4-261wwI7Nw4i0g11l0MgeoJS1KF0Y3MV4m0aj0g8X6G7wt4a0wo-eEU',
-            '__comet_req': '29',
-            'lsd': 'tu2kTRKO1aZl9rMKmRuq9u',
-            'jazoest': '21972',
-            '__spin_r': '1007803729',
-            '__spin_b': 'trunk',
-            '__spin_t': '1688760858',
-            '__jssesw': '1',
-            'fb_api_caller_class': 'RelayModern',
-            'fb_api_req_friendly_name': 'BarcelonaProfileRepliesTabQuery',
-            'variables': '{"userID":"314216"}',
-            'server_timestamps': 'true',
-            'doc_id': '6307072669391286',
-        }
+                'lsd': self.FBLSDToken,
+                'variables': json.dumps(
+                    {
+                        'userID': user_id,
+                    }
+                ),
+                'doc_id': '6307072669391286'
+            }
 
         async with aiohttp.ClientSession() as session:
-            async with session.post(url, headers=headers, data=payload) as response:
+            async with session.post(url, headers=modified_headers, data=payload) as response:
                 try:
                     text = await response.text()
                     data = json.loads(text)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         threads = data['data']['mediaData']['threads']
         return threads
     
-    async def get_post_id_from_url(self, post_url, options=None):
-        url = post_url
-        headers = {
-            "authority": "www.threads.net",
-            "accept": "*/*",
-            'accept-language': 'en-US,en;q=0.9',
-            "cache-control": "no-cache",
-            "origin": "https://www.threads.net",
-            "pragma": "no-cache",
-            "referer": post_url,
-            "x-asbd-id": "129477",
-            "x-fb-lsd": self.fbLSDToken,
-            "x-ig-app-id": "238260118697367",
-        }
+    async def follow_user(self, user_id: str) -> bool:
+        """
+        Follows a user with the given user ID.
+
+        Args:
+            user_id (str): The ID of the user to follow.
+
+        Returns:
+            bool: True if the user was followed successfully, False otherwise.
+
+        Raises:
+            Exception: If an error occurs during the follow process.
+        """
+        if not self.is_logged_in:
+            raise Exception("The action 'follow' can only be perfomed while logged-in")
+        
+        res = await self.__auth_required_post_request(f"{BASE_URL}/friendships/create/{user_id}/")
+        return res["status"] == "ok"
 
+    async def unfollow_user(self, user_id: str) -> bool:
+        """
+        Unfollows a user with the given user ID.
+
+        Args:
+            user_id (str): The ID of the user to unfollow.
+
+        Returns:
+            bool: True if the user was unfollowed successfully, False otherwise.
+
+        Raises:
+            Exception: If an error occurs during the unfollow process.
+        """
+        if not self.is_logged_in:
+            raise Exception("The action 'unfollow' can only be perfomed while logged-in")
+        
+        res = await self.__auth_required_post_request(f"{BASE_URL}/friendships/destroy/{user_id}/")
+        return res["status"] == "ok"
+
+
+    async def get_post_id_from_url(self, post_url):
+        """
+        Retrieves the post ID from a given URL.
+
+        Args:
+            post_url (str): The URL of the post.
+        Returns:
+            str: The post ID if found, or None if the post ID is not found.
+
+        Raises:
+            Exception: If an error occurs during the post ID retrieval process.
+        """        
         async with aiohttp.ClientSession() as session:
-            async with session.get(url, headers=headers) as response:
+            async with session.get(post_url, headers=await self._get_public_headers()) as response:
                 text = await response.text()
 
         text = text.replace('\\s', "").replace('\\n', "")
         post_id = re.search(r'"props":{"post_id":"(\d+)"},', text)
         return post_id.group(1)
 
-    async def get_post(self, thread_id: str):
+    async def get_post(self, post_id: str):
+        """
+        Retrieves the post information for a given post ID.
+
+        Args:
+            post_id (str): The ID of the post.
+
+        Returns:
+            dict: A dictionary representing the post information.
+
+        Raises:
+            Exception: If an error occurs during the post retrieval process.
+        """
         url = 'https://www.threads.net/api/graphql'
-        headers = {
-            'authority': 'www.threads.net',
-            'accept': '*/*',
-            'accept-language': 'en-US,en;q=0.9',
-            'content-type': 'application/x-www-form-urlencoded',
-            'origin': 'https://www.threads.net',
-            'referer': f'https://www.threads.net/t/{thread_id}',
-            'sec-ch-prefers-color-scheme': 'light',
-            'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
-            'sec-ch-ua-full-version-list': '"Not.A/Brand";v="8.0.0.0", "Chromium";v="114.0.5735.199", "Google Chrome";v="114.0.5735.199"',
-            'sec-ch-ua-mobile': '?0',
-            'sec-ch-ua-platform': '"Windows"',
-            'sec-ch-ua-platform-version': '"15.0.0"',
+        
+        modified_headers = copy.deepcopy(await self._get_public_headers())
+
+        modified_headers.update({
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-origin',
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
-            'viewport-width': '897',
-            'x-asbd-id': '129477',
             'x-fb-friendly-name': 'BarcelonaPostPageQuery',
-            'x-fb-lsd': 'bUryVn_O9_i_D9F7WOqEpA',
-            'x-ig-app-id': '238260118697367',
-        }
-
-        payload = {
-        'av': '0',
-        '__user': '0',
-        '__a': '1',
-        '__req': '1',
-        '__hs': '19545.HYP:barcelona_web_pkg.2.1..0.0',
-        'dpr': '1',
-        '__ccg': 'EXCELLENT',
-        '__rev': '1007805316',
-        '__s': 'tygnis:dyq74i:zuyk3e',
-        '__hsi': '7253177132820350526',
-        '__dyn': '7xeUmwlEnwn8K2WnFw9-2i5U4e0yoW3q32360CEbo1nEhw2nVE4W0om78b87C0yE5ufz81s8hwGwQw9m1YwBgao6C0Mo5W3S7Udo5qfK0EUjwGzE2swwwNwKwHw8Xxm16waCm7-0iK2S3qazo7u0zE2ZwrUdUcobU2cwmo6O0A8pw',
-        '__csr': 'hI_yaUBb9sE01kRm1syToiwHc0sW1czEgDc11wwG0Qk1Hw1Co40tixLOw',
-        '__comet_req': '29',
-        'lsd': 'bUryVn_O9_i_D9F7WOqEpA',
-        'jazoest': '21915',
-        '__spin_r': '1007805316',
-        '__spin_b': 'trunk',
-        '__spin_t': '1688761899',
-        '__jssesw': '1',
-        'fb_api_caller_class': 'RelayModern',
-        'fb_api_req_friendly_name': 'BarcelonaPostPageQuery',
-        'variables': '{"postID":"3141737961795561608"}',
-        'server_timestamps': 'true',
-        'doc_id': '6529829603744567',
-        }
+            'x-fb-lsd': self.FBLSDToken,
+        })
         
+        payload = {
+                'lsd': self.FBLSDToken,
+                'variables': json.dumps(
+                    {
+                        'postID': post_id,
+                    }
+                ),
+                'doc_id': '5587632691339264',
+            }
 
         async with aiohttp.ClientSession() as session:
-            async with session.post(url, headers=headers, data=payload) as response:
+            async with session.post(url, headers=modified_headers, data=payload) as response:
                 try:
                     text = await response.text()
                     data = json.loads(text)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         threads = data['data']['data']
         return threads
     
+    async def get_post_likes(self, post_id:int):
+        """
+        Retrieves the likes for a post with the given post ID.
+
+        Args:
+            post_id (int): The ID of the post.
+
+        Returns:
+            list: A list of users who liked the post.
+
+        Raises:
+            Exception: If an error occurs during the post likes retrieval process.
+        """
+        url = 'https://www.threads.net/api/graphql'
+        
+        modified_headers = copy.deepcopy(await self._get_public_headers())
+
+        modified_headers.update({
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'same-origin',
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
+            'x-fb-friendly-name': 'BarcelonaPostPageQuery',
+            'x-fb-lsd': self.FBLSDToken,
+        })
+
+        payload = {
+                'lsd': self.FBLSDToken,
+                'variables': json.dumps(
+                    {
+                        'mediaID': post_id,
+                    }
+                ),
+                'doc_id': '9360915773983802',
+            }
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(url, headers=modified_headers, data=payload) as response:
+                try:
+                    text = await response.text()
+                    data = json.loads(text)
+                except (aiohttp.ContentTypeError, json.JSONDecodeError):
+                    raise Exception('Failed to decode response as JSON')
+
+        return data['data']['likers']['users']
+
     async def post(
         self, caption: str, image_path: str = None, url: str = None, parent_post_id: str = None
     ) -> bool:
+        """
+        Creates a new post with the given caption, image, URL, and parent post ID.
+
+        Args:
+            caption (str): The caption of the post.
+            image_path (str, optional): The path to the image file to be posted. Defaults to None.
+            url (str, optional): The URL to be attached to the post. Defaults to None.
+            parent_post_id (str, optional): The ID of the parent post if this post is a reply. Defaults to None.
+
+        Returns:
+            bool: True if the post was created successfully, False otherwise.
+
+        Raises:
+            Exception: If an error occurs during the post creation process.
+        """
         def __get_app_headers() -> dict:
             headers = {
                 "User-Agent": f"Barcelona 289.0.0.77.109 Android",
                 "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
             }
             if self.token is not None:
                 headers["Authorization"] = f"Bearer IGT:2:{self.token}"
@@ -556,22 +638,8 @@
                 async with session.post(post_url, headers=headers, data=payload) as response:
                     if response.status == 200:
                         return True
                     else:
                         raise Exception("Failed to post")
         except Exception as e:
             print("[ERROR] ", e)
-            raise
-
-    async def follow_user(self, user_id: str) -> bool:
-        if not self.is_logged_in:
-            raise Exception("The action 'follow' can only be perfomed while logged-in")
-        
-        res = await self.__auth_required_post_request(f"{BASE_URL}/friendships/create/{user_id}/")
-        return res["status"] == "ok"
-
-    async def unfollow_user(self, user_id: str) -> bool:
-        if not self.is_logged_in:
-            raise Exception("The action 'unfollow' can only be perfomed while logged-in")
-        
-        res = await self.__auth_required_post_request(f"{BASE_URL}/friendships/destroy/{user_id}/")
-        return res["status"] == "ok"
+            raise
```

### Comparing `threads-api-1.0.8/threads_api.egg-info/PKG-INFO` & `threads-api-1.1.0/threads_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.0.8
+Version: 1.1.0
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -23,15 +23,17 @@
 
 > Unofficial, Reverse-Engineered Python client for Meta's [Threads](https://threads.net).
 
 Inspired by [NPM Threads-API](https://github.com/junhoyeo/threads-api)
 
 # Threads API - Python
 
-Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, post, retrieve user profile information, user IDs and user profile threads.
+Threads API is an unofficial Python client for Meta's Threads API. It allows you to interact with the API to login, read and publish posts, view who liked a post, retrieve user profile information, follow/unfollow and much more.
+
+It is built using `aiohttp` to ease asynchronous execution of the API, for ⚡ super-fast ⚡ results.
 
 Table of content:
 
 * [Demo](#demo)
 * [Getting started](#getting-started)
   * [Installation](#Installation)
 * [Usage Examples](#usage-examples)
@@ -60,15 +62,15 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 async def post():
     threads_api = ThreadsAPI()
-    await threads_api.login(os.environ.get('USERNAME'), os.environ,get('PASSWORD'))
+    await threads_api.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
     result = await threads_api.post("I am posting this from the threads api!")
 
     if result:
         print("Post has been successfully posted")
     else:
         print("Unable to post.")
 
@@ -113,15 +115,15 @@
 async def get_user_profile():
     threads_api = ThreadsAPI()
 
     username = "zuck"
     user_id = await threads_api.get_user_id_from_username(username)
 
     if user_id:
-        user_profile = await threads_api.get_user_profile(username, user_id)
+        user_profile = await threads_api.get_user_profile(user_id)
         print(f"User profile for '{username}':")
         print(f"Name: {user_profile['username']}")
         print(f"Bio: {user_profile['biography']}")
         print(f"Followers: {user_profile['follower_count']}")
     else:
         print(f"User ID not found for username '{username}'")
 ```
@@ -132,25 +134,25 @@
 Name: zuck
 Bio: 
 Followers: 2288633
 ```
 </details>
 
 <details>
-  <summary>"get_user_profile_threads" Function</summary>
+  <summary>"get_user_threads" Function</summary>
 
 ``` python
-async def get_user_profile_threads():
+async def get_user_threads():
     threads_api = ThreadsAPI()
 
     username = "zuck"
     user_id = await threads_api.get_user_id_from_username(username)
 
     if user_id:
-        threads = await threads_api.get_user_profile_threads(username, user_id)
+        threads = await threads_api.get_user_threads(user_id)
         print(f"The threads for user '{username}' are:")
         for thread in threads:
             print(f"Text: {thread['thread_items'][0]['post']['caption']} || Likes: {thread['thread_items'][0]['post']['like_count']}")
     else:
         print(f"User ID not found for username '{username}'")
 
 ```
@@ -167,25 +169,25 @@
 zuck's Post: {'text': "Glad you're all here on day one. Let's build something great together!"} || Likes: 175563
 zuck's Post: {'text': "Let's do this. Welcome to Threads. 🔥"} || Likes: 166987
 ```
 </details>
 
 
 <details>
-  <summary>"get_user_profile_replies" Function</summary>
+  <summary>"get_user_replies" Function</summary>
 
 ``` python
-async def get_user_profile_replies():
+async def get_user_replies():
     threads_api = ThreadsAPI()
 
     username = "zuck"
     user_id = await threads_api.get_user_id_from_username(username)
 
     if user_id:
-        threads = await threads_api.get_user_profile_replies(username, user_id)
+        threads = await threads_api.get_user_replies(user_id)
         print(f"The replies for user '{username}' are:")
         for thread in threads:
             print(f"-\n{thread['thread_items'][0]['post']['user']['username']}'s Post: {thread['thread_items'][0]['post']['caption']} || Likes: {thread['thread_items'][0]['post']['like_count']}")
 
             if len(thread["thread_items"]) > 1:
                 print(f"{username}'s Reply: {thread['thread_items'][1]['post']['caption']} || Likes: {thread['thread_items'][1]['post']['like_count']}\n-")
             else:
@@ -282,14 +284,46 @@
 winchester_757's Reply: {'text': 'If only the meta verse was this good LMAO'} || Likes: 0
 -
 winchester_757's Reply: {'text': 'Only 10 mil more to match the big guy'} || Likes: 0
 ```
 </details>
 
 <details>
+  <summary>"get_post_likes" Function</summary>
+
+``` python
+async def get_post_likes():
+    api = ThreadsAPI()
+    post_url = "https://www.threads.net/t/CuZsgfWLyiI"
+
+    post_id = await api.get_post_id_from_url(post_url)
+
+    likes = await api.get_post_likes(post_id)
+    number_of_likes_to_display = 10
+
+    for user_info in likes[:number_of_likes_to_display]:
+        print(f'Username: {user_info["username"]} || Full Name: {user_info["full_name"]} || Follower Count: {user_info["follower_count"]} ')
+```
+
+Example Output:
+```
+Username: andrew_votava || Full Name: Andrew Votava || Follower Count: 19 
+Username: herson_theeog || Full Name: Herson_theeOG || Follower Count: 323 
+Username: dhruv___kanojia || Full Name: Dhruv🌟 || Follower Count: 38 
+Username: codecrusadepk || Full Name: Code Crusade || Follower Count: 9 
+Username: toxicated_jeshim_007 || Full Name: Jeshim Akhtar Choudhury || Follower Count: 6 
+Username: jay.rex.official || Full Name: Jay Rex || Follower Count: 30 
+Username: jessy.servin || Full Name: Jessica Servín || Follower Count: 343 
+Username: joshxmadrid || Full Name: Josh Madrid || Follower Count: 1092 
+Username: ganjipro || Full Name: Song Ganji || Follower Count: 1649 
+Username: bilalmuhamadi || Full Name: B I L A L  M U H A M A D I || Follower Count: 111 
+```
+</details>
+
+<details>
   <summary>"post" Function</summary>
 
 ``` python
 async def post():
     threads_api = ThreadsAPI()
     # either set USERNAME and PASSWORD as environment variables, or replace these with your actual credentials
     await threads_api.login(os.environ.get('USERNAME'), os.environ.get('PASSWORD'))
@@ -305,33 +339,36 @@
 ```
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
 
-- [x] ✅ Login as User
-- [x] ✅ Write Posts
+- [x] ✅ Login functionality 🔒
+  - [x] 🚧 Cache login token securely (reduce login requests)
+- [x] ✅ Write Posts (Requires Login 🔒)
   - [x] ✅ Posts with just text
   - [x] ✅ Posts with text and an image
   - [x] ✅ Posts with text that share a url
-- [x] ✅ Perform Actions
+  - [ ] 🚧 Post with text and share a video
+  - [ ] 🚧 Reply to Posts
+- [x] ✅ Perform Actions (Requires Login 🔒)
   - [x] ✅ Like Posts
   - [x] ✅ Unlike Posts
   - [x] ✅ Follow User
   - [x] ✅ Unfollow User
-- [x] ✅ Read Data\
+- [x] ✅ Read Data
   - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
-  - [x] ✅ Read user profile info
-  - [x] ✅ Read list of user Threads
-  - [x] ✅ Read list of user Replies
+  - [x] ✅ Read a user's profile info
+  - [x] ✅ Read list of a user's Threads
+  - [x] ✅ Read list of a user's Replies
   - [x] ✅ Read Post and a list of its Replies
-- [ ] 🚧  Upload images and videos
-- [ ] 🚧  Reply to Posts
+  - [x] ✅ View who liked a post
 - [x] ✅  CI/CD
-  - [ ] 🚧  Pytest
   - [x] ✅  GitHub Actions Pipeline
+  - [ ] 🚧  Pytest
 
 
 # License
 This project is licensed under the MIT license.
 
+
```

