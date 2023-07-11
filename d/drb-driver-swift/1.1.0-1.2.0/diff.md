# Comparing `tmp/drb-driver-swift-1.1.0.tar.gz` & `tmp/drb-driver-swift-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-swift-1.1.0.tar", last modified: Wed Dec 28 10:12:07 2022, max compression
+gzip compressed data, was "drb-driver-swift-1.2.0.tar", last modified: Tue Jul 11 13:29:49 2023, max compression
```

## Comparing `drb-driver-swift-1.1.0.tar` & `drb-driver-swift-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 10:12:07.484794 drb-driver-swift-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       62 2022-12-20 15:59:31.000000 drb-driver-swift-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2579 2022-12-28 10:12:07.484794 drb-driver-swift-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2049 2022-12-20 15:59:31.000000 drb-driver-swift-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 10:12:07.472794 drb-driver-swift-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 10:12:07.472794 drb-driver-swift-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 10:12:07.488795 drb-driver-swift-1.1.0/drb/drivers/swift/
--rw-rw-rw-   0 root         (0) root         (0)      298 2022-12-20 15:59:31.000000 drb-driver-swift-1.1.0/drb/drivers/swift/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-28 10:12:07.488795 drb-driver-swift-1.1.0/drb/drivers/swift/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    16167 2022-12-20 16:25:14.000000 drb-driver-swift-1.1.0/drb/drivers/swift/swift.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 10:12:07.472794 drb-driver-swift-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 10:12:07.484794 drb-driver-swift-1.1.0/drb/topics/swift/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 15:59:31.000000 drb-driver-swift-1.1.0/drb/topics/swift/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2022-12-20 15:59:31.000000 drb-driver-swift-1.1.0/drb/topics/swift/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 10:12:07.484794 drb-driver-swift-1.1.0/drb_driver_swift.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2579 2022-12-28 10:12:06.000000 drb-driver-swift-1.1.0/drb_driver_swift.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      457 2022-12-28 10:12:06.000000 drb-driver-swift-1.1.0/drb_driver_swift.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-28 10:12:06.000000 drb-driver-swift-1.1.0/drb_driver_swift.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2022-12-28 10:12:06.000000 drb-driver-swift-1.1.0/drb_driver_swift.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2022-12-28 10:12:06.000000 drb-driver-swift-1.1.0/drb_driver_swift.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-28 10:12:06.000000 drb-driver-swift-1.1.0/drb_driver_swift.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-12-20 15:59:31.000000 drb-driver-swift-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      212 2022-12-28 10:12:07.488795 drb-driver-swift-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1366 2022-12-20 15:59:31.000000 drb-driver-swift-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-20 15:59:31.000000 drb-driver-swift-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 13:29:49.700025 drb-driver-swift-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-07-11 13:29:49.700025 drb-driver-swift-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1995 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 13:29:49.692025 drb-driver-swift-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 13:29:49.692025 drb-driver-swift-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 13:29:49.696025 drb-driver-swift-1.2.0/drb/drivers/swift/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/drb/drivers/swift/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-07-11 13:29:49.700025 drb-driver-swift-1.2.0/drb/drivers/swift/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    14507 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/drb/drivers/swift/swift.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 13:29:49.692025 drb-driver-swift-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 13:29:49.696025 drb-driver-swift-1.2.0/drb/topics/swift/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 13:29:29.000000 drb-driver-swift-1.2.0/drb/topics/swift/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-11 13:29:29.000000 drb-driver-swift-1.2.0/drb/topics/swift/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 13:29:49.700025 drb-driver-swift-1.2.0/drb_driver_swift.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-07-11 13:29:49.000000 drb-driver-swift-1.2.0/drb_driver_swift.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      636 2023-07-11 13:29:49.000000 drb-driver-swift-1.2.0/drb_driver_swift.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 13:29:49.000000 drb-driver-swift-1.2.0/drb_driver_swift.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-11 13:29:49.000000 drb-driver-swift-1.2.0/drb_driver_swift.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 13:29:49.000000 drb-driver-swift-1.2.0/drb_driver_swift.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-11 13:29:49.000000 drb-driver-swift-1.2.0/drb_driver_swift.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-11 13:29:49.000000 drb-driver-swift-1.2.0/drb_driver_swift.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-11 13:21:18.000000 drb-driver-swift-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2023-07-11 13:29:49.700025 drb-driver-swift-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-11 13:00:47.000000 drb-driver-swift-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 13:29:49.700025 drb-driver-swift-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3066 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/tests/test_container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4040 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/tests/test_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     2700 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/tests/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-06-06 15:30:31.000000 drb-driver-swift-1.2.0/versioneer.py
```

### Comparing `drb-driver-swift-1.1.0/PKG-INFO` & `drb-driver-swift-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: drb-driver-swift
-Version: 1.1.0
-Summary: DRB Swift driver
+Version: 1.2.0
+Summary: DRB OpenStack Swift driver
 Home-page: https://gitlab.com/drb-python/impl/swift
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/swift/
+License: LGPLv3
+Project-URL: Documentation, https://drb-python.gitlab.io/drb-python/impl/swift
 Project-URL: Source, https://gitlab.com/drb-python/impl/swift
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # Swift Implementation
 This drb-driver-swift module implements Swift protocol access with DRB data model.
 
 ## Swift Factory and Swift Node
 The module implements the factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -66,8 +67,7 @@
 This implementation doesn't allow to write, modify, delete file on a swift container,
 or it doesn't allow to delete or upload a file.
 This implementation doesn't allow to download directly an all container.
 
 ## Documentation
 
 The documentation of this implementation can be found here https://drb-python.gitlab.io/impl/swift
