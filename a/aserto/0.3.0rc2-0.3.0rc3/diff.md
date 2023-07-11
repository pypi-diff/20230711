# Comparing `tmp/aserto-0.3.0rc2.tar.gz` & `tmp/aserto-0.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aserto-0.3.0rc2.tar", max compression
+gzip compressed data, was "aserto-0.3.0rc3.tar", max compression
```

## Comparing `aserto-0.3.0rc2.tar` & `aserto-0.3.0rc3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      980 2022-10-19 21:06:37.819303 aserto-0.3.0rc2/README.md
--rw-r--r--   0        0        0     2124 2022-10-20 20:38:10.802829 aserto-0.3.0rc2/pyproject.toml
--rw-r--r--   0        0        0      195 2022-10-19 21:09:24.325260 aserto-0.3.0rc2/src/aserto/client/__init__.py
--rw-r--r--   0        0        0      412 2022-02-03 23:43:06.663101 aserto-0.3.0rc2/src/aserto/client/_deadline.py
--rw-r--r--   0        0        0      177 2022-02-03 23:43:06.663211 aserto-0.3.0rc2/src/aserto/client/_typing.py
--rw-r--r--   0        0        0        0 2022-02-03 23:43:06.663305 aserto-0.3.0rc2/src/aserto/client/api/__init__.py
--rw-r--r--   0        0        0     2629 2022-10-20 14:51:28.760249 aserto-0.3.0rc2/src/aserto/client/api/authorizer/__init__.py
--rw-r--r--   0        0        0     1183 2022-10-20 14:48:14.499898 aserto-0.3.0rc2/src/aserto/client/api/authorizer/_protocol.py
--rw-r--r--   0        0        0     8387 2022-10-20 20:33:47.957354 aserto-0.3.0rc2/src/aserto/client/api/authorizer/grpc.py
--rw-r--r--   0        0        0     7758 2022-10-20 15:02:52.608824 aserto-0.3.0rc2/src/aserto/client/api/authorizer/rest.py
--rw-r--r--   0        0        0     2129 2022-02-03 23:43:06.664100 aserto-0.3.0rc2/src/aserto/client/identity.py
--rw-r--r--   0        0        0     1984 2022-10-19 21:05:31.224922 aserto-0.3.0rc2/src/aserto/client/options.py
--rw-r--r--   0        0        0        0 2022-02-03 23:43:06.664143 aserto-0.3.0rc2/src/aserto/client/py.typed
--rw-r--r--   0        0        0      143 2022-02-03 23:43:06.664288 aserto-0.3.0rc2/src/aserto/client/resource_context.py
--rw-r--r--   0        0        0     1964 2022-10-20 20:39:04.559583 aserto-0.3.0rc2/setup.py
--rw-r--r--   0        0        0     2337 2022-10-20 20:39:04.559868 aserto-0.3.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      989 2022-10-20 20:47:21.801751 aserto-0.3.0rc3/README.md
+-rw-r--r--   0        0        0     2124 2022-10-20 21:15:03.857052 aserto-0.3.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      195 2022-10-19 21:09:24.325260 aserto-0.3.0rc3/src/aserto/client/__init__.py
+-rw-r--r--   0        0        0      412 2022-02-03 23:43:06.663101 aserto-0.3.0rc3/src/aserto/client/_deadline.py
+-rw-r--r--   0        0        0      177 2022-02-03 23:43:06.663211 aserto-0.3.0rc3/src/aserto/client/_typing.py
+-rw-r--r--   0        0        0        0 2022-02-03 23:43:06.663305 aserto-0.3.0rc3/src/aserto/client/api/__init__.py
+-rw-r--r--   0        0        0     2629 2022-10-20 14:51:28.760249 aserto-0.3.0rc3/src/aserto/client/api/authorizer/__init__.py
+-rw-r--r--   0        0        0     1183 2022-10-20 14:48:14.499898 aserto-0.3.0rc3/src/aserto/client/api/authorizer/_protocol.py
+-rw-r--r--   0        0        0     8387 2022-10-20 21:14:30.020110 aserto-0.3.0rc3/src/aserto/client/api/authorizer/grpc.py
+-rw-r--r--   0        0        0     7758 2022-10-20 15:02:52.608824 aserto-0.3.0rc3/src/aserto/client/api/authorizer/rest.py
+-rw-r--r--   0        0        0     2129 2022-02-03 23:43:06.664100 aserto-0.3.0rc3/src/aserto/client/identity.py
+-rw-r--r--   0        0        0     1984 2022-10-19 21:05:31.224922 aserto-0.3.0rc3/src/aserto/client/options.py
+-rw-r--r--   0        0        0        0 2022-02-03 23:43:06.664143 aserto-0.3.0rc3/src/aserto/client/py.typed
+-rw-r--r--   0        0        0      143 2022-02-03 23:43:06.664288 aserto-0.3.0rc3/src/aserto/client/resource_context.py
+-rw-r--r--   0        0        0     1973 2022-10-20 21:15:09.675435 aserto-0.3.0rc3/setup.py
+-rw-r--r--   0        0        0     2346 2022-10-20 21:15:09.675737 aserto-0.3.0rc3/PKG-INFO
```

### Comparing `aserto-0.3.0rc2/README.md` & `aserto-0.3.0rc3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         tenant_id=ASERTO_TENANT_ID,
         service_type="gRPC",
     ),
 )
 
 result = await client.decision_tree(
     decisions=["visible", "enabled", "allowed"],
-    policy_name=ASERTO_POLICY_NAME,
+    policy_instance_name=ASERTO_POLICY_NAME,
     policy_path_root=ASERTO_POLICY_PATH_ROOT,
     policy_path_separator="DOT",
 )
 
 assert result == {
     "GET.your.policy.path": {
         "visible": True,
```

### Comparing `aserto-0.3.0rc2/pyproject.toml` & `aserto-0.3.0rc3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aserto"
-version = "0.3.0.rc2"
+version = "0.3.0.rc3"
 description = "Aserto API client"
 readme = "README.md"
 authors = ["Aserto, Inc. <pypi@aserto.com>"]
 maintainers = ["authereal <authereal@aserto.com>"]
 homepage = "https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/aserto"
 repository = "https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/aserto"
 documentation = "https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/aserto"
```

### Comparing `aserto-0.3.0rc2/src/aserto/client/api/authorizer/__init__.py` & `aserto-0.3.0rc3/src/aserto/client/api/authorizer/__init__.py`

 * *Files identical despite different names*

### Comparing `aserto-0.3.0rc2/src/aserto/client/api/authorizer/_protocol.py` & `aserto-0.3.0rc3/src/aserto/client/api/authorizer/_protocol.py`

 * *Files identical despite different names*

### Comparing `aserto-0.3.0rc2/src/aserto/client/api/authorizer/grpc.py` & `aserto-0.3.0rc3/src/aserto/client/api/authorizer/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         return decision_tree
 
     async def decisions(
         self,
         *,
         policy_path: str,
         decisions: Collection[str],
-        policy_insatnce_name: Optional[str],
+        policy_instance_name: Optional[str],
         policy_instance_label: Optional[str] = None,
         resource_context: Optional[ResourceContext] = None,
         deadline: Optional[Union[datetime, timedelta]] = None,
     ) -> Dict[str, bool]:
         try:
             async with self._authorizer_client(deadline=deadline) as client:
                 response = await client.Is(
@@ -189,15 +189,15 @@
                         policy_context=PolicyContext(
                             path=policy_path,
                             decisions=list(decisions),
                         ),
                         identity_context=self._identity_context_field,
                         resource_context=self._serialize_resource_context(resource_context or {}),
                         policy_instance=PolicyInstance(
-                            name=policy_insatnce_name,
+                            name=policy_instance_name,
                             instance_label=policy_instance_label,
                         ),
                     ),
                     metadata=self._metadata,
                     timeout=(monotonic_time_from_deadline(deadline) if deadline is not None else None),
                 )
         except (OSError, grpc.RpcError) as error:
```

### Comparing `aserto-0.3.0rc2/src/aserto/client/api/authorizer/rest.py` & `aserto-0.3.0rc3/src/aserto/client/api/authorizer/rest.py`

 * *Files identical despite different names*

### Comparing `aserto-0.3.0rc2/src/aserto/client/identity.py` & `aserto-0.3.0rc3/src/aserto/client/identity.py`

 * *Files identical despite different names*

### Comparing `aserto-0.3.0rc2/src/aserto/client/options.py` & `aserto-0.3.0rc3/src/aserto/client/options.py`

 * *Files identical despite different names*

### Comparing `aserto-0.3.0rc2/setup.py` & `aserto-0.3.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'aserto-authorizer==0.0.4',
  'grpcio>=1.49.1,<2.0.0',
  'protobuf>=4.21.7,<5.0.0',
  'typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'aserto',
-    'version': '0.3.0rc2',
+    'version': '0.3.0rc3',
     'description': 'Aserto API client',
-    'long_description': '# Aserto API client\nHigh-level client interface to Aserto\'s APIs.\n\nAt the moment this only supports interacting with Aserto\'s [Authorizer service](https://docs.aserto.com/docs/authorizer-guide/overview).\n## Installation\n### Using Pip\n```sh\npip install aserto\n```\n### Using Poetry\n```sh\npoetry add aserto\n```\n## Usage\n```py\nfrom aserto.client import AuthorizerOptions, Identity\nfrom aserto.client.api.authorizer import AuthorizerClient\n\n\nclient = AuthorizerClient(\n    identity=Identity(type="NONE"),\n    options=AuthorizerOptions(\n        api_key=ASERTO_API_KEY,\n        tenant_id=ASERTO_TENANT_ID,\n        service_type="gRPC",\n    ),\n)\n\nresult = await client.decision_tree(\n    decisions=["visible", "enabled", "allowed"],\n    policy_name=ASERTO_POLICY_NAME,\n    policy_path_root=ASERTO_POLICY_PATH_ROOT,\n    policy_path_separator="DOT",\n)\n\nassert result == {\n    "GET.your.policy.path": {\n        "visible": True,\n        "enabled": True,\n        "allowed": False,\n    },\n}\n```\n',
+    'long_description': '# Aserto API client\nHigh-level client interface to Aserto\'s APIs.\n\nAt the moment this only supports interacting with Aserto\'s [Authorizer service](https://docs.aserto.com/docs/authorizer-guide/overview).\n## Installation\n### Using Pip\n```sh\npip install aserto\n```\n### Using Poetry\n```sh\npoetry add aserto\n```\n## Usage\n```py\nfrom aserto.client import AuthorizerOptions, Identity\nfrom aserto.client.api.authorizer import AuthorizerClient\n\n\nclient = AuthorizerClient(\n    identity=Identity(type="NONE"),\n    options=AuthorizerOptions(\n        api_key=ASERTO_API_KEY,\n        tenant_id=ASERTO_TENANT_ID,\n        service_type="gRPC",\n    ),\n)\n\nresult = await client.decision_tree(\n    decisions=["visible", "enabled", "allowed"],\n    policy_instance_name=ASERTO_POLICY_NAME,\n    policy_path_root=ASERTO_POLICY_PATH_ROOT,\n    policy_path_separator="DOT",\n)\n\nassert result == {\n    "GET.your.policy.path": {\n        "visible": True,\n        "enabled": True,\n        "allowed": False,\n    },\n}\n```\n',
     'author': 'Aserto, Inc.',
     'author_email': 'pypi@aserto.com',
     'maintainer': 'authereal',
     'maintainer_email': 'authereal@aserto.com',
     'url': 'https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/aserto',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `aserto-0.3.0rc2/PKG-INFO` & `aserto-0.3.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aserto
-Version: 0.3.0rc2
+Version: 0.3.0rc3
 Summary: Aserto API client
 Home-page: https://github.com/aserto-dev/aserto-python/tree/HEAD/packages/aserto
 License: Apache-2.0
 Author: Aserto, Inc.
 Author-email: pypi@aserto.com
 Maintainer: authereal
 Maintainer-email: authereal@aserto.com
@@ -56,15 +56,15 @@
         tenant_id=ASERTO_TENANT_ID,
         service_type="gRPC",
     ),
 )
 
 result = await client.decision_tree(
     decisions=["visible", "enabled", "allowed"],
-    policy_name=ASERTO_POLICY_NAME,
+    policy_instance_name=ASERTO_POLICY_NAME,
     policy_path_root=ASERTO_POLICY_PATH_ROOT,
     policy_path_separator="DOT",
 )
 
 assert result == {
     "GET.your.policy.path": {
         "visible": True,
```

