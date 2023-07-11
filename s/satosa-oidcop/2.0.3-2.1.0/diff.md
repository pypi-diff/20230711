# Comparing `tmp/satosa_oidcop-2.0.3.tar.gz` & `tmp/satosa_oidcop-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosa_oidcop-2.0.3.tar", last modified: Fri Jul  7 09:48:46 2023, max compression
+gzip compressed data, was "satosa_oidcop-2.1.0.tar", last modified: Tue Jul 11 10:57:52 2023, max compression
```

## Comparing `satosa_oidcop-2.0.3.tar` & `satosa_oidcop-2.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:46.347530 satosa_oidcop-2.0.3/satosa_oidcop/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/satosa_oidcop/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/satosa_oidcop/core/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/user_authn.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/core/user_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    31922 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/satosa_oidcop/idpy_oidcop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-07 09:48:46.000000 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-07 09:48:46.000000 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 09:48:46.000000 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-07 09:48:46.000000 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-07 09:48:46.000000 satosa_oidcop-2.0.3/satosa_oidcop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 09:48:46.351530 satosa_oidcop-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-07 09:48:08.000000 satosa_oidcop-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:57:52.081941 satosa_oidcop-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-11 10:57:52.081941 satosa_oidcop-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:57:52.081941 satosa_oidcop-2.1.0/satosa_oidcop/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:57:52.081941 satosa_oidcop-2.1.0/satosa_oidcop/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/core/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/core/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:57:52.081941 satosa_oidcop-2.1.0/satosa_oidcop/core/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/core/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/core/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/core/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/core/user_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/core/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32833 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/satosa_oidcop/idpy_oidcop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:57:52.081941 satosa_oidcop-2.1.0/satosa_oidcop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-11 10:57:51.000000 satosa_oidcop-2.1.0/satosa_oidcop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-11 10:57:52.000000 satosa_oidcop-2.1.0/satosa_oidcop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:57:51.000000 satosa_oidcop-2.1.0/satosa_oidcop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 10:57:51.000000 satosa_oidcop-2.1.0/satosa_oidcop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 10:57:51.000000 satosa_oidcop-2.1.0/satosa_oidcop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 10:57:52.081941 satosa_oidcop-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-11 10:57:08.000000 satosa_oidcop-2.1.0/setup.py
```

### Comparing `satosa_oidcop-2.0.3/LICENSE` & `satosa_oidcop-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.3/PKG-INFO` & `satosa_oidcop-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosa_oidcop
-Version: 2.0.3
+Version: 2.1.0
 Summary: SATOSA Frontend based on idetity python oidcop
 Home-page: https://github.com/UniversitaDellaCalabria/satosa-oidcop
 Author: Giuseppe De Marco
 Author-email: giuseppe.demarco@unical.it
 License: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `satosa_oidcop-2.0.3/README.md` & `satosa_oidcop-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.3/satosa_oidcop/core/application.py` & `satosa_oidcop-2.1.0/satosa_oidcop/core/application.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.3/satosa_oidcop/core/claims.py` & `satosa_oidcop-2.1.0/satosa_oidcop/core/claims.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.3/satosa_oidcop/core/storage/base.py` & `satosa_oidcop-2.1.0/satosa_oidcop/core/storage/base.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.3/satosa_oidcop/core/storage/mongo.py` & `satosa_oidcop-2.1.0/satosa_oidcop/core/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.3/satosa_oidcop/core/user_authn.py` & `satosa_oidcop-2.1.0/satosa_oidcop/core/user_authn.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.3/satosa_oidcop/core/user_info.py` & `satosa_oidcop-2.1.0/satosa_oidcop/core/user_info.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.3/satosa_oidcop/idpy_oidcop.py` & `satosa_oidcop-2.1.0/satosa_oidcop/idpy_oidcop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 The OpenID Connect frontend module for the satosa proxy
 """
 import base64
 import logging
 import os
 from urllib.parse import urlencode
+from datetime import datetime
 
 from cryptojwt.key_jar import KeyJar
 from idpyoidc.message.oauth2 import ResponseMessage
 from idpyoidc.message.oidc import AccessTokenRequest
 from idpyoidc.message.oidc import AuthnToken
 from idpyoidc.message.oidc import AuthorizationErrorResponse
 from idpyoidc.message.oidc import AuthorizationRequest
@@ -17,14 +18,20 @@
 from idpyoidc.server.exception import ClientAuthenticationError
 from idpyoidc.server.exception import NoSuchGrant
 from idpyoidc.server.exception import InvalidClient
 from idpyoidc.server.exception import UnAuthorizedClient
 from idpyoidc.server.exception import UnknownClient
 from idpyoidc.server.oidc.registration import random_client_id
 from satosa.context import Context
+try:
+    from satosa.context import add_prompt_to_context
+except ImportError:
+    # TODO: remove after https://github.com/IdentityPython/SATOSA/pull/419 is merged
+    def add_prompt_to_context(*args, **kwargs):
+        pass
 from satosa.frontends.base import FrontendModule
 from satosa.internal import InternalData
 import satosa.logging_util as lu
 from satosa.response import SeeOther
 
 from .core.application import oidcop_application as oidcop_app
 from .core.claims import combine_claim_values
@@ -230,14 +237,26 @@
         """
         Processes an OAuth2/OIDC request
         used by Authorization, Token, Userinfo and Introspection enpoints views
         """
         if isinstance(parse_req, JsonResponse):
             return self.send_response(parse_req)
 
+        # do not handle prompt param by oidc-op, handle it here instead
+        prompt_arg = parse_req.pop("prompt", None)
+        if prompt_arg:
+            add_prompt_to_context(context, " ".join(prompt_arg) if isinstance(prompt_arg, list) else prompt_arg)
+
+        # save ACRs
+        acr_values = parse_req.pop("acr_values", None)
+        if acr_values:
+            acr_values = acr_values if isinstance(acr_values, list) else acr_values.split(" ")
+            context.decorate(Context.KEY_AUTHN_CONTEXT_CLASS_REF, acr_values)
+            context.state[Context.KEY_AUTHN_CONTEXT_CLASS_REF] = acr_values
+
         try:
             proc_req = endpoint.process_request(
                 parse_req, http_info=http_headers)
             return proc_req
         except Exception as err:  # pragma: no cover
             logger.error(
                 f"In endpoint.process_request: {parse_req.__dict__} - {err}")
@@ -708,17 +727,16 @@
 
         client_id = parse_req["client_id"]
         sub = internal_resp.subject_id
 
         authn_event = create_authn_event(
             uid=sub,
             salt=base64.b64encode(os.urandom(self.app.salt_size)).decode(),
-            # TODO
-            # authn_info=auth_args['authn_class_ref'],
-            # authn_time=auth_args['iat']
+            authn_info=internal_resp.auth_info.auth_class_ref,
+            # TODO: authn_time=datetime.fromisoformat(internal_resp.auth_info.timestamp).timestamp(),
         )
 
         _ec = endpoint.upstream_get("context")
         _token_usage_rules = _ec.authn_broker.get_method_by_id("user")
 
         session_manager = _ec.session_manager
         client = self.app.storage.get_client_by_id(client_id)
```

### Comparing `satosa_oidcop-2.0.3/satosa_oidcop.egg-info/PKG-INFO` & `satosa_oidcop-2.1.0/satosa_oidcop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satosa-oidcop
-Version: 2.0.3
+Version: 2.1.0
 Summary: SATOSA Frontend based on idetity python oidcop
 Home-page: https://github.com/UniversitaDellaCalabria/satosa-oidcop
 Author: Giuseppe De Marco
 Author-email: giuseppe.demarco@unical.it
 License: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `satosa_oidcop-2.0.3/satosa_oidcop.egg-info/SOURCES.txt` & `satosa_oidcop-2.1.0/satosa_oidcop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-2.0.3/setup.py` & `satosa_oidcop-2.1.0/setup.py`

 * *Files identical despite different names*

