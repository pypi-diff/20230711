# Comparing `tmp/threads-api-1.1.0.tar.gz` & `tmp/threads-api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.1.0.tar", last modified: Tue Jul 11 20:10:55 2023, max compression
+gzip compressed data, was "threads-api-1.1.1.tar", last modified: Tue Jul 11 21:03:15 2023, max compression
```

## Comparing `threads-api-1.1.0.tar` & `threads-api-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:10:55.808246 threads-api-1.1.0/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.0/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    12721 2023-07-11 20:10:55.808246 threads-api-1.1.0/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    12191 2023-07-11 20:10:30.000000 threads-api-1.1.0/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      384 2023-07-11 20:06:05.000000 threads-api-1.1.0/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-11 20:10:55.808246 threads-api-1.1.0/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      768 2023-07-11 20:05:14.000000 threads-api-1.1.0/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:10:55.804246 threads-api-1.1.0/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.0/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:10:55.804246 threads-api-1.1.0/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.0/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    25004 2023-07-11 20:06:05.000000 threads-api-1.1.0/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:10:55.808246 threads-api-1.1.0/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.0/threads_api/tests/__init__.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      406 2023-07-11 20:05:14.000000 threads-api-1.1.0/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 20:10:55.804246 threads-api-1.1.0/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    12721 2023-07-11 20:10:55.000000 threads-api-1.1.0/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-11 20:10:55.000000 threads-api-1.1.0/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-11 20:10:55.000000 threads-api-1.1.0/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-11 20:10:55.000000 threads-api-1.1.0/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-11 20:10:55.000000 threads-api-1.1.0/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 21:03:15.113644 threads-api-1.1.1/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.1/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12748 2023-07-11 21:03:15.113644 threads-api-1.1.1/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12218 2023-07-11 21:00:43.000000 threads-api-1.1.1/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      409 2023-07-11 21:00:43.000000 threads-api-1.1.1/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-11 21:03:15.113644 threads-api-1.1.1/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      768 2023-07-11 21:00:43.000000 threads-api-1.1.1/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 21:03:15.109644 threads-api-1.1.1/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.1/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 21:03:15.113644 threads-api-1.1.1/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.1/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    28252 2023-07-11 21:00:43.000000 threads-api-1.1.1/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 21:03:15.113644 threads-api-1.1.1/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.1/threads_api/tests/__init__.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      406 2023-07-11 20:05:14.000000 threads-api-1.1.1/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 21:03:15.113644 threads-api-1.1.1/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12748 2023-07-11 21:03:15.000000 threads-api-1.1.1/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-11 21:03:15.000000 threads-api-1.1.1/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-11 21:03:15.000000 threads-api-1.1.1/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-11 21:03:15.000000 threads-api-1.1.1/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-11 21:03:15.000000 threads-api-1.1.1/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.1.0/LICENSE` & `threads-api-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.0/PKG-INFO` & `threads-api-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -62,15 +62,15 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 async def post():
     threads_api = ThreadsAPI()
-    await threads_api.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
+    await threads_api.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'), cached_token_path=".token")
     result = await threads_api.post("I am posting this from the threads api!")
 
     if result:
         print("Post has been successfully posted")
     else:
         print("Unable to post.")
 
@@ -340,15 +340,15 @@
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
 
 - [x] ✅ Login functionality 🔒
-  - [x] 🚧 Cache login token securely (reduce login requests)
+  - [x] ✅ Cache login token securely (reduce login requests)
 - [x] ✅ Write Posts (Requires Login 🔒)
   - [x] ✅ Posts with just text
   - [x] ✅ Posts with text and an image
   - [x] ✅ Posts with text that share a url
   - [ ] 🚧 Post with text and share a video
   - [ ] 🚧 Reply to Posts
 - [x] ✅ Perform Actions (Requires Login 🔒)
```

### Comparing `threads-api-1.1.0/README.md` & `threads-api-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 async def post():
     threads_api = ThreadsAPI()
-    await threads_api.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
+    await threads_api.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'), cached_token_path=".token")
     result = await threads_api.post("I am posting this from the threads api!")
 
     if result:
         print("Post has been successfully posted")
     else:
         print("Unable to post.")
 
@@ -323,15 +323,15 @@
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
 
 - [x] ✅ Login functionality 🔒
-  - [x] 🚧 Cache login token securely (reduce login requests)
+  - [x] ✅ Cache login token securely (reduce login requests)
 - [x] ✅ Write Posts (Requires Login 🔒)
   - [x] ✅ Posts with just text
   - [x] ✅ Posts with text and an image
   - [x] ✅ Posts with text that share a url
   - [ ] 🚧 Post with text and share a video
   - [ ] 🚧 Reply to Posts
 - [x] ✅ Perform Actions (Requires Login 🔒)
