# Comparing `tmp/hrequests-0.3.0.tar.gz` & `tmp/hrequests-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrequests-0.3.0.tar", max compression
+gzip compressed data, was "hrequests-0.4.0.tar", max compression
```

## Comparing `hrequests-0.3.0.tar` & `hrequests-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.3.0/hrequests/__init__.py
--rw-r--r--   0        0        0      143 2023-07-09 08:44:09.084639 hrequests-0.3.0/hrequests/__version__.py
--rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.3.0/hrequests/bin/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.3.0/hrequests/bin/LICENSE.txt
--rw-r--r--   0        0        0    23097 2023-07-08 02:07:11.879627 hrequests-0.3.0/hrequests/browser.py
--rw-r--r--   0        0        0     2771 2023-07-07 18:22:10.146220 hrequests-0.3.0/hrequests/cffi.py
--rw-r--r--   0        0        0    15622 2023-07-08 00:43:33.012698 hrequests-0.3.0/hrequests/client.py
--rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.3.0/hrequests/cookies.py
--rw-r--r--   0        0        0      723 2023-07-09 08:14:06.945274 hrequests-0.3.0/hrequests/exceptions.py
--rw-r--r--   0        0        0    19488 2023-07-09 08:47:23.150659 hrequests-0.3.0/hrequests/parser.py
--rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.3.0/hrequests/playwright_mock/__init__.py
--rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.3.0/hrequests/playwright_mock/context.py
--rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.3.0/hrequests/playwright_mock/element_handle.py
--rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.3.0/hrequests/playwright_mock/faker.py
--rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.3.0/hrequests/playwright_mock/frame.py
--rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.3.0/hrequests/playwright_mock/frame_locator.py
--rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.3.0/hrequests/playwright_mock/js_handle.py
--rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.3.0/hrequests/playwright_mock/locale.json
--rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.3.0/hrequests/playwright_mock/locator.py
--rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.3.0/hrequests/playwright_mock/mouse.py
--rw-r--r--   0        0        0    17529 2023-07-07 19:00:57.200997 hrequests-0.3.0/hrequests/playwright_mock/page.py
--rw-r--r--   0        0        0     1823 2023-07-08 02:07:11.739522 hrequests-0.3.0/hrequests/playwright_mock/playwright_mock.py
--rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.3.0/hrequests/playwright_mock/proxy_manager.py
--rw-r--r--   0        0        0    13464 2023-07-08 02:07:11.860477 hrequests-0.3.0/hrequests/reqs.py
--rw-r--r--   0        0        0     7501 2023-07-08 02:07:11.851360 hrequests-0.3.0/hrequests/response.py
--rw-r--r--   0        0        0    11715 2023-07-08 02:54:30.797972 hrequests-0.3.0/hrequests/session.py
--rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.3.0/LICENSE
--rw-r--r--   0        0        0     1022 2023-07-09 08:44:14.453438 hrequests-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    32070 2023-07-09 08:42:09.963610 hrequests-0.3.0/README.md
--rw-r--r--   0        0        0    32516 1970-01-01 00:00:00.000000 hrequests-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.4.0/hrequests/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-11 01:20:05.895609 hrequests-0.4.0/hrequests/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.4.0/hrequests/bin/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.4.0/hrequests/bin/LICENSE.txt
+-rw-r--r--   0        0        0    23097 2023-07-08 02:07:11.879627 hrequests-0.4.0/hrequests/browser.py
+-rw-r--r--   0        0        0     2771 2023-07-07 18:22:10.146220 hrequests-0.4.0/hrequests/cffi.py
+-rw-r--r--   0        0        0    14008 2023-07-10 23:07:26.244002 hrequests-0.4.0/hrequests/client.py
+-rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.4.0/hrequests/cookies.py
+-rw-r--r--   0        0        0      723 2023-07-09 08:14:06.945274 hrequests-0.4.0/hrequests/exceptions.py
+-rw-r--r--   0        0        0    19488 2023-07-09 08:47:23.150659 hrequests-0.4.0/hrequests/parser.py
+-rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.4.0/hrequests/playwright_mock/__init__.py
+-rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.4.0/hrequests/playwright_mock/context.py
+-rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.4.0/hrequests/playwright_mock/element_handle.py
+-rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.4.0/hrequests/playwright_mock/faker.py
+-rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.4.0/hrequests/playwright_mock/frame.py
+-rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.4.0/hrequests/playwright_mock/frame_locator.py
+-rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.4.0/hrequests/playwright_mock/js_handle.py
+-rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.4.0/hrequests/playwright_mock/locale.json
+-rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.4.0/hrequests/playwright_mock/locator.py
+-rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.4.0/hrequests/playwright_mock/mouse.py
+-rw-r--r--   0        0        0    17529 2023-07-07 19:00:57.200997 hrequests-0.4.0/hrequests/playwright_mock/page.py
+-rw-r--r--   0        0        0     1823 2023-07-08 02:07:11.739522 hrequests-0.4.0/hrequests/playwright_mock/playwright_mock.py
+-rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.4.0/hrequests/playwright_mock/proxy_manager.py
+-rw-r--r--   0        0        0    13766 2023-07-10 18:59:11.917298 hrequests-0.4.0/hrequests/reqs.py
+-rw-r--r--   0        0        0     8573 2023-07-11 01:26:16.315730 hrequests-0.4.0/hrequests/response.py
+-rw-r--r--   0        0        0    11808 2023-07-11 01:15:28.768157 hrequests-0.4.0/hrequests/session.py
+-rw-r--r--   0        0        0     4715 2023-07-11 01:15:09.826071 hrequests-0.4.0/hrequests/toolbelt.py
+-rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1022 2023-07-11 01:20:04.224146 hrequests-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    32506 2023-07-11 01:17:13.695947 hrequests-0.4.0/README.md
+-rw-r--r--   0        0        0    32945 1970-01-01 00:00:00.000000 hrequests-0.4.0/PKG-INFO
```

### Comparing `hrequests-0.3.0/hrequests/bin/LICENSE.txt` & `hrequests-0.4.0/hrequests/bin/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/browser.py` & `hrequests-0.4.0/hrequests/browser.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/cffi.py` & `hrequests-0.4.0/hrequests/cffi.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/client.py` & `hrequests-0.4.0/hrequests/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import base64
 import ctypes
 import urllib.parse
 import uuid
-from collections import OrderedDict
-from typing import Mapping, MutableMapping, Optional, Union
+from typing import Optional, Union
 
 from orjson import dumps, loads
 
 import hrequests