-
```

### Comparing `drb-driver-swift-1.1.0/README.md` & `drb-driver-swift-1.2.0/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-# Swift Implementation
-This drb-driver-swift module implements Swift protocol access with DRB data model.
-
-## Swift Factory and Swift Node
-The module implements the factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
-
-The entry point group reference is `drb.driver.swift`.<br/>
-The implementation name is `swift`.<br/>
-The factory class is encoded into `drb.driver.swift`.<br/>
-The Swift signature id is  `86289118-7797-11ec-90d6-0242ac120003`<br/>
-
-
-## Using this module
-The project is present in https://www.pypi.org service. it can be freely 
-loaded into projects with the following command line:
-
-```commandline
-pip install drb-driver-swift
-```
-## Access Data
-`DrbSwiftNode` manages the swift protocol to access remote data. The construction
-parameter is an authentication object.
-
-```python
-from drb.drivers.swift import SwiftService, SwiftAuth
-
-_os_options = {
-    'user_domain_name': 'Default',
-    'project_domain_name': 'Default',
-    'project_name': 'project_name',
-    'project_id': 'project_id',
-    'tenant_name': 'tenant_name',
-    'tenant_id': 'tenant_id',
-    'region_name': 'region_name'
-}
-
-auth = SwiftAuth(authurl="https://your_auth_url/v3",
-                 auth_version=3, tenant_name="tenant_name",
-                 user="user",
-                 key='password', os_options=_os_options)
-
-node = SwiftService(auth=auth)
-```
-When accessing a SwiftService the node gives access to all the container of this service by giving a list of ContainerNode,
-and then each container gives a list of ObjectNode for each object in the container.
-
-## Limitations
-
-This implementation doesn't allow to write, modify, delete file on a swift container,
-or it doesn't allow to delete or upload a file.
-This implementation doesn't allow to download directly an all container.
-
-## Documentation
-
+# Swift Implementation
+This drb-driver-swift module implements Swift protocol access with DRB data model.
+
+## Swift Factory and Swift Node
+The module implements the factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
+
+The entry point group reference is `drb.driver.swift`.<br/>
+The implementation name is `swift`.<br/>
+The factory class is encoded into `drb.driver.swift`.<br/>
+The Swift signature id is  `86289118-7797-11ec-90d6-0242ac120003`<br/>
+
+
+## Using this module
+The project is present in https://www.pypi.org service. it can be freely 
+loaded into projects with the following command line:
+
+```commandline
+pip install drb-driver-swift
+```
+## Access Data
+`DrbSwiftNode` manages the swift protocol to access remote data. The construction
+parameter is an authentication object.
+
+```python
+from drb.drivers.swift import SwiftService, SwiftAuth
+
+_os_options = {
+    'user_domain_name': 'Default',
+    'project_domain_name': 'Default',
+    'project_name': 'project_name',
+    'project_id': 'project_id',
+    'tenant_name': 'tenant_name',
+    'tenant_id': 'tenant_id',
+    'region_name': 'region_name'
+}
+
+auth = SwiftAuth(authurl="https://your_auth_url/v3",
+                 auth_version=3, tenant_name="tenant_name",
+                 user="user",
+                 key='password', os_options=_os_options)
+
+node = SwiftService(auth=auth)
+```
+When accessing a SwiftService the node gives access to all the container of this service by giving a list of ContainerNode,
+and then each container gives a list of ObjectNode for each object in the container.
+
+## Limitations
+
+This implementation doesn't allow to write, modify, delete file on a swift container,
+or it doesn't allow to delete or upload a file.
+This implementation doesn't allow to download directly an all container.
+
+## Documentation
+
 The documentation of this implementation can be found here https://drb-python.gitlab.io/impl/swift