```

### Comparing `threads-api-1.1.0/setup.py` & `threads-api-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.1.0',
+    version='1.1.1',
     description='Unofficial Python client for Meta Threads.net API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
```

### Comparing `threads-api-1.1.0/threads_api/src/threads_api.py` & `threads-api-1.1.1/threads_api/src/threads_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 import os
 import mimetypes
 import uuid
 import time
 import traceback
 import copy
 
+import secrets
+from base64 import urlsafe_b64encode as b64e, urlsafe_b64decode as b64d
+
+from cryptography.fernet import Fernet
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes
+from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
+
 BASE_URL = "https://i.instagram.com/api/v1"
 LOGIN_URL = BASE_URL + "/bloks/apps/com.bloks.www.bloks.caa.login.async.send_login_request/"
 POST_URL_TEXTONLY = BASE_URL + "/media/configure_text_only_post/"
 POST_URL_IMAGE = BASE_URL + "/media/configure_text_post_app_feed/"
 DEFAULT_HEADERS = {
             'Authority': 'www.threads.net',
             'Accept': '*/*',
@@ -42,23 +50,61 @@
             'X-IG-App-ID': '238260118697367',
         }
 
 class ThreadsAPIOptions:
     def __init__(self, token: Optional[str] = None):
         self.token = token
 
+class SimpleEncDec:
+    backend = default_backend()
+    iterations = 100_000
+
+    @staticmethod
+    def _derive_key(password: bytes, salt: bytes, iterations: int = iterations) -> bytes:
+        """Derive a secret key from a given password and salt"""
+        kdf = PBKDF2HMAC(
+            algorithm=hashes.SHA256(), length=32, salt=salt,
+            iterations=iterations, backend=SimpleEncDec.backend)
+        return b64e(kdf.derive(password))
+
+    @staticmethod
+    def password_encrypt(message: bytes, password: str, iterations: int = iterations) -> bytes:
+        salt = secrets.token_bytes(16)
+        key = SimpleEncDec._derive_key(password.encode(), salt, iterations)
+        return b64e(
+            b'%b%b%b' % (
+                salt,
+                iterations.to_bytes(4, 'big'),
+                b64d(Fernet(key).encrypt(message)),
+            )
+        )
+
+    @staticmethod
+    def password_decrypt(token: bytes, password: str) -> bytes:
+        decoded = b64d(token)
+        salt, iter, token = decoded[:16], decoded[16:20], b64e(decoded[20:])
+        iterations = int.from_bytes(iter, 'big')
+        key = SimpleEncDec._derive_key(password.encode(), salt, iterations)
+        return Fernet(key).decrypt(token)
+
+class LoggedOutException(Exception):
+     def __init__(self, message):            
+        # Call the base class constructor with the parameters it needs
+        super().__init__(message)
+
 class ThreadsAPI:
     def __init__(self, options: Optional[ThreadsAPIOptions] = None):
         self.token = None
         self.user_id = None
 
         if options and options.token:
             self.token = options.token
 
         self.is_logged_in = False
+        self.auth_headers = None
 
         self.FBLSDToken = 'NjppQDEgONsU_1LCzrmp6q'
 
     async def _get_public_headers(self) -> str:
         default_headers = copy.deepcopy(DEFAULT_HEADERS)
         default_headers['X-FB-LSD'] = await self._refresh_public_token()
         return default_headers
@@ -72,33 +118,66 @@
                 token_key_value = re.search('LSD",\\[\\],{"token":"(.*?)"},\\d+\\]', data).group()
                 token_key_value = token_key_value.replace('LSD",[],{"token":"', '')
                 token = token_key_value.split('"')[0]
 
         self.FBLSDToken = token
         return self.FBLSDToken
     
-    async def login(self, username, password):
+    async def login(self, username, password, cached_token_path=None):
         """
         Logs in the user with the provided username and password.
 
         Args:
             username (str): The username for authentication.
             password (str): The password for authentication.
 
         Returns:
             bool: True if the login is successful, False otherwise.
 
         Raises:
             Exception: If the username or password are invalid, or if an error occurs during login.
         """