+from .toolbelt import CaseInsensitiveDict
 
 from .cffi import freeMemory, request
 from .cookies import (
+    RequestsCookieJar,
     cookiejar_from_dict,
     cookiejar_to_list,
-    list_to_cookiejar,
     extract_cookies_to_jar,
+    list_to_cookiejar,
     merge_cookies,
-    RequestsCookieJar,
 )
 from .exceptions import ClientException
 
 '''
 TLSClient heavily based on https://github.com/FlorianREGAZ/Python-Tls-Client
 Copyright (c) 2022 Florian Zager
 '''
@@ -269,28 +269,23 @@
         # debugging
         self.debug = debug
 
     def execute_request(
         self,
         method: str,
         url: str,
-        params: Optional[dict] = None,  # Optional[dict[str, str]]
-        data: Optional[Union[str, dict]] = None,
-        headers: Optional[dict] = None,  # Optional[dict[str, str]]
+        data: Optional[Union[str, bytes, bytearray, dict]] = None,
+        headers: Optional[Union[dict, CaseInsensitiveDict]] = None,  # Optional[dict[str, str]]
         cookies: Optional[Union[RequestsCookieJar, dict, list]] = None,  # Optional[dict[str, str]]
         json: Optional[Union[dict, list, str]] = None,  # Optional[dict]
         allow_redirects: Optional[bool] = False,
         insecure_skip_verify: Optional[bool] = False,
         timeout_seconds: int = 30,
         proxy: Optional[dict] = None,  # Optional[dict[str, str]]
     ):
-        # Prepare URL - add params to url
-        if params is not None:
-            url = f'{url}?{urllib.parse.urlencode(params, doseq=True)}'
-
         # Prepare request body - build request body
         # Data has priority. JSON is only used if data is None.
         if data is None and json is not None:
             if type(json) in (dict, list):
                 json = dumps(json).decode('utf-8')
             request_body = json
             content_type = 'application/json'
@@ -344,15 +339,15 @@
         is_byte_request = isinstance(request_body, (bytes, bytearray))
         request_payload = {
             'sessionId': self._session_id,
             'followRedirects': allow_redirects,
             'forceHttp1': self.force_http1,
             'withDebug': self.debug,
             'catchPanics': self.catch_panics,
-            'headers': dict(headers),
+            'headers': dict(headers) if isinstance(headers, CaseInsensitiveDict) else headers,
             'headerOrder': self.header_order,
             'insecureSkipVerify': insecure_skip_verify,
             'isByteRequest': is_byte_request,
             'additionalDecode': self.additional_decode,
             'proxyUrl': proxy,
             'requestUrl': url,
             'requestMethod': method,
@@ -401,56 +396,7 @@
             request_url=url,
             request_headers=headers,
             cookie_jar=self.cookies,
             response_headers=response_object['headers'],
         )
         # build response class
         return hrequests.response.build_response(response_object, response_cookie_jar)
-
-
-class CaseInsensitiveDict(MutableMapping):
-    '''
-    Origin: requests library (https://github.com/psf/requests)
-    A case-insensitive ``dict``-like object.
-    '''
-
-    def __init__(self, data=None, **kwargs):
-        self._store = OrderedDict()
-        if data is None:
-            data = {}
-        self.update(data, **kwargs)
-
-    def __setitem__(self, key, value):
-        # Use the lowercased key for lookups, but store the actual
-        # key alongside the value.
-        self._store[key.lower()] = (key, value)
-
-    def __getitem__(self, key):
-        return self._store[key.lower()][1]
-
-    def __delitem__(self, key):
-        del self._store[key.lower()]
-
-    def __iter__(self):
-        return (casedkey for casedkey, mappedvalue in self._store.values())
-
-    def __len__(self):
-        return len(self._store)
-
-    def lower_items(self):
-        '''Like iteritems(), but with all lowercase keys.'''
-        return ((lowerkey, keyval[1]) for (lowerkey, keyval) in self._store.items())
-
-    def __eq__(self, other):
-        if isinstance(other, Mapping):
-            other = CaseInsensitiveDict(other)
-        else:
-            return NotImplemented
-        # Compare insensitively
-        return dict(self.lower_items()) == dict(other.lower_items())
-
-    # Copy is required
-    def copy(self):
-        return CaseInsensitiveDict(self._store.values())
-
-    def __repr__(self):
-        return str(dict(self.items()))
```

### Comparing `hrequests-0.3.0/hrequests/cookies.py` & `hrequests-0.4.0/hrequests/cookies.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/exceptions.py` & `hrequests-0.4.0/hrequests/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/parser.py` & `hrequests-0.4.0/hrequests/parser.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/context.py` & `hrequests-0.4.0/hrequests/playwright_mock/context.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/element_handle.py` & `hrequests-0.4.0/hrequests/playwright_mock/element_handle.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/faker.py` & `hrequests-0.4.0/hrequests/playwright_mock/faker.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/frame.py` & `hrequests-0.4.0/hrequests/playwright_mock/frame.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/frame_locator.py` & `hrequests-0.4.0/hrequests/playwright_mock/frame_locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/locale.json` & `hrequests-0.4.0/hrequests/playwright_mock/locale.json`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/locator.py` & `hrequests-0.4.0/hrequests/playwright_mock/locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/mouse.py` & `hrequests-0.4.0/hrequests/playwright_mock/mouse.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/page.py` & `hrequests-0.4.0/hrequests/playwright_mock/page.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/playwright_mock.py` & `hrequests-0.4.0/hrequests/playwright_mock/playwright_mock.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/playwright_mock/proxy_manager.py` & `hrequests-0.4.0/hrequests/playwright_mock/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/hrequests/reqs.py` & `hrequests-0.4.0/hrequests/reqs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import traceback
 from functools import partial
 from threading import Thread, get_ident
-from typing import Optional
+from typing import Dict, Optional
 
 import gevent
 from gevent.pool import Pool
 
 import hrequests
 from hrequests.exceptions import NoPauseRuntimeException
+from urllib.parse import urlencode
 
 
 class TLSRequest:
     '''
     Asynchronous request.
     Accepts the same parameters as ``TLSSession.request`` and some additional parameters:
 
     Args:
         method (str): Request method.
         url (str): URL to request.
         session (hrequests.session.TLSSession, optional): Associated `TLSSession`. Defaults to None.
         raise_exception (bool, optional): Raise exceptions (default FALSE for async, TRUE for sync). Defaults to False.
+        params (Dict[str, str], optional): Parameters to pass to request. Defaults to None.
         callback (function, optional): Callback called on response. Same as passing ``hooks={'response': callback}``. Defaults to None.
 
     Attributes:
         method (str): Request method.
         raise_exception (bool): Raise exceptions (default FALSE for async, TRUE for sync).
         url (str): URL to request.
         session (hrequests.session.TLSSession): Associated `TLSSession`.
@@ -53,23 +55,27 @@
     }
 
     def __init__(
         self,
         method: str,
         url: str,
         session: Optional['hrequests.session.TLSSession'] = None,
+        params: Optional[Dict[str, str]] = None,
         raise_exception: bool = True,
         **kwargs,
     ):
         # Request method
         self.method: str = method
         # Raise exceptions (default FALSE for async, TRUE for sync)
         self.raise_exception: bool = raise_exception
         # URL to request
-        self.url: str = url
+        if params is None:
+            self.url: str = url
+        else:
+            self.url: str = f'{url}?{urlencode(params, doseq=True)}'
 
         # Session kwargs
         self.sess_kwargs: dict | None = None
         if kwargs:
             sess_kwargs = set(kwargs.keys()) & TLSRequest.session_kwargs
             if session and sess_kwargs:
                 # If session is already provided, raise TypeError if session-only kwargs are passed
```

