# Comparing `tmp/async_firebase-3.1.1.tar.gz` & `tmp/async_firebase-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_firebase-3.1.1.tar", max compression
+gzip compressed data, was "async_firebase-3.2.0.tar", max compression
```

## Comparing `async_firebase-3.1.1.tar` & `async_firebase-3.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-05-10 12:55:54.782004 async_firebase-3.1.1/LICENSE
--rw-r--r--   0        0        0     8292 2023-05-10 12:55:54.782004 async_firebase-3.1.1/README.md
--rw-r--r--   0        0        0      194 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/__init__.py
--rw-r--r--   0        0        0     7906 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/base.py
--rw-r--r--   0        0        0    23182 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/client.py
--rw-r--r--   0        0        0     1547 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/encoders.py
--rw-r--r--   0        0        0     8142 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/errors.py
--rw-r--r--   0        0        0    16839 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/messages.py
--rw-r--r--   0        0        0    12977 2023-05-10 12:55:54.782004 async_firebase-3.1.1/async_firebase/utils.py
--rw-r--r--   0        0        0     1673 2023-05-10 12:55:54.782004 async_firebase-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     9394 1970-01-01 00:00:00.000000 async_firebase-3.1.1/setup.py
--rw-r--r--   0        0        0     9758 1970-01-01 00:00:00.000000 async_firebase-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-11 11:42:03.003322 async_firebase-3.2.0/LICENSE
+-rw-r--r--   0        0        0     8292 2023-07-11 11:42:03.003322 async_firebase-3.2.0/README.md
+-rw-r--r--   0        0        0      194 2023-07-11 11:42:03.003322 async_firebase-3.2.0/async_firebase/__init__.py
+-rw-r--r--   0        0        0     1162 2023-07-11 11:42:03.003322 async_firebase-3.2.0/async_firebase/_config.py
+-rw-r--r--   0        0        0     8621 2023-07-11 11:42:03.003322 async_firebase-3.2.0/async_firebase/base.py
+-rw-r--r--   0        0        0    23244 2023-07-11 11:42:03.003322 async_firebase-3.2.0/async_firebase/client.py
+-rw-r--r--   0        0        0     1547 2023-07-11 11:42:03.003322 async_firebase-3.2.0/async_firebase/encoders.py
+-rw-r--r--   0        0        0     8142 2023-07-11 11:42:03.003322 async_firebase-3.2.0/async_firebase/errors.py
+-rw-r--r--   0        0        0    16839 2023-07-11 11:42:03.003322 async_firebase-3.2.0/async_firebase/messages.py
+-rw-r--r--   0        0        0    12977 2023-07-11 11:42:03.003322 async_firebase-3.2.0/async_firebase/utils.py
+-rw-r--r--   0        0        0     1673 2023-07-11 11:42:03.003322 async_firebase-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9394 1970-01-01 00:00:00.000000 async_firebase-3.2.0/setup.py
+-rw-r--r--   0        0        0     9758 1970-01-01 00:00:00.000000 async_firebase-3.2.0/PKG-INFO
```

### Comparing `async_firebase-3.1.1/LICENSE` & `async_firebase-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.1/README.md` & `async_firebase-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.1/async_firebase/base.py` & `async_firebase-3.2.0/async_firebase/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 from pathlib import PurePath
 from urllib.parse import urlencode, urljoin
 
 import httpx
 from google.oauth2 import service_account  # type: ignore
 
 import pkg_resources  # type: ignore
+from async_firebase._config import (
+    DEFAULT_REQUEST_LIMITS,
+    DEFAULT_REQUEST_TIMEOUT,
+    RequestLimits,
+    RequestTimeout,
+)
 from async_firebase.messages import FCMBatchResponse, FCMResponse
 from async_firebase.utils import (
     FCMBatchResponseHandler,
     FCMResponseHandler,
     serialize_mime_message,
 )
 
