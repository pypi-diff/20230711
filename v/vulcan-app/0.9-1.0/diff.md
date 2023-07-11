# Comparing `tmp/vulcan-app-0.9.tar.gz` & `tmp/vulcan-app-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-app-0.9.tar", last modified: Fri Feb 24 10:17:14 2023, max compression
+gzip compressed data, was "vulcan-app-1.0.tar", last modified: Tue Jul 11 08:28:41 2023, max compression
```

## Comparing `vulcan-app-0.9.tar` & `vulcan-app-1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:17:14.643606 vulcan-app-0.9/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-15 10:28:00.000000 vulcan-app-0.9/LICENSE
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-02-24 10:17:14.643606 vulcan-app-0.9/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       62 2023-02-15 10:28:00.000000 vulcan-app-0.9/README.md
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-02-24 10:17:14.647606 vulcan-app-0.9/setup.cfg
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1157 2023-02-24 10:17:08.000000 vulcan-app-0.9/setup.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:17:14.643606 vulcan-app-0.9/vulcan_app/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      472 2023-02-15 13:42:27.000000 vulcan-app-0.9/vulcan_app/__init__.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      805 2023-02-23 08:06:39.000000 vulcan-app-0.9/vulcan_app/configuration.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:17:14.643606 vulcan-app-0.9/vulcan_app/database/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1520 2023-02-23 13:43:03.000000 vulcan-app-0.9/vulcan_app/database/__init__.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      251 2023-02-15 06:39:24.000000 vulcan-app-0.9/vulcan_app/database/mongo.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1257 2023-02-15 06:59:22.000000 vulcan-app-0.9/vulcan_app/database/postgre.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      686 2023-01-09 13:08:56.000000 vulcan-app-0.9/vulcan_app/database/tunnel.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     5132 2023-02-15 13:40:54.000000 vulcan-app-0.9/vulcan_app/security.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2442 2023-02-15 10:40:00.000000 vulcan-app-0.9/vulcan_app/services.py
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2860 2023-02-12 04:50:57.000000 vulcan-app-0.9/vulcan_app/worklog_processor.py
-drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-02-24 10:17:14.643606 vulcan-app-0.9/vulcan_app.egg-info/
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-02-24 10:17:14.000000 vulcan-app-0.9/vulcan_app.egg-info/PKG-INFO
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      446 2023-02-24 10:17:14.000000 vulcan-app-0.9/vulcan_app.egg-info/SOURCES.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-02-24 10:17:14.000000 vulcan-app-0.9/vulcan_app.egg-info/dependency_links.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      161 2023-02-24 10:17:14.000000 vulcan-app-0.9/vulcan_app.egg-info/requires.txt
--rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       11 2023-02-24 10:17:14.000000 vulcan-app-0.9/vulcan_app.egg-info/top_level.txt
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 08:28:41.440645 vulcan-app-1.0/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1073 2023-02-15 10:28:00.000000 vulcan-app-1.0/LICENSE
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-07-11 08:28:41.440645 vulcan-app-1.0/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       62 2023-02-15 10:28:00.000000 vulcan-app-1.0/README.md
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       38 2023-07-11 08:28:41.440645 vulcan-app-1.0/setup.cfg
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1157 2023-07-11 08:27:55.000000 vulcan-app-1.0/setup.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 08:28:41.440645 vulcan-app-1.0/vulcan_app/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      475 2023-07-11 08:23:00.000000 vulcan-app-1.0/vulcan_app/__init__.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      805 2023-02-23 08:06:39.000000 vulcan-app-1.0/vulcan_app/configuration.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 08:28:41.440645 vulcan-app-1.0/vulcan_app/database/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1520 2023-02-23 13:43:03.000000 vulcan-app-1.0/vulcan_app/database/__init__.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      251 2023-02-15 06:39:24.000000 vulcan-app-1.0/vulcan_app/database/mongo.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     1257 2023-02-15 06:59:22.000000 vulcan-app-1.0/vulcan_app/database/postgre.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      686 2023-01-09 13:08:56.000000 vulcan-app-1.0/vulcan_app/database/tunnel.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     5693 2023-07-11 08:26:50.000000 vulcan-app-1.0/vulcan_app/security.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2442 2023-02-15 10:40:00.000000 vulcan-app-1.0/vulcan_app/services.py
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)     2860 2023-07-04 14:18:15.000000 vulcan-app-1.0/vulcan_app/worklog_processor.py
+drwxrwxr-x   0 pvirie    (1000) pvirie    (1000)        0 2023-07-11 08:28:41.440645 vulcan-app-1.0/vulcan_app.egg-info/
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      522 2023-07-11 08:28:41.000000 vulcan-app-1.0/vulcan_app.egg-info/PKG-INFO
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      446 2023-07-11 08:28:41.000000 vulcan-app-1.0/vulcan_app.egg-info/SOURCES.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)        1 2023-07-11 08:28:41.000000 vulcan-app-1.0/vulcan_app.egg-info/dependency_links.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)      161 2023-07-11 08:28:41.000000 vulcan-app-1.0/vulcan_app.egg-info/requires.txt
+-rw-rw-r--   0 pvirie    (1000) pvirie    (1000)       11 2023-07-11 08:28:41.000000 vulcan-app-1.0/vulcan_app.egg-info/top_level.txt
```

### Comparing `vulcan-app-0.9/LICENSE` & `vulcan-app-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.9/PKG-INFO` & `vulcan-app-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-app
-Version: 0.9
+Version: 1.0
 Summary: Vulcan's web application server.
 Home-page: https://github.com/vulcan-coalition/vulcan-app.git
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vulcan-app-0.9/setup.py` & `vulcan-app-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from distutils.core import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="vulcan-app",
-    version="0.9",
+    version="1.0",
     author="Chatavut Viriyasuthee",
     author_email="chatavut@lab.ai",
     description="Vulcan's web application server.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vulcan-coalition/vulcan-app.git",
     packages=["vulcan_app", "vulcan_app.database"],