### Comparing `hrequests-0.3.0/hrequests/response.py` & `hrequests-0.4.0/hrequests/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,31 +7,52 @@
 
 import orjson
 
 import hrequests
 from hrequests.exceptions import ClientException
 
 from .cookies import RequestsCookieJar
+from .toolbelt import CaseInsensitiveDict, FileUtils
 
 
 class ProcessResponse:
     def __init__(
         self,
         session,
         method: str,
         url: str,
+        files: Optional[dict] = None,
         allow_redirects: bool = True,
         chain: bool = False,
         cookies: Optional[Union[RequestsCookieJar, dict, list]] = None,
         **kwargs,
     ) -> None:
         self.session: 'hrequests.session.TLSSession' = session
         self.method: str = method
         self.url: str = url
         self.allow_redirects: bool = allow_redirects
+
+        if files:
+            data = kwargs['data']
+            headers = kwargs['headers']
+            # assert that data is a dict
+            if data is not None:
+                assert isinstance(data, dict), "Data must be a dict when files are passed"
+            # convert files to multipart/form-data
+            kwargs['data'], content_type = FileUtils.encode_files(files, data)
+            # content_type needs to be set to Content-Type header
+            # if headers is None, append Content-Type to the existing session headers
+            if headers is None:
+                headers = self.session.headers.copy()
+            # else if headers were provided, append Content-Type to those
+            elif isinstance(headers, dict):
+                headers = CaseInsensitiveDict(headers)
+            headers['Content-Type'] = content_type
+            kwargs['headers'] = headers
+
         self.chain: bool = chain
         self.cookies: Optional[Union[RequestsCookieJar, dict, list]] = cookies
         self.kwargs: dict = kwargs
         self.response: Response
 
     def send(self) -> None:
         time: datetime = datetime.now()
@@ -44,15 +65,19 @@
         self.response.elapsed = datetime.now() - time
 
     def execute_request(self, redirect: Optional[bool] = None) -> 'Response':
         if redirect is None:
             redirect = self.allow_redirects
         try:
             resp = self.session.execute_request(
-                self.method, self.url, cookies=self.cookies, allow_redirects=redirect, **self.kwargs
+                self.method,
+                self.url,
+                cookies=self.cookies,
+                allow_redirects=redirect,
+                **self.kwargs,
             )
         except IOError as e:
             raise ClientException('Connection error') from e
         resp.session = None if self.session.temp else self.session
         return resp
 
     def generate_chain(self):
```

### Comparing `hrequests-0.3.0/hrequests/session.py` & `hrequests-0.4.0/hrequests/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 from fake_headers import Headers
 
 import hrequests
 from hrequests.reqs import *
 from hrequests.response import ProcessResponse
 
 from .cffi import freeMemory
-from .client import CaseInsensitiveDict, TLSClient
+from .client import TLSClient
 from .cookies import RequestsCookieJar
+from .toolbelt import CaseInsensitiveDict
 
 
 class TLSSession(TLSClient):
     """
     Session object that sends requests with TLS client.
 
     Args:
@@ -33,23 +34,23 @@
         force_http1 (bool, optional): Force HTTP/1. Defaults to False.
         catch_panics (bool, optional): Catch panics. Defaults to False.
         debug (bool, optional): Debug mode. Defaults to False.
 
     Methods:
         get(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a GET request
-        post(url, *, params=None, data=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
+        post(url, *, params=None, data=None, files=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a POST request
         options(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a OPTIONS request
         head(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a HEAD request
-        put(url, *, params=None, data=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
+        put(url, *, params=None, data=None, files=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a PUT request
-        patch(url, *, params=None, data=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
+        patch(url, *, params=None, data=None, files=None, headers=None, cookies=None, json=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a PATCH request
         delete(url, *, params=None, headers=None, cookies=None, allow_redirects=True, verify=None, timeout=30, proxies=None):
             Send a DELETE request
         render(url, headless, proxy, response, mock_human):
             Render a page with playwright
     """
 