@@ -36,32 +42,40 @@
         "https://www.googleapis.com/auth/cloud-platform",
     ]
 
     def __init__(
         self,
         credentials: t.Optional[service_account.Credentials] = None,
         scopes: t.Optional[t.List[str]] = None,
+        *,
+        request_timeout: RequestTimeout = DEFAULT_REQUEST_TIMEOUT,
+        request_limits: RequestLimits = DEFAULT_REQUEST_LIMITS,
     ) -> None:
         """
         :param credentials: instance of ``google.oauth2.service_account.Credentials``.
             Usually, you'll create these credentials with one of the helper constructors. To create credentials using a
             Google service account private key JSON file::
 
                 self.creds_from_service_account_file('service-account.json')
 
             Or if you already have the service account file loaded::
 
                 service_account_info = json.load(open('service_account.json'))
                 self.creds_from_service_account_info(service_account_info)
 
         :param scopes: user-defined scopes to request during the authorization grant.
+        :param request_timeout: advanced feature that allows to change request timeout.
+        :param request_limits: advanced feature that allows to control the connection pool size.
         """
         self._credentials: service_account.Credentials = credentials
         self.scopes: t.List[str] = scopes or self.SCOPES
 
+        self._request_timeout = request_timeout
+        self._request_limits = request_limits
+
     def creds_from_service_account_info(self, service_account_info: t.Dict[str, str]) -> None:
         """
         Creates a Credentials instance from parsed service account info.
 
         :param service_account_info: the service account info in Google format.
         """
         self._credentials = service_account.Credentials.from_service_account_info(
@@ -162,15 +176,19 @@
         :param uri: URI to be requested.
         :param response_handler: the model to handle response.
         :param json_payload: request JSON payload
         :param headers: request headers.
         :param content: request content
         :return: HTTP response
         """
-        async with httpx.AsyncClient(base_url=self.BASE_URL) as client:
+        async with httpx.AsyncClient(
+            base_url=self.BASE_URL,
+            timeout=httpx.Timeout(**self._request_timeout.__dict__),
+            limits=httpx.Limits(**self._request_limits.__dict__),
+        ) as client:
             logging.debug(
                 "Requesting POST %s, payload: %s, content: %s, headers: %s",
                 urljoin(self.BASE_URL, self.FCM_ENDPOINT.format(project_id=self._credentials.project_id)),
                 json_payload,
                 content,
                 headers,
             )
```

### Comparing `async_firebase-3.1.1/async_firebase/client.py` & `async_firebase-3.2.0/async_firebase/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 from datetime import datetime, timedelta
 from email.mime.multipart import MIMEMultipart
 from email.mime.nonmultipart import MIMENonMultipart
 from urllib.parse import urljoin
 
 import httpx
 
-from async_firebase.base import AsyncClientBase
+from async_firebase.base import (  # noqa: F401
+    AsyncClientBase,
+    RequestLimits,
+    RequestTimeout,
+)
 from async_firebase.encoders import aps_encoder
 from async_firebase.messages import (
     AndroidConfig,
     AndroidNotification,
     APNSConfig,
     APNSPayload,
     Aps,
```

### Comparing `async_firebase-3.1.1/async_firebase/encoders.py` & `async_firebase-3.2.0/async_firebase/encoders.py`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.1/async_firebase/errors.py` & `async_firebase-3.2.0/async_firebase/errors.py`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.1/async_firebase/messages.py` & `async_firebase-3.2.0/async_firebase/messages.py`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.1/async_firebase/utils.py` & `async_firebase-3.2.0/async_firebase/utils.py`

 * *Files identical despite different names*

### Comparing `async_firebase-3.1.1/pyproject.toml` & `async_firebase-3.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-firebase"
-version = "3.1.1"
+version = "3.2.0"
 description = "Async Firebase Client - a Python asyncio client to interact with Firebase Cloud Messaging in an easy way."
 license = "MIT"
 authors = [
     "Oleksandr Omyshev <oomyshev@healthjoy.com>"
 ]
 maintainers = [
     "Healthjoy Developers <developers@healthjoy.com>",
```

### Comparing `async_firebase-3.1.1/setup.py` & `async_firebase-3.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['google-auth>=2.6.0,<2.7.0', 'httpx>=0.23.0,<1.0.0']
 
 setup_kwargs = {
     'name': 'async-firebase',
-    'version': '3.1.1',
+    'version': '3.2.0',
     'description': 'Async Firebase Client - a Python asyncio client to interact with Firebase Cloud Messaging in an easy way.',
     'long_description': '# async-firebase is a lightweight asynchronous client to interact with Firebase Cloud Messaging for sending push notification to Android and iOS devices\n\n[![PyPI download month](https://img.shields.io/pypi/dm/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI version fury.io](https://badge.fury.io/py/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI license](https://img.shields.io/pypi/l/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/async-firebase.svg)](https://pypi.python.org/pypi/async-firebase/)\n[![CI](https://github.com/healthjoy/async-firebase/actions/workflows/ci.yml/badge.svg)](https://github.com/healthjoy/async-firebase/actions/workflows/ci.yml)\n[![Codacy coverage](https://img.shields.io/codacy/coverage/b6a59cdf5ca64eab9104928d4f9bbb97?logo=codacy)](https://app.codacy.com/gh/healthjoy/async-firebase/dashboard)\n\n\n  * Free software: MIT license\n  * Requires: Python 3.7+\n\n## Features\n\n  * Extremely lightweight and does not rely on ``firebase-admin`` which is hefty\n  * Send push notifications to Android and iOS devices\n  * Send Multicast push notification to Android and iOS devices\n  * Send Web push notifications\n  * Set TTL (time to live) for notifications\n  * Set priority for notifications\n  * Set collapse-key for notifications\n  * Dry-run mode for testing purpose\n\n## Installation\n```shell script\n$ pip install async-firebase\n```\n\n## Getting started\n### async-firebase < 3.0.0\nTo send push notification to Android:\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token = "..."\n\n    android_config = client.build_android_config(\n        priority="high",\n        ttl=2419200,\n        collapse_key="push",\n        data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"},\n        title="Store Changes",\n        body="Recent store changes",\n    )\n    response = await client.push(device_token=device_token, android=android_config)\n\n    print(response.success, response.message_id)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo send push notification to iOS:\n\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token = "..."\n\n    apns_config = client.build_apns_config(\n        priority="normal",\n        ttl=2419200,\n        apns_topic="store-updated",\n        collapse_key="push",\n        title="Store Changes",\n        alert="Recent store changes",\n        badge=1,\n        category="test-category",\n        custom_data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"}\n    )\n    response = await client.push(device_token=device_token, apns=apns_config)\n\n    print(response.success)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nThis prints:\n\n```shell script\n"projects/mobile-app/messages/0:2367799010922733%7606eb557606ebff"\n```\n\nTo manual construct message:\n```python3\nimport asyncio\nfrom datetime import datetime\n\nfrom async_firebase.messages import APNSConfig, APNSPayload, ApsAlert, Aps\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    apns_config = APNSConfig(**{\n        "headers": {\n            "apns-expiration": str(int(datetime.utcnow().timestamp()) + 7200),\n            "apns-priority": "10",\n            "apns-topic": "test-topic",\n            "apns-collapse-id": "something",\n        },\n        "payload": APNSPayload(**{\n            "aps": Aps(**{\n                "alert": ApsAlert(title="some-title", body="alert-message"),\n                "badge": 0,\n                "sound": "default",\n                "content_available": True,\n                "category": "some-category",\n                "mutable_content": False,\n                "custom_data": {\n                    "link": "https://link-to-somewhere.com",\n                    "ticket_id": "YXZ-655512",\n                },\n            })\n        })\n    })\n\n    device_token = "..."\n\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_info({...})\n    response = await client.push(device_token=device_token, apns=apns_config)\n    print(response.success)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n### async-firebase >= 3.0.0\nTo send push notification to Android:\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\nfrom async_firebase.messages import Message\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token: str = "..."\n\n    android_config = client.build_android_config(\n        priority="high",\n        ttl=2419200,\n        collapse_key="push",\n        data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"},\n        title="Store Changes",\n        body="Recent store changes",\n    )\n    message = Message(android=android_config, token=device_token)\n    response = await client.send(message)\n\n    print(response.success, response.message_id)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo send push notification to iOS:\n\n```python3\nimport asyncio\n\nfrom async_firebase import AsyncFirebaseClient\nfrom async_firebase.messages import Message\n\n\nasync def main():\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_file("secret-store/mobile-app-79225efac4bb.json")\n\n    # or using dictionary object\n    # client.creds_from_service_account_info({...}})\n\n    device_token: str = "..."\n\n    apns_config = client.build_apns_config(\n        priority="normal",\n        ttl=2419200,\n        apns_topic="store-updated",\n        collapse_key="push",\n        title="Store Changes",\n        alert="Recent store changes",\n        badge=1,\n        category="test-category",\n        custom_data={"discount": "15%", "key_1": "value_1", "timestamp": "2021-02-24T12:00:15"}\n    )\n    message = Message(apns=apns_config, token=device_token)\n    response = await client.send(message)\n\n    print(response.success)\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nThis prints:\n\n```shell script\n"projects/mobile-app/messages/0:2367799010922733%7606eb557606ebff"\n```\n\nTo manual construct message:\n```python3\nimport asyncio\nfrom datetime import datetime\n\nfrom async_firebase.messages import APNSConfig, APNSPayload, ApsAlert, Aps, Message\nfrom async_firebase import AsyncFirebaseClient\n\n\nasync def main():\n    apns_config = APNSConfig(**{\n        "headers": {\n            "apns-expiration": str(int(datetime.utcnow().timestamp()) + 7200),\n            "apns-priority": "10",\n            "apns-topic": "test-topic",\n            "apns-collapse-id": "something",\n        },\n        "payload": APNSPayload(**{\n            "aps": Aps(**{\n                "alert": ApsAlert(title="some-title", body="alert-message"),\n                "badge": 0,\n                "sound": "default",\n                "content_available": True,\n                "category": "some-category",\n                "mutable_content": False,\n                "custom_data": {\n                    "link": "https://link-to-somewhere.com",\n                    "ticket_id": "YXZ-655512",\n                },\n            })\n        })\n    })\n\n    device_token: str = "..."\n\n    client = AsyncFirebaseClient()\n    client.creds_from_service_account_info({...})\n    message = Message(apns=apns_config, token=device_token)\n    response = await client.send(message)\n    print(response.success)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n## License\n\n``async-firebase`` is offered under the MIT license.\n\n## Source code\n\nThe latest developer version is available in a GitHub repository:\n[https://github.com/healthjoy/async-firebase](https://github.com/healthjoy/async-firebase)\n',
     'author': 'Oleksandr Omyshev',
     'author_email': 'oomyshev@healthjoy.com',
     'maintainer': 'Healthjoy Developers',
     'maintainer_email': 'developers@healthjoy.com',
     'url': 'https://github.com/healthjoy/async-firebase',
```

### Comparing `async_firebase-3.1.1/PKG-INFO` & `async_firebase-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-firebase
-Version: 3.1.1
+Version: 3.2.0
 Summary: Async Firebase Client - a Python asyncio client to interact with Firebase Cloud Messaging in an easy way.
 Home-page: https://github.com/healthjoy/async-firebase
 License: MIT
 Keywords: async,asyncio,firebase,fcm,python3,push-notifications
 Author: Oleksandr Omyshev
 Author-email: oomyshev@healthjoy.com
 Maintainer: Healthjoy Developers
```