+        def _save_token_to_cache(cached_token_path, token, password):
+            with open(cached_token_path, "wb") as fd:
+                fd.write(SimpleEncDec.password_encrypt(token.encode(), password))
+            return
+
+        def _get_token_from_cache(cached_token_path, password):
+            with open(cached_token_path, "rb") as fd:
+                encrypted_token = fd.read()
+            return SimpleEncDec.password_decrypt(encrypted_token, password).decode()
+        
+        async def _set_logged_in_state(username, token):
+            self.token = token
+            self.user_id = await self.get_user_id_from_username(username)
+            self.auth_headers = {
+                'Authorization': f'Bearer IGT:2:{self.token}',
+                'User-Agent': 'Barcelona 289.0.0.77.109 Android',
+                'Sec-Fetch-Site': 'same-origin',
+                'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
+            }
+
+            self.is_logged_in = True
+            return
+
         if username is None or password is None:
             raise Exception("Username or password are invalid")
 
         self.username = username
 
+        # Look in cache before logging in.
+        if cached_token_path is not None and os.path.exists(cached_token_path):
+            try:
+                await _set_logged_in_state(username, _get_token_from_cache(cached_token_path, password))
+                
+                return True
+            except LoggedOutException as e:
+                print(f"[Error] {e}. Attempting to re-login.")
+                pass
+            
         try:
             blockVersion = "5f56efad68e1edec7801f630b5c122704ec5378adbee6609a448f105f34a9c73"
             headers = {
                 "User-Agent": "Barcelona 289.0.0.77.109 Android",
                 "Sec-Fetch-Site": "same-origin",
                 "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
             }
@@ -129,24 +208,19 @@
                 raise Exception("Failed to login")
 
             pos = data.split("Bearer IGT:2:")
             if len(pos) > 1:
                 pos = pos[1]
                 pos = pos.split("==")[0]
                 token = f"{pos}=="
-                self.token = token
-
-                self.user_id = await self.get_user_id_from_username(username)
-                self.auth_headers = {
-                    'Authorization': f'Bearer IGT:2:{self.token}',
-                    'User-Agent': 'Barcelona 289.0.0.77.109 Android',
-                    'Sec-Fetch-Site': 'same-origin',
-                    'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
-                }
-                self.is_logged_in = True
+                
+                await _set_logged_in_state(username, token)
+                
+                if cached_token_path is not None:
+                    _save_token_to_cache(cached_token_path, token)
                 return True
             else:
                 raise Exception("Error with the login response")
         except Exception as e:
             print("[ERROR] ", e)
             raise
 
@@ -164,18 +238,22 @@
         Args:
             username (str): The username to retrieve the user ID for.
         
         Returns:
             str: The user ID if found, or None if the user ID is not found.
         """
         if self.is_logged_in:
-            url = BASE_URL + "/users/{username}/usernameinfo/"
+            url = BASE_URL + f"/users/{username}/usernameinfo/"
             async with aiohttp.ClientSession() as session:
                 async with session.get(url, headers=self.auth_headers) as response:
                     data = await response.json()
+                    
+                    if 'message' in data and data['message'] == "login_required" or \
+                        'status' in data and data['status'] == 'fail':
+                        raise LoggedOutException(str(data))
                     user_id = int(data['user']['pk'])
                     return user_id
         else:
             url = f"https://www.threads.net/@{username}"
             
             async with aiohttp.ClientSession() as session:
                 async with session.get(url, headers=await self._get_public_headers()) as response:
@@ -635,11 +713,12 @@
 
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.post(post_url, headers=headers, data=payload) as response:
                     if response.status == 200:
                         return True
                     else:
-                        raise Exception("Failed to post")
+                        print(response)
+                        raise Exception("Failed to post. Got response:\n" + str(response))
         except Exception as e:
             print("[ERROR] ", e)
             raise
```

### Comparing `threads-api-1.1.0/threads_api.egg-info/PKG-INFO` & `threads-api-1.1.1/threads_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -62,15 +62,15 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
 async def post():
     threads_api = ThreadsAPI()
-    await threads_api.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'))
+    await threads_api.login(os.environ.get('INSTAGRAM_USERNAME'), os.environ.get('INSTAGRAM_PASSWORD'), cached_token_path=".token")
     result = await threads_api.post("I am posting this from the threads api!")
 
     if result:
         print("Post has been successfully posted")
     else:
         print("Unable to post.")
 
@@ -340,15 +340,15 @@
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
 
 - [x] ✅ Login functionality 🔒
-  - [x] 🚧 Cache login token securely (reduce login requests)
+  - [x] ✅ Cache login token securely (reduce login requests)
 - [x] ✅ Write Posts (Requires Login 🔒)
   - [x] ✅ Posts with just text
   - [x] ✅ Posts with text and an image
   - [x] ✅ Posts with text that share a url
   - [ ] 🚧 Post with text and share a video
   - [ ] 🚧 Reply to Posts
 - [x] ✅ Perform Actions (Requires Login 🔒)
```