@@ -124,33 +125,33 @@
         self.resetHeaders(os=os)
 
     def request(
         self,
         method: str,
         url: str,
         *,
-        params: Optional[dict] = None,
-        data: Optional[Union[str, dict]] = None,
-        headers: Optional[dict] = None,
+        data: Optional[Union[str, bytes, bytearray, dict]] = None,
+        files: Optional[dict] = None,
+        headers: Optional[Union[dict, CaseInsensitiveDict]] = None,
         cookies: Optional[Union[RequestsCookieJar, dict, list]] = None,
         json: Optional[Union[dict, list, str]] = None,
         allow_redirects: bool = True,
         history: bool = False,
         verify: bool = True,  # maps to insecure_skip_verify
         timeout: int = 30,  # maps to timeout_seconds
         proxies: Optional[dict] = None,
     ) -> 'hrequests.response.Response':
         """
         Send a request with TLS client
 
         Args:
             method (str): Method of request (GET, POST, OPTIONS, HEAD, PUT, PATCH, DELETE)
             url (str): URL to send request to
-            params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
-            data (Union[str, dict], optional): Data to send to request. Defaults to None.
+            data (Union[str, bytes, bytearray, dict], optional): Data to send to request. Defaults to None.
+            files (dict, optional): Files to send with request. Defaults to None.
             headers (dict, optional): Dictionary of HTTP headers to send with the request. Defaults to None.
             cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults to None.
             json (dict, optional): Json to send in the request body. Defaults to None.
             allow_redirects (bool, optional): Allow request to redirect. Defaults to True.
             history (bool, optional): Remember request history. Defaults to False.
             verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
             timeout (int, optional): Timeout in seconds. Defaults to 30.
@@ -161,16 +162,16 @@
         """
         if verify is None:
             verify = self.verify
         proc = ProcessResponse(
             session=self,
             method=method,
             url=url,
-            params=params,
             data=data,
+            files=files,
             headers=headers,
             cookies=cookies,
             json=json,
             allow_redirects=allow_redirects,
             chain=history,
             insecure_skip_verify=not verify,
             timeout_seconds=timeout,
@@ -193,24 +194,24 @@
     def __del__(self):
         self.close()
 
 
 class Session(TLSSession):
     def __init__(
         self,
-        browser: Literal['firefox', 'chrome', 'opera'] = 'firefox',
+        browser: Literal['firefox', 'chrome', 'opera'] = 'chrome',
         version: Optional[int] = None,
         os: Optional[Literal['win', 'mac', 'lin']] = None,
         headers: Optional[dict] = None,
         *args,
         **kwargs,
     ):
         '''
         Parameters:
-            browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'firefox'.
+            browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'chrome'.
             version (int, optional): Version of the browser to use. Browser must be specified. Default is randomized.
             os (Literal['win', 'mac', 'lin'], optional): OS to use in header. Default is randomized.
             headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
             verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
             ja3_string (str, optional): JA3 string. Defaults to None.
             h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
             additional_decode (str, optional): Additional decode. Defaults to None.
```

### Comparing `hrequests-0.3.0/LICENSE` & `hrequests-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hrequests-0.3.0/pyproject.toml` & `hrequests-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hrequests"
-version = "0.3.0"
+version = "0.4.0"
 description = "Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library."
 authors = ["daijro <daijro.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/daijro/hrequests"
 keywords = ["tls", "client", "http", "scraping", "requests", "humans", "playwright"]
 classifiers = [
```

### Comparing `hrequests-0.3.0/README.md` & `hrequests-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     </a>
     <a href="https://python.org/">
         <img src="https://img.shields.io/badge/python-3.6&#8208;3.11-blue">
     </a>
     <a href="https://pypi.org/project/hrequests/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/hrequests.svg">
     </a>
+    <a href="https://pepy.tech/project/hrequests">
+        <img alt="PyPI" src="https://pepy.tech/badge/hrequests">
+    </a>
     <a href="https://github.com/ambv/black">
         <img src="https://img.shields.io/badge/code%20style-black-black.svg">
     </a>
     <a href="https://github.com/PyCQA/isort">
         <img src="https://img.shields.io/badge/imports-isort-yellow.svg">
     </a>
 </p>
@@ -95,17 +98,18 @@
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     url (str): URL to send request to
-    params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
-    data (Union[str, dict], optional): Data to send to request. Defaults to None.
+    data (Union[str, bytes, bytearray, dict], optional): Data to send to request. Defaults to None.
+    files (Dict[str, Union[BufferedReader, tuple]], optional): Data to send to request. Defaults to None.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Defaults to None.
+    params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
     cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults to None.
     json (dict, optional): Json to send in the request body. Defaults to None.
     allow_redirects (bool, optional): Allow request to redirect. Defaults to True.
     history (bool, optional): Remember request history. Defaults to False.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     timeout (int, optional): Timeout in seconds. Defaults to 30.
     proxies (dict, optional): Dictionary of proxies. Defaults to None.
@@ -178,27 +182,27 @@
 ```
 
 
 <hr width=50>
 
 ## Sessions
 
-Creating a new Firefox Session object:
+Creating a new Chrome Session object:
 
 ```py
 >>> session = hrequests.Session()  # version randomized by default
->>> session = hrequests.Session('firefox', version=110)
+>>> session = hrequests.Session('chrome', version=112)
 ```
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
-    browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'firefox'.
+    browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'chrome'.
     version (int, optional): Version of the browser to use. Browser must be specified. Default is randomized.
     os (Literal['win', 'mac', 'lin'], optional): OS to use in header. Default is randomized.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     ja3_string (str, optional): JA3 string. Defaults to None.
     h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
     additional_decode (str, optional): Additional decode. Defaults to None.
@@ -333,24 +337,26 @@
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     url (str): URL to send request to
-    params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
-    data (Union[str, dict], optional): Data to send to request. Defaults to None.
+    data (Union[str, bytes, bytearray, dict], optional): Data to send to request. Defaults to None.
+    files (Dict[str, Union[BufferedReader, tuple]], optional): Data to send to request. Defaults to None.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Defaults to None.
+    params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
     cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults to None.
     json (dict, optional): Json to send in the request body. Defaults to None.
     allow_redirects (bool, optional): Allow request to redirect. Defaults to True.
     history (bool, optional): Remember request history. Defaults to False.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     timeout (int, optional): Timeout in seconds. Defaults to 30.
     proxies (dict, optional): Dictionary of proxies. Defaults to None.
+    no_pause (bool, optional): Run the request in the background. Defaults to False.
     <Additionally includes all parameters from `hrequests.Session` if a session was not specified>
 
 Returns:
     hrequests.response.Response: Response object
 ```
 
 </details>
@@ -455,15 +461,15 @@
 To handle timeouts or any other exception during the connection of the request, you can add an optional exception handler that will be called with the request and exception inside the main thread.
 
 ```py
 >>> def exception_handler(request, exception):
 ...    return f'Response failed: {exception}'
 
 >>> bad_reqs = [
-...     hrequests.async_get('http://httpbin.org/delay/1', timeout=0.001),
+...     hrequests.async_get('http://httpbin.org/delay/5', timeout=1),
 ...     hrequests.async_get('http://fakedomain/'),
 ...     hrequests.async_get('http://example.com/'),
 ... ]
 >>> hrequests.map(bad_reqs, size=3, exception_handler=exception_handler)
 ['Response failed: Connection error', 'Response failed: Connection error', <Response [200]>]
 ```
 
@@ -737,16 +743,17 @@
 </details>
 
 ### Navigate the browser
 
 Navigate to a url:
 
 ```py
->>> page.url = 'https://bing.com'  # navigate to a url
->>> page.goto('https://bing.com')  # or use goto
+>>> page.url = 'https://bing.com'
+# or use goto
+>>> page.goto('https://bing.com')
 ```
 
 Navigate through page history:
 
 ```py
 >>> page.back()
 >>> page.forward()
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_kzja9d2y_/tmphi28zksz_TarContainer/0/28.md", line 1011, column 3: CDATA terminal not found*

 * *File "/tmp/diffoscope_kzja9d2y_/tmphi28zksz_TarContainer/0/28.md", line 1011, column 3: CDATA terminal not found*

```diff
@@ -1,11 +1,11 @@
 [https://i.imgur.com/r8GcQW1.png]
                              ***** hrequests *****
   *** [https://img.shields.io/github/license/daijro/hrequests.svg] [https://
-       img.shields.io/badge/python-3.6&#8208;3.11-blue] [PyPI] [https://
+   img.shields.io/badge/python-3.6&#8208;3.11-blue] [PyPI] [PyPI] [https://
   img.shields.io/badge/code%20style-black-black.svg] [https://img.shields.io/
     badge/imports-isort-yellow.svg]Hrequests (human requests) is a simple,
  configurable, feature-rich, replacement for the Python requests library. ***
 ### â¨ Features - Seamless transition between HTTP and headless browsing ð»
 - Integrated fast HTML parser ð - High performance concurrency with gevent
 (*without monkey-patching!*) ð - Replication of browser TLS fingerprints
 ð - JavaScript rendering ð - Supports HTTP/2 ð - Realistic browser
@@ -27,27 +27,28 @@
 ## Simple Usage Here is an example of a simple `get` request: ```py >>> resp =
 hrequests.get('https://www.google.com/') ``` Requests are sent through
 [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof
 the TLS client fingerprint. This is done automatically, and is completely
 transparent to the user. Other request methods include `post`, `put`, `delete`,
 `head`, `options`, and `patch`. The `Response` object is a near 1:1 replica of
 the `requests.Response` object, with some additional attributes.  Parameters
-``` Parameters: url (str): URL to send request to params (dict, optional):
-Dictionary of URL parameters to append to the URL. Defaults to None. data
-(Union[str, dict], optional): Data to send to request. Defaults to None.
-headers (dict, optional): Dictionary of HTTP headers to send with the request.
-Defaults to None. cookies (Union[RequestsCookieJar, dict, list], optional):
-Dict or CookieJar to send. Defaults to None. json (dict, optional): Json to
-send in the request body. Defaults to None. allow_redirects (bool, optional):
-Allow request to redirect. Defaults to True. history (bool, optional): Remember
-request history. Defaults to False. verify (bool, optional): Verify the
-server's TLS certificate. Defaults to True. timeout (int, optional): Timeout in
-seconds. Defaults to 30. proxies (dict, optional): Dictionary of proxies.
-Defaults to None. no_pause (bool, optional): Run the request in the background.
-Defaults to False.
+``` Parameters: url (str): URL to send request to data (Union[str, bytes,
+bytearray, dict], optional): Data to send to request. Defaults to None. files
+(Dict[str, Union[BufferedReader, tuple]], optional): Data to send to request.
+Defaults to None. headers (dict, optional): Dictionary of HTTP headers to send
+with the request. Defaults to None. params (dict, optional): Dictionary of URL
+parameters to append to the URL. Defaults to None. cookies (Union
+[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults
+to None. json (dict, optional): Json to send in the request body. Defaults to
+None. allow_redirects (bool, optional): Allow request to redirect. Defaults to
+True. history (bool, optional): Remember request history. Defaults to False.
+verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
+timeout (int, optional): Timeout in seconds. Defaults to 30. proxies (dict,
+optional): Dictionary of proxies. Defaults to None. no_pause (bool, optional):
+Run the request in the background. Defaults to False.
 hrequests.Session` if a session was not specified> Returns:
 hrequests.response.Response: Response object ```  ### Properties Get the
 response url: ```py >>> resp.url: str 'https://www.google.com/' ``` Check if
 the request was successful: ```py >>> resp.status_code: int 200 >>>
 resp.reason: str 'OK' >>> resp.ok: bool True >>> bool(resp) True ``` Getting
 the response body: ```py >>> resp.text: str '
 ..' >>> resp.content: Union[bytes, str] '
@@ -58,19 +59,19 @@
 Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None,
 port_specified=False, domain='.google.com', domain_specified=True... ``` Get
 the response headers: ```py >>> resp.headers: CaseInsensitiveDict {'Alt-Svc':
 'h3=":443"; ma=2592000,h3-29=":443"; ma=2592000', 'Cache-Control': 'private,
 max-age=0', 'Content-Encoding': 'br', 'Content-Length': '51288', 'Content-
 Security-Policy-Report-Only': "object-src 'none';base-uri 'se ```
 ===============================================================================
-## Sessions Creating a new Firefox Session object: ```py >>> session =
+## Sessions Creating a new Chrome Session object: ```py >>> session =
 hrequests.Session() # version randomized by default >>> session =
-hrequests.Session('firefox', version=110) ```  Parameters ``` Parameters:
+hrequests.Session('chrome', version=112) ```  Parameters ``` Parameters:
 browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use.
-Default is 'firefox'. version (int, optional): Version of the browser to use.
+Default is 'chrome'. version (int, optional): Version of the browser to use.
 Browser must be specified. Default is randomized. os (Literal['win', 'mac',
 'lin'], optional): OS to use in header. Default is randomized. headers (dict,
 optional): Dictionary of HTTP headers to send with the request. Default is
 generated from `browser` and `os`. verify (bool, optional): Verify the server's
 TLS certificate. Defaults to True. ja3_string (str, optional): JA3 string.
 Defaults to None. h2_settings (dict, optional): HTTP/2 settings. Defaults to
 None. additional_decode (str, optional): Additional decode. Defaults to None.
@@ -135,26 +136,29 @@
 ', no_pause=True) # resp1 and resp2 are sent concurrently print('Resp 1:',
 resp1.reason) # will pause for resp1 to finish, if it hasn't already print
 ('Resp 2:', resp2.reason) # will pause for resp2 to finish, if it hasn't
 already ``` This is useful for sending multiple requests concurrently, but only
 waiting for the response when it is needed. Note that `no_pause` uses gevent as
 it's backend. Use `no_pause_threadsafe` when running across multiple threads.
 ### Grequests-style Async Requests The method `async_get` will create an unsent
-request.  Parameters ``` Parameters: url (str): URL to send request to params
-(dict, optional): Dictionary of URL parameters to append to the URL. Defaults
-to None. data (Union[str, dict], optional): Data to send to request. Defaults
-to None. headers (dict, optional): Dictionary of HTTP headers to send with the
-request. Defaults to None. cookies (Union[RequestsCookieJar, dict, list],
-optional): Dict or CookieJar to send. Defaults to None. json (dict, optional):
-Json to send in the request body. Defaults to None. allow_redirects (bool,
-optional): Allow request to redirect. Defaults to True. history (bool,
-optional): Remember request history. Defaults to False. verify (bool,
-optional): Verify the server's TLS certificate. Defaults to True. timeout (int,
-optional): Timeout in seconds. Defaults to 30. proxies (dict, optional):
-Dictionary of proxies. Defaults to None.
+request.  Parameters ``` Parameters: url (str): URL to send request to data
+(Union[str, bytes, bytearray, dict], optional): Data to send to request.
+Defaults to None. files (Dict[str, Union[BufferedReader, tuple]], optional):
+Data to send to request. Defaults to None. headers (dict, optional): Dictionary
+of HTTP headers to send with the request. Defaults to None. params (dict,
+optional): Dictionary of URL parameters to append to the URL. Defaults to None.
+cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to
+send. Defaults to None. json (dict, optional): Json to send in the request
+body. Defaults to None. allow_redirects (bool, optional): Allow request to
+redirect. Defaults to True. history (bool, optional): Remember request history.
+Defaults to False. verify (bool, optional): Verify the server's TLS
+certificate. Defaults to True. timeout (int, optional): Timeout in seconds.
+Defaults to 30. proxies (dict, optional): Dictionary of proxies. Defaults to
+None. no_pause (bool, optional): Run the request in the background. Defaults to
+False.
 hrequests.Session` if a session was not specified> Returns:
 hrequests.response.Response: Response object ```  Async requests are evaluated
 on `hrequests.map`, `hrequests.imap`, or `hrequests.imap_enum`. This
 functionality is similar to [grequests](https://github.com/spyoungtech/
 grequests). Unlike grequests, [monkey patching](https://www.gevent.org/api/
 gevent.monkey.html) is not required because this does not rely on the standard
 python SSL library. Create a set of unsent Requests: ```py reqs =
@@ -192,18 +196,18 @@
 requests to make at a time. default is 2 exception_handler - Callback function,
 called when exception occurred. Params: Request, Exception Yields: (index,
 Response) tuples. ```  #### Exception Handling To handle timeouts or any other
 exception during the connection of the request, you can add an optional
 exception handler that will be called with the request and exception inside the
 main thread. ```py >>> def exception_handler(request, exception): ... return
 f'Response failed: {exception}' >>> bad_reqs = [ ... hrequests.async_get('http:
-//httpbin.org/delay/1', timeout=0.001), ... hrequests.async_get('http://
-fakedomain/'), ... hrequests.async_get('http://example.com/'), ... ] >>>
-hrequests.map(bad_reqs, size=3, exception_handler=exception_handler) ['Response
-failed: Connection error', 'Response failed: Connection error',
+//httpbin.org/delay/5', timeout=1), ... hrequests.async_get('http://fakedomain/
+'), ... hrequests.async_get('http://example.com/'), ... ] >>> hrequests.map
+(bad_reqs, size=3, exception_handler=exception_handler) ['Response failed:
+Connection error', 'Response failed: Connection error',
 200]>] ``` The value returned by the exception handler will be used in place of
 the response in the result list:
 ===============================================================================
 ## HTML Parsing HTML scraping uses PyQuery, which is ~7x faster than bs4. This
 functionality is based of [requests-html](https://github.com/psf/requests-
 html). | Library | Time (1e5 trials) | | --- | --- | | BeautifulSoup4 | 52.6 |
 | PyQuery | 7.5 | The HTML parser can be accessed through the `html` attribute
```

### Comparing `hrequests-0.3.0/PKG-INFO` & `hrequests-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrequests
-Version: 0.3.0
+Version: 0.4.0
 Summary: Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
 Home-page: https://github.com/daijro/hrequests
 License: Apache-2.0
 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro
 Author-email: daijro.dev@gmail.com
 Requires-Python: >=3.6,<4.0
@@ -50,14 +50,17 @@
     </a>
     <a href="https://python.org/">
         <img src="https://img.shields.io/badge/python-3.6&#8208;3.11-blue">
     </a>
     <a href="https://pypi.org/project/hrequests/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/hrequests.svg">
     </a>
+    <a href="https://pepy.tech/project/hrequests">
+        <img alt="PyPI" src="https://pepy.tech/badge/hrequests">
+    </a>
     <a href="https://github.com/ambv/black">
         <img src="https://img.shields.io/badge/code%20style-black-black.svg">
     </a>
     <a href="https://github.com/PyCQA/isort">
         <img src="https://img.shields.io/badge/imports-isort-yellow.svg">
     </a>
 </p>
@@ -134,17 +137,18 @@
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     url (str): URL to send request to
-    params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
-    data (Union[str, dict], optional): Data to send to request. Defaults to None.
+    data (Union[str, bytes, bytearray, dict], optional): Data to send to request. Defaults to None.
+    files (Dict[str, Union[BufferedReader, tuple]], optional): Data to send to request. Defaults to None.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Defaults to None.
+    params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
     cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults to None.
     json (dict, optional): Json to send in the request body. Defaults to None.
     allow_redirects (bool, optional): Allow request to redirect. Defaults to True.
     history (bool, optional): Remember request history. Defaults to False.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     timeout (int, optional): Timeout in seconds. Defaults to 30.
     proxies (dict, optional): Dictionary of proxies. Defaults to None.
@@ -217,27 +221,27 @@
 ```
 
 
 <hr width=50>
 
 ## Sessions
 
-Creating a new Firefox Session object:
+Creating a new Chrome Session object:
 
 ```py
 >>> session = hrequests.Session()  # version randomized by default
->>> session = hrequests.Session('firefox', version=110)
+>>> session = hrequests.Session('chrome', version=112)
 ```
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
-    browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'firefox'.
+    browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use. Default is 'chrome'.
     version (int, optional): Version of the browser to use. Browser must be specified. Default is randomized.
     os (Literal['win', 'mac', 'lin'], optional): OS to use in header. Default is randomized.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Default is generated from `browser` and `os`.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     ja3_string (str, optional): JA3 string. Defaults to None.
     h2_settings (dict, optional): HTTP/2 settings. Defaults to None.
     additional_decode (str, optional): Additional decode. Defaults to None.
@@ -372,24 +376,26 @@
 
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     url (str): URL to send request to
-    params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
-    data (Union[str, dict], optional): Data to send to request. Defaults to None.
+    data (Union[str, bytes, bytearray, dict], optional): Data to send to request. Defaults to None.
+    files (Dict[str, Union[BufferedReader, tuple]], optional): Data to send to request. Defaults to None.
     headers (dict, optional): Dictionary of HTTP headers to send with the request. Defaults to None.
+    params (dict, optional): Dictionary of URL parameters to append to the URL. Defaults to None.
     cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults to None.
     json (dict, optional): Json to send in the request body. Defaults to None.
     allow_redirects (bool, optional): Allow request to redirect. Defaults to True.
     history (bool, optional): Remember request history. Defaults to False.
     verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
     timeout (int, optional): Timeout in seconds. Defaults to 30.
     proxies (dict, optional): Dictionary of proxies. Defaults to None.
+    no_pause (bool, optional): Run the request in the background. Defaults to False.
     <Additionally includes all parameters from `hrequests.Session` if a session was not specified>
 
 Returns:
     hrequests.response.Response: Response object
 ```
 
 </details>
@@ -494,15 +500,15 @@
 To handle timeouts or any other exception during the connection of the request, you can add an optional exception handler that will be called with the request and exception inside the main thread.
 
 ```py
 >>> def exception_handler(request, exception):
 ...    return f'Response failed: {exception}'
 
 >>> bad_reqs = [
-...     hrequests.async_get('http://httpbin.org/delay/1', timeout=0.001),
+...     hrequests.async_get('http://httpbin.org/delay/5', timeout=1),
 ...     hrequests.async_get('http://fakedomain/'),
 ...     hrequests.async_get('http://example.com/'),
 ... ]
 >>> hrequests.map(bad_reqs, size=3, exception_handler=exception_handler)
 ['Response failed: Connection error', 'Response failed: Connection error', <Response [200]>]
 ```
 
@@ -776,16 +782,17 @@
 </details>
 
 ### Navigate the browser
 
 Navigate to a url:
 
 ```py
->>> page.url = 'https://bing.com'  # navigate to a url
->>> page.goto('https://bing.com')  # or use goto
+>>> page.url = 'https://bing.com'
+# or use goto
+>>> page.goto('https://bing.com')
 ```
 
 Navigate through page history:
 
 ```py
 >>> page.back()
 >>> page.forward()
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_kzja9d2y_/tmphi28zksz_TarContainer/0/29", line 1051, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_kzja9d2y_/tmphi28zksz_TarContainer/0/29", line 1051, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hrequests Version: 0.3.0 Summary: Hrequests (human
+Metadata-Version: 2.1 Name: hrequests Version: 0.4.0 Summary: Hrequests (human
 requests) is a simple, configurable, feature-rich, replacement for the Python
 requests library. Home-page: https://github.com/daijro/hrequests License:
 Apache-2.0 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro Author-email: daijro.dev@gmail.com Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -16,15 +16,15 @@
 runtime ; sys_platform == "win32" Requires-Dist: numpy Requires-Dist: orjson
 Requires-Dist: parse Requires-Dist: playwright Requires-Dist: playwright-
 stealth Requires-Dist: pyquery Requires-Dist: w3lib Requires-Dist: wget
 Project-URL: Repository, https://github.com/daijro/hrequests Description-
 Content-Type: text/markdown [https://i.imgur.com/r8GcQW1.png]
                              ***** hrequests *****
   *** [https://img.shields.io/github/license/daijro/hrequests.svg] [https://
-       img.shields.io/badge/python-3.6&#8208;3.11-blue] [PyPI] [https://
+   img.shields.io/badge/python-3.6&#8208;3.11-blue] [PyPI] [PyPI] [https://
   img.shields.io/badge/code%20style-black-black.svg] [https://img.shields.io/
     badge/imports-isort-yellow.svg]Hrequests (human requests) is a simple,
  configurable, feature-rich, replacement for the Python requests library. ***
 ### â¨ Features - Seamless transition between HTTP and headless browsing ð»
 - Integrated fast HTML parser ð - High performance concurrency with gevent
 (*without monkey-patching!*) ð - Replication of browser TLS fingerprints
 ð - JavaScript rendering ð - Supports HTTP/2 ð - Realistic browser
@@ -46,27 +46,28 @@
 ## Simple Usage Here is an example of a simple `get` request: ```py >>> resp =
 hrequests.get('https://www.google.com/') ``` Requests are sent through
 [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof
 the TLS client fingerprint. This is done automatically, and is completely
 transparent to the user. Other request methods include `post`, `put`, `delete`,
 `head`, `options`, and `patch`. The `Response` object is a near 1:1 replica of
 the `requests.Response` object, with some additional attributes.  Parameters
-``` Parameters: url (str): URL to send request to params (dict, optional):
-Dictionary of URL parameters to append to the URL. Defaults to None. data
-(Union[str, dict], optional): Data to send to request. Defaults to None.
-headers (dict, optional): Dictionary of HTTP headers to send with the request.
-Defaults to None. cookies (Union[RequestsCookieJar, dict, list], optional):
-Dict or CookieJar to send. Defaults to None. json (dict, optional): Json to
-send in the request body. Defaults to None. allow_redirects (bool, optional):
-Allow request to redirect. Defaults to True. history (bool, optional): Remember
-request history. Defaults to False. verify (bool, optional): Verify the
-server's TLS certificate. Defaults to True. timeout (int, optional): Timeout in
-seconds. Defaults to 30. proxies (dict, optional): Dictionary of proxies.
-Defaults to None. no_pause (bool, optional): Run the request in the background.
-Defaults to False.
+``` Parameters: url (str): URL to send request to data (Union[str, bytes,
+bytearray, dict], optional): Data to send to request. Defaults to None. files
+(Dict[str, Union[BufferedReader, tuple]], optional): Data to send to request.
+Defaults to None. headers (dict, optional): Dictionary of HTTP headers to send
+with the request. Defaults to None. params (dict, optional): Dictionary of URL
+parameters to append to the URL. Defaults to None. cookies (Union
+[RequestsCookieJar, dict, list], optional): Dict or CookieJar to send. Defaults
+to None. json (dict, optional): Json to send in the request body. Defaults to
+None. allow_redirects (bool, optional): Allow request to redirect. Defaults to
+True. history (bool, optional): Remember request history. Defaults to False.
+verify (bool, optional): Verify the server's TLS certificate. Defaults to True.
+timeout (int, optional): Timeout in seconds. Defaults to 30. proxies (dict,
+optional): Dictionary of proxies. Defaults to None. no_pause (bool, optional):
+Run the request in the background. Defaults to False.
 hrequests.Session` if a session was not specified> Returns:
 hrequests.response.Response: Response object ```  ### Properties Get the
 response url: ```py >>> resp.url: str 'https://www.google.com/' ``` Check if
 the request was successful: ```py >>> resp.status_code: int 200 >>>
 resp.reason: str 'OK' >>> resp.ok: bool True >>> bool(resp) True ``` Getting
 the response body: ```py >>> resp.text: str '
 ..' >>> resp.content: Union[bytes, str] '
@@ -77,19 +78,19 @@
 Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None,
 port_specified=False, domain='.google.com', domain_specified=True... ``` Get
 the response headers: ```py >>> resp.headers: CaseInsensitiveDict {'Alt-Svc':
 'h3=":443"; ma=2592000,h3-29=":443"; ma=2592000', 'Cache-Control': 'private,
 max-age=0', 'Content-Encoding': 'br', 'Content-Length': '51288', 'Content-
 Security-Policy-Report-Only': "object-src 'none';base-uri 'se ```
 ===============================================================================
-## Sessions Creating a new Firefox Session object: ```py >>> session =
+## Sessions Creating a new Chrome Session object: ```py >>> session =
 hrequests.Session() # version randomized by default >>> session =
-hrequests.Session('firefox', version=110) ```  Parameters ``` Parameters:
+hrequests.Session('chrome', version=112) ```  Parameters ``` Parameters:
 browser (Literal['firefox', 'chrome', 'opera'], optional): Browser to use.
-Default is 'firefox'. version (int, optional): Version of the browser to use.
+Default is 'chrome'. version (int, optional): Version of the browser to use.
 Browser must be specified. Default is randomized. os (Literal['win', 'mac',
 'lin'], optional): OS to use in header. Default is randomized. headers (dict,
 optional): Dictionary of HTTP headers to send with the request. Default is
 generated from `browser` and `os`. verify (bool, optional): Verify the server's
 TLS certificate. Defaults to True. ja3_string (str, optional): JA3 string.
 Defaults to None. h2_settings (dict, optional): HTTP/2 settings. Defaults to
 None. additional_decode (str, optional): Additional decode. Defaults to None.
@@ -154,26 +155,29 @@
 ', no_pause=True) # resp1 and resp2 are sent concurrently print('Resp 1:',
 resp1.reason) # will pause for resp1 to finish, if it hasn't already print
 ('Resp 2:', resp2.reason) # will pause for resp2 to finish, if it hasn't
 already ``` This is useful for sending multiple requests concurrently, but only
 waiting for the response when it is needed. Note that `no_pause` uses gevent as
 it's backend. Use `no_pause_threadsafe` when running across multiple threads.
 ### Grequests-style Async Requests The method `async_get` will create an unsent
-request.  Parameters ``` Parameters: url (str): URL to send request to params
-(dict, optional): Dictionary of URL parameters to append to the URL. Defaults
-to None. data (Union[str, dict], optional): Data to send to request. Defaults
-to None. headers (dict, optional): Dictionary of HTTP headers to send with the
-request. Defaults to None. cookies (Union[RequestsCookieJar, dict, list],
-optional): Dict or CookieJar to send. Defaults to None. json (dict, optional):
-Json to send in the request body. Defaults to None. allow_redirects (bool,
-optional): Allow request to redirect. Defaults to True. history (bool,
-optional): Remember request history. Defaults to False. verify (bool,
-optional): Verify the server's TLS certificate. Defaults to True. timeout (int,
-optional): Timeout in seconds. Defaults to 30. proxies (dict, optional):
-Dictionary of proxies. Defaults to None.
+request.  Parameters ``` Parameters: url (str): URL to send request to data
+(Union[str, bytes, bytearray, dict], optional): Data to send to request.
+Defaults to None. files (Dict[str, Union[BufferedReader, tuple]], optional):
+Data to send to request. Defaults to None. headers (dict, optional): Dictionary
+of HTTP headers to send with the request. Defaults to None. params (dict,
+optional): Dictionary of URL parameters to append to the URL. Defaults to None.
+cookies (Union[RequestsCookieJar, dict, list], optional): Dict or CookieJar to
+send. Defaults to None. json (dict, optional): Json to send in the request
+body. Defaults to None. allow_redirects (bool, optional): Allow request to
+redirect. Defaults to True. history (bool, optional): Remember request history.
+Defaults to False. verify (bool, optional): Verify the server's TLS
+certificate. Defaults to True. timeout (int, optional): Timeout in seconds.
+Defaults to 30. proxies (dict, optional): Dictionary of proxies. Defaults to
+None. no_pause (bool, optional): Run the request in the background. Defaults to
+False.
 hrequests.Session` if a session was not specified> Returns:
 hrequests.response.Response: Response object ```  Async requests are evaluated
 on `hrequests.map`, `hrequests.imap`, or `hrequests.imap_enum`. This
 functionality is similar to [grequests](https://github.com/spyoungtech/
 grequests). Unlike grequests, [monkey patching](https://www.gevent.org/api/
 gevent.monkey.html) is not required because this does not rely on the standard
 python SSL library. Create a set of unsent Requests: ```py reqs =
@@ -211,18 +215,18 @@
 requests to make at a time. default is 2 exception_handler - Callback function,
 called when exception occurred. Params: Request, Exception Yields: (index,
 Response) tuples. ```  #### Exception Handling To handle timeouts or any other
 exception during the connection of the request, you can add an optional
 exception handler that will be called with the request and exception inside the
 main thread. ```py >>> def exception_handler(request, exception): ... return
 f'Response failed: {exception}' >>> bad_reqs = [ ... hrequests.async_get('http:
-//httpbin.org/delay/1', timeout=0.001), ... hrequests.async_get('http://
-fakedomain/'), ... hrequests.async_get('http://example.com/'), ... ] >>>
-hrequests.map(bad_reqs, size=3, exception_handler=exception_handler) ['Response
-failed: Connection error', 'Response failed: Connection error',
+//httpbin.org/delay/5', timeout=1), ... hrequests.async_get('http://fakedomain/
+'), ... hrequests.async_get('http://example.com/'), ... ] >>> hrequests.map
+(bad_reqs, size=3, exception_handler=exception_handler) ['Response failed:
+Connection error', 'Response failed: Connection error',
 200]>] ``` The value returned by the exception handler will be used in place of
 the response in the result list:
 ===============================================================================
 ## HTML Parsing HTML scraping uses PyQuery, which is ~7x faster than bs4. This
 functionality is based of [requests-html](https://github.com/psf/requests-
 html). | Library | Time (1e5 trials) | | --- | --- | | BeautifulSoup4 | 52.6 |
 | PyQuery | 7.5 | The HTML parser can be accessed through the `html` attribute
```