```

### Comparing `vulcan-app-0.9/vulcan_app/configuration.py` & `vulcan-app-1.0/vulcan_app/configuration.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.9/vulcan_app/database/__init__.py` & `vulcan-app-1.0/vulcan_app/database/__init__.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.9/vulcan_app/database/postgre.py` & `vulcan-app-1.0/vulcan_app/database/postgre.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.9/vulcan_app/database/tunnel.py` & `vulcan-app-1.0/vulcan_app/database/tunnel.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.9/vulcan_app/security.py` & `vulcan-app-1.0/vulcan_app/security.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-from fastapi import Depends, HTTPException, status, Form, Header
+from fastapi import Depends, HTTPException, status, Form, Header, APIRouter
 from fastapi.security import OAuth2PasswordBearer, OAuth2PasswordRequestForm
 from typing import Optional
 import jwt
 from pydantic import BaseModel
 from datetime import datetime, timedelta
 from .configuration import get_config
 from .services import *
 
 
-bypass_security = get_config("test")
-
 # to get a string like this run:
 # openssl rand -hex 32
-SECRET_KEY = get_config("secret_key")
 ALGORITHM = "HS256"
 ACCESS_TOKEN_EXPIRE_MINUTES = 24 * 60
 REFRESH_TOKEN_EXPIRE_MINUTES = 24 * 60 * 5
 
 
 def create_access_token(data: dict, expires_delta: Optional[timedelta] = timedelta(minutes=15)):
+    SECRET_KEY = get_config("secret_key")
     expire = datetime.utcnow() + expires_delta
     to_encode = data.copy()
     to_encode.update({"exp": expire})
     encoded_jwt = jwt.encode(to_encode, SECRET_KEY, algorithm=ALGORITHM)
     return encoded_jwt
 
 
@@ -50,14 +48,15 @@
     status_code=status.HTTP_401_UNAUTHORIZED,
     detail="Could not validate credentials",
     headers={"Authorization": "Bearer"},
 )
 
 
 def decode_token(token: str):
+    SECRET_KEY = get_config("secret_key")
     try:
         payload = jwt.decode(token, SECRET_KEY, algorithms=[ALGORITHM])
         email: str = payload.get("email")
         exp = payload.get("exp")
         disability = payload.get("disability")
         expired = datetime.now() > datetime.fromtimestamp(exp)
         if expired:
@@ -72,93 +71,96 @@
             detail="Token is expired.",
             headers={"WWW-Authenticate": "Bearer"},
         )
 
     return email, disability
 
 
-async def get_active_current_user(Authorization: str = Header(None)):
-
-    if Authorization is None:
-        raise HTTPException(
-            status_code=status.HTTP_401_UNAUTHORIZED,
-            detail="Token is missing.",
-            headers={"WWW-Authenticate": "Bearer"},
-        )
-
-    token = Authorization[len("Bearer "):]
-
-    if bypass_security:
-        return User(email="testuser@vulcan", disability=0)
-
-    email, disability = decode_token(token)
-
-    user = User(email=email, disability=disability)
-    return user
-
-
 class Token(BaseModel):
     access_token: str
     refresh_token: str
     token_type: str
 
 