```

### Comparing `drb-driver-swift-1.1.0/drb/drivers/swift/swift.py` & `drb-driver-swift-1.2.0/drb/drivers/swift/swift.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,460 +1,408 @@
-import io
-import os
-from abc import ABC
-from typing import Optional, Any, List, Dict, Tuple
-import requests
-import secrets
-
-import swiftclient
-from drb.core import DrbNode, ParsedPath, DrbFactory
-from drb.drivers.http import DrbHttpNode
-from drb.exceptions.core import DrbException
-from drb.nodes.abstract_node import AbstractNode
-from requests.auth import HTTPBasicAuth
-
-
-from swiftclient.utils import generate_temp_url
-
-
-class SwiftAuth:
-    """
-    This class give us all the requirement to connect to a swift service.
-
-    Parameters:
-        authurl: authentication URL (default: None)
-        user: user name to authenticate as (default: None)
-        key: key/password to authenticate with (default: None)
-        retries: Number of times to retry the request before failing
-                 (default: 5)
-        preauthurl: storage URL (if you have already authenticated)
-                    (default: None)
-        preauthtoken: authentication token (if you have already
-                      authenticated) note authurl/user/key/tenant_name
-                      are not required when specifying preauthtoken
-                      (default: None)
-        snet: use SERVICENET internal network default is False (default: False)
-        starting_backoff: initial delay between retries
-                          (seconds) (default: 1)
-        max_backoff: maximum delay between retries
-        (seconds) (default: 64)
-        auth_version: OpenStack auth version (default: 1)
-        tenant_name: The tenant/account name, required when connecting
-                     to an auth 2.0 system (default: None).
-        os_options: The OpenStack options which can have tenant_id,
-                    auth_token, service_type, endpoint_type,
-                    tenant_name, object_storage_url, region_name,
-                    service_username, service_project_name,
-                    service_key (default: None).
-        insecure: Allow to access servers without checking SSL certs.
-                  The server's certificate will not be verified
-                  (default: False).
-        cert: Client certificate file to connect on SSL server
-              requiring SSL client certificate (default: None).
-        cert_key: Client certificate private key file (default: None).
-        ssl_compression: Whether to enable compression at the SSL layer.
-                         If set to 'False' and the pyOpenSSL library is
-                         present an attempt to disable SSL compression
-                         will be made. This may provide a performance
-                         increase for https upload/download operations
-                         (default: True).
-        retry_on_ratelimit: by default, a ratelimited connection will
-                            raise an exception to the caller. Setting
-                            this parameter to True will cause a retry
-                            after a backoff (default: False).
-        timeout: The connect timeout for the HTTP connection (default: None).
-        session: A keystoneauth session object (default: None).
-        force_auth_retry: reset auth info even if client got unexpected
-                          error except 401 Unauthorized (default: False).
-    """
-
-    def __init__(self, authurl=None, user=None,
-                 key=None, preauthurl=None,
-                 preauthtoken=None,
-                 os_options: Dict = None,
-                 auth_version="1",
-                 **kwargs):
-        if authurl is not None:
-            self.authurl = authurl.replace('+swift', '') \
-                if '+swift' in authurl else authurl
-        else:
-            self.authurl = None
-        self.user = user
-        self.key = key
-        self.preauthurl = preauthurl
-        self.preauthtoken = preauthtoken
-        self.os_options = os_options
-        self.auth_version = auth_version
-        self.retries = kwargs.get('retries', 5)
-        self.snet = kwargs.get('snet', False)
-        self.starting_backoff = kwargs.get('starting_backoff', 1)
-        self.max_backoff = kwargs.get('max_backoff', 64)
-        self.tenant_name = kwargs.get('tenant_name', None)
-        self.cacert = kwargs.get('cacert', None)
-        self.insecure = kwargs.get('insecure', False)
-        self.cert = kwargs.get('cert', None)
-        self.cert_key = kwargs.get('cert_key', None)
-        self.ssl_compression = kwargs.get('ssl_compression', True)
-        self.retry_on_ratelimit = kwargs.get('retry_on_ratelimit', False)
-        self.timeout = kwargs.get('timeout', None)
-        self.session = kwargs.get('session', None)
-        self.force_auth_retry = kwargs.get('force_auth_retry', False)
-
-
-class SwiftConnection:
-    """
-    This class use the singleton pattern to provide too
-    much connection to the swift server.
-
-    Parameters:
-        auth: An Auth object to provide all the information required
-              to establish the connection with the server.
-    """
-    swift = None
-
-    def __new__(cls,
-                auth: SwiftAuth):
-        if cls.swift is None:
-            cls.swift = swiftclient.client.Connection(
-                auth.authurl, auth.user,
-                auth.key, auth.retries,
-                auth.preauthurl,
-                auth.preauthtoken, auth.snet,
-                auth.starting_backoff,
-                auth.max_backoff, auth.tenant_name,
-                auth.os_options,
-                auth.auth_version, auth.cacert,
-                auth.insecure, auth.cert,
-                auth.cert_key,
-                auth.ssl_compression,
-                auth.retry_on_ratelimit,
-                auth.timeout, auth.session,
-                auth.force_auth_retry)
-        return cls.swift
-
-
-class Download(io.BytesIO):
-
-    def __init__(self, response: swiftclient.client._RetryBody):
-        self._resp = response
-        self._buff = bytearray(0)
-        super().__init__(self._buff)
-
-    def read(self, *args, **kwargs):
-        if isinstance(self._resp, bytes):
-            return self._resp
-        if not (len(args) > 0 and isinstance(
-                args[0], int) and args[0] > 0):
-            for chunk in self._resp:
-                self._buff.extend(chunk)
-
-            return self._buff
-        for chunk in self._resp:
-            self._buff.extend(chunk)
-            if len(self._buff) >= args[0]:
-                return self._buff
-
-    def close(self) -> None:
-        super().close()
-        self._resp.close()
-
-    def seekable(self) -> bool:
-        return False
-
-
-class SwiftNode(AbstractNode, ABC):
-    """
-    Common SwiftNode interface
-    """
-
-    def __init__(self, auth: SwiftAuth):
-        super(SwiftNode, self).__init__()
-        self._auth = auth
-        self._swift = None
-
-    def get_service_url(self) -> Optional[str]:
-        """
-        Returns URL of the swift auth service.
-
-        :returns: string URL representation the swift auth service
-        :rtype: str
-        """
-        return self._auth.authurl
-
-    def get_storage(self) -> Optional[str]:
-        """
-        Returns URL of the swift storage.
-
-        :returns: string URL representation the swift storage
-        :rtype: str
-        """
-        return self._auth.preauthurl
-
-    def get_auth(self) -> SwiftAuth:
-        """
-        Return the Auth object created to access the service.
-
-        :returns: an Auth object.
-        :rtype: SwiftAuth
-        """
-        return self._auth
-
-    def close(self) -> None:
-        """
-        Close The swift connection
-        """
-        if self._swift is not None:
-            self._swift.close()
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return None
-
-    @property
-    def value(self) -> Optional[Any]:
-        return None
-
-    def __eq__(self, other):
-        return isinstance(other, SwiftNode) and \
-               self._auth == other._auth
-
-    def __hash__(self):
-        return hash(self.auth)
-
-
-class SwiftObject(SwiftNode):
-
-    def __init__(self, path: str, obj: dict,
-                 auth: SwiftAuth, parent: SwiftNode):
-        super().__init__(auth)
-        self._auth = self.get_auth()
-        self._name = obj.get('name')
-        self._path = os.path.join(path, self._name)
-        self._attributes = obj
-        self._children = None
-        self._parent = parent
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        if namespace_uri is None:
-            try:
-                return self._attributes[name]
-            except KeyError:
-                pass
-        raise DrbException(f'No attribute found: ({name}, {namespace_uri})')
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def path(self) -> ParsedPath:
-        return ParsedPath(self._path)
-
-    @property
-    def children(self) -> List[DrbNode]:
-        return []
-
-    def has_impl(self, impl: type) -> bool:
-        return issubclass(io.BytesIO, impl)
-
-    """
-    These class allow the download of object in a container.
-
-    Parameters:
-        impl (type): The type supported by this implementation,
-                     here only subclass of io.BytesIO are supported.
-        chunk_size (int): The size of the chunk used during the download can
-                          be set here (default: 12000).
-        temp_url (Boolean): If using temp url set a secret key to download.
-    """
-
-    def get_impl(self, impl: type, **kwargs) -> Any:
-        self._swift = SwiftConnection(self._auth)
-
-        if self.has_impl(impl):
-            if kwargs.get('temp_url', False):
-                storage, token = self._swift.get_auth()
-                key = secrets.token_hex(nbytes=8)
-                # Set secret key to enable download
-                myobj = {
-                    'X-Account-Meta-Temp-URL-Key': key,
-                    'X-Auth-Token': token
-                }
-                requests.post(storage, headers=myobj)
-
-                storage_url = storage.split('v1')
-                total = '/v1' + storage_url[1] + '/' \
-                        + self.parent.name + '/' \
-                        + self.name
-                url = generate_temp_url(total, 3600,
-                                        key,
-                                        'GET')
-                node = DrbHttpNode(storage_url[0] + url[1:])
-
-                return node.get_impl(impl, resp_chunk_size=kwargs.get(
-                    'chunk_size', 12000))
-            else:
-                _, body = self._swift.get_object(container=self.parent.name,
-                                                 obj=self.name,
-                                                 resp_chunk_size=kwargs.get(
-                                                     'chunk_size', 12000))
-                return Download(body)
-
-        raise DrbException(f'Not supported implementation: {impl}')
-
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        return False
-
-
-class SwiftContainer(SwiftNode):
-
-    def __init__(self, obj: dict, auth: SwiftAuth, parent: SwiftNode):
-        super().__init__(auth)
-        self._auth = auth
-        self._name = obj.get('name')
-        self._path = os.path.join(parent.name, self._name)
-        self._attributes = obj
-        self._children = None
-        self._parent = parent
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        if namespace_uri is None:
-            try:
-                return self._attributes[name]
-            except KeyError:
-                pass
-        raise DrbException(f'No attribute found: ({name}, {namespace_uri})')
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def path(self) -> ParsedPath:
-        return ParsedPath(self._path)
-
-    @property
-    def children(self) -> List[DrbNode]:
-        self._swift = SwiftConnection(self._auth)
-        if self._children is None:
-            _, objects = self._swift.get_container(
-                self._name, full_listing=True)
-            self._children = [
-                SwiftObject(self._path, obj, self._auth, self)
-                for obj in objects]
-        return self._children
-
-    def has_impl(self, impl: type) -> bool:
-        return False
-
-    def get_impl(self, impl: type, **kwargs) -> Any:
-        raise DrbException(
-            f"SwiftService doesn't support {impl} implementation")
-
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        if namespace is None:
-            if name is not None:
-                return name in [x.name for x in self.children]
-            return len(self.children) > 0
-        return False
-
-
-class SwiftService(SwiftNode):
-
-    def __init__(self, auth: SwiftAuth):
-        super().__init__(auth)
-        self._auth = auth
-        self._attributes = {}
-        self._children = None
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        self._swift = SwiftConnection(self._auth)
-        self._attributes = self._swift.get_capabilities()
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        if self._attributes is {}:
-            self.attributes
-        if namespace_uri is None:
-            try:
-                return self._attributes[name]
-            except KeyError:
-                pass
-        raise DrbException(f'No attribute found: ({name}, {namespace_uri})')
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return None
-
-    @property
-    def path(self) -> ParsedPath:
-        return ParsedPath(os.path.sep)
-
-    @property
-    def children(self) -> List[DrbNode]:
-        self._swift = SwiftConnection(self._auth)
-        if self._children is None:
-            _, containers = self._swift.get_account()
-            self._children = [
-                SwiftContainer(container, self._auth, self)
-                for container in containers]
-        return self._children
-
-    @property
-    def name(self) -> str:
-        if self._auth.preauthurl:
-            return self._auth.preauthurl
-        return self._auth.authurl
-
-    def has_impl(self, impl: type) -> bool:
-        return False
-
-    def get_impl(self, impl: type, **kwargs) -> Any:
-        raise DrbException(
-            f"SwiftService doesn't support {impl} implementation")
-
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        if namespace is None:
-            if name is not None:
-                return name in [x.name for x in self.children]
-            return len(self.children) > 0
-        return False
-
-
-class SwiftNodeFactory(DrbFactory):
-    """ authurl=None, user=None,
-                 key=None, preauthurl=None,
-                 preauthtoken=None,
-                 os_options: Dict = None,
-                 auth_version="1",
-                 """
-
-    def _create(self, node: DrbNode) -> DrbNode:
-        if isinstance(node, SwiftNode):
-            return node
-        if isinstance(node, DrbHttpNode):
-            if isinstance(node.auth, HTTPBasicAuth):
-                auth = SwiftAuth(authurl=node.path.path,
-                                 user=node.auth.username,
-                                 key=node.auth.password
-                                 )
-            else:
-                auth = SwiftAuth(authurl=node.path.path)
-            return SwiftService(auth=auth)
-        raise NotImplementedError("Call impl method")
+from typing import Optional, Any, List, Dict, Tuple
+from pathlib import Path
+from abc import ABC
+from requests.auth import HTTPBasicAuth
+from swiftclient.utils import generate_temp_url
+from deprecated import deprecated
+from drb.core import DrbNode, ParsedPath, DrbFactory
+from drb.drivers.http import DrbHttpNode
+from drb.exceptions.core import DrbException
+from drb.nodes.abstract_node import AbstractNode
+import io
+import os
+import requests
+import secrets
+import swiftclient
+
+
+class SwiftAuth:
+    """
+    This class give us all the requirement to connect to a swift service.
+
+    Parameters:
+        authurl: authentication URL (default: None)
+        user: user name to authenticate as (default: None)
+        key: key/password to authenticate with (default: None)
+        retries: Number of times to retry the request before failing
+                 (default: 5)
+        preauthurl: storage URL (if you have already authenticated)
+                    (default: None)
+        preauthtoken: authentication token (if you have already
+                      authenticated) note authurl/user/key/tenant_name
+                      are not required when specifying preauthtoken
+                      (default: None)
+        snet: use SERVICENET internal network default is False (default: False)
+        starting_backoff: initial delay between retries
+                          (seconds) (default: 1)
+        max_backoff: maximum delay between retries
+        (seconds) (default: 64)
+        auth_version: OpenStack auth version (default: 1)
+        tenant_name: The tenant/account name, required when connecting
+                     to an auth 2.0 system (default: None).
+        os_options: The OpenStack options which can have tenant_id,
+                    auth_token, service_type, endpoint_type,
+                    tenant_name, object_storage_url, region_name,
+                    service_username, service_project_name,
+                    service_key (default: None).
+        insecure: Allow to access servers without checking SSL certs.
+                  The server's certificate will not be verified
+                  (default: False).
+        cert: Client certificate file to connect on SSL server
+              requiring SSL client certificate (default: None).
+        cert_key: Client certificate private key file (default: None).
+        ssl_compression: Whether to enable compression at the SSL layer.
+                         If set to 'False' and the pyOpenSSL library is
+                         present an attempt to disable SSL compression
+                         will be made. This may provide a performance
+                         increase for https upload/download operations
+                         (default: True).
+        retry_on_ratelimit: by default, a ratelimited connection will
+                            raise an exception to the caller. Setting
+                            this parameter to True will cause a retry
+                            after a backoff (default: False).
+        timeout: The connect timeout for the HTTP connection (default: None).
+        session: A keystoneauth session object (default: None).
+        force_auth_retry: reset auth info even if client got unexpected
+                          error except 401 Unauthorized (default: False).
+    """
+
+    def __init__(self, authurl=None, user=None,
+                 key=None, preauthurl=None,
+                 preauthtoken=None,
+                 os_options: Dict = None,
+                 auth_version="1",
+                 **kwargs):
+        if authurl is not None:
+            self.authurl = authurl.replace('+swift', '') \
+                if '+swift' in authurl else authurl
+        else:
+            self.authurl = None
+        self.user = user
+        self.key = key
+        self.preauthurl = preauthurl
+        self.preauthtoken = preauthtoken
+        self.os_options = os_options
+        self.auth_version = auth_version
+        self.retries = kwargs.get('retries', 5)
+        self.snet = kwargs.get('snet', False)
+        self.starting_backoff = kwargs.get('starting_backoff', 1)
+        self.max_backoff = kwargs.get('max_backoff', 64)
+        self.tenant_name = kwargs.get('tenant_name', None)
+        self.cacert = kwargs.get('cacert', None)
+        self.insecure = kwargs.get('insecure', False)
+        self.cert = kwargs.get('cert', None)
+        self.cert_key = kwargs.get('cert_key', None)
+        self.ssl_compression = kwargs.get('ssl_compression', True)
+        self.retry_on_ratelimit = kwargs.get('retry_on_ratelimit', False)
+        self.timeout = kwargs.get('timeout', None)
+        self.session = kwargs.get('session', None)
+        self.force_auth_retry = kwargs.get('force_auth_retry', False)
+
+
+class SwiftConnection:
+    """
+    This class use the singleton pattern to provide too
+    much connection to the swift server.
+
+    Parameters:
+        auth: An Auth object to provide all the information required
+              to establish the connection with the server.
+    """
+    swift = None
+
+    def __new__(cls,
+                auth: SwiftAuth):
+        if cls.swift is None:
+            cls.swift = swiftclient.client.Connection(
+                auth.authurl, auth.user,
+                auth.key, auth.retries,
+                auth.preauthurl,
+                auth.preauthtoken, auth.snet,
+                auth.starting_backoff,
+                auth.max_backoff, auth.tenant_name,
+                auth.os_options,
+                auth.auth_version, auth.cacert,
+                auth.insecure, auth.cert,
+                auth.cert_key,
+                auth.ssl_compression,
+                auth.retry_on_ratelimit,
+                auth.timeout, auth.session,
+                auth.force_auth_retry)
+        return cls.swift
+
+
+class Download(io.BytesIO):
+
+    def __init__(self, response: swiftclient.client._RetryBody):
+        self._resp = response
+        self._buff = bytearray(0)
+        super().__init__(self._buff)
+
+    def read(self, *args, **kwargs):
+        if isinstance(self._resp, bytes):
+            return self._resp
+        if not (len(args) > 0 and isinstance(
+                args[0], int) and args[0] > 0):
+            for chunk in self._resp:
+                self._buff.extend(chunk)
+
+            return self._buff
+        for chunk in self._resp:
+            self._buff.extend(chunk)
+            if len(self._buff) >= args[0]:
+                return self._buff
+
+    def close(self) -> None:
+        super().close()
+        self._resp.close()
+
+    def seekable(self) -> bool:
+        return False
+
+
+class SwiftNode(AbstractNode, ABC):
+    """
+    Common SwiftNode interface
+    """
+
+    def __init__(self, auth: SwiftAuth):
+        super().__init__()
+        self._auth = auth
+        self._swift = None
+
+    def get_service_url(self) -> Optional[str]:
+        """
+        Returns URL of the swift auth service.
+
+        :returns: string URL representation the swift auth service
+        :rtype: str
+        """
+        return self._auth.authurl
+
+    def get_storage(self) -> Optional[str]:
+        """
+        Returns URL of the swift storage.
+
+        :returns: string URL representation the swift storage
+        :rtype: str
+        """
+        return self._auth.preauthurl
+
+    def get_auth(self) -> SwiftAuth:
+        """
+        Return the Auth object created to access the service.
+
+        :returns: an Auth object.
+        :rtype: SwiftAuth
+        """
+        return self._auth
+
+    def close(self) -> None:
+        """
+        Close The swift connection
+        """
+        if self._swift is not None:
+            self._swift.close()
+
+    def __eq__(self, other):
+        return isinstance(other, SwiftNode) and \
+               self._auth == other._auth
+
+    def __hash__(self):
+        return hash(self.auth)
+
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, key):
+        raise NotImplementedError
+
+
+class SwiftObject(SwiftNode):
+
+    def __init__(self, path: str, obj: dict,
+                 auth: SwiftAuth, parent: SwiftNode):
+        super().__init__(auth)
+        self._available_impl.append(io.BytesIO)
+        self.name = obj.get('name')
+        if path.endswith("/"):
+            self._path = path + self.name
+        else:
+            self._path = path + "/" + self.name
+        for k, v in obj.items():
+            self @= (k, v)
+        self.parent = parent
+
+    @property
+    def path(self) -> ParsedPath:
+        return ParsedPath(self._path)
+
+    @property
+    @deprecated(version='1.2.0')
+    def children(self) -> List[DrbNode]:
+        return []
+
+    def get_impl(self, impl: type, **kwargs) -> Any:
+        """
+        These class allow the download of object in a container.
+
+        Parameters:
+            impl (type): The type supported by this implementation,
+                         here only subclass of io.BytesIO are supported.
+        Keywords Parameters:
+            chunk_size (int): The size of the chunk used during the download
+                              can be set here (default: 12000).
+            temp_url (Boolean): If using temp url set a secret key to download.
+        """
+        self._swift = SwiftConnection(self._auth)
+
+        if self.has_impl(impl):
+            if kwargs.get('temp_url', False):
+                storage, token = self._swift.get_auth()
+                key = secrets.token_hex(nbytes=8)
+                # Set secret key to enable download
+                myobj = {
+                    'X-Account-Meta-Temp-URL-Key': key,
+                    'X-Auth-Token': token
+                }
+                requests.post(storage, headers=myobj)
+
+                storage_url = storage.split('v1')
+                total = '/v1' + storage_url[1] + '/' \
+                        + self.parent.name + '/' \
+                        + self.name
+                url = generate_temp_url(total, 3600,
+                                        key,
+                                        'GET')
+                node = DrbHttpNode(storage_url[0] + url[1:])
+
+                return node.get_impl(impl, resp_chunk_size=kwargs.get(
+                    'chunk_size', 12000))
+            else:
+                _, body = self._swift.get_object(container=self.parent.name,
+                                                 obj=self.name,
+                                                 resp_chunk_size=kwargs.get(
+                                                     'chunk_size', 12000))
+                return Download(body)
+
+        raise DrbException(f'Not supported implementation: {impl}')
+
+
+class SwiftContainer(SwiftNode):
+
+    def __init__(self, obj: dict, auth: SwiftAuth, parent: SwiftNode):
+        super().__init__(auth)
+        self._available_impl.clear()
+        self.name = obj.get('name')
+        if parent.name.endswith("/"):
+            self._path = parent.name + self.name
+        else:
+            self._path = parent.name + "/" + self.name
+        for k, v in obj.items():
+            self @= (k, v)
+        self._children = None
+        self.parent = parent
+
+    @property
+    def path(self) -> ParsedPath:
+        return ParsedPath(self._path)
+
+    @property
+    @deprecated(version='1.2.0')
+    def children(self) -> List[DrbNode]:
+        self._swift = SwiftConnection(self._auth)
+        if self._children is None:
+            _, objects = self._swift.get_container(self.name,
+                                                   full_listing=True)
+            self._children = [
+                SwiftObject(self._path, obj, self._auth, self)
+                for obj in objects
+            ]
+        return self._children
+
+    def get_impl(self, impl: type, **kwargs) -> Any:
+        raise DrbException(
+            f"SwiftContainer doesn't support {impl} implementation")
+
+    # def has_child(self, name: str = None, namespace: str = None) -> bool:
+    #     if namespace is None:
+    #         if name is not None:
+    #             return name in [x.name for x in self.children]
+    #         return len(self.children) > 0
+    #     return False
+
+
+class SwiftService(SwiftNode):
+
+    def __init__(self, auth: SwiftAuth):
+        super().__init__(auth)
+        self._available_impl.clear()
+        self._children = None
+
+    @property
+    @deprecated(version='1.2.0')
+    def attributes(self) -> Dict[Tuple[str, str], Any]:
+        if not self._attrs:
+            self._swift = SwiftConnection(self._auth)
+            for k, v in self._swift.get_capabilities().items():
+                self @= (k, v)
+        return super().attributes
+
+    @property
+    def parent(self) -> Optional[DrbNode]:
+        return None
+
+    @property
+    def path(self) -> ParsedPath:
+        return ParsedPath(Path(os.path.sep).as_posix())
+
+    @property
+    @deprecated(version='1.2.0')
+    def children(self) -> List[DrbNode]:
+        self._swift = SwiftConnection(self._auth)
+        if self._children is None:
+            _, containers = self._swift.get_account()
+            self._children = [
+                SwiftContainer(container, self._auth, self)
+                for container in containers]
+        return self._children
+
+    @property
+    def name(self) -> str:
+        if self._auth.preauthurl:
+            return self._auth.preauthurl
+        return self._auth.authurl
+
+    def get_impl(self, impl: type, **kwargs) -> Any:
+        raise DrbException(
+            f"SwiftService doesn't support {impl} implementation")
+
+    # def has_child(self, name: str = None, namespace: str = None) -> bool:
+    #     if namespace is None:
+    #         if name is not None:
+    #             return name in [x.name for x in self.children]
+    #         return len(self.children) > 0
+    #     return False
+
+
+class SwiftNodeFactory(DrbFactory):
+    """ authurl=None, user=None,
+                 key=None, preauthurl=None,
+                 preauthtoken=None,
+                 os_options: Dict = None,
+                 auth_version="1",
+                 """
+
+    def _create(self, node: DrbNode) -> DrbNode:
+        if isinstance(node, SwiftNode):
+            return node
+        if isinstance(node, DrbHttpNode):
+            if isinstance(node.auth, HTTPBasicAuth):
+                auth = SwiftAuth(authurl=node.path.path,
+                                 user=node.auth.username,
+                                 key=node.auth.password
+                                 )
+            else:
+                auth = SwiftAuth(authurl=node.path.path)
+            return SwiftService(auth=auth)
+        raise NotImplementedError("Call impl method")
```

### Comparing `drb-driver-swift-1.1.0/drb_driver_swift.egg-info/PKG-INFO` & `drb-driver-swift-1.2.0/drb_driver_swift.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: drb-driver-swift
-Version: 1.1.0
-Summary: DRB Swift driver
+Version: 1.2.0
+Summary: DRB OpenStack Swift driver
 Home-page: https://gitlab.com/drb-python/impl/swift
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/swift/
+License: LGPLv3
+Project-URL: Documentation, https://drb-python.gitlab.io/drb-python/impl/swift
 Project-URL: Source, https://gitlab.com/drb-python/impl/swift
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # Swift Implementation
 This drb-driver-swift module implements Swift protocol access with DRB data model.
 
 ## Swift Factory and Swift Node
 The module implements the factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -66,8 +67,7 @@
 This implementation doesn't allow to write, modify, delete file on a swift container,
 or it doesn't allow to delete or upload a file.
 This implementation doesn't allow to download directly an all container.
 
 ## Documentation
 
 The documentation of this implementation can be found here https://drb-python.gitlab.io/impl/swift
-
```

### Comparing `drb-driver-swift-1.1.0/versioneer.py` & `drb-driver-swift-1.2.0/versioneer.py`

 * *Files identical despite different names*