-def initialize(app):
+def initialize(app, security_prefix=""):
 
-    @app.post("/exchange", response_model=Token)
-    async def exchange_access_token(token: str = Form(...)):
+    router = APIRouter(prefix=security_prefix, tags=[security_prefix[1:] if security_prefix.startswith("/") else security_prefix])
 
+    @router.post("/exchange", response_model=Token)
+    async def exchange_access_token(token: str = Form(...)):
+        bypass_security = get_config("test")
         if bypass_security:
             userdata = {'email': "testuser@vulcan", 'disability': 0}
         else:
             result, userdata = await login(token)
             if not result:
                 raise HTTPException(
                     status_code=status.HTTP_401_UNAUTHORIZED,
                     detail="Incorrect username or password",
                     headers={"WWW-Authenticate": "Bearer"},
                 )
 
         return create_tokens(userdata)
 
-    @app.post('/refresh', response_model=Token)
+    @router.post('/refresh', response_model=Token)
     async def refresh_token(refresher: str = Form(...)):
 
         email, disability = decode_token(refresher)
 
         return create_tokens({"email": email, "disability": disability})
 
-    @app.post("/token", response_model=Token)
+    @router.post("/token", response_model=Token)
     async def login_for_admin_token(form_data: OAuth2PasswordRequestForm = Depends()):
-
+        bypass_security = get_config("test")
         if bypass_security:
             userdata = {'email': "testuser@vulcan", 'data': True}
         else:
             result, userdata = await admin_login(form_data.username, form_data.password)
             if not result:
                 raise HTTPException(
                     status_code=status.HTTP_401_UNAUTHORIZED,
                     detail="Incorrect username or password",
                     headers={"WWW-Authenticate": "Bearer"},
                 )
             userdata["data"] = True
 
         return create_tokens(userdata)
 
+    app.include_router(router)
 
-oauth2_scheme = OAuth2PasswordBearer(tokenUrl="token")
+    async def get_active_current_user(Authorization: str = Header(None)):
+        bypass_security = get_config("test")
+        if Authorization is None:
+            raise HTTPException(
+                status_code=status.HTTP_401_UNAUTHORIZED,
+                detail="Token is missing.",
+                headers={"WWW-Authenticate": "Bearer"},
+            )
 
+        token = Authorization[len("Bearer "):]
 
-async def check_is_admin(token: str = Depends(oauth2_scheme)):
+        if bypass_security:
+            return User(email="testuser@vulcan", disability=0)
 
-    try:
-        payload = jwt.decode(token, SECRET_KEY, algorithms=[ALGORITHM])
-        email: str = payload.get("email")
-        exp = payload.get("exp")
-        data = payload.get("data")
-        expired = datetime.now() > datetime.fromtimestamp(exp)
-        if email is None or expired or data is None:
+        email, disability = decode_token(token)
+
+        user = User(email=email, disability=disability)
+        return user
+
+    oauth2_scheme = OAuth2PasswordBearer(tokenUrl=security_prefix + "/token")
+
+    async def check_is_admin(token: str = Depends(oauth2_scheme)):
+        SECRET_KEY = get_config("secret_key")
+        try:
+            payload = jwt.decode(token, SECRET_KEY, algorithms=[ALGORITHM])
+            email: str = payload.get("email")
+            exp = payload.get("exp")
+            data = payload.get("data")
+            expired = datetime.now() > datetime.fromtimestamp(exp)
+            if email is None or expired or data is None:
+                raise credentials_exception
+        except jwt.DecodeError:
             raise credentials_exception
-    except jwt.DecodeError:
-        raise credentials_exception
 
-    return True
+        return True
+
+    return get_active_current_user, check_is_admin
```

### Comparing `vulcan-app-0.9/vulcan_app/services.py` & `vulcan-app-1.0/vulcan_app/services.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.9/vulcan_app/worklog_processor.py` & `vulcan-app-1.0/vulcan_app/worklog_processor.py`

 * *Files identical despite different names*

### Comparing `vulcan-app-0.9/vulcan_app.egg-info/PKG-INFO` & `vulcan-app-1.0/vulcan_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-app
-Version: 0.9
+Version: 1.0
 Summary: Vulcan's web application server.
 Home-page: https://github.com/vulcan-coalition/vulcan-app.git
 Author: Chatavut Viriyasuthee
 Author-email: chatavut@lab.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

